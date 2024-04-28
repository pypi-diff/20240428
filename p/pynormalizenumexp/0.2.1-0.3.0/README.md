# Comparing `tmp/pynormalizenumexp-0.2.1.tar.gz` & `tmp/pynormalizenumexp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynormalizenumexp-0.2.1.tar", max compression
+gzip compressed data, was "pynormalizenumexp-0.3.0.tar", max compression
```

## Comparing `pynormalizenumexp-0.2.1.tar` & `pynormalizenumexp-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0     1525 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/LICENSE
--rw-r--r--   0        0        0     6537 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/README.md
--rw-r--r--   0        0        0       65 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/__init__.py
--rw-r--r--   0        0        0        0 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/expression/__init__.py
--rw-r--r--   0        0        0     2631 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/expression/abstime.py
--rw-r--r--   0        0        0    12056 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/expression/base.py
--rw-r--r--   0        0        0     2629 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/expression/duration.py
--rw-r--r--   0        0        0     2891 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/expression/numerical.py
--rw-r--r--   0        0        0     3284 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/expression/reltime.py
--rw-r--r--   0        0        0     9479 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalize_numexp.py
--rw-r--r--   0        0        0        0 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/__init__.py
--rw-r--r--   0        0        0    31127 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/abstime_expr_normalizer.py
--rw-r--r--   0        0        0    16741 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/base.py
--rw-r--r--   0        0        0        0 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/converter/__init__.py
--rw-r--r--   0        0        0     1671 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/converter/japanese_number_converter.py
--rw-r--r--   0        0        0     3501 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/converter/number_converter.py
--rw-r--r--   0        0        0    19525 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/duration_expr_normalizer.py
--rw-r--r--   0        0        0    11692 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/inappropriate_expr_remover.py
--rw-r--r--   0        0        0     9250 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/number_extractor.py
--rw-r--r--   0        0        0    13820 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/number_normalizer.py
--rw-r--r--   0        0        0    14279 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/numerical_expr_normalizer.py
--rw-r--r--   0        0        0    32717 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/reltime_expr_normalizer.py
--rw-r--r--   0        0        0     9236 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/symbol_fixer.py
--rw-r--r--   0        0        0        0 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/py.typed
--rw-r--r--   0        0        0        0 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/__init__.py
--rw-r--r--   0        0        0        0 2024-01-16 13:16:29.041531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/__init__.py
--rw-r--r--   0        0        0   780034 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/abstime_expression.json
--rw-r--r--   0        0        0     1504 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/abstime_prefix.json
--rw-r--r--   0        0        0    47427 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/abstime_prefix_counter.json
--rw-r--r--   0        0        0     3491 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/abstime_suffix.json
--rw-r--r--   0        0        0     2247 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/chinese_character.json
--rw-r--r--   0        0        0     8470 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/duration_expression.json
--rw-r--r--   0        0        0     1105 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/duration_prefix.json
--rw-r--r--   0        0        0       20 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/duration_prefix_counter.json
--rw-r--r--   0        0        0     2341 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/duration_suffix.json
--rw-r--r--   0        0        0      371 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/inappropriate_strings.json
--rw-r--r--   0        0        0   265283 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/num_counter.json
--rw-r--r--   0        0        0     1105 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/num_prefix.json
--rw-r--r--   0        0        0     4886 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/num_prefix_counter.json
--rw-r--r--   0        0        0     2810 2024-01-16 13:16:29.045531 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/num_suffix.json
--rw-r--r--   0        0        0   925242 2024-01-16 13:16:29.049532 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/reltime_expression.json
--rw-r--r--   0        0        0     1035 2024-01-16 13:16:29.049532 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/reltime_prefix.json
--rw-r--r--   0        0        0     3265 2024-01-16 13:16:29.049532 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/reltime_prefix_counter.json
--rw-r--r--   0        0        0     3491 2024-01-16 13:16:29.049532 pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/reltime_suffix.json
--rw-r--r--   0        0        0        0 2024-01-16 13:16:29.049532 pynormalizenumexp-0.2.1/pynormalizenumexp/utility/__init__.py
--rw-r--r--   0        0        0     2105 2024-01-16 13:16:29.049532 pynormalizenumexp-0.2.1/pynormalizenumexp/utility/custom_type.py
--rw-r--r--   0        0        0     7583 2024-01-16 13:16:29.049532 pynormalizenumexp-0.2.1/pynormalizenumexp/utility/dict_loader.py
--rw-r--r--   0        0        0    10081 2024-01-16 13:16:29.049532 pynormalizenumexp-0.2.1/pynormalizenumexp/utility/digit_utility.py
--rw-r--r--   0        0        0     6797 2024-01-16 13:16:29.049532 pynormalizenumexp-0.2.1/pynormalizenumexp/utility/normalizer_utility.py
--rw-r--r--   0        0        0     1042 2024-01-16 13:16:29.049532 pynormalizenumexp-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7205 1970-01-01 00:00:00.000000 pynormalizenumexp-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1525 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7496 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/README.md
+-rw-r--r--   0        0        0       65 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/expression/__init__.py
+-rw-r--r--   0        0        0     2631 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/expression/abstime.py
+-rw-r--r--   0        0        0    12056 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/expression/base.py
+-rw-r--r--   0        0        0     2629 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/expression/duration.py
+-rw-r--r--   0        0        0     2891 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/expression/numerical.py
+-rw-r--r--   0        0        0     3284 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/expression/reltime.py
+-rw-r--r--   0        0        0     9634 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalize_numexp.py
+-rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/__init__.py
+-rw-r--r--   0        0        0    31439 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/abstime_expr_normalizer.py
+-rw-r--r--   0        0        0    16741 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/base.py
+-rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/converter/__init__.py
+-rw-r--r--   0        0        0     1671 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/converter/japanese_number_converter.py
+-rw-r--r--   0        0        0     3501 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/converter/number_converter.py
+-rw-r--r--   0        0        0    19841 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/duration_expr_normalizer.py
+-rw-r--r--   0        0        0    11692 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/inappropriate_expr_remover.py
+-rw-r--r--   0        0        0     9250 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/number_extractor.py
+-rw-r--r--   0        0        0    13820 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/number_normalizer.py
+-rw-r--r--   0        0        0    14587 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/numerical_expr_normalizer.py
+-rw-r--r--   0        0        0    33029 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/reltime_expr_normalizer.py
+-rw-r--r--   0        0        0     9236 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/symbol_fixer.py
+-rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/py.typed
+-rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/__init__.py
+-rw-r--r--   0        0        0     3268 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/README.md
+-rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 08:06:51.035862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/__init__.py
+-rw-r--r--   0        0        0   780034 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_expression.json
+-rw-r--r--   0        0        0     1504 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_prefix.json
+-rw-r--r--   0        0        0    47427 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_prefix_counter.json
+-rw-r--r--   0        0        0     3491 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_suffix.json
+-rw-r--r--   0        0        0     2247 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/chinese_character.json
+-rw-r--r--   0        0        0     8470 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_expression.json
+-rw-r--r--   0        0        0     1105 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_prefix.json
+-rw-r--r--   0        0        0       20 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_prefix_counter.json
+-rw-r--r--   0        0        0     2341 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_suffix.json
+-rw-r--r--   0        0        0      371 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/inappropriate_strings.json
+-rw-r--r--   0        0        0   265283 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_counter.json
+-rw-r--r--   0        0        0     1105 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_prefix.json
+-rw-r--r--   0        0        0     4886 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_prefix_counter.json
+-rw-r--r--   0        0        0     2810 2024-04-28 08:06:51.039862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_suffix.json
+-rw-r--r--   0        0        0   925242 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_expression.json
+-rw-r--r--   0        0        0     1035 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_prefix.json
+-rw-r--r--   0        0        0     3265 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_prefix_counter.json
+-rw-r--r--   0        0        0     3491 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_suffix.json
+-rw-r--r--   0        0        0        0 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/utility/__init__.py
+-rw-r--r--   0        0        0     2105 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/utility/custom_type.py
+-rw-r--r--   0        0        0    13789 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/utility/dict_loader.py
+-rw-r--r--   0        0        0    10081 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/utility/digit_utility.py
+-rw-r--r--   0        0        0     6797 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pynormalizenumexp/utility/normalizer_utility.py
+-rw-r--r--   0        0        0     1042 2024-04-28 08:06:51.043862 pynormalizenumexp-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8164 1970-01-01 00:00:00.000000 pynormalizenumexp-0.3.0/PKG-INFO
```

### Comparing `pynormalizenumexp-0.2.1/LICENSE` & `pynormalizenumexp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/README.md` & `pynormalizenumexp-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,40 @@
+Metadata-Version: 2.1
+Name: pynormalizenumexp
+Version: 0.3.0
+Summary: NormalizeNumExp for Python
+Home-page: https://github.com/tkscode/pyNormalizeNumExp
+License: BSD 3-Clause
+Keywords: Python,NLP,NormalizeNumExp
+Author: tkscode
+Requires-Python: >=3.9,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Project-URL: Repository, https://github.com/tkscode/pyNormalizeNumExp
+Description-Content-Type: text/markdown
+
 [![PyPI version](https://badge.fury.io/py/pynormalizenumexp.svg)](https://badge.fury.io/py/pynormalizenumexp)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pynormalizenumexp.svg)](https://pypi.org/project/pynormalizenumexp/)
 [![pytest](https://github.com/tkscode/pyNormalizeNumExp/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/tkscode/pyNormalizeNumExp/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/tkscode/pyNormalizeNumExp/branch/main/graph/badge.svg?token=3Z0YIZV5U1)](https://codecov.io/gh/tkscode/pyNormalizeNumExp)
 
 
 # pyNormalizeNumexp
 
 数量表現や時間表現の抽出・正規化を行う[NormalizeNumexp](https://www.cl.ecei.tohoku.ac.jp/Open_Resources-normalizeNumexp.html)のPython実装です。  
 本家でもSWIGによるPythonバインディングが提供されていますが、NormalizeNumexp本体のインストールでトラブルに遭うことが多いため、全実装をPythonに移植しました。
 
 
 ## Prerequisites
 
-Python >=3.9, <=3.12
+Python `>=3.9`, `<=3.12`
 
 
 ## Installation
 
 ```
 pip install pynormalizenumexp
 ```
@@ -32,20 +50,20 @@
 results = normalizer.normalize("魔女狩りは15世紀～18世紀にかけてみられ、全ヨーロッパで4万人が処刑された", as_dict=True)
 for r in results:
 	print(r)
 # {'type': 'abstime', 'original_expr': '15世紀～18世紀', 'position_start': 5, 'position_end': 14, 'counter': 'none', 'value_lower_bound': {'year': 1401, 'month': inf, 'day': inf, 'hour': inf, 'minute': inf, 'second': inf}, 'value_upper_bound': {'year': 1800, 'month': -inf, 'day': -inf, 'hour': -inf, 'minute': -inf, 'second': -inf}, 'value_lower_bound_abs': None, 'value_upper_bound_abs': None, 'value_lower_bound_rel': None, 'value_upper_bound_rel': None, 'options': []}
 # {'type': 'numerical', 'original_expr': '4万人', 'position_start': 29, 'position_end': 32, 'counter': '人', 'value_lower_bound': 40000, 'value_upper_bound': 40000, 'value_lower_bound_abs': None, 'value_upper_bound_abs': None, 'value_lower_bound_rel': None, 'value_upper_bound_rel': None, 'options': []}
 ```
 
-+ `NormalizeNumexp`クラスの引数に言語識別子を指定します（例：日本語であれば`ja`）
-	+ 本家では英語`en`や中国語`zh`にも対応していますが、本ライブラリでは日本語のみに対応しています（将来的には英語・中国語も入れる予定です）
-+ `NormalizeNumexp`クラスの`normalize`関数に抽出・正規化対象のテキストを指定します
-	+ `as_dict`引数に`True`を指定することで、返り値の数量・時間表現のオブジェクトが`dict`型になります
-		+ 数量・時間表現のオブジェクトの属性については[`Expression`](./pynormalizenumexp/normalize_numexp.py#L19)クラスを参照してください
-+ 返り値が`dict`型の場合のデータ構造は以下の通りです
++ `NormalizeNumexp`クラスの引数に言語識別子を指定します。（例：日本語であれば`ja`）
+	+ 本家では英語`en`や中国語`zh`にも対応していますが、本ライブラリでは日本語のみに対応しています。（将来的には英語・中国語も入れる予定です）
++ `NormalizeNumexp`クラスの`normalize`関数に抽出・正規化対象のテキストを指定します。
+	+ `as_dict`引数に`True`を指定することで、返り値の数量・時間表現のオブジェクトが`dict`型になります。
+		+ 数量・時間表現のオブジェクトの属性については[`Expression`](./pynormalizenumexp/normalize_numexp.py#L19)クラスを参照してください。
++ 返り値が`dict`型の場合のデータ構造は以下の通りです。
 	```python
 	{
 		"type": str, # 表現種別（numerical：数量、abstime：絶対時間、reltime：相対時間、duration：期間）
 		"original_expr": str, # 数値・時間表現の文字列
 		"position_start": int, # 抽出元テキストにおける開始位置
 		"position_end": int, # 抽出元テキストにおける終了位置
 		"counter": str, # 「人」や「匹」などの単位（typeがnumerical以外の場合は "none" になる）
@@ -54,33 +72,49 @@
 		"value_lower_bound_abs": None | Dict[str, int | float], # ※2
 		"value_upper_bound_abs": None | Dict[str, int | float], # ※2
 		"value_lower_bound_rel": None | Dict[str, int | float], # ※3
 		"value_upper_bound_rel": None | Dict[str, int | float], # ※3
 		"options": List[str]
 	}
 	```
-	+ ※1：数量・時間表現の下限値（lower）・上限値（upper）が入るが、`type`によって値の種類が変化する
+	+ ※1：数量・時間表現の下限値（lower）・上限値（upper）が入るが、`type`によって値の種類が変化します。
 		+ `numerical`の場合：`int`または`float`
 			+ 例：`15.3ポイント`の場合は下限・上限ともに`15.3`
 			+ 例：`1～2人`の場合は下限が`1`、上限が`2`
 		+ `abstime`または`duration`の場合：`Dict[str, int | float]`
-			+ 例：`2021年1月1日`の場合は下限・上限ともに`{"year": 2021, "month": 1, "day": 1}`となる（`hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になる）
-			+ 例：`3/3～3/5`の場合は下限が`{"month": 3, "day": 3}`、上限が`{"month": 3, "day": 5}`となる（`year`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になる）
-			+ 例：`100年間`の場合は下限・上限ともに`{"year": 100}`となる（`month`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になる）
+			+ 例：`2021年1月1日`の場合は下限・上限ともに`{"year": 2021, "month": 1, "day": 1}`（`hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になります）
+			+ 例：`3/3～3/5`の場合は下限が`{"month": 3, "day": 3}`、上限が`{"month": 3, "day": 5}`（`year`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になります）
+			+ 例：`100年間`の場合は下限・上限ともに`{"year": 100}`（`month`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になります）
 		+ `reltime`の場合：`None`
-	+ ※2：`type`が`reltime`の場合に絶対時間表現の下限値（lower）・上限値（upper）が入る（その他の`type`の場合は`None`になる）
-		+ 例：`昨年3月`の場合は下限・上限ともに`{"month": 3}`となる（`year`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になる）
-	+ ※3：`type`が`reltime`の場合に相対時間表現の下限値（lower）・上限値（upper）が入る（その他の`type`の場合は`None`になる）
-		+ 例：`昨年3月`の場合は下限・上限ともに`{"year": -1}`となる（`month`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になる）
-		+ 例：`15年前`の場合下限・上限ともに`{"year": -15}`となる（`month`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になる）
+	+ ※2：`type`が`reltime`の場合に絶対時間表現の下限値（lower）・上限値（upper）が入ります。（その他の`type`の場合は`None`になります）
+		+ 例：`昨年3月`の場合は下限・上限ともに`{"month": 3}`（`year`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になります）
+	+ ※3：`type`が`reltime`の場合に相対時間表現の下限値（lower）・上限値（upper）が入ります。（その他の`type`の場合は`None`になります）
+		+ 例：`昨年3月`の場合は下限・上限ともに`{"year": -1}`（`month`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になります）
+		+ 例：`15年前`の場合下限・上限ともに`{"year": -15}`（`month`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になります）
+
+### 抽出する数値表現パターンを追加したい場合
+
+[予め用意した辞書](./pynormalizenumexp/resources/dict/ja/)に定義されていないパターンの数値表現を抽出したい場合、カスタム辞書ファイルを別途定義して読み込ませることができます。
+
+任意のディレクトリにJSON形式の辞書ファイル（以下の例では`/path/to/custom_dict.json`）を定義し、`NormalizeNumexp`クラスの第2引数に辞書ファイルのパスを指定することで反映することができます。  
+辞書の作り方については[こちら](./pynormalizenumexp/resources/dict/README.md)を参照してください。
+```python
+from pynormalizenumexp.normalize_numexp import NormalizeNumexp
+
+normalizer = NormalizeNumexp("ja", "/path/to/custom_dict.json")
+
+results = normalizer.normalize("メールに2ファイル添付する", as_dict=True)
+```
+
 
 ## 免責事項
 
 + 本ライブラリの作成にあたり、単体テスト等で動作確認はしていますが、ケースによっては期待通りの振る舞いをしない可能性があります
 + 本ライブラリの利用により、万一、利用者に何らかの不都合や損害が発生したとしても、作者は何らの責任を負うものではありません
 
 
 ## Special thanks
 
 + [東北大学 乾・鈴木研究室](https://www.cl.ecei.tohoku.ac.jp/Open_Resources-normalizeNumexp.html)
 + [nullnull/normalizeNumexp](https://github.com/nullnull/normalizeNumexp)（本家実装）
 + [cotogoto/normalize-numexp](https://github.com/cotogoto/normalize-numexp)（Java移植版）
+
```

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/expression/abstime.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/expression/abstime.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/expression/base.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/expression/base.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/expression/duration.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/expression/duration.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/expression/numerical.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/expression/numerical.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/expression/reltime.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/expression/reltime.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/normalize_numexp.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/normalize_numexp.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,23 +73,25 @@
     value_upper_bound_rel: Optional[Time] = None
     options: list[str] = field(default_factory=list)
 
 
 class NormalizeNumexp(object):
     """各種数値表現の抽出・正規化を行うクラス."""
 
-    def __init__(self, language: str) -> None:
+    def __init__(self, language: str, custom_dict_file: Optional[str] = None) -> None:
         """コンストラクタ.
 
         Parameters
         ----------
         language : str
-            利用する言語（ja | en | zh）
+            利用する言語（ja）
+        custom_dict_file : Optional[str]
+            カスタム辞書のファイルパス, default None
         """
-        dict_loader = DictLoader(language)
+        dict_loader = DictLoader(language, custom_dict_file)
 
         self.numerical_expr_normalizer = NumericalExpressionNormalizer(dict_loader)
         self.abstime_expr_normalizer = AbstimeExpressionNormalizer(dict_loader)
         self.reltime_expr_normalizer = ReltimeExpressionNormalizer(dict_loader)
         self.duration_expr_normalizer = DurationExpressionNormalizer(dict_loader)
         self.inappropriate_expr_remover = InappropriateExpressionRemover(dict_loader)
```

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/abstime_expr_normalizer.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/abstime_expr_normalizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """絶対時間の抽出・正規化処理を定義するモジュール."""
 from copy import deepcopy
 
 from pynormalizenumexp.expression.abstime import AbstimeExpression, AbstimePattern
 from pynormalizenumexp.expression.base import INF, NNumber, NTime, NumberModifier
-from pynormalizenumexp.utility.dict_loader import DictLoader
+from pynormalizenumexp.utility.dict_loader import DictLoader, EnumExprType
 
 from .base import BaseNormalizer
 from .number_normalizer import NumberNormalizer
 
 
 class AbstimeExpressionNormalizer(BaseNormalizer):
     """絶対時間の抽出・正規化を行うクラス."""
@@ -41,18 +41,20 @@
         prefix_counter_dict_file : str
             接頭表現（単位や年代など）を定義した辞書ファイル名
         prefix_number_modifier_dict_file : str
             接尾表現（範囲表現）を定義した辞書ファイル名
         suffix_number_modifier_dict_file : str
             接尾表現を定義した辞書ファイル名
         """
-        self.limited_expressions = self.dict_loader.load_limited_abstime_expr_dict(limited_expr_dict_file)
-        self.prefix_counters = self.dict_loader.load_limited_abstime_expr_dict(prefix_counter_dict_file)
-        self.prefix_number_modifier = self.dict_loader.load_number_modifier_dict(prefix_number_modifier_dict_file)
-        self.suffix_number_modifier = self.dict_loader.load_number_modifier_dict(suffix_number_modifier_dict_file)
+        self.limited_expressions = self.dict_loader.load_limited_abstime_expr_dict(limited_expr_dict_file, EnumExprType.ABSTIME_LIMITED)
+        self.prefix_counters = self.dict_loader.load_limited_abstime_expr_dict(prefix_counter_dict_file, EnumExprType.ABSTIME_COUNTER)
+        self.prefix_number_modifier = self.dict_loader.load_number_modifier_dict(prefix_number_modifier_dict_file,
+                                                                                 EnumExprType.ABSTIME_PREFIX_MODIFIER)
+        self.suffix_number_modifier = self.dict_loader.load_number_modifier_dict(suffix_number_modifier_dict_file,
+                                                                                 EnumExprType.ABSTIME_SUFFIX_MODIFIER)
 
         self.limited_expression_patterns = self.build_patterns(self.limited_expressions)
         self.prefix_counter_patterns = self.build_patterns(self.prefix_counters)
         self.prefix_number_modifier_patterns = self.build_patterns(self.prefix_number_modifier)
         self.suffix_number_modifier_patterns = self.build_patterns(self.suffix_number_modifier)
 
         for expr in self.limited_expressions:
```

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/base.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/base.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/converter/japanese_number_converter.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/converter/japanese_number_converter.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/converter/number_converter.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/converter/number_converter.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/duration_expr_normalizer.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/duration_expr_normalizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """期間の抽出・正規化処理を定義するモジュール."""
 from copy import deepcopy
 
 from pynormalizenumexp.expression.base import INF, NNumber, NTime, NumberModifier
 from pynormalizenumexp.expression.duration import DurationExpression, DurationPattern
-from pynormalizenumexp.utility.dict_loader import DictLoader
+from pynormalizenumexp.utility.dict_loader import DictLoader, EnumExprType
 
 from .base import BaseNormalizer
 from .number_normalizer import NumberNormalizer
 
 
 class DurationExpressionNormalizer(BaseNormalizer):
     """期間の抽出・正規化を行うクラス."""
@@ -41,18 +41,20 @@
         prefix_counter_dict_file : str
             接頭表現（単位や年代など）を定義した辞書ファイル名
         prefix_number_modifier_dict_file : str
             接尾表現（範囲表現）を定義した辞書ファイル名
         suffix_number_modifier_dict_file : str
             接尾表現を定義した辞書ファイル名
         """
-        self.limited_expressions = self.dict_loader.load_limited_duration_expr_dict(limited_expr_dict_file)
-        self.prefix_counters = self.dict_loader.load_limited_duration_expr_dict(prefix_counter_dict_file)
-        self.prefix_number_modifier = self.dict_loader.load_number_modifier_dict(prefix_number_modifier_dict_file)
-        self.suffix_number_modifier = self.dict_loader.load_number_modifier_dict(suffix_number_modifier_dict_file)
+        self.limited_expressions = self.dict_loader.load_limited_duration_expr_dict(limited_expr_dict_file, EnumExprType.DURATION_LIMITED)
+        self.prefix_counters = self.dict_loader.load_limited_duration_expr_dict(prefix_counter_dict_file, EnumExprType.DURATION_COUNTER)
+        self.prefix_number_modifier = self.dict_loader.load_number_modifier_dict(prefix_number_modifier_dict_file,
+                                                                                 EnumExprType.DURATION_PREFIX_MODIFIER)
+        self.suffix_number_modifier = self.dict_loader.load_number_modifier_dict(suffix_number_modifier_dict_file,
+                                                                                 EnumExprType.DURATION_SUFFIX_MODIFIER)
 
         self.limited_expression_patterns = self.build_patterns(self.limited_expressions)
         self.prefix_counter_patterns = self.build_patterns(self.prefix_counters)
         self.prefix_number_modifier_patterns = self.build_patterns(self.prefix_number_modifier)
         self.suffix_number_modifier_patterns = self.build_patterns(self.suffix_number_modifier)
 
         for expr in self.limited_expressions:
```

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/inappropriate_expr_remover.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/inappropriate_expr_remover.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/number_extractor.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/number_extractor.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/number_normalizer.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/number_normalizer.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/numerical_expr_normalizer.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/numerical_expr_normalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """時間系以外の数値表現の抽出・正規化処理を定義するモジュール."""
 from copy import deepcopy
 
 from pynormalizenumexp.expression.base import INF, NumberModifier
 from pynormalizenumexp.expression.numerical import NumericalExpression, NumericalPattern
-from pynormalizenumexp.utility.dict_loader import DictLoader
+from pynormalizenumexp.utility.dict_loader import DictLoader, EnumExprType
 
 from .base import BaseNormalizer, NNumber
 from .number_normalizer import NumberNormalizer
 
 
 class NumericalExpressionNormalizer(BaseNormalizer):
     """時間系以外の数値表現の抽出・正規化を行うクラス."""
@@ -38,18 +38,20 @@
         prefix_counter_dict_file : str
             接頭表現（単位や年代など）を定義した辞書ファイル名
         prefix_number_modifier_dict_file : str
             接尾表現（範囲表現）を定義した辞書ファイル名
         suffix_number_modifier_dict_file : str
             接尾表現を定義した辞書ファイル名
         """
-        self.limited_expressions = self.dict_loader.load_counter_expr_dict(limited_expr_dict_file)
-        self.prefix_counters = self.dict_loader.load_counter_expr_dict(prefix_counter_dict_file)
-        self.prefix_number_modifier = self.dict_loader.load_number_modifier_dict(prefix_number_modifier_dict_file)
-        self.suffix_number_modifier = self.dict_loader.load_number_modifier_dict(suffix_number_modifier_dict_file)
+        self.limited_expressions = self.dict_loader.load_counter_expr_dict(limited_expr_dict_file, EnumExprType.NUMBER_LIMITED)
+        self.prefix_counters = self.dict_loader.load_counter_expr_dict(prefix_counter_dict_file, EnumExprType.NUMBER_COUNTER)
+        self.prefix_number_modifier = self.dict_loader.load_number_modifier_dict(prefix_number_modifier_dict_file,
+                                                                                 EnumExprType.NUMBER_PREFIX_MODIFIER)
+        self.suffix_number_modifier = self.dict_loader.load_number_modifier_dict(suffix_number_modifier_dict_file,
+                                                                                 EnumExprType.NUMBER_SUFFIX_MODIFIER)
 
         self.limited_expression_patterns = self.build_patterns(self.limited_expressions)
         self.prefix_counter_patterns = self.build_patterns(self.prefix_counters)
         self.prefix_number_modifier_patterns = self.build_patterns(self.prefix_number_modifier)
         self.suffix_number_modifier_patterns = self.build_patterns(self.suffix_number_modifier)
 
         for expr in self.limited_expressions:
```

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/reltime_expr_normalizer.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/reltime_expr_normalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """相対時間の抽出・正規化処理を定義するモジュール."""
 from copy import deepcopy
 
 from pynormalizenumexp.expression.base import INF, NNumber, NTime, NumberModifier
 from pynormalizenumexp.expression.reltime import ReltimeExpression, ReltimePattern
-from pynormalizenumexp.utility.dict_loader import DictLoader
+from pynormalizenumexp.utility.dict_loader import DictLoader, EnumExprType
 
 from .base import BaseNormalizer
 from .number_normalizer import NumberNormalizer
 
 
 class ReltimeExpressionNormalizer(BaseNormalizer):
     """相対時間の抽出・正規化を行うクラス."""
@@ -41,18 +41,20 @@
         prefix_counter_dict_file : str
             接頭表現（単位や年代など）を定義した辞書ファイル名
         prefix_number_modifier_dict_file : str
             接尾表現（範囲表現）を定義した辞書ファイル名
         suffix_number_modifier_dict_file : str
             接尾表現を定義した辞書ファイル名
         """
-        self.limited_expressions = self.dict_loader.load_limited_reltime_expr_dict(limited_expr_dict_file)
-        self.prefix_counters = self.dict_loader.load_limited_reltime_expr_dict(prefix_counter_dict_file)
-        self.prefix_number_modifier = self.dict_loader.load_number_modifier_dict(prefix_number_modifier_dict_file)
-        self.suffix_number_modifier = self.dict_loader.load_number_modifier_dict(suffix_number_modifier_dict_file)
+        self.limited_expressions = self.dict_loader.load_limited_reltime_expr_dict(limited_expr_dict_file, EnumExprType.RELTIME_LIMITED)
+        self.prefix_counters = self.dict_loader.load_limited_reltime_expr_dict(prefix_counter_dict_file, EnumExprType.RELTIME_COUNTER)
+        self.prefix_number_modifier = self.dict_loader.load_number_modifier_dict(prefix_number_modifier_dict_file,
+                                                                                 EnumExprType.RELTIME_PREFIX_MODIFIER)
+        self.suffix_number_modifier = self.dict_loader.load_number_modifier_dict(suffix_number_modifier_dict_file,
+                                                                                 EnumExprType.RELTIME_SUFFIX_MODIFIER)
 
         self.limited_expression_patterns = self.build_patterns(self.limited_expressions)
         self.prefix_counter_patterns = self.build_patterns(self.prefix_counters)
         self.prefix_number_modifier_patterns = self.build_patterns(self.prefix_number_modifier)
         self.suffix_number_modifier_patterns = self.build_patterns(self.suffix_number_modifier)
 
         for expr in self.limited_expressions:
```

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/normalizer/symbol_fixer.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/normalizer/symbol_fixer.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/abstime_expression.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_expression.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/abstime_prefix.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_prefix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/abstime_prefix_counter.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_prefix_counter.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/abstime_suffix.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/abstime_suffix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/chinese_character.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/chinese_character.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/duration_expression.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_expression.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/duration_prefix.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_prefix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/duration_suffix.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/duration_suffix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/num_counter.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_counter.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/num_prefix.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_prefix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/num_prefix_counter.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_prefix_counter.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/num_suffix.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/num_suffix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/reltime_expression.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_expression.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/reltime_prefix.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_prefix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/reltime_prefix_counter.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_prefix_counter.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/resources/dict/ja/reltime_suffix.json` & `pynormalizenumexp-0.3.0/pynormalizenumexp/resources/dict/ja/reltime_suffix.json`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/utility/custom_type.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/utility/custom_type.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/utility/dict_loader.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/utility/normalizer_utility.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,217 +1,208 @@
-"""辞書ファイルの読み込み定義モジュール."""
-import json
-import os
-from dataclasses import dataclass
-from importlib.resources import files
+"""正規化・補正処理における共通処理を定義モジュール."""
+import re
+from typing import Optional, Tuple
 
-import pynormalizenumexp
-from pynormalizenumexp.expression.abstime import AbstimePattern
-from pynormalizenumexp.expression.base import NumberModifier
-from pynormalizenumexp.expression.duration import DurationPattern
-from pynormalizenumexp.expression.numerical import NumericalPattern
-from pynormalizenumexp.expression.reltime import ReltimePattern
+from pynormalizenumexp.expression.base import INF, PLACE_HOLDER, NNumber, NTime
 
-from .custom_type import (AbstimePatternDict, ChineseCharacterDict, DurationPatternDict, InappropriateStringDict, NumberModifierDict,
-                          NumericalPatternDict, ReltimePatternDict)
 
-BASE_DICT_PKG = "resources.dict"
+class NormalizerUtility(object):
+    """正規化・補正処理における共通処理のクラス."""
 
-
-@dataclass
-class ChineseCharacter:
-    """漢数字用クラス."""
-
-    character: str
-    value: int
-    notation_type: str
-
-
-class DictLoader(object):
-    """辞書ファイルの読み込み定義クラス."""
-
-    def __init__(self, language: str) -> None:
-        """コンストラクタ.
+    def replace_numbers_in_text(self, text: str, numbers: list[NNumber]) -> str:
+        """テキスト中の数値表現をPlaceholderに置換する.
 
         Parameters
         ----------
-        language : str
-            利用言語（ja | en）
+        text : str
+            置換対象のテキスト
+        numbers : list[NNumber]
+            数値表現
+
+        Returns
+        -------
+        str
+            置換後のテキスト
         """
-        # TODO ja, en, zh以外はエラーになるようにする
-        self.language = language
-        self.resouce_dirpath = files(f'{pynormalizenumexp.__package__}.{BASE_DICT_PKG}.{self.language}')
+        # 数値表現の開始・終了位置をもとに置換するため、テキストをリスト（要素は各文字）にする
+        new_text_list = list(text)
+        for number in numbers:
+            new_text_list[number.position_start:number.position_end] = \
+                [PLACE_HOLDER] * (number.position_end - number.position_start)
+
+        return "".join(new_text_list)
 
-    def load_chinese_character_dict(self, dict_file: str) -> list[ChineseCharacter]:
-        """漢数字辞書の読み込み.
+    def shorten_place_holder_in_text(self, text: str) -> str:
+        """連続するPlaceholderを縮約する.
 
         Parameters
         ----------
-        dict_file : str
-            辞書ファイル名
+        text : str
+            縮約対象のテキスト
 
         Returns
         -------
-        list[ChineseCharacter]
-            漢数字情報のリスト
-        """
-        with open(os.path.join(self.resouce_dirpath, dict_file)) as fp:
-            characters: list[ChineseCharacterDict] = json.load(fp)["characters"]
-            load_target = [ChineseCharacter(character=char["character"], value=char["value"],
-                                            notation_type=char["notation_type"]) for char in characters]
+        str
+            縮約後のテキスト
 
-        return load_target
+        Notes
+        -----
+            「****年*月」 -> 「*年*月」のように数の部分を縮約する
+        """
+        return re.sub(f"[{PLACE_HOLDER}]{{2,}}", PLACE_HOLDER, text, flags=re.DOTALL)
 
-    def load_counter_expr_dict(self, dict_file: str) -> list[NumericalPattern]:
-        """時間系以外のパターン辞書の読み込み.
+    def search_pattern(self, text: str, patterns: dict[str, int], search_type: str) -> int:
+        """patternsの中から、テキストのprefix/suffixになっているものを探索する.
 
         Parameters
         ----------
-        dict_file : str
-            辞書ファイル名
+        text : str
+            探索対象のテキスト
+        patterns : dict[str, int]
+            パターン情報（Key：パターン文字列、Value：パターンID）
+        search_type : str
+            先頭から見るprefixか末尾から見るsuffixか
 
         Returns
         -------
-        list[NumericalPattern]
-            時間系以外のパターン情報のリスト
+        int
+            マッチしたパターンID
+
+        Notes
+        -----
+            複数パターンがある場合はテキストのprefix/suffixが最長一致するものを採用する
         """
-        def make_expression(pattern: NumericalPatternDict) -> NumericalPattern:
-            expr = NumericalPattern()
-            expr.pattern = pattern["pattern"]
-            expr.counter = pattern["counter"]
-            expr.si_prefix = pattern["SI_prefix"]
-            expr.optional_power_of_ten = pattern["optional_power_of_ten"]
-            expr.ordinary = pattern["ordinary"]
-            expr.option = pattern["option"]
+        shortened_text = self.shorten_place_holder_in_text(text)
+        if search_type == "prefix":
+            match_patterns = [(p_str, p_id) for p_str, p_id in patterns.items() if shortened_text.startswith(p_str)]
+        elif search_type == "suffix":
+            match_patterns = [(p_str, p_id) for p_str, p_id in patterns.items() if shortened_text.endswith(p_str)]
+        else:
+            raise ValueError(f'Invalid search_type: "{search_type}"')
 
-            return expr
+        fixed_pattern: Optional[Tuple[str, int]] = None
+        for pattern in match_patterns:
+            if fixed_pattern is None or len(pattern[0]) > len(fixed_pattern[0]):
+                fixed_pattern = pattern
 
-        with open(os.path.join(self.resouce_dirpath, dict_file)) as fp:
-            patterns: list[NumericalPatternDict] = json.load(fp)["patterns"]
-            load_target = [make_expression(pattern) for pattern in patterns]
+        if fixed_pattern is not None:
+            return fixed_pattern[1]
 
-        return load_target
+        return -1
 
-    def load_limited_abstime_expr_dict(self, dict_file: str) -> list[AbstimePattern]:
-        """絶対時間のパターン辞書の読み込み.
+    def search_prefix_number_modifier(self, text: str, expr_position_start: int, patterns: dict[str, int]) -> int:
+        """数値表現の前に来る修飾表現を検索する.
 
         Parameters
         ----------
-        dict_file : str
-            辞書ファイル名
+        text : str
+            検索対象のテキスト
+        expr_position_start : int
+            数値表現の開始位置
+        patterns : dict[str, int]
+            修飾表現パターン
 
         Returns
         -------
-        list[AbstimePattern]
-            絶対時間のパターン情報のリスト
-        """
-        def make_expression(pattern: AbstimePatternDict) -> AbstimePattern:
-            expr = AbstimePattern()
-            expr.pattern = pattern["pattern"]
-            expr.corresponding_time_position = pattern["corresponding_time_position"]
-            expr.process_type = pattern["process_type"]
-            expr.ordinary = pattern["ordinary"]
-            expr.option = pattern["option"]
+        int
+            マッチした修飾表現パターンのID
 
-            return expr
-
-        with open(os.path.join(self.resouce_dirpath, dict_file)) as fp:
-            patterns: list[AbstimePatternDict] = json.load(fp)["patterns"]
-            load_target = [make_expression(pattern) for pattern in patterns]
+        Notes
+        -----
+            数値表現の直前から探していくので、search_patternにはsuffixを指定している
+        """
+        before_text = text[:expr_position_start]
 
-        return load_target
+        # 「コンビニで$100を払った」の場合、「100」が数値表現になるので「コンビニで$」を末尾から見ていく
+        # -> 「$」が修飾表現に該当する
+        return self.search_pattern(before_text, patterns, "suffix")
 
-    def load_limited_reltime_expr_dict(self, dict_file: str) -> list[ReltimePattern]:
-        """相対時間のパターン辞書の読み込み.
+    def search_suffix_number_modifier(self, text: str, expr_position_end: int, patterns: dict[str, int]) -> int:
+        """数値表現の後に来る修飾表現を検索する.
 
         Parameters
         ----------
-        dict_file : str
-            辞書ファイル名
+        text : str
+            検索対象のテキスト
+        expr_position_end : int
+            数値表現の終了位置
+        patterns : dict[str, int]
+            修飾表現パターン
 
         Returns
         -------
-        list[ReltimePattern]
-            相対時間のパターン情報のリスト
-        """
-        def make_expression(pattern: ReltimePatternDict) -> ReltimePattern:
-            expr = ReltimePattern()
-            expr.pattern = pattern["pattern"]
-            expr.corresponding_time_position = pattern["corresponding_time_position"]
-            expr.process_type = pattern["process_type"]
-            expr.ordinary = pattern["ordinary"]
-            expr.option = pattern["option"]
+        int
+            マッチした修飾表現パターンのID
 
-            return expr
-
-        with open(os.path.join(self.resouce_dirpath, dict_file)) as fp:
-            patterns: list[AbstimePatternDict] = json.load(fp)["patterns"]
-            load_target = [make_expression(pattern) for pattern in patterns]
+        Notes
+        -----
+            数値表現の直後から探していくので、search_patternにはprefixを指定している
+        """
+        after_text = text[expr_position_end:]
 
-        return load_target
+        return self.search_pattern(after_text, patterns, "prefix")
 
-    def load_limited_duration_expr_dict(self, dict_file: str) -> list[DurationPattern]:
-        """期間のパターン辞書の読み込み.
+    def is_finite(self, value: float) -> bool:
+        """与えられた数値が正負の無限大でないかどうかを判定する.
 
         Parameters
         ----------
-        dict_file : str
-            辞書ファイル名
+        value : float
+            判定対象の数値
 
         Returns
         -------
-        list[DurationPattern]
-            期間のパターン情報のリスト
+        bool
+            判定結果（True：正負の無限大でない、False：正負の無限大である）
         """
-        def make_expression(pattern: DurationPatternDict) -> DurationPattern:
-            expr = DurationPattern()
-            expr.pattern = pattern["pattern"]
-            expr.corresponding_time_position = pattern["corresponding_time_position"]
-            expr.process_type = pattern["process_type"]
-            expr.ordinary = pattern["ordinary"]
-            expr.option = pattern["option"]
-
-            return expr
+        return value != INF and value != -INF
 
-        with open(os.path.join(self.resouce_dirpath, dict_file)) as fp:
-            patterns: list[AbstimePatternDict] = json.load(fp)["patterns"]
-            load_target = [make_expression(pattern) for pattern in patterns]
-
-        return load_target
-
-    def load_number_modifier_dict(self, dict_file: str) -> list[NumberModifier]:
-        """各種表現のprefix/suffixパターン辞書の読み込み.
+    def is_null_time(self, time: NTime) -> bool:
+        """与えられた時間オブジェクトがNullかどうかを判定する.
 
         Parameters
         ----------
-        dict_file : str
-            辞書ファイル名
+        time : NTime
+            判定対象の時間オブジェクト
 
         Returns
         -------
-        list[NumberModifier]
-            各種表現のprefix/suffixパターン情報のリスト
-        """
-        with open(os.path.join(self.resouce_dirpath, dict_file)) as fp:
-            patterns: list[NumberModifierDict] = json.load(fp)["patterns"]
-            load_target = [NumberModifier(pattern["pattern"], pattern["process_type"]) for pattern in patterns]
+        bool
+            判定結果（True：Nullである、False：Nullでない）
 
-        return load_target
+        Notes
+        -----
+            Nullの場合はNTimeのすべての属性がINFまたは-INFになっている
+        """
+        return time == NTime(INF) or time == NTime(-INF)
 
-    def load_inappropriate_strings_dict(self, dict_file: str) -> list[str]:
-        """不適切な数値表現パターン辞書の読み込み.
+    def identify_time_detail(self, time: NTime) -> str:
+        """与えられた時間オブジェクトがどの単位のものかを判定する.
 
         Parameters
         ----------
-        dict_file : str
-            辞書ファイル名
+        time : NTime
+            判定対象の時間オブジェクト
 
         Returns
         -------
-        list[str]
-            不適切な数値表現の文字列
-        """
-        with open(os.path.join(self.resouce_dirpath, dict_file)) as fp:
-            strings: list[InappropriateStringDict] = json.load(fp)["strings"]
-            load_target = [string["str"] for string in strings]
+        str
+            単位を表す文字列
 
-        return load_target
+        Notes
+        -----
+            s: 秒、mn: 分、h: 時、d: 日、m: 月、 y: 年
+        """
+        if self.is_finite(time.second):
+            return "s"
+        elif self.is_finite(time.minute):
+            return "mn"
+        elif self.is_finite(time.hour):
+            return "h"
+        elif self.is_finite(time.day):
+            return "d"
+        elif self.is_finite(time.month):
+            return "m"
+        elif self.is_finite(time.year):
+            return "y"
+        else:
+            return ""
```

### Comparing `pynormalizenumexp-0.2.1/pynormalizenumexp/utility/digit_utility.py` & `pynormalizenumexp-0.3.0/pynormalizenumexp/utility/digit_utility.py`

 * *Files identical despite different names*

### Comparing `pynormalizenumexp-0.2.1/pyproject.toml` & `pynormalizenumexp-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynormalizenumexp"
-version = "0.2.1"
+version = "0.3.0"
 description = "NormalizeNumExp for Python"
 authors = ["tkscode"]
 license = "BSD 3-Clause"
 readme = "README.md"
 repository = "https://github.com/tkscode/pyNormalizeNumExp"
 homepage = "https://github.com/tkscode/pyNormalizeNumExp"
 keywords = ["Python", "NLP", "NormalizeNumExp"]
```

### Comparing `pynormalizenumexp-0.2.1/PKG-INFO` & `pynormalizenumexp-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,22 @@
-Metadata-Version: 2.1
-Name: pynormalizenumexp
-Version: 0.2.1
-Summary: NormalizeNumExp for Python
-Home-page: https://github.com/tkscode/pyNormalizeNumExp
-License: BSD 3-Clause
-Keywords: Python,NLP,NormalizeNumExp
-Author: tkscode
-Requires-Python: >=3.9,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Project-URL: Repository, https://github.com/tkscode/pyNormalizeNumExp
-Description-Content-Type: text/markdown
-
 [![PyPI version](https://badge.fury.io/py/pynormalizenumexp.svg)](https://badge.fury.io/py/pynormalizenumexp)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pynormalizenumexp.svg)](https://pypi.org/project/pynormalizenumexp/)
 [![pytest](https://github.com/tkscode/pyNormalizeNumExp/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/tkscode/pyNormalizeNumExp/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/tkscode/pyNormalizeNumExp/branch/main/graph/badge.svg?token=3Z0YIZV5U1)](https://codecov.io/gh/tkscode/pyNormalizeNumExp)
 
 
 # pyNormalizeNumexp
 
 数量表現や時間表現の抽出・正規化を行う[NormalizeNumexp](https://www.cl.ecei.tohoku.ac.jp/Open_Resources-normalizeNumexp.html)のPython実装です。  
 本家でもSWIGによるPythonバインディングが提供されていますが、NormalizeNumexp本体のインストールでトラブルに遭うことが多いため、全実装をPythonに移植しました。
 
 
 ## Prerequisites
 
-Python >=3.9, <=3.12
+Python `>=3.9`, `<=3.12`
 
 
 ## Installation
 
 ```
 pip install pynormalizenumexp
 ```
@@ -50,20 +32,20 @@
 results = normalizer.normalize("魔女狩りは15世紀～18世紀にかけてみられ、全ヨーロッパで4万人が処刑された", as_dict=True)
 for r in results:
 	print(r)
 # {'type': 'abstime', 'original_expr': '15世紀～18世紀', 'position_start': 5, 'position_end': 14, 'counter': 'none', 'value_lower_bound': {'year': 1401, 'month': inf, 'day': inf, 'hour': inf, 'minute': inf, 'second': inf}, 'value_upper_bound': {'year': 1800, 'month': -inf, 'day': -inf, 'hour': -inf, 'minute': -inf, 'second': -inf}, 'value_lower_bound_abs': None, 'value_upper_bound_abs': None, 'value_lower_bound_rel': None, 'value_upper_bound_rel': None, 'options': []}
 # {'type': 'numerical', 'original_expr': '4万人', 'position_start': 29, 'position_end': 32, 'counter': '人', 'value_lower_bound': 40000, 'value_upper_bound': 40000, 'value_lower_bound_abs': None, 'value_upper_bound_abs': None, 'value_lower_bound_rel': None, 'value_upper_bound_rel': None, 'options': []}
 ```
 
-+ `NormalizeNumexp`クラスの引数に言語識別子を指定します（例：日本語であれば`ja`）
-	+ 本家では英語`en`や中国語`zh`にも対応していますが、本ライブラリでは日本語のみに対応しています（将来的には英語・中国語も入れる予定です）
-+ `NormalizeNumexp`クラスの`normalize`関数に抽出・正規化対象のテキストを指定します
-	+ `as_dict`引数に`True`を指定することで、返り値の数量・時間表現のオブジェクトが`dict`型になります
-		+ 数量・時間表現のオブジェクトの属性については[`Expression`](./pynormalizenumexp/normalize_numexp.py#L19)クラスを参照してください
-+ 返り値が`dict`型の場合のデータ構造は以下の通りです
++ `NormalizeNumexp`クラスの引数に言語識別子を指定します。（例：日本語であれば`ja`）
+	+ 本家では英語`en`や中国語`zh`にも対応していますが、本ライブラリでは日本語のみに対応しています。（将来的には英語・中国語も入れる予定です）
++ `NormalizeNumexp`クラスの`normalize`関数に抽出・正規化対象のテキストを指定します。
+	+ `as_dict`引数に`True`を指定することで、返り値の数量・時間表現のオブジェクトが`dict`型になります。
+		+ 数量・時間表現のオブジェクトの属性については[`Expression`](./pynormalizenumexp/normalize_numexp.py#L19)クラスを参照してください。
++ 返り値が`dict`型の場合のデータ構造は以下の通りです。
 	```python
 	{
 		"type": str, # 表現種別（numerical：数量、abstime：絶対時間、reltime：相対時間、duration：期間）
 		"original_expr": str, # 数値・時間表現の文字列
 		"position_start": int, # 抽出元テキストにおける開始位置
 		"position_end": int, # 抽出元テキストにおける終了位置
 		"counter": str, # 「人」や「匹」などの単位（typeがnumerical以外の場合は "none" になる）
@@ -72,34 +54,48 @@
 		"value_lower_bound_abs": None | Dict[str, int | float], # ※2
 		"value_upper_bound_abs": None | Dict[str, int | float], # ※2
 		"value_lower_bound_rel": None | Dict[str, int | float], # ※3
 		"value_upper_bound_rel": None | Dict[str, int | float], # ※3
 		"options": List[str]
 	}
 	```
-	+ ※1：数量・時間表現の下限値（lower）・上限値（upper）が入るが、`type`によって値の種類が変化する
+	+ ※1：数量・時間表現の下限値（lower）・上限値（upper）が入るが、`type`によって値の種類が変化します。
 		+ `numerical`の場合：`int`または`float`
 			+ 例：`15.3ポイント`の場合は下限・上限ともに`15.3`
 			+ 例：`1～2人`の場合は下限が`1`、上限が`2`
 		+ `abstime`または`duration`の場合：`Dict[str, int | float]`
-			+ 例：`2021年1月1日`の場合は下限・上限ともに`{"year": 2021, "month": 1, "day": 1}`となる（`hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になる）
-			+ 例：`3/3～3/5`の場合は下限が`{"month": 3, "day": 3}`、上限が`{"month": 3, "day": 5}`となる（`year`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になる）
-			+ 例：`100年間`の場合は下限・上限ともに`{"year": 100}`となる（`month`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になる）
+			+ 例：`2021年1月1日`の場合は下限・上限ともに`{"year": 2021, "month": 1, "day": 1}`（`hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になります）
+			+ 例：`3/3～3/5`の場合は下限が`{"month": 3, "day": 3}`、上限が`{"month": 3, "day": 5}`（`year`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になります）
+			+ 例：`100年間`の場合は下限・上限ともに`{"year": 100}`（`month`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になります）
 		+ `reltime`の場合：`None`
-	+ ※2：`type`が`reltime`の場合に絶対時間表現の下限値（lower）・上限値（upper）が入る（その他の`type`の場合は`None`になる）
-		+ 例：`昨年3月`の場合は下限・上限ともに`{"month": 3}`となる（`year`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になる）
-	+ ※3：`type`が`reltime`の場合に相対時間表現の下限値（lower）・上限値（upper）が入る（その他の`type`の場合は`None`になる）
-		+ 例：`昨年3月`の場合は下限・上限ともに`{"year": -1}`となる（`month`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になる）
-		+ 例：`15年前`の場合下限・上限ともに`{"year": -15}`となる（`month`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になる）
+	+ ※2：`type`が`reltime`の場合に絶対時間表現の下限値（lower）・上限値（upper）が入ります。（その他の`type`の場合は`None`になります）
+		+ 例：`昨年3月`の場合は下限・上限ともに`{"month": 3}`（`year`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になります）
+	+ ※3：`type`が`reltime`の場合に相対時間表現の下限値（lower）・上限値（upper）が入ります。（その他の`type`の場合は`None`になります）
+		+ 例：`昨年3月`の場合は下限・上限ともに`{"year": -1}`（`month`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になります）
+		+ 例：`15年前`の場合下限・上限ともに`{"year": -15}`（`month`, `day`, `hour`, `minute`, `second`は該当する情報がないので`inf`または`-inf`になります）
+
+### 抽出する数値表現パターンを追加したい場合
+
+[予め用意した辞書](./pynormalizenumexp/resources/dict/ja/)に定義されていないパターンの数値表現を抽出したい場合、カスタム辞書ファイルを別途定義して読み込ませることができます。
+
+任意のディレクトリにJSON形式の辞書ファイル（以下の例では`/path/to/custom_dict.json`）を定義し、`NormalizeNumexp`クラスの第2引数に辞書ファイルのパスを指定することで反映することができます。  
+辞書の作り方については[こちら](./pynormalizenumexp/resources/dict/README.md)を参照してください。
+```python
+from pynormalizenumexp.normalize_numexp import NormalizeNumexp
+
+normalizer = NormalizeNumexp("ja", "/path/to/custom_dict.json")
+
+results = normalizer.normalize("メールに2ファイル添付する", as_dict=True)
+```
+
 
 ## 免責事項
 
 + 本ライブラリの作成にあたり、単体テスト等で動作確認はしていますが、ケースによっては期待通りの振る舞いをしない可能性があります
 + 本ライブラリの利用により、万一、利用者に何らかの不都合や損害が発生したとしても、作者は何らの責任を負うものではありません
 
 
 ## Special thanks
 
 + [東北大学 乾・鈴木研究室](https://www.cl.ecei.tohoku.ac.jp/Open_Resources-normalizeNumexp.html)
 + [nullnull/normalizeNumexp](https://github.com/nullnull/normalizeNumexp)（本家実装）
 + [cotogoto/normalize-numexp](https://github.com/cotogoto/normalize-numexp)（Java移植版）
-
```

