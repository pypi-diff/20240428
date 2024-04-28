# Comparing `tmp/jz3-0.1.3.tar.gz` & `tmp/jz3-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jz3-0.1.3.tar", last modified: Fri Apr 26 16:57:15 2024, max compression
+gzip compressed data, was "jz3-0.1.4.tar", last modified: Sun Apr 28 05:14:58 2024, max compression
```

## Comparing `jz3-0.1.3.tar` & `jz3-0.1.4.tar`

### file list

```diff
@@ -1,208 +1,40 @@
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.792554 jz3-0.1.3/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1096 2024-04-18 04:18:37.000000 jz3-0.1.3/LICENSE-Z3.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1092 2024-04-18 04:24:33.000000 jz3-0.1.3/LICENSE.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2961 2024-04-26 16:57:15.792400 jz3-0.1.3/PKG-INFO
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2347 2024-04-19 04:33:39.000000 jz3-0.1.3/README.md
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.752909 jz3-0.1.3/jz3/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       56 2024-04-26 16:56:48.000000 jz3-0.1.3/jz3/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.754504 jz3-0.1.3/jz3/analysis/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.3/jz3/analysis/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.754951 jz3-0.1.3/jz3/analysis/archive/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.3/jz3/analysis/archive/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2859 2024-04-19 01:59:02.000000 jz3-0.1.3/jz3/analysis/archive/export_to_excel.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7252 2024-04-19 16:25:42.000000 jz3-0.1.3/jz3/analysis/compare_whole_problems.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7093 2024-04-26 16:09:39.000000 jz3-0.1.3/jz3/analysis/plot_comparison.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.755256 jz3-0.1.3/jz3/solvers/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.755503 jz3-0.1.3/jz3/solvers/cvc5-main/
--rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.3/jz3/solvers/cvc5-main/__init__ 2.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.755626 jz3-0.1.3/jz3/solvers/cvc5-main/build/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.755741 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.755851 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.755951 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.756057 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.757389 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3116 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/cad.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1148 2024-03-01 13:47:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/plot.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1462 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/examples/cad/sign_table.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.757791 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.758587 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1801 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/check.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4904 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/polypy_test.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.763316 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     4580 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/algebraic_number.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     5869 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_arithmetic.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1595 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_eval.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3805 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_factorization.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     5610 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_feasibility.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     4946 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_gcd.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     4434 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_mgcd.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     6784 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_resultants.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4241 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_roots.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3185 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/polynomial_sgn.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3694 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_factor.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3292 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_gcd.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3150 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/upolynomial_roots.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2528 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/value.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1941 2023-11-02 19:49:25.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/Poly-EP/test/python/tests/variable.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.3/jz3/solvers/cvc5-main/build/deps/src/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.764460 jz3-0.1.3/jz3/solvers/cvc5-main/contrib/
--rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.3/jz3/solvers/cvc5-main/contrib/__init__ 2.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/contrib/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     6875 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/contrib/learn_resource_weights.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     3724 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/contrib/make-release.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.764981 jz3-0.1.3/jz3/solvers/cvc5-main/contrib/packaging_python/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/contrib/packaging_python/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1258 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/contrib/packaging_python/mk_build_dir.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4275 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/contrib/packaging_python/mk_wheel.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     1501 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/contrib/uncovered-api-functions.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.765282 jz3-0.1.3/jz3/solvers/cvc5-main/docs/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/docs/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.766271 jz3-0.1.3/jz3/solvers/cvc5-main/docs/ext/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/docs/ext/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1380 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/docs/ext/autoenum.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4089 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/docs/ext/examples.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1522 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/docs/ext/include_build_file.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1809 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/docs/ext/run_command.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     6014 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/docs/ext/smtliblexer.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.766755 jz3-0.1.3/jz3/solvers/cvc5-main/examples/
--rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/__init__ 2.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.766878 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.770782 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3445 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/bags.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4302 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/bitvectors.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3399 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/bitvectors_and_arrays.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3390 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/combination.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     6001 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/datatypes.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1428 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/exceptions.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1570 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/extract.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1538 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/finite_field.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4111 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/floating_point.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      842 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/helloworld.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1026 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/id.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2257 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/linear_arith.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.773667 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1000 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/bitvectors.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      946 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/bitvectors_and_arrays.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      801 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/combination.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1459 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/datatypes.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      390 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/exceptions.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      402 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/extract.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      766 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/floating_point.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      102 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/helloworld.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      348 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/id.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      232 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/linear_arith.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1444 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/quickstart.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      441 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/sets.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      156 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/pythonic/transcendentals.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     6561 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/quickstart.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     6283 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/relations.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2035 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/sequences.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2878 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/sets.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3128 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/strings.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3243 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/sygus-fun.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2152 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/sygus-inv.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1375 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/transcendentals.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1847 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/examples/api/python/utils.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.773889 jz3-0.1.3/jz3/solvers/cvc5-main/src/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.774086 jz3-0.1.3/jz3/solvers/cvc5-main/src/api/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/api/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.774462 jz3-0.1.3/jz3/solvers/cvc5-main/src/api/java/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/api/java/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7110 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/api/parseenums.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.774567 jz3-0.1.3/jz3/solvers/cvc5-main/src/api/python/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/api/python/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.774772 jz3-0.1.3/jz3/solvers/cvc5-main/src/base/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/base/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3208 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/base/collect_tags.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.775221 jz3-0.1.3/jz3/solvers/cvc5-main/src/options/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/options/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    43409 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/options/mkoptions.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.777757 jz3-0.1.3/jz3/solvers/cvc5-main/src/rewriter/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/rewriter/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    11371 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/rewriter/mkrewrites.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7288 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/rewriter/node.py
--rw-------   0 jiazhenghao   (501) staff       (20)     1382 2023-11-02 15:53:34.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/rewriter/rule 2.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1382 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/rewriter/rule.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    10506 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/rewriter/rw_parser.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2178 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/src/rewriter/util.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.778314 jz3-0.1.3/jz3/solvers/cvc5-main/test/
--rw-------   0 jiazhenghao   (501) staff       (20)        0 2024-03-01 13:46:21.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/__init__ 2.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.778440 jz3-0.1.3/jz3/solvers/cvc5-main/test/api/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/api/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.780467 jz3-0.1.3/jz3/solvers/cvc5-main/test/api/python/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/api/python/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      824 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/api/python/boilerplate.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1433 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/api/python/finite_field.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1127 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/api/python/issue4889.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      888 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/api/python/issue5074.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1519 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/api/python/issue6111.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1008 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/api/python/proj-issue306.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1545 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/api/python/reset_assertions.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     6607 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/api/python/sep_log_api.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      756 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/api/python/two_solvers.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.780931 jz3-0.1.3/jz3/solvers/cvc5-main/test/binary/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/binary/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2445 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/binary/interactive_shell.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.781284 jz3-0.1.3/jz3/solvers/cvc5-main/test/regress/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/regress/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.781524 jz3-0.1.3/jz3/solvers/cvc5-main/test/regress/cli/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/regress/cli/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)    31784 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/regress/cli/run_regression.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.782006 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.782125 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.788100 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/python/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/python/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    18818 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/python/test_datatype_api.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1506 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/python/test_finite_field.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4112 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/python/test_grammar.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7537 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/python/test_op.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2221 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/python/test_proof.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2456 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/python/test_result.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    99840 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/python/test_solver.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    19318 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/python/test_sort.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1822 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/python/test_synth_result.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    42934 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/python/test_term.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3300 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/solvers/cvc5-main/test/unit/api/python/test_to_python_obj.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.789435 jz3-0.1.3/jz3/src/
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.790396 jz3-0.1.3/jz3/src/SMTs/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    11530 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/src/SMTs/SMTs.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/src/SMTs/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.791662 jz3-0.1.3/jz3/src/Sudokus/
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)    36923 2024-04-26 16:08:11.000000 jz3-0.1.3/jz3/src/Sudokus/Sudoku.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/src/Sudokus/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)    23468 2024-04-26 15:30:20.000000 jz3-0.1.3/jz3/src/Sudokus/sudoku_exhaustive_search_condition.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    22912 2024-04-19 04:23:09.000000 jz3-0.1.3/jz3/src/Sudokus/sudoku_heuristic_search_condition.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.3/jz3/src/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       84 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/src/clean_up.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     3437 2024-04-26 05:20:00.000000 jz3-0.1.3/jz3/src/run_solvers.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      335 2024-04-18 02:04:15.000000 jz3-0.1.3/jz3/src/z3_quick_start_guide.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    10939 2024-04-26 02:43:34.000000 jz3-0.1.3/jz3/src/z3_wrapper.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.792184 jz3-0.1.3/jz3/tests/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:12.000000 jz3-0.1.3/jz3/tests/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:20.000000 jz3-0.1.3/jz3/tests/test_solver.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-26 16:57:15.753800 jz3-0.1.3/jz3.egg-info/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2961 2024-04-26 16:57:15.000000 jz3-0.1.3/jz3.egg-info/PKG-INFO
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     8386 2024-04-26 16:57:15.000000 jz3-0.1.3/jz3.egg-info/SOURCES.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        1 2024-04-26 16:57:15.000000 jz3-0.1.3/jz3.egg-info/dependency_links.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       21 2024-04-26 16:57:15.000000 jz3-0.1.3/jz3.egg-info/requires.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        4 2024-04-26 16:57:15.000000 jz3-0.1.3/jz3.egg-info/top_level.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       38 2024-04-26 16:57:15.792619 jz3-0.1.3/setup.cfg
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      810 2024-04-26 16:57:12.000000 jz3-0.1.3/setup.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.118718 jz3-0.1.4/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1096 2024-04-18 04:18:37.000000 jz3-0.1.4/LICENSE-Z3.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1092 2024-04-18 04:24:33.000000 jz3-0.1.4/LICENSE.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-28 05:14:58.118604 jz3-0.1.4/PKG-INFO
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2347 2024-04-19 04:33:39.000000 jz3-0.1.4/README.md
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.113770 jz3-0.1.4/jz3/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       55 2024-04-26 16:59:15.000000 jz3-0.1.4/jz3/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.114794 jz3-0.1.4/jz3/analysis/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.4/jz3/analysis/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.115009 jz3-0.1.4/jz3/analysis/archive/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.4/jz3/analysis/archive/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2859 2024-04-19 01:59:02.000000 jz3-0.1.4/jz3/analysis/archive/export_to_excel.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.116199 jz3-0.1.4/jz3/analysis/scripts/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 04:00:01.000000 jz3-0.1.4/jz3/analysis/scripts/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     7252 2024-04-19 16:25:42.000000 jz3-0.1.4/jz3/analysis/scripts/compare_whole_problems.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     7955 2024-04-28 04:25:24.000000 jz3-0.1.4/jz3/analysis/scripts/plot_comparison.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.116537 jz3-0.1.4/jz3/solvers/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.4/jz3/solvers/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.117484 jz3-0.1.4/jz3/src/
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.118150 jz3-0.1.4/jz3/src/SMTs/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    11530 2024-04-18 02:04:15.000000 jz3-0.1.4/jz3/src/SMTs/SMTs.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.4/jz3/src/SMTs/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.118255 jz3-0.1.4/jz3/src/Sudokus/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.4/jz3/src/Sudokus/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.4/jz3/src/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       84 2024-04-18 02:04:15.000000 jz3-0.1.4/jz3/src/clean_up.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     3542 2024-04-28 05:00:33.000000 jz3-0.1.4/jz3/src/run_solvers.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      282 2024-04-28 04:36:42.000000 jz3-0.1.4/jz3/src/z3_quick_start_guide.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    10939 2024-04-26 02:43:34.000000 jz3-0.1.4/jz3/src/z3_wrapper.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.118451 jz3-0.1.4/jz3/tests/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:12.000000 jz3-0.1.4/jz3/tests/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:20.000000 jz3-0.1.4/jz3/tests/test_solver.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:14:58.114665 jz3-0.1.4/jz3.egg-info/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-28 05:14:58.000000 jz3-0.1.4/jz3.egg-info/PKG-INFO
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      675 2024-04-28 05:14:58.000000 jz3-0.1.4/jz3.egg-info/SOURCES.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        1 2024-04-28 05:14:58.000000 jz3-0.1.4/jz3.egg-info/dependency_links.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       21 2024-04-28 05:14:58.000000 jz3-0.1.4/jz3.egg-info/requires.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        4 2024-04-28 05:14:58.000000 jz3-0.1.4/jz3.egg-info/top_level.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       38 2024-04-28 05:14:58.118780 jz3-0.1.4/setup.cfg
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      839 2024-04-28 05:14:32.000000 jz3-0.1.4/setup.py
```

### Comparing `jz3-0.1.3/LICENSE-Z3.txt` & `jz3-0.1.4/LICENSE-Z3.txt`

 * *Files identical despite different names*

### Comparing `jz3-0.1.3/LICENSE.txt` & `jz3-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jz3-0.1.3/PKG-INFO` & `jz3-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: jz3
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple wrapper for Z3 solver
 Home-page: https://github.com/Robert-Jia00129/jz3
 Author: Sebastiaan Joosten, Zheng Robert Jia
 Author-email: jia00129@umn.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE-Z3.txt
 License-File: LICENSE.txt
 
 # Argyle_Sudoku
 > This project was partly based on the code from [z3-sudoku](https://github.com/awkwardbunny/z3-sudoku)
```

### Comparing `jz3-0.1.3/README.md` & `jz3-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `jz3-0.1.3/jz3/analysis/archive/export_to_excel.py` & `jz3-0.1.4/jz3/analysis/archive/export_to_excel.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.3/jz3/analysis/compare_whole_problems.py` & `jz3-0.1.4/jz3/analysis/scripts/compare_whole_problems.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.3/jz3/analysis/plot_comparison.py` & `jz3-0.1.4/jz3/analysis/scripts/plot_comparison.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,34 +43,47 @@
     def plot_constraints_comparison(self, constraint_comparison_num, solvers=None, combined_plot=False, constraint_names=None):
         times_constraint_true = {}
         times_constraint_false = {}
         combined_times_true = []
         combined_times_false = []
 
         for entry in self.parsed_data:
-            for constraint, solvers_data in entry.items():
-                if type(constraint) == tuple:
-                    constraint_value = constraint[constraint_comparison_num]
-
-                    for solver_key, values in solvers_data.items():
-                        if solver_key != 'smt_path':
-                            time = values[0][0]
+            processed_keys = set()  # To keep track of processed keys
+            for key in list(entry.keys()):
+                if key not in processed_keys and isinstance(key, tuple):
+                    # Create the complement key
+                    complement_key = list(key)
+                    complement_key[constraint_comparison_num] = not key[constraint_comparison_num]
+                    complement_key = tuple(complement_key)
+                    if complement_key in entry:
+                        # Determine which is the True key and which is the False key
+                        true_key, false_key = (key, complement_key) if key[constraint_comparison_num] else (
+                        complement_key, key)
+
+                        true_data = entry[true_key]
+                        false_data = entry[false_key]
+
+                        for solver_key in true_data:
+                            if solver_key != 'smt_path' and (solvers is None or solver_key in solvers):
+                                time_true = true_data[solver_key][0][0]
+                                time_false = false_data[solver_key][0][0]
 
-                            if solvers is None or solver_key in solvers:
                                 if solver_key not in times_constraint_true:
                                     times_constraint_true[solver_key] = []
                                 if solver_key not in times_constraint_false:
                                     times_constraint_false[solver_key] = []
 
-                                if constraint_value:
-                                    times_constraint_true[solver_key].append(time)
-                                    combined_times_true.append(time)
-                                else:
-                                    times_constraint_false[solver_key].append(time)
-                                    combined_times_false.append(time)
+                                times_constraint_true[solver_key].append(time_true)
+                                combined_times_true.append(time_true)
+
+                                times_constraint_false[solver_key].append(time_false)
+                                combined_times_false.append(time_false)
+
+                        processed_keys.add(true_key)
+                        processed_keys.add(false_key)
 
         if solvers is None:
             solvers = list(times_constraint_true.keys())
 
         num_plots = len(solvers) + 1 if combined_plot else len(solvers)
         fig, axs = plt.subplots(num_plots, 1, figsize=(self.width, self.height * num_plots))
 
@@ -82,15 +95,15 @@
                 min_length = min(len(times_constraint_true[solver_key]), len(times_constraint_false[solver_key]))
                 true_times = times_constraint_true[solver_key][:min_length]
                 false_times = times_constraint_false[solver_key][:min_length]
                 # adjusting the datapoints to be within or at the edge of the graph
                 true_times = np.clip(true_times, 0, self.x_max)
                 false_times = np.clip(false_times, 0, self.y_max)
                 for ele in false_times:
-                    if ele >= self.y_max:
+                    if ele > self.y_max:
                         raise "AS"
 
                 axs[i].scatter(true_times, false_times, alpha=self.opacity,s=self.marker_size)
                 axs[i].plot([0, self.x_max], [0, self.y_max], self.line_style)
                 axs[i].set_title(f'Time comparison for {solver_key}')
 
                 # set x y label according to constraint name
@@ -130,17 +143,18 @@
             axs[-1].grid(self.grid)
 
         plt.tight_layout()
         plt.show()
 
 
 if __name__ == '__main__':
-    time_instances_file_path = '../time-record/particular_hard_instance_time_record/argyle_time.txt'
+    time_instances_file_path = '../../time-record/particular_hard_instance_time_record/argyle_time.txt'
     constraint_names = [("classic","argyle"),
                         ("distinct","PbEq"),
                         ("percol","inorder"),
                         ("is_bool","is_num"),
                         ("prefill","no_prefill"),
                         ("gen_time","solve_time")]
     plotter = ConstraintPlotter(time_instances_file_path)
     plotter.set_graph_properties(x_max=5,y_max=5)
-    plotter.plot_constraints_comparison(1, solvers=["z3", "cvc5"],  combined_plot=True, constraint_names=constraint_names)
+    # plotter.plot_constraints_comparison(3, solvers=["z3", "cvc5"],  combined_plot=True, constraint_names=constraint_names)
+    plotter.plot_constraints_comparison(1, solvers=["z3","cvc5"],  combined_plot=True, constraint_names=constraint_names)
```

### Comparing `jz3-0.1.3/jz3/src/SMTs/SMTs.py` & `jz3-0.1.4/jz3/src/SMTs/SMTs.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.3/jz3/src/run_solvers.py` & `jz3-0.1.4/jz3/src/run_solvers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 import subprocess
 import time
 import os
 from pathlib import Path
 
-def run_cvc5(smt2_file, time_out:int=5):
+
+def run_cvc5(smt2_file, time_out: int = 5):
     cvc_path = get_executable_path("cvc5-macOS-arm64")
-    command = [cvc_path,smt2_file,"--lang","smt2"]
+    command = [cvc_path, smt2_file, "--lang", "smt2"]
     start_time = time.time()
     did_timeout = False
     try:
         result = subprocess.run(command,
                                 capture_output=True, text=True, timeout=time_out)
         combined_output = ((result.stdout if result.stdout is not None else "") +
                            (result.stderr if result.stderr is not None else ""))  # capture all output
     except subprocess.TimeoutExpired as exc:
         did_timeout = True
         combined_output = ((exc.stdout.decode('utf-8') if exc.stdout else "") +
                            (exc.stderr.decode('utf-8') if exc.stderr else ""))  # capture all output
     ans = "timeout"
 
     end_time = time.time()
-    total_time = end_time-start_time
+    total_time = end_time - start_time
     if not did_timeout:
         if "unsat" in combined_output:
             ans = "unsat"
         elif "sat" in combined_output:
             ans = "sat"
         else:
             ans = "unknown"
     else:
-        total_time=time_out
+        total_time = time_out
     return (total_time, did_timeout, ans)
 
-def run_z3(smt2_file: str, time_out:int = 5):
+
+def run_z3(smt2_file: str, time_out: int = 5):
     """
     :param smt_log_file_path:
     :param time_out: in seconds
     :return:
     """
     start_time = time.time()
     did_timeout = False
@@ -46,59 +48,65 @@
         combined_output = ((result.stdout if result.stdout is not None else "") +
                            (result.stderr if result.stderr is not None else ""))  # capture all output
     except subprocess.TimeoutExpired as exc:
         did_timeout = True
         result = exc
     ans = "timeout"
     end_time = time.time()
-    total_time = end_time-start_time
+    total_time = end_time - start_time
     if not did_timeout:
         if "unsat" in combined_output:
             ans = "unsat"
         elif "sat" in combined_output:
             ans = "sat"
         else:
             ans = "unknown"
     else:
-        total_time=time_out
+        total_time = time_out
     return (total_time, did_timeout, ans)
 
 
-
 def run_yices(smt2_file):
     command = f"yices-smt2 {smt2_file}"
     try:
         result = subprocess.run(command, shell=True, capture_output=True, text=True, check=True)
         return result.stdout.strip()
     except subprocess.CalledProcessError as e:
         return f"Error: {e}"
 
+
 # Dictionary to map solver names to their corresponding functions
 solvers = {
     "cvc5": run_cvc5,
     "z3": run_z3
     # "yices": run_yices
 }
 
-def run_solvers(smt2_file,verbose=False):
+
+def run_solvers(smt2_file, verbose=False, time_out=5):
+    """
+    time_out: in seconds
+    """
     results = {}
 
     for solver, run_function in solvers.items():
         if verbose:
             print(f"Running {solver}...")
-        result = run_function(smt2_file)
+        result = run_function(smt2_file,time_out=time_out)
         results[solver] = result
 
     return results
 
 
 def get_executable_path(solver_path_in_solvers_dir):
     # Get the directory of the current file (__file__ refers to the script in which this code is written)
     dir_of_jz3 = Path(os.path.dirname(__file__)).parent
 
     # Build the path to the executable
-    executable_path = os.path.join(dir_of_jz3, "solvers/"+solver_path_in_solvers_dir)
+    executable_path = os.path.join(dir_of_jz3, "solvers/" + solver_path_in_solvers_dir)
 
     return executable_path
 
-if __name__=='__main__':
-    print(run_cvc5('/Users/jiazhenghao/Desktop/CodingProjects/jz3/jz3/problems_instances/particular_hard_instances_records/smt2_files/04_25_00_58_021714024682.151314'))
+
+if __name__ == '__main__':
+    print(run_cvc5(
+        '/Users/jiazhenghao/Desktop/CodingProjects/jz3/jz3/problems_instances/particular_hard_instances_records/smt2_files/04_25_00_58_021714024682.151314'))
```

### Comparing `jz3-0.1.3/jz3/src/z3_wrapper.py` & `jz3-0.1.4/jz3/src/z3_wrapper.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.3/jz3.egg-info/PKG-INFO` & `jz3-0.1.4/jz3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: jz3
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple wrapper for Z3 solver
 Home-page: https://github.com/Robert-Jia00129/jz3
 Author: Sebastiaan Joosten, Zheng Robert Jia
 Author-email: jia00129@umn.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE-Z3.txt
 License-File: LICENSE.txt
 
 # Argyle_Sudoku
 > This project was partly based on the code from [z3-sudoku](https://github.com/awkwardbunny/z3-sudoku)
```

### Comparing `jz3-0.1.3/setup.py` & `jz3-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='jz3',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     description='A simple wrapper for Z3 solver',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Sebastiaan Joosten, Zheng Robert Jia',
     author_email='jia00129@umn.edu',
     url='https://github.com/Robert-Jia00129/jz3',
     license='MIT',
     install_requires=[
         'z3-solver',
         'matplotlib',
     ],
+    python_requires='>3.11',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
```

