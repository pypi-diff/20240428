# Comparing `tmp/pynormalizenumexp-0.3.0.tar.gz` & `tmp/pynormalizenumexp-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynormalizenumexp-0.3.0.tar", max compression
+gzip compressed data, was "pynormalizenumexp-0.3.1.tar", max compression
```

## Comparing `pynormalizenumexp-0.3.0.tar` & `pynormalizenumexp-0.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1525 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/LICENSE
--rw-r--r--   0        0        0     7496 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/README.md
--rw-r--r--   0        0        0       65 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/expression/__init__.py
--rw-r--r--   0        0        0     2631 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/expression/abstime.py
--rw-r--r--   0        0        0    12056 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/expression/base.py
--rw-r--r--   0        0        0     2629 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/expression/duration.py
--rw-r--r--   0        0        0     2891 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/expression/numerical.py
--rw-r--r--   0        0        0     3284 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/expression/reltime.py
--rw-r--r--   0        0        0     9634 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalize_numexp.py
--rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/__init__.py
--rw-r--r--   0        0        0    31439 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/abstime_expr_normalizer.py
--rw-r--r--   0        0        0    16741 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/base.py
--rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/converter/__init__.py
--rw-r--r--   0        0        0     1671 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/converter/japanese_number_converter.py
--rw-r--r--   0        0        0     3501 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/converter/number_converter.py
--rw-r--r--   0        0        0    19841 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/duration_expr_normalizer.py
--rw-r--r--   0        0        0    11692 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/inappropriate_expr_remover.py
--rw-r--r--   0        0        0     9250 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/number_extractor.py
--rw-r--r--   0        0        0    13820 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/number_normalizer.py
--rw-r--r--   0        0        0    14587 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/numerical_expr_normalizer.py
--rw-r--r--   0        0        0    33029 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/reltime_expr_normalizer.py
--rw-r--r--   0        0        0     9236 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/symbol_fixer.py
--rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/py.typed
--rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/__init__.py
--rw-r--r--   0        0        0     3268 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/README.md
--rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/__init__.py
--rw-r--r--   0        0        0   780034 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_expression.json
--rw-r--r--   0        0        0     1504 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_prefix.json
--rw-r--r--   0        0        0    47427 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_prefix_counter.json
--rw-r--r--   0        0        0     3491 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_suffix.json
--rw-r--r--   0        0        0     2247 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/chinese_character.json
--rw-r--r--   0        0        0     8470 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_expression.json
--rw-r--r--   0        0        0     1105 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_prefix.json
--rw-r--r--   0        0        0       20 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_prefix_counter.json
--rw-r--r--   0        0        0     2341 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_suffix.json
--rw-r--r--   0        0        0      371 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/inappropriate_strings.json
--rw-r--r--   0        0        0   265283 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_counter.json
--rw-r--r--   0        0        0     1105 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_prefix.json
--rw-r--r--   0        0        0     4886 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_prefix_counter.json
--rw-r--r--   0        0        0     2810 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_suffix.json
--rw-r--r--   0        0        0   925242 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_expression.json
--rw-r--r--   0        0        0     1035 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_prefix.json
--rw-r--r--   0        0        0     3265 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_prefix_counter.json
--rw-r--r--   0        0        0     3491 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_suffix.json
--rw-r--r--   0        0        0        0 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/utility/__init__.py
--rw-r--r--   0        0        0     2105 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/utility/custom_type.py
--rw-r--r--   0        0        0    13789 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/utility/dict_loader.py
--rw-r--r--   0        0        0    10081 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/utility/digit_utility.py
--rw-r--r--   0        0        0     6797 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/utility/normalizer_utility.py
--rw-r--r--   0        0        0     1042 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8164 1970-01-01 00:00:00.000000 pynormalizenumexp-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1525 2024-04-28 10:29:58.063441 pynormalizenumexp-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7484 2024-04-28 10:29:58.063441 pynormalizenumexp-0.3.1/README.md
+-rw-r--r--   0        0        0       65 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/expression/__init__.py
+-rw-r--r--   0        0        0     2631 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/expression/abstime.py
+-rw-r--r--   0        0        0    12056 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/expression/base.py
+-rw-r--r--   0        0        0     2629 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/expression/duration.py
+-rw-r--r--   0        0        0     2891 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/expression/numerical.py
+-rw-r--r--   0        0        0     3284 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/expression/reltime.py
+-rw-r--r--   0        0        0     9634 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalize_numexp.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/__init__.py
+-rw-r--r--   0        0        0    31439 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/abstime_expr_normalizer.py
+-rw-r--r--   0        0        0    16741 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/base.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/converter/__init__.py
+-rw-r--r--   0        0        0     1671 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/converter/japanese_number_converter.py
+-rw-r--r--   0        0        0     3501 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/converter/number_converter.py
+-rw-r--r--   0        0        0    19841 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/duration_expr_normalizer.py
+-rw-r--r--   0        0        0    11692 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/inappropriate_expr_remover.py
+-rw-r--r--   0        0        0     9250 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/number_extractor.py
+-rw-r--r--   0        0        0    13820 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/number_normalizer.py
+-rw-r--r--   0        0        0    14587 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/numerical_expr_normalizer.py
+-rw-r--r--   0        0        0    33029 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/reltime_expr_normalizer.py
+-rw-r--r--   0        0        0     9236 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/symbol_fixer.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/py.typed
+-rw-r--r--   0        0        0        0 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/__init__.py
+-rw-r--r--   0        0        0     3268 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/README.md
+-rw-r--r--   0        0        0        0 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:29:58.067441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/__init__.py
+-rw-r--r--   0        0        0   780034 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/abstime_expression.json
+-rw-r--r--   0        0        0     1504 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/abstime_prefix.json
+-rw-r--r--   0        0        0    47427 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/abstime_prefix_counter.json
+-rw-r--r--   0        0        0     3491 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/abstime_suffix.json
+-rw-r--r--   0        0        0     2247 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/chinese_character.json
+-rw-r--r--   0        0        0     8470 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/duration_expression.json
+-rw-r--r--   0        0        0     1105 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/duration_prefix.json
+-rw-r--r--   0        0        0       20 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/duration_prefix_counter.json
+-rw-r--r--   0        0        0     2341 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/duration_suffix.json
+-rw-r--r--   0        0        0      371 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/inappropriate_strings.json
+-rw-r--r--   0        0        0   265283 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/num_counter.json
+-rw-r--r--   0        0        0     1105 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/num_prefix.json
+-rw-r--r--   0        0        0     4886 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/num_prefix_counter.json
+-rw-r--r--   0        0        0     2810 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/num_suffix.json
+-rw-r--r--   0        0        0   925242 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/reltime_expression.json
+-rw-r--r--   0        0        0     1035 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/reltime_prefix.json
+-rw-r--r--   0        0        0     3265 2024-04-28 10:29:58.071441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/reltime_prefix_counter.json
+-rw-r--r--   0        0        0     3491 2024-04-28 10:29:58.075441 pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/reltime_suffix.json
+-rw-r--r--   0        0        0        0 2024-04-28 10:29:58.075441 pynormalizenumexp-0.3.1/pynormalizenumexp/utility/__init__.py
+-rw-r--r--   0        0        0     2105 2024-04-28 10:29:58.075441 pynormalizenumexp-0.3.1/pynormalizenumexp/utility/custom_type.py
+-rw-r--r--   0        0        0    13789 2024-04-28 10:29:58.075441 pynormalizenumexp-0.3.1/pynormalizenumexp/utility/dict_loader.py
+-rw-r--r--   0        0        0    10081 2024-04-28 10:29:58.075441 pynormalizenumexp-0.3.1/pynormalizenumexp/utility/digit_utility.py
+-rw-r--r--   0        0        0     6797 2024-04-28 10:29:58.075441 pynormalizenumexp-0.3.1/pynormalizenumexp/utility/normalizer_utility.py
+-rw-r--r--   0        0        0     1042 2024-04-28 10:29:58.075441 pynormalizenumexp-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8152 1970-01-01 00:00:00.000000 pynormalizenumexp-0.3.1/PKG-INFO
```

### Comparing `pynormalizenumexp-0.3.0/LICENSE` & `pynormalizenumexp-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/README.md` & `pynormalizenumexp-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![PyPI version](https://badge.fury.io/py/pynormalizenumexp.svg)](https://badge.fury.io/py/pynormalizenumexp)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pynormalizenumexp.svg)](https://pypi.org/project/pynormalizenumexp/)
 [![pytest](https://github.com/tkscode/pyNormalizeNumExp/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/tkscode/pyNormalizeNumExp/actions/workflows/pytest.yml)
-[![codecov](https://codecov.io/gh/tkscode/pyNormalizeNumExp/branch/main/graph/badge.svg?token=3Z0YIZV5U1)](https://codecov.io/gh/tkscode/pyNormalizeNumExp)
+[![codecov](https://codecov.io/gh/tkscode/pyNormalizeNumExp/graph/badge.svg?token=3Z0YIZV5U1)](https://codecov.io/gh/tkscode/pyNormalizeNumExp)
 
 
 # pyNormalizeNumexp
 
 数量表現や時間表現の抽出・正規化を行う[NormalizeNumexp](https://www.cl.ecei.tohoku.ac.jp/Open_Resources-normalizeNumexp.html)のPython実装です。  
 本家でもSWIGによるPythonバインディングが提供されていますが、NormalizeNumexp本体のインストールでトラブルに遭うことが多いため、全実装をPythonに移植しました。
```

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/expression/abstime.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/expression/abstime.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/expression/base.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/expression/base.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/expression/duration.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/expression/duration.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/expression/numerical.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/expression/numerical.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/expression/reltime.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/expression/reltime.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/normalize_numexp.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/normalize_numexp.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/abstime_expr_normalizer.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/abstime_expr_normalizer.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/base.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/base.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/converter/japanese_number_converter.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/converter/japanese_number_converter.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/converter/number_converter.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/converter/number_converter.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/duration_expr_normalizer.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/duration_expr_normalizer.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/inappropriate_expr_remover.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/inappropriate_expr_remover.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/number_extractor.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/number_extractor.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/number_normalizer.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/number_normalizer.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/numerical_expr_normalizer.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/numerical_expr_normalizer.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/reltime_expr_normalizer.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/reltime_expr_normalizer.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/symbol_fixer.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/normalizer/symbol_fixer.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/README.md` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/README.md`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_expression.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/abstime_expression.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_prefix.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/abstime_prefix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_prefix_counter.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/abstime_prefix_counter.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_suffix.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/abstime_suffix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/chinese_character.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/chinese_character.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_expression.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/duration_expression.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_prefix.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/duration_prefix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_suffix.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/duration_suffix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_counter.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/num_counter.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_prefix.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/num_prefix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_prefix_counter.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/num_prefix_counter.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_suffix.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/num_suffix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_expression.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/reltime_expression.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_prefix.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/reltime_prefix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_prefix_counter.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/reltime_prefix_counter.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_suffix.json` & `pynormalizenumexp-0.3.1/pynormalizenumexp/resources/dict/ja/reltime_suffix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/utility/custom_type.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/utility/custom_type.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/utility/dict_loader.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/utility/dict_loader.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/utility/digit_utility.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/utility/digit_utility.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pynormalizenumexp/utility/normalizer_utility.py` & `pynormalizenumexp-0.3.1/pynormalizenumexp/utility/normalizer_utility.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.3.0/pyproject.toml` & `pynormalizenumexp-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynormalizenumexp"
-version = "0.3.0"
+version = "0.3.1"
 description = "NormalizeNumExp for Python"
 authors = ["tkscode"]
 license = "BSD 3-Clause"
 readme = "README.md"
 repository = "https://github.com/tkscode/pyNormalizeNumExp"
 homepage = "https://github.com/tkscode/pyNormalizeNumExp"
 keywords = ["Python", "NLP", "NormalizeNumExp"]
```

### Comparing `pynormalizenumexp-0.3.0/PKG-INFO` & `pynormalizenumexp-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynormalizenumexp
-Version: 0.3.0
+Version: 0.3.1
 Summary: NormalizeNumExp for Python
 Home-page: https://github.com/tkscode/pyNormalizeNumExp
 License: BSD 3-Clause
 Keywords: Python,NLP,NormalizeNumExp
 Author: tkscode
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/tkscode/pyNormalizeNumExp
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/pynormalizenumexp.svg)](https://badge.fury.io/py/pynormalizenumexp)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pynormalizenumexp.svg)](https://pypi.org/project/pynormalizenumexp/)
 [![pytest](https://github.com/tkscode/pyNormalizeNumExp/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/tkscode/pyNormalizeNumExp/actions/workflows/pytest.yml)
-[![codecov](https://codecov.io/gh/tkscode/pyNormalizeNumExp/branch/main/graph/badge.svg?token=3Z0YIZV5U1)](https://codecov.io/gh/tkscode/pyNormalizeNumExp)
+[![codecov](https://codecov.io/gh/tkscode/pyNormalizeNumExp/graph/badge.svg?token=3Z0YIZV5U1)](https://codecov.io/gh/tkscode/pyNormalizeNumExp)
 
 
 # pyNormalizeNumexp
 
 数量表現や時間表現の抽出・正規化を行う[NormalizeNumexp](https://www.cl.ecei.tohoku.ac.jp/Open_Resources-normalizeNumexp.html)のPython実装です。  
 本家でもSWIGによるPythonバインディングが提供されていますが、NormalizeNumexp本体のインストールでトラブルに遭うことが多いため、全実装をPythonに移植しました。
```

