# Comparing `tmp/cnfc-0.5.0.tar.gz` & `tmp/cnfc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnfc-0.5.0.tar", max compression
+gzip compressed data, was "cnfc-0.6.0.tar", max compression
```

## Comparing `cnfc-0.5.0.tar` & `cnfc-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1211 2023-07-15 12:36:58.873252 cnfc-0.5.0/LICENSE
--rw-r--r--   0        0        0     6360 2023-11-10 22:39:52.133682 cnfc-0.5.0/README.md
--rw-r--r--   0        0        0       44 2023-10-18 22:31:32.653663 cnfc-0.5.0/cnfc/__init__.py
--rw-r--r--   0        0        0      788 2023-10-15 13:16:51.732378 cnfc-0.5.0/cnfc/bool_lit.py
--rw-r--r--   0        0        0     3195 2023-10-24 12:23:15.758652 cnfc-0.5.0/cnfc/buffer.py
--rw-r--r--   0        0        0      561 2023-08-02 11:53:20.261023 cnfc-0.5.0/cnfc/cache.py
--rw-r--r--   0        0        0     4257 2023-10-09 14:05:25.470515 cnfc-0.5.0/cnfc/cardinality.py
--rw-r--r--   0        0        0     1856 2023-10-15 13:07:16.093383 cnfc-0.5.0/cnfc/expr.py
--rw-r--r--   0        0        0     2163 2023-09-29 11:41:02.667371 cnfc-0.5.0/cnfc/extractor.py
--rw-r--r--   0        0        0     2634 2023-11-10 22:55:23.966674 cnfc-0.5.0/cnfc/formula.py
--rw-r--r--   0        0        0      318 2023-11-08 13:00:34.235130 cnfc-0.5.0/cnfc/log.py
--rw-r--r--   0        0        0    14735 2023-11-10 13:13:06.489666 cnfc-0.5.0/cnfc/model.py
--rw-r--r--   0        0        0    14812 2023-10-14 17:27:21.357433 cnfc-0.5.0/cnfc/regex.py
--rw-r--r--   0        0        0     4957 2023-11-08 13:00:56.203130 cnfc-0.5.0/cnfc/simplify.py
--rw-r--r--   0        0        0      766 2023-10-09 14:09:41.613513 cnfc-0.5.0/cnfc/tseytin.py
--rw-r--r--   0        0        0     5162 2023-11-06 12:34:32.730472 cnfc-0.5.0/cnfc/tuples.py
--rw-r--r--   0        0        0      687 2023-10-20 11:46:58.788746 cnfc-0.5.0/cnfc/util.py
--rw-r--r--   0        0        0      311 2023-11-11 14:06:50.458493 cnfc-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6837 1970-01-01 00:00:00.000000 cnfc-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-15 12:36:58.873252 cnfc-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6907 2024-04-28 14:57:16.078586 cnfc-0.6.0/README.md
+-rw-r--r--   0        0        0       44 2023-10-18 22:31:32.653663 cnfc-0.6.0/cnfc/__init__.py
+-rw-r--r--   0        0        0      788 2023-10-15 13:16:51.732378 cnfc-0.6.0/cnfc/bool_lit.py
+-rw-r--r--   0        0        0     3195 2023-10-24 12:23:15.758652 cnfc-0.6.0/cnfc/buffer.py
+-rw-r--r--   0        0        0      561 2023-08-02 11:53:20.261023 cnfc-0.6.0/cnfc/cache.py
+-rw-r--r--   0        0        0     4257 2023-10-09 14:05:25.470515 cnfc-0.6.0/cnfc/cardinality.py
+-rw-r--r--   0        0        0     1856 2023-10-15 13:07:16.093383 cnfc-0.6.0/cnfc/expr.py
+-rw-r--r--   0        0        0     2163 2023-09-29 11:41:02.667371 cnfc-0.6.0/cnfc/extractor.py
+-rw-r--r--   0        0        0     2634 2023-11-10 22:55:23.966674 cnfc-0.6.0/cnfc/formula.py
+-rw-r--r--   0        0        0      318 2023-11-08 13:00:34.235130 cnfc-0.6.0/cnfc/log.py
+-rw-r--r--   0        0        0    15459 2024-04-28 14:56:10.548587 cnfc-0.6.0/cnfc/model.py
+-rw-r--r--   0        0        0    14812 2023-10-14 17:27:21.357433 cnfc-0.6.0/cnfc/regex.py
+-rw-r--r--   0        0        0     4957 2023-11-08 13:00:56.203130 cnfc-0.6.0/cnfc/simplify.py
+-rw-r--r--   0        0        0      766 2023-10-09 14:09:41.613513 cnfc-0.6.0/cnfc/tseytin.py
+-rw-r--r--   0        0        0     5162 2023-11-06 12:34:32.730472 cnfc-0.6.0/cnfc/tuples.py
+-rw-r--r--   0        0        0      687 2023-10-20 11:46:58.788746 cnfc-0.6.0/cnfc/util.py
+-rw-r--r--   0        0        0      311 2024-04-28 14:59:58.590585 cnfc-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7384 1970-01-01 00:00:00.000000 cnfc-0.6.0/PKG-INFO
```

### Comparing `cnfc-0.5.0/LICENSE` & `cnfc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cnfc-0.5.0/README.md` & `cnfc-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: cnfc
+Version: 0.6.0
+Summary: A DIMACS CNF compiler
+License: Unlicense
+Author: Aaron Windsor
+Author-email: aaron.windsor@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
 # cnfc
 
 A [CNF](https://en.wikipedia.org/wiki/Conjunctive_normal_form) compiler that generates
 compact DIMACS CNF encodings from higher-level primitives in Python. DIMACS CNF is
 the input format accepted by most SAT solvers.
 
 In contrast to optimization libraries like Z3, PySAT or ortools that provide both
@@ -153,31 +168,39 @@
 UNSATISFIABLE
 ```
 
 instead of a schedule, which tells us that there's no assignment of people to shifts that satisfies all of the criteria we've laid out.
 
 A [runnable version of this script](examples/scheduling) is in the [examples subdirectory](examples) of this repository.
 
-Installation
-============
+## Features
+
+Arbitrary clauses can be built, composed, and added to formulas with:
+
+   * Familiar boolean operators `And`, `Or`, `Not`, `If`, `Eq`, `Neq`.
+   * `Tuple`s that can be compared for equality, inequality, or lexicographic order.
+   * `Integer`s that can be added, multiplied, or compared as `Tuple`s (see [examples/prime](examples/prime)).
+   * `NumTrue` and `NumFalse` for cardinality constraints (see [examples/nqueens](examples/nqueens)).
+   * `RegexMatch` to apply binary regular expressions to `Tuple`s (see [examples/nonagram](examples/nonagram)).
+
+## Installation
 
 cnfc is tested on [these versions](https://github.com/aaw/cnfc/blob/master/.github/workflows/python-package.yml#L19) of Python 3. To install
 the latest stable release of cnfc, run:
 
 ```
 pip install cnfc
 ```
 
-Development
-===========
+## Development
 
 Install [poetry](https://python-poetry.org/docs/#installation) and run `poetry install`. Then you can bring up a shell, etc. Run tests with:
 
 ```
 poetry run python3 -m unittest discover
 ```
 
 To release a new version to PyPI, bump the version in `pyproject.toml` and run:
 
 ```
 poetry publish --build --username=__token__ --password=$PYPI_TOKEN
-```
+```
```

### Comparing `cnfc-0.5.0/cnfc/bool_lit.py` & `cnfc-0.6.0/cnfc/bool_lit.py`

 * *Files identical despite different names*

### Comparing `cnfc-0.5.0/cnfc/buffer.py` & `cnfc-0.6.0/cnfc/buffer.py`

 * *Files identical despite different names*

### Comparing `cnfc-0.5.0/cnfc/cache.py` & `cnfc-0.6.0/cnfc/cache.py`

 * *Files identical despite different names*

### Comparing `cnfc-0.5.0/cnfc/cardinality.py` & `cnfc-0.6.0/cnfc/cardinality.py`

 * *Files identical despite different names*

### Comparing `cnfc-0.5.0/cnfc/expr.py` & `cnfc-0.6.0/cnfc/expr.py`

 * *Files identical despite different names*

### Comparing `cnfc-0.5.0/cnfc/extractor.py` & `cnfc-0.6.0/cnfc/extractor.py`

 * *Files identical despite different names*

### Comparing `cnfc-0.5.0/cnfc/formula.py` & `cnfc-0.6.0/cnfc/formula.py`

 * *Files identical despite different names*

### Comparing `cnfc-0.5.0/cnfc/model.py` & `cnfc-0.6.0/cnfc/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 class OrderedBinaryBoolExpr(BoolExpr):
     def __init__(self, first, second):
         self.first, self.second = first, second
 
     def __repr__(self):
         return '{}({},{})'.format(self.__class__.__name__, self.first, self.second)
 
-class Implies(OrderedBinaryBoolExpr):
+class If(OrderedBinaryBoolExpr):
     def generate_var(self, formula):
         return Or(Not(self.first), self.second).generate_var(formula)
 
     def generate_cnf(self, formula):
         fv = self.first.generate_var(formula)
         sv = self.second.generate_var(formula)
         yield (~fv, sv)
@@ -275,64 +275,75 @@
         if isinstance(self.first, NumTrue):
             yield from at_least_n_true(formula, vars, self.second)
         elif isinstance(self.first, NumFalse):
             yield from at_most_n_true(formula, vars, len(vars) - self.second)
         else:
             raise ValueError("Only NumTrue and NumFalse are supported.")
 
-class TupleEq(OrderedBinaryBoolExpr):
+class OrderedBinaryTupleBoolExpr(BoolExpr):
+    def __init__(self, first, second):
+        self.first, self.second = first, second
+        if isinstance(self.first, int):
+            self.first = Integer(self.first)
+        if isinstance(self.second, int):
+            self.second = Integer(self.second)
+
+    def __repr__(self):
+        return '{}({},{})'.format(self.__class__.__name__, self.first, self.second)
+
+class TupleEq(OrderedBinaryTupleBoolExpr):
     def generate_var(self, formula):
         return generate_var_from_cnf(self, formula)
 
     def generate_cnf(self, formula):
         t1 = self.first.evaluate(formula)
         t2 = self.second.evaluate(formula)
         t1 = lpad(t1, len(t2) - len(t1))
         t2 = lpad(t2, len(t1) - len(t2))
         yield from And(*(Eq(c1, c2) for c1, c2 in zip(t1, t2))).generate_cnf(formula)
 
-class TupleNeq(OrderedBinaryBoolExpr):
+class TupleNeq(OrderedBinaryTupleBoolExpr):
     def generate_var(self, formula):
         return generate_var_from_cnf(self, formula)
 
     def generate_cnf(self, formula):
         t1 = self.first.evaluate(formula)
         t2 = self.second.evaluate(formula)
         t1 = lpad(t1, len(t2) - len(t1))
         t2 = lpad(t2, len(t1) - len(t2))
         yield from Or(*(Neq(c1, c2) for c1, c2 in zip(t1, t2))).generate_cnf(formula)
 
-class TupleLt(OrderedBinaryBoolExpr):
+class TupleLt(OrderedBinaryTupleBoolExpr):
     def generate_var(self, formula):
         return generate_var_from_cnf(self, formula)
 
     def generate_cnf(self, formula):
         t1 = self.first.evaluate(formula)
         t2 = self.second.evaluate(formula)
         yield from tuple_less_than(formula, t1, t2, strict=True)
 
-class TupleLe(OrderedBinaryBoolExpr):
+class TupleLe(OrderedBinaryTupleBoolExpr):
     def generate_var(self, formula):
         return generate_var_from_cnf(self, formula)
 
     def generate_cnf(self, formula):
         t1 = self.first.evaluate(formula)
         t2 = self.second.evaluate(formula)
         yield from tuple_less_than(formula, t1, t2, strict=False)
 
-class TupleGt(OrderedBinaryBoolExpr):
+class TupleGt(OrderedBinaryTupleBoolExpr):
     def generate_var(self, formula):
         return generate_var_from_cnf(self, formula)
 
     def generate_cnf(self, formula):
         t1 = self.first.evaluate(formula)
         t2 = self.second.evaluate(formula)
         yield from tuple_less_than(formula, t2, t1, strict=True)
 
-class TupleGe(OrderedBinaryBoolExpr):
+class TupleGe(OrderedBinaryTupleBoolExpr):
     def generate_var(self, formula):
         return generate_var_from_cnf(self, formula)
 
     def generate_cnf(self, formula):
         t1 = self.first.evaluate(formula)
         t2 = self.second.evaluate(formula)
         yield from tuple_less_than(formula, t2, t1, strict=False)
@@ -356,24 +367,34 @@
 
     def __gt__(self, other: 'TupleExpr'):
         return TupleGt(self, other)
 
     def __ge__(self, other: 'TupleExpr'):
         return TupleGe(self, other)
 
-    def __add__(self, other: 'TupleExpr'):
+    def __add__(self, other):
+        return TupleAdd(self, other)
+
+    def __radd__(self, other):
         return TupleAdd(self, other)
 
-    def __mul__(self, other: 'TupleExpr'):
+    def __mul__(self, other):
+        return TupleMul(self, other)
+
+    def __rmul__(self, other):
         return TupleMul(self, other)
 
 # An expression combining two Tuples (addition, multiplication) that results in a Tuple
 class TupleCompositeExpr(TupleExpr):
     def __init__(self, first, second):
         self.first, self.second = first, second
+        if isinstance(self.first, int):
+            self.first = Integer(self.first)
+        if isinstance(self.second, int):
+            self.second = Integer(self.second)
         # TODO: dummy exprs to make asserts work, fix later when we don't do these asserts any more
         self.exprs = [None]*(len(self.first))
 
     def __repr__(self):
         return '{}({},{})'.format(self.__class__.__name__, self.first, self.second)
 
 class TupleAdd(TupleCompositeExpr):
```

### Comparing `cnfc-0.5.0/cnfc/regex.py` & `cnfc-0.6.0/cnfc/regex.py`

 * *Files identical despite different names*

### Comparing `cnfc-0.5.0/cnfc/simplify.py` & `cnfc-0.6.0/cnfc/simplify.py`

 * *Files identical despite different names*

### Comparing `cnfc-0.5.0/cnfc/tseytin.py` & `cnfc-0.6.0/cnfc/tseytin.py`

 * *Files identical despite different names*

### Comparing `cnfc-0.5.0/cnfc/tuples.py` & `cnfc-0.6.0/cnfc/tuples.py`

 * *Files identical despite different names*

### Comparing `cnfc-0.5.0/cnfc/util.py` & `cnfc-0.6.0/cnfc/util.py`

 * *Files identical despite different names*

### Comparing `cnfc-0.5.0/PKG-INFO` & `cnfc-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: cnfc
-Version: 0.5.0
-Summary: A DIMACS CNF compiler
-License: Unlicense
-Author: Aaron Windsor
-Author-email: aaron.windsor@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
 # cnfc
 
 A [CNF](https://en.wikipedia.org/wiki/Conjunctive_normal_form) compiler that generates
 compact DIMACS CNF encodings from higher-level primitives in Python. DIMACS CNF is
 the input format accepted by most SAT solvers.
 
 In contrast to optimization libraries like Z3, PySAT or ortools that provide both
@@ -168,31 +153,39 @@
 UNSATISFIABLE
 ```
 
 instead of a schedule, which tells us that there's no assignment of people to shifts that satisfies all of the criteria we've laid out.
 
 A [runnable version of this script](examples/scheduling) is in the [examples subdirectory](examples) of this repository.
 
-Installation
-============
+## Features
+
+Arbitrary clauses can be built, composed, and added to formulas with:
+
+   * Familiar boolean operators `And`, `Or`, `Not`, `If`, `Eq`, `Neq`.
+   * `Tuple`s that can be compared for equality, inequality, or lexicographic order.
+   * `Integer`s that can be added, multiplied, or compared as `Tuple`s (see [examples/prime](examples/prime)).
+   * `NumTrue` and `NumFalse` for cardinality constraints (see [examples/nqueens](examples/nqueens)).
+   * `RegexMatch` to apply binary regular expressions to `Tuple`s (see [examples/nonagram](examples/nonagram)).
+
+## Installation
 
 cnfc is tested on [these versions](https://github.com/aaw/cnfc/blob/master/.github/workflows/python-package.yml#L19) of Python 3. To install
 the latest stable release of cnfc, run:
 
 ```
 pip install cnfc
 ```
 
-Development
-===========
+## Development
 
 Install [poetry](https://python-poetry.org/docs/#installation) and run `poetry install`. Then you can bring up a shell, etc. Run tests with:
 
 ```
 poetry run python3 -m unittest discover
 ```
 
 To release a new version to PyPI, bump the version in `pyproject.toml` and run:
 
 ```
 poetry publish --build --username=__token__ --password=$PYPI_TOKEN
-```
+```
```

