# Comparing `tmp/totolo-1.5.2.tar.gz` & `tmp/totolo-1.5.2.dev202404281659.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totolo-1.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "totolo-1.5.2.dev202404281659.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `totolo-1.5.2.tar` & `totolo-1.5.2.dev202404281659.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0      834 2024-04-28 16:58:04.255380 totolo-1.5.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2024-04-28 16:58:04.255380 totolo-1.5.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1096 2024-04-28 16:58:04.255380 totolo-1.5.2/.github/workflows/coverage-branch.yaml
--rw-r--r--   0        0        0     1106 2024-04-28 16:58:04.259380 totolo-1.5.2/.github/workflows/coverage.yaml
--rw-r--r--   0        0        0     5091 2024-04-28 16:58:04.259380 totolo-1.5.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      825 2024-04-28 16:58:04.259380 totolo-1.5.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0     3088 2024-04-28 16:58:04.259380 totolo-1.5.2/.gitignore
--rw-r--r--   0        0        0     1550 2024-04-28 16:58:04.259380 totolo-1.5.2/.vscode/launch.json
--rw-r--r--   0        0        0      277 2024-04-28 16:58:04.259380 totolo-1.5.2/.vscode/settings.json
--rw-r--r--   0        0        0     1071 2024-04-28 16:58:04.259380 totolo-1.5.2/LICENSE
--rw-r--r--   0        0        0     4126 2024-04-28 16:58:04.259380 totolo-1.5.2/README.md
--rw-r--r--   0        0        0     1104 2024-04-28 16:58:04.259380 totolo-1.5.2/examples/basics.py
--rw-r--r--   0        0        0     1663 2024-04-28 16:58:04.259380 totolo-1.5.2/pyproject.toml
--rw-r--r--   0        0        0       60 2024-04-28 16:58:04.259380 totolo-1.5.2/requirements-dev.txt
--rw-r--r--   0        0        0        0 2024-04-28 16:58:04.259380 totolo-1.5.2/tests/__init__.py
--rw-r--r--   0        0        0       24 2024-04-28 16:58:04.259380 totolo-1.5.2/tests/data/cycles1.th.txt
--rw-r--r--   0        0        0       47 2024-04-28 16:58:04.259380 totolo-1.5.2/tests/data/cycles2.th.txt
--rw-r--r--   0        0        0       71 2024-04-28 16:58:04.259380 totolo-1.5.2/tests/data/cycles3.th.txt
--rw-r--r--   0        0        0   173716 2024-04-28 16:58:04.259380 totolo-1.5.2/tests/data/film-timeout-top100.st.txt
--rw-r--r--   0        0        0   332534 2024-04-28 16:58:04.259380 totolo-1.5.2/tests/data/flat.tar.gz
--rw-r--r--   0        0        0      166 2024-04-28 16:58:04.259380 totolo-1.5.2/tests/data/messy.st.txt
--rw-r--r--   0        0        0   332557 2024-04-28 16:58:04.259380 totolo-1.5.2/tests/data/sample-2023.07.23.tar.gz
--rw-r--r--   0        0        0    34632 2024-04-28 16:58:04.259380 totolo-1.5.2/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt
--rw-r--r--   0        0        0    28050 2024-04-28 16:58:04.259380 totolo-1.5.2/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt
--rw-r--r--   0        0        0    48760 2024-04-28 16:58:04.263380 totolo-1.5.2/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt
--rw-r--r--   0        0        0  1011578 2024-04-28 16:58:04.267380 totolo-1.5.2/tests/data/sample-2023.07.23/notes/themes/primary.th.txt
--rw-r--r--   0        0        0    14882 2024-04-28 16:58:04.267380 totolo-1.5.2/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt
--rwxr-xr-x   0        0        0    10486 2024-04-28 16:58:04.267380 totolo-1.5.2/tests/data/scifi1920-mergelist.xlsx
--rw-r--r--   0        0        0      428 2024-04-28 16:58:04.267380 totolo-1.5.2/tests/data/storytree.st.txt
--rw-r--r--   0        0        0  1011579 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/data/to-2023.07.09.th.txt
--rw-r--r--   0        0        0     2365 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/data/to-sample-2023.07.09-copy.st.txt
--rw-r--r--   0        0        0     2365 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/data/to-sample-2023.07.09.st.txt
--rw-r--r--   0        0        0        0 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/lib/__init__.py
--rw-r--r--   0        0        0      745 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/lib/test_excel.py
--rw-r--r--   0        0        0      800 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/lib/test_files.py
--rw-r--r--   0        0        0      794 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/lib/test_logging.py
--rw-r--r--   0        0        0     1419 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/lib/test_textformat.py
--rw-r--r--   0        0        0     6170 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/test_entries.py
--rw-r--r--   0        0        0     6158 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/test_impl.py
--rw-r--r--   0        0        0     1909 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/test_toset.py
--rw-r--r--   0        0        0    15084 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/test_totolo.py
--rw-r--r--   0        0        0        0 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/utils/__init__.py
--rw-r--r--   0        0        0     1968 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/utils/test_mergefiles.py
--rw-r--r--   0        0        0     3191 2024-04-28 16:58:04.271380 totolo-1.5.2/tests/utils/test_mergelist.py
--rw-r--r--   0        0        0      191 2024-04-28 16:58:04.271380 totolo-1.5.2/totolo/__init__.py
--rw-r--r--   0        0        0     1201 2024-04-28 16:58:04.271380 totolo-1.5.2/totolo/api.py
--rw-r--r--   0        0        0     1893 2024-04-28 16:58:04.271380 totolo-1.5.2/totolo/collection.py
--rw-r--r--   0        0        0        0 2024-04-28 16:58:04.271380 totolo-1.5.2/totolo/impl/__init__.py
--rw-r--r--   0        0        0     3367 2024-04-28 16:58:04.271380 totolo-1.5.2/totolo/impl/core.py
--rw-r--r--   0        0        0     6525 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/impl/entry.py
--rw-r--r--   0        0        0     4595 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/impl/field.py
--rw-r--r--   0        0        0      666 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/impl/keyword.py
--rw-r--r--   0        0        0     8111 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/impl/parser.py
--rw-r--r--   0        0        0        0 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/lib/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/lib/excel.py
--rw-r--r--   0        0        0     1134 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/lib/files.py
--rw-r--r--   0        0        0      248 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/lib/log.py
--rw-r--r--   0        0        0     1283 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/lib/textformat.py
--rw-r--r--   0        0        0     3605 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/story.py
--rw-r--r--   0        0        0     2395 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/theme.py
--rw-r--r--   0        0        0    11866 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/themeontology.py
--rw-r--r--   0        0        0        0 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/util/__init__.py
--rw-r--r--   0        0        0     2221 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/util/mergefiles.py
--rw-r--r--   0        0        0     7321 2024-04-28 16:58:04.275380 totolo-1.5.2/totolo/util/mergelist.py
--rw-r--r--   0        0        0     4560 1970-01-01 00:00:00.000000 totolo-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0      834 2024-04-28 16:58:04.231597 totolo-1.5.2.dev202404281659/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2024-04-28 16:58:04.231597 totolo-1.5.2.dev202404281659/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1096 2024-04-28 16:58:04.231597 totolo-1.5.2.dev202404281659/.github/workflows/coverage-branch.yaml
+-rw-r--r--   0        0        0     1106 2024-04-28 16:58:04.231597 totolo-1.5.2.dev202404281659/.github/workflows/coverage.yaml
+-rw-r--r--   0        0        0     5091 2024-04-28 16:58:04.231597 totolo-1.5.2.dev202404281659/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      825 2024-04-28 16:58:04.231597 totolo-1.5.2.dev202404281659/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     3088 2024-04-28 16:58:04.231597 totolo-1.5.2.dev202404281659/.gitignore
+-rw-r--r--   0        0        0     1550 2024-04-28 16:58:04.231597 totolo-1.5.2.dev202404281659/.vscode/launch.json
+-rw-r--r--   0        0        0      277 2024-04-28 16:58:04.231597 totolo-1.5.2.dev202404281659/.vscode/settings.json
+-rw-r--r--   0        0        0     1071 2024-04-28 16:58:04.231597 totolo-1.5.2.dev202404281659/LICENSE
+-rw-r--r--   0        0        0     4126 2024-04-28 16:58:04.231597 totolo-1.5.2.dev202404281659/README.md
+-rw-r--r--   0        0        0     1104 2024-04-28 16:58:04.231597 totolo-1.5.2.dev202404281659/examples/basics.py
+-rw-r--r--   0        0        0     1663 2024-04-28 16:58:04.231597 totolo-1.5.2.dev202404281659/pyproject.toml
+-rw-r--r--   0        0        0       60 2024-04-28 16:58:04.235597 totolo-1.5.2.dev202404281659/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2024-04-28 16:58:04.235597 totolo-1.5.2.dev202404281659/tests/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-28 16:58:04.235597 totolo-1.5.2.dev202404281659/tests/data/cycles1.th.txt
+-rw-r--r--   0        0        0       47 2024-04-28 16:58:04.235597 totolo-1.5.2.dev202404281659/tests/data/cycles2.th.txt
+-rw-r--r--   0        0        0       71 2024-04-28 16:58:04.235597 totolo-1.5.2.dev202404281659/tests/data/cycles3.th.txt
+-rw-r--r--   0        0        0   173716 2024-04-28 16:58:04.235597 totolo-1.5.2.dev202404281659/tests/data/film-timeout-top100.st.txt
+-rw-r--r--   0        0        0   332534 2024-04-28 16:58:04.235597 totolo-1.5.2.dev202404281659/tests/data/flat.tar.gz
+-rw-r--r--   0        0        0      166 2024-04-28 16:58:04.235597 totolo-1.5.2.dev202404281659/tests/data/messy.st.txt
+-rw-r--r--   0        0        0   332557 2024-04-28 16:58:04.235597 totolo-1.5.2.dev202404281659/tests/data/sample-2023.07.23.tar.gz
+-rw-r--r--   0        0        0    34632 2024-04-28 16:58:04.235597 totolo-1.5.2.dev202404281659/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt
+-rw-r--r--   0        0        0    28050 2024-04-28 16:58:04.235597 totolo-1.5.2.dev202404281659/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt
+-rw-r--r--   0        0        0    48760 2024-04-28 16:58:04.235597 totolo-1.5.2.dev202404281659/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt
+-rw-r--r--   0        0        0  1011578 2024-04-28 16:58:04.243597 totolo-1.5.2.dev202404281659/tests/data/sample-2023.07.23/notes/themes/primary.th.txt
+-rw-r--r--   0        0        0    14882 2024-04-28 16:58:04.243597 totolo-1.5.2.dev202404281659/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt
+-rwxr-xr-x   0        0        0    10486 2024-04-28 16:58:04.243597 totolo-1.5.2.dev202404281659/tests/data/scifi1920-mergelist.xlsx
+-rw-r--r--   0        0        0      428 2024-04-28 16:58:04.243597 totolo-1.5.2.dev202404281659/tests/data/storytree.st.txt
+-rw-r--r--   0        0        0  1011579 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/data/to-2023.07.09.th.txt
+-rw-r--r--   0        0        0     2365 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/data/to-sample-2023.07.09-copy.st.txt
+-rw-r--r--   0        0        0     2365 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/data/to-sample-2023.07.09.st.txt
+-rw-r--r--   0        0        0        0 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/lib/__init__.py
+-rw-r--r--   0        0        0      745 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/lib/test_excel.py
+-rw-r--r--   0        0        0      800 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/lib/test_files.py
+-rw-r--r--   0        0        0      794 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/lib/test_logging.py
+-rw-r--r--   0        0        0     1419 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/lib/test_textformat.py
+-rw-r--r--   0        0        0     6170 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/test_entries.py
+-rw-r--r--   0        0        0     6158 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/test_impl.py
+-rw-r--r--   0        0        0     1909 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/test_toset.py
+-rw-r--r--   0        0        0    15084 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/test_totolo.py
+-rw-r--r--   0        0        0        0 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1968 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/utils/test_mergefiles.py
+-rw-r--r--   0        0        0     3191 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/tests/utils/test_mergelist.py
+-rw-r--r--   0        0        0      207 2024-04-28 16:59:11.003991 totolo-1.5.2.dev202404281659/totolo/__init__.py
+-rw-r--r--   0        0        0     1201 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/totolo/api.py
+-rw-r--r--   0        0        0     1893 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/totolo/collection.py
+-rw-r--r--   0        0        0        0 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/totolo/impl/__init__.py
+-rw-r--r--   0        0        0     3367 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/totolo/impl/core.py
+-rw-r--r--   0        0        0     6525 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/totolo/impl/entry.py
+-rw-r--r--   0        0        0     4595 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/totolo/impl/field.py
+-rw-r--r--   0        0        0      666 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/totolo/impl/keyword.py
+-rw-r--r--   0        0        0     8111 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/totolo/impl/parser.py
+-rw-r--r--   0        0        0        0 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/totolo/lib/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/totolo/lib/excel.py
+-rw-r--r--   0        0        0     1134 2024-04-28 16:58:04.247597 totolo-1.5.2.dev202404281659/totolo/lib/files.py
+-rw-r--r--   0        0        0      248 2024-04-28 16:58:04.251597 totolo-1.5.2.dev202404281659/totolo/lib/log.py
+-rw-r--r--   0        0        0     1283 2024-04-28 16:58:04.251597 totolo-1.5.2.dev202404281659/totolo/lib/textformat.py
+-rw-r--r--   0        0        0     3605 2024-04-28 16:58:04.251597 totolo-1.5.2.dev202404281659/totolo/story.py
+-rw-r--r--   0        0        0     2395 2024-04-28 16:58:04.251597 totolo-1.5.2.dev202404281659/totolo/theme.py
+-rw-r--r--   0        0        0    11866 2024-04-28 16:58:04.251597 totolo-1.5.2.dev202404281659/totolo/themeontology.py
+-rw-r--r--   0        0        0        0 2024-04-28 16:58:04.251597 totolo-1.5.2.dev202404281659/totolo/util/__init__.py
+-rw-r--r--   0        0        0     2221 2024-04-28 16:58:04.251597 totolo-1.5.2.dev202404281659/totolo/util/mergefiles.py
+-rw-r--r--   0        0        0     7321 2024-04-28 16:58:04.251597 totolo-1.5.2.dev202404281659/totolo/util/mergelist.py
+-rw-r--r--   0        0        0     4576 1970-01-01 00:00:00.000000 totolo-1.5.2.dev202404281659/PKG-INFO
```

### Comparing `totolo-1.5.2/.github/ISSUE_TEMPLATE/bug_report.md` & `totolo-1.5.2.dev202404281659/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/.github/ISSUE_TEMPLATE/feature_request.md` & `totolo-1.5.2.dev202404281659/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/.github/workflows/coverage-branch.yaml` & `totolo-1.5.2.dev202404281659/.github/workflows/coverage-branch.yaml`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/.github/workflows/coverage.yaml` & `totolo-1.5.2.dev202404281659/.github/workflows/coverage.yaml`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/.github/workflows/publish.yaml` & `totolo-1.5.2.dev202404281659/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/.github/workflows/test.yaml` & `totolo-1.5.2.dev202404281659/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/.gitignore` & `totolo-1.5.2.dev202404281659/.gitignore`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/.vscode/launch.json` & `totolo-1.5.2.dev202404281659/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/LICENSE` & `totolo-1.5.2.dev202404281659/LICENSE`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/README.md` & `totolo-1.5.2.dev202404281659/README.md`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/examples/basics.py` & `totolo-1.5.2.dev202404281659/examples/basics.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/pyproject.toml` & `totolo-1.5.2.dev202404281659/pyproject.toml`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/data/film-timeout-top100.st.txt` & `totolo-1.5.2.dev202404281659/tests/data/film-timeout-top100.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/data/flat.tar.gz` & `totolo-1.5.2.dev202404281659/tests/data/flat.tar.gz`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/data/sample-2023.07.23.tar.gz` & `totolo-1.5.2.dev202404281659/tests/data/sample-2023.07.23.tar.gz`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt` & `totolo-1.5.2.dev202404281659/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt` & `totolo-1.5.2.dev202404281659/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt` & `totolo-1.5.2.dev202404281659/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/data/sample-2023.07.23/notes/themes/primary.th.txt` & `totolo-1.5.2.dev202404281659/tests/data/sample-2023.07.23/notes/themes/primary.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt` & `totolo-1.5.2.dev202404281659/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/data/scifi1920-mergelist.xlsx` & `totolo-1.5.2.dev202404281659/tests/data/scifi1920-mergelist.xlsx`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/data/to-2023.07.09.th.txt` & `totolo-1.5.2.dev202404281659/tests/data/to-2023.07.09.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/data/to-sample-2023.07.09-copy.st.txt` & `totolo-1.5.2.dev202404281659/tests/data/to-sample-2023.07.09-copy.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/data/to-sample-2023.07.09.st.txt` & `totolo-1.5.2.dev202404281659/tests/data/to-sample-2023.07.09.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/lib/test_excel.py` & `totolo-1.5.2.dev202404281659/tests/lib/test_excel.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/lib/test_files.py` & `totolo-1.5.2.dev202404281659/tests/lib/test_files.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/lib/test_logging.py` & `totolo-1.5.2.dev202404281659/tests/lib/test_logging.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/lib/test_textformat.py` & `totolo-1.5.2.dev202404281659/tests/lib/test_textformat.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/test_entries.py` & `totolo-1.5.2.dev202404281659/tests/test_entries.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/test_impl.py` & `totolo-1.5.2.dev202404281659/tests/test_impl.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/test_toset.py` & `totolo-1.5.2.dev202404281659/tests/test_toset.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/test_totolo.py` & `totolo-1.5.2.dev202404281659/tests/test_totolo.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/utils/test_mergefiles.py` & `totolo-1.5.2.dev202404281659/tests/utils/test_mergefiles.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/tests/utils/test_mergelist.py` & `totolo-1.5.2.dev202404281659/tests/utils/test_mergelist.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/api.py` & `totolo-1.5.2.dev202404281659/totolo/api.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/collection.py` & `totolo-1.5.2.dev202404281659/totolo/collection.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/impl/core.py` & `totolo-1.5.2.dev202404281659/totolo/impl/core.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/impl/entry.py` & `totolo-1.5.2.dev202404281659/totolo/impl/entry.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/impl/field.py` & `totolo-1.5.2.dev202404281659/totolo/impl/field.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/impl/keyword.py` & `totolo-1.5.2.dev202404281659/totolo/impl/keyword.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/impl/parser.py` & `totolo-1.5.2.dev202404281659/totolo/impl/parser.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/lib/excel.py` & `totolo-1.5.2.dev202404281659/totolo/lib/excel.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/lib/files.py` & `totolo-1.5.2.dev202404281659/totolo/lib/files.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/lib/textformat.py` & `totolo-1.5.2.dev202404281659/totolo/lib/textformat.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/story.py` & `totolo-1.5.2.dev202404281659/totolo/story.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/theme.py` & `totolo-1.5.2.dev202404281659/totolo/theme.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/themeontology.py` & `totolo-1.5.2.dev202404281659/totolo/themeontology.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/util/mergefiles.py` & `totolo-1.5.2.dev202404281659/totolo/util/mergefiles.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/totolo/util/mergelist.py` & `totolo-1.5.2.dev202404281659/totolo/util/mergelist.py`

 * *Files identical despite different names*

### Comparing `totolo-1.5.2/PKG-INFO` & `totolo-1.5.2.dev202404281659/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totolo
-Version: 1.5.2
+Version: 1.5.2.dev202404281659
 Summary: The Python interface to themeontology.org.
 Author-email: Mikael Onsjö <mikael@odinlake.net>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Documentation, https://github.com/theme-ontology/theming
 Project-URL: Home, https://www.themeontology.org/
 Project-URL: Source, https://github.com/theme-ontology/python-totolo
```

