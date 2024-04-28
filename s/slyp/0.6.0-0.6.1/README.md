# Comparing `tmp/slyp-0.6.0.tar.gz` & `tmp/slyp-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slyp-0.6.0.tar", last modified: Fri Mar  1 04:48:04 2024, max compression
+gzip compressed data, was "slyp-0.6.1.tar", last modified: Sun Apr 28 04:14:12 2024, max compression
```

## Comparing `slyp-0.6.0.tar` & `slyp-0.6.1.tar`

### file list

```diff
@@ -1,60 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:48:04.878653 slyp-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-01 04:47:54.000000 slyp-0.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:48:04.870653 slyp-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-01 04:47:54.000000 slyp-0.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:48:04.870653 slyp-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-03-01 04:47:54.000000 slyp-0.6.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-01 04:47:54.000000 slyp-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-01 04:47:54.000000 slyp-0.6.0/.github/workflows/publish_testpypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-01 04:47:54.000000 slyp-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-01 04:47:54.000000 slyp-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-01 04:47:54.000000 slyp-0.6.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-03-01 04:47:54.000000 slyp-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-01 04:47:54.000000 slyp-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-01 04:47:54.000000 slyp-0.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-01 04:48:04.878653 slyp-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-03-01 04:47:54.000000 slyp-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-01 04:47:54.000000 slyp-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:48:04.870653 slyp-0.6.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1838 2024-03-01 04:47:54.000000 slyp-0.6.0/scripts/bump-version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-01 04:47:54.000000 slyp-0.6.0/scripts/update-generated-reference.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 04:48:04.878653 slyp-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:48:04.870653 slyp-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:48:04.874652 slyp-0.6.0/src/slyp/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:48:04.874652 slyp-0.6.0/src/slyp/checkers/
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/checkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:48:04.874652 slyp-0.6.0/src/slyp/checkers/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/checkers/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/checkers/abstract/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/checkers/abstract/matching_branches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:48:04.874652 slyp-0.6.0/src/slyp/checkers/concrete/
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/checkers/concrete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/checkers/concrete/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/checkers/concrete/str_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/file_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:48:04.874652 slyp-0.6.0/src/slyp/fixer/
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/fixer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29037 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/fixer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/hashable_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-01 04:47:54.000000 slyp-0.6.0/src/slyp/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:48:04.878653 slyp-0.6.0/src/slyp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-01 04:48:04.000000 slyp-0.6.0/src/slyp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-01 04:48:04.000000 slyp-0.6.0/src/slyp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 04:48:04.000000 slyp-0.6.0/src/slyp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-01 04:48:04.000000 slyp-0.6.0/src/slyp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-01 04:48:04.000000 slyp-0.6.0/src/slyp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-01 04:48:04.000000 slyp-0.6.0/src/slyp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:48:04.874652 slyp-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-01 04:47:54.000000 slyp-0.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:48:04.878653 slyp-0.6.0/tests/fixers/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-01 04:47:54.000000 slyp-0.6.0/tests/fixers/test_fix_none_checked_var_return.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-03-01 04:47:54.000000 slyp-0.6.0/tests/fixers/test_insert_parens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-03-01 04:47:54.000000 slyp-0.6.0/tests/fixers/test_string_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-03-01 04:47:54.000000 slyp-0.6.0/tests/fixers/test_unnecessary_parens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-03-01 04:47:54.000000 slyp-0.6.0/tests/test_result_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-01 04:47:54.000000 slyp-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.085147 slyp-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-28 04:14:01.000000 slyp-0.6.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.077147 slyp-0.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-28 04:14:01.000000 slyp-0.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.077147 slyp-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-28 04:14:01.000000 slyp-0.6.1/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-28 04:14:01.000000 slyp-0.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-28 04:14:01.000000 slyp-0.6.1/.github/workflows/publish_testpypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-28 04:14:01.000000 slyp-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-28 04:14:01.000000 slyp-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-28 04:14:01.000000 slyp-0.6.1/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-28 04:14:01.000000 slyp-0.6.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-28 04:14:01.000000 slyp-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-28 04:14:01.000000 slyp-0.6.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-28 04:14:12.085147 slyp-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-28 04:14:01.000000 slyp-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-28 04:14:01.000000 slyp-0.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.077147 slyp-0.6.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1838 2024-04-28 04:14:01.000000 slyp-0.6.1/scripts/bump-version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-28 04:14:01.000000 slyp-0.6.1/scripts/update-generated-reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 04:14:12.085147 slyp-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.077147 slyp-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.081147 slyp-0.6.1/src/slyp/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.081147 slyp-0.6.1/src/slyp/checkers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/checkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.081147 slyp-0.6.1/src/slyp/checkers/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/checkers/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/checkers/abstract/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/checkers/abstract/matching_branches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.081147 slyp-0.6.1/src/slyp/checkers/concrete/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/checkers/concrete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/checkers/concrete/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/checkers/concrete/str_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/file_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.085147 slyp-0.6.1/src/slyp/fixer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/fixer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34133 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/fixer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/hashable_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-28 04:14:01.000000 slyp-0.6.1/src/slyp/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.085147 slyp-0.6.1/src/slyp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-28 04:14:12.000000 slyp-0.6.1/src/slyp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-28 04:14:12.000000 slyp-0.6.1/src/slyp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 04:14:12.000000 slyp-0.6.1/src/slyp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-28 04:14:12.000000 slyp-0.6.1/src/slyp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-28 04:14:12.000000 slyp-0.6.1/src/slyp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-28 04:14:12.000000 slyp-0.6.1/src/slyp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.085147 slyp-0.6.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.085147 slyp-0.6.1/tests/checkers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-28 04:14:01.000000 slyp-0.6.1/tests/checkers/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-28 04:14:01.000000 slyp-0.6.1/tests/checkers/test_matching_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-28 04:14:01.000000 slyp-0.6.1/tests/checkers/test_str_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-28 04:14:01.000000 slyp-0.6.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:14:12.085147 slyp-0.6.1/tests/fixers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-28 04:14:01.000000 slyp-0.6.1/tests/fixers/test_fix_none_checked_var_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-28 04:14:01.000000 slyp-0.6.1/tests/fixers/test_insert_parens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-28 04:14:01.000000 slyp-0.6.1/tests/fixers/test_string_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-28 04:14:01.000000 slyp-0.6.1/tests/fixers/test_unnecessary_parens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-28 04:14:01.000000 slyp-0.6.1/tests/test_result_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-28 04:14:01.000000 slyp-0.6.1/tox.ini
```

### Comparing `slyp-0.6.0/.github/workflows/build.yaml` & `slyp-0.6.1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/.github/workflows/publish.yaml` & `slyp-0.6.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/.github/workflows/publish_testpypi.yaml` & `slyp-0.6.1/.github/workflows/publish_testpypi.yaml`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/.pre-commit-config.yaml` & `slyp-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/CHANGELOG.md` & `slyp-0.6.1/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 # Unreleased
 <!-- changelog-unreleased-marker -->
 
+# 0.6.1
+
+- Enable autofixing of some concatenated strings which combine f-strings with
+  simple strings, as long as no extra escaping is needed
+- Autofixing can be disabled with comments containing `slyp: disable`,
+  `slyp: disable=format`, or `fmt: off`. Inverse comments, `slyp: enable` and
+  `fmt: on` can be used to re-enable autofixing.
+
 # 0.6.0
 
 - Unexpected errors encountered when parsing files are now reported as failures, rather
   than causing `slyp` to abort
 - Replace E110 with autofixer behavior, which rewrites the return of a known-`None`
   variable immediately after testing it to return `None` instead
 - Replace W102 with autofixer behavior, which parenthesizes multiline
```

### Comparing `slyp-0.6.0/LICENSE.txt` & `slyp-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/PKG-INFO` & `slyp-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slyp
-Version: 0.6.0
+Version: 0.6.1
 Summary: Stephen Lints Your Python
 Author-email: Stephen Rosen <sirosen@globus.org>
 License: MIT
 Project-URL: source, https://github.com/sirosen/slyp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -67,15 +67,15 @@
 slyp
 ```
 
 Or as a pre-commit hook using the following `pre-commit-config.yaml`:
 
 ```yaml
 - repo: https://github.com/sirosen/slyp
-  rev: 0.6.0
+  rev: 0.6.1
   hooks:
     - id: slyp
 ```
 
 ### Options and Arguments
 
 `[files...]`: If passed positional arguments, `slyp` will treat them as
```

### Comparing `slyp-0.6.0/README.md` & `slyp-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 slyp
 ```
 
 Or as a pre-commit hook using the following `pre-commit-config.yaml`:
 
 ```yaml
 - repo: https://github.com/sirosen/slyp
-  rev: 0.6.0
+  rev: 0.6.1
   hooks:
     - id: slyp
 ```
 
 ### Options and Arguments
 
 `[files...]`: If passed positional arguments, `slyp` will treat them as
```

### Comparing `slyp-0.6.0/pyproject.toml` & `slyp-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slyp"
-version = "0.6.0"
+version = "0.6.1"
 description = "Stephen Lints Your Python"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { "text" = "MIT" }
 keywords = []
 authors = [
   { name = "Stephen Rosen", email = "sirosen@globus.org" },
```

### Comparing `slyp-0.6.0/scripts/bump-version.py` & `slyp-0.6.1/scripts/bump-version.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/scripts/update-generated-reference.py` & `slyp-0.6.1/scripts/update-generated-reference.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/src/slyp/checkers/__init__.py` & `slyp-0.6.1/src/slyp/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/src/slyp/checkers/abstract/__init__.py` & `slyp-0.6.1/src/slyp/checkers/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/src/slyp/checkers/abstract/matching_branches.py` & `slyp-0.6.1/src/slyp/checkers/abstract/matching_branches.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/src/slyp/checkers/concrete/__init__.py` & `slyp-0.6.1/src/slyp/checkers/concrete/__init__.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/src/slyp/checkers/concrete/str_concat.py` & `slyp-0.6.1/src/slyp/checkers/concrete/str_concat.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/src/slyp/cli.py` & `slyp-0.6.1/src/slyp/cli.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/src/slyp/codes.py` & `slyp-0.6.1/src/slyp/codes.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/src/slyp/driver.py` & `slyp-0.6.1/src/slyp/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from slyp.codes import CODE_MAP
 from slyp.file_cache import PassingFileCache
 from slyp.fixer import fix_file
 from slyp.hashable_file import HashableFile
 from slyp.result import Message, Result
 
 DEFAULT_DISABLED_CODES: set[str] = {"W201", "W202", "W203"}
+CONTRACT_VERSION: str = "1.4"
 
 
 def driver_main(args: argparse.Namespace) -> bool:
     # parse inputs from comma delimited lists
     disabled_codes = {x for x in args.disable.split(",") if x != ""}
     enabled_codes = {x for x in args.enable.split(",") if x != ""}
     # add default disables if "all" is not in --enable
@@ -61,15 +62,15 @@
 
 
 def parallel_process(
     args: argparse.Namespace, disabled_codes: set[str], enabled_codes: set[str]
 ) -> bool:
     if not args.no_cache:
         passing_cache: PassingFileCache | None = PassingFileCache(
-            contract_version="1.3",
+            contract_version=CONTRACT_VERSION,
             config_id=compute_config_id(enabled_codes, disabled_codes),
         )
     else:
         passing_cache = None
 
     process_pool = multiprocessing.pool.Pool()
```

### Comparing `slyp-0.6.0/src/slyp/file_cache.py` & `slyp-0.6.1/src/slyp/file_cache.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/src/slyp/fixer/transformer.py` & `slyp-0.6.1/src/slyp/fixer/transformer.py`

 * *Files 13% similar despite different names*

```diff
@@ -108,14 +108,42 @@
 
 class SlypTransformer(libcst.CSTTransformer):
     METADATA_DEPENDENCIES = (
         libcst.metadata.PositionProvider,
         libcst.metadata.ParentNodeProvider,
     )
 
+    def __init__(self, disabled_line_ranges: list[tuple[int, int | float]]) -> None:
+        self.disabled_line_ranges = disabled_line_ranges
+
+    def on_leave(
+        self, original_node: libcst.CSTNodeT, updated_node: libcst.CSTNodeT
+    ) -> (
+        libcst.CSTNodeT
+        | libcst.RemovalSentinel
+        | libcst.FlattenSentinel[libcst.CSTNodeT]
+    ):
+        new_updated_node = super().on_leave(original_node, updated_node)
+        if new_updated_node != updated_node:
+            # if the node has been updated, check if disabled
+            if not self._node_is_disabled(original_node):
+                return new_updated_node
+        return updated_node
+
+    def _node_is_disabled(self, node: libcst.CSTNode) -> bool:
+        if not self.disabled_line_ranges:
+            return False
+        start_line = self.get_metadata(
+            libcst.metadata.PositionProvider, node
+        ).start.line
+        for start, end in self.disabled_line_ranges:
+            if start <= start_line < end:
+                return True
+        return False
+
     def _singular_parens_are_same_line(
         self, node: libcst.With | libcst.ImportFrom
     ) -> bool:
         if node.lpar is not None and libcst.matchers.matches(
             node.lpar, libcst.matchers.LeftParen()
         ):
             lpar_line = self.get_metadata(
@@ -496,20 +524,25 @@
             return updated_node
         return self.modify_parenthesized_node(original_node, updated_node)
 
     def leave_ConcatenatedString(
         self,
         original_node: libcst.ConcatenatedString,
         updated_node: libcst.ConcatenatedString,
-    ) -> libcst.ConcatenatedString | libcst.SimpleString:
+    ) -> libcst.ConcatenatedString | libcst.SimpleString | libcst.FormattedString:
         new_node = updated_node
         # if the node is parenthesized, potentially strip parens
         if original_node.lpar:
             new_node = self.modify_parenthesized_node(original_node, updated_node)
 
+        left: libcst.SimpleString
+        right: libcst.SimpleString
+        left_f: libcst.FormattedString
+        right_f: libcst.FormattedString
+
         # if the node is a pair of simple strings with no newline between them,
         # this may be a chance to join them into a single string node
         if libcst.matchers.matches(
             new_node,
             libcst.matchers.ConcatenatedString(
                 whitespace_between=SIMPLE_WHITESPACE_NO_NEWLINE_MATCHER,
                 left=libcst.matchers.SimpleString(),
@@ -520,16 +553,16 @@
             # and forbid this change (for now) when one of the two is a multiline string
             # (TODO: consider when it might be safe to join multiline strings)
             #
             # the restriction against differing quote characters allows us to avoid any
             # attempt to manipulate unescaped quotes in the string values
             # having done this verification, join the strings into a single node,
             # preserving the prefix and quote style
-            left: libcst.SimpleString = new_node.left  # type: ignore[assignment]
-            right: libcst.SimpleString = new_node.right  # type: ignore[assignment]
+            left = new_node.left  # type: ignore[assignment]
+            right = new_node.right  # type: ignore[assignment]
             if (
                 (
                     left.prefix == right.prefix
                     or {left.prefix, right.prefix}.issubset({"br", "rb"})
                 )
                 and left.quote == right.quote
                 and left.quote in {"'", '"'}
@@ -539,14 +572,109 @@
                     rpar=new_node.rpar,
                     value=left.prefix
                     + left.quote
                     + left.raw_value
                     + right.raw_value
                     + left.quote,
                 )
+        # two f-strings on a line, like
+        #   f"{foo} " f"{bar}"
+        # which can merge to
+        #   f"{foo} {bar}"
+        elif libcst.matchers.matches(
+            new_node,
+            libcst.matchers.ConcatenatedString(
+                whitespace_between=SIMPLE_WHITESPACE_NO_NEWLINE_MATCHER,
+                left=libcst.matchers.FormattedString(),
+                right=libcst.matchers.FormattedString(),
+            ),
+        ):
+            left_f = new_node.left  # type: ignore[assignment]
+            right_f = new_node.right  # type: ignore[assignment]
+
+            if (
+                (
+                    left_f.prefix == right_f.prefix
+                    or {left_f.prefix, right_f.prefix}.issubset({"fr", "rf"})
+                )
+                and left_f.quote == right_f.quote
+                and left_f.quote in {"'", '"'}
+            ):
+                return libcst.FormattedString(
+                    lpar=new_node.lpar,
+                    rpar=new_node.rpar,
+                    parts=(left_f.parts + right_f.parts),  # type: ignore[operator]
+                    start=left_f.start,
+                    end=right_f.end,
+                )
+        # if it's a format string with a string that has no curly-braces (left)
+        # then we can join it, e.g.
+        #   "foo " f"{bar}"  ->  f"foo {bar}"
+        elif libcst.matchers.matches(
+            new_node,
+            libcst.matchers.ConcatenatedString(
+                whitespace_between=SIMPLE_WHITESPACE_NO_NEWLINE_MATCHER,
+                left=libcst.matchers.SimpleString(),
+                right=libcst.matchers.FormattedString(),
+            ),
+        ):
+            left = new_node.left  # type: ignore[assignment]
+            right_f = new_node.right  # type: ignore[assignment]
+            if (
+                (
+                    (left.prefix, right_f.prefix) == ("", "f")
+                    or {left.prefix, right_f.prefix}.issubset({"r", "rf", "fr"})
+                )
+                and left.quote == right_f.quote
+                and left.quote in {"'", '"'}
+                and "{" not in left.raw_value
+                and "}" not in left.raw_value
+            ):
+                return libcst.FormattedString(
+                    lpar=new_node.lpar,
+                    rpar=new_node.rpar,
+                    parts=(
+                        [libcst.FormattedStringText(value=left.raw_value)]
+                        + list(right_f.parts)
+                    ),
+                    start=right_f.start,
+                    end=right_f.end,
+                )
+        # same as the above, right-hand side; e.g.
+        #   f"{foo} " "bar"  ->  f"{foo} bar"
+        elif libcst.matchers.matches(
+            new_node,
+            libcst.matchers.ConcatenatedString(
+                whitespace_between=SIMPLE_WHITESPACE_NO_NEWLINE_MATCHER,
+                left=libcst.matchers.FormattedString(),
+                right=libcst.matchers.SimpleString(),
+            ),
+        ):
+            left_f = new_node.left  # type: ignore[assignment]
+            right = new_node.right  # type: ignore[assignment]
+            if (
+                (
+                    (left_f.prefix, right.prefix) == ("f", "")
+                    or {left_f.prefix, right.prefix}.issubset({"r", "rf", "fr"})
+                )
+                and left_f.quote == right.quote
+                and left_f.quote in {"'", '"'}
+                and "{" not in right.raw_value
+                and "}" not in right.raw_value
+            ):
+                return libcst.FormattedString(
+                    lpar=new_node.lpar,
+                    rpar=new_node.rpar,
+                    parts=(
+                        list(left_f.parts)
+                        + [libcst.FormattedStringText(value=right.raw_value)]
+                    ),
+                    start=left_f.start,
+                    end=left_f.end,
+                )
 
         return new_node
 
     def leave_FormattedString(
         self,
         original_node: libcst.FormattedString,
         updated_node: libcst.FormattedString,
```

### Comparing `slyp-0.6.0/src/slyp/hashable_file.py` & `slyp-0.6.1/src/slyp/hashable_file.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/src/slyp/result.py` & `slyp-0.6.1/src/slyp/result.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/src/slyp.egg-info/PKG-INFO` & `slyp-0.6.1/src/slyp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slyp
-Version: 0.6.0
+Version: 0.6.1
 Summary: Stephen Lints Your Python
 Author-email: Stephen Rosen <sirosen@globus.org>
 License: MIT
 Project-URL: source, https://github.com/sirosen/slyp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -67,15 +67,15 @@
 slyp
 ```
 
 Or as a pre-commit hook using the following `pre-commit-config.yaml`:
 
 ```yaml
 - repo: https://github.com/sirosen/slyp
-  rev: 0.6.0
+  rev: 0.6.1
   hooks:
     - id: slyp
 ```
 
 ### Options and Arguments
 
 `[files...]`: If passed positional arguments, `slyp` will treat them as
```

### Comparing `slyp-0.6.0/tests/conftest.py` & `slyp-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/tests/fixers/test_insert_parens.py` & `slyp-0.6.1/tests/fixers/test_insert_parens.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,29 @@
                 "foo"
                 "bar"
             ))
         """
     )
 
 
+@pytest.mark.parametrize(
+    "disable_comment",
+    ("# fmt: off", "#fmt:off ", "#slyp: disable", "# slyp: disable=format "),
+)
+def test_missing_paren_transform_disabled_with_fmt_off(fix_text, disable_comment):
+    fix_text(
+        f"""\
+        #{disable_comment}
+        foo(x="foo"
+        "bar")
+        """,
+        expect_changes=False,
+    )
+
+
 def test_fixer_inserts_missing_parens_call_arg_in_list(fix_text):
     # normal case for paren insertion fixer, in an arg list
     # black fixing will be a no-op because we already handle indents nicely for this
     new_text, _ = fix_text(
         """\
         foo(
             x=1,
```

### Comparing `slyp-0.6.0/tests/fixers/test_string_concat.py` & `slyp-0.6.1/tests/fixers/test_string_concat.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,14 +24,31 @@
         e = b"foo bar"
         f = br"foo bar"
         g = rb"foo bar"
         """
     )
 
 
+def test_fmt_toggle_can_reenable_fixing(fix_text):
+    new_text, _ = fix_text(
+        """\
+        # slyp: disable
+        # fmt: on
+        a = "foo " "bar"
+        """,
+    )
+    assert new_text == textwrap.dedent(
+        """\
+        # slyp: disable
+        # fmt: on
+        a = "foo bar"
+        """
+    )
+
+
 def test_quote_style_mismatch_suppresses_fixing(fix_text):
     fix_text(
         """\
         a = "foo " 'bar'
         """,
         expect_changes=False,
     )
@@ -82,7 +99,61 @@
         """,
     )
     assert new_text == textwrap.dedent(
         """\
         x = "foo bar baz"
         """
     )
+
+
+def test_concat_fstrings(fix_text):
+    new_text, _ = fix_text(
+        """\
+        x = f"{foo}" f"{bar}"
+        y = fr"{foo}" Fr"{bar}"
+        """,
+    )
+    assert new_text == textwrap.dedent(
+        """\
+        x = f"{foo}{bar}"
+        y = fr"{foo}{bar}"
+        """
+    )
+
+
+def test_concat_fstring_with_simple(fix_text):
+    new_text, _ = fix_text(
+        """\
+        x = f"{foo}" "bar"
+        y = "foo" f"{bar}"
+        p = fr"{foo}" r"bar"
+        q = r"foo" rf"{bar}"
+        """,
+    )
+    assert new_text == textwrap.dedent(
+        """\
+        x = f"{foo}bar"
+        y = f"foo{bar}"
+        p = fr"{foo}bar"
+        q = rf"foo{bar}"
+        """
+    )
+
+
+def test_concat_fstring_skips_mismatched_quotes(fix_text):
+    fix_text(
+        """\
+        x = f'{foo}' "bar"
+        y = 'foo' f"{bar}"
+        """,
+        expect_changes=False,
+    )
+
+
+def test_concat_fstring_skips_if_curly_braces_present(fix_text):
+    fix_text(
+        """\
+        x = f'{foo}' "bar{}"
+        x = 'foo{}' f"{bar}"
+        """,
+        expect_changes=False,
+    )
```

### Comparing `slyp-0.6.0/tests/fixers/test_unnecessary_parens.py` & `slyp-0.6.1/tests/fixers/test_unnecessary_parens.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/tests/test_result_caching.py` & `slyp-0.6.1/tests/test_result_caching.py`

 * *Files identical despite different names*

### Comparing `slyp-0.6.0/tox.ini` & `slyp-0.6.1/tox.ini`

 * *Files identical despite different names*

