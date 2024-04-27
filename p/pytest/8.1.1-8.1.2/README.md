# Comparing `tmp/pytest-8.1.1.tar.gz` & `tmp/pytest-8.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-8.1.1.tar", last modified: Sat Mar  9 11:49:46 2024, max compression
+gzip compressed data, was "pytest-8.1.2.tar", last modified: Fri Apr 26 17:05:53 2024, max compression
```

## Comparing `pytest-8.1.1.tar` & `pytest-8.1.2.tar`

### file list

```diff
@@ -1,679 +1,680 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.633274 pytest-8.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-09 11:49:29.000000 pytest-8.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-09 11:49:29.000000 pytest-8.1.1/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-09 11:49:29.000000 pytest-8.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.521274 pytest-8.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.521274 pytest-8.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/ISSUE_TEMPLATE/1_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/ISSUE_TEMPLATE/2_feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/labels.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.525274 pytest-8.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/workflows/backport.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/workflows/prepare-release-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-09 11:49:29.000000 pytest-8.1.1/.github/workflows/update-plugin-list.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-09 11:49:29.000000 pytest-8.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-09 11:49:29.000000 pytest-8.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-09 11:49:29.000000 pytest-8.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-03-09 11:49:29.000000 pytest-8.1.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-09 11:49:29.000000 pytest-8.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-09 11:49:29.000000 pytest-8.1.1/CITATION
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-09 11:49:29.000000 pytest-8.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    20372 2024-03-09 11:49:29.000000 pytest-8.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-09 11:49:29.000000 pytest-8.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-09 11:49:29.000000 pytest-8.1.1/OPENCOLLECTIVE.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-03-09 11:49:46.633274 pytest-8.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-03-09 11:49:29.000000 pytest-8.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-03-09 11:49:29.000000 pytest-8.1.1/RELEASING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-09 11:49:29.000000 pytest-8.1.1/TIDELIFT.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.525274 pytest-8.1.1/bench/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/bench_argcomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/manyparam.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/skip.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/unit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-09 11:49:29.000000 pytest-8.1.1/bench/xunit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.525274 pytest-8.1.1/changelog/
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-09 11:49:29.000000 pytest-8.1.1/changelog/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-09 11:49:29.000000 pytest-8.1.1/changelog/_template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-09 11:49:29.000000 pytest-8.1.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.509275 pytest-8.1.1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.529274 pytest-8.1.1/doc/en/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.533274 pytest-8.1.1/doc/en/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/_templates/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/_templates/links.html
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/_templates/relations.html
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/_templates/sidebarintro.html
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/_templates/slim_searchbox.html
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/adopt.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.565274 pytest-8.1.1/doc/en/announce/
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.0.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.1.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.1.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.2.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.2.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.3.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.3.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.3.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.3.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.3.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.4.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.5.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.5.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.5.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.6.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.6.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.6.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.6.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.7.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.7.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.7.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.8.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.8.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.8.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.8.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.8.6.rst
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.8.7.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.9.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.9.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-2.9.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.6.rst
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.0.7.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.1.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.1.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.10.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.10.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.2.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.2.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.2.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.2.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.3.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.3.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.4.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.5.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.5.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.6.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.6.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.6.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.6.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.6.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.7.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.7.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.7.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.7.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.7.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.8.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.8.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.8.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.9.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.9.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.9.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-3.9.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.3.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.4.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.5.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.6.rst
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.7.rst
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.8.rst
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-4.6.9.rst
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.1.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.1.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.2.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.2.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.2.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.3.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.3.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.3.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.3.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.3.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.4.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-5.4.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.0.0rc1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.1.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.2.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.2.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.2.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-6.2.5.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.0.0rc1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.1.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.1.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.2.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.3.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.3.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.4.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.4.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-7.4.4.rst
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.0.0rc1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.0.0rc2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/release-8.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/announce/sprint2016.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/backwards-compatibility.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/builtin.rst
--rw-r--r--   0 runner    (1001) docker     (127)   405803 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/contents.rst
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    38963 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/deprecations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/development_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.569274 pytest-8.1.1/doc/en/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.569274 pytest-8.1.1/doc/en/example/assertion/
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/assertion/failure_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.569274 pytest-8.1.1/doc/en/example/assertion/global_testmodule_config/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/assertion/global_testmodule_config/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/assertion/global_testmodule_config/test_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/assertion/test_failures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/assertion/test_setup_flow_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/attic.rst
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.569274 pytest-8.1.1/doc/en/example/customdirectory/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.569274 pytest-8.1.1/doc/en/example/customdirectory/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory/tests/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory/tests/test_first.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory/tests/test_second.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory/tests/test_third.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/customdirectory.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.573274 pytest-8.1.1/doc/en/example/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/fixture_availability.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/fixture_availability_plugins.svg
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_flat.svg
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.svg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.svg
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies_flat.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies_unclear.svg
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_scope.svg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_request_different_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/fixtures/test_fixtures_request_different_scope.svg
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    26471 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/markers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/multipython.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.573274 pytest-8.1.1/doc/en/example/nonpython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/nonpython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/nonpython/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/nonpython/test_simple.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/nonpython.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22718 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/parametrize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/pythoncollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/pythoncollection.rst
--rw-r--r--   0 runner    (1001) docker     (127)    27266 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/reportingdemo.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35232 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/simple.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/special.rst
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/example/xfail_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.573274 pytest-8.1.1/doc/en/explanation/
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/explanation/anatomy.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/explanation/fixtures.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/explanation/flaky.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11681 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/explanation/goodpractices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/explanation/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/explanation/pythonpath.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8766 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/funcarg_compare.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/funcargs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/historical-notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.581274 pytest-8.1.1/doc/en/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/assert.rst
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/bash-completion.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/cache.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/capture-stdout-stderr.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/capture-warnings.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/doctest.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/existingtestsuite.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/failures.rst
--rw-r--r--   0 runner    (1001) docker     (127)    62010 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/fixtures.rst
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/mark.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15797 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/monkeypatch.rst
--rw-r--r--   0 runner    (1001) docker     (127)    29330 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/output.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9828 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/parametrize.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12148 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/skipping.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/tmp_path.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/unittest.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/writing_hook_functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/writing_plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/how-to/xunit_setup.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.581274 pytest-8.1.1/doc/en/img/
--rw-r--r--   0 runner    (1001) docker     (127)    25291 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/cramer2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)   104057 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/freiburg2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    23032 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/gaynor3.png
--rw-r--r--   0 runner    (1001) docker     (127)    23246 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/keleshev.png
--rw-r--r--   0 runner    (1001) docker     (127)    17035 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/pullrequest.png
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/pylib.png
--rw-r--r--   0 runner    (1001) docker     (127)    40974 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/pytest1.png
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/pytest_logo_curves.svg
--rw-r--r--   0 runner    (1001) docker     (127)    31476 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/img/theuni.png
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/naming20.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.581274 pytest-8.1.1/doc/en/proposals/
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/proposals/parametrize_with_fixtures.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/recwarn.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.585274 pytest-8.1.1/doc/en/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/reference/customize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/reference/exit-codes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16327 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/reference/fixtures.rst
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)   921217 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/reference/plugin_list.rst
--rw-r--r--   0 runner    (1001) docker     (127)    66318 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/reference/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/sponsor.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/talks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/tidelift.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-09 11:49:29.000000 pytest-8.1.1/doc/en/yieldfixture.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.585274 pytest-8.1.1/extra/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-09 11:49:29.000000 pytest-8.1.1/extra/get_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-03-09 11:49:29.000000 pytest-8.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.585274 pytest-8.1.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/generate-gh-release-notes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/prepare-release-pr.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/release.major.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/release.minor.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/release.patch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/release.pre.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/release.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/towncrier-draft-to-file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-03-09 11:49:29.000000 pytest-8.1.1/scripts/update-plugin-list.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 11:49:46.633274 pytest-8.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.585274 pytest-8.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.593274 pytest-8.1.1/src/_pytest/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_argcomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.593274 pytest-8.1.1/src/_pytest/_code/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50043 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_code/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_code/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.597274 pytest-8.1.1/src/_pytest/_io/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19665 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_io/pprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_io/saferepr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_io/terminalwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_io/wcwidth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.597274 pytest-8.1.1/src/_pytest/_py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_py/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    49888 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/_py/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-09 11:49:46.000000 pytest-8.1.1/src/_pytest/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.597274 pytest-8.1.1/src/_pytest/assertion/
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/assertion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47200 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/assertion/rewrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/assertion/truncate.py
--rw-r--r--   0 runner    (1001) docker     (127)    20307 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/assertion/util.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21140 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/cacheprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)    34963 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/capture.py
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.597274 pytest-8.1.1/src/_pytest/config/
--rw-r--r--   0 runner    (1001) docker     (127)    69979 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/config/argparsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/config/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/config/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/config/findpaths.py
--rw-r--r--   0 runner    (1001) docker     (127)    13571 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/debugging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    26051 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/doctest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/faulthandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    67942 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/freeze_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/helpconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    41418 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/hookspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    25664 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/junitxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    16891 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/legacypath.py
--rw-r--r--   0 runner    (1001) docker     (127)    35440 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    37564 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.597274 pytest-8.1.1/src/_pytest/mark/
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/mark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/mark/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/mark/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    26733 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/outcomes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (127)    31138 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    61879 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/pytester.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/pytester_assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)    70069 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/python.py
--rw-r--r--   0 runner    (1001) docker     (127)    39138 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/python_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/python_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    13690 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/recwarn.py
--rw-r--r--   0 runner    (1001) docker     (127)    20911 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    19311 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/setuponly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/setupplan.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/skipping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/stepwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    54950 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/threadexception.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/tmpdir.py
--rw-r--r--   0 runner    (1001) docker     (127)    15052 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/unraisableexception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/warning_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-03-09 11:49:29.000000 pytest-8.1.1/src/_pytest/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-09 11:49:29.000000 pytest-8.1.1/src/py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.601274 pytest-8.1.1/src/pytest/
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-03-09 11:49:29.000000 pytest-8.1.1/src/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-09 11:49:29.000000 pytest-8.1.1/src/pytest/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/src/pytest/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.633274 pytest-8.1.1/src/pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-03-09 11:49:46.000000 pytest-8.1.1/src/pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21867 2024-03-09 11:49:46.000000 pytest-8.1.1/src/pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 11:49:46.000000 pytest-8.1.1/src/pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-09 11:49:46.000000 pytest-8.1.1/src/pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-09 11:49:46.000000 pytest-8.1.1/src/pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-09 11:49:46.000000 pytest-8.1.1/src/pytest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.609274 pytest-8.1.1/testing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.609274 pytest-8.1.1/testing/_py/
--rw-r--r--   0 runner    (1001) docker     (127)    52687 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/_py/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    49641 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/acceptance_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/code/
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/code/test_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    59954 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/code/test_excinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/code/test_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/deprecated_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/acceptance/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/acceptance/fixture_mock_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.513275 pytest-8.1.1/testing/example_scripts/collect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/collect/collect_init_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/collect_init_tests/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/collect/collect_init_tests/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/collect_init_tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/collect_init_tests/tests/test_foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/collect/package_infinite_recursion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/package_infinite_recursion/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/package_infinite_recursion/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/collect/package_infinite_recursion/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/package_infinite_recursion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/package_infinite_recursion/tests/test_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.513275 pytest-8.1.1/testing/example_scripts/collect/package_init_given_as_arg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/collect/package_init_given_as_arg/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/package_init_given_as_arg/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/collect/package_init_given_as_arg/pkg/test_foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.513275 pytest-8.1.1/testing/example_scripts/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/config/collect_pytest_prefix/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/config/collect_pytest_prefix/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/config/collect_pytest_prefix/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/config/collect_pytest_prefix/test_foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.613274 pytest-8.1.1/testing/example_scripts/conftest_usageerror/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/conftest_usageerror/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/conftest_usageerror/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/customdirectory/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/customdirectory/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/customdirectory/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/customdirectory/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/customdirectory/tests/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/customdirectory/tests/test_first.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/customdirectory/tests/test_second.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/customdirectory/tests/test_third.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/dataclasses/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_dataclasses_field_comparison_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_dataclasses_verbose.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_dataclasses_with_custom_eq.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_initvar.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_recursive_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_two_different_dataclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.513275 pytest-8.1.1/testing/example_scripts/doctest/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/doctest/main_py/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/doctest/main_py/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/doctest/main_py/test_normal_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/fixtures/custom_item/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/custom_item/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/custom_item/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.617274 pytest-8.1.1/testing/example_scripts/fixtures/custom_item/foo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/custom_item/foo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/custom_item/foo/test_foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.513275 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/test_in_sub1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/test_in_sub2.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_detect_recursive_dependency_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/test_spam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/test_extend_fixture_conftest_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_module_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_lookup_classlevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_lookup_modulelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_lookupfails.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/test_fixture_named_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/fixtures/test_getfixturevalue_dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/issue88_initial_file_multinodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/issue88_initial_file_multinodes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/issue88_initial_file_multinodes/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/issue88_initial_file_multinodes/test_hello.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/issue_519.py
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/junit-10.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.517274 pytest-8.1.1/testing/example_scripts/marks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.621274 pytest-8.1.1/testing/example_scripts/marks/marks_considered_keywords/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/marks/marks_considered_keywords/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/marks/marks_considered_keywords/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/marks/marks_considered_keywords/test_marks_as_keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.517274 pytest-8.1.1/testing/example_scripts/perf_examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/example_scripts/perf_examples/collect_stats/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/perf_examples/collect_stats/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/perf_examples/collect_stats/generate_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/perf_examples/collect_stats/template_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/example_scripts/tmpdir/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/tmpdir/tmp_path_fixture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/example_scripts/unittest/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_parametrized_fixture_error_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_setup_skip.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_setup_skip_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_setup_skip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_unittest_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_unittest_asynctest.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/unittest/test_unittest_plain_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/example_scripts/warnings/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/warnings/test_group_warnings_by_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/example_scripts/warnings/test_group_warnings_by_message_summary/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/warnings/test_group_warnings_by_message_summary/test_1.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/example_scripts/warnings/test_group_warnings_by_message_summary/test_2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/examples/test_issue519.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/freeze/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/freeze/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/freeze/create_executable.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/freeze/runtests_script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.625274 pytest-8.1.1/testing/freeze/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/freeze/tests/test_doctest.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/freeze/tests/test_trivial.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/freeze/tox_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.629274 pytest-8.1.1/testing/io/
--rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/io/test_pprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/io/test_saferepr.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/io/test_terminalwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/io/test_wcwidth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.629274 pytest-8.1.1/testing/logging/
--rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/logging/test_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/logging/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    47293 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/logging/test_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.629274 pytest-8.1.1/testing/plugins_integration/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/bdd_wallet.feature
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/bdd_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/django_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/pytest_anyio_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/pytest_asyncio_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/pytest_mock_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/pytest_trio_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/pytest_twisted_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/plugins_integration/simple_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:49:46.633274 pytest-8.1.1/testing/python/
--rw-r--r--   0 runner    (1001) docker     (127)    34588 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/approx.py
--rw-r--r--   0 runner    (1001) docker     (127)    52366 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)   140883 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    70079 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/metafunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11768 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/python/show_fixtures_per_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_argcomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)    65668 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_assertion.py
--rw-r--r--   0 runner    (1001) docker     (127)    66663 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_assertrewrite.py
--rw-r--r--   0 runner    (1001) docker     (127)    45293 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_cacheprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)    52300 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)    65092 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    79579 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25187 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    42797 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_debugging.py
--rw-r--r--   0 runner    (1001) docker     (127)    50721 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_error_diffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_faulthandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_findpaths.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_helpconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    57790 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_junitxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_legacypath.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_link_resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)    11332 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    34663 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_mark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_mark_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    12801 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_parseopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_pastebin.py
--rw-r--r--   0 runner    (1001) docker     (127)    43988 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    17284 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_pluginmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    27327 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_pytester.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_python_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_recwarn.py
--rw-r--r--   0 runner    (1001) docker     (127)    19992 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    34598 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_runner_xunit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    15424 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_setuponly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_setupplan.py
--rw-r--r--   0 runner    (1001) docker     (127)    43971 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_skipping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    10633 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_stepwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    98552 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_threadexception.py
--rw-r--r--   0 runner    (1001) docker     (127)    19532 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_tmpdir.py
--rw-r--r--   0 runner    (1001) docker     (127)    45389 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_unraisableexception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_warning_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    27546 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/test_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-09 11:49:29.000000 pytest-8.1.1/testing/typing_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-03-09 11:49:29.000000 pytest-8.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.874562 pytest-8.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-26 17:05:36.000000 pytest-8.1.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-26 17:05:36.000000 pytest-8.1.2/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-26 17:05:36.000000 pytest-8.1.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.762563 pytest-8.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.766563 pytest-8.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/ISSUE_TEMPLATE/1_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/ISSUE_TEMPLATE/2_feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/labels.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.766563 pytest-8.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/workflows/backport.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/workflows/prepare-release-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-26 17:05:36.000000 pytest-8.1.2/.github/workflows/update-plugin-list.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-26 17:05:36.000000 pytest-8.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-26 17:05:36.000000 pytest-8.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-26 17:05:36.000000 pytest-8.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-26 17:05:36.000000 pytest-8.1.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-26 17:05:36.000000 pytest-8.1.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-26 17:05:36.000000 pytest-8.1.2/CITATION
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-26 17:05:36.000000 pytest-8.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20372 2024-04-26 17:05:36.000000 pytest-8.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-26 17:05:36.000000 pytest-8.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-26 17:05:36.000000 pytest-8.1.2/OPENCOLLECTIVE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-04-26 17:05:53.874562 pytest-8.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-26 17:05:36.000000 pytest-8.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-26 17:05:36.000000 pytest-8.1.2/RELEASING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-26 17:05:36.000000 pytest-8.1.2/TIDELIFT.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.766563 pytest-8.1.2/bench/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-26 17:05:36.000000 pytest-8.1.2/bench/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-26 17:05:36.000000 pytest-8.1.2/bench/bench_argcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 17:05:36.000000 pytest-8.1.2/bench/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-26 17:05:36.000000 pytest-8.1.2/bench/manyparam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-26 17:05:36.000000 pytest-8.1.2/bench/skip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-26 17:05:36.000000 pytest-8.1.2/bench/unit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-26 17:05:36.000000 pytest-8.1.2/bench/xunit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.766563 pytest-8.1.2/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-26 17:05:36.000000 pytest-8.1.2/changelog/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-26 17:05:36.000000 pytest-8.1.2/changelog/_template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-26 17:05:36.000000 pytest-8.1.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.754563 pytest-8.1.2/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.774563 pytest-8.1.2/doc/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.774563 pytest-8.1.2/doc/en/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/_templates/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/_templates/links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/_templates/relations.html
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/_templates/sidebarintro.html
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/_templates/slim_searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/adopt.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.806563 pytest-8.1.2/doc/en/announce/
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.0.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.1.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.2.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.2.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.3.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.3.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.3.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.3.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.3.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.4.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.5.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.5.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.5.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.6.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.6.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.6.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.6.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.7.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.7.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.7.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.8.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.8.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.8.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.8.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.8.6.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.8.7.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.9.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.9.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-2.9.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.0.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.0.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.0.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.0.6.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.0.7.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.1.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.10.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.10.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.2.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.2.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.2.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.2.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.3.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.3.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.4.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.5.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.5.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.6.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.6.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.6.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.6.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.6.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.7.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.7.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.7.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.7.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.7.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.8.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.8.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.8.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.9.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.9.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.9.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-3.9.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.3.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.4.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.5.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.6.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.6.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.6.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.6.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.6.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.6.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.6.6.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.6.7.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.6.8.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-4.6.9.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.1.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.2.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.2.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.2.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.3.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.3.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.3.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.3.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.3.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.4.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-5.4.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-6.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-6.0.0rc1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-6.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-6.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-6.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-6.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-6.1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-6.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-6.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-6.2.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-6.2.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-6.2.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-6.2.5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.0.0rc1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.1.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.2.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.3.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.3.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.4.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.4.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-7.4.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-8.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-8.0.0rc1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-8.0.0rc2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-8.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-8.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-8.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-8.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/release-8.1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/announce/sprint2016.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/backwards-compatibility.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/builtin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   406043 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    38963 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/deprecations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/development_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.806563 pytest-8.1.2/doc/en/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.806563 pytest-8.1.2/doc/en/example/assertion/
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/assertion/failure_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.806563 pytest-8.1.2/doc/en/example/assertion/global_testmodule_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/assertion/global_testmodule_config/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/assertion/global_testmodule_config/test_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/assertion/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/assertion/test_setup_flow_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/attic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.810563 pytest-8.1.2/doc/en/example/customdirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/customdirectory/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/customdirectory/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.810563 pytest-8.1.2/doc/en/example/customdirectory/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/customdirectory/tests/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/customdirectory/tests/test_first.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/customdirectory/tests/test_second.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/customdirectory/tests/test_third.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/customdirectory.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.810563 pytest-8.1.2/doc/en/example/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/fixture_availability.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/fixture_availability_plugins.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse_flat.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_dependencies.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_dependencies_flat.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_dependencies_unclear.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_scope.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_request_different_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/fixtures/test_fixtures_request_different_scope.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26471 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/markers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/multipython.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.814563 pytest-8.1.2/doc/en/example/nonpython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/nonpython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/nonpython/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/nonpython/test_simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/nonpython.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22718 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/parametrize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/pythoncollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/pythoncollection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    27266 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/reportingdemo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35232 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/simple.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/special.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/example/xfail_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.814563 pytest-8.1.2/doc/en/explanation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/explanation/anatomy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/explanation/fixtures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/explanation/flaky.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11681 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/explanation/goodpractices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/explanation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/explanation/pythonpath.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8766 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/funcarg_compare.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/funcargs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/historical-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.818563 pytest-8.1.2/doc/en/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/assert.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/bash-completion.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/cache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/capture-stdout-stderr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/capture-warnings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/doctest.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/existingtestsuite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/failures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    62010 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/fixtures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/mark.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15797 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/monkeypatch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    29330 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/output.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9828 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/parametrize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12148 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/skipping.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/tmp_path.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/unittest.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/writing_hook_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/writing_plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/how-to/xunit_setup.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.818563 pytest-8.1.2/doc/en/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    25291 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/img/cramer2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/img/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   104057 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/img/freiburg2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    23032 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/img/gaynor3.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23246 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/img/keleshev.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17035 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/img/pullrequest.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/img/pylib.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40974 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/img/pytest1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/img/pytest_logo_curves.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    31476 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/img/theuni.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/naming20.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.818563 pytest-8.1.2/doc/en/proposals/
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/proposals/parametrize_with_fixtures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/recwarn.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.822563 pytest-8.1.2/doc/en/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/reference/customize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/reference/exit-codes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16327 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/reference/fixtures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   921217 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/reference/plugin_list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    66318 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/reference/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/sponsor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/talks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/tidelift.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-26 17:05:36.000000 pytest-8.1.2/doc/en/yieldfixture.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.822563 pytest-8.1.2/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-26 17:05:36.000000 pytest-8.1.2/extra/get_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-04-26 17:05:36.000000 pytest-8.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.822563 pytest-8.1.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 17:05:36.000000 pytest-8.1.2/scripts/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-26 17:05:36.000000 pytest-8.1.2/scripts/generate-gh-release-notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-26 17:05:36.000000 pytest-8.1.2/scripts/prepare-release-pr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-26 17:05:36.000000 pytest-8.1.2/scripts/release.major.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-26 17:05:36.000000 pytest-8.1.2/scripts/release.minor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-26 17:05:36.000000 pytest-8.1.2/scripts/release.patch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-26 17:05:36.000000 pytest-8.1.2/scripts/release.pre.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-26 17:05:36.000000 pytest-8.1.2/scripts/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-26 17:05:36.000000 pytest-8.1.2/scripts/towncrier-draft-to-file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-26 17:05:36.000000 pytest-8.1.2/scripts/update-plugin-list.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 17:05:53.874562 pytest-8.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.822563 pytest-8.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.834562 pytest-8.1.2/src/_pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/_argcomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.834562 pytest-8.1.2/src/_pytest/_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50074 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/_code/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/_code/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.834562 pytest-8.1.2/src/_pytest/_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19665 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/_io/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/_io/saferepr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/_io/terminalwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/_io/wcwidth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.834562 pytest-8.1.2/src/_pytest/_py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/_py/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49888 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/_py/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 17:05:53.000000 pytest-8.1.2/src/_pytest/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.838562 pytest-8.1.2/src/_pytest/assertion/
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/assertion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47200 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/assertion/rewrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/assertion/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20307 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/assertion/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21140 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/cacheprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34963 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.838562 pytest-8.1.2/src/_pytest/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    69979 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/config/argparsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/config/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/config/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/config/findpaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13571 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/debugging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26051 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/doctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/faulthandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67942 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/freeze_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/helpconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41418 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/hookspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25664 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/junitxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16891 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/legacypath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35440 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37564 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.838562 pytest-8.1.2/src/_pytest/mark/
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/mark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/mark/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/mark/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26733 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31138 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    61879 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/pytester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/pytester_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70069 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39382 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/python_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/python_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13690 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/recwarn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20911 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19311 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/setuponly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/setupplan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/skipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54950 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/threadexception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/tmpdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15052 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/unraisableexception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/warning_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-26 17:05:36.000000 pytest-8.1.2/src/_pytest/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-26 17:05:36.000000 pytest-8.1.2/src/py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.838562 pytest-8.1.2/src/pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-26 17:05:36.000000 pytest-8.1.2/src/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-26 17:05:36.000000 pytest-8.1.2/src/pytest/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/src/pytest/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.870562 pytest-8.1.2/src/pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-04-26 17:05:53.000000 pytest-8.1.2/src/pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21901 2024-04-26 17:05:53.000000 pytest-8.1.2/src/pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:05:53.000000 pytest-8.1.2/src/pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 17:05:53.000000 pytest-8.1.2/src/pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-26 17:05:53.000000 pytest-8.1.2/src/pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 17:05:53.000000 pytest-8.1.2/src/pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.850562 pytest-8.1.2/testing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.850562 pytest-8.1.2/testing/_py/
+-rw-r--r--   0 runner    (1001) docker     (127)    52687 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/_py/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49641 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/acceptance_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.850562 pytest-8.1.2/testing/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/code/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59954 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/code/test_excinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/code/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/deprecated_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.850562 pytest-8.1.2/testing/example_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.850562 pytest-8.1.2/testing/example_scripts/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/acceptance/fixture_mock_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.758563 pytest-8.1.2/testing/example_scripts/collect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.850562 pytest-8.1.2/testing/example_scripts/collect/collect_init_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/collect/collect_init_tests/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.854562 pytest-8.1.2/testing/example_scripts/collect/collect_init_tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/collect/collect_init_tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/collect/collect_init_tests/tests/test_foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.854562 pytest-8.1.2/testing/example_scripts/collect/package_infinite_recursion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/collect/package_infinite_recursion/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/collect/package_infinite_recursion/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.854562 pytest-8.1.2/testing/example_scripts/collect/package_infinite_recursion/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/collect/package_infinite_recursion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/collect/package_infinite_recursion/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.758563 pytest-8.1.2/testing/example_scripts/collect/package_init_given_as_arg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.854562 pytest-8.1.2/testing/example_scripts/collect/package_init_given_as_arg/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/collect/package_init_given_as_arg/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/collect/package_init_given_as_arg/pkg/test_foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.758563 pytest-8.1.2/testing/example_scripts/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.854562 pytest-8.1.2/testing/example_scripts/config/collect_pytest_prefix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/config/collect_pytest_prefix/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/config/collect_pytest_prefix/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/config/collect_pytest_prefix/test_foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.854562 pytest-8.1.2/testing/example_scripts/conftest_usageerror/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/conftest_usageerror/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/conftest_usageerror/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.854562 pytest-8.1.2/testing/example_scripts/customdirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/customdirectory/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/customdirectory/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.854562 pytest-8.1.2/testing/example_scripts/customdirectory/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/customdirectory/tests/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/customdirectory/tests/test_first.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/customdirectory/tests/test_second.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/customdirectory/tests/test_third.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.858562 pytest-8.1.2/testing/example_scripts/dataclasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/dataclasses/test_compare_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/dataclasses/test_compare_dataclasses_field_comparison_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/dataclasses/test_compare_dataclasses_verbose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/dataclasses/test_compare_dataclasses_with_custom_eq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/dataclasses/test_compare_initvar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/dataclasses/test_compare_recursive_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/dataclasses/test_compare_two_different_dataclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.758563 pytest-8.1.2/testing/example_scripts/doctest/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.858562 pytest-8.1.2/testing/example_scripts/doctest/main_py/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/doctest/main_py/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/doctest/main_py/test_normal_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.858562 pytest-8.1.2/testing/example_scripts/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.858562 pytest-8.1.2/testing/example_scripts/fixtures/custom_item/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/custom_item/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/custom_item/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.858562 pytest-8.1.2/testing/example_scripts/fixtures/custom_item/foo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/custom_item/foo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/custom_item/foo/test_foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.858562 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.758563 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.858562 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub1/test_in_sub1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.858562 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_conftest_funcargs_only_available_in_subdir/sub2/test_in_sub2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_detect_recursive_dependency_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.862562 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.862562 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_conftest/pkg/test_spam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.862562 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_conftest_module/test_extend_fixture_conftest_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_extend_fixture_module_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_lookup_classlevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_lookup_modulelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/fill_fixtures/test_funcarg_lookupfails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/test_fixture_named_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/fixtures/test_getfixturevalue_dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.862562 pytest-8.1.2/testing/example_scripts/issue88_initial_file_multinodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/issue88_initial_file_multinodes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/issue88_initial_file_multinodes/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/issue88_initial_file_multinodes/test_hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/issue_519.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/junit-10.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.758563 pytest-8.1.2/testing/example_scripts/marks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.862562 pytest-8.1.2/testing/example_scripts/marks/marks_considered_keywords/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/marks/marks_considered_keywords/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/marks/marks_considered_keywords/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/marks/marks_considered_keywords/test_marks_as_keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.758563 pytest-8.1.2/testing/example_scripts/perf_examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.862562 pytest-8.1.2/testing/example_scripts/perf_examples/collect_stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/perf_examples/collect_stats/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/perf_examples/collect_stats/generate_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/perf_examples/collect_stats/template_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.862562 pytest-8.1.2/testing/example_scripts/tmpdir/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/tmpdir/tmp_path_fixture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.866562 pytest-8.1.2/testing/example_scripts/unittest/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/unittest/test_parametrized_fixture_error_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/unittest/test_setup_skip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/unittest/test_setup_skip_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/unittest/test_setup_skip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/unittest/test_unittest_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/unittest/test_unittest_asynctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/unittest/test_unittest_plain_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.866562 pytest-8.1.2/testing/example_scripts/warnings/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/warnings/test_group_warnings_by_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.866562 pytest-8.1.2/testing/example_scripts/warnings/test_group_warnings_by_message_summary/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/warnings/test_group_warnings_by_message_summary/test_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/example_scripts/warnings/test_group_warnings_by_message_summary/test_2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.866562 pytest-8.1.2/testing/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/examples/test_issue519.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.866562 pytest-8.1.2/testing/freeze/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/freeze/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/freeze/create_executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/freeze/runtests_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.866562 pytest-8.1.2/testing/freeze/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/freeze/tests/test_doctest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/freeze/tests/test_trivial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/freeze/tox_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.866562 pytest-8.1.2/testing/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/io/test_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/io/test_saferepr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/io/test_terminalwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/io/test_wcwidth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.866562 pytest-8.1.2/testing/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/logging/test_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/logging/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47293 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/logging/test_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.870562 pytest-8.1.2/testing/plugins_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/plugins_integration/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/plugins_integration/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/plugins_integration/bdd_wallet.feature
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/plugins_integration/bdd_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/plugins_integration/django_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/plugins_integration/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/plugins_integration/pytest_anyio_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/plugins_integration/pytest_asyncio_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/plugins_integration/pytest_mock_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/plugins_integration/pytest_trio_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/plugins_integration/pytest_twisted_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/plugins_integration/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/plugins_integration/simple_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:05:53.870562 pytest-8.1.2/testing/python/
+-rw-r--r--   0 runner    (1001) docker     (127)    35158 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/python/approx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52366 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/python/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)   140883 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/python/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/python/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70079 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/python/metafunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11768 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/python/raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/python/show_fixtures_per_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_argcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65668 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66663 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_assertrewrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45293 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_cacheprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52300 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65092 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79579 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25187 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42797 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50721 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_error_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_faulthandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_findpaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_helpconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57790 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_junitxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_legacypath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_link_resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11332 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34663 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_mark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_mark_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12801 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_parseopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43988 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17284 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_pluginmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27327 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_pytester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_python_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_recwarn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19992 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34598 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_runner_xunit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15424 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_setuponly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_setupplan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43971 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_skipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10633 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98552 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_threadexception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19532 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_tmpdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45389 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_unraisableexception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_warning_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27546 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/test_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-26 17:05:36.000000 pytest-8.1.2/testing/typing_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-26 17:05:36.000000 pytest-8.1.2/tox.ini
```

### Comparing `pytest-8.1.1/.coveragerc` & `pytest-8.1.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/.git-blame-ignore-revs` & `pytest-8.1.2/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/.github/ISSUE_TEMPLATE/2_feature_request.md` & `pytest-8.1.2/.github/ISSUE_TEMPLATE/2_feature_request.md`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/.github/PULL_REQUEST_TEMPLATE.md` & `pytest-8.1.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/.github/labels.toml` & `pytest-8.1.2/.github/labels.toml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/.github/workflows/backport.yml` & `pytest-8.1.2/.github/workflows/backport.yml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/.github/workflows/deploy.yml` & `pytest-8.1.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/.github/workflows/prepare-release-pr.yml` & `pytest-8.1.2/.github/workflows/prepare-release-pr.yml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/.github/workflows/stale.yml` & `pytest-8.1.2/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/.github/workflows/test.yml` & `pytest-8.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/.github/workflows/update-plugin-list.yml` & `pytest-8.1.2/.github/workflows/update-plugin-list.yml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/.gitignore` & `pytest-8.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/.pre-commit-config.yaml` & `pytest-8.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/AUTHORS` & `pytest-8.1.2/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,15 @@
 Pedro Algarvio
 Petter Strandmark
 Philipp Loose
 Pierre Sassoulas
 Pieter Mulder
 Piotr Banaszkiewicz
 Piotr Helm
+Poulami Sau
 Prakhar Gurunani
 Prashant Anand
 Prashant Sharma
 Pulkit Goyal
 Punyashloka Biswal
 Quentin Pradet
 q0w
```

### Comparing `pytest-8.1.1/CODE_OF_CONDUCT.md` & `pytest-8.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/CONTRIBUTING.rst` & `pytest-8.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/LICENSE` & `pytest-8.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/OPENCOLLECTIVE.rst` & `pytest-8.1.2/OPENCOLLECTIVE.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/PKG-INFO` & `pytest-8.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest
-Version: 8.1.1
+Version: 8.1.2
 Summary: pytest: simple powerful testing with Python
 Author: Holger Krekel, Bruno Oliveira, Ronny Pfannschmidt, Floris Bruynooghe, Brianna Laugher, Florian Bruhin, Others (See AUTHORS)
 License: MIT
 Project-URL: Changelog, https://docs.pytest.org/en/stable/changelog.html
 Project-URL: Homepage, https://docs.pytest.org/en/latest/
 Project-URL: Source, https://github.com/pytest-dev/pytest
 Project-URL: Tracker, https://github.com/pytest-dev/pytest/issues
```

### Comparing `pytest-8.1.1/README.rst` & `pytest-8.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/RELEASING.rst` & `pytest-8.1.2/RELEASING.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/TIDELIFT.rst` & `pytest-8.1.2/TIDELIFT.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/bench/bench_argcomplete.py` & `pytest-8.1.2/bench/bench_argcomplete.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/changelog/README.rst` & `pytest-8.1.2/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/changelog/_template.rst` & `pytest-8.1.2/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/Makefile` & `pytest-8.1.2/doc/en/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/_templates/globaltoc.html` & `pytest-8.1.2/doc/en/_templates/globaltoc.html`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/_templates/layout.html` & `pytest-8.1.2/doc/en/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/_templates/relations.html` & `pytest-8.1.2/doc/en/_templates/relations.html`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/_templates/slim_searchbox.html` & `pytest-8.1.2/doc/en/_templates/slim_searchbox.html`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/adopt.rst` & `pytest-8.1.2/doc/en/adopt.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/index.rst` & `pytest-8.1.2/doc/en/announce/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Release announcements
 ===========================================
 
 .. toctree::
    :maxdepth: 2
 
 
+   release-8.1.2
    release-8.1.1
    release-8.1.0
    release-8.0.2
    release-8.0.1
    release-8.0.0
    release-8.0.0rc2
    release-8.0.0rc1
```

### Comparing `pytest-8.1.1/doc/en/announce/release-2.0.0.rst` & `pytest-8.1.2/doc/en/announce/release-2.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.0.1.rst` & `pytest-8.1.2/doc/en/announce/release-2.0.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.0.2.rst` & `pytest-8.1.2/doc/en/announce/release-2.0.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.0.3.rst` & `pytest-8.1.2/doc/en/announce/release-2.0.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.1.0.rst` & `pytest-8.1.2/doc/en/announce/release-2.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.1.1.rst` & `pytest-8.1.2/doc/en/announce/release-2.1.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.1.2.rst` & `pytest-8.1.2/doc/en/announce/release-2.1.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.1.3.rst` & `pytest-8.1.2/doc/en/announce/release-2.1.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.2.0.rst` & `pytest-8.1.2/doc/en/announce/release-2.2.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.2.1.rst` & `pytest-8.1.2/doc/en/announce/release-2.2.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.2.2.rst` & `pytest-8.1.2/doc/en/announce/release-2.2.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.2.4.rst` & `pytest-8.1.2/doc/en/announce/release-2.2.4.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.3.0.rst` & `pytest-8.1.2/doc/en/announce/release-2.3.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.3.1.rst` & `pytest-8.1.2/doc/en/announce/release-2.3.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.3.2.rst` & `pytest-8.1.2/doc/en/announce/release-2.3.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.3.3.rst` & `pytest-8.1.2/doc/en/announce/release-2.3.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.3.4.rst` & `pytest-8.1.2/doc/en/announce/release-2.3.4.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.3.5.rst` & `pytest-8.1.2/doc/en/announce/release-2.3.5.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.4.0.rst` & `pytest-8.1.2/doc/en/announce/release-2.4.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.4.1.rst` & `pytest-8.1.2/doc/en/announce/release-2.4.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.4.2.rst` & `pytest-8.1.2/doc/en/announce/release-2.4.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.5.0.rst` & `pytest-8.1.2/doc/en/announce/release-2.5.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.5.1.rst` & `pytest-8.1.2/doc/en/announce/release-2.5.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.5.2.rst` & `pytest-8.1.2/doc/en/announce/release-2.5.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.6.0.rst` & `pytest-8.1.2/doc/en/announce/release-2.6.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.6.1.rst` & `pytest-8.1.2/doc/en/announce/release-2.6.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.6.2.rst` & `pytest-8.1.2/doc/en/announce/release-2.6.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.6.3.rst` & `pytest-8.1.2/doc/en/announce/release-2.6.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.7.0.rst` & `pytest-8.1.2/doc/en/announce/release-2.7.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.7.1.rst` & `pytest-8.1.2/doc/en/announce/release-2.7.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.7.2.rst` & `pytest-8.1.2/doc/en/announce/release-2.7.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.8.2.rst` & `pytest-8.1.2/doc/en/announce/release-2.8.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.8.3.rst` & `pytest-8.1.2/doc/en/announce/release-2.8.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.8.4.rst` & `pytest-8.1.2/doc/en/announce/release-2.8.4.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.8.5.rst` & `pytest-8.1.2/doc/en/announce/release-2.8.5.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.8.6.rst` & `pytest-8.1.2/doc/en/announce/release-2.8.6.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.8.7.rst` & `pytest-8.1.2/doc/en/announce/release-2.8.7.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.9.0.rst` & `pytest-8.1.2/doc/en/announce/release-2.9.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.9.1.rst` & `pytest-8.1.2/doc/en/announce/release-2.9.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-2.9.2.rst` & `pytest-8.1.2/doc/en/announce/release-2.9.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.0.0.rst` & `pytest-8.1.2/doc/en/announce/release-3.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.0.1.rst` & `pytest-8.1.2/doc/en/announce/release-3.0.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.0.2.rst` & `pytest-8.1.2/doc/en/announce/release-3.0.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.0.3.rst` & `pytest-8.1.2/doc/en/announce/release-3.0.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.0.4.rst` & `pytest-8.1.2/doc/en/announce/release-3.0.4.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.0.5.rst` & `pytest-8.1.2/doc/en/announce/release-3.0.5.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.0.6.rst` & `pytest-8.1.2/doc/en/announce/release-3.0.6.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.0.7.rst` & `pytest-8.1.2/doc/en/announce/release-3.0.7.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.1.0.rst` & `pytest-8.1.2/doc/en/announce/release-3.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.10.0.rst` & `pytest-8.1.2/doc/en/announce/release-3.10.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.10.1.rst` & `pytest-8.1.2/doc/en/announce/release-3.10.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.2.0.rst` & `pytest-8.1.2/doc/en/announce/release-3.2.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.2.2.rst` & `pytest-8.1.2/doc/en/announce/release-3.2.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.2.4.rst` & `pytest-8.1.2/doc/en/announce/release-3.2.4.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.3.0.rst` & `pytest-8.1.2/doc/en/announce/release-3.3.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.3.1.rst` & `pytest-8.1.2/doc/en/announce/release-3.3.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.3.2.rst` & `pytest-8.1.2/doc/en/announce/release-3.3.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.4.0.rst` & `pytest-8.1.2/doc/en/announce/release-3.4.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.4.1.rst` & `pytest-8.1.2/doc/en/announce/release-3.4.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.4.2.rst` & `pytest-8.1.2/doc/en/announce/release-3.4.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.5.0.rst` & `pytest-8.1.2/doc/en/announce/release-3.5.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.5.1.rst` & `pytest-8.1.2/doc/en/announce/release-3.5.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.6.0.rst` & `pytest-8.1.2/doc/en/announce/release-3.6.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.6.1.rst` & `pytest-8.1.2/doc/en/announce/release-3.6.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.6.2.rst` & `pytest-8.1.2/doc/en/announce/release-3.6.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.6.3.rst` & `pytest-8.1.2/doc/en/announce/release-3.6.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.7.0.rst` & `pytest-8.1.2/doc/en/announce/release-3.7.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.7.2.rst` & `pytest-8.1.2/doc/en/announce/release-3.7.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.7.3.rst` & `pytest-8.1.2/doc/en/announce/release-3.7.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.8.0.rst` & `pytest-8.1.2/doc/en/announce/release-3.8.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.8.1.rst` & `pytest-8.1.2/doc/en/announce/release-3.8.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.8.2.rst` & `pytest-8.1.2/doc/en/announce/release-3.8.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-3.9.0.rst` & `pytest-8.1.2/doc/en/announce/release-3.9.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-4.0.0.rst` & `pytest-8.1.2/doc/en/announce/release-4.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-4.1.0.rst` & `pytest-8.1.2/doc/en/announce/release-4.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-4.1.1.rst` & `pytest-8.1.2/doc/en/announce/release-4.1.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-4.2.0.rst` & `pytest-8.1.2/doc/en/announce/release-4.2.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-4.2.1.rst` & `pytest-8.1.2/doc/en/announce/release-4.2.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-4.3.0.rst` & `pytest-8.1.2/doc/en/announce/release-4.3.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-4.3.1.rst` & `pytest-8.1.2/doc/en/announce/release-4.3.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-4.4.0.rst` & `pytest-8.1.2/doc/en/announce/release-4.4.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-4.4.2.rst` & `pytest-8.1.2/doc/en/announce/release-4.4.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-4.5.0.rst` & `pytest-8.1.2/doc/en/announce/release-4.5.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-4.6.0.rst` & `pytest-8.1.2/doc/en/announce/release-4.6.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-5.0.0.rst` & `pytest-8.1.2/doc/en/announce/release-5.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-5.0.1.rst` & `pytest-8.1.2/doc/en/announce/release-5.0.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-5.1.0.rst` & `pytest-8.1.2/doc/en/announce/release-5.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-5.1.1.rst` & `pytest-8.1.2/doc/en/announce/release-5.1.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-5.2.0.rst` & `pytest-8.1.2/doc/en/announce/release-5.2.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-5.2.2.rst` & `pytest-8.1.2/doc/en/announce/release-5.2.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-5.2.3.rst` & `pytest-8.1.2/doc/en/announce/release-5.2.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-5.3.0.rst` & `pytest-8.1.2/doc/en/announce/release-5.3.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-5.3.1.rst` & `pytest-8.1.2/doc/en/announce/release-5.3.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-5.3.2.rst` & `pytest-8.1.2/doc/en/announce/release-5.3.2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-5.3.3.rst` & `pytest-8.1.2/doc/en/announce/release-5.3.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-5.4.0.rst` & `pytest-8.1.2/doc/en/announce/release-5.4.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-6.0.0.rst` & `pytest-8.1.2/doc/en/announce/release-6.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-6.0.0rc1.rst` & `pytest-8.1.2/doc/en/announce/release-6.0.0rc1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-6.1.0.rst` & `pytest-8.1.2/doc/en/announce/release-6.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-6.2.0.rst` & `pytest-8.1.2/doc/en/announce/release-6.2.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-6.2.5.rst` & `pytest-8.1.2/doc/en/announce/release-6.2.5.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-7.0.0.rst` & `pytest-8.1.2/doc/en/announce/release-7.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-7.0.0rc1.rst` & `pytest-8.1.2/doc/en/announce/release-7.0.0rc1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-7.1.0.rst` & `pytest-8.1.2/doc/en/announce/release-7.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-7.1.3.rst` & `pytest-8.1.2/doc/en/announce/release-7.1.3.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-7.2.0.rst` & `pytest-8.1.2/doc/en/announce/release-7.2.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-7.2.1.rst` & `pytest-8.1.2/doc/en/announce/release-7.2.1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-7.3.0.rst` & `pytest-8.1.2/doc/en/announce/release-7.3.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-7.4.0.rst` & `pytest-8.1.2/doc/en/announce/release-7.4.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-8.0.0.rst` & `pytest-8.1.2/doc/en/announce/release-8.0.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-8.0.0rc1.rst` & `pytest-8.1.2/doc/en/announce/release-8.0.0rc1.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-8.0.0rc2.rst` & `pytest-8.1.2/doc/en/announce/release-8.0.0rc2.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/release-8.1.0.rst` & `pytest-8.1.2/doc/en/announce/release-8.1.0.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/announce/sprint2016.rst` & `pytest-8.1.2/doc/en/announce/sprint2016.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/backwards-compatibility.rst` & `pytest-8.1.2/doc/en/backwards-compatibility.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/builtin.rst` & `pytest-8.1.2/doc/en/builtin.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/changelog.rst` & `pytest-8.1.2/doc/en/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,23 @@
     .. The 'changelog_towncrier_draft' tag is included by our 'tox -e docs',
        but not on readthedocs.
 
     .. include:: _changelog_towncrier_draft.rst
 
 .. towncrier release notes start
 
+pytest 8.1.2 (2024-04-26)
+=========================
+
+Bug Fixes
+---------
+
+- `#12114 <https://github.com/pytest-dev/pytest/issues/12114>`_: Fixed error in :func:`pytest.approx` when used with `numpy` arrays and comparing with other types.
+
+
 pytest 8.1.1 (2024-03-08)
 =========================
 
 .. note::
 
        This release is not a usual bug fix release -- it contains features and improvements, being a follow up
        to ``8.1.0``, which has been yanked from PyPI.
```

### Comparing `pytest-8.1.1/doc/en/conf.py` & `pytest-8.1.2/doc/en/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 # A unique identification for the text.
 # epub_uid = ''
 
 # HTML files that should be inserted before the pages created by sphinx.
 # The format is a list of tuples containing the path and title.
 # epub_pre_files = []
 
-# HTML files shat should be inserted after the pages created by sphinx.
+# HTML files that should be inserted after the pages created by sphinx.
 # The format is a list of tuples containing the path and title.
 # epub_post_files = []
 
 # A list of files that should not be packed into the epub file.
 # epub_exclude_files = []
 
 # The depth of the table of contents in toc.ncx.
```

### Comparing `pytest-8.1.1/doc/en/contact.rst` & `pytest-8.1.2/doc/en/contact.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/contents.rst` & `pytest-8.1.2/doc/en/contents.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/deprecations.rst` & `pytest-8.1.2/doc/en/deprecations.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/assertion/failure_demo.py` & `pytest-8.1.2/doc/en/example/assertion/failure_demo.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/assertion/test_setup_flow_example.py` & `pytest-8.1.2/doc/en/example/assertion/test_setup_flow_example.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/attic.rst` & `pytest-8.1.2/doc/en/example/attic.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/customdirectory/conftest.py` & `pytest-8.1.2/doc/en/example/customdirectory/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/customdirectory.rst` & `pytest-8.1.2/doc/en/example/customdirectory.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/fixture_availability.svg` & `pytest-8.1.2/doc/en/example/fixtures/fixture_availability.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/fixture_availability_plugins.svg` & `pytest-8.1.2/doc/en/example/fixtures/fixture_availability_plugins.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse.py` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse.svg` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_flat.svg` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse_flat.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.py` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.svg` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse_multiple_scopes.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.py` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.svg` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_autouse_temp_effects.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies.py` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_dependencies.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies.svg` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_dependencies.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies_flat.svg` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_dependencies_flat.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_dependencies_unclear.svg` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_dependencies_unclear.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_scope.py` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_scope.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_order_scope.svg` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_order_scope.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/fixtures/test_fixtures_request_different_scope.svg` & `pytest-8.1.2/doc/en/example/fixtures/test_fixtures_request_different_scope.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/index.rst` & `pytest-8.1.2/doc/en/example/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/markers.rst` & `pytest-8.1.2/doc/en/example/markers.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/multipython.py` & `pytest-8.1.2/doc/en/example/multipython.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/nonpython/conftest.py` & `pytest-8.1.2/doc/en/example/nonpython/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/nonpython.rst` & `pytest-8.1.2/doc/en/example/nonpython.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/parametrize.rst` & `pytest-8.1.2/doc/en/example/parametrize.rst`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
     $ pytest test_time.py --collect-only
     =========================== test session starts ============================
     platform linux -- Python 3.x.y, pytest-8.x.y, pluggy-1.x.y
     rootdir: /home/sweet/project
     collected 8 items
 
-    <Dir parametrize.rst-196>
+    <Dir parametrize.rst-197>
       <Module test_time.py>
         <Function test_timedistance_v0[a0-b0-expected0]>
         <Function test_timedistance_v0[a1-b1-expected1]>
         <Function test_timedistance_v1[forward]>
         <Function test_timedistance_v1[backward]>
         <Function test_timedistance_v2[20011212-20011211-expected0]>
         <Function test_timedistance_v2[20011211-20011212-expected1]>
@@ -235,15 +235,15 @@
 
     $ pytest --collect-only test_scenarios.py
     =========================== test session starts ============================
     platform linux -- Python 3.x.y, pytest-8.x.y, pluggy-1.x.y
     rootdir: /home/sweet/project
     collected 4 items
 
-    <Dir parametrize.rst-196>
+    <Dir parametrize.rst-197>
       <Module test_scenarios.py>
         <Class TestSampleWithScenarios>
           <Function test_demo1[basic]>
           <Function test_demo2[basic]>
           <Function test_demo1[advanced]>
           <Function test_demo2[advanced]>
 
@@ -314,15 +314,15 @@
 
     $ pytest test_backends.py --collect-only
     =========================== test session starts ============================
     platform linux -- Python 3.x.y, pytest-8.x.y, pluggy-1.x.y
     rootdir: /home/sweet/project
     collected 2 items
 
-    <Dir parametrize.rst-196>
+    <Dir parametrize.rst-197>
       <Module test_backends.py>
         <Function test_db_initialized[d1]>
         <Function test_db_initialized[d2]>
 
     ======================== 2 tests collected in 0.12s ========================
 
 And then when we run the test:
```

### Comparing `pytest-8.1.1/doc/en/example/pythoncollection.rst` & `pytest-8.1.2/doc/en/example/pythoncollection.rst`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     $ pytest --collect-only
     =========================== test session starts ============================
     platform linux -- Python 3.x.y, pytest-8.x.y, pluggy-1.x.y
     rootdir: /home/sweet/project
     configfile: pytest.ini
     collected 2 items
 
-    <Dir pythoncollection.rst-197>
+    <Dir pythoncollection.rst-198>
       <Module check_myapp.py>
         <Class CheckMyApp>
           <Function simple_check>
           <Function complex_check>
 
     ======================== 2 tests collected in 0.12s ========================
 
@@ -211,15 +211,15 @@
     . $ pytest --collect-only pythoncollection.py
     =========================== test session starts ============================
     platform linux -- Python 3.x.y, pytest-8.x.y, pluggy-1.x.y
     rootdir: /home/sweet/project
     configfile: pytest.ini
     collected 3 items
 
-    <Dir pythoncollection.rst-197>
+    <Dir pythoncollection.rst-198>
       <Dir CWD>
         <Module pythoncollection.py>
           <Function test_function>
           <Class TestClass>
             <Function test_method>
             <Function test_anothermethod>
```

### Comparing `pytest-8.1.1/doc/en/example/reportingdemo.rst` & `pytest-8.1.2/doc/en/example/reportingdemo.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/simple.rst` & `pytest-8.1.2/doc/en/example/simple.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/example/special.rst` & `pytest-8.1.2/doc/en/example/special.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/explanation/anatomy.rst` & `pytest-8.1.2/doc/en/explanation/anatomy.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/explanation/fixtures.rst` & `pytest-8.1.2/doc/en/explanation/fixtures.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/explanation/flaky.rst` & `pytest-8.1.2/doc/en/explanation/flaky.rst`

 * *Files 4% similar despite different names*

```diff
@@ -48,18 +48,17 @@
 
 
 Plugins
 ~~~~~~~
 
 Rerunning any failed tests can mitigate the negative effects of flaky tests by giving them additional chances to pass, so that the overall build does not fail. Several pytest plugins support this:
 
-* `flaky <https://github.com/box/flaky>`_
-* `pytest-flakefinder <https://github.com/dropbox/pytest-flakefinder>`_ - `blog post <https://blogs.dropbox.com/tech/2016/03/open-sourcing-pytest-tools/>`_
 * `pytest-rerunfailures <https://github.com/pytest-dev/pytest-rerunfailures>`_
 * `pytest-replay <https://github.com/ESSS/pytest-replay>`_: This plugin helps to reproduce locally crashes or flaky tests observed during CI runs.
+* `pytest-flakefinder <https://github.com/dropbox/pytest-flakefinder>`_ - `blog post <https://blogs.dropbox.com/tech/2016/03/open-sourcing-pytest-tools/>`_
 
 Plugins to deliberately randomize tests can help expose tests with state problems:
 
 * `pytest-random-order <https://github.com/jbasko/pytest-random-order>`_
 * `pytest-randomly <https://github.com/pytest-dev/pytest-randomly>`_
 
 
@@ -102,15 +101,15 @@
 ^^^^^^^^
 
 This is a limited list, please submit an issue or pull request to expand it!
 
 * Gao, Zebao, Yalan Liang, Myra B. Cohen, Atif M. Memon, and Zhen Wang. "Making system user interactive tests repeatable: When and what should we control?." In *Software Engineering (ICSE), 2015 IEEE/ACM 37th IEEE International Conference on*, vol. 1, pp. 55-65. IEEE, 2015.  `PDF <http://www.cs.umd.edu/~atif/pubs/gao-icse15.pdf>`__
 * Palomba, Fabio, and Andy Zaidman. "Does refactoring of test smells induce fixing flaky tests?." In *Software Maintenance and Evolution (ICSME), 2017 IEEE International Conference on*, pp. 1-12. IEEE, 2017. `PDF in Google Drive <https://drive.google.com/file/d/10HdcCQiuQVgW3yYUJD-TSTq1NbYEprl0/view>`__
 *  Bell, Jonathan, Owolabi Legunsen, Michael Hilton, Lamyaa Eloussi, Tifany Yung, and Darko Marinov. "DeFlaker: Automatically detecting flaky tests." In *Proceedings of the 2018 International Conference on Software Engineering*. 2018. `PDF <https://www.jonbell.net/icse18-deflaker.pdf>`__
-
+*  Dutta, Saikat and Shi, August and Choudhary, Rutvik and Zhang, Zhekun and Jain, Aryaman and Misailovic, Sasa. "Detecting flaky tests in probabilistic and machine learning applications." In *Proceedings of the 29th ACM SIGSOFT International Symposium on Software Testing and Analysis (ISSTA)*, pp. 211-224. ACM, 2020. `PDF <https://www.cs.cornell.edu/~saikatd/papers/flash-issta20.pdf>`__
 
 Resources
 ^^^^^^^^^
 
 * `Eradicating Non-Determinism in Tests <https://martinfowler.com/articles/nonDeterminism.html>`_ by Martin Fowler, 2011
 * `No more flaky tests on the Go team <https://www.thoughtworks.com/insights/blog/no-more-flaky-tests-go-team>`_ by Pavan Sudarshan, 2012
 * `The Build That Cried Broken: Building Trust in your Continuous Integration Tests <https://www.youtube.com/embed/VotJqV4n8ig>`_ talk (video) by `Angie Jones <https://angiejones.tech/>`_ at SeleniumConf Austin 2017
```

### Comparing `pytest-8.1.1/doc/en/explanation/goodpractices.rst` & `pytest-8.1.2/doc/en/explanation/goodpractices.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/explanation/pythonpath.rst` & `pytest-8.1.2/doc/en/explanation/pythonpath.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/funcarg_compare.rst` & `pytest-8.1.2/doc/en/funcarg_compare.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/getting-started.rst` & `pytest-8.1.2/doc/en/getting-started.rst`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     pip install -U pytest
 
 2. Check that you installed the correct version:
 
 .. code-block:: bash
 
     $ pytest --version
-    pytest 8.1.1
+    pytest 8.1.2
 
 .. _`simpletest`:
 
 Create your first test
 ----------------------------------------------------------
 
 Create a new file called ``test_sample.py``, containing a function, and a test:
```

### Comparing `pytest-8.1.1/doc/en/historical-notes.rst` & `pytest-8.1.2/doc/en/historical-notes.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/history.rst` & `pytest-8.1.2/doc/en/history.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/assert.rst` & `pytest-8.1.2/doc/en/how-to/assert.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/bash-completion.rst` & `pytest-8.1.2/doc/en/how-to/bash-completion.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/cache.rst` & `pytest-8.1.2/doc/en/how-to/cache.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/capture-stdout-stderr.rst` & `pytest-8.1.2/doc/en/how-to/capture-stdout-stderr.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/capture-warnings.rst` & `pytest-8.1.2/doc/en/how-to/capture-warnings.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/doctest.rst` & `pytest-8.1.2/doc/en/how-to/doctest.rst`

 * *Files 0% similar despite different names*

```diff
@@ -220,14 +220,15 @@
 
 ``doctest_namespace`` is a standard ``dict`` object into which you
 place the objects you want to appear in the doctest namespace:
 
 .. code-block:: python
 
     # content of conftest.py
+    import pytest
     import numpy
 
 
     @pytest.fixture(autouse=True)
     def add_np(doctest_namespace):
         doctest_namespace["np"] = numpy
```

### Comparing `pytest-8.1.1/doc/en/how-to/existingtestsuite.rst` & `pytest-8.1.2/doc/en/how-to/existingtestsuite.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/failures.rst` & `pytest-8.1.2/doc/en/how-to/failures.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/fixtures.rst` & `pytest-8.1.2/doc/en/how-to/fixtures.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1414,15 +1414,15 @@
 
    $ pytest --collect-only
    =========================== test session starts ============================
    platform linux -- Python 3.x.y, pytest-8.x.y, pluggy-1.x.y
    rootdir: /home/sweet/project
    collected 12 items
 
-   <Dir fixtures.rst-215>
+   <Dir fixtures.rst-216>
      <Module test_anothersmtp.py>
        <Function test_showhelo[smtp.gmail.com]>
        <Function test_showhelo[mail.python.org]>
      <Module test_emaillib.py>
        <Function test_email_received>
      <Module test_finalizers.py>
        <Function test_bar>
```

### Comparing `pytest-8.1.1/doc/en/how-to/index.rst` & `pytest-8.1.2/doc/en/how-to/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/logging.rst` & `pytest-8.1.2/doc/en/how-to/logging.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/mark.rst` & `pytest-8.1.2/doc/en/how-to/mark.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/monkeypatch.rst` & `pytest-8.1.2/doc/en/how-to/monkeypatch.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/output.rst` & `pytest-8.1.2/doc/en/how-to/output.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/parametrize.rst` & `pytest-8.1.2/doc/en/how-to/parametrize.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/plugins.rst` & `pytest-8.1.2/doc/en/how-to/plugins.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/skipping.rst` & `pytest-8.1.2/doc/en/how-to/skipping.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/tmp_path.rst` & `pytest-8.1.2/doc/en/how-to/tmp_path.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/unittest.rst` & `pytest-8.1.2/doc/en/how-to/unittest.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/usage.rst` & `pytest-8.1.2/doc/en/how-to/usage.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/writing_hook_functions.rst` & `pytest-8.1.2/doc/en/how-to/writing_hook_functions.rst`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 In other cases, the wrapper wants the adjust or adapt the result, in which case
 it can return a new value. If the result of the underlying hook is a mutable
 object, the wrapper may modify that result, but it's probably better to avoid it.
 
 If the hook implementation failed with an exception, the wrapper can handle that
 exception using a ``try-catch-finally`` around the ``yield``, by propagating it,
-supressing it, or raising a different exception entirely.
+suppressing it, or raising a different exception entirely.
 
 For more information, consult the
 :ref:`pluggy documentation about hook wrappers <pluggy:hookwrappers>`.
 
 .. _plugin-hookorder:
 
 Hook function ordering / call example
```

### Comparing `pytest-8.1.1/doc/en/how-to/writing_plugins.rst` & `pytest-8.1.2/doc/en/how-to/writing_plugins.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/how-to/xunit_setup.rst` & `pytest-8.1.2/doc/en/how-to/xunit_setup.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/img/cramer2.png` & `pytest-8.1.2/doc/en/img/cramer2.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/img/favicon.png` & `pytest-8.1.2/doc/en/img/favicon.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/img/freiburg2.jpg` & `pytest-8.1.2/doc/en/img/freiburg2.jpg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/img/gaynor3.png` & `pytest-8.1.2/doc/en/img/gaynor3.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/img/keleshev.png` & `pytest-8.1.2/doc/en/img/keleshev.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/img/pullrequest.png` & `pytest-8.1.2/doc/en/img/pullrequest.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/img/pylib.png` & `pytest-8.1.2/doc/en/img/pylib.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/img/pytest1.png` & `pytest-8.1.2/doc/en/img/pytest1.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/img/pytest_logo_curves.svg` & `pytest-8.1.2/doc/en/img/pytest_logo_curves.svg`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/img/theuni.png` & `pytest-8.1.2/doc/en/img/theuni.png`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/index.rst` & `pytest-8.1.2/doc/en/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 :orphan:
 
 .. sidebar:: Next Open Trainings and Events
 
    - `Professional Testing with Python <https://python-academy.com/courses/python_course_testing.html>`_, via `Python Academy <https://www.python-academy.com/>`_ (3 day in-depth training):
       * **June 11th to 13th 2024**, Remote
       * **March 4th to 6th 2025**, Leipzig, Germany / Remote
-   - `pytest development sprint <https://github.com/pytest-dev/pytest/discussions/11655>`_, June 2024 (`date poll <https://nuudel.digitalcourage.de/2tEsEpRcwMNcAXVO>`_)
+   - `pytest development sprint <https://github.com/pytest-dev/pytest/discussions/11655>`_, **June 17th -- 22nd 2024**
+   - pytest tips and tricks for a better testsuite, `Europython 2024 <https://ep2024.europython.eu/>`_, **July 8th -- 14th 2024** (3h), Prague
 
    Also see :doc:`previous talks and blogposts <talks>`.
 
 .. _features:
 
 pytest: helps you write better programs
 =======================================
@@ -83,15 +84,15 @@
 
 - Rich plugin architecture, with over 1300+ :ref:`external plugins <plugin-list>` and thriving community
 
 
 Documentation
 -------------
 
-* :ref:`Get started <get-started>` - install pytest and grasp its basics just twenty minutes
+* :ref:`Get started <get-started>` - install pytest and grasp its basics in just twenty minutes
 * :ref:`How-to guides <how-to>` - step-by-step guides, covering a vast range of use-cases and needs
 * :ref:`Reference guides <reference>` - includes the complete pytest API reference, lists of plugins and more
 * :ref:`Explanation <explanation>` - background, discussion of key topics, answers to higher-level questions
 
 
 Bugs/Requests
 -------------
```

### Comparing `pytest-8.1.1/doc/en/license.rst` & `pytest-8.1.2/doc/en/license.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/naming20.rst` & `pytest-8.1.2/doc/en/naming20.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/proposals/parametrize_with_fixtures.rst` & `pytest-8.1.2/doc/en/proposals/parametrize_with_fixtures.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/reference/customize.rst` & `pytest-8.1.2/doc/en/reference/customize.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/reference/exit-codes.rst` & `pytest-8.1.2/doc/en/reference/exit-codes.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/reference/fixtures.rst` & `pytest-8.1.2/doc/en/reference/fixtures.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/reference/plugin_list.rst` & `pytest-8.1.2/doc/en/reference/plugin_list.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/reference/reference.rst` & `pytest-8.1.2/doc/en/reference/reference.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/sponsor.rst` & `pytest-8.1.2/doc/en/sponsor.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/talks.rst` & `pytest-8.1.2/doc/en/talks.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/doc/en/tidelift.rst` & `pytest-8.1.2/doc/en/tidelift.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/extra/get_issues.py` & `pytest-8.1.2/extra/get_issues.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/pyproject.toml` & `pytest-8.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/scripts/generate-gh-release-notes.py` & `pytest-8.1.2/scripts/generate-gh-release-notes.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/scripts/prepare-release-pr.py` & `pytest-8.1.2/scripts/prepare-release-pr.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/scripts/release.major.rst` & `pytest-8.1.2/scripts/release.major.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/scripts/release.minor.rst` & `pytest-8.1.2/scripts/release.minor.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/scripts/release.pre.rst` & `pytest-8.1.2/scripts/release.pre.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/scripts/release.py` & `pytest-8.1.2/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/scripts/update-plugin-list.py` & `pytest-8.1.2/scripts/update-plugin-list.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/_argcomplete.py` & `pytest-8.1.2/src/_pytest/_argcomplete.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/_code/code.py` & `pytest-8.1.2/src/_pytest/_code/code.py`

 * *Files 0% similar despite different names*

```diff
@@ -784,14 +784,16 @@
             To match a literal string that may contain :ref:`special characters
             <re-syntax>`, the pattern can first be escaped with :func:`re.escape`.
 
         :param Optional[int] depth:
             If `None`, will search for a matching exception at any nesting depth.
             If >= 1, will only match an exception if it's at the specified depth (depth = 1 being
             the exceptions contained within the topmost exception group).
+
+        .. versionadded:: 8.0
         """
         msg = "Captured exception is not an instance of `BaseExceptionGroup`"
         assert isinstance(self.value, BaseExceptionGroup), msg
         msg = "`depth` must be >= 1 if specified"
         assert (depth is None) or (depth >= 1), msg
         return self._group_contains(self.value, expected_exception, match, depth)
```

### Comparing `pytest-8.1.1/src/_pytest/_code/source.py` & `pytest-8.1.2/src/_pytest/_code/source.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/_io/pprint.py` & `pytest-8.1.2/src/_pytest/_io/pprint.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/_io/saferepr.py` & `pytest-8.1.2/src/_pytest/_io/saferepr.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/_io/terminalwriter.py` & `pytest-8.1.2/src/_pytest/_io/terminalwriter.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/_io/wcwidth.py` & `pytest-8.1.2/src/_pytest/_io/wcwidth.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/_py/error.py` & `pytest-8.1.2/src/_pytest/_py/error.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/_py/path.py` & `pytest-8.1.2/src/_pytest/_py/path.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/assertion/__init__.py` & `pytest-8.1.2/src/_pytest/assertion/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/assertion/rewrite.py` & `pytest-8.1.2/src/_pytest/assertion/rewrite.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/assertion/truncate.py` & `pytest-8.1.2/src/_pytest/assertion/truncate.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/assertion/util.py` & `pytest-8.1.2/src/_pytest/assertion/util.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/cacheprovider.py` & `pytest-8.1.2/src/_pytest/cacheprovider.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/capture.py` & `pytest-8.1.2/src/_pytest/capture.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/compat.py` & `pytest-8.1.2/src/_pytest/compat.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/config/__init__.py` & `pytest-8.1.2/src/_pytest/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/config/argparsing.py` & `pytest-8.1.2/src/_pytest/config/argparsing.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/config/compat.py` & `pytest-8.1.2/src/_pytest/config/compat.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/config/findpaths.py` & `pytest-8.1.2/src/_pytest/config/findpaths.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/debugging.py` & `pytest-8.1.2/src/_pytest/debugging.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/deprecated.py` & `pytest-8.1.2/src/_pytest/deprecated.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/doctest.py` & `pytest-8.1.2/src/_pytest/doctest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/faulthandler.py` & `pytest-8.1.2/src/_pytest/faulthandler.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/fixtures.py` & `pytest-8.1.2/src/_pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/freeze_support.py` & `pytest-8.1.2/src/_pytest/freeze_support.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/helpconfig.py` & `pytest-8.1.2/src/_pytest/helpconfig.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/hookspec.py` & `pytest-8.1.2/src/_pytest/hookspec.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/junitxml.py` & `pytest-8.1.2/src/_pytest/junitxml.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/legacypath.py` & `pytest-8.1.2/src/_pytest/legacypath.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/logging.py` & `pytest-8.1.2/src/_pytest/logging.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/main.py` & `pytest-8.1.2/src/_pytest/main.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/mark/__init__.py` & `pytest-8.1.2/src/_pytest/mark/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/mark/expression.py` & `pytest-8.1.2/src/_pytest/mark/expression.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/mark/structures.py` & `pytest-8.1.2/src/_pytest/mark/structures.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/monkeypatch.py` & `pytest-8.1.2/src/_pytest/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/nodes.py` & `pytest-8.1.2/src/_pytest/nodes.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/outcomes.py` & `pytest-8.1.2/src/_pytest/outcomes.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/pastebin.py` & `pytest-8.1.2/src/_pytest/pastebin.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/pathlib.py` & `pytest-8.1.2/src/_pytest/pathlib.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/pytester.py` & `pytest-8.1.2/src/_pytest/pytester.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/pytester_assertions.py` & `pytest-8.1.2/src/_pytest/pytester_assertions.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/python.py` & `pytest-8.1.2/src/_pytest/python.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/python_api.py` & `pytest-8.1.2/src/_pytest/python_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
     def __repr__(self) -> str:
         list_scalars = _recursive_sequence_map(
             self._approx_scalar, self.expected.tolist()
         )
         return f"approx({list_scalars!r})"
 
-    def _repr_compare(self, other_side: "ndarray") -> List[str]:
+    def _repr_compare(self, other_side: Union["ndarray", List[Any]]) -> List[str]:
         import itertools
         import math
 
         def get_value_from_nested_list(
             nested_list: List[Any], nd_index: Tuple[Any, ...]
         ) -> Any:
             """
@@ -159,40 +159,44 @@
             return value
 
         np_array_shape = self.expected.shape
         approx_side_as_seq = _recursive_sequence_map(
             self._approx_scalar, self.expected.tolist()
         )
 
-        if np_array_shape != other_side.shape:
+        # Convert other_side to numpy array to ensure shape attribute is available.
+        other_side_as_array = _as_numpy_array(other_side)
+        assert other_side_as_array is not None
+
+        if np_array_shape != other_side_as_array.shape:
             return [
                 "Impossible to compare arrays with different shapes.",
-                f"Shapes: {np_array_shape} and {other_side.shape}",
+                f"Shapes: {np_array_shape} and {other_side_as_array.shape}",
             ]
 
         number_of_elements = self.expected.size
         max_abs_diff = -math.inf
         max_rel_diff = -math.inf
         different_ids = []
         for index in itertools.product(*(range(i) for i in np_array_shape)):
             approx_value = get_value_from_nested_list(approx_side_as_seq, index)
-            other_value = get_value_from_nested_list(other_side, index)
+            other_value = get_value_from_nested_list(other_side_as_array, index)
             if approx_value != other_value:
                 abs_diff = abs(approx_value.expected - other_value)
                 max_abs_diff = max(max_abs_diff, abs_diff)
                 if other_value == 0.0:
                     max_rel_diff = math.inf
                 else:
                     max_rel_diff = max(max_rel_diff, abs_diff / abs(other_value))
                 different_ids.append(index)
 
         message_data = [
             (
                 str(index),
-                str(get_value_from_nested_list(other_side, index)),
+                str(get_value_from_nested_list(other_side_as_array, index)),
                 str(get_value_from_nested_list(approx_side_as_seq, index)),
             )
             for index in different_ids
         ]
         return _compare_approx(
             self.expected,
             message_data,
```

### Comparing `pytest-8.1.1/src/_pytest/python_path.py` & `pytest-8.1.2/src/_pytest/python_path.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/recwarn.py` & `pytest-8.1.2/src/_pytest/recwarn.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/reports.py` & `pytest-8.1.2/src/_pytest/reports.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/runner.py` & `pytest-8.1.2/src/_pytest/runner.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/scope.py` & `pytest-8.1.2/src/_pytest/scope.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/setuponly.py` & `pytest-8.1.2/src/_pytest/setuponly.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/setupplan.py` & `pytest-8.1.2/src/_pytest/setupplan.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/skipping.py` & `pytest-8.1.2/src/_pytest/skipping.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/stash.py` & `pytest-8.1.2/src/_pytest/stash.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 class StashKey(Generic[T]):
     """``StashKey`` is an object used as a key to a :class:`Stash`.
 
     A ``StashKey`` is associated with the type ``T`` of the value of the key.
 
     A ``StashKey`` is unique and cannot conflict with another key.
+
+    .. versionadded:: 7.0
     """
 
     __slots__ = ()
 
 
 class Stash:
     r"""``Stash`` is a type-safe heterogeneous mutable mapping that
@@ -57,14 +59,16 @@
 
     .. code-block:: python
 
         # The static type of some_str is str.
         some_str = stash[some_str_key]
         # The static type of some_bool is bool.
         some_bool = stash[some_bool_key]
+
+    .. versionadded:: 7.0
     """
 
     __slots__ = ("_storage",)
 
     def __init__(self) -> None:
         self._storage: Dict[StashKey[Any], object] = {}
```

### Comparing `pytest-8.1.1/src/_pytest/stepwise.py` & `pytest-8.1.2/src/_pytest/stepwise.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/terminal.py` & `pytest-8.1.2/src/_pytest/terminal.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/threadexception.py` & `pytest-8.1.2/src/_pytest/threadexception.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/tmpdir.py` & `pytest-8.1.2/src/_pytest/tmpdir.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/unittest.py` & `pytest-8.1.2/src/_pytest/unittest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/unraisableexception.py` & `pytest-8.1.2/src/_pytest/unraisableexception.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/warning_types.py` & `pytest-8.1.2/src/_pytest/warning_types.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/_pytest/warnings.py` & `pytest-8.1.2/src/_pytest/warnings.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/pytest/__init__.py` & `pytest-8.1.2/src/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/src/pytest.egg-info/PKG-INFO` & `pytest-8.1.2/src/pytest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest
-Version: 8.1.1
+Version: 8.1.2
 Summary: pytest: simple powerful testing with Python
 Author: Holger Krekel, Bruno Oliveira, Ronny Pfannschmidt, Floris Bruynooghe, Brianna Laugher, Florian Bruhin, Others (See AUTHORS)
 License: MIT
 Project-URL: Changelog, https://docs.pytest.org/en/stable/changelog.html
 Project-URL: Homepage, https://docs.pytest.org/en/latest/
 Project-URL: Source, https://github.com/pytest-dev/pytest
 Project-URL: Tracker, https://github.com/pytest-dev/pytest/issues
```

### Comparing `pytest-8.1.1/src/pytest.egg-info/SOURCES.txt` & `pytest-8.1.2/src/pytest.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,15 @@
 doc/en/announce/release-8.0.0.rst
 doc/en/announce/release-8.0.0rc1.rst
 doc/en/announce/release-8.0.0rc2.rst
 doc/en/announce/release-8.0.1.rst
 doc/en/announce/release-8.0.2.rst
 doc/en/announce/release-8.1.0.rst
 doc/en/announce/release-8.1.1.rst
+doc/en/announce/release-8.1.2.rst
 doc/en/announce/sprint2016.rst
 doc/en/example/attic.rst
 doc/en/example/conftest.py
 doc/en/example/customdirectory.rst
 doc/en/example/index.rst
 doc/en/example/markers.rst
 doc/en/example/multipython.py
```

### Comparing `pytest-8.1.1/testing/_py/test_local.py` & `pytest-8.1.2/testing/_py/test_local.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/acceptance_test.py` & `pytest-8.1.2/testing/acceptance_test.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/code/test_code.py` & `pytest-8.1.2/testing/code/test_code.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/code/test_excinfo.py` & `pytest-8.1.2/testing/code/test_excinfo.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/code/test_source.py` & `pytest-8.1.2/testing/code/test_source.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/conftest.py` & `pytest-8.1.2/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/deprecated_test.py` & `pytest-8.1.2/testing/deprecated_test.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/example_scripts/customdirectory/conftest.py` & `pytest-8.1.2/testing/example_scripts/customdirectory/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/example_scripts/dataclasses/test_compare_recursive_dataclasses.py` & `pytest-8.1.2/testing/example_scripts/dataclasses/test_compare_recursive_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/example_scripts/issue_519.py` & `pytest-8.1.2/testing/example_scripts/issue_519.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/example_scripts/junit-10.xsd` & `pytest-8.1.2/testing/example_scripts/junit-10.xsd`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/example_scripts/perf_examples/collect_stats/generate_folders.py` & `pytest-8.1.2/testing/example_scripts/perf_examples/collect_stats/generate_folders.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/example_scripts/unittest/test_unittest_asyncio.py` & `pytest-8.1.2/testing/example_scripts/unittest/test_unittest_asyncio.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/io/test_pprint.py` & `pytest-8.1.2/testing/io/test_pprint.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/io/test_saferepr.py` & `pytest-8.1.2/testing/io/test_saferepr.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/io/test_terminalwriter.py` & `pytest-8.1.2/testing/io/test_terminalwriter.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/io/test_wcwidth.py` & `pytest-8.1.2/testing/io/test_wcwidth.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/logging/test_fixture.py` & `pytest-8.1.2/testing/logging/test_fixture.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/logging/test_formatter.py` & `pytest-8.1.2/testing/logging/test_formatter.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/logging/test_reporting.py` & `pytest-8.1.2/testing/logging/test_reporting.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/plugins_integration/README.rst` & `pytest-8.1.2/testing/plugins_integration/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/plugins_integration/bdd_wallet.py` & `pytest-8.1.2/testing/plugins_integration/bdd_wallet.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/python/approx.py` & `pytest-8.1.2/testing/python/approx.py`

 * *Files 2% similar despite different names*

```diff
@@ -759,14 +759,32 @@
 
         a12 = np.array([[1, 2]])
         a21 = np.array([[1], [2]])
 
         assert a12 != approx(a21)
         assert a21 != approx(a12)
 
+    def test_numpy_array_implicit_conversion(self) -> None:
+        """#12114."""
+        np = pytest.importorskip("numpy")
+
+        class ImplicitArray:
+            """Type which is implicitly convertible to a numpy array."""
+
+            def __init__(self, vals):
+                self.vals = vals
+
+            def __array__(self, dtype=None, copy=None):
+                return np.array(self.vals)
+
+        vec1 = ImplicitArray([1.0, 2.0, 3.0])
+        vec2 = ImplicitArray([1.0, 2.0, 4.0])
+        # see issue #12114 for test case
+        assert vec1 != approx(vec2)
+
     def test_numpy_array_protocol(self):
         """
         array-like objects such as tensorflow's DeviceArray are handled like ndarray.
         See issue #8132
         """
         np = pytest.importorskip("numpy")
```

### Comparing `pytest-8.1.1/testing/python/collect.py` & `pytest-8.1.2/testing/python/collect.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/python/fixtures.py` & `pytest-8.1.2/testing/python/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/python/integration.py` & `pytest-8.1.2/testing/python/integration.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/python/metafunc.py` & `pytest-8.1.2/testing/python/metafunc.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/python/raises.py` & `pytest-8.1.2/testing/python/raises.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/python/show_fixtures_per_test.py` & `pytest-8.1.2/testing/python/show_fixtures_per_test.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_argcomplete.py` & `pytest-8.1.2/testing/test_argcomplete.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_assertion.py` & `pytest-8.1.2/testing/test_assertion.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_assertrewrite.py` & `pytest-8.1.2/testing/test_assertrewrite.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_cacheprovider.py` & `pytest-8.1.2/testing/test_cacheprovider.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_capture.py` & `pytest-8.1.2/testing/test_capture.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_collection.py` & `pytest-8.1.2/testing/test_collection.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_compat.py` & `pytest-8.1.2/testing/test_compat.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_config.py` & `pytest-8.1.2/testing/test_config.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_conftest.py` & `pytest-8.1.2/testing/test_conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_debugging.py` & `pytest-8.1.2/testing/test_debugging.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_doctest.py` & `pytest-8.1.2/testing/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_error_diffs.py` & `pytest-8.1.2/testing/test_error_diffs.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_faulthandler.py` & `pytest-8.1.2/testing/test_faulthandler.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_findpaths.py` & `pytest-8.1.2/testing/test_findpaths.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_helpconfig.py` & `pytest-8.1.2/testing/test_helpconfig.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_junitxml.py` & `pytest-8.1.2/testing/test_junitxml.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_legacypath.py` & `pytest-8.1.2/testing/test_legacypath.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_link_resolve.py` & `pytest-8.1.2/testing/test_link_resolve.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_main.py` & `pytest-8.1.2/testing/test_main.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_mark.py` & `pytest-8.1.2/testing/test_mark.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_mark_expression.py` & `pytest-8.1.2/testing/test_mark_expression.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_meta.py` & `pytest-8.1.2/testing/test_meta.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_monkeypatch.py` & `pytest-8.1.2/testing/test_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_nodes.py` & `pytest-8.1.2/testing/test_nodes.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_parseopt.py` & `pytest-8.1.2/testing/test_parseopt.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_pastebin.py` & `pytest-8.1.2/testing/test_pastebin.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_pathlib.py` & `pytest-8.1.2/testing/test_pathlib.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_pluginmanager.py` & `pytest-8.1.2/testing/test_pluginmanager.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_pytester.py` & `pytest-8.1.2/testing/test_pytester.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_python_path.py` & `pytest-8.1.2/testing/test_python_path.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_recwarn.py` & `pytest-8.1.2/testing/test_recwarn.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_reports.py` & `pytest-8.1.2/testing/test_reports.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_runner.py` & `pytest-8.1.2/testing/test_runner.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_runner_xunit.py` & `pytest-8.1.2/testing/test_runner_xunit.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_scope.py` & `pytest-8.1.2/testing/test_scope.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_session.py` & `pytest-8.1.2/testing/test_session.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_setuponly.py` & `pytest-8.1.2/testing/test_setuponly.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_setupplan.py` & `pytest-8.1.2/testing/test_setupplan.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_skipping.py` & `pytest-8.1.2/testing/test_skipping.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_stash.py` & `pytest-8.1.2/testing/test_stash.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_stepwise.py` & `pytest-8.1.2/testing/test_stepwise.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_terminal.py` & `pytest-8.1.2/testing/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_threadexception.py` & `pytest-8.1.2/testing/test_threadexception.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_tmpdir.py` & `pytest-8.1.2/testing/test_tmpdir.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_unittest.py` & `pytest-8.1.2/testing/test_unittest.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_unraisableexception.py` & `pytest-8.1.2/testing/test_unraisableexception.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_warning_types.py` & `pytest-8.1.2/testing/test_warning_types.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/test_warnings.py` & `pytest-8.1.2/testing/test_warnings.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/testing/typing_checks.py` & `pytest-8.1.2/testing/typing_checks.py`

 * *Files identical despite different names*

### Comparing `pytest-8.1.1/tox.ini` & `pytest-8.1.2/tox.ini`

 * *Files identical despite different names*

