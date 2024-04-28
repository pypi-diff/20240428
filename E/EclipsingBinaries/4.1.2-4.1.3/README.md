# Comparing `tmp/eclipsingbinaries-4.1.2.tar.gz` & `tmp/eclipsingbinaries-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eclipsingbinaries-4.1.2.tar", last modified: Mon Apr 22 17:21:30 2024, max compression
+gzip compressed data, was "eclipsingbinaries-4.1.3.tar", last modified: Sat Apr 27 23:58:44 2024, max compression
```

## Comparing `eclipsingbinaries-4.1.2.tar` & `eclipsingbinaries-4.1.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:21:30.649291 eclipsingbinaries-4.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:21:30.637291 eclipsingbinaries-4.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:21:30.637291 eclipsingbinaries-4.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:21:30.637291 eclipsingbinaries-4.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/.github/workflows/ci_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)   112224 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:21:30.641291 eclipsingbinaries-4.1.2/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    22282 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (127)    31253 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:21:30.645291 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/APASS_Catalog_ex.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/Gaia_output.txt
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/O-C_paper_table.txt
--rw-r--r--   0 runner    (1001) docker     (127)    85904 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/OConnell_plot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/OConnell_table.txt
--rw-r--r--   0 runner    (1001) docker     (127)    48237 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/O_C_ex.png
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:21:15.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:21:30.645291 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/calibration_images/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-22 17:21:18.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/calibration_images/purpose.txt
--rw-r--r--   0 runner    (1001) docker     (127)   135237 2024-04-22 17:21:18.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/color_light_curve_ex.png
--rw-r--r--   0 runner    (1001) docker     (127)    35357 2024-04-22 17:21:18.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/example_OC_table.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-22 17:21:18.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/example_regression.txt
--rw-r--r--   0 runner    (1001) docker     (127)   118184 2024-04-22 17:21:18.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/gui_color_light.png
--rw-r--r--   0 runner    (1001) docker     (127)   109712 2024-04-22 17:21:18.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/light_curve_ex.png
--rw-r--r--   0 runner    (1001) docker     (127)   136591 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/min_program_demo.png
--rw-r--r--   0 runner    (1001) docker     (127)   131114 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/overlay_example.png
--rw-r--r--   0 runner    (1001) docker     (127)    31361 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25814 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (127)    30132 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (127)    39669 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25329 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    16127 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/multi_aperture_photometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/tess_ccd_info.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:21:30.649291 eclipsingbinaries-4.1.2/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/tests/test_IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/tests/test_apass.py
--rw-r--r--   0 runner    (1001) docker     (127)    56086 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:21:30.649291 eclipsingbinaries-4.1.2/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-22 17:21:26.000000 eclipsingbinaries-4.1.2/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-22 17:21:30.000000 eclipsingbinaries-4.1.2/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:21:26.000000 eclipsingbinaries-4.1.2/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-22 17:21:26.000000 eclipsingbinaries-4.1.2/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:21:26.000000 eclipsingbinaries-4.1.2/EclipsingBinaries.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 17:21:26.000000 eclipsingbinaries-4.1.2/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 17:21:26.000000 eclipsingbinaries-4.1.2/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-22 17:21:30.649291 eclipsingbinaries-4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:21:30.649291 eclipsingbinaries-4.1.2/changelog/
--rw-r--r--   0 runner    (1001) docker     (127)   222548 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/changelog/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/changelog/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:21:30.649291 eclipsingbinaries-4.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/docs/EB.rst
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:21:30.637291 eclipsingbinaries-4.1.2/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:21:30.649291 eclipsingbinaries-4.1.2/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/docs/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)    24030 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/docs/toolbox.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-22 17:21:30.653291 eclipsingbinaries-4.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-22 17:21:19.000000 eclipsingbinaries-4.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:44.570975 eclipsingbinaries-4.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:44.550975 eclipsingbinaries-4.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:44.554975 eclipsingbinaries-4.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:44.554975 eclipsingbinaries-4.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/.github/workflows/ci_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   112224 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:44.558975 eclipsingbinaries-4.1.3/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22282 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31639 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:44.566975 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/APASS_Catalog_ex.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/Gaia_output.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/O-C_paper_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    85904 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/OConnell_plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/OConnell_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    48237 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/O_C_ex.png
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 23:58:29.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:44.566975 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/calibration_images/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/calibration_images/purpose.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   135237 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/color_light_curve_ex.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35357 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/example_OC_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/example_regression.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   118184 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/gui_color_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   109712 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/light_curve_ex.png
+-rw-r--r--   0 runner    (1001) docker     (127)   136591 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/min_program_demo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   131114 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/overlay_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31361 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25814 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    30132 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    39669 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25329 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16127 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/multi_aperture_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/tess_ccd_info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:44.566975 eclipsingbinaries-4.1.3/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/tests/test_IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/tests/test_apass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56822 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:44.570975 eclipsingbinaries-4.1.3/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-27 23:58:40.000000 eclipsingbinaries-4.1.3/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-27 23:58:44.000000 eclipsingbinaries-4.1.3/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 23:58:40.000000 eclipsingbinaries-4.1.3/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-27 23:58:40.000000 eclipsingbinaries-4.1.3/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 23:58:40.000000 eclipsingbinaries-4.1.3/EclipsingBinaries.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 23:58:40.000000 eclipsingbinaries-4.1.3/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-27 23:58:40.000000 eclipsingbinaries-4.1.3/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-27 23:58:44.570975 eclipsingbinaries-4.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:44.566975 eclipsingbinaries-4.1.3/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)   222548 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/changelog/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/changelog/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:44.566975 eclipsingbinaries-4.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/docs/EB.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:44.550975 eclipsingbinaries-4.1.3/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:44.566975 eclipsingbinaries-4.1.3/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/docs/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    24030 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/docs/toolbox.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-27 23:58:44.570975 eclipsingbinaries-4.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-27 23:58:33.000000 eclipsingbinaries-4.1.3/tox.ini
```

### Comparing `eclipsingbinaries-4.1.2/.github/ISSUE_TEMPLATE/bug_report.md` & `eclipsingbinaries-4.1.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `eclipsingbinaries-4.1.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/.github/workflows/ci_tests.yml` & `eclipsingbinaries-4.1.3/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/.github/workflows/python-publish.yml` & `eclipsingbinaries-4.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/CHANGELOG.md` & `eclipsingbinaries-4.1.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/CODE_OF_CONDUCT.md` & `eclipsingbinaries-4.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/IRAF_Reduction.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/IRAF_Reduction.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/Night_Filters.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/OC_plot.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/OC_plot.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/OConnell.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/apass.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/apass.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/color_light_curve.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/color_light_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Sep 17 12:45:40 2020
 Created on Tue Feb 16 19:29:16 2021
 @author: Alec Neal
 
-Last Edited: 04/05/2024
+Last Edited: 04/27/2024
 Editor: Kyle Koeller
 """
 
-# from vseq_updated import io, calc, FT, binning, plot, Flower  # testing purposes
-from .vseq_updated import io, calc, FT, binning, plot, Flower
+# from vseq_updated import io, calc, FT, binning, plot, Flower, Pecaut  # testing purposes
+from .vseq_updated import io, calc, FT, binning, plot, Flower, Pecaut
 import numpy as np
 import matplotlib.pyplot as plt
 import statistics as st
 from tkinter import *
 from matplotlib.backends.backend_tkagg import (
     FigureCanvasTkAgg)
 from matplotlib.figure import Figure
@@ -138,32 +138,36 @@
     B = [aBphase, aB_mag, aB_interp_mag]
     V = [aVphase, aV_mag]
 
     # print('T =', vseq.Flower.T.Teff(quadcolor - (0.641 / 3.1)))
     if index == "BV":
         temp = []
         # temp = vseq.Flower.T.Teff(quadcolor - (0.641 / 3.1), colorerr)
-        t1 = Flower.T.Teff(quadcolor - (0.641 / 3.1))
-        temp_high = Flower.T.Teff(quadcolor - (0.641 / 3.1) - colorerr)
-        temp_low = Flower.T.Teff(quadcolor - (0.641 / 3.1) + colorerr)
-
-        temp_err = (temp_high - temp_low)/2
-        temp.append(t1)
+        t1 = Flower.T.Teff(quadcolor - (0.641 / 3.1), colorerr)
+        temp_high = Flower.T.Teff(quadcolor - (0.641 / 3.1) - colorerr, colorerr)
+        temp_low = Flower.T.Teff(quadcolor - (0.641 / 3.1) + colorerr, colorerr)
+
+        # temp_err = (temp_high[0] - temp_low[0])/2
+        temp_err = np.sqrt(temp_high[1]**2 + temp_low[1]**2)
+        temp.append(t1[0])
         temp.append(temp_err)
         print('T_BV =', temp[0], '+/-', temp[1])
     elif index == "VR":
-        # temp = vseq.Pecaut.T.Teff(quadcolor - (0.58 / 3.1), colorerr)
+        t1 = Pecaut.T.Teff(quadcolor - (0.58 / 3.1), colorerr)
         temp = []
-        t1 = Flower.T.Teff(quadcolor - 0.561 * (0.641 / 3.1))
+        # t1 = Flower.T.Teff(quadcolor - 0.561 * (0.641 / 3.1), colorerr)
         # E_V-R = 0.561*E_B-V
-        temp_high = Flower.T.Teff(quadcolor - 0.561* (0.641 / 3.1) - colorerr)
-        temp_low = Flower.T.Teff(quadcolor - 0.561* (0.641 / 3.1) + colorerr)
-
-        temp_err = (temp_high - temp_low) / 2
-        temp.append(t1)
+        temp_high = Pecaut.T.Teff(quadcolor - (0.58 / 3.1) - colorerr, colorerr)
+        temp_low = Pecaut.T.Teff(quadcolor - (0.58 / 3.1) + colorerr, colorerr)
+        # temp_high = Flower.T.Teff(quadcolor - 0.561* (0.641 / 3.1) - colorerr, colorerr)
+        # temp_low = Flower.T.Teff(quadcolor - 0.561* (0.641 / 3.1) + colorerr, colorerr)
+
+        # temp_err = (temp_high[0] - temp_low[0]) / 2
+        temp_err = np.sqrt(temp_high[1] ** 2 + temp_low[1] ** 2)
+        temp.append(t1[0])
         temp.append(temp_err)
         if temp[0] == 0:
             print("V-R color cannot be used to determine temperature.")
         else:
             print('T_VR =', temp[0], '+/-', temp[1])
 
     return B_V, B, V, quadcolor, colorerr, temp
@@ -340,15 +344,15 @@
     root = Tk()
     root.option_add('*Font', '12')
     root.title('CLC-gui v0.2.1')
     # root.geometry('1200x800')
     # disp=3
     # T=Text(root,height=disp,width=25)
     # T.grid(row=0,column=1)
-    Intro = Label(root, text='Color Light Curve - gui\nversion 0.4.1 (2/19/21)\nby Alec Neal\n')
+    Intro = Label(root, text='Color Light Curve - gui\nversion 0.4.2 (4/27/24)\nby Alec Neal\n')
     Intro.grid(row=0, column=0, columnspan=2)
     # Intro.config(font=('Arial',12))
     # T.insert(END,'Hello world!')
 
     Label(root, text=autowrap('Program to determine light curve colors. Mouse over the fields for more information.',
                               width=50) + '\n').grid(row=1, column=0, columnspan=2)
     entries = [['B file'],
```

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/APASS_Catalog_ex.txt` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/APASS_Catalog_ex.txt`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/O-C_paper_table.txt` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/O-C_paper_table.txt`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/OConnell_plot.png` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/OConnell_plot.png`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/OConnell_table.txt` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/OConnell_table.txt`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/O_C_ex.png` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/O_C_ex.png`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/color_light_curve_ex.png` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/color_light_curve_ex.png`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/example_OC_table.txt` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/example_OC_table.txt`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/example_regression.txt` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/example_regression.txt`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/gui_color_light.png` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/gui_color_light.png`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/light_curve_ex.png` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/light_curve_ex.png`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/min_program_demo.png` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/min_program_demo.png`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/overlay_example.png` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/overlay_example.png`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/test_B.txt` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/test_R.txt` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/test_V.txt` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/examples/test_minimums.txt` & `eclipsingbinaries-4.1.3/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/find_min.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/find_min.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/gaia.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/menu.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/multi_aperture_photometry.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/multi_aperture_photometry.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/pipeline.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/pipeline.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/tess_ccd_info.txt` & `eclipsingbinaries-4.1.3/EclipsingBinaries/tess_ccd_info.txt`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/tess_data_search.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/tesscut.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/tests/test_IRAF_Reduction.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/tests/test_IRAF_Reduction.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/tests/test_OC_plot.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/tests/test_apass.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/tests/test_apass.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries/vseq_updated.py` & `eclipsingbinaries-4.1.3/EclipsingBinaries/vseq_updated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Feb 22 16:09:28 2020
 @author: Alec Neal
 
-Last Updated: 04/22/2024
+Last Updated: 04/27/2024
 Last Editor: Kyle Koeller
 
 Collection of functions, coefficients and equations commonly used
 with short-period variable stars, but many can be used more
 generally
 """
 import numpy as np
@@ -106,14 +106,15 @@
     b = list()
     for i in a:
         num = float(i)
         num2 = format(num, ".2f")
         b.append(num2)
     return b
 
+
 # ======================================
 class io:
     def importFile_pd(inputFile, delimit=None, header=None, file_type='text', engine='python', delim_whitespace=True):
         if file_type == 'text':
             if delim_whitespace == True:
                 file = pd.read_csv(inputFile, delim_whitespace=True, header=header, engine='python')
             else:
@@ -124,14 +125,15 @@
             print('File type not currently supported. Choose text or excel type.')
         columnlist = []
         for column in range(len(list(file))):
             columnlist.append(list(file[column]))
             # print(columnlist)
         return columnlist
 
+
 # =======================================
 class calc:  # assortment of functions
     def frac(x):
         return x - np.floor(x)
 
     def Newton(f, x0, e=1e-8, fprime=None, max_iter=None, dx=1e-8, central_diff=True, print_iters=False):
         x = x0
@@ -160,14 +162,33 @@
                     break
             if iters == max_iter:
                 return False
             else:
                 return x
 
     class poly:
+        def result(coeflist, value, deriv=False):
+            """
+            Result of a polynomial given an ascending order coefficient list, and
+            an x value.
+            """
+            # n0=0
+            # n=n0
+            # termlist=[]
+            # while(n<len(coeflist)):
+            # termlist.append(coeflist[n]*value**n)
+            # n+=1
+            # return sum(termlist)
+            # deg = len(coeflist)-1
+            # coeflist=np.array(coeflist)
+            # if deriv == True:
+            #
+
+            return sum(np.array(coeflist) * value ** np.arange(len(coeflist)))
+
         def error(coeflist, value, error):
             """
             Propagated uncertainty of a standard polynomial.
 
             coeflist: ascending order coefficient list
 
             value: input value
@@ -236,15 +257,16 @@
             return abs(calc.poly.error(coeflist, value, error) * np.log(base) * calc.poly.power(coeflist, value, base))
 
         def t_eff_err(coeflist, value, error, temp, coeferror=[], base=10):
             if len(coeferror) == 0:
                 return temp * np.log(base) * calc.poly.error(coeflist, value, error)
             else:
                 return temp * np.log(base) * np.sqrt(calc.poly.error(coeflist, value, error) ** 2 +
-                                                     sum(np.array(coeferror) * ((value ** np.arange(len(coeflist))) ** 2)))
+                                                     sum(np.array(coeferror) * (
+                                                                 (value ** np.arange(len(coeflist))) ** 2)))
             # return np.log(base) * calc.poly.power(coeflist, value, base) * \
             #        np.sqrt(calc.poly.error(coeflist, value, error) ** 2 + \
             #                sum(np.array(coeferror) * value ** np.arange(len(coeflist)) ** 2))
 
     class error:
         def per_diff(x1, x2):
             return 100 * (abs(x1 - x2) / np.mean([x1, x2]))
@@ -363,14 +385,15 @@
             class fluxTomag:
                 def mag(flux):
                     return -2.5 * np.log10(flux)
 
                 def error(flux, fluxerr):
                     return (2.5 * fluxerr) / (flux * np.log(10))
 
+
 # ======================================
 class binning:
     def makebin(phase, bins, phasefluxlist):
         """
         Component of minibinner().
         """
         halfbin = 0.5 / bins
@@ -724,14 +747,15 @@
             a, b = FT.coefficients(section_polyflux)[1:3]
         # FTcoef=FT.coefficients(section_polyflux)
         # a=FTcoef[1]
         # b=FTcoef[2]
         # print(len(section_polyphase))
         return [a, b], [c_MB, nc_MB], [section_polyphase, section_polyflux]
 
+
 # ======================================
 class FT:  # Fourier transform
     def coefficients(binnedvaluelist):
         """
         Calculates Fourier coefficients based on numPy's fft.ifft function
 
         Parameters
@@ -881,14 +905,15 @@
         for k in range(1, orderp1):
             int_unc += ((a_unc[k] / k) * np.sin(2 * np.pi * phase * k)) ** 2 + (
                     (b_unc[k] / k) * np.cos(2 * np.pi * phase * k)) ** 2
         int_unc *= 0.25 / np.pi ** 2
         int_unc += (a_unc[0] * phase) ** 2
         return np.sqrt(int_unc)
 
+
 # ======================================
 class OConnell:  # O'Connell effect
     def OER_FT(a, b, order):
         nlist = np.arange(order + 1)[1::]
         A = 0.5 * sum(a[nlist])
         B = sum(b[nlist[::2]] / nlist[::2]) / np.pi
         return 1 - (2 / (1 + A / B))
@@ -1101,40 +1126,43 @@
             if 0.25 - phase_range < ob_phaselist[n] < 0.25 + phase_range:
                 Iplist.append(ob_fluxlist[n])
             if 0.75 - phase_range < ob_phaselist[n] < 0.75 + phase_range:
                 Islist.append(ob_fluxlist[n])
         dI_mean_obs = np.mean(Iplist) - np.mean(Islist)
         return dI_mean_obs
 
+
 # weighted averages
 def M(errorlist):  # sum of 1/errors
     M0 = 0
     M = M0
     for error in errorlist:
         M += 1 / error ** 2
     return M
 
 
 #
 def wfactor(errorlist, n, M):
     return 1 / (errorlist[n] ** 2 * M)
 
+
 # ======================================
 class Flower:  # stuff from Flower 1996, Torres 2010
     class T:
         # c=[c0,c1,c2,c3,c4,c5,c6,c7]
         c = [3.97914510671409, -0.654992268598245, 1.74069004238509, -4.60881515405716, 6.79259977994447,
              -5.39690989132252, 2.19297037652249, -0.359495739295671]
 
         def Teff(BV, error):
             # return 10**((Flower.T.c[0]*BV**0)+(Flower.T.c[1]*BV**1)+(Flower.T.c[2]*BV**2)+(Flower.T.c[3]*BV**3)+(Flower.T.c[4]*BV**4)+(Flower.T.c[5]*BV**5)+(Flower.T.c[6]*BV**6)+(Flower.T.c[7]*BV**7))
             temp = calc.poly.power(Flower.T.c, BV, 10)
             err = calc.poly.t_eff_err(Flower.T.c, BV, error, temp)
             return temp, err
 
+
 # ======================================
 class Harmanec:
     class mass:
         c = [-121.6782, 88.057, -21.46965, 1.771141]
 
         def M1(BV):
             # M1=10**((Harmanec.mass.c0*np.log10(Flower.T.Teff(BV))**0)+(Harmanec.mass.c1*np.log10(Flower.T.Teff(BV))**1)+(Harmanec.mass.c2*np.log10(Flower.T.Teff(BV))**2)+(Harmanec.mass.c3*np.log10(Flower.T.Teff(BV))**3))
@@ -1153,14 +1181,15 @@
         if excess == 'J_K':
             return Av * Red.J_K
         elif excess == 'J_H':
             return Av * Red.J_H
         elif excess == 'V_R':
             return Av * Red.V_R
 
+
 # ======================================
 class plot:
     def amp(valuelist):
         # test documentation
         return max(valuelist) - min(valuelist)
 
     def aliasing2(phaselist, maglist, errorlist, alias=0.6):
@@ -1231,14 +1260,15 @@
             ax.xaxis.set_major_formatter(FormatStrFormatter('$%g$'))
         # for label in ax.get_xticklabels():
         # label.set_fontproperties('DejaVu Sans')
         # for label in ax.get_yticklabels():
         # label.set_fontproperties('DejaVu Sans')
         return 'DONE'
 
+
 # ======================================
 class Roche:
     def Kopal_cyl(rho, phi, z, q):
         return 1 / np.sqrt(rho ** 2 + z ** 2) + q / (
             np.sqrt(1 + rho ** 2 + z ** 2 - 2 * rho * np.cos(phi))) - q * rho * np.cos(phi) + 0.5 * (1 + q) * rho ** 2
 
     def gen_Kopal_cyl(rho, phi, z, q,
@@ -1286,27 +1316,28 @@
 
             return print('Invalid body, choose M1 or M2.')
 
     def gen_Kopal_zero(rho, phi, z, q, Kopal,
                        xcm=None, ycm=0, zcm=0):
         return Roche.gen_Kopal_cyl(rho, phi, z, q, xcm=xcm, ycm=ycm, zcm=zcm) - Kopal
 
+
 class Pecaut:  # V-R effective temperature fit from Pecaut and Mamajek 2013 https://arxiv.org/pdf/1307.2657.pdf
     class T:
         # c=[c0,c1,c2,c3]
         c1 = [3.98007, -1.2742, 32.41373, 98.06855]  # -0.115 < V-R < 0.019
         c2 = [3.9764, -0.80319, 0.64832, -0.2651]  # 0.019 < V-R < 1.079
 
         c1_err = [0.00499, 0.25431, 6.60765, 41.6003]
         c2_err = [0.00179, 0.01409, 0.03136, 0.0197]
 
         def Teff(VR, error):
-            if -0.115 < VR < 0.019:
+            if -0.115 < VR <= 0.019: # B1V to A1V
                 temp = calc.poly.power(Pecaut.T.c1, VR, 10)
                 err = calc.poly.t_eff_err(Pecaut.T.c1, VR, error, temp, coeferror=Pecaut.T.c1_err)
                 return temp, err
-            elif 0.019 < VR < 1.079:
+            elif 0.019 < VR < 1.079: # A1V to M3V
                 temp = calc.poly.power(Pecaut.T.c2, VR, 10)
                 err = calc.poly.t_eff_err(Pecaut.T.c2, VR, error, temp, coeferror=Pecaut.T.c2_err)
                 return temp, err
             else:
                 return 0, 0
```

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries.egg-info/PKG-INFO` & `eclipsingbinaries-4.1.3/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 4.1.2
+Version: 4.1.3
 Summary: "Binary Star Package for Ball State University's Astronomy Research Group"
 Home-page: https://eclipsingbinaries.readthedocs.io/
 Author: Kyle Koeller
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `eclipsingbinaries-4.1.2/EclipsingBinaries.egg-info/SOURCES.txt` & `eclipsingbinaries-4.1.3/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/LICENSE` & `eclipsingbinaries-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/PKG-INFO` & `eclipsingbinaries-4.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 4.1.2
+Version: 4.1.3
 Summary: "Binary Star Package for Ball State University's Astronomy Research Group"
 Home-page: https://eclipsingbinaries.readthedocs.io/
 Author: Kyle Koeller
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `eclipsingbinaries-4.1.2/README.md` & `eclipsingbinaries-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/changelog/package-lock.json` & `eclipsingbinaries-4.1.3/changelog/package-lock.json`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/changelog/package.json` & `eclipsingbinaries-4.1.3/changelog/package.json`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/docs/conf.py` & `eclipsingbinaries-4.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/docs/contributing.rst` & `eclipsingbinaries-4.1.3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/docs/index.rst` & `eclipsingbinaries-4.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/docs/installation.rst` & `eclipsingbinaries-4.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/docs/pipeline.rst` & `eclipsingbinaries-4.1.3/docs/pipeline.rst`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/docs/toolbox.rst` & `eclipsingbinaries-4.1.3/docs/toolbox.rst`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/setup.cfg` & `eclipsingbinaries-4.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `eclipsingbinaries-4.1.2/tox.ini` & `eclipsingbinaries-4.1.3/tox.ini`

 * *Files identical despite different names*

