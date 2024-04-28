# Comparing `tmp/dataretrieval-1.0.6.tar.gz` & `tmp/dataretrieval-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataretrieval-1.0.6.tar", last modified: Thu Sep 28 20:43:51 2023, max compression
+gzip compressed data, was "dataretrieval-1.0.7.tar", last modified: Sun Apr 28 16:10:07 2024, max compression
```

## Comparing `dataretrieval-1.0.6.tar` & `dataretrieval-1.0.7.tar`

### file list

```diff
@@ -1,132 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.148707 dataretrieval-1.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.084705 dataretrieval-1.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.084705 dataretrieval-1.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/.github/workflows/sphinx-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.084705 dataretrieval-1.0.6/.gitlab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.084705 dataretrieval-1.0.6/.gitlab/issue_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/.gitlab/issue_templates/reviewer_checklist.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.084705 dataretrieval-1.0.6/.gitlab/merge_request_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/.gitlab/merge_request_templates/reviewer_checklist.md
--rw-r--r--   0 runner    (1001) docker     (127)     8812 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/DISCLAIMER.md
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2023-09-28 20:43:51.148707 dataretrieval-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/code.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.088705 dataretrieval-1.0.6/dataretrieval/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/dataretrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-09-28 20:43:50.000000 dataretrieval-1.0.6/dataretrieval/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.088705 dataretrieval-1.0.6/dataretrieval/codes/
--rwxr-xr-x   0 runner    (1001) docker     (127)       47 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/dataretrieval/codes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/dataretrieval/codes/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/dataretrieval/codes/timezones.py
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/dataretrieval/nadp.py
--rw-r--r--   0 runner    (1001) docker     (127)    45334 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/dataretrieval/nwis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/dataretrieval/streamstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7944 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/dataretrieval/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/dataretrieval/waterwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    14127 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/dataretrieval/wqp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.088705 dataretrieval-1.0.6/dataretrieval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2023-09-28 20:43:50.000000 dataretrieval-1.0.6/dataretrieval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2023-09-28 20:43:51.000000 dataretrieval-1.0.6/dataretrieval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-28 20:43:50.000000 dataretrieval-1.0.6/dataretrieval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-28 20:43:50.000000 dataretrieval-1.0.6/dataretrieval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-28 20:43:50.000000 dataretrieval-1.0.6/dataretrieval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.088705 dataretrieval-1.0.6/demos/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9869 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/NWIS_demo_1.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (127)    13027 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/R Python Vignette equivalents.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.088705 dataretrieval-1.0.6/demos/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)   535225 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/datasets/peak_discharge_trends.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.088705 dataretrieval-1.0.6/demos/hydroshare/
--rw-r--r--   0 runner    (1001) docker     (127)     9236 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9847 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10147 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9852 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10356 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8783 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.088705 dataretrieval-1.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.088705 dataretrieval-1.0.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.092705 dataretrieval-1.0.6/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/USGS_dataretrieval_DailyValues_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/USGS_dataretrieval_GroundwaterLevels_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/USGS_dataretrieval_Measurements_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/USGS_dataretrieval_ParameterCodes_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/USGS_dataretrieval_Peaks_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/USGS_dataretrieval_Ratings_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/USGS_dataretrieval_SiteInfo_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/USGS_dataretrieval_SiteInventory_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/USGS_dataretrieval_Statistics_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/USGS_dataretrieval_UnitValues_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/USGS_dataretrieval_WaterSamples_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/USGS_dataretrieval_WaterUse_Examples.nblink
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.092705 dataretrieval-1.0.6/docs/source/examples/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)   535225 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/datasets/peak_discharge_trends.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/nwisdemo01.nblink
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/readme_examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/rvignettes.nblink
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/examples/siteinfo_examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.092705 dataretrieval-1.0.6/docs/source/meta/
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/meta/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/meta/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/meta/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.092705 dataretrieval-1.0.6/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/reference/nadp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/reference/nwis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/reference/streamstats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/reference/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/reference/waterwatch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/reference/wqp.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.092705 dataretrieval-1.0.6/docs/source/userguide/
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/userguide/dataportals.rst
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/userguide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/docs/source/userguide/timeconventions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/requirements-dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       45 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-28 20:43:51.148707 dataretrieval-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.096706 dataretrieval-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:43:51.148707 dataretrieval-1.0.6/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)    22902 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/nwis_sites.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    48992 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/water_use_allegheny.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2485 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/water_use_national.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    14065 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/waterdata_measurements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      491 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/waterdata_pmcodes.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)  5998995 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/waterdata_qwdata.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    14869 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/waterservices_dv.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3221 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/waterservices_gwlevels.txt
--rwxr-xr-x   0 runner    (1001) docker     (127) 22180871 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/waterservices_iv.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/waterservices_peaks.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2323 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/waterservices_ratings.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1429 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/waterservices_site.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)   198769 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/waterservices_stats.txt
--rw-r--r--   0 runner    (1001) docker     (127) 21772141 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/wqp_activities.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/wqp_activity_metrics.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1442378 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/wqp_detection_limits.txt
--rw-r--r--   0 runner    (1001) docker     (127)   436730 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/wqp_habitat_metrics.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/wqp_organizations.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1029205 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/wqp_project_weights.txt
--rw-r--r--   0 runner    (1001) docker     (127)    28500 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/wqp_projects.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3155 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/wqp_results.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)  2276131 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/data/wqp_sites.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/nadp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/nwis_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/utils_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13451 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/waterservices_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7787 2023-09-28 20:43:33.000000 dataretrieval-1.0.6/tests/wqp_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.671178 dataretrieval-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.575177 dataretrieval-1.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.583177 dataretrieval-1.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.github/workflows/sphinx-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.575177 dataretrieval-1.0.7/.gitlab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.583177 dataretrieval-1.0.7/.gitlab/issue_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.gitlab/issue_templates/reviewer_checklist.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.583177 dataretrieval-1.0.7/.gitlab/merge_request_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.gitlab/merge_request_templates/reviewer_checklist.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.prettierrc.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8812 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/DISCLAIMER.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-28 16:10:07.671178 dataretrieval-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/code.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.583177 dataretrieval-1.0.7/dataretrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 16:10:07.000000 dataretrieval-1.0.7/dataretrieval/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.583177 dataretrieval-1.0.7/dataretrieval/codes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       47 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/codes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/codes/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/codes/timezones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/nadp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18261 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/nldi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51276 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/nwis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/streamstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/waterwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15116 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/wqp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.667178 dataretrieval-1.0.7/dataretrieval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-28 16:10:07.000000 dataretrieval-1.0.7/dataretrieval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-28 16:10:07.000000 dataretrieval-1.0.7/dataretrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:10:07.000000 dataretrieval-1.0.7/dataretrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-28 16:10:07.000000 dataretrieval-1.0.7/dataretrieval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 16:10:07.000000 dataretrieval-1.0.7/dataretrieval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.583177 dataretrieval-1.0.7/demos/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9869 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/NWIS_demo_1.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13027 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/R Python Vignette equivalents.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.587177 dataretrieval-1.0.7/demos/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)   535225 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/datasets/peak_discharge_trends.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.587177 dataretrieval-1.0.7/demos/hydroshare/
+-rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.587177 dataretrieval-1.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.587177 dataretrieval-1.0.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.591177 dataretrieval-1.0.7/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_DailyValues_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_GroundwaterLevels_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_Measurements_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_ParameterCodes_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_Peaks_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_Ratings_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_SiteInfo_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_SiteInventory_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_Statistics_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_UnitValues_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_WaterSamples_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_WaterUse_Examples.nblink
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.591177 dataretrieval-1.0.7/docs/source/examples/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)   535225 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/datasets/peak_discharge_trends.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/nwisdemo01.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/readme_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/rvignettes.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/siteinfo_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.595177 dataretrieval-1.0.7/docs/source/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/meta/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/meta/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/meta/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.595177 dataretrieval-1.0.7/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/nadp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/nwis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/streamstats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/waterwatch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/wqp.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.595177 dataretrieval-1.0.7/docs/source/userguide/
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/userguide/dataportals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/userguide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/userguide/timeconventions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:10:07.671178 dataretrieval-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.595177 dataretrieval-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.667178 dataretrieval-1.0.7/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_basin.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26880 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_features_by_comid.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_features_by_feature_source_with_nav_mode.json
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_features_by_feature_source_without_nav_mode.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_features_by_lat_long.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_flowlines.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_flowlines_by_comid.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22920 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nwis_sites.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48992 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/water_use_allegheny.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2485 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/water_use_national.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14065 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/waterdata_measurements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/waterdata_pmcodes.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)  5998995 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/waterdata_qwdata.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14869 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/waterservices_dv.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3221 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/waterservices_gwlevels.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127) 22180871 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/waterservices_iv.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/waterservices_peaks.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2323 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/waterservices_ratings.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1447 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/waterservices_site.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)   198769 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/waterservices_stats.txt
+-rw-r--r--   0 runner    (1001) docker     (127) 21772141 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_activities.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_activity_metrics.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1442378 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_detection_limits.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   436730 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_habitat_metrics.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_organizations.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1029205 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_project_weights.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    28500 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_projects.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3155 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_results.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)  2276131 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_sites.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/nadp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10464 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/nldi_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/nwis_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/utils_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22144 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/waterservices_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7787 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/wqp_test.py
```

### Comparing `dataretrieval-1.0.6/.github/workflows/python-package.yml` & `dataretrieval-1.0.7/.github/workflows/python-package.yml`

 * *Files 6% similar despite different names*

```diff
@@ -5,37 +5,36 @@
 
 on:
   push:
   pull_request:
 
 jobs:
   build:
-
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [3.8, 3.9, '3.10']
+        os: [ubuntu-latest, windows-latest]
+        python-version: [3.8, 3.9, '3.10', 3.11]
 
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
-      with:
-        python-version: ${{ matrix.python-version }}
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install -r requirements-dev.txt
-    - name: Lint with flake8
-      run: |
-        # stop the build if there are Python syntax errors or undefined names
-        flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-        # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-        flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
-    - name: Test with pytest and report coverage
-      run: |
-        cd tests
-        coverage run -m pytest
-        coverage report -m
-        cd ..
+      - uses: actions/checkout@v2
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install .[test,nldi]
+      - name: Lint with flake8
+        run: |
+          # stop the build if there are Python syntax errors or undefined names
+          flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
+          # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
+          flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
+      - name: Test with pytest and report coverage
+        run: |
+          cd tests
+          coverage run -m pytest
+          coverage report -m
+          cd ..
```

### Comparing `dataretrieval-1.0.6/.github/workflows/python-publish.yml` & `dataretrieval-1.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/.github/workflows/sphinx-docs.yml` & `dataretrieval-1.0.7/.github/workflows/sphinx-docs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -6,36 +6,35 @@
   push:
   pull_request:
 
 jobs:
   docs:
     runs-on: ubuntu-latest
     steps:
-    - name: Checkout
-      uses: actions/checkout@v3
-      with:
-        persist-credentials: false
-    - name: Install dataretrieval, dependencies, and Sphinx then build docs
-      shell: bash -l {0}
-      run: |
-        python -m pip install --upgrade pip
-        pip install -r requirements-dev.txt
-        pip install .
-        sudo apt update -y && sudo apt install -y latexmk texlive-latex-recommended texlive-latex-extra texlive-fonts-recommended dvipng pandoc
-        (cd docs && make docs)
-        (cd docs && make html)
-    - name: Debug
-      run: |
-        echo $REF
-        echo $EVENT_NAME
-        echo ${{ github.event_name == 'push' }}
-        echo ${{ github.ref == 'refs/heads/master' }}
-        echo ${{ github.event_name == 'push' && github.ref == 'refs/heads/master' }}
-    - name: Deploy to GitHub Pages
-      uses: JamesIves/github-pages-deploy-action@v4.4.1
-      if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/master' }}
-      with:
+      - name: Checkout
+        uses: actions/checkout@v3
+        with:
+          persist-credentials: false
+      - name: Install dataretrieval, dependencies, and Sphinx then build docs
+        shell: bash -l {0}
+        run: |
+          python -m pip install --upgrade pip
+          pip install .[doc]
+          sudo apt update -y && sudo apt install -y latexmk texlive-latex-recommended texlive-latex-extra texlive-fonts-recommended dvipng pandoc
+          (cd docs && make docs)
+          (cd docs && make html)
+      - name: Debug
+        run: |
+          echo $REF
+          echo $EVENT_NAME
+          echo ${{ github.event_name == 'push' }}
+          echo ${{ github.ref == 'refs/heads/master' }}
+          echo ${{ github.event_name == 'push' && github.ref == 'refs/heads/master' }}
+      - name: Deploy to GitHub Pages
+        uses: JamesIves/github-pages-deploy-action@v4.4.1
+        if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/master' }}
+        with:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           EVENT_NAME: ${{ github.event_name }}
           REF: ${{ github.ref }}
           BRANCH: gh-pages
-          FOLDER: docs/build/html
+          FOLDER: docs/build/html
```

### Comparing `dataretrieval-1.0.6/.gitignore` & `dataretrieval-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/.gitlab/issue_templates/reviewer_checklist.md` & `dataretrieval-1.0.7/.gitlab/issue_templates/reviewer_checklist.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/.gitlab/merge_request_templates/reviewer_checklist.md` & `dataretrieval-1.0.7/.gitlab/merge_request_templates/reviewer_checklist.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/CONTRIBUTING.md` & `dataretrieval-1.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/DISCLAIMER.md` & `dataretrieval-1.0.7/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/LICENSE.md` & `dataretrieval-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/PKG-INFO` & `dataretrieval-1.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dataretrieval
-Version: 1.0.6
+Version: 1.0.7
 Summary: Discover and retrieve water data from U.S. federal hydrologic web services.
-Maintainer-email: Timothy Hodson <thodson@usgs.gov>, Jayaram Hariharan <jhariharan@usgs.gov>
+Maintainer-email: Timothy Hodson <thodson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United
         States because it contains materials that originally came from the United
         States Geological Survey, an agency of the United States Department of
         Interior. For more information, see the official USGS copyright policy at
@@ -55,23 +55,34 @@
 Project-URL: repository, https://github.com/DOI-USGS/dataretrieval-python.git
 Keywords: USGS,water data
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests
-Requires-Dist: pandas
+Requires-Dist: pandas==2.*
 Provides-Extra: test
 Requires-Dist: pytest>5.0.0; extra == "test"
 Requires-Dist: pytest-cov[all]; extra == "test"
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: requests-mock; extra == "test"
+Requires-Dist: flake8; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx_rtd_theme; extra == "doc"
+Requires-Dist: nbsphinx; extra == "doc"
+Requires-Dist: nbsphinx_link; extra == "doc"
+Provides-Extra: nldi
+Requires-Dist: geopandas>=0.10; extra == "nldi"
 
 # dataretrieval: Download hydrologic data
 
+:warning: USGS data availability and format are changing on Water Quality Portal (WQP). Beginning in February 2024 data obtained from WQP legacy profiles will not include new USGS data or recent updates to existing data. 
+To view the status of changes in data availability and code functionality, visit: https://doi-usgs.github.io/dataRetrieval/articles/Status.html
+
 ## What is dataretrieval?
 `dataretrieval` was created to simplify the process of loading hydrologic data into the Python environment.
 Like the original R version [`dataRetrieval`](https://github.com/DOI-USGS/dataRetrieval),
 it is designed to retrieve the major data types of U.S. Geological Survey (USGS) hydrology
 data that are available on the Web, as well as data from the Water
 Quality Portal (WQP), which currently houses water quality data from the
 Environmental Protection Agency (EPA), U.S. Department of Agriculture
```

### Comparing `dataretrieval-1.0.6/README.md` & `dataretrieval-1.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # dataretrieval: Download hydrologic data
 
+:warning: USGS data availability and format are changing on Water Quality Portal (WQP). Beginning in February 2024 data obtained from WQP legacy profiles will not include new USGS data or recent updates to existing data. 
+To view the status of changes in data availability and code functionality, visit: https://doi-usgs.github.io/dataRetrieval/articles/Status.html
+
 ## What is dataretrieval?
 `dataretrieval` was created to simplify the process of loading hydrologic data into the Python environment.
 Like the original R version [`dataRetrieval`](https://github.com/DOI-USGS/dataRetrieval),
 it is designed to retrieve the major data types of U.S. Geological Survey (USGS) hydrology
 data that are available on the Web, as well as data from the Water
 Quality Portal (WQP), which currently houses water quality data from the
 Environmental Protection Agency (EPA), U.S. Department of Agriculture
```

### Comparing `dataretrieval-1.0.6/code.json` & `dataretrieval-1.0.7/code.json`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/dataretrieval/codes/states.py` & `dataretrieval-1.0.7/dataretrieval/codes/states.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 """List of 2-digit state codes with commented full names."""
 state_codes = [
-    'al', # Alabama
-    'ak', # Alaska
-    'az', # Arizona
-    'ar', # Arkansas
-    'ca', # California
-    'co', # Colorado
-    'ct', # Connecticut
-    'de', # Delaware
-    'dc', # District of Columbia
-    'fl', # Florida
-    'ga', # Georgia
-    'hi', # Hawaii
-    'id', # Idaho
-    'il', # Illinois
-    'in', # Indiana
-    'ia', # Iowa
-    'ks', # Kansas
-    'ky', # Kentucky
-    'la', # Louisiana
-    'me', # Maine
-    'md', # Maryland
-    'ma', # Massachusetts
-    'mi', # Michigan
-    'mn', # Minnesota
-    'ms', # Mississippi
-    'mo', # Missouri
-    'mt', # Montana
-    'ne', # Nebraska
-    'nv', # Nevada
-    'nh', # New Hampshire
-    'nj', # New Jersey
-    'nm', # New Mexico
-    'ny', # New York
-    'nc', # North Carolina
-    'nd', # North Dakota
-    'oh', # Ohio
-    'ok', # Oklahoma
-    'or', # Oregon
-    'pa', # Pennsylvania
-    'ri', # Rhode Island
-    'sc', # South Carolina
-    'sd', # South Dakota
-    'tn', # Tennessee
-    'tx', # Texas
-    'ut', # Utah
-    'vt', # Vermont
-    'va', # Virginia
-    'wa', # Washington
-    'wv', # West Virginia
-    'wi', # Wisconsin
-    'wy', # Wyoming
+    'al',  # Alabama
+    'ak',  # Alaska
+    'az',  # Arizona
+    'ar',  # Arkansas
+    'ca',  # California
+    'co',  # Colorado
+    'ct',  # Connecticut
+    'de',  # Delaware
+    'dc',  # District of Columbia
+    'fl',  # Florida
+    'ga',  # Georgia
+    'hi',  # Hawaii
+    'id',  # Idaho
+    'il',  # Illinois
+    'in',  # Indiana
+    'ia',  # Iowa
+    'ks',  # Kansas
+    'ky',  # Kentucky
+    'la',  # Louisiana
+    'me',  # Maine
+    'md',  # Maryland
+    'ma',  # Massachusetts
+    'mi',  # Michigan
+    'mn',  # Minnesota
+    'ms',  # Mississippi
+    'mo',  # Missouri
+    'mt',  # Montana
+    'ne',  # Nebraska
+    'nv',  # Nevada
+    'nh',  # New Hampshire
+    'nj',  # New Jersey
+    'nm',  # New Mexico
+    'ny',  # New York
+    'nc',  # North Carolina
+    'nd',  # North Dakota
+    'oh',  # Ohio
+    'ok',  # Oklahoma
+    'or',  # Oregon
+    'pa',  # Pennsylvania
+    'ri',  # Rhode Island
+    'sc',  # South Carolina
+    'sd',  # South Dakota
+    'tn',  # Tennessee
+    'tx',  # Texas
+    'ut',  # Utah
+    'vt',  # Vermont
+    'va',  # Virginia
+    'wa',  # Washington
+    'wv',  # West Virginia
+    'wi',  # Wisconsin
+    'wy',  # Wyoming
 ]
```

### Comparing `dataretrieval-1.0.6/dataretrieval/codes/timezones.py` & `dataretrieval-1.0.7/dataretrieval/codes/timezones.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/dataretrieval/nadp.py` & `dataretrieval-1.0.7/dataretrieval/nadp.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
-Tools for retrieving data from the National Atmospheric Deposition Program (NADP) including
-the National Trends Network (NTN), the Mercury Deposition Network (MDN).
+Tools for retrieving data from the National Atmospheric Deposition Program
+(NADP) including the National Trends Network (NTN), the Mercury Deposition
+Network (MDN).
 
 National Trends Network
 -----------------------
 The  NTN provides long-term records of precipitation chemistry across the
 United States. See https://nadp.slh.wisc.edu/ntn for more info.
 
 Mercury Deposition Network
@@ -24,40 +25,51 @@
     - include AIRMoN, AMNet, and AMoN
     - flexible handling of strings for parameters and measurement types
     - add errorchecking
     - add tests
 
 """
 
-import requests
-import zipfile
 import io
 import os
 import re
+import zipfile
 from os.path import basename
 
+import requests
 
 NADP_URL = 'https://nadp.slh.wisc.edu'
 NADP_MAP_EXT = 'filelib/maps'
 
-NTN_CONC_PARAMS = ['pH', 'So4', 'NO3', 'NH4', 'Ca',
-                   'Mg', 'K', 'Na', 'Cl', 'Br']
-NTN_DEP_PARAMS  = ['H', 'So4', 'NO3', 'NH4', 'Ca', 'Mg',
-                   'K', 'Na', 'Cl', 'Br', 'N', 'SPlusN']
+NTN_CONC_PARAMS = ['pH', 'So4', 'NO3', 'NH4', 'Ca', 'Mg', 'K', 'Na', 'Cl', 'Br']
+NTN_DEP_PARAMS = [
+    'H',
+    'So4',
+    'NO3',
+    'NH4',
+    'Ca',
+    'Mg',
+    'K',
+    'Na',
+    'Cl',
+    'Br',
+    'N',
+    'SPlusN',
+]
 
 NTN_MEAS_TYPE = ['conc', 'dep', 'precip']  # concentration or deposition
 
 
 class NADP_ZipFile(zipfile.ZipFile):
-    """Extend zipfile.ZipFile for working on data from NADP
-    """
+    """Extend zipfile.ZipFile for working on data from NADP"""
+
     def tif_name(self):
         """Get the name of the tif file in the zip file."""
         filenames = self.namelist()
-        r = re.compile(".*tif$")
+        r = re.compile('.*tif$')
         tif_list = list(filter(r.match, filenames))
         return tif_list[0]
 
     def tif(self):
         """Read the tif file in the zip file."""
         return self.read(self.tif_name())
 
@@ -89,31 +101,31 @@
 
     Examples
     --------
     .. code::
 
         >>> # get map of mercury concentration in 2010 and extract it to a path
         >>> data_path = dataretrieval.nadp.get_annual_MDN_map(
-        ...     measurement_type='conc', year='2010', path='somepath')
+        ...     measurement_type='conc', year='2010', path='somepath'
+        ... )
 
     """
-    url = '{}/{}/MDN/grids/'.format(NADP_URL, NADP_MAP_EXT)
+    url = f'{NADP_URL}/{NADP_MAP_EXT}/MDN/grids/'
 
-    filename = 'Hg_{}_{}.zip'.format(measurement_type, year)
+    filename = f'Hg_{measurement_type}_{year}.zip'
 
     z = get_zip(url, filename)
 
     if path:
         z.extractall(path)
 
-    return '{}{}{}'.format(path, os.sep, basename(filename))
+    return f'{path}{os.sep}{basename(filename)}'
 
 
-def get_annual_NTN_map(measurement_type, measurement=None, year=None,
-                       path="."):
+def get_annual_NTN_map(measurement_type, measurement=None, year=None, path='.'):
     """Download a NTN map from NDAP.
 
     This function looks for a zip file containing gridded information at:
     https://nadp.slh.wisc.edu/maps-data/ntn-gradient-maps/.
     The function will download the zip file and extract it, exposing the tif
     file at the provided path.
 
@@ -142,30 +154,31 @@
 
     Examples
     --------
     .. code::
 
         >>> # get a map of precipitation in 2015 and extract it to a path
         >>> data_path = dataretrieval.nadp.get_annual_NTN_map(
-        ...     measurement_type='Precip', year='2015', path='somepath')
+        ...     measurement_type='Precip', year='2015', path='somepath'
+        ... )
 
     """
-    url = '{}/{}/NTN/grids/{}/'.format(NADP_URL, NADP_MAP_EXT, year)
+    url = f'{NADP_URL}/{NADP_MAP_EXT}/NTN/grids/{year}/'
 
-    filename = '{}_{}.zip'.format(measurement_type, year)
+    filename = f'{measurement_type}_{year}.zip'
 
     if measurement:
-        filename = '{}_{}'.format(measurement, filename)
+        filename = f'{measurement}_{filename}'
 
     z = get_zip(url, filename)
 
     if path:
         z.extractall(path)
 
-    return '{}{}{}'.format(path, os.sep, basename(filename))
+    return f'{path}{os.sep}{basename(filename)}'
 
 
 def get_zip(url, filename):
     """Gets a ZipFile at url and returns it
 
     Parameters
     ----------
```

### Comparing `dataretrieval-1.0.6/dataretrieval/nwis.py` & `dataretrieval-1.0.7/dataretrieval/nwis.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,64 @@
-# -*- coding: utf-8 -*-
 """Functions for downloading data from the `National Water Information System (NWIS)`_.
 
 .. _National Water Information System (NWIS): https://waterdata.usgs.gov/nwis
 
 
 .. todo::
 
     * Create a test to check whether functions pull multiple sites
     * Work on multi-index capabilities.
     * Check that all timezones are handled properly for each service.
 
 """
 
+import re
 import warnings
-import pandas as pd
 from io import StringIO
-import re
+from typing import List, Optional, Tuple, Union
+
+import pandas as pd
+import requests
+
+from dataretrieval.utils import BaseMetadata, format_datetime, to_str
 
-from dataretrieval.utils import to_str, format_datetime, update_merge
-from dataretrieval.utils import BaseMetadata
 from .utils import query
 
 WATERDATA_BASE_URL = 'https://nwis.waterdata.usgs.gov/'
 WATERDATA_URL = WATERDATA_BASE_URL + 'nwis/'
 WATERSERVICE_URL = 'https://waterservices.usgs.gov/nwis/'
 PARAMCODES_URL = 'https://help.waterdata.usgs.gov/code/parameter_cd_nm_query?'
 ALLPARAMCODES_URL = 'https://help.waterdata.usgs.gov/code/parameter_cd_query?'
 
 WATERSERVICES_SERVICES = ['dv', 'iv', 'site', 'stat', 'gwlevels']
-WATERDATA_SERVICES = ['qwdata', 'measurements', 'peaks', 'pmcodes', 'water_use', 'ratings']
+WATERDATA_SERVICES = [
+    'qwdata',
+    'measurements',
+    'peaks',
+    'pmcodes',
+    'water_use',
+    'ratings',
+]
 
 
-def format_response(df: pd.DataFrame, service=None, **kwargs) -> pd.DataFrame:
+def format_response(
+    df: pd.DataFrame, service: Optional[str] = None, **kwargs
+) -> pd.DataFrame:
     """Setup index for response from query.
 
     This function formats the response from the NWIS web services, in
     particular it sets the index of the data frame. This function tries to
     convert the NWIS response into pandas datetime values localized to UTC,
     and if possible, uses these timestamps to define the data frame index.
 
     Parameters
     ----------
     df: ``pandas.DataFrame``
         The data frame to format
-    service: string
+    service: string, optional, default is None
         The NWIS service that was queried, important because the 'peaks'
         service returns a different format than the other services.
     **kwargs: optional
         Additional keyword arguments, e.g., 'multi_index'
 
     Returns
     -------
@@ -75,15 +86,15 @@
         df.set_index(['datetime'], inplace=True)
         if hasattr(df.index, 'tzinfo') and df.index.tzinfo is None:
             df = df.tz_localize('UTC')
 
     return df.sort_index()
 
 
-def preformat_peaks_response(df: pd.DataFrame):
+def preformat_peaks_response(df: pd.DataFrame) -> pd.DataFrame:
     """Datetime formatting for the 'peaks' service response.
 
     Function to format the datetime column of the 'peaks' service response.
 
     Parameters
     ----------
     df: ``pandas.DataFrame``
@@ -96,47 +107,58 @@
 
     """
     df['datetime'] = pd.to_datetime(df.pop('peak_dt'), errors='coerce')
     df.dropna(subset=['datetime'], inplace=True)
     return df
 
 
-def get_qwdata(sites=None, start=None, end=None,
-               multi_index=True, wide_format=True, datetime_index=True,
-               ssl_check=True, **kwargs):
+def get_qwdata(
+    sites: Optional[Union[List[str], str]] = None,
+    start: Optional[str] = None,
+    end: Optional[str] = None,
+    multi_index: bool = True,
+    wide_format: bool = True,
+    datetime_index: bool = True,
+    ssl_check: bool = True,
+    **kwargs,
+) -> Tuple[pd.DataFrame, BaseMetadata]:
     """
     Get water sample data from qwdata service.
 
     .. warning::
 
-        The NWIS qw data service is being deprecated. See this note from the
-        R package for more information:
-        https://doi-usgs.github.io/dataRetrieval/articles/qwdata_changes.html
+        WARNING: Beginning in March 2024 the NWIS qw data endpoint will
+        not deliver new data or updates to existing data.
+        Eventually the endpoint will be retired. For updated information visit:
+        https://waterdata.usgs.gov.nwis/qwdata
+        For additional details, see the R package vignette:
+        https://doi-usgs.github.io/dataRetrieval/articles/Status.html
         If you have additional questions about the qw data service,
-        email gs-w-IOW_PO_team@usgs.gov.
+        email CompTools@usgs.gov.
 
     Parameters
     ----------
-    sites: array of strings
+    sites: string or list of strings, optional, default is None
         If the qwdata parameter site_no is supplied, it will overwrite the
         sites parameter
-    start: string
+    start: string, optional, default is None
         If the qwdata parameter begin_date is supplied, it will overwrite the
         start parameter (YYYY-MM-DD)
-    end: string
+    end: string, optional, default is None
         If the qwdata parameter end_date is supplied, it will overwrite the
         end parameter (YYYY-MM-DD)
-    multi_index: boolean
-        If False, a dataframe with a single-level index (datetime) is returned
-    wide_format : boolean
+    multi_index: bool, optional
+        If False, a dataframe with a single-level index (datetime) is returned,
+        default is True
+    wide_format : bool, optional
         If True, return data in wide format with multiple samples per row and
-        one row per time
-    datetime_index : boolean
-        If True, create a datetime index
-    ssl_check: bool
+        one row per time, default is True
+    datetime_index : bool, optional
+        If True, create a datetime index, default is True
+    ssl_check: bool, optional
         If True, check SSL certificates, if False, do not check SSL,
         default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
@@ -147,94 +169,102 @@
 
     Examples
     --------
     .. doctest::
 
         >>> # get water sample information for site 11447650
         >>> df, md = dataretrieval.nwis.get_qwdata(
-        ...     sites='11447650', start='2010-01-01', end='2010-02-01')
+        ...     sites='11447650', start='2010-01-01', end='2010-02-01'
+        ... )
 
     """
+    warnings.warn(('WARNING: Starting in March 2024, the NWIS qw data endpoint is '
+                       'retiring and no longer receives updates. For more information, '
+                       'refer to https://waterdata.usgs.gov.nwis/qwdata and '
+                       'https://doi-usgs.github.io/dataRetrieval/articles/Status.html '
+                       'or email CompTools@usgs.gov.'))
+
+    _check_sites_value_types(sites)
+
+    kwargs['site_no'] = kwargs.pop('site_no', sites)
+    kwargs['begin_date'] = kwargs.pop('begin_date', start)
+    kwargs['end_date'] = kwargs.pop('end_date', end)
+    kwargs['multi_index'] = multi_index
     if wide_format:
         kwargs['qw_sample_wide'] = 'qw_sample_wide'
-    start = kwargs.pop('begin_date', start)
-    end = kwargs.pop('end_date', end)
-    sites = kwargs.pop('site_no', sites)
-    return _qwdata(site_no=sites, begin_date=start, end_date=end,
-                   datetime_index=datetime_index,
-                   multi_index=multi_index, ssl_check=ssl_check, **kwargs)
-
-
-def _qwdata(datetime_index=True, ssl_check=True, **kwargs):
-    # check number of sites, may need to create multiindex
-
-    payload = {'agency_cd': 'USGS',
-               'format': 'rdb',
-               'pm_cd_compare': 'Greater than',
-               'inventory_output': '0',
-               'rdb_inventory_output': 'file',
-               'TZoutput': '0',
-               'rdb_qw_attributes': 'expanded',
-               'date_format': 'YYYY-MM-DD',
-               'rdb_compression': 'value',
-               'submitted_form': 'brief_list'}
-    # 'qw_sample_wide': 'separated_wide'}
+
+    payload = {
+        'agency_cd': 'USGS',
+        'format': 'rdb',
+        'pm_cd_compare': 'Greater than',
+        'inventory_output': '0',
+        'rdb_inventory_output': 'file',
+        'TZoutput': '0',
+        'rdb_qw_attributes': 'expanded',
+        'date_format': 'YYYY-MM-DD',
+        'rdb_compression': 'value',
+        'submitted_form': 'brief_list',
+    }
 
     # check for parameter codes, and reformat query args
     qwdata_parameter_code_field = 'parameterCd'
     if kwargs.get(qwdata_parameter_code_field):
         parameter_codes = kwargs.pop(qwdata_parameter_code_field)
         parameter_codes = to_str(parameter_codes)
         kwargs['multiple_parameter_cds'] = parameter_codes
         kwargs['param_cd_operator'] = 'OR'
 
         search_criteria = kwargs.get('list_of_search_criteria')
         if search_criteria:
             kwargs['list_of_search_criteria'] = '{},{}'.format(
-                search_criteria, 'multiple_parameter_cds')
+                search_criteria, 'multiple_parameter_cds'
+            )
         else:
             kwargs['list_of_search_criteria'] = 'multiple_parameter_cds'
-        #search_criteria = kwargs.get('list_of_search_criteria
 
-    #kwargs = {**payload, **kwargs}
     kwargs.update(payload)
 
     warnings.warn(
-        "NWIS qw web services are being retired. " +
-        "See this note from the R package for more: " +
-        "https://doi-usgs.github.io/dataRetrieval/articles/qwdata_changes.html",
-        category=DeprecationWarning)
+        'NWIS qw web services are being retired. '
+        + 'See this note from the R package for more: '
+        + 'https://doi-usgs.github.io/dataRetrieval/articles/qwdata_changes.html',
+        category=DeprecationWarning,
+    )
     response = query_waterdata('qwdata', ssl_check=ssl_check, **kwargs)
 
     df = _read_rdb(response.text)
 
-    if datetime_index == True:
-        df = format_datetime(df, 'sample_dt', 'sample_tm',
-                             'sample_start_time_datum_cd')
+    if datetime_index is True:
+        df = format_datetime(df, 'sample_dt', 'sample_tm', 'sample_start_time_datum_cd')
 
     return format_response(df, **kwargs), NWIS_Metadata(response, **kwargs)
 
 
-def get_discharge_measurements(sites=None, start=None, end=None,
-                               ssl_check=True, **kwargs):
+def get_discharge_measurements(
+    sites: Optional[Union[List[str], str]] = None,
+    start: Optional[str] = None,
+    end: Optional[str] = None,
+    ssl_check: bool = True,
+    **kwargs,
+) -> Tuple[pd.DataFrame, BaseMetadata]:
     """
     Get discharge measurements from the waterdata service.
 
     Parameters
     ----------
-    sites: array of strings
+    sites: string or list of strings, optional, default is None
         If the qwdata parameter site_no is supplied, it will overwrite the
         sites parameter
-    start: string
+    start: string, optional, default is None
         If the qwdata parameter begin_date is supplied, it will overwrite the
         start parameter (YYYY-MM-DD)
-    end: string
+    end: string, optional, default is None
         If the qwdata parameter end_date is supplied, it will overwrite the
         end parameter (YYYY-MM-DD)
-    ssl_check: bool
+    ssl_check: bool, optional
         If True, check SSL certificates, if False, do not check SSL,
         default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
@@ -245,54 +275,61 @@
 
     Examples
     --------
     .. doctest::
 
         >>> # Get discharge measurements for site 05114000
         >>> df, md = dataretrieval.nwis.get_discharge_measurements(
-        ...     sites='05114000', start='2000-01-01', end='2000-01-30')
+        ...     sites='05114000', start='2000-01-01', end='2000-01-30'
+        ... )
 
         >>> # Get discharge measurements for sites in Alaska
         >>> df, md = dataretrieval.nwis.get_discharge_measurements(
-        ...     start='2012-01-09', end='2012-01-10', stateCd='AK')
+        ...     start='2012-01-09', end='2012-01-10', stateCd='AK'
+        ... )
 
     """
-    start = kwargs.pop('begin_date', start)
-    end = kwargs.pop('end_date', end)
-    sites = kwargs.pop('site_no', sites)
-    return _discharge_measurements(
-        site_no=sites, begin_date=start, end_date=end,
-        ssl_check=ssl_check, **kwargs)
+    _check_sites_value_types(sites)
 
+    kwargs['site_no'] = kwargs.pop('site_no', sites)
+    kwargs['begin_date'] = kwargs.pop('begin_date', start)
+    kwargs['end_date'] = kwargs.pop('end_date', end)
 
-def _discharge_measurements(ssl_check=True, **kwargs):
-    response = query_waterdata('measurements', format='rdb',
-                               ssl_check=ssl_check, **kwargs)
+    response = query_waterdata(
+        'measurements', format='rdb', ssl_check=ssl_check, **kwargs
+    )
     return _read_rdb(response.text), NWIS_Metadata(response, **kwargs)
 
 
-def get_discharge_peaks(sites=None, start=None, end=None,
-                        multi_index=True, ssl_check=True, **kwargs):
+def get_discharge_peaks(
+    sites: Optional[Union[List[str], str]] = None,
+    start: Optional[str] = None,
+    end: Optional[str] = None,
+    multi_index: bool = True,
+    ssl_check: bool = True,
+    **kwargs,
+) -> Tuple[pd.DataFrame, BaseMetadata]:
     """
     Get discharge peaks from the waterdata service.
 
     Parameters
     ----------
-    sites: array of strings
+    sites: string or list of strings, optional, default is None
         If the waterdata parameter site_no is supplied, it will overwrite the
         sites parameter
-    start: string
+    start: string, optional, default is None
         If the waterdata parameter begin_date is supplied, it will overwrite
         the start parameter (YYYY-MM-DD)
-    end: string
+    end: string, optional, default is None
         If the waterdata parameter end_date is supplied, it will overwrite
         the end parameter (YYYY-MM-DD)
-    multi_index: boolean
-        If False, a dataframe with a single-level index (datetime) is returned
-    ssl_check: bool
+    multi_index: bool, optional
+        If False, a dataframe with a single-level index (datetime) is returned,
+        default is True
+    ssl_check: bool, optional
         If True, check SSL certificates, if False, do not check SSL,
         default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
@@ -303,58 +340,68 @@
 
     Examples
     --------
     .. doctest::
 
         >>> # Get discharge peaks for site 01491000
         >>> df, md = dataretrieval.nwis.get_discharge_peaks(
-        ...     sites='01491000', start='1980-01-01', end='1990-01-01')
+        ...     sites='01491000', start='1980-01-01', end='1990-01-01'
+        ... )
 
         >>> # Get discharge peaks for sites in Hawaii
         >>> df, md = dataretrieval.nwis.get_discharge_peaks(
-        ...     start='1980-01-01', end='1980-01-02', stateCd='HI')
+        ...     start='1980-01-01', end='1980-01-02', stateCd='HI'
+        ... )
 
     """
-    start = kwargs.pop('begin_date', start)
-    end = kwargs.pop('end_date', end)
-    sites = kwargs.pop('site_no', sites)
-    return _discharge_peaks(site_no=sites, begin_date=start, end_date=end,
-                            multi_index=multi_index, ssl_check=ssl_check,
-                            **kwargs)
+    _check_sites_value_types(sites)
 
+    kwargs['site_no'] = kwargs.pop('site_no', sites)
+    kwargs['begin_date'] = kwargs.pop('begin_date', start)
+    kwargs['end_date'] = kwargs.pop('end_date', end)
+    kwargs['multi_index'] = multi_index
 
-def _discharge_peaks(ssl_check=True, **kwargs):
-    response = query_waterdata('peaks', format='rdb',
-                               ssl_check=ssl_check, **kwargs)
+    response = query_waterdata('peaks', format='rdb', ssl_check=ssl_check, **kwargs)
 
     df = _read_rdb(response.text)
 
     return format_response(df, service='peaks', **kwargs), NWIS_Metadata(
-        response, **kwargs)
+        response, **kwargs
+    )
 
 
-def get_gwlevels(sites=None, start='1851-01-01', end=None,
-                 multi_index=True, datetime_index=True,
-                 ssl_check=True, **kwargs):
+def get_gwlevels(
+    sites: Optional[Union[List[str], str]] = None,
+    start: str = '1851-01-01',
+    end: Optional[str] = None,
+    multi_index: bool = True,
+    datetime_index: bool = True,
+    ssl_check: bool = True,
+    **kwargs,
+) -> Tuple[pd.DataFrame, BaseMetadata]:
     """
     Queries the groundwater level service from waterservices
 
     Parameters
     ----------
-    start: string
+    sites: string or list of strings, optional, default is None
+        If the waterdata parameter site_no is supplied, it will overwrite the
+        sites parameter
+    start: string, optional, default is '1851-01-01'
         If the waterdata parameter begin_date is supplied, it will overwrite
-        the start parameter (defaults to '1851-01-01')
-    end: string
+        the start parameter
+    end: string, optional, default is None
         If the waterdata parameter end_date is supplied, it will overwrite the
         end parameter (YYYY-MM-DD)
-    multi_index: boolean
-        If False, a dataframe with a single-level index (datetime) is returned
-    datetime_index : boolean
-        If True, create a datetime index
-    ssl_check: bool
+    multi_index: bool, optional
+        If False, a dataframe with a single-level index (datetime) is returned,
+        default is True
+    datetime_index : bool, optional
+        If True, create a datetime index, default is True
+    ssl_check: bool, optional
         If True, check SSL certificates, if False, do not check SSL,
         default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
@@ -367,58 +414,56 @@
     --------
     .. doctest::
 
         >>> # Get groundwater levels for site 434400121275801
         >>> df, md = dataretrieval.nwis.get_gwlevels(sites='434400121275801')
 
     """
-    start = kwargs.pop('startDT', start)
-    end = kwargs.pop('endDT', end)
-    sites = kwargs.pop('sites', sites)
-    return _gwlevels(startDT=start, endDT=end,
-                     datetime_index=datetime_index, sites=sites,
-                     multi_index=multi_index, ssl_check=ssl_check, **kwargs)
+    _check_sites_value_types(sites)
 
-
-def _gwlevels(datetime_index=True, ssl_check=True, **kwargs):
+    kwargs['startDT'] = kwargs.pop('startDT', start)
+    kwargs['endDT'] = kwargs.pop('endDT', end)
+    kwargs['sites'] = kwargs.pop('sites', sites)
+    kwargs['multi_index'] = multi_index
 
     response = query_waterservices('gwlevels', ssl_check=ssl_check, **kwargs)
 
     df = _read_rdb(response.text)
 
-    if datetime_index == True:
+    if datetime_index is True:
         df = format_datetime(df, 'lev_dt', 'lev_tm', 'lev_tz_cd')
 
     return format_response(df, **kwargs), NWIS_Metadata(response, **kwargs)
 
 
-def get_stats(sites, ssl_check=True, **kwargs):
+def get_stats(
+    sites: Optional[Union[List[str], str]] = None, ssl_check: bool = True, **kwargs
+) -> Tuple[pd.DataFrame, BaseMetadata]:
     """
     Queries water services statistics information.
 
     For more information about the water services statistics service, visit
-    https://waterservices.usgs.gov/rest/Statistics-Service.html
+    https://waterservices.usgs.gov/docs/statistics/statistics-details/
 
     Parameters
     ----------
-    sites: string or list
+    sites: string or list of strings, optional, default is None
         USGS site number (or list of site numbers)
-    ssl_check: bool
+    ssl_check: bool, optional
         If True, check SSL certificates, if False, do not check SSL,
         default is True
+    **kwargs: optional
+        If supplied, will be used as query parameters
 
-    Additional Parameters
+    Keyword Arguments
     ---------------------
     statReportType: string
         daily (default), monthly, or annual
     statTypeCd: string
         all, mean, max, min, median
-    **kwargs: optional
-        Additional parameters that, if supplied, will be used as
-        query parameters
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Statistics data from the statistics service
     md: :obj:`dataretrieval.utils.Metadata`
         A custom metadata object
@@ -429,129 +474,170 @@
 
     Examples
     --------
     .. doctest::
 
         >>> # Get annual water statistics for a site
         >>> df, md = dataretrieval.nwis.get_stats(
-        ...     sites='01646500', statReportType='annual', statYearType='water')
+        ...     sites='01646500', statReportType='annual', statYearType='water'
+        ... )
 
         >>> # Get monthly statistics for a site
         >>> df, md = dataretrieval.nwis.get_stats(
-        ...     sites='01646500', statReportType='monthly')
+        ...     sites='01646500', statReportType='monthly'
+        ... )
 
     """
-    response = query_waterservices('stat', sites=sites,
-                                   ssl_check=ssl_check, **kwargs)
+    _check_sites_value_types(sites)
+
+    response = query_waterservices(
+        service='stat', sites=sites, ssl_check=ssl_check, **kwargs
+    )
 
     return _read_rdb(response.text), NWIS_Metadata(response, **kwargs)
 
 
-def query_waterdata(service, ssl_check=True, **kwargs):
+def query_waterdata(
+    service: str, ssl_check: bool = True, **kwargs
+) -> requests.models.Response:
     """
     Queries waterdata.
+
+    Parameters
+    ----------
+    service: string
+        Name of the service to query: 'site', 'stats', etc.
+    ssl_check: bool, optional
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
+    **kwargs: optional
+        If supplied, will be used as query parameters
+
+    Returns
+    -------
+    request: ``requests.models.Response``
+        The response object from the API request to the web service
     """
     major_params = ['site_no', 'state_cd']
-    bbox_params = ['nw_longitude_va', 'nw_latitude_va',
-                   'se_longitude_va', 'se_latitude_va']
+    bbox_params = [
+        'nw_longitude_va',
+        'nw_latitude_va',
+        'se_longitude_va',
+        'se_latitude_va',
+    ]
 
     if not any(key in kwargs for key in major_params + bbox_params):
         raise TypeError('Query must specify a major filter: site_no, stateCd, bBox')
 
-    elif any(key in kwargs for key in bbox_params) \
-            and not all(key in kwargs for key in bbox_params):
+    elif any(key in kwargs for key in bbox_params) and not all(
+        key in kwargs for key in bbox_params
+    ):
         raise TypeError('One or more lat/long coordinates missing or invalid.')
 
     if service not in WATERDATA_SERVICES:
         raise TypeError('Service not recognized')
 
     url = WATERDATA_URL + service
 
     return query(url, payload=kwargs, ssl_check=ssl_check)
 
 
-def query_waterservices(service, ssl_check=True, **kwargs):
+def query_waterservices(
+    service: str, ssl_check: bool = True, **kwargs
+) -> requests.models.Response:
     """
     Queries waterservices.usgs.gov
 
-    For more documentation see https://waterservices.usgs.gov/rest/
+    For more documentation see https://waterservices.usgs.gov/docs/
 
     .. note::
 
         User must specify one major filter: sites, stateCd, or bBox
 
     Parameters
     ----------
     service: string
-        String specifying the service to query: 'site', 'stats', etc.
-    ssl_check: bool
+        Name of the service to query: 'site', 'stats', etc.
+    ssl_check: bool, optional
         If True, check SSL certificates, if False, do not check SSL,
         default is True
+    ssl_check: bool, optional
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
+    **kwargs: optional
+        If supplied, will be used as query parameters
+
+    Keyword Arguments
+    ----------------
     bBox: string
         7-digit Hydrologic Unit Code (HUC)
     startDT: string
         Start date (e.g., '2017-12-31')
     endDT: string
         End date (e.g., '2018-01-01')
     modifiedSince: string
         Used to return only sites where attributes or period of record data
         have changed during the request period. String expected to be formatted
         in ISO-8601 duration format (e.g., 'P1D' for one day,
         'P1Y' for one year)
-    ssl_check: bool
-        If True, check SSL certificates, if False, do not check SSL,
-        default is True
-
-    Other Parameters
-    ----------------
-    **kwargs: optional
-        If supplied, will be used as query parameters
 
     Returns
     -------
     request: ``requests.models.Response``
         The response object from the API request to the web service
 
     """
-    if not any(key in kwargs for key in ['sites', 'stateCd', 'bBox', 'huc', 'countyCd']):
-        raise TypeError('Query must specify a major filter: sites, stateCd, bBox, huc, or countyCd')
+    if not any(
+        key in kwargs for key in ['sites', 'stateCd', 'bBox', 'huc', 'countyCd']
+    ):
+        raise TypeError(
+            'Query must specify a major filter: sites, stateCd, bBox, huc, or countyCd'
+        )
 
     if service not in WATERSERVICES_SERVICES:
         raise TypeError('Service not recognized')
 
     if 'format' not in kwargs:
         kwargs['format'] = 'rdb'
 
     url = WATERSERVICE_URL + service
 
     return query(url, payload=kwargs, ssl_check=ssl_check)
 
 
-def get_dv(sites=None, start=None, end=None, multi_index=True,
-           ssl_check=True, **kwargs):
+def get_dv(
+    sites: Optional[Union[List[str], str]] = None,
+    start: Optional[str] = None,
+    end: Optional[str] = None,
+    multi_index: bool = True,
+    ssl_check: bool = True,
+    **kwargs,
+) -> Tuple[pd.DataFrame, BaseMetadata]:
     """
     Get daily values data from NWIS and return it as a ``pandas.DataFrame``.
 
     .. note:
 
         If no start or end date are provided, only the most recent record
         is returned.
 
     Parameters
     ----------
-    start: string
+    sites: string or list of strings, optional, default is None
+        USGS site number (or list of site numbers)
+    start: string, optional, default is None
         If the waterdata parameter startDT is supplied, it will overwrite the
         start parameter (YYYY-MM-DD)
-    end: string
+    end: string, optional, default is None
         If the waterdata parameter endDT is supplied, it will overwrite the
         end parameter (YYYY-MM-DD)
-    multi_index: bool
+    multi_index: bool, optional
         If True, return a multi-index dataframe, if False, return a
         single-index dataframe, default is True
-    ssl_check: bool
+    ssl_check: bool, optional
         If True, check SSL certificates, if False, do not check SSL,
         default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
@@ -562,105 +648,103 @@
 
     Examples
     --------
     .. doctest::
 
         >>> # Get mean statistic daily values for site 04085427
         >>> df, md = dataretrieval.nwis.get_dv(
-        ...     sites='04085427', start='2012-01-01', end='2012-06-30',
-        ...     statCd='00003')
+        ...     sites='04085427', start='2012-01-01', end='2012-06-30', statCd='00003'
+        ... )
 
         >>> # Get the latest daily values for site 01646500
         >>> df, md = dataretrieval.nwis.get_dv(sites='01646500')
 
     """
-    start = kwargs.pop('startDT', start)
-    end = kwargs.pop('endDT', end)
-    sites = kwargs.pop('sites', sites)
-    return _dv(startDT=start, endDT=end, sites=sites,
-               multi_index=multi_index, ssl_check=ssl_check, **kwargs)
+    _check_sites_value_types(sites)
 
+    kwargs['startDT'] = kwargs.pop('startDT', start)
+    kwargs['endDT'] = kwargs.pop('endDT', end)
+    kwargs['sites'] = kwargs.pop('sites', sites)
+    kwargs['multi_index'] = multi_index
 
-def _dv(ssl_check=True, **kwargs):
-    response = query_waterservices('dv', format='json',
-                                   ssl_check=ssl_check, **kwargs)
+    response = query_waterservices('dv', format='json', ssl_check=ssl_check, **kwargs)
     df = _read_json(response.json())
 
     return format_response(df, **kwargs), NWIS_Metadata(response, **kwargs)
 
 
-def get_info(ssl_check=True, **kwargs):
+def get_info(ssl_check: bool = True, **kwargs) -> Tuple[pd.DataFrame, BaseMetadata]:
     """
     Get site description information from NWIS.
 
     **Note:** *Must specify one major parameter.*
 
     For additional parameter options see
-    https://waterservices.usgs.gov/rest/Site-Service.html#stateCd
+    https://waterservices.usgs.gov/docs/site-service/site-service-details/
 
     Parameters
     ----------
-    sites: string or list
+    ssl_check: bool, optional
+        If True, check SSL certificates, if False, do not check SSL,
+        default is True
+    **kwargs: optional
+        If supplied, will be used as query parameters
+
+    Keyword Arguments
+    ----------------
+    sites: string or list of strings
         A list of site numbers. Sites may be prefixed with an optional agency
         code followed by a colon.
     stateCd: string
         U.S. postal service (2-digit) state code. Only 1 state can be specified
         per request.
-    huc: string or list
+    huc: string or list of strings
         A list of hydrologic unit codes (HUC) or aggregated watersheds. Only 1
         major HUC can be specified per request, or up to 10 minor HUCs. A major
         HUC has two digits.
-    bBox: list
+    bBox: string or list of strings
         A contiguous range of decimal latitude and longitude, starting with the
         west longitude, then the south latitude, then the east longitude, and
         then the north latitude with each value separated by a comma. The
         product of the range of latitude range and longitude cannot exceed 25
         degrees. Whole or decimal degrees must be specified, up to six digits
         of precision. Minutes and seconds are not allowed.
-    countyCd: string or list
+    countyCd: string or list of strings
         A list of county numbers, in a 5 digit numeric format. The first two
         digits of a county's code are the FIPS State Code.
         (url: https://help.waterdata.usgs.gov/code/county_query?fmt=html)
-    ssl_check: bool
-        If True, check SSL certificates, if False, do not check SSL,
-        default is True
-    **kwargs: optional
-        If supplied, will be used as query parameters
-
-    Other Parameters
-    ----------------
     startDt: string
         Selects sites based on whether data was collected at a point in time
         beginning after startDt (start date). Dates must be in ISO-8601
         Calendar Date format (for example: 1990-01-01).
     endDt: string
         The end date for the period of record. Dates must be in ISO-8601
         Calendar Date format (for example: 1990-01-01).
     period: string
-        Selects sites based on whether or not they were active between now
+        Selects sites based on whether they were active between now
         and a time in the past. For example, period=P10W will select sites
         active in the last ten weeks.
     modifiedSince: string
         Returns only sites where site attributes or period of record data have
         changed during the request period.
-    parameterCd: string or list
+    parameterCd: string or list of strings
         Returns only site data for those sites containing the requested USGS
         parameter codes.
-    siteType: string or list
+    siteType: string or list of strings
         Restricts sites to those having one or more major and/or minor site
         types, such as stream, spring or well. For a list of all valid site
         types see https://help.waterdata.usgs.gov/site_tp_cd
         For example, siteType='ST' returns streams only.
     siteOutput: string ('basic' or 'expanded')
         Indicates the richness of metadata you want for site attributes. Note
         that for visually oriented formats like Google Map format, this
         argument has no meaning. Note: for performance reasons,
         siteOutput=expanded cannot be used if seriesCatalogOutput=true or with
         any values for outputDataTypeCd.
-    seriesCatalogOutput: boolean
+    seriesCatalogOutput: bool
         A switch that provides detailed period of record information for
         certain output formats. The period of record indicates date ranges for
         a certain kind of information about a site, for example the start and
         end dates for a site's daily mean streamflow.
 
     Returns
     -------
@@ -673,95 +757,122 @@
     --------
     .. doctest::
 
         >>> # Get site information for a single site
         >>> df, md = dataretrieval.nwis.get_info(sites='05114000')
 
         >>> # Get site information for multiple sites
-        >>> df, md = dataretrieval.nwis.get_info(
-        ...     sites=['05114000', '09423350'])
+        >>> df, md = dataretrieval.nwis.get_info(sites=['05114000', '09423350'])
 
     """
     seriesCatalogOutput = kwargs.pop('seriesCatalogOutput', None)
     if seriesCatalogOutput in ['True', 'TRUE', 'true', True]:
+
+        warnings.warn(('WARNING: Starting in March 2024, the NWIS qw data endpoint is '
+                       'retiring and no longer receives updates. For more information, '
+                       'refer to https://waterdata.usgs.gov.nwis/qwdata and '
+                       'https://doi-usgs.github.io/dataRetrieval/articles/Status.html '
+                       'or email CompTools@usgs.gov.'))
         # convert bool to string if necessary
         kwargs['seriesCatalogOutput'] = 'True'
     else:
         # cannot have both seriesCatalogOutput and the expanded format
         kwargs['siteOutput'] = 'Expanded'
 
     response = query_waterservices('site', ssl_check=ssl_check, **kwargs)
 
     return _read_rdb(response.text), NWIS_Metadata(response, **kwargs)
 
 
-def get_iv(sites=None, start=None, end=None, multi_index=True,
-           ssl_check=True, **kwargs):
+def get_iv(
+    sites: Optional[Union[List[str], str]] = None,
+    start: Optional[str] = None,
+    end: Optional[str] = None,
+    multi_index: bool = True,
+    ssl_check: bool = True,
+    **kwargs,
+) -> Tuple[pd.DataFrame, BaseMetadata]:
     """Get instantaneous values data from NWIS and return it as a DataFrame.
 
     .. note::
 
         If no start or end date are provided, only the most recent record
         is returned.
 
     Parameters
     ----------
-    start: string
+    sites: string or list of strings, optional, default is None
+        If the waterdata parameter site_no is supplied, it will overwrite the
+        sites parameter
+    start: string, optional, default is None
         If the waterdata parameter startDT is supplied, it will overwrite the
         start parameter (YYYY-MM-DD)
-    end: string
+    end: string, optional, default is None
         If the waterdata parameter endDT is supplied, it will overwrite the
         end parameter (YYYY-MM-DD)
-    ssl_check: bool
+    multi_index: bool, optional
+        If False, a dataframe with a single-level index (datetime) is returned,
+        default is True
+    ssl_check: bool, optional
         If True, check SSL certificates, if False, do not check SSL,
         default is True
+    **kwargs: optional
+        If supplied, will be used as query parameters
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Times series data from the NWIS JSON
     md: :obj:`dataretrieval.utils.Metadata`
         A custom metadata object
 
     Examples
     --------
     .. doctest::
 
         >>> # Get instantaneous discharge data for site 05114000
         >>> df, md = dataretrieval.nwis.get_iv(
-        ...     sites='05114000', start='2013-11-03', end='2013-11-03',
-        ...     parameterCd='00060')
+        ...     sites='05114000',
+        ...     start='2013-11-03',
+        ...     end='2013-11-03',
+        ...     parameterCd='00060',
+        ... )
+
+    """
+    _check_sites_value_types(sites)
+
+    kwargs['startDT'] = kwargs.pop('startDT', start)
+    kwargs['endDT'] = kwargs.pop('endDT', end)
+    kwargs['sites'] = kwargs.pop('sites', sites)
+    kwargs['multi_index'] = multi_index
+
+    response = query_waterservices(
+        service='iv', format='json', ssl_check=ssl_check, **kwargs
+    )
 
-    """
-    start = kwargs.pop('startDT', start)
-    end = kwargs.pop('endDT', end)
-    sites = kwargs.pop('sites', sites)
-    return _iv(startDT=start, endDT=end, sites=sites,
-               multi_index=multi_index, ssl_check=ssl_check, **kwargs)
-
-
-def _iv(ssl_check=True, **kwargs):
-    response = query_waterservices('iv', format='json',
-                                   ssl_check=ssl_check, **kwargs)
     df = _read_json(response.json())
     return format_response(df, **kwargs), NWIS_Metadata(response, **kwargs)
 
 
-def get_pmcodes(parameterCd='All', partial=True, ssl_check=True):
+def get_pmcodes(
+    parameterCd: Union[str, List[str]] = 'All',
+    partial: bool = True,
+    ssl_check: bool = True,
+) -> Tuple[pd.DataFrame, BaseMetadata]:
     """
     Return a ``pandas.DataFrame`` containing all NWIS parameter codes.
 
     Parameters
     ----------
-    parameterCd: string or list
+    parameterCd: string or list of strings, default is 'All'
         Accepts parameter codes or names
-    partial: boolean
+    partial: bool, optional
         Default is True (partial querying). If False, the function will query
-        only exact matches
-    ssl_check: bool
+        only exact matches, default is True
+    ssl_check: bool, optional
         If True, check SSL certificates, if False, do not check SSL,
         default is True
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Data retrieved from the NWIS web service.
@@ -769,138 +880,159 @@
         A custom metadata object
 
     Examples
     --------
     .. doctest::
 
         >>> # Get information about the '00060' pcode
-        >>> df, md = dataretrieval.nwis.get_pmcodes(
-        ...     parameterCd='00060', partial=False)
+        >>> df, md = dataretrieval.nwis.get_pmcodes(parameterCd='00060', partial=False)
 
         >>> # Get information about all 'Discharge' pcodes
         >>> df, md = dataretrieval.nwis.get_pmcodes(
-        ...     parameterCd='Discharge', partial=True)
+        ...     parameterCd='Discharge', partial=True
+        ... )
 
     """
-    if parameterCd is None:
-        raise TypeError('The query must include a parameter name or code')
 
     payload = {'fmt': 'rdb'}
     url = PARAMCODES_URL
 
     if isinstance(parameterCd, str):  # when a single code or name is given
-        if parameterCd.lower() == "all":
+        if parameterCd.lower() == 'all':
             payload.update({'group_cd': '%'})
             url = ALLPARAMCODES_URL
             response = query(url, payload, ssl_check=ssl_check)
             return _read_rdb(response.text), NWIS_Metadata(response)
 
         else:
             parameterCd = [parameterCd]
 
     if not isinstance(parameterCd, list):
-        raise TypeError('Parameter information (code or name) must be type string or list')
+        raise TypeError(
+            'Parameter information (code or name) must be type string or list'
+        )
 
     # Querying with a list of parameters names, codes, or mixed
-    l = []
+    return_list = []
     for param in parameterCd:
         if isinstance(param, str):
             if partial:
-                param ='%{0}%'.format(param)
+                param = f'%{param}%'
             payload.update({'parm_nm_cd': param})
             response = query(url, payload, ssl_check=ssl_check)
             if len(response.text.splitlines()) < 10:  # empty query
-                raise TypeError('One of the parameter codes or names entered does not return any information,'\
-                                ' please try a different value')
-            l.append(_read_rdb(response.text))
+                raise TypeError(
+                    'One of the parameter codes or names entered does not'
+                    'return any information, please try a different value'
+                )
+            return_list.append(_read_rdb(response.text))
         else:
             raise TypeError('Parameter information (code or name) must be type string')
-    return pd.concat(l), NWIS_Metadata(response)
+    return pd.concat(return_list), NWIS_Metadata(response)
 
 
-def get_water_use(years="ALL", state=None, counties="ALL", categories="ALL",
-                  ssl_check=True):
+def get_water_use(
+    years: Union[str, List[str]] = 'ALL',
+    state: Optional[str] = None,
+    counties: Union[str, List[str]] = 'ALL',
+    categories: Union[str, List[str]] = 'ALL',
+    ssl_check: bool = True,
+) -> Tuple[pd.DataFrame, BaseMetadata]:
     """
     Water use data retrieval from USGS (NWIS).
 
     Parameters
     ----------
-    years: list-like
+    years: string or list of strings
         List or comma delimited string of years.  Must be years ending in 0 or
-        5, or "ALL", which retrieves all available years
-    state: string
+        5, or "ALL", which retrieves all available years, default is "ALL"
+    state: string, optional, default is None
         full name, abbreviation or id
-    county: string
-        County IDs from county lookup or "ALL"
-    categories: list-like
-        List or comma delimited string of Two-letter category abbreviations
-    ssl_check: bool
+    counties: string or list of strings
+        County IDs from county lookup or "ALL", default is "ALL"
+    categories: string or list of strings
+        List or comma delimited string of Two-letter category abbreviations,
+        default is "ALL"
+    ssl_check: bool, optional
         If True, check SSL certificates, if False, do not check SSL,
         default is True
-    **kwargs: optional
-        If supplied, will be used as query parameters
 
     Returns
     -------
     df: ``pandas.DataFrame``
         Data from NWIS
     md: :obj:`dataretrieval.utils.Metadata`
         A custom metadata object
 
     Examples
     --------
     .. doctest::
 
         >>> # Get total population for RI from the NWIS water use service
         >>> df, md = dataretrieval.nwis.get_water_use(
-        ...     years='2000', state='RI', categories='TP')
+        ...     years='2000', state='RI', categories='TP'
+        ... )
 
         >>> # Get the national total water use for livestock in Bgal/day
-        >>> df, md = dataretrieval.nwis.get_water_use(
-        ...     years='2010', categories='L')
+        >>> df, md = dataretrieval.nwis.get_water_use(years='2010', categories='L')
 
         >>> # Get 2005 domestic water use for Apache County in Arizona
         >>> df, md = dataretrieval.nwis.get_water_use(
-        ...     years='2005', state='Arizona',
-        ...     counties='001', categories='DO')
+        ...     years='2005', state='Arizona', counties='001', categories='DO'
+        ... )
 
     """
-    payload = {'rdb_compression': 'value',
-               'format': 'rdb',
-               'wu_year': years,
-               'wu_category': categories,
-               'wu_county': counties}
+    if years:
+        if not isinstance(years, list) and not isinstance(years, str):
+            raise TypeError('years must be a string or a list of strings')
+
+    if counties:
+        if not isinstance(counties, list) and not isinstance(counties, str):
+            raise TypeError('counties must be a string or a list of strings')
+
+    if categories:
+        if not isinstance(categories, list) and not isinstance(categories, str):
+            raise TypeError('categories must be a string or a list of strings')
+
+    payload = {
+        'rdb_compression': 'value',
+        'format': 'rdb',
+        'wu_year': years,
+        'wu_category': categories,
+        'wu_county': counties,
+    }
     url = WATERDATA_URL + 'water_use'
     if state is not None:
-        url = WATERDATA_BASE_URL + state + "/nwis/water_use"
-        payload.update({"wu_area": "county"})
+        url = WATERDATA_BASE_URL + state + '/nwis/water_use'
+        payload.update({'wu_area': 'county'})
     response = query(url, payload, ssl_check=ssl_check)
     return _read_rdb(response.text), NWIS_Metadata(response)
 
 
-def get_ratings(site=None, file_type="base", ssl_check=True, **kwargs):
+def get_ratings(
+    site: Optional[str] = None,
+    file_type: str = 'base',
+    ssl_check: bool = True,
+    **kwargs,
+) -> Tuple[pd.DataFrame, BaseMetadata]:
     """
     Rating table for an active USGS streamgage retrieval.
 
     Reads current rating table for an active USGS streamgage from NWISweb.
     Data is retrieved from https://waterdata.usgs.gov/nwis.
 
     Parameters
     ----------
-    site: string
+    site: string, optional, default is None
         USGS site number.  This is usually an 8 digit number as a string.
         If the nwis parameter site_no is supplied, it will overwrite the site
         parameter
-    base: string
+    file_type: string, default is "base"
         can be "base", "corr", or "exsa"
-    county: string
-        County IDs from county lookup or "ALL"
-    categories: list-like
-        List or comma delimited string of Two-letter category abbreviations
-    ssl_check: bool
+    ssl_check: bool, optional
         If True, check SSL certificates, if False, do not check SSL,
         default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Return
     ------
@@ -914,96 +1046,118 @@
     .. doctest::
 
         >>> # Get the rating table for USGS streamgage 01594440
         >>> df, md = dataretrieval.nwis.get_ratings(site='01594440')
 
     """
     site = kwargs.pop('site_no', site)
-    return _ratings(site=site, file_type=file_type, ssl_check=ssl_check,
-                    **kwargs)
 
-
-def _ratings(site, file_type, ssl_check=True):
     payload = {}
     url = WATERDATA_BASE_URL + 'nwisweb/get_ratings/'
     if site is not None:
-        payload.update({"site_no": site})
+        payload.update({'site_no': site})
     if file_type is not None:
-        if file_type not in ["base", "corr", "exsa"]:
-            raise ValueError('Unrecognized file_type: {}, must be "base", "corr" or "exsa"'.format(file_type))
-        payload.update({"file_type" : file_type})
+        if file_type not in ['base', 'corr', 'exsa']:
+            raise ValueError(
+                f'Unrecognized file_type: {file_type}, must be "base", "corr" or "exsa"'
+            )
+        payload.update({'file_type': file_type})
     response = query(url, payload, ssl_check=ssl_check)
     return _read_rdb(response.text), NWIS_Metadata(response, site_no=site)
 
 
-def what_sites(ssl_check=True, **kwargs):
+def what_sites(ssl_check: bool = True, **kwargs) -> Tuple[pd.DataFrame, BaseMetadata]:
     """
     Search NWIS for sites within a region with specific data.
 
     Parameters
     ----------
-    ssl_check: bool
+    ssl_check: bool, optional
         If True, check SSL certificates, if False, do not check SSL,
         default is True
     **kwargs: optional
         Accepts the same parameters as :obj:`dataretrieval.nwis.get_info`
 
+    Return
+    ------
+    df: ``pandas.DataFrame``
+        Formatted requested data
+    md: :obj:`dataretrieval.utils.Metadata`
+        A custom metadata object
+
     Examples
     --------
     .. doctest::
 
         >>> # get information about a single site
         >>> df, md = dataretrieval.nwis.what_sites(sites='05114000')
 
         >>> # get information about sites with phosphorus in Ohio
-        >>> df, md = dataretrieval.nwis.what_sites(
-        ...     stateCd='OH', parameterCd='00665')
+        >>> df, md = dataretrieval.nwis.what_sites(stateCd='OH', parameterCd='00665')
 
     """
 
-    response = query_waterservices(service='site', ssl_check=ssl_check,
-                                   **kwargs)
+    response = query_waterservices(service='site', ssl_check=ssl_check, **kwargs)
 
     df = _read_rdb(response.text)
 
     return df, NWIS_Metadata(response, **kwargs)
 
 
-def get_record(sites=None, start=None, end=None,
-               multi_index=True, wide_format=True, datetime_index=True,
-               state=None, service='iv', ssl_check=True, **kwargs):
+def get_record(
+    sites: Optional[Union[List[str], str]] = None,
+    start: Optional[str] = None,
+    end: Optional[str] = None,
+    multi_index: bool = True,
+    wide_format: bool = True,
+    datetime_index: bool = True,
+    state: Optional[str] = None,
+    service: str = 'iv',
+    ssl_check: bool = True,
+    **kwargs,
+) -> pd.DataFrame:
     """
     Get data from NWIS and return it as a ``pandas.DataFrame``.
 
     .. note::
 
         If no start or end date are provided, only the most recent record is
         returned.
 
     Parameters
     ----------
-    sites: list-like
+    sites: string or list of strings, optional, default is None
         List or comma delimited string of site.
-    start: string
+    start: string, optional, default is None
         Starting date of record (YYYY-MM-DD)
-    end: string
+    end: string, optional, default is None
         Ending date of record. (YYYY-MM-DD)
-    service: string
+    multi_index: bool, optional
+        If False, a dataframe with a single-level index (datetime) is returned,
+        default is True
+    wide_format : bool, optional
+        If True, return data in wide format with multiple samples per row and
+        one row per time, default is True
+    datetime_index : bool, optional
+        If True, create a datetime index. default is True
+    state: string, optional, default is None
+        full name, abbreviation or id
+    service: string, default is 'iv'
         - 'iv' : instantaneous data
         - 'dv' : daily mean data
         - 'qwdata' : discrete samples
         - 'site' : site description
         - 'measurements' : discharge measurements
         - 'peaks': discharge peaks
         - 'gwlevels': groundwater levels
         - 'pmcodes': get parameter codes
         - 'water_use': get water use data
         - 'ratings': get rating table
         - 'stat': get statistics
-    ssl_check: bool
+    ssl_check: bool, optional
         If True, check SSL certificates, if False, do not check SSL,
         default is True
     **kwargs: optional
         If supplied, will be used as query parameters
 
     Returns
     -------
@@ -1016,93 +1170,120 @@
         >>> # Get latest instantaneous data from site 01585200
         >>> df = dataretrieval.nwis.get_record(sites='01585200', service='iv')
 
         >>> # Get latest daily mean data from site 01585200
         >>> df = dataretrieval.nwis.get_record(sites='01585200', service='dv')
 
         >>> # Get all discrete sample data from site 01585200
-        >>> df = dataretrieval.nwis.get_record(
-        ...     sites='01585200', service='qwdata')
+        >>> df = dataretrieval.nwis.get_record(sites='01585200', service='qwdata')
 
         >>> # Get site description for site 01585200
-        >>> df = dataretrieval.nwis.get_record(
-        ...     sites='01585200', service='site')
+        >>> df = dataretrieval.nwis.get_record(sites='01585200', service='site')
 
         >>> # Get discharge measurements for site 01585200
-        >>> df = dataretrieval.nwis.get_record(
-        ...     sites='01585200', service='measurements')
+        >>> df = dataretrieval.nwis.get_record(sites='01585200', service='measurements')
 
         >>> # Get discharge peaks for site 01585200
-        >>> df = dataretrieval.nwis.get_record(
-        ...     sites='01585200', service='peaks')
+        >>> df = dataretrieval.nwis.get_record(sites='01585200', service='peaks')
 
         >>> # Get latest groundwater level for site 434400121275801
         >>> df = dataretrieval.nwis.get_record(
-        ...     sites='434400121275801', service='gwlevels')
+        ...     sites='434400121275801', service='gwlevels'
+        ... )
 
         >>> # Get information about the discharge parameter code
-        >>> df = dataretrieval.nwis.get_record(
-        ...     service='pmcodes', parameterCd='00060')
+        >>> df = dataretrieval.nwis.get_record(service='pmcodes', parameterCd='00060')
 
         >>> # Get water use data for livestock nationally in 2010
         >>> df = dataretrieval.nwis.get_record(
-        ...     service='water_use', years='2010', categories='L')
+        ...     service='water_use', years='2010', categories='L'
+        ... )
 
         >>> # Get rating table for USGS streamgage 01585200
-        >>> df = dataretrieval.nwis.get_record(
-        ...     sites='01585200', service='ratings')
+        >>> df = dataretrieval.nwis.get_record(sites='01585200', service='ratings')
 
         >>> # Get annual statistics for USGS station 01646500
         >>> df = dataretrieval.nwis.get_record(
-        ...     sites='01646500', service='stat', statReportType='annual',
-        ...     statYearType='water')
+        ...     sites='01646500',
+        ...     service='stat',
+        ...     statReportType='annual',
+        ...     statYearType='water',
+        ... )
 
     """
+    _check_sites_value_types(sites)
+
     if service not in WATERSERVICES_SERVICES + WATERDATA_SERVICES:
-        raise TypeError('Unrecognized service: {}'.format(service))
+        raise TypeError(f'Unrecognized service: {service}')
 
     if service == 'iv':
-        df, _ = get_iv(sites=sites, startDT=start, endDT=end,
-                       multi_index=multi_index, ssl_check=ssl_check, **kwargs)
+        df, _ = get_iv(
+            sites=sites,
+            startDT=start,
+            endDT=end,
+            multi_index=multi_index,
+            ssl_check=ssl_check,
+            **kwargs,
+        )
         return df
 
     elif service == 'dv':
-        df, _ = get_dv(sites=sites, startDT=start, endDT=end,
-                       multi_index=multi_index, ssl_check=ssl_check, **kwargs)
+        df, _ = get_dv(
+            sites=sites,
+            startDT=start,
+            endDT=end,
+            multi_index=multi_index,
+            ssl_check=ssl_check,
+            **kwargs,
+        )
         return df
 
     elif service == 'qwdata':
-        df, _ = get_qwdata(site_no=sites, begin_date=start, end_date=end,
-                           multi_index=multi_index,
-                           wide_format=wide_format, ssl_check=ssl_check,
-                           **kwargs)
+        df, _ = get_qwdata(
+            site_no=sites,
+            begin_date=start,
+            end_date=end,
+            multi_index=multi_index,
+            wide_format=wide_format,
+            ssl_check=ssl_check,
+            **kwargs,
+        )
         return df
 
     elif service == 'site':
         df, _ = get_info(sites=sites, ssl_check=ssl_check, **kwargs)
         return df
 
     elif service == 'measurements':
-        df, _ = get_discharge_measurements(site_no=sites, begin_date=start,
-                                           end_date=end, ssl_check=ssl_check,
-                                           **kwargs)
+        df, _ = get_discharge_measurements(
+            site_no=sites, begin_date=start, end_date=end, ssl_check=ssl_check, **kwargs
+        )
         return df
 
     elif service == 'peaks':
-        df, _ = get_discharge_peaks(site_no=sites, begin_date=start,
-                                    end_date=end,
-                                    multi_index=multi_index,
-                                    ssl_check=ssl_check, **kwargs)
+        df, _ = get_discharge_peaks(
+            site_no=sites,
+            begin_date=start,
+            end_date=end,
+            multi_index=multi_index,
+            ssl_check=ssl_check,
+            **kwargs,
+        )
         return df
 
     elif service == 'gwlevels':
-        df, _ = get_gwlevels(sites=sites, startDT=start, endDT=end,
-                             multi_index=multi_index,
-                             datetime_index=datetime_index,
-                             ssl_check=ssl_check, **kwargs)
+        df, _ = get_gwlevels(
+            sites=sites,
+            startDT=start,
+            endDT=end,
+            multi_index=multi_index,
+            datetime_index=datetime_index,
+            ssl_check=ssl_check,
+            **kwargs,
+        )
         return df
 
     elif service == 'pmcodes':
         df, _ = get_pmcodes(ssl_check=ssl_check, **kwargs)
         return df
 
     elif service == 'water_use':
@@ -1114,15 +1295,15 @@
         return df
 
     elif service == 'stat':
         df, _ = get_stats(sites=sites, ssl_check=ssl_check, **kwargs)
         return df
 
     else:
-        raise TypeError('{} service not yet implemented'.format(service))
+        raise TypeError(f'{service} service not yet implemented')
 
 
 def _read_json(json):
     """
     Reads a NWIS Water Services formatted JSON into a ``pandas.DataFrame``.
 
     Parameters
@@ -1134,68 +1315,95 @@
     -------
     df: ``pandas.DataFrame``
         Times series data from the NWIS JSON
     md: :obj:`dataretrieval.utils.Metadata`
         A custom metadata object
 
     """
-    merged_df = pd.DataFrame()
+    merged_df = pd.DataFrame(columns=['site_no', 'datetime'])
 
-    for timeseries in json['value']['timeSeries']:
-
-        site_no = timeseries['sourceInfo']['siteCode'][0]['value']
-        param_cd = timeseries['variable']['variableCode'][0]['value']
-        # check whether min, max, mean record XXX
-        option = timeseries['variable']['options']['option'][0].get('value')
-
-        # loop through each parameter in timeseries.
-        for parameter in timeseries['values']:
-            col_name = param_cd
-            method = parameter['method'][0]['methodDescription']
-
-            # if len(timeseries['values']) > 1 and method:
-            if method:
-                # get method, format it, and append to column name
-                method = method.strip("[]()").lower()
-                col_name = '{}_{}'.format(col_name, method)
-
-            if option:
-                col_name = '{}_{}'.format(col_name, option)
-
-            record_json = parameter['value']
-
-            if not record_json:
-                # no data in record
-                continue
-            # should be able to avoid this by dumping
-            record_json = str(record_json).replace("'", '"')
-
-            # read json, converting all values to float64 and all qualifiers
-            # Lists can't be hashed, thus we cannot df.merge on a list column
-            record_df = pd.read_json(StringIO(record_json),
-                                     orient='records',
-                                     dtype={'value': 'float64',
-                                            'qualifiers': 'unicode'},
-                                     convert_dates=False)
-
-            record_df['qualifiers'] = (record_df['qualifiers']
-                                       .str.strip("[]").str.replace("'", ""))
-            record_df['site_no'] = site_no
-
-            record_df.rename(columns={'value': col_name,
-                                      'dateTime': 'datetime',
-                                      'qualifiers': col_name + '_cd'},
-                             inplace=True)
-
-            if merged_df.empty:
-                merged_df = record_df
-
-            else:
-                merged_df = update_merge(merged_df, record_df, na_only=True,
-                                         on=['site_no', 'datetime'])
+    site_list = [
+        ts['sourceInfo']['siteCode'][0]['value'] for ts in json['value']['timeSeries']
+    ]
+
+    # create a list of indexes for each change in site no
+    # for example, [0, 21, 22] would be the first and last indeces
+    index_list = [0]
+    index_list.extend(
+        [i + 1 for i, (a, b) in enumerate(zip(site_list[:-1], site_list[1:])) if a != b]
+    )
+    index_list.append(len(site_list))
+
+    for i in range(len(index_list) - 1):
+        start = index_list[i]  # [0]
+        end = index_list[i + 1]  # [21]
+
+        # grab a block containing timeseries 0:21,
+        # which are all from the same site
+        site_block = json['value']['timeSeries'][start:end]
+        if not site_block:
+            continue
+
+        site_no = site_block[0]['sourceInfo']['siteCode'][0]['value']
+        site_df = pd.DataFrame(columns=['datetime'])
+
+        for timeseries in site_block:
+            param_cd = timeseries['variable']['variableCode'][0]['value']
+            # check whether min, max, mean record XXX
+            option = timeseries['variable']['options']['option'][0].get('value')
+
+            # loop through each parameter in timeseries, then concat to the merged_df
+            for parameter in timeseries['values']:
+                col_name = param_cd
+                method = parameter['method'][0]['methodDescription']
+
+                # if len(timeseries['values']) > 1 and method:
+                if method:
+                    # get method, format it, and append to column name
+                    method = method.strip('[]()').lower()
+                    col_name = f'{col_name}_{method}'
+
+                if option:
+                    col_name = f'{col_name}_{option}'
+
+                record_json = parameter['value']
+
+                if not record_json:
+                    # no data in record
+                    continue
+                # should be able to avoid this by dumping
+                record_json = str(record_json).replace("'", '"')
+
+                # read json, converting all values to float64 and all qualifiers
+                # Lists can't be hashed, thus we cannot df.merge on a list column
+                record_df = pd.read_json(
+                    StringIO(record_json),
+                    orient='records',
+                    dtype={'value': 'float64', 'qualifiers': 'unicode'},
+                    convert_dates=False,
+                )
+
+                record_df['qualifiers'] = (
+                    record_df['qualifiers'].str.strip('[]').str.replace("'", '')
+                )
+
+                record_df.rename(
+                    columns={
+                        'value': col_name,
+                        'dateTime': 'datetime',
+                        'qualifiers': col_name + '_cd',
+                    },
+                    inplace=True,
+                )
+
+                site_df = site_df.merge(record_df, how='outer', on='datetime')
+
+        # end of site loop
+        site_df['site_no'] = site_no
+        merged_df = pd.concat([merged_df, site_df])
 
     # convert to datetime, normalizing the timezone to UTC when doing so
     if 'datetime' in merged_df.columns:
         merged_df['datetime'] = pd.to_datetime(merged_df['datetime'], utc=True)
 
     return merged_df
 
@@ -1221,46 +1429,65 @@
         # ignore comment lines
         if line.startswith('#'):
             count = count + 1
 
         else:
             break
 
-    fields = re.split("[\t]", rdb.splitlines()[count])
-    fields = [field.replace(",", "") for field in fields]
-    dtypes = {'site_no': str, 'dec_long_va': float,
-              'dec_lat_va': float, 'parm_cd': str, 'parameter_cd': str}
-
-    df = pd.read_csv(StringIO(rdb), delimiter='\t', skiprows=count + 2,
-                     names=fields, na_values='NaN', dtype=dtypes)
+    fields = re.split('[\t]', rdb.splitlines()[count])
+    fields = [field.replace(',', '') for field in fields]
+    dtypes = {
+        'site_no': str,
+        'dec_long_va': float,
+        'dec_lat_va': float,
+        'parm_cd': str,
+        'parameter_cd': str,
+    }
+
+    df = pd.read_csv(
+        StringIO(rdb),
+        delimiter='\t',
+        skiprows=count + 2,
+        names=fields,
+        na_values='NaN',
+        dtype=dtypes,
+    )
 
     df = format_response(df)
     return df
 
+
+def _check_sites_value_types(sites):
+    if sites:
+        if not isinstance(sites, list) and not isinstance(sites, str):
+            raise TypeError('sites must be a string or a list of strings')
+
+
 class NWIS_Metadata(BaseMetadata):
     """Metadata class for NWIS service, derived from BaseMetadata.
-    
+
     Attributes
     ----------
     url : str
         Response url
     query_time: datetme.timedelta
         Response elapsed time
     header: requests.structures.CaseInsensitiveDict
         Response headers
     comments: str | None
         Metadata comments, if any
     site_info: tuple[pd.DataFrame, NWIS_Metadata] | None
         Site information if the query included `site_no`, `sites`, `stateCd`,
-        `huc`, `countyCd` or `bBox`. `site_no` is preferred over `sites` if 
+        `huc`, `countyCd` or `bBox`. `site_no` is preferred over `sites` if
         both are present.
     variable_info: tuple[pd.DataFrame, NWIS_Metadata] | None
-        Variable information if the query included `parameterCd`. 
-    
+        Variable information if the query included `parameterCd`.
+
     """
+
     def __init__(self, response, **parameters) -> None:
         """Generates a standard set of metadata informed by the response with specific
         metadata for NWIS data.
 
         Parameters
         ----------
         response: Response
@@ -1272,54 +1499,52 @@
         -------
         md: :obj:`dataretrieval.nwis.NWIS_Metadata`
             A ``dataretrieval`` custom :obj:`dataretrieval.nwis.NWIS_Metadata` object.
 
         """
         super().__init__(response)
 
-        comments = ""
+        comments = ''
         for line in response.text.splitlines():
-            if line.startswith("#"):
-                comments += line.lstrip("#") + "\n"
+            if line.startswith('#'):
+                comments += line.lstrip('#') + '\n'
         if comments:
             self.comment = comments
 
         self._parameters = parameters
 
     @property
-    def site_info(self):
+    def site_info(self) -> Optional[Tuple[pd.DataFrame, BaseMetadata]]:
         """
         Return
         ------
         df: ``pandas.DataFrame``
             Formatted requested data from calling `nwis.what_sites`
         md: :obj:`dataretrieval.nwis.NWIS_Metadata`
-            A NWIS_Metadata object        
+            A NWIS_Metadata object
         """
         if 'site_no' in self._parameters:
             return what_sites(sites=self._parameters['site_no'])
 
         elif 'sites' in self._parameters:
             return what_sites(sites=self._parameters['sites'])
 
         elif 'stateCd' in self._parameters:
             return what_sites(stateCd=self._parameters['stateCd'])
-        
+
         elif 'huc' in self._parameters:
             return what_sites(huc=self._parameters['huc'])
-        
+
         elif 'countyCd' in self._parameters:
             return what_sites(countyCd=self._parameters['countyCd'])
-        
+
         elif 'bBox' in self._parameters:
             return what_sites(bBox=self._parameters['bBox'])
-        
+
         else:
             return None  # don't set metadata site_info attribute
 
     @property
-    def variable_info(self):
-        
+    def variable_info(self) -> Optional[Tuple[pd.DataFrame, BaseMetadata]]:
         # define variable_info metadata based on parameterCd if available
         if 'parameterCd' in self._parameters:
             return get_pmcodes(parameterCd=self._parameters['parameterCd'])
-
```

### Comparing `dataretrieval-1.0.6/dataretrieval/streamstats.py` & `dataretrieval-1.0.7/dataretrieval/streamstats.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This module is a wrapper for the streamstats API (`streamstats documentation`_).
 
 .. _streamstats documentation: https://streamstats.usgs.gov/streamstatsservices/#/
 
 """
 
 import json
+
 import requests
 
 
 def download_workspace(workspaceID, format=''):
     """Function to download streamstats workspace.
 
     Parameters
@@ -31,20 +32,20 @@
     payload = {'workspaceID': workspaceID, 'format': format}
     url = 'https://streamstats.usgs.gov/streamstatsservices/download'
 
     r = requests.get(url, params=payload)
 
     r.raise_for_status()
     return r
-    #data = r.raw.read()
+    # data = r.raw.read()
 
-    #with open(filepath, 'wb') as f:
+    # with open(filepath, 'wb') as f:
     #    f.write(data)
 
-    #return
+    # return
 
 
 def get_sample_watershed():
     """Sample function to get a watershed object for a location in NY.
 
     Makes the function call :obj:`dataretrieval.streamstats.get_watershed`
     with the parameters 'NY', -74.524, 43.939, and returns the watershed
@@ -56,18 +57,26 @@
         Custom object that contains the watershed information as extracted
         from the streamstats JSON object.
 
     """
     return get_watershed('NY', -74.524, 43.939)
 
 
-def get_watershed(rcode, xlocation, ylocation, crs=4326,
-                  includeparameters=True, includeflowtypes=False,
-                  includefeatures=True, simplify=True, format='geojson'):
-    """ Get watershed object based on location
+def get_watershed(
+    rcode,
+    xlocation,
+    ylocation,
+    crs=4326,
+    includeparameters=True,
+    includeflowtypes=False,
+    includefeatures=True,
+    simplify=True,
+    format='geojson',
+):
+    """Get watershed object based on location
 
     **Streamstats documentation:**
     Returns a watershed object. The request configuration will determine the
     overall request response. However all returns will return a watershed
     object with at least the workspaceid. The workspace id is the id to the
     service workspace where files are stored and can be used for further
     processing such as for downloads and flow statistic computations.
@@ -100,18 +109,24 @@
     Returns
     -------
     Watershed: :obj:`dataretrieval.streamstats.Watershed`
         Custom object that contains the watershed information as extracted
         from the streamstats JSON object.
 
     """
-    payload = {'rcode': rcode, 'xlocation': xlocation, 'ylocation': ylocation,
-               'crs': crs, 'includeparameters': includeparameters,
-               'includeflowtypes': includeflowtypes,
-               'includefeatures': includefeatures, 'simplify': simplify}
+    payload = {
+        'rcode': rcode,
+        'xlocation': xlocation,
+        'ylocation': ylocation,
+        'crs': crs,
+        'includeparameters': includeparameters,
+        'includeflowtypes': includeflowtypes,
+        'includefeatures': includefeatures,
+        'simplify': simplify,
+    }
     url = 'https://streamstats.usgs.gov/streamstatsservices/watershed.geojson'
 
     r = requests.get(url, params=payload)
 
     r.raise_for_status()
 
     if format == 'geojson':
@@ -127,14 +142,15 @@
 
     data = json.loads(r.text)
     return Watershed.from_streamstats_json(data)
 
 
 class Watershed:
     """Class to extract information from the streamstats JSON object."""
+
     @classmethod
     def from_streamstats_json(cls, streamstats_json):
         """Method that creates a Watershed object from a streamstats JSON."""
         cls.watershed_point = streamstats_json['featurecollection'][0]['feature']
         cls.watershed_polygon = streamstats_json['featurecollection'][1]['feature']
         cls.parameters = streamstats_json['parameters']
         cls._workspaceID = streamstats_json['workspaceID']
```

### Comparing `dataretrieval-1.0.6/dataretrieval/utils.py` & `dataretrieval-1.0.7/dataretrieval/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 Useful utilities for data munging.
 """
 import warnings
+
 import pandas as pd
 import requests
+
 import dataretrieval
 from dataretrieval.codes import tz
 
+
 def to_str(listlike, delimiter=','):
     """Translates list-like objects into strings.
 
     Parameters
     ----------
     listlike: list-like object
         An object that is a list, or list-like
@@ -70,88 +73,46 @@
     df: ``pandas.DataFrame``
         The data frame with a formatted 'datetime' column
 
     """
     # create a datetime index from the columns in qwdata response
     df[tz_field] = df[tz_field].map(tz)
 
-    df['datetime'] = pd.to_datetime(df[date_field] + ' ' +
-                                    df[time_field] + ' ' +
-                                    df[tz_field],
-                                    format='ISO8601',
-                                    utc=True)
+    df['datetime'] = pd.to_datetime(
+        df[date_field] + ' ' + df[time_field] + ' ' + df[tz_field],
+        format='ISO8601',
+        utc=True,
+    )
 
     # if there are any incomplete dates, warn the user
-    if any(pd.isna(df['datetime'])):
-        count = sum(pd.isna(df['datetime']) == True)
+    if df['datetime'].isna().any():
+        count = df['datetime'].isna().sum()
         warnings.warn(
-            f'Warning: {count} incomplete dates found, ' +
-            'consider setting datetime_index to False.', UserWarning)
+            f'Warning: {count} incomplete dates found, '
+            + 'consider setting datetime_index to False.',
+            UserWarning,
+        )
 
     return df
 
 
-#This function may be deprecated once pandas.update support joins besides left.
-def update_merge(left, right, na_only=False, on=None, **kwargs):
-    """Performs a combination update and merge.
-
-    Parameters
-    ----------
-    left: ``pandas.DataFrame``
-        Original data
-    right: ``pandas.DataFrame``
-        Updated data
-    na_only: bool
-        If True, only update na values
-
-    Returns
-    -------
-    df: ``pandas.DataFrame``
-        Updated data frame
-
-    .. todo::
-
-        add na_only parameter support
-
-    """
-    #df = left.merge(right, how='outer',
-    #                left_index=True, right_index=True)
-    df = left.merge(right, how='outer', on=on, **kwargs)
-
-
-    # check for column overlap and resolve update
-    for column in df.columns:
-        #if duplicated column, use the value from right
-        if column[-2:] == '_x':
-            name = column[:-2] # find column name
-
-            if na_only:
-                df[name] = df[name+'_x'].fillna(df[name+'_y'])
-
-            else:
-                df[name] = df[name+'_x'].update(df[name+'_y'])
-
-            df.drop([name + '_x', name + '_y'], axis=1, inplace=True)
-
-    return df
-
 class BaseMetadata:
     """Base class for metadata.
-    
+
     Attributes
     ----------
     url : str
         Response url
     query_time: datetme.timedelta
         Response elapsed time
     header: requests.structures.CaseInsensitiveDict
         Response headers
-    
+
     """
-    
+
     def __init__(self, response) -> None:
         """Generates a standard set of metadata informed by the response.
 
         Parameters
         ----------
         response: Response
             Response object from requests module
@@ -164,38 +125,37 @@
         """
 
         # These are built from the API response
         self.url = response.url
         self.query_time = response.elapsed
         self.header = response.headers
         self.comment = None
-        
+
         # # not sure what statistic_info is
         # self.statistic_info = None
-        
+
         # # disclaimer seems to be only part of importWaterML1
         # self.disclaimer = None
-    
+
     # These properties are to be set by `nwis` or `wqp`-specific metadata classes.
     @property
     def site_info(self):
         raise NotImplementedError(
-            "site_info must be implemented by utils.BaseMetadata children"
+            'site_info must be implemented by utils.BaseMetadata children'
         )
-    
+
     @property
     def variable_info(self):
         raise NotImplementedError(
-            "variable_info must be implemented by utils.BaseMetadata children"
+            'variable_info must be implemented by utils.BaseMetadata children'
         )
 
-
     def __repr__(self) -> str:
-        return f"{type(self).__name__}(url={self.url})"
-        
+        return f'{type(self).__name__}(url={self.url})'
+
 
 def query(url, payload, delimiter=',', ssl_check=True):
     """Send a query.
 
     Wrapper for requests.get that handles errors, converts listed
     query parameters to comma separated strings, and returns response.
 
@@ -215,54 +175,59 @@
     -------
     string: query response
         The response from the API query ``requests.get`` function call.
     """
 
     for key, value in payload.items():
         payload[key] = to_str(value, delimiter)
-    #for index in range(len(payload)):
+    # for index in range(len(payload)):
     #    key, value = payload[index]
     #    payload[index] = (key, to_str(value))
 
     # define the user agent for the query
-    user_agent = {
-        'user-agent': f"python-dataretrieval/{dataretrieval.__version__}"}
+    user_agent = {'user-agent': f'python-dataretrieval/{dataretrieval.__version__}'}
 
-    response = requests.get(url, params=payload,
-                            headers=user_agent, verify=ssl_check)
+    response = requests.get(url, params=payload, headers=user_agent, verify=ssl_check)
 
     if response.status_code == 400:
-        raise ValueError("Bad Request, check that your parameters are correct. URL: {}".format(response.url))
+        raise ValueError(
+            f'Bad Request, check that your parameters are correct. URL: {response.url}'
+        )
     elif response.status_code == 404:
         raise ValueError(
-            "Page Not Found Error. May be the result of an empty query. " +
-            f"URL: {response.url}")
+            'Page Not Found Error. May be the result of an empty query. '
+            + f'URL: {response.url}'
+        )
     elif response.status_code == 414:
         _reason = response.reason
         _example = """
-                    split_list = np.array_split(site_list, n)  # n is number of chunks to divide query into \n
+                    # n is the number of chunks to divide the query into \n
+                    split_list = np.array_split(site_list, n)
                     data_list = []  # list to store chunk results in \n
                     # loop through chunks and make requests \n
                     for site_list in split_list: \n
-                        data = nwis.get_record(sites=site_list, service='dv', start=start, end=end) \n
+                        data = nwis.get_record(sites=site_list, service='dv', \n
+                                               start=start, end=end) \n
                         data_list.append(data)  # append results to list"""
         raise ValueError(
-            "Request URL too long. Modify your query to use fewer sites. " +
-            f"API response reason: {_reason}. Pseudo-code example of how to " +
-            f"split your query: \n {_example}"
-            )
+            'Request URL too long. Modify your query to use fewer sites. '
+            + f'API response reason: {_reason}. Pseudo-code example of how to '
+            + f'split your query: \n {_example}'
+        )
 
     if response.text.startswith('No sites/data'):
         raise NoSitesError(response.url)
 
     return response
 
 
 class NoSitesError(Exception):
-    """Custom error class used when selection criteria returns no sites/data.
-    """
+    """Custom error class used when selection criteria returns no sites/data."""
+
     def __init__(self, url):
         self.url = url
 
     def __str__(self):
-        return "No sites/data found using the selection criteria specified in url: {}".format(self.url)
-
+        return (
+            'No sites/data found using the selection criteria specified in url: '
+            '{url}'
+        ).format(url=self.url)
```

### Comparing `dataretrieval-1.0.6/dataretrieval/waterwatch.py` & `dataretrieval-1.0.7/dataretrieval/waterwatch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from typing import Dict, List, Union
 
-import requests
 import pandas as pd
+import requests
 
-ResponseFormat = "json"  # json, xml
+ResponseFormat = 'json'  # json, xml
 
 # WaterWatch won't receive any new features but it will continue to operate.
-waterwatch_url = "https://waterwatch.usgs.gov/webservices/"
+waterwatch_url = 'https://waterwatch.usgs.gov/webservices/'
 
 
 def _read_json(data: Dict) -> pd.DataFrame:
     return pd.DataFrame(data).T
 
-def get_flood_stage(sites: List[str] = None, fmt: str= "DF") -> Union[pd.DataFrame, Dict]:
+
+def get_flood_stage(
+    sites: List[str] = None, fmt: str = 'DF'
+) -> Union[pd.DataFrame, Dict]:
     """
     Retrieves flood stages for a list of station numbers.
 
     Parameters
     ----------
     sites: List of strings
         Site numbers
@@ -33,39 +36,45 @@
     Examples
     --------
     .. doctest::
 
         >> stations = ["07144100", "07144101"]
         >> res = get_flood_stage(stations, fmt="dict")  # dictionary output
         >> print(res)
-        {'07144100': {'action_stage': '20', 'flood_stage': '22', 'moderate_flood_stage': '25', 'major_flood_stage': '26'},
+        {'07144100': {'action_stage': '20',
+                      'flood_stage': '22',
+                      'moderate_flood_stage': '25',
+                      'major_flood_stage': '26'},
          '07144101': None}
         >> print(get_flood_stage(stations))
         >> print(res)
                 action_stage flood_stage moderate_flood_stage major_flood_stage
         07144100           20          22                   25                26
         07144101         None        None                 None              None
         50057000           16          20                   24                30
 
     """
-    res = requests.get(waterwatch_url + 'floodstage', params={"format": ResponseFormat})
+    res = requests.get(waterwatch_url + 'floodstage', params={'format': ResponseFormat})
 
     if res.ok:
         json_res = res.json()
-        stages = {site['site_no']: {k: v for k, v in site.items() if k != 'site_no'} for site in json_res['sites']}
+        stages = {
+            site['site_no']: {k: v for k, v in site.items() if k != 'site_no'}
+            for site in json_res['sites']
+        }
     else:
-        raise requests.RequestException(f"[{res.status_code}] - {res.reason}")
+        raise requests.RequestException(f'[{res.status_code}] - {res.reason}')
 
     if not sites:
         stations_stages = stages
     else:
         stations_stages = {}
         for site in sites:
             try:
                 stations_stages[site] = stages[site]
             except KeyError:
                 stations_stages[site] = None
 
-    if fmt == "dict":
+    if fmt == 'dict':
         return stations_stages
     else:
         return _read_json(stations_stages)
```

### Comparing `dataretrieval-1.0.6/dataretrieval/wqp.py` & `dataretrieval-1.0.7/dataretrieval/wqp.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 See https://waterqualitydata.us/webservices_documentation for API reference
 
 .. todo::
 
     - implement other services like Organization, Activity, etc.
 
 """
-import pandas as pd
-from io import StringIO
-from .utils import query, BaseMetadata
 import warnings
+from io import StringIO
+
+import pandas as pd
+
+from .utils import BaseMetadata, query
 
 
 def get_results(ssl_check=True, **kwargs):
     """Query the WQP for results.
 
     Parameters
     ----------
@@ -69,24 +71,25 @@
 
     Examples
     --------
     .. code::
 
         >>> # Get results within a radial distance of a point
         >>> df, md = dataretrieval.wqp.get_results(
-        ...     lat='44.2', long='-88.9', within='0.5')
+        ...     lat='44.2', long='-88.9', within='0.5'
+        ... )
 
         >>> # Get results within a bounding box
-        >>> df, md = dataretrieval.wqp.get_results(
-        ...     bBox='-92.8,44.2,-88.9,46.0')
+        >>> df, md = dataretrieval.wqp.get_results(bBox='-92.8,44.2,-88.9,46.0')
 
     """
+    _warn_v3_profiles_outage()
+
     kwargs = _alter_kwargs(kwargs)
-    response = query(wqp_url('Result'), kwargs, delimiter=';',
-                     ssl_check=ssl_check)
+    response = query(wqp_url('Result'), kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
     return df, WQP_Metadata(response)
 
 
 def what_sites(ssl_check=True, **kwargs):
     """Search WQP for sites within a region with specific data.
@@ -108,17 +111,20 @@
 
     Examples
     --------
     .. code::
 
         >>> # Get sites within a radial distance of a point
         >>> df, md = dataretrieval.wqp.what_sites(
-        ...     lat='44.2', long='-88.9', within='2.5')
+        ...     lat='44.2', long='-88.9', within='2.5'
+        ... )
 
     """
+    _warn_v3_profiles_outage()
+
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('Station')
     response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
@@ -147,14 +153,16 @@
     --------
     .. code::
 
         >>> # Get all organizations in the WQP
         >>> df, md = dataretrieval.wqp.what_organizations()
 
     """
+    _warn_v3_profiles_outage()
+
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('Organization')
     response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
@@ -183,14 +191,16 @@
     --------
     .. code::
 
         >>> # Get projects within a HUC region
         >>> df, md = dataretrieval.wqp.what_projects(huc='19')
 
     """
+    _warn_v3_profiles_outage()
+
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('Project')
     response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
@@ -218,18 +228,20 @@
     Examples
     --------
     .. code::
 
         >>> # Get activities within Washington D.C.
         >>> # during a specific time period
         >>> df, md = dataretrieval.wqp.what_activities(
-        ...     statecode='US:11', startDateLo='12-30-2019',
-        ...     startDateHi='01-01-2020')
+        ...     statecode='US:11', startDateLo='12-30-2019', startDateHi='01-01-2020'
+        ... )
 
     """
+    _warn_v3_profiles_outage()
+
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('Activity')
     response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
@@ -258,18 +270,23 @@
     Examples
     --------
     .. code::
 
         >>> # Get detection limits for Nitrite measurements in Rhode Island
         >>> # between specific dates
         >>> df, md = dataretrieval.wqp.what_detection_limits(
-        ...     statecode='US:44', characteristicName='Nitrite',
-        ...     startDateLo='01-01-2021', startDateHi='02-20-2021')
+        ...     statecode='US:44',
+        ...     characteristicName='Nitrite',
+        ...     startDateLo='01-01-2021',
+        ...     startDateHi='02-20-2021',
+        ... )
 
     """
+    _warn_v3_profiles_outage()
+
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('ResultDetectionQuantitationLimit')
     response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
@@ -295,18 +312,19 @@
         Custom metadata object pertaining to the query.
 
     Examples
     --------
     .. code::
 
         >>> # Get habitat metrics for a state (Rhode Island in this case)
-        >>> df, md = dataretrieval.wqp.what_habitat_metrics(
-        ...     statecode='US:44')
+        >>> df, md = dataretrieval.wqp.what_habitat_metrics(statecode='US:44')
 
     """
+    _warn_v3_profiles_outage()
+
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('BiologicalMetric')
     response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
@@ -334,18 +352,20 @@
     Examples
     --------
     .. code::
 
         >>> # Get project weights for a state (North Dakota in this case)
         >>> # within a set time period
         >>> df, md = dataretrieval.wqp.what_project_weights(
-        ...     statecode='US:38', startDateLo='01-01-2006',
-        ...     startDateHi='01-01-2009')
+        ...     statecode='US:38', startDateLo='01-01-2006', startDateHi='01-01-2009'
+        ... )
 
     """
+    _warn_v3_profiles_outage()
+
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('ProjectMonitoringLocationWeighting')
     response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
@@ -373,38 +393,39 @@
     Examples
     --------
     .. code::
 
         >>> # Get activity metrics for a state (North Dakota in this case)
         >>> # within a set time period
         >>> df, md = dataretrieval.wqp.what_activity_metrics(
-        ...     statecode='US:38', startDateLo='07-01-2006',
-        ...     startDateHi='12-01-2006')
+        ...     statecode='US:38', startDateLo='07-01-2006', startDateHi='12-01-2006'
+        ... )
 
     """
+    _warn_v3_profiles_outage()
+
     kwargs = _alter_kwargs(kwargs)
 
     url = wqp_url('ActivityMetric')
     response = query(url, payload=kwargs, delimiter=';', ssl_check=ssl_check)
 
     df = pd.read_csv(StringIO(response.text), delimiter=',')
 
     return df, WQP_Metadata(response)
 
 
 def wqp_url(service):
-    """Construct the WQP URL for a given service.
-    """
+    """Construct the WQP URL for a given service."""
     base_url = 'https://www.waterqualitydata.us/data/'
-    return '{}{}/Search?'.format(base_url, service)
+    return f'{base_url}{service}/Search?'
 
 
 class WQP_Metadata(BaseMetadata):
     """Metadata class for WQP service, derived from BaseMetadata.
-    
+
     Attributes
     ----------
     url : str
         Response url
     query_time: datetme.timedelta
         Response elapsed time
     header: requests.structures.CaseInsensitiveDict
@@ -414,30 +435,30 @@
     site_info: tuple[pd.DataFrame, NWIS_Metadata] | None
         Site information if the query included `sites`, `site` or `site_no`.
     """
 
     def __init__(self, response, **parameters) -> None:
         """Generates a standard set of metadata informed by the response with specific
         metadata for WQP data.
-        
+
         Parameters
         ----------
         response: Response
             Response object from requests module
-        
+
         parameters: unpacked dictionary
             Unpacked dictionary of the parameters supplied in the request
 
         Returns
         -------
         md: :obj:`dataretrieval.wqp.WQP_Metadata`
             A ``dataretrieval`` custom :obj:`dataretrieval.wqp.WQP_Metadata` object.
 
         """
-        
+
         super().__init__(response)
 
         self._parameters = parameters
 
         @property
         def site_info(self):
             if 'sites' in self._parameters:
@@ -461,7 +482,21 @@
     kwargs['zip'] = 'no'
 
     if kwargs.get('mimeType', 'csv') == 'geojson':
         warnings.warn('GeoJSON not yet supported, mimeType set to csv.')
     kwargs['mimeType'] = 'csv'
 
     return kwargs
+
+def _warn_v3_profiles_outage():
+    """Private function for warning message about WQX 3.0 profiles
+    """
+
+    warnings.warn(('USGS discrete water quality data availability '
+                   'and format are changing. Beginning in March 2024 '
+                   'the data obtained from legacy profiles will not '
+                   'include new USGS data or recent updates to existing '
+                   'data. To view the status of changes in data '
+                   'availability and code functionality, visit: '
+                   'https://doi-usgs.github.io/dataRetrieval/articles/Status.html. '
+                   'If you have additional questions about these changes, '
+                   'email CompTools@usgs.gov.'))
```

### Comparing `dataretrieval-1.0.6/dataretrieval.egg-info/PKG-INFO` & `dataretrieval-1.0.7/dataretrieval.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dataretrieval
-Version: 1.0.6
+Version: 1.0.7
 Summary: Discover and retrieve water data from U.S. federal hydrologic web services.
-Maintainer-email: Timothy Hodson <thodson@usgs.gov>, Jayaram Hariharan <jhariharan@usgs.gov>
+Maintainer-email: Timothy Hodson <thodson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United
         States because it contains materials that originally came from the United
         States Geological Survey, an agency of the United States Department of
         Interior. For more information, see the official USGS copyright policy at
@@ -55,23 +55,34 @@
 Project-URL: repository, https://github.com/DOI-USGS/dataretrieval-python.git
 Keywords: USGS,water data
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests
-Requires-Dist: pandas
+Requires-Dist: pandas==2.*
 Provides-Extra: test
 Requires-Dist: pytest>5.0.0; extra == "test"
 Requires-Dist: pytest-cov[all]; extra == "test"
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: requests-mock; extra == "test"
+Requires-Dist: flake8; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx_rtd_theme; extra == "doc"
+Requires-Dist: nbsphinx; extra == "doc"
+Requires-Dist: nbsphinx_link; extra == "doc"
+Provides-Extra: nldi
+Requires-Dist: geopandas>=0.10; extra == "nldi"
 
 # dataretrieval: Download hydrologic data
 
+:warning: USGS data availability and format are changing on Water Quality Portal (WQP). Beginning in February 2024 data obtained from WQP legacy profiles will not include new USGS data or recent updates to existing data. 
+To view the status of changes in data availability and code functionality, visit: https://doi-usgs.github.io/dataRetrieval/articles/Status.html
+
 ## What is dataretrieval?
 `dataretrieval` was created to simplify the process of loading hydrologic data into the Python environment.
 Like the original R version [`dataRetrieval`](https://github.com/DOI-USGS/dataRetrieval),
 it is designed to retrieve the major data types of U.S. Geological Survey (USGS) hydrology
 data that are available on the Web, as well as data from the Water
 Quality Portal (WQP), which currently houses water quality data from the
 Environmental Protection Agency (EPA), U.S. Department of Agriculture
```

### Comparing `dataretrieval-1.0.6/dataretrieval.egg-info/SOURCES.txt` & `dataretrieval-1.0.7/dataretrieval.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+.flake8
 .gitignore
+.pre-commit-config.yaml
+.prettierrc.toml
 CONTRIBUTING.md
 DISCLAIMER.md
 LICENSE.md
 README.md
 code.json
 pyproject.toml
 requirements-dev.txt
-requirements.txt
 setup.py
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
 .github/workflows/sphinx-docs.yml
 .gitlab/issue_templates/reviewer_checklist.md
 .gitlab/merge_request_templates/reviewer_checklist.md
 dataretrieval/__init__.py
 dataretrieval/_version.py
 dataretrieval/nadp.py
+dataretrieval/nldi.py
 dataretrieval/nwis.py
 dataretrieval/streamstats.py
 dataretrieval/utils.py
 dataretrieval/waterwatch.py
 dataretrieval/wqp.py
 dataretrieval.egg-info/PKG-INFO
 dataretrieval.egg-info/SOURCES.txt
@@ -77,18 +80,26 @@
 docs/source/reference/waterwatch.rst
 docs/source/reference/wqp.rst
 docs/source/userguide/dataportals.rst
 docs/source/userguide/index.rst
 docs/source/userguide/timeconventions.rst
 tests/__init__.py
 tests/nadp_test.py
+tests/nldi_test.py
 tests/nwis_test.py
 tests/utils_test.py
 tests/waterservices_test.py
 tests/wqp_test.py
+tests/data/nldi_get_basin.json
+tests/data/nldi_get_features_by_comid.json
+tests/data/nldi_get_features_by_feature_source_with_nav_mode.json
+tests/data/nldi_get_features_by_feature_source_without_nav_mode.json
+tests/data/nldi_get_features_by_lat_long.json
+tests/data/nldi_get_flowlines.json
+tests/data/nldi_get_flowlines_by_comid.json
 tests/data/nwis_sites.txt
 tests/data/water_use_allegheny.txt
 tests/data/water_use_national.txt
 tests/data/waterdata_measurements.txt
 tests/data/waterdata_pmcodes.txt
 tests/data/waterdata_qwdata.txt
 tests/data/waterservices_dv.txt
```

### Comparing `dataretrieval-1.0.6/demos/NWIS_demo_1.ipynb` & `dataretrieval-1.0.7/demos/NWIS_demo_1.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/demos/R Python Vignette equivalents.ipynb` & `dataretrieval-1.0.7/demos/R Python Vignette equivalents.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/demos/datasets/peak_discharge_trends.csv` & `dataretrieval-1.0.7/demos/datasets/peak_discharge_trends.csv`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb` & `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb` & `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb` & `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb` & `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb` & `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb` & `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb` & `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb`

 * *Files 2% similar despite different names*

```diff
@@ -331,305 +331,305 @@
 000014a0: 6527 7320 6461 696c 7920 6d65 616e 2073  e's daily mean s
 000014b0: 7472 6561 6d66 6c6f 772e 5c6e 222c 0a20  treamflow.\n",. 
 000014c0: 2020 2022 5c6e 222c 0a20 2020 2022 466f     "\n",.    "Fo
 000014d0: 7220 6164 6469 7469 6f6e 616c 2070 6172  r additional par
 000014e0: 616d 6574 6572 206f 7074 696f 6e73 2073  ameter options s
 000014f0: 6565 2068 7474 7073 3a2f 2f77 6174 6572  ee https://water
 00001500: 7365 7276 6963 6573 2e75 7367 732e 676f  services.usgs.go
-00001510: 762f 7265 7374 2f53 6974 652d 5365 7276  v/rest/Site-Serv
-00001520: 6963 652e 6874 6d6c 2373 7461 7465 4364  ice.html#stateCd
-00001530: 220a 2020 205d 0a20 207d 2c0a 2020 7b0a  ".   ].  },.  {.
-00001540: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
-00001550: 226d 6172 6b64 6f77 6e22 2c0a 2020 2022  "markdown",.   "
-00001560: 6d65 7461 6461 7461 223a 207b 7d2c 0a20  metadata": {},. 
-00001570: 2020 2273 6f75 7263 6522 3a20 5b0a 2020    "source": [.  
-00001580: 2020 2223 2323 2045 7861 6d70 6c65 2031    "### Example 1
-00001590: 3a20 4765 7420 7369 7465 2069 6e66 6f72  : Get site infor
-000015a0: 6d61 7469 6f6e 2066 6f72 2061 2055 5347  mation for a USG
-000015b0: 5320 4e57 4953 206d 6f6e 6974 6f72 696e  S NWIS monitorin
-000015c0: 6720 7369 7465 220a 2020 205d 0a20 207d  g site".   ].  }
-000015d0: 2c0a 2020 7b0a 2020 2022 6365 6c6c 5f74  ,.  {.   "cell_t
-000015e0: 7970 6522 3a20 2263 6f64 6522 2c0a 2020  ype": "code",.  
-000015f0: 2022 6578 6563 7574 696f 6e5f 636f 756e   "execution_coun
-00001600: 7422 3a20 6e75 6c6c 2c0a 2020 2022 6d65  t": null,.   "me
-00001610: 7461 6461 7461 223a 207b 0a20 2020 2022  tadata": {.    "
-00001620: 636f 6c6c 6170 7365 6422 3a20 6661 6c73  collapsed": fals
-00001630: 652c 0a20 2020 2022 6a75 7079 7465 7222  e,.    "jupyter"
-00001640: 3a20 7b0a 2020 2020 2022 6f75 7470 7574  : {.     "output
-00001650: 735f 6869 6464 656e 223a 2066 616c 7365  s_hidden": false
-00001660: 0a20 2020 207d 2c0a 2020 2020 2270 7963  .    },.    "pyc
-00001670: 6861 726d 223a 207b 0a20 2020 2020 226e  harm": {.     "n
-00001680: 616d 6522 3a20 2223 2525 5c6e 220a 2020  ame": "#%%\n".  
-00001690: 2020 7d0a 2020 207d 2c0a 2020 2022 6f75    }.   },.   "ou
-000016a0: 7470 7574 7322 3a20 5b5d 2c0a 2020 2022  tputs": [],.   "
-000016b0: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
-000016c0: 2320 5370 6563 6966 7920 7468 6520 7369  # Specify the si
-000016d0: 7465 2079 6f75 2077 616e 7420 746f 2072  te you want to r
-000016e0: 6574 7269 6576 6520 696e 666f 726d 6174  etrieve informat
-000016f0: 696f 6e20 666f 725c 6e22 2c0a 2020 2020  ion for\n",.    
-00001700: 2273 6974 6549 4420 3d20 5c22 3130 3130  "siteID = \"1010
-00001710: 3930 3030 5c22 5c6e 222c 0a20 2020 2022  9000\"\n",.    "
-00001720: 5c6e 222c 0a20 2020 2022 2320 4765 7420  \n",.    "# Get 
-00001730: 7468 6520 7369 7465 2069 6e66 6f72 6d61  the site informa
-00001740: 7469 6f6e 5c6e 222c 0a20 2020 2022 7369  tion\n",.    "si
-00001750: 7465 494e 464f 203d 206e 7769 732e 6765  teINFO = nwis.ge
-00001760: 745f 696e 666f 2873 6974 6573 3d73 6974  t_info(sites=sit
-00001770: 6549 4429 220a 2020 205d 0a20 207d 2c0a  eID)".   ].  },.
-00001780: 2020 7b0a 2020 2022 6365 6c6c 5f74 7970    {.   "cell_typ
-00001790: 6522 3a20 226d 6172 6b64 6f77 6e22 2c0a  e": "markdown",.
-000017a0: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-000017b0: 7d2c 0a20 2020 2273 6f75 7263 6522 3a20  },.   "source": 
-000017c0: 5b0a 2020 2020 2223 2323 2049 6e74 6572  [.    "### Inter
-000017d0: 7072 6574 696e 6720 7468 6520 5265 7375  preting the Resu
-000017e0: 6c74 5c6e 222c 0a20 2020 2022 5c6e 222c  lt\n",.    "\n",
-000017f0: 0a20 2020 2022 5468 6520 7265 7375 6c74  .    "The result
-00001800: 206f 6620 6361 6c6c 696e 6720 7468 6520   of calling the 
-00001810: 6067 6574 5f69 6e66 6f28 2960 2066 756e  `get_info()` fun
-00001820: 6374 696f 6e20 6973 2061 6e20 6f62 6a65  ction is an obje
-00001830: 6374 2074 6861 7420 636f 6e74 6169 6e73  ct that contains
-00001840: 2061 2050 616e 6461 7320 6461 7461 2066   a Pandas data f
-00001850: 7261 6d65 206f 626a 6563 7420 616e 6420  rame object and 
-00001860: 616e 2061 7373 6f63 6961 7465 6420 6d65  an associated me
-00001870: 7461 6461 7461 206f 626a 6563 742e 2054  tadata object. T
-00001880: 6865 2050 616e 6461 7320 6461 7461 2066  he Pandas data f
-00001890: 7261 6d65 2063 6f6e 7461 696e 7320 7468  rame contains th
-000018a0: 6520 7369 7465 2069 6e66 6f72 6d61 7469  e site informati
-000018b0: 6f6e 2066 6f72 2074 6865 2072 6571 7565  on for the reque
-000018c0: 7374 6564 2073 6974 652e 5c6e 222c 0a20  sted site.\n",. 
-000018d0: 2020 2022 5c6e 222c 0a20 2020 2022 4f6e     "\n",.    "On
-000018e0: 6365 2079 6f75 2776 6520 676f 7420 7468  ce you've got th
-000018f0: 6520 6461 7461 2066 7261 6d65 2c20 7468  e data frame, th
-00001900: 6572 6527 7320 7365 7665 7261 6c20 7573  ere's several us
-00001910: 6566 756c 2074 6869 6e67 7320 796f 7520  eful things you 
-00001920: 6361 6e20 646f 2074 6f20 6578 706c 6f72  can do to explor
-00001930: 6520 7468 6520 696e 666f 726d 6174 696f  e the informatio
-00001940: 6e20 6162 6f75 7420 7468 6520 7369 7465  n about the site
-00001950: 2e22 0a20 2020 5d0a 2020 7d2c 0a20 207b  .".   ].  },.  {
-00001960: 0a20 2020 2263 656c 6c5f 7479 7065 223a  .   "cell_type":
-00001970: 2022 636f 6465 222c 0a20 2020 2265 7865   "code",.   "exe
-00001980: 6375 7469 6f6e 5f63 6f75 6e74 223a 206e  cution_count": n
-00001990: 756c 6c2c 0a20 2020 226d 6574 6164 6174  ull,.   "metadat
-000019a0: 6122 3a20 7b0a 2020 2020 2263 6f6c 6c61  a": {.    "colla
-000019b0: 7073 6564 223a 2066 616c 7365 2c0a 2020  psed": false,.  
-000019c0: 2020 226a 7570 7974 6572 223a 207b 0a20    "jupyter": {. 
-000019d0: 2020 2020 226f 7574 7075 7473 5f68 6964      "outputs_hid
-000019e0: 6465 6e22 3a20 6661 6c73 650a 2020 2020  den": false.    
-000019f0: 7d2c 0a20 2020 2022 7079 6368 6172 6d22  },.    "pycharm"
-00001a00: 3a20 7b0a 2020 2020 2022 6e61 6d65 223a  : {.     "name":
-00001a10: 2022 2325 255c 6e22 0a20 2020 207d 0a20   "#%%\n".    }. 
-00001a20: 2020 7d2c 0a20 2020 226f 7574 7075 7473    },.   "outputs
-00001a30: 223a 205b 5d2c 0a20 2020 2273 6f75 7263  ": [],.   "sourc
-00001a40: 6522 3a20 5b0a 2020 2020 2223 2044 6973  e": [.    "# Dis
-00001a50: 706c 6179 2074 6865 2064 6174 6120 6672  play the data fr
-00001a60: 616d 6520 6173 2061 2074 6162 6c65 5c6e  ame as a table\n
-00001a70: 222c 0a20 2020 2022 6469 7370 6c61 7928  ",.    "display(
-00001a80: 7369 7465 494e 464f 5b30 5d29 220a 2020  siteINFO[0])".  
-00001a90: 205d 0a20 207d 2c0a 2020 7b0a 2020 2022   ].  },.  {.   "
-00001aa0: 6365 6c6c 5f74 7970 6522 3a20 226d 6172  cell_type": "mar
-00001ab0: 6b64 6f77 6e22 2c0a 2020 2022 6d65 7461  kdown",.   "meta
-00001ac0: 6461 7461 223a 207b 7d2c 0a20 2020 2273  data": {},.   "s
-00001ad0: 6f75 7263 6522 3a20 5b0a 2020 2020 2253  ource": [.    "S
-00001ae0: 686f 7720 7468 6520 6461 7461 2074 7970  how the data typ
-00001af0: 6573 206f 6620 7468 6520 636f 6c75 6d6e  es of the column
-00001b00: 7320 696e 2074 6865 2072 6573 756c 7469  s in the resulti
-00001b10: 6e67 2064 6174 6120 6672 616d 652e 220a  ng data frame.".
-00001b20: 2020 205d 0a20 207d 2c0a 2020 7b0a 2020     ].  },.  {.  
-00001b30: 2022 6365 6c6c 5f74 7970 6522 3a20 2263   "cell_type": "c
-00001b40: 6f64 6522 2c0a 2020 2022 6578 6563 7574  ode",.   "execut
-00001b50: 696f 6e5f 636f 756e 7422 3a20 6e75 6c6c  ion_count": null
-00001b60: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
-00001b70: 207b 0a20 2020 2022 636f 6c6c 6170 7365   {.    "collapse
-00001b80: 6422 3a20 6661 6c73 652c 0a20 2020 2022  d": false,.    "
-00001b90: 6a75 7079 7465 7222 3a20 7b0a 2020 2020  jupyter": {.    
-00001ba0: 2022 6f75 7470 7574 735f 6869 6464 656e   "outputs_hidden
-00001bb0: 223a 2066 616c 7365 0a20 2020 207d 2c0a  ": false.    },.
-00001bc0: 2020 2020 2270 7963 6861 726d 223a 207b      "pycharm": {
-00001bd0: 0a20 2020 2020 226e 616d 6522 3a20 2223  .     "name": "#
-00001be0: 2525 5c6e 220a 2020 2020 7d0a 2020 207d  %%\n".    }.   }
-00001bf0: 2c0a 2020 2022 6f75 7470 7574 7322 3a20  ,.   "outputs": 
-00001c00: 5b5d 2c0a 2020 2022 736f 7572 6365 223a  [],.   "source":
-00001c10: 205b 0a20 2020 2022 7072 696e 7428 7369   [.    "print(si
-00001c20: 7465 494e 464f 5b30 5d2e 6474 7970 6573  teINFO[0].dtypes
-00001c30: 2922 0a20 2020 5d0a 2020 7d2c 0a20 207b  )".   ].  },.  {
-00001c40: 0a20 2020 2263 656c 6c5f 7479 7065 223a  .   "cell_type":
-00001c50: 2022 6d61 726b 646f 776e 222c 0a20 2020   "markdown",.   
-00001c60: 226d 6574 6164 6174 6122 3a20 7b7d 2c0a  "metadata": {},.
-00001c70: 2020 2022 736f 7572 6365 223a 205b 0a20     "source": [. 
-00001c80: 2020 2022 5468 6520 6f74 6865 7220 7061     "The other pa
-00001c90: 7274 206f 6620 7468 6520 7265 7375 6c74  rt of the result
-00001ca0: 2072 6574 7572 6e65 6420 6672 6f6d 2074   returned from t
-00001cb0: 6865 2060 6765 745f 696e 666f 2829 6020  he `get_info()` 
-00001cc0: 6675 6e63 7469 6f6e 2069 7320 6120 6d65  function is a me
-00001cd0: 7461 6461 7461 206f 626a 6563 7420 7468  tadata object th
-00001ce0: 6174 2063 6f6e 7461 696e 7320 696e 666f  at contains info
-00001cf0: 726d 6174 696f 6e20 6162 6f75 7420 7468  rmation about th
-00001d00: 6520 7175 6572 7920 7468 6174 2077 6173  e query that was
-00001d10: 2065 7865 6375 7465 6420 746f 2072 6574   executed to ret
-00001d20: 7572 6e20 7468 6520 6461 7461 2e20 466f  urn the data. Fo
-00001d30: 7220 6578 616d 706c 652c 2079 6f75 2063  r example, you c
-00001d40: 616e 2061 6363 6573 7320 7468 6520 5552  an access the UR
-00001d50: 4c20 7468 6174 2077 6173 2061 7373 656d  L that was assem
-00001d60: 626c 6564 2074 6f20 7265 7472 6965 7665  bled to retrieve
-00001d70: 2074 6865 2072 6571 7565 7374 6564 2064   the requested d
-00001d80: 6174 6120 6672 6f6d 2074 6865 2055 5347  ata from the USG
-00001d90: 5320 7765 6220 7365 7276 6963 652e 2054  S web service. T
-00001da0: 6865 2055 5347 5320 7765 6220 7365 7276  he USGS web serv
-00001db0: 6963 6520 7265 7370 6f6e 7365 7320 636f  ice responses co
-00001dc0: 6e74 6169 6e20 6120 6465 7363 7269 7074  ntain a descript
-00001dd0: 6976 6520 6865 6164 6572 2074 6861 7420  ive header that 
-00001de0: 6465 6669 6e65 7320 616e 6420 6361 6e20  defines and can 
-00001df0: 6265 2068 656c 7066 756c 2069 6e20 696e  be helpful in in
-00001e00: 7465 7270 7265 7469 6e67 2074 6865 2063  terpreting the c
-00001e10: 6f6e 7465 6e74 7320 6f66 2074 6865 2072  ontents of the r
-00001e20: 6573 706f 6e73 652e 220a 2020 205d 0a20  esponse.".   ]. 
-00001e30: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
-00001e40: 5f74 7970 6522 3a20 2263 6f64 6522 2c0a  _type": "code",.
-00001e50: 2020 2022 6578 6563 7574 696f 6e5f 636f     "execution_co
-00001e60: 756e 7422 3a20 6e75 6c6c 2c0a 2020 2022  unt": null,.   "
-00001e70: 6d65 7461 6461 7461 223a 207b 0a20 2020  metadata": {.   
-00001e80: 2022 636f 6c6c 6170 7365 6422 3a20 6661   "collapsed": fa
-00001e90: 6c73 652c 0a20 2020 2022 6a75 7079 7465  lse,.    "jupyte
-00001ea0: 7222 3a20 7b0a 2020 2020 2022 6f75 7470  r": {.     "outp
-00001eb0: 7574 735f 6869 6464 656e 223a 2066 616c  uts_hidden": fal
-00001ec0: 7365 0a20 2020 207d 2c0a 2020 2020 2270  se.    },.    "p
-00001ed0: 7963 6861 726d 223a 207b 0a20 2020 2020  ycharm": {.     
-00001ee0: 226e 616d 6522 3a20 2223 2525 5c6e 220a  "name": "#%%\n".
-00001ef0: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
-00001f00: 6f75 7470 7574 7322 3a20 5b5d 2c0a 2020  outputs": [],.  
-00001f10: 2022 736f 7572 6365 223a 205b 0a20 2020   "source": [.   
-00001f20: 2022 7072 696e 7428 5c22 5468 6520 7175   "print(\"The qu
-00001f30: 6572 7920 5552 4c20 7573 6564 2074 6f20  ery URL used to 
-00001f40: 7265 7472 6965 7665 2074 6865 2064 6174  retrieve the dat
-00001f50: 6120 6672 6f6d 204e 5749 5320 7761 733a  a from NWIS was:
-00001f60: 205c 2220 2b20 7369 7465 494e 464f 5b31   \" + siteINFO[1
-00001f70: 5d2e 7572 6c29 220a 2020 205d 0a20 207d  ].url)".   ].  }
-00001f80: 2c0a 2020 7b0a 2020 2022 6365 6c6c 5f74  ,.  {.   "cell_t
-00001f90: 7970 6522 3a20 226d 6172 6b64 6f77 6e22  ype": "markdown"
-00001fa0: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
-00001fb0: 207b 7d2c 0a20 2020 2273 6f75 7263 6522   {},.   "source"
-00001fc0: 3a20 5b0a 2020 2020 2223 2323 2041 6464  : [.    "### Add
-00001fd0: 6974 696f 6e61 6c20 4578 616d 706c 6573  itional Examples
-00001fe0: 5c6e 222c 0a20 2020 2022 5c6e 222c 0a20  \n",.    "\n",. 
-00001ff0: 2020 2022 2323 2323 2045 7861 6d70 6c65     "#### Example
-00002000: 2032 3a20 4765 7420 7369 7465 2069 6e66   2: Get site inf
-00002010: 6f72 6d61 7469 6f6e 2066 6f72 206d 756c  ormation for mul
-00002020: 7469 706c 6520 7369 7465 7320 696e 2061  tiple sites in a
-00002030: 206c 6973 7422 0a20 2020 5d0a 2020 7d2c   list".   ].  },
-00002040: 0a20 207b 0a20 2020 2263 656c 6c5f 7479  .  {.   "cell_ty
-00002050: 7065 223a 2022 636f 6465 222c 0a20 2020  pe": "code",.   
-00002060: 2265 7865 6375 7469 6f6e 5f63 6f75 6e74  "execution_count
-00002070: 223a 206e 756c 6c2c 0a20 2020 226d 6574  ": null,.   "met
-00002080: 6164 6174 6122 3a20 7b0a 2020 2020 2263  adata": {.    "c
-00002090: 6f6c 6c61 7073 6564 223a 2066 616c 7365  ollapsed": false
-000020a0: 2c0a 2020 2020 226a 7570 7974 6572 223a  ,.    "jupyter":
-000020b0: 207b 0a20 2020 2020 226f 7574 7075 7473   {.     "outputs
-000020c0: 5f68 6964 6465 6e22 3a20 6661 6c73 650a  _hidden": false.
-000020d0: 2020 2020 7d2c 0a20 2020 2022 7079 6368      },.    "pych
-000020e0: 6172 6d22 3a20 7b0a 2020 2020 2022 6e61  arm": {.     "na
-000020f0: 6d65 223a 2022 2325 255c 6e22 0a20 2020  me": "#%%\n".   
-00002100: 207d 0a20 2020 7d2c 0a20 2020 226f 7574   }.   },.   "out
-00002110: 7075 7473 223a 205b 5d2c 0a20 2020 2273  puts": [],.   "s
-00002120: 6f75 7263 6522 3a20 5b0a 2020 2020 2223  ource": [.    "#
-00002130: 2043 7265 6174 6520 6120 6c69 7374 206f   Create a list o
-00002140: 6620 7468 6520 7369 7465 2069 6465 6e74  f the site ident
-00002150: 6966 6965 7273 2079 6f75 2077 616e 7420  ifiers you want 
-00002160: 746f 2072 6574 7269 6576 6520 696e 666f  to retrieve info
-00002170: 726d 6174 696f 6e20 666f 725c 6e22 2c0a  rmation for\n",.
-00002180: 2020 2020 2273 6974 6549 4473 203d 205b      "siteIDs = [
-00002190: 5c22 3035 3131 3430 3030 5c22 2c20 5c22  \"05114000\", \"
-000021a0: 3039 3432 3333 3530 5c22 5d5c 6e22 2c0a  09423350\"]\n",.
-000021b0: 2020 2020 225c 6e22 2c0a 2020 2020 2223      "\n",.    "#
-000021c0: 2047 6574 2074 6865 2073 6974 6520 696e   Get the site in
-000021d0: 666f 726d 6174 696f 6e5c 6e22 2c0a 2020  formation\n",.  
-000021e0: 2020 2273 6974 6549 4e46 4f5f 6d75 6c74    "siteINFO_mult
-000021f0: 6920 3d20 6e77 6973 2e67 6574 5f69 6e66  i = nwis.get_inf
-00002200: 6f28 7369 7465 733d 7369 7465 4944 7329  o(sites=siteIDs)
-00002210: 5c6e 222c 0a20 2020 2022 6469 7370 6c61  \n",.    "displa
-00002220: 7928 7369 7465 494e 464f 5f6d 756c 7469  y(siteINFO_multi
-00002230: 5b30 5d29 220a 2020 205d 0a20 207d 2c0a  [0])".   ].  },.
-00002240: 2020 7b0a 2020 2022 6365 6c6c 5f74 7970    {.   "cell_typ
-00002250: 6522 3a20 226d 6172 6b64 6f77 6e22 2c0a  e": "markdown",.
-00002260: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-00002270: 7d2c 0a20 2020 2273 6f75 7263 6522 3a20  },.   "source": 
-00002280: 5b0a 2020 2020 2223 2323 2320 4578 616d  [.    "#### Exam
-00002290: 706c 6520 333a 2047 6574 2073 6974 6520  ple 3: Get site 
-000022a0: 696e 666f 726d 6174 696f 6e20 666f 7220  information for 
-000022b0: 616c 6c20 7369 7465 7320 7769 7468 696e  all sites within
-000022c0: 2061 2073 7461 7465 220a 2020 205d 0a20   a state".   ]. 
-000022d0: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
-000022e0: 5f74 7970 6522 3a20 2263 6f64 6522 2c0a  _type": "code",.
-000022f0: 2020 2022 6578 6563 7574 696f 6e5f 636f     "execution_co
-00002300: 756e 7422 3a20 6e75 6c6c 2c0a 2020 2022  unt": null,.   "
-00002310: 6d65 7461 6461 7461 223a 207b 7d2c 0a20  metadata": {},. 
-00002320: 2020 226f 7574 7075 7473 223a 205b 5d2c    "outputs": [],
-00002330: 0a20 2020 2273 6f75 7263 6522 3a20 5b0a  .   "source": [.
-00002340: 2020 2020 2223 2047 6574 2074 6865 2073      "# Get the s
-00002350: 6974 6520 696e 666f 726d 6174 696f 6e20  ite information 
-00002360: 666f 7220 6120 7374 6174 655c 6e22 2c0a  for a state\n",.
-00002370: 2020 2020 2273 6974 6549 4e46 4f5f 7374      "siteINFO_st
-00002380: 6174 6520 3d20 6e77 6973 2e67 6574 5f69  ate = nwis.get_i
-00002390: 6e66 6f28 7374 6174 6543 643d 2755 5427  nfo(stateCd='UT'
-000023a0: 295c 6e22 2c0a 2020 2020 2264 6973 706c  )\n",.    "displ
-000023b0: 6179 2873 6974 6549 4e46 4f5f 7374 6174  ay(siteINFO_stat
-000023c0: 655b 305d 2922 0a20 2020 5d0a 2020 7d2c  e[0])".   ].  },
-000023d0: 0a20 207b 0a20 2020 2263 656c 6c5f 7479  .  {.   "cell_ty
-000023e0: 7065 223a 2022 6d61 726b 646f 776e 222c  pe": "markdown",
-000023f0: 0a20 2020 226d 6574 6164 6174 6122 3a20  .   "metadata": 
-00002400: 7b7d 2c0a 2020 2022 736f 7572 6365 223a  {},.   "source":
-00002410: 205b 0a20 2020 2022 2323 2323 2045 7861   [.    "#### Exa
-00002420: 6d70 6c65 2034 3a20 4765 7420 7369 7465  mple 4: Get site
-00002430: 2069 6e66 6f72 6d61 7469 6f6e 2066 6f72   information for
-00002440: 2061 6c6c 205c 2273 7472 6561 6d5c 2220   all \"stream\" 
-00002450: 7369 7465 7320 7769 7468 696e 2061 2055  sites within a U
-00002460: 5347 5320 4855 4322 0a20 2020 5d0a 2020  SGS HUC".   ].  
-00002470: 7d2c 0a20 207b 0a20 2020 2263 656c 6c5f  },.  {.   "cell_
-00002480: 7479 7065 223a 2022 636f 6465 222c 0a20  type": "code",. 
-00002490: 2020 2265 7865 6375 7469 6f6e 5f63 6f75    "execution_cou
-000024a0: 6e74 223a 206e 756c 6c2c 0a20 2020 226d  nt": null,.   "m
-000024b0: 6574 6164 6174 6122 3a20 7b7d 2c0a 2020  etadata": {},.  
-000024c0: 2022 6f75 7470 7574 7322 3a20 5b5d 2c0a   "outputs": [],.
-000024d0: 2020 2022 736f 7572 6365 223a 205b 0a20     "source": [. 
-000024e0: 2020 2022 2320 4372 6561 7465 2061 206c     "# Create a l
-000024f0: 6973 7420 6f66 2068 7563 7320 666f 7220  ist of hucs for 
-00002500: 7768 6963 6820 746f 2071 7565 7279 2073  which to query s
-00002510: 6974 6573 5c6e 222c 0a20 2020 2022 6875  ites\n",.    "hu
-00002520: 635f 6c69 7374 203d 205b 2731 3630 3130  c_list = ['16010
-00002530: 3230 3327 5d5c 6e22 2c0a 2020 2020 225c  203']\n",.    "\
-00002540: 6e22 2c0a 2020 2020 2223 2047 6574 2074  n",.    "# Get t
-00002550: 6865 2073 6974 6520 696e 666f 726d 6174  he site informat
-00002560: 696f 6e20 2d20 6c69 6d69 7420 746f 2073  ion - limit to s
-00002570: 7472 6561 6d20 7369 7465 735c 6e22 2c0a  tream sites\n",.
-00002580: 2020 2020 2273 6974 6549 4e46 4f5f 6875      "siteINFO_hu
-00002590: 6320 3d20 6e77 6973 2e67 6574 5f69 6e66  c = nwis.get_inf
-000025a0: 6f28 6875 633d 6875 635f 6c69 7374 2c20  o(huc=huc_list, 
-000025b0: 7369 7465 5479 7065 3d27 5354 2729 5c6e  siteType='ST')\n
-000025c0: 222c 0a20 2020 2022 6469 7370 6c61 7928  ",.    "display(
-000025d0: 7369 7465 494e 464f 5f68 7563 5b30 5d29  siteINFO_huc[0])
-000025e0: 220a 2020 205d 0a20 207d 0a20 5d2c 0a20  ".   ].  }. ],. 
-000025f0: 226d 6574 6164 6174 6122 3a20 7b0a 2020  "metadata": {.  
-00002600: 226b 6572 6e65 6c73 7065 6322 3a20 7b0a  "kernelspec": {.
-00002610: 2020 2022 6469 7370 6c61 795f 6e61 6d65     "display_name
-00002620: 223a 2022 5079 7468 6f6e 2033 2028 6970  ": "Python 3 (ip
-00002630: 796b 6572 6e65 6c29 222c 0a20 2020 226c  ykernel)",.   "l
-00002640: 616e 6775 6167 6522 3a20 2270 7974 686f  anguage": "pytho
-00002650: 6e22 2c0a 2020 2022 6e61 6d65 223a 2022  n",.   "name": "
-00002660: 7079 7468 6f6e 3322 0a20 207d 2c0a 2020  python3".  },.  
-00002670: 226c 616e 6775 6167 655f 696e 666f 223a  "language_info":
-00002680: 207b 0a20 2020 2263 6f64 656d 6972 726f   {.   "codemirro
-00002690: 725f 6d6f 6465 223a 207b 0a20 2020 2022  r_mode": {.    "
-000026a0: 6e61 6d65 223a 2022 6970 7974 686f 6e22  name": "ipython"
-000026b0: 2c0a 2020 2020 2276 6572 7369 6f6e 223a  ,.    "version":
-000026c0: 2033 0a20 2020 7d2c 0a20 2020 2266 696c   3.   },.   "fil
-000026d0: 655f 6578 7465 6e73 696f 6e22 3a20 222e  e_extension": ".
-000026e0: 7079 222c 0a20 2020 226d 696d 6574 7970  py",.   "mimetyp
-000026f0: 6522 3a20 2274 6578 742f 782d 7079 7468  e": "text/x-pyth
-00002700: 6f6e 222c 0a20 2020 226e 616d 6522 3a20  on",.   "name": 
-00002710: 2270 7974 686f 6e22 2c0a 2020 2022 6e62  "python",.   "nb
-00002720: 636f 6e76 6572 745f 6578 706f 7274 6572  convert_exporter
-00002730: 223a 2022 7079 7468 6f6e 222c 0a20 2020  ": "python",.   
-00002740: 2270 7967 6d65 6e74 735f 6c65 7865 7222  "pygments_lexer"
-00002750: 3a20 2269 7079 7468 6f6e 3322 2c0a 2020  : "ipython3",.  
-00002760: 2022 7665 7273 696f 6e22 3a20 2233 2e39   "version": "3.9
-00002770: 2e37 220a 2020 7d0a 207d 2c0a 2022 6e62  .7".  }. },. "nb
-00002780: 666f 726d 6174 223a 2034 2c0a 2022 6e62  format": 4,. "nb
-00002790: 666f 726d 6174 5f6d 696e 6f72 223a 2034  format_minor": 4
-000027a0: 0a7d 0a                                  .}.
+00001510: 762f 646f 6373 2f73 6974 652d 7365 7276  v/docs/site-serv
+00001520: 6963 652f 7369 7465 2d73 6572 7669 6365  ice/site-service
+00001530: 2d64 6574 6169 6c73 2f0a 2020 205d 0a20  -details/.   ]. 
+00001540: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
+00001550: 5f74 7970 6522 3a20 226d 6172 6b64 6f77  _type": "markdow
+00001560: 6e22 2c0a 2020 2022 6d65 7461 6461 7461  n",.   "metadata
+00001570: 223a 207b 7d2c 0a20 2020 2273 6f75 7263  ": {},.   "sourc
+00001580: 6522 3a20 5b0a 2020 2020 2223 2323 2045  e": [.    "### E
+00001590: 7861 6d70 6c65 2031 3a20 4765 7420 7369  xample 1: Get si
+000015a0: 7465 2069 6e66 6f72 6d61 7469 6f6e 2066  te information f
+000015b0: 6f72 2061 2055 5347 5320 4e57 4953 206d  or a USGS NWIS m
+000015c0: 6f6e 6974 6f72 696e 6720 7369 7465 220a  onitoring site".
+000015d0: 2020 205d 0a20 207d 2c0a 2020 7b0a 2020     ].  },.  {.  
+000015e0: 2022 6365 6c6c 5f74 7970 6522 3a20 2263   "cell_type": "c
+000015f0: 6f64 6522 2c0a 2020 2022 6578 6563 7574  ode",.   "execut
+00001600: 696f 6e5f 636f 756e 7422 3a20 6e75 6c6c  ion_count": null
+00001610: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
+00001620: 207b 0a20 2020 2022 636f 6c6c 6170 7365   {.    "collapse
+00001630: 6422 3a20 6661 6c73 652c 0a20 2020 2022  d": false,.    "
+00001640: 6a75 7079 7465 7222 3a20 7b0a 2020 2020  jupyter": {.    
+00001650: 2022 6f75 7470 7574 735f 6869 6464 656e   "outputs_hidden
+00001660: 223a 2066 616c 7365 0a20 2020 207d 2c0a  ": false.    },.
+00001670: 2020 2020 2270 7963 6861 726d 223a 207b      "pycharm": {
+00001680: 0a20 2020 2020 226e 616d 6522 3a20 2223  .     "name": "#
+00001690: 2525 5c6e 220a 2020 2020 7d0a 2020 207d  %%\n".    }.   }
+000016a0: 2c0a 2020 2022 6f75 7470 7574 7322 3a20  ,.   "outputs": 
+000016b0: 5b5d 2c0a 2020 2022 736f 7572 6365 223a  [],.   "source":
+000016c0: 205b 0a20 2020 2022 2320 5370 6563 6966   [.    "# Specif
+000016d0: 7920 7468 6520 7369 7465 2079 6f75 2077  y the site you w
+000016e0: 616e 7420 746f 2072 6574 7269 6576 6520  ant to retrieve 
+000016f0: 696e 666f 726d 6174 696f 6e20 666f 725c  information for\
+00001700: 6e22 2c0a 2020 2020 2273 6974 6549 4420  n",.    "siteID 
+00001710: 3d20 5c22 3130 3130 3930 3030 5c22 5c6e  = \"10109000\"\n
+00001720: 222c 0a20 2020 2022 5c6e 222c 0a20 2020  ",.    "\n",.   
+00001730: 2022 2320 4765 7420 7468 6520 7369 7465   "# Get the site
+00001740: 2069 6e66 6f72 6d61 7469 6f6e 5c6e 222c   information\n",
+00001750: 0a20 2020 2022 7369 7465 494e 464f 203d  .    "siteINFO =
+00001760: 206e 7769 732e 6765 745f 696e 666f 2873   nwis.get_info(s
+00001770: 6974 6573 3d73 6974 6549 4429 220a 2020  ites=siteID)".  
+00001780: 205d 0a20 207d 2c0a 2020 7b0a 2020 2022   ].  },.  {.   "
+00001790: 6365 6c6c 5f74 7970 6522 3a20 226d 6172  cell_type": "mar
+000017a0: 6b64 6f77 6e22 2c0a 2020 2022 6d65 7461  kdown",.   "meta
+000017b0: 6461 7461 223a 207b 7d2c 0a20 2020 2273  data": {},.   "s
+000017c0: 6f75 7263 6522 3a20 5b0a 2020 2020 2223  ource": [.    "#
+000017d0: 2323 2049 6e74 6572 7072 6574 696e 6720  ## Interpreting 
+000017e0: 7468 6520 5265 7375 6c74 5c6e 222c 0a20  the Result\n",. 
+000017f0: 2020 2022 5c6e 222c 0a20 2020 2022 5468     "\n",.    "Th
+00001800: 6520 7265 7375 6c74 206f 6620 6361 6c6c  e result of call
+00001810: 696e 6720 7468 6520 6067 6574 5f69 6e66  ing the `get_inf
+00001820: 6f28 2960 2066 756e 6374 696f 6e20 6973  o()` function is
+00001830: 2061 6e20 6f62 6a65 6374 2074 6861 7420   an object that 
+00001840: 636f 6e74 6169 6e73 2061 2050 616e 6461  contains a Panda
+00001850: 7320 6461 7461 2066 7261 6d65 206f 626a  s data frame obj
+00001860: 6563 7420 616e 6420 616e 2061 7373 6f63  ect and an assoc
+00001870: 6961 7465 6420 6d65 7461 6461 7461 206f  iated metadata o
+00001880: 626a 6563 742e 2054 6865 2050 616e 6461  bject. The Panda
+00001890: 7320 6461 7461 2066 7261 6d65 2063 6f6e  s data frame con
+000018a0: 7461 696e 7320 7468 6520 7369 7465 2069  tains the site i
+000018b0: 6e66 6f72 6d61 7469 6f6e 2066 6f72 2074  nformation for t
+000018c0: 6865 2072 6571 7565 7374 6564 2073 6974  he requested sit
+000018d0: 652e 5c6e 222c 0a20 2020 2022 5c6e 222c  e.\n",.    "\n",
+000018e0: 0a20 2020 2022 4f6e 6365 2079 6f75 2776  .    "Once you'v
+000018f0: 6520 676f 7420 7468 6520 6461 7461 2066  e got the data f
+00001900: 7261 6d65 2c20 7468 6572 6527 7320 7365  rame, there's se
+00001910: 7665 7261 6c20 7573 6566 756c 2074 6869  veral useful thi
+00001920: 6e67 7320 796f 7520 6361 6e20 646f 2074  ngs you can do t
+00001930: 6f20 6578 706c 6f72 6520 7468 6520 696e  o explore the in
+00001940: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+00001950: 7468 6520 7369 7465 2e22 0a20 2020 5d0a  the site.".   ].
+00001960: 2020 7d2c 0a20 207b 0a20 2020 2263 656c    },.  {.   "cel
+00001970: 6c5f 7479 7065 223a 2022 636f 6465 222c  l_type": "code",
+00001980: 0a20 2020 2265 7865 6375 7469 6f6e 5f63  .   "execution_c
+00001990: 6f75 6e74 223a 206e 756c 6c2c 0a20 2020  ount": null,.   
+000019a0: 226d 6574 6164 6174 6122 3a20 7b0a 2020  "metadata": {.  
+000019b0: 2020 2263 6f6c 6c61 7073 6564 223a 2066    "collapsed": f
+000019c0: 616c 7365 2c0a 2020 2020 226a 7570 7974  alse,.    "jupyt
+000019d0: 6572 223a 207b 0a20 2020 2020 226f 7574  er": {.     "out
+000019e0: 7075 7473 5f68 6964 6465 6e22 3a20 6661  puts_hidden": fa
+000019f0: 6c73 650a 2020 2020 7d2c 0a20 2020 2022  lse.    },.    "
+00001a00: 7079 6368 6172 6d22 3a20 7b0a 2020 2020  pycharm": {.    
+00001a10: 2022 6e61 6d65 223a 2022 2325 255c 6e22   "name": "#%%\n"
+00001a20: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
+00001a30: 226f 7574 7075 7473 223a 205b 5d2c 0a20  "outputs": [],. 
+00001a40: 2020 2273 6f75 7263 6522 3a20 5b0a 2020    "source": [.  
+00001a50: 2020 2223 2044 6973 706c 6179 2074 6865    "# Display the
+00001a60: 2064 6174 6120 6672 616d 6520 6173 2061   data frame as a
+00001a70: 2074 6162 6c65 5c6e 222c 0a20 2020 2022   table\n",.    "
+00001a80: 6469 7370 6c61 7928 7369 7465 494e 464f  display(siteINFO
+00001a90: 5b30 5d29 220a 2020 205d 0a20 207d 2c0a  [0])".   ].  },.
+00001aa0: 2020 7b0a 2020 2022 6365 6c6c 5f74 7970    {.   "cell_typ
+00001ab0: 6522 3a20 226d 6172 6b64 6f77 6e22 2c0a  e": "markdown",.
+00001ac0: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
+00001ad0: 7d2c 0a20 2020 2273 6f75 7263 6522 3a20  },.   "source": 
+00001ae0: 5b0a 2020 2020 2253 686f 7720 7468 6520  [.    "Show the 
+00001af0: 6461 7461 2074 7970 6573 206f 6620 7468  data types of th
+00001b00: 6520 636f 6c75 6d6e 7320 696e 2074 6865  e columns in the
+00001b10: 2072 6573 756c 7469 6e67 2064 6174 6120   resulting data 
+00001b20: 6672 616d 652e 220a 2020 205d 0a20 207d  frame.".   ].  }
+00001b30: 2c0a 2020 7b0a 2020 2022 6365 6c6c 5f74  ,.  {.   "cell_t
+00001b40: 7970 6522 3a20 2263 6f64 6522 2c0a 2020  ype": "code",.  
+00001b50: 2022 6578 6563 7574 696f 6e5f 636f 756e   "execution_coun
+00001b60: 7422 3a20 6e75 6c6c 2c0a 2020 2022 6d65  t": null,.   "me
+00001b70: 7461 6461 7461 223a 207b 0a20 2020 2022  tadata": {.    "
+00001b80: 636f 6c6c 6170 7365 6422 3a20 6661 6c73  collapsed": fals
+00001b90: 652c 0a20 2020 2022 6a75 7079 7465 7222  e,.    "jupyter"
+00001ba0: 3a20 7b0a 2020 2020 2022 6f75 7470 7574  : {.     "output
+00001bb0: 735f 6869 6464 656e 223a 2066 616c 7365  s_hidden": false
+00001bc0: 0a20 2020 207d 2c0a 2020 2020 2270 7963  .    },.    "pyc
+00001bd0: 6861 726d 223a 207b 0a20 2020 2020 226e  harm": {.     "n
+00001be0: 616d 6522 3a20 2223 2525 5c6e 220a 2020  ame": "#%%\n".  
+00001bf0: 2020 7d0a 2020 207d 2c0a 2020 2022 6f75    }.   },.   "ou
+00001c00: 7470 7574 7322 3a20 5b5d 2c0a 2020 2022  tputs": [],.   "
+00001c10: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
+00001c20: 7072 696e 7428 7369 7465 494e 464f 5b30  print(siteINFO[0
+00001c30: 5d2e 6474 7970 6573 2922 0a20 2020 5d0a  ].dtypes)".   ].
+00001c40: 2020 7d2c 0a20 207b 0a20 2020 2263 656c    },.  {.   "cel
+00001c50: 6c5f 7479 7065 223a 2022 6d61 726b 646f  l_type": "markdo
+00001c60: 776e 222c 0a20 2020 226d 6574 6164 6174  wn",.   "metadat
+00001c70: 6122 3a20 7b7d 2c0a 2020 2022 736f 7572  a": {},.   "sour
+00001c80: 6365 223a 205b 0a20 2020 2022 5468 6520  ce": [.    "The 
+00001c90: 6f74 6865 7220 7061 7274 206f 6620 7468  other part of th
+00001ca0: 6520 7265 7375 6c74 2072 6574 7572 6e65  e result returne
+00001cb0: 6420 6672 6f6d 2074 6865 2060 6765 745f  d from the `get_
+00001cc0: 696e 666f 2829 6020 6675 6e63 7469 6f6e  info()` function
+00001cd0: 2069 7320 6120 6d65 7461 6461 7461 206f   is a metadata o
+00001ce0: 626a 6563 7420 7468 6174 2063 6f6e 7461  bject that conta
+00001cf0: 696e 7320 696e 666f 726d 6174 696f 6e20  ins information 
+00001d00: 6162 6f75 7420 7468 6520 7175 6572 7920  about the query 
+00001d10: 7468 6174 2077 6173 2065 7865 6375 7465  that was execute
+00001d20: 6420 746f 2072 6574 7572 6e20 7468 6520  d to return the 
+00001d30: 6461 7461 2e20 466f 7220 6578 616d 706c  data. For exampl
+00001d40: 652c 2079 6f75 2063 616e 2061 6363 6573  e, you can acces
+00001d50: 7320 7468 6520 5552 4c20 7468 6174 2077  s the URL that w
+00001d60: 6173 2061 7373 656d 626c 6564 2074 6f20  as assembled to 
+00001d70: 7265 7472 6965 7665 2074 6865 2072 6571  retrieve the req
+00001d80: 7565 7374 6564 2064 6174 6120 6672 6f6d  uested data from
+00001d90: 2074 6865 2055 5347 5320 7765 6220 7365   the USGS web se
+00001da0: 7276 6963 652e 2054 6865 2055 5347 5320  rvice. The USGS 
+00001db0: 7765 6220 7365 7276 6963 6520 7265 7370  web service resp
+00001dc0: 6f6e 7365 7320 636f 6e74 6169 6e20 6120  onses contain a 
+00001dd0: 6465 7363 7269 7074 6976 6520 6865 6164  descriptive head
+00001de0: 6572 2074 6861 7420 6465 6669 6e65 7320  er that defines 
+00001df0: 616e 6420 6361 6e20 6265 2068 656c 7066  and can be helpf
+00001e00: 756c 2069 6e20 696e 7465 7270 7265 7469  ul in interpreti
+00001e10: 6e67 2074 6865 2063 6f6e 7465 6e74 7320  ng the contents 
+00001e20: 6f66 2074 6865 2072 6573 706f 6e73 652e  of the response.
+00001e30: 220a 2020 205d 0a20 207d 2c0a 2020 7b0a  ".   ].  },.  {.
+00001e40: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
+00001e50: 2263 6f64 6522 2c0a 2020 2022 6578 6563  "code",.   "exec
+00001e60: 7574 696f 6e5f 636f 756e 7422 3a20 6e75  ution_count": nu
+00001e70: 6c6c 2c0a 2020 2022 6d65 7461 6461 7461  ll,.   "metadata
+00001e80: 223a 207b 0a20 2020 2022 636f 6c6c 6170  ": {.    "collap
+00001e90: 7365 6422 3a20 6661 6c73 652c 0a20 2020  sed": false,.   
+00001ea0: 2022 6a75 7079 7465 7222 3a20 7b0a 2020   "jupyter": {.  
+00001eb0: 2020 2022 6f75 7470 7574 735f 6869 6464     "outputs_hidd
+00001ec0: 656e 223a 2066 616c 7365 0a20 2020 207d  en": false.    }
+00001ed0: 2c0a 2020 2020 2270 7963 6861 726d 223a  ,.    "pycharm":
+00001ee0: 207b 0a20 2020 2020 226e 616d 6522 3a20   {.     "name": 
+00001ef0: 2223 2525 5c6e 220a 2020 2020 7d0a 2020  "#%%\n".    }.  
+00001f00: 207d 2c0a 2020 2022 6f75 7470 7574 7322   },.   "outputs"
+00001f10: 3a20 5b5d 2c0a 2020 2022 736f 7572 6365  : [],.   "source
+00001f20: 223a 205b 0a20 2020 2022 7072 696e 7428  ": [.    "print(
+00001f30: 5c22 5468 6520 7175 6572 7920 5552 4c20  \"The query URL 
+00001f40: 7573 6564 2074 6f20 7265 7472 6965 7665  used to retrieve
+00001f50: 2074 6865 2064 6174 6120 6672 6f6d 204e   the data from N
+00001f60: 5749 5320 7761 733a 205c 2220 2b20 7369  WIS was: \" + si
+00001f70: 7465 494e 464f 5b31 5d2e 7572 6c29 220a  teINFO[1].url)".
+00001f80: 2020 205d 0a20 207d 2c0a 2020 7b0a 2020     ].  },.  {.  
+00001f90: 2022 6365 6c6c 5f74 7970 6522 3a20 226d   "cell_type": "m
+00001fa0: 6172 6b64 6f77 6e22 2c0a 2020 2022 6d65  arkdown",.   "me
+00001fb0: 7461 6461 7461 223a 207b 7d2c 0a20 2020  tadata": {},.   
+00001fc0: 2273 6f75 7263 6522 3a20 5b0a 2020 2020  "source": [.    
+00001fd0: 2223 2323 2041 6464 6974 696f 6e61 6c20  "### Additional 
+00001fe0: 4578 616d 706c 6573 5c6e 222c 0a20 2020  Examples\n",.   
+00001ff0: 2022 5c6e 222c 0a20 2020 2022 2323 2323   "\n",.    "####
+00002000: 2045 7861 6d70 6c65 2032 3a20 4765 7420   Example 2: Get 
+00002010: 7369 7465 2069 6e66 6f72 6d61 7469 6f6e  site information
+00002020: 2066 6f72 206d 756c 7469 706c 6520 7369   for multiple si
+00002030: 7465 7320 696e 2061 206c 6973 7422 0a20  tes in a list". 
+00002040: 2020 5d0a 2020 7d2c 0a20 207b 0a20 2020    ].  },.  {.   
+00002050: 2263 656c 6c5f 7479 7065 223a 2022 636f  "cell_type": "co
+00002060: 6465 222c 0a20 2020 2265 7865 6375 7469  de",.   "executi
+00002070: 6f6e 5f63 6f75 6e74 223a 206e 756c 6c2c  on_count": null,
+00002080: 0a20 2020 226d 6574 6164 6174 6122 3a20  .   "metadata": 
+00002090: 7b0a 2020 2020 2263 6f6c 6c61 7073 6564  {.    "collapsed
+000020a0: 223a 2066 616c 7365 2c0a 2020 2020 226a  ": false,.    "j
+000020b0: 7570 7974 6572 223a 207b 0a20 2020 2020  upyter": {.     
+000020c0: 226f 7574 7075 7473 5f68 6964 6465 6e22  "outputs_hidden"
+000020d0: 3a20 6661 6c73 650a 2020 2020 7d2c 0a20  : false.    },. 
+000020e0: 2020 2022 7079 6368 6172 6d22 3a20 7b0a     "pycharm": {.
+000020f0: 2020 2020 2022 6e61 6d65 223a 2022 2325       "name": "#%
+00002100: 255c 6e22 0a20 2020 207d 0a20 2020 7d2c  %\n".    }.   },
+00002110: 0a20 2020 226f 7574 7075 7473 223a 205b  .   "outputs": [
+00002120: 5d2c 0a20 2020 2273 6f75 7263 6522 3a20  ],.   "source": 
+00002130: 5b0a 2020 2020 2223 2043 7265 6174 6520  [.    "# Create 
+00002140: 6120 6c69 7374 206f 6620 7468 6520 7369  a list of the si
+00002150: 7465 2069 6465 6e74 6966 6965 7273 2079  te identifiers y
+00002160: 6f75 2077 616e 7420 746f 2072 6574 7269  ou want to retri
+00002170: 6576 6520 696e 666f 726d 6174 696f 6e20  eve information 
+00002180: 666f 725c 6e22 2c0a 2020 2020 2273 6974  for\n",.    "sit
+00002190: 6549 4473 203d 205b 5c22 3035 3131 3430  eIDs = [\"051140
+000021a0: 3030 5c22 2c20 5c22 3039 3432 3333 3530  00\", \"09423350
+000021b0: 5c22 5d5c 6e22 2c0a 2020 2020 225c 6e22  \"]\n",.    "\n"
+000021c0: 2c0a 2020 2020 2223 2047 6574 2074 6865  ,.    "# Get the
+000021d0: 2073 6974 6520 696e 666f 726d 6174 696f   site informatio
+000021e0: 6e5c 6e22 2c0a 2020 2020 2273 6974 6549  n\n",.    "siteI
+000021f0: 4e46 4f5f 6d75 6c74 6920 3d20 6e77 6973  NFO_multi = nwis
+00002200: 2e67 6574 5f69 6e66 6f28 7369 7465 733d  .get_info(sites=
+00002210: 7369 7465 4944 7329 5c6e 222c 0a20 2020  siteIDs)\n",.   
+00002220: 2022 6469 7370 6c61 7928 7369 7465 494e   "display(siteIN
+00002230: 464f 5f6d 756c 7469 5b30 5d29 220a 2020  FO_multi[0])".  
+00002240: 205d 0a20 207d 2c0a 2020 7b0a 2020 2022   ].  },.  {.   "
+00002250: 6365 6c6c 5f74 7970 6522 3a20 226d 6172  cell_type": "mar
+00002260: 6b64 6f77 6e22 2c0a 2020 2022 6d65 7461  kdown",.   "meta
+00002270: 6461 7461 223a 207b 7d2c 0a20 2020 2273  data": {},.   "s
+00002280: 6f75 7263 6522 3a20 5b0a 2020 2020 2223  ource": [.    "#
+00002290: 2323 2320 4578 616d 706c 6520 333a 2047  ### Example 3: G
+000022a0: 6574 2073 6974 6520 696e 666f 726d 6174  et site informat
+000022b0: 696f 6e20 666f 7220 616c 6c20 7369 7465  ion for all site
+000022c0: 7320 7769 7468 696e 2061 2073 7461 7465  s within a state
+000022d0: 220a 2020 205d 0a20 207d 2c0a 2020 7b0a  ".   ].  },.  {.
+000022e0: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
+000022f0: 2263 6f64 6522 2c0a 2020 2022 6578 6563  "code",.   "exec
+00002300: 7574 696f 6e5f 636f 756e 7422 3a20 6e75  ution_count": nu
+00002310: 6c6c 2c0a 2020 2022 6d65 7461 6461 7461  ll,.   "metadata
+00002320: 223a 207b 7d2c 0a20 2020 226f 7574 7075  ": {},.   "outpu
+00002330: 7473 223a 205b 5d2c 0a20 2020 2273 6f75  ts": [],.   "sou
+00002340: 7263 6522 3a20 5b0a 2020 2020 2223 2047  rce": [.    "# G
+00002350: 6574 2074 6865 2073 6974 6520 696e 666f  et the site info
+00002360: 726d 6174 696f 6e20 666f 7220 6120 7374  rmation for a st
+00002370: 6174 655c 6e22 2c0a 2020 2020 2273 6974  ate\n",.    "sit
+00002380: 6549 4e46 4f5f 7374 6174 6520 3d20 6e77  eINFO_state = nw
+00002390: 6973 2e67 6574 5f69 6e66 6f28 7374 6174  is.get_info(stat
+000023a0: 6543 643d 2755 5427 295c 6e22 2c0a 2020  eCd='UT')\n",.  
+000023b0: 2020 2264 6973 706c 6179 2873 6974 6549    "display(siteI
+000023c0: 4e46 4f5f 7374 6174 655b 305d 2922 0a20  NFO_state[0])". 
+000023d0: 2020 5d0a 2020 7d2c 0a20 207b 0a20 2020    ].  },.  {.   
+000023e0: 2263 656c 6c5f 7479 7065 223a 2022 6d61  "cell_type": "ma
+000023f0: 726b 646f 776e 222c 0a20 2020 226d 6574  rkdown",.   "met
+00002400: 6164 6174 6122 3a20 7b7d 2c0a 2020 2022  adata": {},.   "
+00002410: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
+00002420: 2323 2323 2045 7861 6d70 6c65 2034 3a20  #### Example 4: 
+00002430: 4765 7420 7369 7465 2069 6e66 6f72 6d61  Get site informa
+00002440: 7469 6f6e 2066 6f72 2061 6c6c 205c 2273  tion for all \"s
+00002450: 7472 6561 6d5c 2220 7369 7465 7320 7769  tream\" sites wi
+00002460: 7468 696e 2061 2055 5347 5320 4855 4322  thin a USGS HUC"
+00002470: 0a20 2020 5d0a 2020 7d2c 0a20 207b 0a20  .   ].  },.  {. 
+00002480: 2020 2263 656c 6c5f 7479 7065 223a 2022    "cell_type": "
+00002490: 636f 6465 222c 0a20 2020 2265 7865 6375  code",.   "execu
+000024a0: 7469 6f6e 5f63 6f75 6e74 223a 206e 756c  tion_count": nul
+000024b0: 6c2c 0a20 2020 226d 6574 6164 6174 6122  l,.   "metadata"
+000024c0: 3a20 7b7d 2c0a 2020 2022 6f75 7470 7574  : {},.   "output
+000024d0: 7322 3a20 5b5d 2c0a 2020 2022 736f 7572  s": [],.   "sour
+000024e0: 6365 223a 205b 0a20 2020 2022 2320 4372  ce": [.    "# Cr
+000024f0: 6561 7465 2061 206c 6973 7420 6f66 2068  eate a list of h
+00002500: 7563 7320 666f 7220 7768 6963 6820 746f  ucs for which to
+00002510: 2071 7565 7279 2073 6974 6573 5c6e 222c   query sites\n",
+00002520: 0a20 2020 2022 6875 635f 6c69 7374 203d  .    "huc_list =
+00002530: 205b 2731 3630 3130 3230 3327 5d5c 6e22   ['16010203']\n"
+00002540: 2c0a 2020 2020 225c 6e22 2c0a 2020 2020  ,.    "\n",.    
+00002550: 2223 2047 6574 2074 6865 2073 6974 6520  "# Get the site 
+00002560: 696e 666f 726d 6174 696f 6e20 2d20 6c69  information - li
+00002570: 6d69 7420 746f 2073 7472 6561 6d20 7369  mit to stream si
+00002580: 7465 735c 6e22 2c0a 2020 2020 2273 6974  tes\n",.    "sit
+00002590: 6549 4e46 4f5f 6875 6320 3d20 6e77 6973  eINFO_huc = nwis
+000025a0: 2e67 6574 5f69 6e66 6f28 6875 633d 6875  .get_info(huc=hu
+000025b0: 635f 6c69 7374 2c20 7369 7465 5479 7065  c_list, siteType
+000025c0: 3d27 5354 2729 5c6e 222c 0a20 2020 2022  ='ST')\n",.    "
+000025d0: 6469 7370 6c61 7928 7369 7465 494e 464f  display(siteINFO
+000025e0: 5f68 7563 5b30 5d29 220a 2020 205d 0a20  _huc[0])".   ]. 
+000025f0: 207d 0a20 5d2c 0a20 226d 6574 6164 6174   }. ],. "metadat
+00002600: 6122 3a20 7b0a 2020 226b 6572 6e65 6c73  a": {.  "kernels
+00002610: 7065 6322 3a20 7b0a 2020 2022 6469 7370  pec": {.   "disp
+00002620: 6c61 795f 6e61 6d65 223a 2022 5079 7468  lay_name": "Pyth
+00002630: 6f6e 2033 2028 6970 796b 6572 6e65 6c29  on 3 (ipykernel)
+00002640: 222c 0a20 2020 226c 616e 6775 6167 6522  ",.   "language"
+00002650: 3a20 2270 7974 686f 6e22 2c0a 2020 2022  : "python",.   "
+00002660: 6e61 6d65 223a 2022 7079 7468 6f6e 3322  name": "python3"
+00002670: 0a20 207d 2c0a 2020 226c 616e 6775 6167  .  },.  "languag
+00002680: 655f 696e 666f 223a 207b 0a20 2020 2263  e_info": {.   "c
+00002690: 6f64 656d 6972 726f 725f 6d6f 6465 223a  odemirror_mode":
+000026a0: 207b 0a20 2020 2022 6e61 6d65 223a 2022   {.    "name": "
+000026b0: 6970 7974 686f 6e22 2c0a 2020 2020 2276  ipython",.    "v
+000026c0: 6572 7369 6f6e 223a 2033 0a20 2020 7d2c  ersion": 3.   },
+000026d0: 0a20 2020 2266 696c 655f 6578 7465 6e73  .   "file_extens
+000026e0: 696f 6e22 3a20 222e 7079 222c 0a20 2020  ion": ".py",.   
+000026f0: 226d 696d 6574 7970 6522 3a20 2274 6578  "mimetype": "tex
+00002700: 742f 782d 7079 7468 6f6e 222c 0a20 2020  t/x-python",.   
+00002710: 226e 616d 6522 3a20 2270 7974 686f 6e22  "name": "python"
+00002720: 2c0a 2020 2022 6e62 636f 6e76 6572 745f  ,.   "nbconvert_
+00002730: 6578 706f 7274 6572 223a 2022 7079 7468  exporter": "pyth
+00002740: 6f6e 222c 0a20 2020 2270 7967 6d65 6e74  on",.   "pygment
+00002750: 735f 6c65 7865 7222 3a20 2269 7079 7468  s_lexer": "ipyth
+00002760: 6f6e 3322 2c0a 2020 2022 7665 7273 696f  on3",.   "versio
+00002770: 6e22 3a20 2233 2e39 2e37 220a 2020 7d0a  n": "3.9.7".  }.
+00002780: 207d 2c0a 2022 6e62 666f 726d 6174 223a   },. "nbformat":
+00002790: 2034 2c0a 2022 6e62 666f 726d 6174 5f6d   4,. "nbformat_m
+000027a0: 696e 6f72 223a 2034 0a7d 0a              inor": 4.}.
```

### Comparing `dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb` & `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb`

 * *Files 1% similar despite different names*

```diff
@@ -316,301 +316,302 @@
 000013b0: 6120 7369 7465 2773 2064 6169 6c79 206d  a site's daily m
 000013c0: 6561 6e20 7374 7265 616d 666c 6f77 2e5c  ean streamflow.\
 000013d0: 6e22 2c0a 2020 2020 225c 6e22 2c0a 2020  n",.    "\n",.  
 000013e0: 2020 2246 6f72 2061 6464 6974 696f 6e61    "For additiona
 000013f0: 6c20 7061 7261 6d65 7465 7220 6f70 7469  l parameter opti
 00001400: 6f6e 7320 7365 6520 6874 7470 733a 2f2f  ons see https://
 00001410: 7761 7465 7273 6572 7669 6365 732e 7573  waterservices.us
-00001420: 6773 2e67 6f76 2f72 6573 742f 5369 7465  gs.gov/rest/Site
-00001430: 2d53 6572 7669 6365 2e68 746d 6c23 7374  -Service.html#st
-00001440: 6174 6543 6422 0a20 2020 5d0a 2020 7d2c  ateCd".   ].  },
-00001450: 0a20 207b 0a20 2020 2263 656c 6c5f 7479  .  {.   "cell_ty
-00001460: 7065 223a 2022 6d61 726b 646f 776e 222c  pe": "markdown",
-00001470: 0a20 2020 226d 6574 6164 6174 6122 3a20  .   "metadata": 
-00001480: 7b7d 2c0a 2020 2022 736f 7572 6365 223a  {},.   "source":
-00001490: 205b 0a20 2020 2022 2323 2323 2045 7861   [.    "#### Exa
-000014a0: 6d70 6c65 2031 3a20 5265 7472 6965 7665  mple 1: Retrieve
-000014b0: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
-000014c0: 7574 2073 6974 6573 2069 6e20 4f68 696f  ut sites in Ohio
-000014d0: 2077 6865 7265 2070 686f 7370 686f 7275   where phosphoru
-000014e0: 7320 6461 7461 2077 6173 2063 6f6c 6c65  s data was colle
-000014f0: 6374 6564 220a 2020 205d 0a20 207d 2c0a  cted".   ].  },.
-00001500: 2020 7b0a 2020 2022 6365 6c6c 5f74 7970    {.   "cell_typ
-00001510: 6522 3a20 2263 6f64 6522 2c0a 2020 2022  e": "code",.   "
-00001520: 6578 6563 7574 696f 6e5f 636f 756e 7422  execution_count"
-00001530: 3a20 6e75 6c6c 2c0a 2020 2022 6d65 7461  : null,.   "meta
-00001540: 6461 7461 223a 207b 0a20 2020 2022 636f  data": {.    "co
-00001550: 6c6c 6170 7365 6422 3a20 6661 6c73 652c  llapsed": false,
-00001560: 0a20 2020 2022 6a75 7079 7465 7222 3a20  .    "jupyter": 
-00001570: 7b0a 2020 2020 2022 6f75 7470 7574 735f  {.     "outputs_
-00001580: 6869 6464 656e 223a 2066 616c 7365 0a20  hidden": false. 
-00001590: 2020 207d 2c0a 2020 2020 2270 7963 6861     },.    "pycha
-000015a0: 726d 223a 207b 0a20 2020 2020 226e 616d  rm": {.     "nam
-000015b0: 6522 3a20 2223 2525 5c6e 220a 2020 2020  e": "#%%\n".    
-000015c0: 7d0a 2020 207d 2c0a 2020 2022 6f75 7470  }.   },.   "outp
-000015d0: 7574 7322 3a20 5b5d 2c0a 2020 2022 736f  uts": [],.   "so
-000015e0: 7572 6365 223a 205b 0a20 2020 2022 7369  urce": [.    "si
-000015f0: 7465 4c69 7374 5068 6f73 203d 206e 7769  teListPhos = nwi
-00001600: 732e 7768 6174 5f73 6974 6573 2873 7461  s.what_sites(sta
-00001610: 7465 4364 3d5c 224f 485c 222c 2070 6172  teCd=\"OH\", par
-00001620: 616d 6574 6572 4364 3d5c 2230 3036 3635  ameterCd=\"00665
-00001630: 5c22 2922 0a20 2020 5d0a 2020 7d2c 0a20  \")".   ].  },. 
-00001640: 207b 0a20 2020 2263 656c 6c5f 7479 7065   {.   "cell_type
-00001650: 223a 2022 6d61 726b 646f 776e 222c 0a20  ": "markdown",. 
-00001660: 2020 226d 6574 6164 6174 6122 3a20 7b7d    "metadata": {}
-00001670: 2c0a 2020 2022 736f 7572 6365 223a 205b  ,.   "source": [
-00001680: 0a20 2020 2022 2323 2320 496e 7465 7270  .    "### Interp
-00001690: 7265 7469 6e67 2074 6865 2052 6573 756c  reting the Resul
-000016a0: 745c 6e22 2c0a 2020 2020 225c 6e22 2c0a  t\n",.    "\n",.
-000016b0: 2020 2020 2254 6865 2072 6573 756c 7420      "The result 
-000016c0: 6f66 2063 616c 6c69 6e67 2074 6865 2060  of calling the `
-000016d0: 7768 6174 5f73 6974 6573 2829 6020 6675  what_sites()` fu
-000016e0: 6e63 7469 6f6e 2069 7320 616e 206f 626a  nction is an obj
-000016f0: 6563 7420 7468 6174 2063 6f6e 7461 696e  ect that contain
-00001700: 7320 6120 5061 6e64 6173 2064 6174 6120  s a Pandas data 
-00001710: 6672 616d 6520 6f62 6a65 6374 2061 6e64  frame object and
-00001720: 2061 6e20 6173 736f 6369 6174 6564 206d   an associated m
-00001730: 6574 6164 6174 6120 6f62 6a65 6374 2e20  etadata object. 
-00001740: 5468 6520 5061 6e64 6173 2064 6174 6120  The Pandas data 
-00001750: 6672 616d 6520 636f 6e74 6169 6e73 2074  frame contains t
-00001760: 6865 2072 6571 7565 7374 6573 2073 6974  he requestes sit
-00001770: 6520 696e 7665 6e74 6f72 7920 6461 7461  e inventory data
-00001780: 2e5c 6e22 2c0a 2020 2020 225c 6e22 2c0a  .\n",.    "\n",.
-00001790: 2020 2020 224f 6e63 6520 796f 7527 7665      "Once you've
-000017a0: 2067 6f74 2074 6865 2064 6174 6120 6672   got the data fr
-000017b0: 616d 652c 2074 6865 7265 2773 2073 6576  ame, there's sev
-000017c0: 6572 616c 2075 7365 6675 6c20 7468 696e  eral useful thin
-000017d0: 6773 2079 6f75 2063 616e 2064 6f20 746f  gs you can do to
-000017e0: 2065 7870 6c6f 7265 2074 6865 2064 6174   explore the dat
-000017f0: 612e 220a 2020 205d 0a20 207d 2c0a 2020  a.".   ].  },.  
-00001800: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
-00001810: 3a20 2263 6f64 6522 2c0a 2020 2022 6578  : "code",.   "ex
-00001820: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
-00001830: 6e75 6c6c 2c0a 2020 2022 6d65 7461 6461  null,.   "metada
-00001840: 7461 223a 207b 0a20 2020 2022 636f 6c6c  ta": {.    "coll
-00001850: 6170 7365 6422 3a20 6661 6c73 652c 0a20  apsed": false,. 
-00001860: 2020 2022 6a75 7079 7465 7222 3a20 7b0a     "jupyter": {.
-00001870: 2020 2020 2022 6f75 7470 7574 735f 6869       "outputs_hi
-00001880: 6464 656e 223a 2066 616c 7365 0a20 2020  dden": false.   
-00001890: 207d 2c0a 2020 2020 2270 7963 6861 726d   },.    "pycharm
-000018a0: 223a 207b 0a20 2020 2020 226e 616d 6522  ": {.     "name"
-000018b0: 3a20 2223 2525 5c6e 220a 2020 2020 7d0a  : "#%%\n".    }.
-000018c0: 2020 207d 2c0a 2020 2022 6f75 7470 7574     },.   "output
-000018d0: 7322 3a20 5b5d 2c0a 2020 2022 736f 7572  s": [],.   "sour
-000018e0: 6365 223a 205b 0a20 2020 2022 2320 4469  ce": [.    "# Di
-000018f0: 7370 6c61 7920 7468 6520 6461 7461 2066  splay the data f
-00001900: 7261 6d65 2061 7320 6120 7461 626c 655c  rame as a table\
-00001910: 6e22 2c0a 2020 2020 2264 6973 706c 6179  n",.    "display
-00001920: 2873 6974 654c 6973 7450 686f 735b 305d  (siteListPhos[0]
-00001930: 2922 0a20 2020 5d0a 2020 7d2c 0a20 207b  )".   ].  },.  {
-00001940: 0a20 2020 2263 656c 6c5f 7479 7065 223a  .   "cell_type":
-00001950: 2022 6d61 726b 646f 776e 222c 0a20 2020   "markdown",.   
-00001960: 226d 6574 6164 6174 6122 3a20 7b0a 2020  "metadata": {.  
-00001970: 2020 2270 7963 6861 726d 223a 207b 0a20    "pycharm": {. 
-00001980: 2020 2020 226e 616d 6522 3a20 2223 2525      "name": "#%%
-00001990: 206d 645c 6e22 0a20 2020 207d 0a20 2020   md\n".    }.   
-000019a0: 7d2c 0a20 2020 2273 6f75 7263 6522 3a20  },.   "source": 
-000019b0: 5b0a 2020 2020 2254 6865 206f 7468 6572  [.    "The other
-000019c0: 2070 6172 7420 6f66 2074 6865 2072 6573   part of the res
-000019d0: 756c 7420 7265 7475 726e 6564 2066 726f  ult returned fro
-000019e0: 6d20 7468 6520 6077 6861 745f 7369 7465  m the `what_site
-000019f0: 7328 2960 2066 756e 6374 696f 6e20 6973  s()` function is
-00001a00: 2061 206d 6574 6164 6174 6120 6f62 6a65   a metadata obje
-00001a10: 6374 2074 6861 7420 636f 6e74 6169 6e73  ct that contains
-00001a20: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
-00001a30: 7574 2074 6865 2071 7565 7279 2074 6861  ut the query tha
-00001a40: 7420 7761 7320 6578 6563 7574 6564 2074  t was executed t
-00001a50: 6f20 7265 7475 726e 2074 6865 2064 6174  o return the dat
-00001a60: 612e 2046 6f72 2065 7861 6d70 6c65 2c20  a. For example, 
-00001a70: 796f 7520 6361 6e20 6163 6365 7373 2074  you can access t
-00001a80: 6865 2055 524c 2074 6861 7420 7761 7320  he URL that was 
-00001a90: 6173 7365 6d62 6c65 6420 746f 2072 6574  assembled to ret
-00001aa0: 7269 6576 6520 7468 6520 7265 7175 6573  rieve the reques
-00001ab0: 7465 6420 6461 7461 2066 726f 6d20 7468  ted data from th
-00001ac0: 6520 5553 4753 2077 6562 2073 6572 7669  e USGS web servi
-00001ad0: 6365 2e20 5468 6520 5553 4753 2077 6562  ce. The USGS web
-00001ae0: 2073 6572 7669 6365 2072 6573 706f 6e73   service respons
-00001af0: 6573 2063 6f6e 7461 696e 2061 2064 6573  es contain a des
-00001b00: 6372 6970 7469 7665 2068 6561 6465 7220  criptive header 
-00001b10: 7468 6174 2064 6566 696e 6573 2061 6e64  that defines and
-00001b20: 2063 616e 2062 6520 6865 6c70 6675 6c20   can be helpful 
-00001b30: 696e 2069 6e74 6572 7072 6574 696e 6720  in interpreting 
-00001b40: 7468 6520 636f 6e74 656e 7473 206f 6620  the contents of 
-00001b50: 7468 6520 7265 7370 6f6e 7365 2e22 0a20  the response.". 
-00001b60: 2020 5d0a 2020 7d2c 0a20 207b 0a20 2020    ].  },.  {.   
-00001b70: 2263 656c 6c5f 7479 7065 223a 2022 636f  "cell_type": "co
-00001b80: 6465 222c 0a20 2020 2265 7865 6375 7469  de",.   "executi
-00001b90: 6f6e 5f63 6f75 6e74 223a 206e 756c 6c2c  on_count": null,
-00001ba0: 0a20 2020 226d 6574 6164 6174 6122 3a20  .   "metadata": 
-00001bb0: 7b0a 2020 2020 2263 6f6c 6c61 7073 6564  {.    "collapsed
-00001bc0: 223a 2066 616c 7365 2c0a 2020 2020 226a  ": false,.    "j
-00001bd0: 7570 7974 6572 223a 207b 0a20 2020 2020  upyter": {.     
-00001be0: 226f 7574 7075 7473 5f68 6964 6465 6e22  "outputs_hidden"
-00001bf0: 3a20 6661 6c73 650a 2020 2020 7d2c 0a20  : false.    },. 
-00001c00: 2020 2022 7079 6368 6172 6d22 3a20 7b0a     "pycharm": {.
-00001c10: 2020 2020 2022 6e61 6d65 223a 2022 2325       "name": "#%
-00001c20: 255c 6e22 0a20 2020 207d 0a20 2020 7d2c  %\n".    }.   },
-00001c30: 0a20 2020 226f 7574 7075 7473 223a 205b  .   "outputs": [
-00001c40: 5d2c 0a20 2020 2273 6f75 7263 6522 3a20  ],.   "source": 
-00001c50: 5b0a 2020 2020 2270 7269 6e74 2827 5468  [.    "print('Th
-00001c60: 6520 7175 6572 7920 5552 4c20 7573 6564  e query URL used
-00001c70: 2074 6f20 7265 7472 6965 7665 2074 6865   to retrieve the
-00001c80: 2064 6174 6120 6672 6f6d 204e 5749 5320   data from NWIS 
-00001c90: 7761 733a 2027 202b 2073 6974 654c 6973  was: ' + siteLis
-00001ca0: 7450 686f 735b 315d 2e75 726c 2922 0a20  tPhos[1].url)". 
-00001cb0: 2020 5d0a 2020 7d2c 0a20 207b 0a20 2020    ].  },.  {.   
-00001cc0: 2263 656c 6c5f 7479 7065 223a 2022 6d61  "cell_type": "ma
-00001cd0: 726b 646f 776e 222c 0a20 2020 226d 6574  rkdown",.   "met
-00001ce0: 6164 6174 6122 3a20 7b7d 2c0a 2020 2022  adata": {},.   "
-00001cf0: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
-00001d00: 2323 2320 4164 6469 7469 6f6e 616c 2045  ### Additional E
-00001d10: 7861 6d70 6c65 735c 6e22 2c0a 2020 2020  xamples\n",.    
-00001d20: 225c 6e22 2c0a 2020 2020 2223 2323 2320  "\n",.    "#### 
-00001d30: 4578 616d 706c 6520 323a 2052 6574 7269  Example 2: Retri
-00001d40: 6576 6520 7369 7465 2069 6e66 6f72 6d61  eve site informa
-00001d50: 7469 6f6e 2066 6f72 2061 2073 696e 676c  tion for a singl
-00001d60: 6520 7369 7465 220a 2020 205d 0a20 207d  e site".   ].  }
-00001d70: 2c0a 2020 7b0a 2020 2022 6365 6c6c 5f74  ,.  {.   "cell_t
-00001d80: 7970 6522 3a20 2263 6f64 6522 2c0a 2020  ype": "code",.  
-00001d90: 2022 6578 6563 7574 696f 6e5f 636f 756e   "execution_coun
-00001da0: 7422 3a20 6e75 6c6c 2c0a 2020 2022 6d65  t": null,.   "me
-00001db0: 7461 6461 7461 223a 207b 0a20 2020 2022  tadata": {.    "
-00001dc0: 636f 6c6c 6170 7365 6422 3a20 6661 6c73  collapsed": fals
-00001dd0: 652c 0a20 2020 2022 6a75 7079 7465 7222  e,.    "jupyter"
-00001de0: 3a20 7b0a 2020 2020 2022 6f75 7470 7574  : {.     "output
-00001df0: 735f 6869 6464 656e 223a 2066 616c 7365  s_hidden": false
-00001e00: 0a20 2020 207d 2c0a 2020 2020 2270 7963  .    },.    "pyc
-00001e10: 6861 726d 223a 207b 0a20 2020 2020 226e  harm": {.     "n
-00001e20: 616d 6522 3a20 2223 2525 5c6e 220a 2020  ame": "#%%\n".  
-00001e30: 2020 7d0a 2020 207d 2c0a 2020 2022 6f75    }.   },.   "ou
-00001e40: 7470 7574 7322 3a20 5b5d 2c0a 2020 2022  tputs": [],.   "
-00001e50: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
-00001e60: 6f6e 6553 6974 6520 3d20 6e77 6973 2e77  oneSite = nwis.w
-00001e70: 6861 745f 7369 7465 7328 7369 7465 733d  hat_sites(sites=
-00001e80: 2730 3531 3134 3030 3027 295c 6e22 2c0a  '05114000')\n",.
-00001e90: 2020 2020 2264 6973 706c 6179 286f 6e65      "display(one
-00001ea0: 5369 7465 5b30 5d29 220a 2020 205d 0a20  Site[0])".   ]. 
-00001eb0: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
-00001ec0: 5f74 7970 6522 3a20 226d 6172 6b64 6f77  _type": "markdow
-00001ed0: 6e22 2c0a 2020 2022 6d65 7461 6461 7461  n",.   "metadata
-00001ee0: 223a 207b 7d2c 0a20 2020 2273 6f75 7263  ": {},.   "sourc
-00001ef0: 6522 3a20 5b0a 2020 2020 2223 2323 2320  e": [.    "#### 
-00001f00: 4578 616d 706c 6520 333a 2052 6574 7269  Example 3: Retri
-00001f10: 6576 6520 7369 7465 2069 6e66 6f72 6d61  eve site informa
-00001f20: 7469 6f6e 2066 6f72 2061 2073 696e 676c  tion for a singl
-00001f30: 6520 7369 7465 2061 6e64 2073 686f 7720  e site and show 
-00001f40: 7468 6520 7265 7375 6c74 2077 6974 6820  the result with 
-00001f50: 6578 7061 6e64 6564 206f 7574 7075 7422  expanded output"
-00001f60: 0a20 2020 5d0a 2020 7d2c 0a20 207b 0a20  .   ].  },.  {. 
-00001f70: 2020 2263 656c 6c5f 7479 7065 223a 2022    "cell_type": "
-00001f80: 636f 6465 222c 0a20 2020 2265 7865 6375  code",.   "execu
-00001f90: 7469 6f6e 5f63 6f75 6e74 223a 206e 756c  tion_count": nul
-00001fa0: 6c2c 0a20 2020 226d 6574 6164 6174 6122  l,.   "metadata"
-00001fb0: 3a20 7b7d 2c0a 2020 2022 6f75 7470 7574  : {},.   "output
-00001fc0: 7322 3a20 5b5d 2c0a 2020 2022 736f 7572  s": [],.   "sour
-00001fd0: 6365 223a 205b 0a20 2020 2022 6f6e 6553  ce": [.    "oneS
-00001fe0: 6974 6520 3d20 6e77 6973 2e77 6861 745f  ite = nwis.what_
-00001ff0: 7369 7465 7328 7369 7465 733d 2730 3531  sites(sites='051
-00002000: 3134 3030 3027 2c20 7369 7465 4f75 7470  14000', siteOutp
-00002010: 7574 3d27 6578 7061 6e64 6564 2729 5c6e  ut='expanded')\n
-00002020: 222c 0a20 2020 2022 6469 7370 6c61 7928  ",.    "display(
-00002030: 6f6e 6553 6974 655b 305d 2922 0a20 2020  oneSite[0])".   
-00002040: 5d0a 2020 7d2c 0a20 207b 0a20 2020 2263  ].  },.  {.   "c
-00002050: 656c 6c5f 7479 7065 223a 2022 6d61 726b  ell_type": "mark
-00002060: 646f 776e 222c 0a20 2020 226d 6574 6164  down",.   "metad
-00002070: 6174 6122 3a20 7b0a 2020 2020 2270 7963  ata": {.    "pyc
-00002080: 6861 726d 223a 207b 0a20 2020 2020 226e  harm": {.     "n
-00002090: 616d 6522 3a20 2223 2525 206d 645c 6e22  ame": "#%% md\n"
-000020a0: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
-000020b0: 2273 6f75 7263 6522 3a20 5b0a 2020 2020  "source": [.    
-000020c0: 2223 2323 2320 4578 616d 706c 6520 343a  "#### Example 4:
-000020d0: 2052 6574 7269 6576 6520 7369 7465 2069   Retrieve site i
-000020e0: 6e66 6f72 6d61 7469 6f6e 2066 6f72 2073  nformation for s
-000020f0: 6974 6573 2069 6e20 5574 6168 2077 6974  ites in Utah wit
-00002100: 6820 6461 696c 7920 7661 6c75 6573 2064  h daily values d
-00002110: 6174 6120 6661 6c6c 696e 6720 7769 7468  ata falling with
-00002120: 696e 2061 2073 7065 6369 6669 6564 2064  in a specified d
-00002130: 6174 6520 7261 6e67 6522 0a20 2020 5d0a  ate range".   ].
-00002140: 2020 7d2c 0a20 207b 0a20 2020 2263 656c    },.  {.   "cel
-00002150: 6c5f 7479 7065 223a 2022 636f 6465 222c  l_type": "code",
-00002160: 0a20 2020 2265 7865 6375 7469 6f6e 5f63  .   "execution_c
-00002170: 6f75 6e74 223a 206e 756c 6c2c 0a20 2020  ount": null,.   
-00002180: 226d 6574 6164 6174 6122 3a20 7b0a 2020  "metadata": {.  
-00002190: 2020 2263 6f6c 6c61 7073 6564 223a 2066    "collapsed": f
-000021a0: 616c 7365 2c0a 2020 2020 226a 7570 7974  alse,.    "jupyt
-000021b0: 6572 223a 207b 0a20 2020 2020 226f 7574  er": {.     "out
-000021c0: 7075 7473 5f68 6964 6465 6e22 3a20 6661  puts_hidden": fa
-000021d0: 6c73 650a 2020 2020 7d2c 0a20 2020 2022  lse.    },.    "
-000021e0: 7079 6368 6172 6d22 3a20 7b0a 2020 2020  pycharm": {.    
-000021f0: 2022 6e61 6d65 223a 2022 2325 255c 6e22   "name": "#%%\n"
-00002200: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
-00002210: 226f 7574 7075 7473 223a 205b 5d2c 0a20  "outputs": [],. 
-00002220: 2020 2273 6f75 7263 6522 3a20 5b0a 2020    "source": [.  
-00002230: 2020 2255 5473 6974 6573 203d 206e 7769    "UTsites = nwi
-00002240: 732e 7768 6174 5f73 6974 6573 2873 7461  s.what_sites(sta
-00002250: 7465 4364 3d27 5554 272c 206f 7574 7075  teCd='UT', outpu
-00002260: 7444 6174 6154 7970 6543 643d 2764 7627  tDataTypeCd='dv'
-00002270: 2c20 7374 6172 7444 543d 2731 3937 312d  , startDT='1971-
-00002280: 3037 2d30 3127 2c20 656e 6444 543d 2732  07-01', endDT='2
-00002290: 3032 312d 3037 2d32 3827 295c 6e22 2c0a  021-07-28')\n",.
-000022a0: 2020 2020 2264 6973 706c 6179 2855 5473      "display(UTs
-000022b0: 6974 6573 5b30 5d29 220a 2020 205d 0a20  ites[0])".   ]. 
-000022c0: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
-000022d0: 5f74 7970 6522 3a20 226d 6172 6b64 6f77  _type": "markdow
-000022e0: 6e22 2c0a 2020 2022 6d65 7461 6461 7461  n",.   "metadata
-000022f0: 223a 207b 7d2c 0a20 2020 2273 6f75 7263  ": {},.   "sourc
-00002300: 6522 3a20 5b0a 2020 2020 2223 2323 2320  e": [.    "#### 
-00002310: 4578 616d 706c 6520 353a 2052 6574 7269  Example 5: Retri
-00002320: 6576 6520 7369 7465 2069 6e66 6f72 6d61  eve site informa
-00002330: 7469 6f6e 2066 6f72 2061 2073 696e 676c  tion for a singl
-00002340: 6520 7369 7465 2061 6e64 2073 686f 7720  e site and show 
-00002350: 7468 6520 7365 7269 6573 2063 6174 616c  the series catal
-00002360: 6f67 206f 7574 7075 745c 6e22 2c0a 2020  og output\n",.  
-00002370: 2020 225c 6e22 2c0a 2020 2020 2254 6865    "\n",.    "The
-00002380: 2073 6572 6965 7320 6361 7461 6c6f 6720   series catalog 
-00002390: 6f75 7470 7574 2069 7320 6120 6c69 7374  output is a list
-000023a0: 206f 6620 7468 6520 7061 7261 6d65 7465   of the paramete
-000023b0: 7273 2074 6861 7420 6861 7665 2062 6565  rs that have bee
-000023c0: 6e20 636f 6c6c 6563 7465 6420 6174 2074  n collected at t
-000023d0: 6861 7420 7369 7465 220a 2020 205d 0a20  hat site".   ]. 
-000023e0: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
-000023f0: 5f74 7970 6522 3a20 2263 6f64 6522 2c0a  _type": "code",.
-00002400: 2020 2022 6578 6563 7574 696f 6e5f 636f     "execution_co
-00002410: 756e 7422 3a20 6e75 6c6c 2c0a 2020 2022  unt": null,.   "
-00002420: 6d65 7461 6461 7461 223a 207b 7d2c 0a20  metadata": {},. 
-00002430: 2020 226f 7574 7075 7473 223a 205b 5d2c    "outputs": [],
-00002440: 0a20 2020 2273 6f75 7263 6522 3a20 5b0a  .   "source": [.
-00002450: 2020 2020 226f 6e65 5369 7465 203d 206e      "oneSite = n
-00002460: 7769 732e 7768 6174 5f73 6974 6573 2873  wis.what_sites(s
-00002470: 6974 6573 3d27 3035 3131 3430 3030 272c  ites='05114000',
-00002480: 2073 6572 6965 7343 6174 616c 6f67 4f75   seriesCatalogOu
-00002490: 7470 7574 3d27 7472 7565 2729 5c6e 222c  tput='true')\n",
-000024a0: 0a20 2020 2022 6469 7370 6c61 7928 6f6e  .    "display(on
-000024b0: 6553 6974 655b 305d 2922 0a20 2020 5d0a  eSite[0])".   ].
-000024c0: 2020 7d0a 205d 2c0a 2022 6d65 7461 6461    }. ],. "metada
-000024d0: 7461 223a 207b 0a20 2022 6b65 726e 656c  ta": {.  "kernel
-000024e0: 7370 6563 223a 207b 0a20 2020 2264 6973  spec": {.   "dis
-000024f0: 706c 6179 5f6e 616d 6522 3a20 2250 7974  play_name": "Pyt
-00002500: 686f 6e20 3320 2869 7079 6b65 726e 656c  hon 3 (ipykernel
-00002510: 2922 2c0a 2020 2022 6c61 6e67 7561 6765  )",.   "language
-00002520: 223a 2022 7079 7468 6f6e 222c 0a20 2020  ": "python",.   
-00002530: 226e 616d 6522 3a20 2270 7974 686f 6e33  "name": "python3
-00002540: 220a 2020 7d2c 0a20 2022 6c61 6e67 7561  ".  },.  "langua
-00002550: 6765 5f69 6e66 6f22 3a20 7b0a 2020 2022  ge_info": {.   "
-00002560: 636f 6465 6d69 7272 6f72 5f6d 6f64 6522  codemirror_mode"
-00002570: 3a20 7b0a 2020 2020 226e 616d 6522 3a20  : {.    "name": 
-00002580: 2269 7079 7468 6f6e 222c 0a20 2020 2022  "ipython",.    "
-00002590: 7665 7273 696f 6e22 3a20 330a 2020 207d  version": 3.   }
-000025a0: 2c0a 2020 2022 6669 6c65 5f65 7874 656e  ,.   "file_exten
-000025b0: 7369 6f6e 223a 2022 2e70 7922 2c0a 2020  sion": ".py",.  
-000025c0: 2022 6d69 6d65 7479 7065 223a 2022 7465   "mimetype": "te
-000025d0: 7874 2f78 2d70 7974 686f 6e22 2c0a 2020  xt/x-python",.  
-000025e0: 2022 6e61 6d65 223a 2022 7079 7468 6f6e   "name": "python
-000025f0: 222c 0a20 2020 226e 6263 6f6e 7665 7274  ",.   "nbconvert
-00002600: 5f65 7870 6f72 7465 7222 3a20 2270 7974  _exporter": "pyt
-00002610: 686f 6e22 2c0a 2020 2022 7079 676d 656e  hon",.   "pygmen
-00002620: 7473 5f6c 6578 6572 223a 2022 6970 7974  ts_lexer": "ipyt
-00002630: 686f 6e33 222c 0a20 2020 2276 6572 7369  hon3",.   "versi
-00002640: 6f6e 223a 2022 332e 392e 3722 0a20 207d  on": "3.9.7".  }
-00002650: 0a20 7d2c 0a20 226e 6266 6f72 6d61 7422  . },. "nbformat"
-00002660: 3a20 342c 0a20 226e 6266 6f72 6d61 745f  : 4,. "nbformat_
-00002670: 6d69 6e6f 7222 3a20 340a 7d0a            minor": 4.}.
+00001420: 6773 2e67 6f76 2f64 6f63 732f 7369 7465  gs.gov/docs/site
+00001430: 2d73 6572 7669 6365 2f73 6974 652d 7365  -service/site-se
+00001440: 7276 6963 652d 6465 7461 696c 732f 0a20  rvice-details/. 
+00001450: 2020 5d0a 2020 7d2c 0a20 207b 0a20 2020    ].  },.  {.   
+00001460: 2263 656c 6c5f 7479 7065 223a 2022 6d61  "cell_type": "ma
+00001470: 726b 646f 776e 222c 0a20 2020 226d 6574  rkdown",.   "met
+00001480: 6164 6174 6122 3a20 7b7d 2c0a 2020 2022  adata": {},.   "
+00001490: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
+000014a0: 2323 2323 2045 7861 6d70 6c65 2031 3a20  #### Example 1: 
+000014b0: 5265 7472 6965 7665 2069 6e66 6f72 6d61  Retrieve informa
+000014c0: 7469 6f6e 2061 626f 7574 2073 6974 6573  tion about sites
+000014d0: 2069 6e20 4f68 696f 2077 6865 7265 2070   in Ohio where p
+000014e0: 686f 7370 686f 7275 7320 6461 7461 2077  hosphorus data w
+000014f0: 6173 2063 6f6c 6c65 6374 6564 220a 2020  as collected".  
+00001500: 205d 0a20 207d 2c0a 2020 7b0a 2020 2022   ].  },.  {.   "
+00001510: 6365 6c6c 5f74 7970 6522 3a20 2263 6f64  cell_type": "cod
+00001520: 6522 2c0a 2020 2022 6578 6563 7574 696f  e",.   "executio
+00001530: 6e5f 636f 756e 7422 3a20 6e75 6c6c 2c0a  n_count": null,.
+00001540: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
+00001550: 0a20 2020 2022 636f 6c6c 6170 7365 6422  .    "collapsed"
+00001560: 3a20 6661 6c73 652c 0a20 2020 2022 6a75  : false,.    "ju
+00001570: 7079 7465 7222 3a20 7b0a 2020 2020 2022  pyter": {.     "
+00001580: 6f75 7470 7574 735f 6869 6464 656e 223a  outputs_hidden":
+00001590: 2066 616c 7365 0a20 2020 207d 2c0a 2020   false.    },.  
+000015a0: 2020 2270 7963 6861 726d 223a 207b 0a20    "pycharm": {. 
+000015b0: 2020 2020 226e 616d 6522 3a20 2223 2525      "name": "#%%
+000015c0: 5c6e 220a 2020 2020 7d0a 2020 207d 2c0a  \n".    }.   },.
+000015d0: 2020 2022 6f75 7470 7574 7322 3a20 5b5d     "outputs": []
+000015e0: 2c0a 2020 2022 736f 7572 6365 223a 205b  ,.   "source": [
+000015f0: 0a20 2020 2022 7369 7465 4c69 7374 5068  .    "siteListPh
+00001600: 6f73 203d 206e 7769 732e 7768 6174 5f73  os = nwis.what_s
+00001610: 6974 6573 2873 7461 7465 4364 3d5c 224f  ites(stateCd=\"O
+00001620: 485c 222c 2070 6172 616d 6574 6572 4364  H\", parameterCd
+00001630: 3d5c 2230 3036 3635 5c22 2922 0a20 2020  =\"00665\")".   
+00001640: 5d0a 2020 7d2c 0a20 207b 0a20 2020 2263  ].  },.  {.   "c
+00001650: 656c 6c5f 7479 7065 223a 2022 6d61 726b  ell_type": "mark
+00001660: 646f 776e 222c 0a20 2020 226d 6574 6164  down",.   "metad
+00001670: 6174 6122 3a20 7b7d 2c0a 2020 2022 736f  ata": {},.   "so
+00001680: 7572 6365 223a 205b 0a20 2020 2022 2323  urce": [.    "##
+00001690: 2320 496e 7465 7270 7265 7469 6e67 2074  # Interpreting t
+000016a0: 6865 2052 6573 756c 745c 6e22 2c0a 2020  he Result\n",.  
+000016b0: 2020 225c 6e22 2c0a 2020 2020 2254 6865    "\n",.    "The
+000016c0: 2072 6573 756c 7420 6f66 2063 616c 6c69   result of calli
+000016d0: 6e67 2074 6865 2060 7768 6174 5f73 6974  ng the `what_sit
+000016e0: 6573 2829 6020 6675 6e63 7469 6f6e 2069  es()` function i
+000016f0: 7320 616e 206f 626a 6563 7420 7468 6174  s an object that
+00001700: 2063 6f6e 7461 696e 7320 6120 5061 6e64   contains a Pand
+00001710: 6173 2064 6174 6120 6672 616d 6520 6f62  as data frame ob
+00001720: 6a65 6374 2061 6e64 2061 6e20 6173 736f  ject and an asso
+00001730: 6369 6174 6564 206d 6574 6164 6174 6120  ciated metadata 
+00001740: 6f62 6a65 6374 2e20 5468 6520 5061 6e64  object. The Pand
+00001750: 6173 2064 6174 6120 6672 616d 6520 636f  as data frame co
+00001760: 6e74 6169 6e73 2074 6865 2072 6571 7565  ntains the reque
+00001770: 7374 6573 2073 6974 6520 696e 7665 6e74  stes site invent
+00001780: 6f72 7920 6461 7461 2e5c 6e22 2c0a 2020  ory data.\n",.  
+00001790: 2020 225c 6e22 2c0a 2020 2020 224f 6e63    "\n",.    "Onc
+000017a0: 6520 796f 7527 7665 2067 6f74 2074 6865  e you've got the
+000017b0: 2064 6174 6120 6672 616d 652c 2074 6865   data frame, the
+000017c0: 7265 2773 2073 6576 6572 616c 2075 7365  re's several use
+000017d0: 6675 6c20 7468 696e 6773 2079 6f75 2063  ful things you c
+000017e0: 616e 2064 6f20 746f 2065 7870 6c6f 7265  an do to explore
+000017f0: 2074 6865 2064 6174 612e 220a 2020 205d   the data.".   ]
+00001800: 0a20 207d 2c0a 2020 7b0a 2020 2022 6365  .  },.  {.   "ce
+00001810: 6c6c 5f74 7970 6522 3a20 2263 6f64 6522  ll_type": "code"
+00001820: 2c0a 2020 2022 6578 6563 7574 696f 6e5f  ,.   "execution_
+00001830: 636f 756e 7422 3a20 6e75 6c6c 2c0a 2020  count": null,.  
+00001840: 2022 6d65 7461 6461 7461 223a 207b 0a20   "metadata": {. 
+00001850: 2020 2022 636f 6c6c 6170 7365 6422 3a20     "collapsed": 
+00001860: 6661 6c73 652c 0a20 2020 2022 6a75 7079  false,.    "jupy
+00001870: 7465 7222 3a20 7b0a 2020 2020 2022 6f75  ter": {.     "ou
+00001880: 7470 7574 735f 6869 6464 656e 223a 2066  tputs_hidden": f
+00001890: 616c 7365 0a20 2020 207d 2c0a 2020 2020  alse.    },.    
+000018a0: 2270 7963 6861 726d 223a 207b 0a20 2020  "pycharm": {.   
+000018b0: 2020 226e 616d 6522 3a20 2223 2525 5c6e    "name": "#%%\n
+000018c0: 220a 2020 2020 7d0a 2020 207d 2c0a 2020  ".    }.   },.  
+000018d0: 2022 6f75 7470 7574 7322 3a20 5b5d 2c0a   "outputs": [],.
+000018e0: 2020 2022 736f 7572 6365 223a 205b 0a20     "source": [. 
+000018f0: 2020 2022 2320 4469 7370 6c61 7920 7468     "# Display th
+00001900: 6520 6461 7461 2066 7261 6d65 2061 7320  e data frame as 
+00001910: 6120 7461 626c 655c 6e22 2c0a 2020 2020  a table\n",.    
+00001920: 2264 6973 706c 6179 2873 6974 654c 6973  "display(siteLis
+00001930: 7450 686f 735b 305d 2922 0a20 2020 5d0a  tPhos[0])".   ].
+00001940: 2020 7d2c 0a20 207b 0a20 2020 2263 656c    },.  {.   "cel
+00001950: 6c5f 7479 7065 223a 2022 6d61 726b 646f  l_type": "markdo
+00001960: 776e 222c 0a20 2020 226d 6574 6164 6174  wn",.   "metadat
+00001970: 6122 3a20 7b0a 2020 2020 2270 7963 6861  a": {.    "pycha
+00001980: 726d 223a 207b 0a20 2020 2020 226e 616d  rm": {.     "nam
+00001990: 6522 3a20 2223 2525 206d 645c 6e22 0a20  e": "#%% md\n". 
+000019a0: 2020 207d 0a20 2020 7d2c 0a20 2020 2273     }.   },.   "s
+000019b0: 6f75 7263 6522 3a20 5b0a 2020 2020 2254  ource": [.    "T
+000019c0: 6865 206f 7468 6572 2070 6172 7420 6f66  he other part of
+000019d0: 2074 6865 2072 6573 756c 7420 7265 7475   the result retu
+000019e0: 726e 6564 2066 726f 6d20 7468 6520 6077  rned from the `w
+000019f0: 6861 745f 7369 7465 7328 2960 2066 756e  hat_sites()` fun
+00001a00: 6374 696f 6e20 6973 2061 206d 6574 6164  ction is a metad
+00001a10: 6174 6120 6f62 6a65 6374 2074 6861 7420  ata object that 
+00001a20: 636f 6e74 6169 6e73 2069 6e66 6f72 6d61  contains informa
+00001a30: 7469 6f6e 2061 626f 7574 2074 6865 2071  tion about the q
+00001a40: 7565 7279 2074 6861 7420 7761 7320 6578  uery that was ex
+00001a50: 6563 7574 6564 2074 6f20 7265 7475 726e  ecuted to return
+00001a60: 2074 6865 2064 6174 612e 2046 6f72 2065   the data. For e
+00001a70: 7861 6d70 6c65 2c20 796f 7520 6361 6e20  xample, you can 
+00001a80: 6163 6365 7373 2074 6865 2055 524c 2074  access the URL t
+00001a90: 6861 7420 7761 7320 6173 7365 6d62 6c65  hat was assemble
+00001aa0: 6420 746f 2072 6574 7269 6576 6520 7468  d to retrieve th
+00001ab0: 6520 7265 7175 6573 7465 6420 6461 7461  e requested data
+00001ac0: 2066 726f 6d20 7468 6520 5553 4753 2077   from the USGS w
+00001ad0: 6562 2073 6572 7669 6365 2e20 5468 6520  eb service. The 
+00001ae0: 5553 4753 2077 6562 2073 6572 7669 6365  USGS web service
+00001af0: 2072 6573 706f 6e73 6573 2063 6f6e 7461   responses conta
+00001b00: 696e 2061 2064 6573 6372 6970 7469 7665  in a descriptive
+00001b10: 2068 6561 6465 7220 7468 6174 2064 6566   header that def
+00001b20: 696e 6573 2061 6e64 2063 616e 2062 6520  ines and can be 
+00001b30: 6865 6c70 6675 6c20 696e 2069 6e74 6572  helpful in inter
+00001b40: 7072 6574 696e 6720 7468 6520 636f 6e74  preting the cont
+00001b50: 656e 7473 206f 6620 7468 6520 7265 7370  ents of the resp
+00001b60: 6f6e 7365 2e22 0a20 2020 5d0a 2020 7d2c  onse.".   ].  },
+00001b70: 0a20 207b 0a20 2020 2263 656c 6c5f 7479  .  {.   "cell_ty
+00001b80: 7065 223a 2022 636f 6465 222c 0a20 2020  pe": "code",.   
+00001b90: 2265 7865 6375 7469 6f6e 5f63 6f75 6e74  "execution_count
+00001ba0: 223a 206e 756c 6c2c 0a20 2020 226d 6574  ": null,.   "met
+00001bb0: 6164 6174 6122 3a20 7b0a 2020 2020 2263  adata": {.    "c
+00001bc0: 6f6c 6c61 7073 6564 223a 2066 616c 7365  ollapsed": false
+00001bd0: 2c0a 2020 2020 226a 7570 7974 6572 223a  ,.    "jupyter":
+00001be0: 207b 0a20 2020 2020 226f 7574 7075 7473   {.     "outputs
+00001bf0: 5f68 6964 6465 6e22 3a20 6661 6c73 650a  _hidden": false.
+00001c00: 2020 2020 7d2c 0a20 2020 2022 7079 6368      },.    "pych
+00001c10: 6172 6d22 3a20 7b0a 2020 2020 2022 6e61  arm": {.     "na
+00001c20: 6d65 223a 2022 2325 255c 6e22 0a20 2020  me": "#%%\n".   
+00001c30: 207d 0a20 2020 7d2c 0a20 2020 226f 7574   }.   },.   "out
+00001c40: 7075 7473 223a 205b 5d2c 0a20 2020 2273  puts": [],.   "s
+00001c50: 6f75 7263 6522 3a20 5b0a 2020 2020 2270  ource": [.    "p
+00001c60: 7269 6e74 2827 5468 6520 7175 6572 7920  rint('The query 
+00001c70: 5552 4c20 7573 6564 2074 6f20 7265 7472  URL used to retr
+00001c80: 6965 7665 2074 6865 2064 6174 6120 6672  ieve the data fr
+00001c90: 6f6d 204e 5749 5320 7761 733a 2027 202b  om NWIS was: ' +
+00001ca0: 2073 6974 654c 6973 7450 686f 735b 315d   siteListPhos[1]
+00001cb0: 2e75 726c 2922 0a20 2020 5d0a 2020 7d2c  .url)".   ].  },
+00001cc0: 0a20 207b 0a20 2020 2263 656c 6c5f 7479  .  {.   "cell_ty
+00001cd0: 7065 223a 2022 6d61 726b 646f 776e 222c  pe": "markdown",
+00001ce0: 0a20 2020 226d 6574 6164 6174 6122 3a20  .   "metadata": 
+00001cf0: 7b7d 2c0a 2020 2022 736f 7572 6365 223a  {},.   "source":
+00001d00: 205b 0a20 2020 2022 2323 2320 4164 6469   [.    "### Addi
+00001d10: 7469 6f6e 616c 2045 7861 6d70 6c65 735c  tional Examples\
+00001d20: 6e22 2c0a 2020 2020 225c 6e22 2c0a 2020  n",.    "\n",.  
+00001d30: 2020 2223 2323 2320 4578 616d 706c 6520    "#### Example 
+00001d40: 323a 2052 6574 7269 6576 6520 7369 7465  2: Retrieve site
+00001d50: 2069 6e66 6f72 6d61 7469 6f6e 2066 6f72   information for
+00001d60: 2061 2073 696e 676c 6520 7369 7465 220a   a single site".
+00001d70: 2020 205d 0a20 207d 2c0a 2020 7b0a 2020     ].  },.  {.  
+00001d80: 2022 6365 6c6c 5f74 7970 6522 3a20 2263   "cell_type": "c
+00001d90: 6f64 6522 2c0a 2020 2022 6578 6563 7574  ode",.   "execut
+00001da0: 696f 6e5f 636f 756e 7422 3a20 6e75 6c6c  ion_count": null
+00001db0: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
+00001dc0: 207b 0a20 2020 2022 636f 6c6c 6170 7365   {.    "collapse
+00001dd0: 6422 3a20 6661 6c73 652c 0a20 2020 2022  d": false,.    "
+00001de0: 6a75 7079 7465 7222 3a20 7b0a 2020 2020  jupyter": {.    
+00001df0: 2022 6f75 7470 7574 735f 6869 6464 656e   "outputs_hidden
+00001e00: 223a 2066 616c 7365 0a20 2020 207d 2c0a  ": false.    },.
+00001e10: 2020 2020 2270 7963 6861 726d 223a 207b      "pycharm": {
+00001e20: 0a20 2020 2020 226e 616d 6522 3a20 2223  .     "name": "#
+00001e30: 2525 5c6e 220a 2020 2020 7d0a 2020 207d  %%\n".    }.   }
+00001e40: 2c0a 2020 2022 6f75 7470 7574 7322 3a20  ,.   "outputs": 
+00001e50: 5b5d 2c0a 2020 2022 736f 7572 6365 223a  [],.   "source":
+00001e60: 205b 0a20 2020 2022 6f6e 6553 6974 6520   [.    "oneSite 
+00001e70: 3d20 6e77 6973 2e77 6861 745f 7369 7465  = nwis.what_site
+00001e80: 7328 7369 7465 733d 2730 3531 3134 3030  s(sites='0511400
+00001e90: 3027 295c 6e22 2c0a 2020 2020 2264 6973  0')\n",.    "dis
+00001ea0: 706c 6179 286f 6e65 5369 7465 5b30 5d29  play(oneSite[0])
+00001eb0: 220a 2020 205d 0a20 207d 2c0a 2020 7b0a  ".   ].  },.  {.
+00001ec0: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
+00001ed0: 226d 6172 6b64 6f77 6e22 2c0a 2020 2022  "markdown",.   "
+00001ee0: 6d65 7461 6461 7461 223a 207b 7d2c 0a20  metadata": {},. 
+00001ef0: 2020 2273 6f75 7263 6522 3a20 5b0a 2020    "source": [.  
+00001f00: 2020 2223 2323 2320 4578 616d 706c 6520    "#### Example 
+00001f10: 333a 2052 6574 7269 6576 6520 7369 7465  3: Retrieve site
+00001f20: 2069 6e66 6f72 6d61 7469 6f6e 2066 6f72   information for
+00001f30: 2061 2073 696e 676c 6520 7369 7465 2061   a single site a
+00001f40: 6e64 2073 686f 7720 7468 6520 7265 7375  nd show the resu
+00001f50: 6c74 2077 6974 6820 6578 7061 6e64 6564  lt with expanded
+00001f60: 206f 7574 7075 7422 0a20 2020 5d0a 2020   output".   ].  
+00001f70: 7d2c 0a20 207b 0a20 2020 2263 656c 6c5f  },.  {.   "cell_
+00001f80: 7479 7065 223a 2022 636f 6465 222c 0a20  type": "code",. 
+00001f90: 2020 2265 7865 6375 7469 6f6e 5f63 6f75    "execution_cou
+00001fa0: 6e74 223a 206e 756c 6c2c 0a20 2020 226d  nt": null,.   "m
+00001fb0: 6574 6164 6174 6122 3a20 7b7d 2c0a 2020  etadata": {},.  
+00001fc0: 2022 6f75 7470 7574 7322 3a20 5b5d 2c0a   "outputs": [],.
+00001fd0: 2020 2022 736f 7572 6365 223a 205b 0a20     "source": [. 
+00001fe0: 2020 2022 6f6e 6553 6974 6520 3d20 6e77     "oneSite = nw
+00001ff0: 6973 2e77 6861 745f 7369 7465 7328 7369  is.what_sites(si
+00002000: 7465 733d 2730 3531 3134 3030 3027 2c20  tes='05114000', 
+00002010: 7369 7465 4f75 7470 7574 3d27 6578 7061  siteOutput='expa
+00002020: 6e64 6564 2729 5c6e 222c 0a20 2020 2022  nded')\n",.    "
+00002030: 6469 7370 6c61 7928 6f6e 6553 6974 655b  display(oneSite[
+00002040: 305d 2922 0a20 2020 5d0a 2020 7d2c 0a20  0])".   ].  },. 
+00002050: 207b 0a20 2020 2263 656c 6c5f 7479 7065   {.   "cell_type
+00002060: 223a 2022 6d61 726b 646f 776e 222c 0a20  ": "markdown",. 
+00002070: 2020 226d 6574 6164 6174 6122 3a20 7b0a    "metadata": {.
+00002080: 2020 2020 2270 7963 6861 726d 223a 207b      "pycharm": {
+00002090: 0a20 2020 2020 226e 616d 6522 3a20 2223  .     "name": "#
+000020a0: 2525 206d 645c 6e22 0a20 2020 207d 0a20  %% md\n".    }. 
+000020b0: 2020 7d2c 0a20 2020 2273 6f75 7263 6522    },.   "source"
+000020c0: 3a20 5b0a 2020 2020 2223 2323 2320 4578  : [.    "#### Ex
+000020d0: 616d 706c 6520 343a 2052 6574 7269 6576  ample 4: Retriev
+000020e0: 6520 7369 7465 2069 6e66 6f72 6d61 7469  e site informati
+000020f0: 6f6e 2066 6f72 2073 6974 6573 2069 6e20  on for sites in 
+00002100: 5574 6168 2077 6974 6820 6461 696c 7920  Utah with daily 
+00002110: 7661 6c75 6573 2064 6174 6120 6661 6c6c  values data fall
+00002120: 696e 6720 7769 7468 696e 2061 2073 7065  ing within a spe
+00002130: 6369 6669 6564 2064 6174 6520 7261 6e67  cified date rang
+00002140: 6522 0a20 2020 5d0a 2020 7d2c 0a20 207b  e".   ].  },.  {
+00002150: 0a20 2020 2263 656c 6c5f 7479 7065 223a  .   "cell_type":
+00002160: 2022 636f 6465 222c 0a20 2020 2265 7865   "code",.   "exe
+00002170: 6375 7469 6f6e 5f63 6f75 6e74 223a 206e  cution_count": n
+00002180: 756c 6c2c 0a20 2020 226d 6574 6164 6174  ull,.   "metadat
+00002190: 6122 3a20 7b0a 2020 2020 2263 6f6c 6c61  a": {.    "colla
+000021a0: 7073 6564 223a 2066 616c 7365 2c0a 2020  psed": false,.  
+000021b0: 2020 226a 7570 7974 6572 223a 207b 0a20    "jupyter": {. 
+000021c0: 2020 2020 226f 7574 7075 7473 5f68 6964      "outputs_hid
+000021d0: 6465 6e22 3a20 6661 6c73 650a 2020 2020  den": false.    
+000021e0: 7d2c 0a20 2020 2022 7079 6368 6172 6d22  },.    "pycharm"
+000021f0: 3a20 7b0a 2020 2020 2022 6e61 6d65 223a  : {.     "name":
+00002200: 2022 2325 255c 6e22 0a20 2020 207d 0a20   "#%%\n".    }. 
+00002210: 2020 7d2c 0a20 2020 226f 7574 7075 7473    },.   "outputs
+00002220: 223a 205b 5d2c 0a20 2020 2273 6f75 7263  ": [],.   "sourc
+00002230: 6522 3a20 5b0a 2020 2020 2255 5473 6974  e": [.    "UTsit
+00002240: 6573 203d 206e 7769 732e 7768 6174 5f73  es = nwis.what_s
+00002250: 6974 6573 2873 7461 7465 4364 3d27 5554  ites(stateCd='UT
+00002260: 272c 206f 7574 7075 7444 6174 6154 7970  ', outputDataTyp
+00002270: 6543 643d 2764 7627 2c20 7374 6172 7444  eCd='dv', startD
+00002280: 543d 2731 3937 312d 3037 2d30 3127 2c20  T='1971-07-01', 
+00002290: 656e 6444 543d 2732 3032 312d 3037 2d32  endDT='2021-07-2
+000022a0: 3827 295c 6e22 2c0a 2020 2020 2264 6973  8')\n",.    "dis
+000022b0: 706c 6179 2855 5473 6974 6573 5b30 5d29  play(UTsites[0])
+000022c0: 220a 2020 205d 0a20 207d 2c0a 2020 7b0a  ".   ].  },.  {.
+000022d0: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
+000022e0: 226d 6172 6b64 6f77 6e22 2c0a 2020 2022  "markdown",.   "
+000022f0: 6d65 7461 6461 7461 223a 207b 7d2c 0a20  metadata": {},. 
+00002300: 2020 2273 6f75 7263 6522 3a20 5b0a 2020    "source": [.  
+00002310: 2020 2223 2323 2320 4578 616d 706c 6520    "#### Example 
+00002320: 353a 2052 6574 7269 6576 6520 7369 7465  5: Retrieve site
+00002330: 2069 6e66 6f72 6d61 7469 6f6e 2066 6f72   information for
+00002340: 2061 2073 696e 676c 6520 7369 7465 2061   a single site a
+00002350: 6e64 2073 686f 7720 7468 6520 7365 7269  nd show the seri
+00002360: 6573 2063 6174 616c 6f67 206f 7574 7075  es catalog outpu
+00002370: 745c 6e22 2c0a 2020 2020 225c 6e22 2c0a  t\n",.    "\n",.
+00002380: 2020 2020 2254 6865 2073 6572 6965 7320      "The series 
+00002390: 6361 7461 6c6f 6720 6f75 7470 7574 2069  catalog output i
+000023a0: 7320 6120 6c69 7374 206f 6620 7468 6520  s a list of the 
+000023b0: 7061 7261 6d65 7465 7273 2074 6861 7420  parameters that 
+000023c0: 6861 7665 2062 6565 6e20 636f 6c6c 6563  have been collec
+000023d0: 7465 6420 6174 2074 6861 7420 7369 7465  ted at that site
+000023e0: 220a 2020 205d 0a20 207d 2c0a 2020 7b0a  ".   ].  },.  {.
+000023f0: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
+00002400: 2263 6f64 6522 2c0a 2020 2022 6578 6563  "code",.   "exec
+00002410: 7574 696f 6e5f 636f 756e 7422 3a20 6e75  ution_count": nu
+00002420: 6c6c 2c0a 2020 2022 6d65 7461 6461 7461  ll,.   "metadata
+00002430: 223a 207b 7d2c 0a20 2020 226f 7574 7075  ": {},.   "outpu
+00002440: 7473 223a 205b 5d2c 0a20 2020 2273 6f75  ts": [],.   "sou
+00002450: 7263 6522 3a20 5b0a 2020 2020 226f 6e65  rce": [.    "one
+00002460: 5369 7465 203d 206e 7769 732e 7768 6174  Site = nwis.what
+00002470: 5f73 6974 6573 2873 6974 6573 3d27 3035  _sites(sites='05
+00002480: 3131 3430 3030 272c 2073 6572 6965 7343  114000', seriesC
+00002490: 6174 616c 6f67 4f75 7470 7574 3d27 7472  atalogOutput='tr
+000024a0: 7565 2729 5c6e 222c 0a20 2020 2022 6469  ue')\n",.    "di
+000024b0: 7370 6c61 7928 6f6e 6553 6974 655b 305d  splay(oneSite[0]
+000024c0: 2922 0a20 2020 5d0a 2020 7d0a 205d 2c0a  )".   ].  }. ],.
+000024d0: 2022 6d65 7461 6461 7461 223a 207b 0a20   "metadata": {. 
+000024e0: 2022 6b65 726e 656c 7370 6563 223a 207b   "kernelspec": {
+000024f0: 0a20 2020 2264 6973 706c 6179 5f6e 616d  .   "display_nam
+00002500: 6522 3a20 2250 7974 686f 6e20 3320 2869  e": "Python 3 (i
+00002510: 7079 6b65 726e 656c 2922 2c0a 2020 2022  pykernel)",.   "
+00002520: 6c61 6e67 7561 6765 223a 2022 7079 7468  language": "pyth
+00002530: 6f6e 222c 0a20 2020 226e 616d 6522 3a20  on",.   "name": 
+00002540: 2270 7974 686f 6e33 220a 2020 7d2c 0a20  "python3".  },. 
+00002550: 2022 6c61 6e67 7561 6765 5f69 6e66 6f22   "language_info"
+00002560: 3a20 7b0a 2020 2022 636f 6465 6d69 7272  : {.   "codemirr
+00002570: 6f72 5f6d 6f64 6522 3a20 7b0a 2020 2020  or_mode": {.    
+00002580: 226e 616d 6522 3a20 2269 7079 7468 6f6e  "name": "ipython
+00002590: 222c 0a20 2020 2022 7665 7273 696f 6e22  ",.    "version"
+000025a0: 3a20 330a 2020 207d 2c0a 2020 2022 6669  : 3.   },.   "fi
+000025b0: 6c65 5f65 7874 656e 7369 6f6e 223a 2022  le_extension": "
+000025c0: 2e70 7922 2c0a 2020 2022 6d69 6d65 7479  .py",.   "mimety
+000025d0: 7065 223a 2022 7465 7874 2f78 2d70 7974  pe": "text/x-pyt
+000025e0: 686f 6e22 2c0a 2020 2022 6e61 6d65 223a  hon",.   "name":
+000025f0: 2022 7079 7468 6f6e 222c 0a20 2020 226e   "python",.   "n
+00002600: 6263 6f6e 7665 7274 5f65 7870 6f72 7465  bconvert_exporte
+00002610: 7222 3a20 2270 7974 686f 6e22 2c0a 2020  r": "python",.  
+00002620: 2022 7079 676d 656e 7473 5f6c 6578 6572   "pygments_lexer
+00002630: 223a 2022 6970 7974 686f 6e33 222c 0a20  ": "ipython3",. 
+00002640: 2020 2276 6572 7369 6f6e 223a 2022 332e    "version": "3.
+00002650: 392e 3722 0a20 207d 0a20 7d2c 0a20 226e  9.7".  }. },. "n
+00002660: 6266 6f72 6d61 7422 3a20 342c 0a20 226e  bformat": 4,. "n
+00002670: 6266 6f72 6d61 745f 6d69 6e6f 7222 3a20  bformat_minor": 
+00002680: 340a 7d0a                                4.}.
```

### Comparing `dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb` & `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb` & `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb` & `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb` & `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/docs/Makefile` & `dataretrieval-1.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/docs/source/conf.py` & `dataretrieval-1.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/docs/source/examples/datasets/peak_discharge_trends.csv` & `dataretrieval-1.0.7/docs/source/examples/datasets/peak_discharge_trends.csv`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/docs/source/examples/index.rst` & `dataretrieval-1.0.7/docs/source/examples/index.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/docs/source/examples/readme_examples.rst` & `dataretrieval-1.0.7/docs/source/examples/readme_examples.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/docs/source/examples/siteinfo_examples.rst` & `dataretrieval-1.0.7/docs/source/examples/siteinfo_examples.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ``seriesCatalogOutput`` that can be set to "True" if you wish to retrieve the
 detailed period of record information for a site instead. Refer to the
 `NWIS water services documentation`_ for additional information. The below
 example illustrates the use of the ``seriesCatalogOutput`` switch and displays
 the resulting column names for the output dataframes (example prompted by
 `GitHub Issue #34`_).
 
-.. _NWIS water services documentation: https://nwis.waterservices.usgs.gov/rest/Site-Service.html
+.. _NWIS water services documentation: https://waterservices.usgs.gov/docs/site-service/site-service-details/
 
 .. _GitHub Issue #34: https://github.com/DOI-USGS/dataretrieval-python/issues/34
 
 .. doctest::
 
     # first import the functions for downloading data from NWIS
     >>> import dataretrieval.nwis as nwis
```

### Comparing `dataretrieval-1.0.6/docs/source/index.rst` & `dataretrieval-1.0.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/docs/source/meta/contributing.rst` & `dataretrieval-1.0.7/docs/source/meta/contributing.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/docs/source/meta/installing.rst` & `dataretrieval-1.0.7/docs/source/meta/installing.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/docs/source/meta/license.rst` & `dataretrieval-1.0.7/docs/source/meta/license.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/docs/source/userguide/dataportals.rst` & `dataretrieval-1.0.7/docs/source/userguide/dataportals.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/docs/source/userguide/timeconventions.rst` & `dataretrieval-1.0.7/docs/source/userguide/timeconventions.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/pyproject.toml` & `dataretrieval-1.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,37 +7,51 @@
 description = "Discover and retrieve water data from U.S. federal hydrologic web services."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["USGS", "water data"]
 license = {file = "LICENSE.md"}
 maintainers = [
   {name = "Timothy Hodson", email = "thodson@usgs.gov"},
-  {name = "Jayaram Hariharan", email = "jhariharan@usgs.gov"},
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "requests",
-    "pandas",
+    "pandas==2.*",
 ]
 dynamic = ["version"]
 
 [tool.setuptools]
 packages = ["dataretrieval", "dataretrieval.codes"]
 
 [project.optional-dependencies]
 test = [
   "pytest > 5.0.0",
-  "pytest-cov[all]"
+  "pytest-cov[all]",
+  "coverage",
+  "requests-mock",
+  "flake8",
 ]
 doc = [
   "sphinx",
+  "sphinx_rtd_theme",
+  "nbsphinx",
+  "nbsphinx_link",
+]
+nldi = [
+  'geopandas>=0.10'
 ]
 
 [project.urls]
 homepage = "https://github.com/DOI-USGS/dataretrieval-python"
 documentation = "https://doi-usgs.github.io/dataretrieval-python/"
 repository = "https://github.com/DOI-USGS/dataretrieval-python.git"
 
 [tool.setuptools_scm]
 write_to = "dataretrieval/_version.py"
+
+[tool.isort]
+profile = "black"
+
+[tool.black]
+skip-string-normalization = true
```

### Comparing `dataretrieval-1.0.6/tests/data/nwis_sites.txt` & `dataretrieval-1.0.7/tests/data/nwis_sites.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # retrieved: 2020-03-06 11:23:28 -05:00	(caas01)
 #
 # The Site File stores location and general information about groundwater,
 # surface water, and meteorological sites
 # for sites in USA.
 #
 # File-format description:  http://help.waterdata.usgs.gov/faq/about-tab-delimited-output
-# Automated-retrieval info: http://waterservices.usgs.gov/rest/Site-Service.html
+# Automated-retrieval info: https://waterservices.usgs.gov/docs/site-service/site-service-details/
 #
 # Contact:   gs-w_support_nwisweb@usgs.gov
 # Warning: A site search criterion has been used for which the data may be unavailable.
 #
 # The following selected fields are included in this output:
 #
 #  agency_cd       -- Agency
```

### Comparing `dataretrieval-1.0.6/tests/data/water_use_allegheny.txt` & `dataretrieval-1.0.7/tests/data/water_use_allegheny.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/water_use_national.txt` & `dataretrieval-1.0.7/tests/data/water_use_national.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/waterdata_measurements.txt` & `dataretrieval-1.0.7/tests/data/waterdata_measurements.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/waterdata_qwdata.txt` & `dataretrieval-1.0.7/tests/data/waterdata_qwdata.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/waterservices_dv.txt` & `dataretrieval-1.0.7/tests/data/waterservices_dv.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/waterservices_gwlevels.txt` & `dataretrieval-1.0.7/tests/data/waterservices_gwlevels.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/waterservices_iv.txt` & `dataretrieval-1.0.7/tests/data/waterservices_iv.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/waterservices_peaks.txt` & `dataretrieval-1.0.7/tests/data/waterservices_peaks.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/waterservices_ratings.txt` & `dataretrieval-1.0.7/tests/data/waterservices_ratings.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/waterservices_site.txt` & `dataretrieval-1.0.7/tests/data/waterservices_site.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # retrieved: 2020-02-14 13:17:02 -05:00	(sdas01)
 #
 # The Site File stores location and general information about groundwater,
 # surface water, and meteorological sites
 # for sites in USA.
 #
 # File-format description:  http://help.waterdata.usgs.gov/faq/about-tab-delimited-output
-# Automated-retrieval info: http://waterservices.usgs.gov/rest/Site-Service.html
+# Automated-retrieval info: https://waterservices.usgs.gov/docs/site-service/site-service-details/
 #
 # Contact:   gs-w_support_nwisweb@usgs.gov
 #
 # The following selected fields are included in this output:
 #
 #  agency_cd       -- Agency
 #  site_no         -- Site identification number
```

### Comparing `dataretrieval-1.0.6/tests/data/waterservices_stats.txt` & `dataretrieval-1.0.7/tests/data/waterservices_stats.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/wqp_activities.txt` & `dataretrieval-1.0.7/tests/data/wqp_activities.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/wqp_activity_metrics.txt` & `dataretrieval-1.0.7/tests/data/wqp_activity_metrics.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/wqp_detection_limits.txt` & `dataretrieval-1.0.7/tests/data/wqp_detection_limits.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/wqp_habitat_metrics.txt` & `dataretrieval-1.0.7/tests/data/wqp_habitat_metrics.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/wqp_organizations.txt` & `dataretrieval-1.0.7/tests/data/wqp_organizations.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/wqp_project_weights.txt` & `dataretrieval-1.0.7/tests/data/wqp_project_weights.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/wqp_projects.txt` & `dataretrieval-1.0.7/tests/data/wqp_projects.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/wqp_results.txt` & `dataretrieval-1.0.7/tests/data/wqp_results.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/data/wqp_sites.txt` & `dataretrieval-1.0.7/tests/data/wqp_sites.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/nadp_test.py` & `dataretrieval-1.0.7/tests/nadp_test.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/nwis_test.py` & `dataretrieval-1.0.7/tests/nwis_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,57 @@
+import datetime
+import unittest.mock as mock
+
 import numpy as np
 import pandas as pd
 import pytest
-import requests
-import datetime
-from dataretrieval.nwis import get_record, preformat_peaks_response, get_info
-from dataretrieval.nwis import what_sites, get_iv, get_dv, get_discharge_peaks
-from dataretrieval.nwis import NWIS_Metadata
-import unittest.mock as mock
 
+from dataretrieval.nwis import NWIS_Metadata
+from dataretrieval.nwis import get_info, get_record, preformat_peaks_response, get_iv, what_sites
 
 START_DATE = '2018-01-24'
-END_DATE   = '2018-01-25'
+END_DATE = '2018-01-25'
 
 DATETIME_COL = 'datetime'
 SITENO_COL = 'site_no'
 
 
 def test_measurements_service():
     """Test measurement service
     """
     start = '2018-01-24'
-    end   = '2018-01-25'
+    end = '2018-01-25'
     service = 'measurements'
     site = '03339000'
     df = get_record(site, start, end, service=service)
     return df
 
+
 def test_measurements_service_answer():
     df = test_measurements_service()
     # check parsing
     assert df.iloc[0]['measurement_nu'] == 801
 
+
 def test_iv_service():
     """Unit test of instantaneous value service
     """
     start = START_DATE
-    end   = END_DATE
+    end = END_DATE
     service = 'iv'
     site = ['03339000', '05447500', '03346500']
     return get_record(site, start, end, service=service)
 
+
 def test_iv_service_answer():
     df = test_iv_service()
     # check multiindex function
     assert df.index.names == [SITENO_COL, DATETIME_COL], "iv service returned incorrect index: {}".format(df.index.names)
 
+
 def test_preformat_peaks_response():
     # make a data frame with a "peak_dt" datetime column
     # it will have some nan and none values
     data = {"peak_dt": ["2000-03-22",
                         np.nan,
                         None],
             "peak_va": [1000,
@@ -59,17 +62,33 @@
     df = pd.DataFrame(data)
     # run preformat function
     df = preformat_peaks_response(df)
     # assertions
     assert 'datetime' in df.columns
     assert df['datetime'].isna().sum() == 0
 
-if __name__=='__main__':
-     test_measurements_service_answer()
-     test_iv_service_answer()
+
+@pytest.mark.parametrize("site_input_type_list", [True, False])
+def test_get_record_site_value_types(site_input_type_list):
+    """Test that get_record method for valid input types for the 'sites' parameter."""
+    start = '2018-01-24'
+    end = '2018-01-25'
+    service = 'measurements'
+    site = '03339000'
+    if site_input_type_list:
+        sites = [site]
+    else:
+        sites = site
+    df = get_record(sites=sites, start=start, end=end, service=service)
+    assert df.iloc[0]['measurement_nu'] == 801
+
+
+if __name__ == '__main__':
+    test_measurements_service_answer()
+    test_iv_service_answer()
 
 
 # tests using real queries to USGS webservices
 # these specific queries represent some edge-cases and the tests to address
 # incomplete date-time information
 
 def test_inc_date_01():
```

### Comparing `dataretrieval-1.0.6/tests/utils_test.py` & `dataretrieval-1.0.7/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.6/tests/waterservices_test.py` & `dataretrieval-1.0.7/tests/waterservices_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,29 @@
-import pytest
-import requests
 import datetime
 
+import pytest
 from pandas import DataFrame
 
-from dataretrieval.nwis import query_waterservices, get_record, query_waterdata, what_sites, get_stats, get_dv, get_iv, \
-    get_info, get_qwdata, get_gwlevels, get_discharge_peaks, get_discharge_measurements, get_pmcodes, get_water_use, \
-    get_ratings
+from dataretrieval.nwis import (
+    get_discharge_measurements,
+    get_discharge_peaks,
+    get_dv,
+    get_gwlevels,
+    get_info,
+    get_iv,
+    get_pmcodes,
+    get_qwdata,
+    get_ratings,
+    get_record,
+    get_stats,
+    get_water_use,
+    query_waterdata,
+    query_waterservices,
+    what_sites
+)
 from dataretrieval.utils import NoSitesError
 
 
 def test_query_waterdata_validation():
     """Tests the validation parameters of the query_waterservices method"""
     with pytest.raises(TypeError) as type_error:
         query_waterdata(service='pmcodes', format='rdb')
@@ -68,29 +81,66 @@
     mock_request(requests_mock, request_url, response_file_path)
     df, md = get_dv(sites=["01491000", "01645000"], start='2020-02-14', end='2020-02-15')
     assert type(df) is DataFrame
     assert df.size == 8
     assert_metadata(requests_mock, request_url, md, site, None, format)
 
 
+@pytest.mark.parametrize("site_input_type_list", [True, False])
+def test_get_dv_site_value_types(requests_mock, site_input_type_list):
+    """Tests get_dv method for valid input types for the 'sites' parameter"""
+    _format = "json"
+    site = '01491000'
+    request_url = 'https://waterservices.usgs.gov/nwis/dv?format={}' \
+                  '&startDT=2020-02-14&endDT=2020-02-15&sites={}'.format(_format, site)
+    response_file_path = 'data/waterservices_dv.txt'
+    mock_request(requests_mock, request_url, response_file_path)
+    if site_input_type_list:
+        sites = [site]
+    else:
+        sites = site
+    df, md = get_dv(sites=sites, start='2020-02-14', end='2020-02-15')
+    assert type(df) is DataFrame
+    assert df.size == 8
+
+
 def test_get_iv(requests_mock):
-    """Tests get_dv method correctly generates the request url and returns the result in a DataFrame"""
+    """Tests get_iv method correctly generates the request url and returns the result in a DataFrame"""
     format = "json"
     site = '01491000%2C01645000'
     request_url = 'https://waterservices.usgs.gov/nwis/iv?format={}' \
                   '&startDT=2019-02-14&endDT=2020-02-15&sites={}'.format(format, site)
     response_file_path = 'data/waterservices_iv.txt'
     mock_request(requests_mock, request_url, response_file_path)
     df, md = get_iv(sites=["01491000", "01645000"], start='2019-02-14', end='2020-02-15')
     assert type(df) is DataFrame
     assert df.size == 563380
     assert md.url == request_url
     assert_metadata(requests_mock, request_url, md, site, None, format)
 
 
+@pytest.mark.parametrize("site_input_type_list", [True, False])
+def test_get_iv_site_value_types(requests_mock, site_input_type_list):
+    """Tests get_iv method for valid input type for the 'sites' parameter"""
+    _format = "json"
+    site = '01491000'
+    request_url = 'https://waterservices.usgs.gov/nwis/iv?format={}' \
+                  '&startDT=2019-02-14&endDT=2020-02-15&sites={}'.format(_format, site)
+    response_file_path = 'data/waterservices_iv.txt'
+    mock_request(requests_mock, request_url, response_file_path)
+    if site_input_type_list:
+        sites = [site]
+    else:
+        sites = site
+    df, md = get_iv(sites=sites, start='2019-02-14', end='2020-02-15')
+    assert type(df) is DataFrame
+    assert df.size == 563380
+    assert md.url == request_url
+
+
 def test_get_info(requests_mock):
     """
     Tests get_info method correctly generates the request url and returns the result in a DataFrame.
     Note that only sites and format are passed as query params
     """
     format = "rdb"
     site = '01491000%2C01645000'
@@ -118,42 +168,101 @@
     with pytest.warns(DeprecationWarning):
         df, md = get_qwdata(sites=["01491000", "01645000"])
     assert type(df) is DataFrame
     assert df.size == 1821472
     assert_metadata(requests_mock, request_url, md, site, None, format)
 
 
+@pytest.mark.parametrize("site_input_type_list", [True, False])
+def test_get_qwdata_site_value_types(requests_mock, site_input_type_list):
+    """Tests get_qwdata method for valid input types for the 'sites' parameter"""
+    _format = "rdb"
+    site = '01491000'
+    request_url = 'https://nwis.waterdata.usgs.gov/nwis/qwdata?site_no={}' \
+                  '&qw_sample_wide=qw_sample_wide&agency_cd=USGS&format={}&pm_cd_compare=Greater+than' \
+                  '&inventory_output=0&rdb_inventory_output=file&TZoutput=0&rdb_qw_attributes=expanded' \
+                  '&date_format=YYYY-MM-DD&rdb_compression=value&submitted_form=brief_list'.format(site, _format)
+    response_file_path = 'data/waterdata_qwdata.txt'
+    mock_request(requests_mock, request_url, response_file_path)
+    if site_input_type_list:
+        sites = [site]
+    else:
+        sites = site
+    with pytest.warns(DeprecationWarning):
+        df, md = get_qwdata(sites=sites)
+    assert type(df) is DataFrame
+    assert df.size == 1821472
+
+
 def test_get_gwlevels(requests_mock):
     """Tests get_gwlevels method correctly generates the request url and returns the result in a DataFrame."""
     format = "rdb"
     site = '434400121275801'
     request_url = 'https://waterservices.usgs.gov/nwis/gwlevels?startDT=1851-01-01' \
                   '&sites={}&format={}'.format(site, format)
     response_file_path = 'data/waterservices_gwlevels.txt'
     mock_request(requests_mock, request_url, response_file_path)
     df, md = get_gwlevels(sites=[site])
     assert type(df) is DataFrame
     assert df.size == 16
     assert_metadata(requests_mock, request_url, md, site, None, format)
 
 
+@pytest.mark.parametrize("site_input_type_list", [True, False])
+def test_get_gwlevels_site_value_types(requests_mock, site_input_type_list):
+    """Tests get_gwlevels method for valid input types for the 'sites' parameter."""
+    _format = "rdb"
+    site = '434400121275801'
+    request_url = 'https://waterservices.usgs.gov/nwis/gwlevels?startDT=1851-01-01' \
+                  '&sites={}&format={}'.format(site, _format)
+    response_file_path = 'data/waterservices_gwlevels.txt'
+    mock_request(requests_mock, request_url, response_file_path)
+    if site_input_type_list:
+        sites = [site]
+    else:
+        sites = site
+    df, md = get_gwlevels(sites=sites)
+    assert type(df) is DataFrame
+    assert df.size == 16
+
+
 def test_get_discharge_peaks(requests_mock):
     """Tests get_discharge_peaks method correctly generates the request url and returns the result in a DataFrame"""
     format = "rdb"
     site = '01594440'
     request_url = 'https://nwis.waterdata.usgs.gov/nwis/peaks?format={}&site_no={}' \
                   '&begin_date=2000-02-14&end_date=2020-02-15'.format(format, site)
     response_file_path = 'data/waterservices_peaks.txt'
     mock_request(requests_mock, request_url, response_file_path)
     df, md = get_discharge_peaks(sites=[site], start='2000-02-14', end='2020-02-15')
     assert type(df) is DataFrame
     assert df.size == 240
     assert_metadata(requests_mock, request_url, md, site, None, format)
 
 
+@pytest.mark.parametrize("site_input_type_list", [True, False])
+def test_get_discharge_peaks_sites_value_types(requests_mock, site_input_type_list):
+    """Tests get_discharge_peaks for valid input types of the 'sites' parameter"""
+
+    _format = "rdb"
+    site = '01594440'
+    request_url = 'https://nwis.waterdata.usgs.gov/nwis/peaks?format={}&site_no={}' \
+                  '&begin_date=2000-02-14&end_date=2020-02-15'.format(_format, site)
+    response_file_path = 'data/waterservices_peaks.txt'
+    mock_request(requests_mock, request_url, response_file_path)
+    if site_input_type_list:
+        sites = [site]
+    else:
+        sites = site
+
+    df, md = get_discharge_peaks(sites=sites, start='2000-02-14', end='2020-02-15')
+    assert type(df) is DataFrame
+    assert df.size == 240
+
+
 def test_get_discharge_measurements(requests_mock):
     """Tests get_discharge_measurements method correctly generates the request url and returns the result in a
     DataFrame"""
     format = "rdb"
     site = "01594440"
     request_url = 'https://nwis.waterdata.usgs.gov/nwis/measurements?format={}&site_no={}' \
                   '&begin_date=2000-02-14&end_date=2020-02-15'.format(format, site)
@@ -161,41 +270,131 @@
     mock_request(requests_mock, request_url, response_file_path)
     df, md = get_discharge_measurements(sites=[site], start='2000-02-14', end='2020-02-15')
     assert type(df) is DataFrame
     assert df.size == 2130
     assert_metadata(requests_mock, request_url, md, site, None, format)
 
 
+@pytest.mark.parametrize("site_input_type_list", [True, False])
+def test_get_discharge_measurements_sites_value_types(requests_mock, site_input_type_list):
+    """Tests get_discharge_measurements method for valid input types for 'sites' parameter"""
+    _format = "rdb"
+    site = "01594440"
+    request_url = 'https://nwis.waterdata.usgs.gov/nwis/measurements?format={}&site_no={}' \
+                  '&begin_date=2000-02-14&end_date=2020-02-15'.format(_format, site)
+    response_file_path = 'data/waterdata_measurements.txt'
+    mock_request(requests_mock, request_url, response_file_path)
+    if site_input_type_list:
+        sites = [site]
+    else:
+        sites = site
+    df, md = get_discharge_measurements(sites=sites, start='2000-02-14', end='2020-02-15')
+    assert type(df) is DataFrame
+    assert df.size == 2130
+
+
 def test_get_pmcodes(requests_mock):
-    """Tests get_discharge_measurements method correctly generates the request url and returns the result in a
+    """Tests get_pmcodes method correctly generates the request url and returns the result in a
     DataFrame"""
     format = "rdb"
     request_url = "https://help.waterdata.usgs.gov/code/parameter_cd_nm_query?fmt=rdb&parm_nm_cd=%2500618%25"
     response_file_path = 'data/waterdata_pmcodes.txt'
     mock_request(requests_mock, request_url, response_file_path)
     df, md = get_pmcodes(parameterCd='00618')
     assert type(df) is DataFrame
     assert df.size == 13
     assert_metadata(requests_mock, request_url, md, None, None, format)
 
 
+@pytest.mark.parametrize("parameterCd_input_type_list", [True, False])
+def test_get_pmcodes_parameterCd_value_types(requests_mock, parameterCd_input_type_list):
+    """Tests get_pmcodes method for valid input types for the 'parameterCd' parameter"""
+    _format = "rdb"
+    parameterCd = '00618'
+    request_url = "https://help.waterdata.usgs.gov/code/parameter_cd_nm_query?fmt={}&parm_nm_cd=%25{}%25"
+    request_url = request_url.format(_format, parameterCd)
+    response_file_path = 'data/waterdata_pmcodes.txt'
+    mock_request(requests_mock, request_url, response_file_path)
+    if parameterCd_input_type_list:
+        parameterCd = [parameterCd]
+    else:
+        parameterCd = parameterCd
+    df, md = get_pmcodes(parameterCd=parameterCd)
+    assert type(df) is DataFrame
+    assert df.size == 13
+
+
 def test_get_water_use_national(requests_mock):
     """Tests get_discharge_measurements method correctly generates the request url and returns the result in a
     DataFrame"""
     format = "rdb"
     request_url = 'https://nwis.waterdata.usgs.gov/nwis/water_use?rdb_compression=value&format={}&wu_year=ALL' \
                   '&wu_category=ALL&wu_county=ALL'.format(format)
     response_file_path = 'data/water_use_national.txt'
     mock_request(requests_mock, request_url, response_file_path)
     df, md = get_water_use()
     assert type(df) is DataFrame
     assert df.size == 225
     assert_metadata(requests_mock, request_url, md, None, None, format)
 
 
+@pytest.mark.parametrize("year_input_type_list", [True, False])
+def test_get_water_use_national_year_value_types(requests_mock, year_input_type_list):
+    """Tests get_water_use method for valid input types for the 'years' parameter"""
+    _format = "rdb"
+    year = "ALL"
+    request_url = 'https://nwis.waterdata.usgs.gov/nwis/water_use?rdb_compression=value&format={}&wu_year=ALL' \
+                  '&wu_category=ALL&wu_county=ALL'.format(_format)
+    response_file_path = 'data/water_use_national.txt'
+    mock_request(requests_mock, request_url, response_file_path)
+    if year_input_type_list:
+        years = [year]
+    else:
+        years = year
+    df, md = get_water_use(years=years)
+    assert type(df) is DataFrame
+    assert df.size == 225
+
+
+@pytest.mark.parametrize("county_input_type_list", [True, False])
+def test_get_water_use_national_county_value_types(requests_mock, county_input_type_list):
+    """Tests get_water_use method for valid input types for the 'counties' parameter"""
+    _format = "rdb"
+    county = "ALL"
+    request_url = 'https://nwis.waterdata.usgs.gov/nwis/water_use?rdb_compression=value&format={}&wu_year=ALL' \
+                  '&wu_category=ALL&wu_county=ALL'.format(_format)
+    response_file_path = 'data/water_use_national.txt'
+    mock_request(requests_mock, request_url, response_file_path)
+    if county_input_type_list:
+        counties = [county]
+    else:
+        counties = county
+    df, md = get_water_use(counties=counties)
+    assert type(df) is DataFrame
+    assert df.size == 225
+
+
+@pytest.mark.parametrize("category_input_type_list", [True, False])
+def test_get_water_use_national_county_value_types(requests_mock, category_input_type_list):
+    """Tests get_water_use method for valid input types for the 'categories' parameter"""
+    _format = "rdb"
+    category = "ALL"
+    request_url = 'https://nwis.waterdata.usgs.gov/nwis/water_use?rdb_compression=value&format={}&wu_year=ALL' \
+                  '&wu_category=ALL&wu_county=ALL'.format(_format)
+    response_file_path = 'data/water_use_national.txt'
+    mock_request(requests_mock, request_url, response_file_path)
+    if category_input_type_list:
+        categories = [category]
+    else:
+        categories = category
+    df, md = get_water_use(categories=categories)
+    assert type(df) is DataFrame
+    assert df.size == 225
+
+
 def test_get_water_use_allegheny(requests_mock):
     """Tests get_discharge_measurements method correctly generates the request url and returns the result in a
     DataFrame"""
     format = "rdb"
     request_url = 'https://nwis.waterdata.usgs.gov/PA/nwis/water_use?rdb_compression=value&format=rdb&wu_year=ALL' \
                   '&wu_category=ALL&wu_county=003&wu_area=county'
     response_file_path = 'data/water_use_allegheny.txt'
@@ -233,17 +432,15 @@
     parameter_cd = '00010%2C00060'
     parameter_cd_list = ["00010","00060"]
     request_url = "https://waterservices.usgs.gov/nwis/site?bBox=-83.0%2C36.5%2C-81.0%2C38.5" \
                   "&parameterCd={}&hasDataTypeCd=dv&format={}".format(parameter_cd, format)
     response_file_path = 'data/nwis_sites.txt'
     mock_request(requests_mock, request_url, response_file_path)
 
-    df, md = what_sites(bBox=[-83.0,36.5,-81.0,38.5],
-                         parameterCd=parameter_cd_list,
-                         hasDataTypeCd="dv")
+    df, md = what_sites(bBox=[-83.0,36.5,-81.0,38.5], parameterCd=parameter_cd_list, hasDataTypeCd="dv")
     assert type(df) is DataFrame
     assert df.size == 2472
     assert_metadata(requests_mock, request_url, md, None, parameter_cd_list, format)
 
 
 def test_get_stats(requests_mock):
     """Tests get_stats method correctly generates the request url and returns the result in a DataFrame"""
@@ -254,14 +451,31 @@
 
     df, md = get_stats(sites=["01491000", "01645000"])
     assert type(df) is DataFrame
     assert df.size == 51936
     assert_metadata(requests_mock, request_url, md, None, None, format)
 
 
+@pytest.mark.parametrize("site_input_type_list", [True, False])
+def test_get_stats_site_value_types(requests_mock, site_input_type_list):
+    """Tests get_stats method for valid input types for the 'sites' parameter"""
+    _format = "rdb"
+    site = '01491000'
+    request_url = "https://waterservices.usgs.gov/nwis/stat?sites={}&format={}".format(site, _format)
+    response_file_path = 'data/waterservices_stats.txt'
+    mock_request(requests_mock, request_url, response_file_path)
+    if site_input_type_list:
+        sites = [site]
+    else:
+        sites = site
+    df, md = get_stats(sites=sites)
+    assert type(df) is DataFrame
+    assert df.size == 51936
+
+
 def mock_request(requests_mock, request_url, file_path):
     with open(file_path) as text:
         requests_mock.get(request_url, text=text.read(), headers={"mock_header": "value"})
 
 
 def assert_metadata(requests_mock, request_url, md, site, parameter_cd, format):
     assert md.url == request_url
```

### Comparing `dataretrieval-1.0.6/tests/wqp_test.py` & `dataretrieval-1.0.7/tests/wqp_test.py`

 * *Files identical despite different names*

