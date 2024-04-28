# Comparing `tmp/aideml-0.1.1.tar.gz` & `tmp/aideml-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aideml-0.1.1.tar", last modified: Wed Apr 17 15:30:34 2024, max compression
+gzip compressed data, was "aideml-0.1.3.tar", last modified: Sun Apr 28 14:48:38 2024, max compression
```

## Comparing `aideml-0.1.1.tar` & `aideml-0.1.3.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:30:34.043348 aideml-0.1.1/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3120 2024-04-17 15:10:16.000000 aideml-0.1.1/.gitignore
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1068 2024-04-17 15:10:16.000000 aideml-0.1.1/LICENSE
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    24137 2024-04-17 15:30:34.043205 aideml-0.1.1/PKG-INFO
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    23683 2024-04-17 15:26:29.000000 aideml-0.1.1/README.md
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:30:34.031548 aideml-0.1.1/aide/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1892 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/__init__.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    14729 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/agent.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:30:34.032089 aideml-0.1.1/aide/backend/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1941 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/backend/__init__.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1968 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/backend/backend_anthropic.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2272 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/backend/backend_openai.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1703 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/backend/utils.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:30:34.032335 aideml-0.1.1/aide/example_tasks/
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:30:34.032474 aideml-0.1.1/aide/example_tasks/bitcoin_price/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    41966 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/example_tasks/bitcoin_price/BTC-USD.csv
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      207 2024-04-17 15:26:29.000000 aideml-0.1.1/aide/example_tasks/bitcoin_price.md
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:30:34.033269 aideml-0.1.1/aide/example_tasks/house_prices/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    13370 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/example_tasks/house_prices/data_description.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    31939 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/example_tasks/house_prices/sample_submission.csv
--rw-r--r--   0 yuxiangwu   (501) staff       (20)   451405 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/example_tasks/house_prices/test.csv
--rw-r--r--   0 yuxiangwu   (501) staff       (20)   460676 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/example_tasks/house_prices/train.csv
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1356 2024-04-17 15:26:29.000000 aideml-0.1.1/aide/example_tasks/house_prices.md
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    11106 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/interpreter.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     7065 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/journal.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1278 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/journal2report.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4059 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/run.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:30:34.034545 aideml-0.1.1/aide/utils/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3322 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/utils/__init__.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     5371 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/utils/config.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1376 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/utils/config.yaml
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     5266 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/utils/data_preview.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2284 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/utils/metric.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2755 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/utils/response.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1463 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/utils/serialize.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2406 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/utils/tree_export.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:30:34.034762 aideml-0.1.1/aide/utils/viz_templates/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1675 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/utils/viz_templates/template.html
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     8969 2024-04-17 15:10:16.000000 aideml-0.1.1/aide/utils/viz_templates/template.js
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:30:34.035473 aideml-0.1.1/aideml.egg-info/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    24137 2024-04-17 15:30:33.000000 aideml-0.1.1/aideml.egg-info/PKG-INFO
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4111 2024-04-17 15:30:34.000000 aideml-0.1.1/aideml.egg-info/SOURCES.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)        1 2024-04-17 15:30:33.000000 aideml-0.1.1/aideml.egg-info/dependency_links.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)       38 2024-04-17 15:30:33.000000 aideml-0.1.1/aideml.egg-info/entry_points.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      849 2024-04-17 15:30:33.000000 aideml-0.1.1/aideml.egg-info/requires.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)        5 2024-04-17 15:30:33.000000 aideml-0.1.1/aideml.egg-info/top_level.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1049 2024-04-17 15:10:16.000000 aideml-0.1.1/requirements.txt
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-17 15:30:34.043028 aideml-0.1.1/sample_results/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2086 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/bike-sharing-demand.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1649 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/career-con-2019.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2645 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/cat-in-the-dat-ii.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1822 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/cat-in-the-dat.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2150 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/ciphertext-challenge-ii.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1115 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/ciphertext-challenge-iii.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2560 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/competitive-data-science-predict-future-sales.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2451 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/digit-recognizer.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1657 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/dont-overfit-ii.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3290 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/facial-keypoints-detection.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1017 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/forest-cover-type-prediction.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2670 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/godaddy-microbusiness-density-forecasting.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2072 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/home-data-for-ml-course.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2574 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/house-prices-advanced-regression-techniques.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1928 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/icr-identify-age-related-conditions.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1206 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/jigsaw-toxic-comment-classification-challenge.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3571 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/new-york-city-taxi-fare-prediction.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1207 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/nlp-getting-started.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1857 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/optiver-trading-at-the-close.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1824 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e1.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      990 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e11.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2077 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e13.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2101 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e14.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1759 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e15.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2940 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e16.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2299 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e17.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3109 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e18.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2568 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e19.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2077 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e20.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2086 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e22.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2254 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e23.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3368 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e24.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2063 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e25.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2001 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e26.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2069 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e3.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1292 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e5.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1217 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e7.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1102 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s3e9.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1917 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s4e1.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2087 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/playground-series-s4e2.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3855 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/santa-2019-revenge-of-the-accountants.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1609 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/scrabble-player-rating.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1887 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/sentiment-analysis-on-movie-reviews.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2413 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/spaceship-titanic.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1868 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-apr-2021.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1533 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-apr-2022.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1370 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-aug-2021.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2479 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-aug-2022.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1114 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-dec-2021.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2330 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-feb-2021.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2088 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-feb-2022.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1145 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-jan-2021.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2594 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-jan-2022.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3354 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-jul-2021.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1506 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-jul-2022.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1721 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-jun-2021.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1397 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-jun-2022.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1885 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-mar-2021.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1740 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-mar-2022.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1106 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-may-2021.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1308 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-may-2022.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1819 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-oct-2021.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2421 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-oct-2022.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1234 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-sep-2021.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2244 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tabular-playground-series-sep-2022.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3410 2024-04-17 15:10:16.000000 aideml-0.1.1/sample_results/tmdb-box-office-prediction.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)       38 2024-04-17 15:30:34.043388 aideml-0.1.1/setup.cfg
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1135 2024-04-17 15:30:23.000000 aideml-0.1.1/setup.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-28 14:48:38.174259 aideml-0.1.3/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3120 2024-04-17 15:10:16.000000 aideml-0.1.3/.gitignore
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1068 2024-04-17 15:10:16.000000 aideml-0.1.3/LICENSE
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    24137 2024-04-28 14:48:38.174083 aideml-0.1.3/PKG-INFO
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    23683 2024-04-25 14:01:14.000000 aideml-0.1.3/README.md
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-28 14:48:38.161672 aideml-0.1.3/aide/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1892 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    14729 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/agent.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-28 14:48:38.162377 aideml-0.1.3/aide/backend/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1941 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/backend/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1968 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/backend/backend_anthropic.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2272 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/backend/backend_openai.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1703 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/backend/utils.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-28 14:48:38.162652 aideml-0.1.3/aide/example_tasks/
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-28 14:48:38.162795 aideml-0.1.3/aide/example_tasks/bitcoin_price/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    41966 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/example_tasks/bitcoin_price/BTC-USD.csv
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      207 2024-04-17 15:26:29.000000 aideml-0.1.3/aide/example_tasks/bitcoin_price.md
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-28 14:48:38.163791 aideml-0.1.3/aide/example_tasks/house_prices/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    13370 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/example_tasks/house_prices/data_description.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    31939 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/example_tasks/house_prices/sample_submission.csv
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)   451405 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/example_tasks/house_prices/test.csv
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)   460676 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/example_tasks/house_prices/train.csv
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1356 2024-04-17 15:26:29.000000 aideml-0.1.3/aide/example_tasks/house_prices.md
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    11106 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/interpreter.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     7065 2024-04-28 13:53:38.000000 aideml-0.1.3/aide/journal.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1278 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/journal2report.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4059 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/run.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-28 14:48:38.165099 aideml-0.1.3/aide/utils/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3322 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/utils/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     5371 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/utils/config.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1376 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/utils/config.yaml
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     5266 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/utils/data_preview.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2243 2024-04-28 14:39:10.000000 aideml-0.1.3/aide/utils/metric.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2755 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/utils/response.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1463 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/utils/serialize.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2406 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/utils/tree_export.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-28 14:48:38.165354 aideml-0.1.3/aide/utils/viz_templates/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1675 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/utils/viz_templates/template.html
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     8969 2024-04-17 15:10:16.000000 aideml-0.1.3/aide/utils/viz_templates/template.js
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-28 14:48:38.166145 aideml-0.1.3/aideml.egg-info/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    24137 2024-04-28 14:48:38.000000 aideml-0.1.3/aideml.egg-info/PKG-INFO
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4111 2024-04-28 14:48:38.000000 aideml-0.1.3/aideml.egg-info/SOURCES.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)        1 2024-04-28 14:48:38.000000 aideml-0.1.3/aideml.egg-info/dependency_links.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)       38 2024-04-28 14:48:38.000000 aideml-0.1.3/aideml.egg-info/entry_points.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      856 2024-04-28 14:48:38.000000 aideml-0.1.3/aideml.egg-info/requires.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)        5 2024-04-28 14:48:38.000000 aideml-0.1.3/aideml.egg-info/top_level.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1056 2024-04-28 14:37:23.000000 aideml-0.1.3/requirements.txt
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2024-04-28 14:48:38.173892 aideml-0.1.3/sample_results/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2086 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/bike-sharing-demand.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1649 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/career-con-2019.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2645 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/cat-in-the-dat-ii.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1822 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/cat-in-the-dat.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2150 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/ciphertext-challenge-ii.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1115 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/ciphertext-challenge-iii.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2560 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/competitive-data-science-predict-future-sales.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2451 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/digit-recognizer.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1657 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/dont-overfit-ii.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3290 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/facial-keypoints-detection.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1017 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/forest-cover-type-prediction.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2670 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/godaddy-microbusiness-density-forecasting.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2072 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/home-data-for-ml-course.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2574 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/house-prices-advanced-regression-techniques.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1928 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/icr-identify-age-related-conditions.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1206 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/jigsaw-toxic-comment-classification-challenge.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3571 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/new-york-city-taxi-fare-prediction.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1207 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/nlp-getting-started.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1857 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/optiver-trading-at-the-close.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1824 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e1.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      990 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e11.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2077 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e13.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2101 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e14.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1759 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e15.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2940 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e16.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2299 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e17.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3109 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e18.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2568 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e19.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2077 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e20.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2086 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e22.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2254 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e23.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3368 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e24.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2063 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e25.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2001 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e26.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2069 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e3.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1292 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e5.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1217 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e7.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1102 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s3e9.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1917 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s4e1.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2087 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/playground-series-s4e2.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3855 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/santa-2019-revenge-of-the-accountants.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1609 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/scrabble-player-rating.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1887 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/sentiment-analysis-on-movie-reviews.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2413 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/spaceship-titanic.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1868 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-apr-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1533 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-apr-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1370 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-aug-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2479 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-aug-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1114 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-dec-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2330 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-feb-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2088 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-feb-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1145 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-jan-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2594 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-jan-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3354 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-jul-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1506 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-jul-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1721 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-jun-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1397 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-jun-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1885 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-mar-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1740 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-mar-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1106 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-may-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1308 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-may-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1819 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-oct-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2421 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-oct-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1234 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-sep-2021.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2244 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tabular-playground-series-sep-2022.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3410 2024-04-17 15:10:16.000000 aideml-0.1.3/sample_results/tmdb-box-office-prediction.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)       38 2024-04-28 14:48:38.174302 aideml-0.1.3/setup.cfg
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1135 2024-04-28 14:37:44.000000 aideml-0.1.3/setup.py
```

### Comparing `aideml-0.1.1/.gitignore` & `aideml-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/LICENSE` & `aideml-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/PKG-INFO` & `aideml-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aideml
-Version: 0.1.1
+Version: 0.1.3
 Summary: Autonomous AI for Data Science and Machine Learning
 Home-page: https://github.com/Wecoai/aideml
 Author: Weco AI
 Author-email: contact@weco.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `aideml-0.1.1/README.md` & `aideml-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/__init__.py` & `aideml-0.1.3/aide/__init__.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/agent.py` & `aideml-0.1.3/aide/agent.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/backend/__init__.py` & `aideml-0.1.3/aide/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/backend/backend_anthropic.py` & `aideml-0.1.3/aide/backend/backend_anthropic.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/backend/backend_openai.py` & `aideml-0.1.3/aide/backend/backend_openai.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/backend/utils.py` & `aideml-0.1.3/aide/backend/utils.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/example_tasks/bitcoin_price/BTC-USD.csv` & `aideml-0.1.3/aide/example_tasks/bitcoin_price/BTC-USD.csv`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/example_tasks/house_prices/data_description.txt` & `aideml-0.1.3/aide/example_tasks/house_prices/data_description.txt`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/example_tasks/house_prices/sample_submission.csv` & `aideml-0.1.3/aide/example_tasks/house_prices/sample_submission.csv`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/example_tasks/house_prices/test.csv` & `aideml-0.1.3/aide/example_tasks/house_prices/test.csv`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/example_tasks/house_prices/train.csv` & `aideml-0.1.3/aide/example_tasks/house_prices/train.csv`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/example_tasks/house_prices.md` & `aideml-0.1.3/aide/example_tasks/house_prices.md`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/interpreter.py` & `aideml-0.1.3/aide/interpreter.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/journal.py` & `aideml-0.1.3/aide/journal.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/journal2report.py` & `aideml-0.1.3/aide/journal2report.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/run.py` & `aideml-0.1.3/aide/run.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/utils/__init__.py` & `aideml-0.1.3/aide/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/utils/config.py` & `aideml-0.1.3/aide/utils/config.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/utils/config.yaml` & `aideml-0.1.3/aide/utils/config.yaml`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/utils/data_preview.py` & `aideml-0.1.3/aide/utils/data_preview.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/utils/metric.py` & `aideml-0.1.3/aide/utils/metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         if self.value == other.value:
             return False
 
         comp = self.value > other.value
         return comp if self.maximize else not comp  # type: ignore
 
     def __eq__(self, other: Any) -> bool:
-        assert type(self) is type(other)
         return self.value == other.value
 
     def __repr__(self) -> str:
         return str(self)
 
     def __str__(self) -> str:
         if self.maximize is None:
```

### Comparing `aideml-0.1.1/aide/utils/response.py` & `aideml-0.1.3/aide/utils/response.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/utils/serialize.py` & `aideml-0.1.3/aide/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/utils/tree_export.py` & `aideml-0.1.3/aide/utils/tree_export.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/utils/viz_templates/template.html` & `aideml-0.1.3/aide/utils/viz_templates/template.html`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aide/utils/viz_templates/template.js` & `aideml-0.1.3/aide/utils/viz_templates/template.js`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aideml.egg-info/PKG-INFO` & `aideml-0.1.3/aideml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aideml
-Version: 0.1.1
+Version: 0.1.3
 Summary: Autonomous AI for Data Science and Machine Learning
 Home-page: https://github.com/Wecoai/aideml
 Author: Weco AI
 Author-email: contact@weco.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `aideml-0.1.1/aideml.egg-info/SOURCES.txt` & `aideml-0.1.3/aideml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/aideml.egg-info/requires.txt` & `aideml-0.1.3/aideml.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 imgaug
 scikit-optimize
 plotly
 hyperopt
 bayesian-optimization
 imagecodecs
 hmmlearn
-bayespy
+bayespy==0.5.1
 sklearn-pandas
 tensorpack
 sentencepiece
 librosa
 ipykernel
 ipython
 nbformat
```

### Comparing `aideml-0.1.1/requirements.txt` & `aideml-0.1.3/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 imgaug
 scikit-optimize
 plotly
 hyperopt
 bayesian-optimization
 imagecodecs
 hmmlearn
-bayespy
+bayespy==0.5.1
 sklearn-pandas
 tensorpack
 sentencepiece
 librosa
 ipykernel
 ipython
 nbformat
```

### Comparing `aideml-0.1.1/sample_results/bike-sharing-demand.py` & `aideml-0.1.3/sample_results/bike-sharing-demand.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/career-con-2019.py` & `aideml-0.1.3/sample_results/career-con-2019.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/cat-in-the-dat-ii.py` & `aideml-0.1.3/sample_results/cat-in-the-dat-ii.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/cat-in-the-dat.py` & `aideml-0.1.3/sample_results/cat-in-the-dat.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/ciphertext-challenge-ii.py` & `aideml-0.1.3/sample_results/ciphertext-challenge-ii.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/ciphertext-challenge-iii.py` & `aideml-0.1.3/sample_results/ciphertext-challenge-iii.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/competitive-data-science-predict-future-sales.py` & `aideml-0.1.3/sample_results/competitive-data-science-predict-future-sales.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/digit-recognizer.py` & `aideml-0.1.3/sample_results/digit-recognizer.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/dont-overfit-ii.py` & `aideml-0.1.3/sample_results/dont-overfit-ii.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/facial-keypoints-detection.py` & `aideml-0.1.3/sample_results/facial-keypoints-detection.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/forest-cover-type-prediction.py` & `aideml-0.1.3/sample_results/forest-cover-type-prediction.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/godaddy-microbusiness-density-forecasting.py` & `aideml-0.1.3/sample_results/godaddy-microbusiness-density-forecasting.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/home-data-for-ml-course.py` & `aideml-0.1.3/sample_results/home-data-for-ml-course.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/house-prices-advanced-regression-techniques.py` & `aideml-0.1.3/sample_results/house-prices-advanced-regression-techniques.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/icr-identify-age-related-conditions.py` & `aideml-0.1.3/sample_results/icr-identify-age-related-conditions.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/jigsaw-toxic-comment-classification-challenge.py` & `aideml-0.1.3/sample_results/jigsaw-toxic-comment-classification-challenge.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/new-york-city-taxi-fare-prediction.py` & `aideml-0.1.3/sample_results/new-york-city-taxi-fare-prediction.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/nlp-getting-started.py` & `aideml-0.1.3/sample_results/nlp-getting-started.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/optiver-trading-at-the-close.py` & `aideml-0.1.3/sample_results/optiver-trading-at-the-close.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e1.py` & `aideml-0.1.3/sample_results/playground-series-s3e1.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e11.py` & `aideml-0.1.3/sample_results/playground-series-s3e11.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e13.py` & `aideml-0.1.3/sample_results/playground-series-s3e13.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e14.py` & `aideml-0.1.3/sample_results/playground-series-s3e14.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e15.py` & `aideml-0.1.3/sample_results/playground-series-s3e15.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e16.py` & `aideml-0.1.3/sample_results/playground-series-s3e16.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e17.py` & `aideml-0.1.3/sample_results/playground-series-s3e17.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e18.py` & `aideml-0.1.3/sample_results/playground-series-s3e18.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e19.py` & `aideml-0.1.3/sample_results/playground-series-s3e19.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e20.py` & `aideml-0.1.3/sample_results/playground-series-s3e20.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e22.py` & `aideml-0.1.3/sample_results/playground-series-s3e22.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e23.py` & `aideml-0.1.3/sample_results/playground-series-s3e23.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e24.py` & `aideml-0.1.3/sample_results/playground-series-s3e24.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e25.py` & `aideml-0.1.3/sample_results/playground-series-s3e25.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e26.py` & `aideml-0.1.3/sample_results/playground-series-s3e26.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e3.py` & `aideml-0.1.3/sample_results/playground-series-s3e3.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e5.py` & `aideml-0.1.3/sample_results/playground-series-s3e5.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e7.py` & `aideml-0.1.3/sample_results/playground-series-s3e7.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s3e9.py` & `aideml-0.1.3/sample_results/playground-series-s3e9.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s4e1.py` & `aideml-0.1.3/sample_results/playground-series-s4e1.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/playground-series-s4e2.py` & `aideml-0.1.3/sample_results/playground-series-s4e2.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/santa-2019-revenge-of-the-accountants.py` & `aideml-0.1.3/sample_results/santa-2019-revenge-of-the-accountants.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/scrabble-player-rating.py` & `aideml-0.1.3/sample_results/scrabble-player-rating.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/sentiment-analysis-on-movie-reviews.py` & `aideml-0.1.3/sample_results/sentiment-analysis-on-movie-reviews.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/spaceship-titanic.py` & `aideml-0.1.3/sample_results/spaceship-titanic.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-apr-2021.py` & `aideml-0.1.3/sample_results/tabular-playground-series-apr-2021.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-apr-2022.py` & `aideml-0.1.3/sample_results/tabular-playground-series-apr-2022.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-aug-2021.py` & `aideml-0.1.3/sample_results/tabular-playground-series-aug-2021.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-aug-2022.py` & `aideml-0.1.3/sample_results/tabular-playground-series-aug-2022.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-dec-2021.py` & `aideml-0.1.3/sample_results/tabular-playground-series-dec-2021.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-feb-2021.py` & `aideml-0.1.3/sample_results/tabular-playground-series-feb-2021.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-feb-2022.py` & `aideml-0.1.3/sample_results/tabular-playground-series-feb-2022.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-jan-2021.py` & `aideml-0.1.3/sample_results/tabular-playground-series-jan-2021.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-jan-2022.py` & `aideml-0.1.3/sample_results/tabular-playground-series-jan-2022.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-jul-2021.py` & `aideml-0.1.3/sample_results/tabular-playground-series-jul-2021.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-jul-2022.py` & `aideml-0.1.3/sample_results/tabular-playground-series-jul-2022.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-jun-2021.py` & `aideml-0.1.3/sample_results/tabular-playground-series-jun-2021.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-jun-2022.py` & `aideml-0.1.3/sample_results/tabular-playground-series-jun-2022.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-mar-2021.py` & `aideml-0.1.3/sample_results/tabular-playground-series-mar-2021.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-mar-2022.py` & `aideml-0.1.3/sample_results/tabular-playground-series-mar-2022.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-may-2021.py` & `aideml-0.1.3/sample_results/tabular-playground-series-may-2021.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-may-2022.py` & `aideml-0.1.3/sample_results/tabular-playground-series-may-2022.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-oct-2021.py` & `aideml-0.1.3/sample_results/tabular-playground-series-oct-2021.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-oct-2022.py` & `aideml-0.1.3/sample_results/tabular-playground-series-oct-2022.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-sep-2021.py` & `aideml-0.1.3/sample_results/tabular-playground-series-sep-2021.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tabular-playground-series-sep-2022.py` & `aideml-0.1.3/sample_results/tabular-playground-series-sep-2022.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/sample_results/tmdb-box-office-prediction.py` & `aideml-0.1.3/sample_results/tmdb-box-office-prediction.py`

 * *Files identical despite different names*

### Comparing `aideml-0.1.1/setup.py` & `aideml-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="aideml",
-    version="0.1.1",
+    version="0.1.3",
     author="Weco AI",
     author_email="contact@weco.ai",
     description="Autonomous AI for Data Science and Machine Learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Wecoai/aideml",
     packages=find_packages(),
```

