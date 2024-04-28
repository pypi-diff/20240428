# Comparing `tmp/chainforge-0.3.1.6.tar.gz` & `tmp/chainforge-0.3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainforge-0.3.1.6.tar", last modified: Fri Apr 26 11:25:42 2024, max compression
+gzip compressed data, was "chainforge-0.3.1.7.tar", last modified: Sun Apr 28 18:32:18 2024, max compression
```

## Comparing `chainforge-0.3.1.6.tar` & `chainforge-0.3.1.7.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-26 11:25:42.100252 chainforge-0.3.1.6/
--rw-r--r--   0 ianarawjo   (501) staff       (20)     1067 2023-04-11 20:15:11.000000 chainforge-0.3.1.6/LICENSE.md
--rw-r--r--   0 ianarawjo   (501) staff       (20)       79 2023-06-03 18:33:55.000000 chainforge-0.3.1.6/MANIFEST.in
--rw-r--r--   0 ianarawjo   (501) staff       (20)    12297 2024-04-26 11:25:42.099886 chainforge-0.3.1.6/PKG-INFO
--rw-r--r--   0 ianarawjo   (501) staff       (20)    11612 2024-04-25 16:57:46.000000 chainforge-0.3.1.6/README.md
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-26 11:25:42.009694 chainforge-0.3.1.6/chainforge/
--rw-r--r--   0 ianarawjo   (501) staff       (20)       22 2023-05-18 04:19:30.000000 chainforge-0.3.1.6/chainforge/__init__.py
--rw-r--r--   0 ianarawjo   (501) staff       (20)     1799 2024-01-08 23:20:01.000000 chainforge-0.3.1.6/chainforge/app.py
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-26 11:25:42.024884 chainforge-0.3.1.6/chainforge/examples/
--rw-r--r--   0 ianarawjo   (501) staff       (20)     8196 2024-03-14 16:05:55.000000 chainforge-0.3.1.6/chainforge/examples/.DS_Store
--rw-r--r--   0 ianarawjo   (501) staff       (20)   141071 2024-03-15 02:24:15.000000 chainforge-0.3.1.6/chainforge/examples/basic-comparison.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)   128447 2024-03-15 02:24:15.000000 chainforge-0.3.1.6/chainforge/examples/basic-function-calls.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)   144733 2024-03-15 02:24:15.000000 chainforge-0.3.1.6/chainforge/examples/basic-math.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)   237904 2024-03-15 02:24:15.000000 chainforge-0.3.1.6/chainforge/examples/chaining-prompts.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)  1524201 2024-03-15 02:24:15.000000 chainforge-0.3.1.6/chainforge/examples/comparing-system-msg.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     1897 2023-08-27 19:12:06.000000 chainforge-0.3.1.6/chainforge/examples/custom_provider_cohere.py
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-26 11:25:42.059812 chainforge-0.3.1.6/chainforge/examples/oaievals/
--rw-r--r--   0 ianarawjo   (501) staff       (20)    30489 2023-06-28 22:13:17.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/2d_movement.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     5213 2023-06-21 00:14:03.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/adultery_state_laws.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     7931 2023-06-21 00:08:17.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/aime_evaluation.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     4706 2023-06-28 15:51:36.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/algebra-word-problems.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)    13381 2023-06-23 13:09:21.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/ambiguous-sentences.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)    26494 2023-06-15 18:12:38.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/bitwise.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)    14333 2023-06-21 00:14:31.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/born-first.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)   318543 2023-07-08 00:20:04.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/brazilian_laws.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)   117153 2023-06-21 00:07:22.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/chess-piece-count.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)    22194 2023-06-15 18:11:11.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/chess.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)    24710 2023-06-21 00:15:38.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/compare-countries-area.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     4877 2023-06-21 00:06:47.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/counterfactual-reasoning.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)    13384 2023-06-15 18:11:26.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/countries.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     9806 2023-06-15 18:12:13.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/cricket_situations.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     7465 2023-06-17 13:27:04.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/day-of-week-from-date.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)    44972 2023-06-21 00:07:37.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/directions.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)   574499 2023-06-21 00:14:41.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/guess-the-singer.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)    12595 2023-06-16 13:47:50.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/hebrew-same-noun-gender.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     8975 2023-06-17 13:25:37.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/hindi_words.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)    13395 2023-06-17 12:27:51.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/japanese_populer_video_game_title_and_the_publisher.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)   205977 2023-06-17 13:27:42.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/jee-math.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)    13967 2023-06-15 18:13:08.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/mate-in-one.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     5198 2023-06-21 00:15:02.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/nepali-song-singer.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     8499 2023-06-16 13:48:40.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/number-reading.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     8232 2023-06-17 13:26:34.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/pure_korean.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)    53397 2023-06-17 12:29:15.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/regex-match.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     9520 2023-06-17 13:24:39.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/reverse-string.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)    11295 2023-06-28 22:13:45.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/russian_medical.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     6229 2023-06-17 13:26:03.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/shared-borders.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)     8339 2023-06-16 16:38:51.000000 chainforge-0.3.1.6/chainforge/examples/oaievals/tetris.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)  1083834 2024-03-15 02:24:15.000000 chainforge-0.3.1.6/chainforge/examples/prompt-injection-test.cforge
--rw-r--r--   0 ianarawjo   (501) staff       (20)    30067 2024-04-25 16:57:46.000000 chainforge-0.3.1.6/chainforge/flask_app.py
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-26 11:25:42.061744 chainforge-0.3.1.6/chainforge/providers/
--rw-r--r--   0 ianarawjo   (501) staff       (20)      141 2023-08-27 19:12:06.000000 chainforge-0.3.1.6/chainforge/providers/__init__.py
--rw-r--r--   0 ianarawjo   (501) staff       (20)     3595 2023-08-27 19:12:06.000000 chainforge-0.3.1.6/chainforge/providers/dalai.py
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-26 11:25:42.062783 chainforge-0.3.1.6/chainforge/providers/dalaipy/
--rw-r--r--   0 ianarawjo   (501) staff       (20)       43 2023-08-27 19:12:06.000000 chainforge-0.3.1.6/chainforge/providers/dalaipy/__init__.py
--rw-r--r--   0 ianarawjo   (501) staff       (20)     3996 2023-08-27 19:12:06.000000 chainforge-0.3.1.6/chainforge/providers/dalaipy/main.py
--rw-r--r--   0 ianarawjo   (501) staff       (20)     6126 2024-04-25 16:57:46.000000 chainforge-0.3.1.6/chainforge/providers/protocol.py
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-26 11:25:42.004644 chainforge-0.3.1.6/chainforge/react-server/
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-26 11:25:42.066709 chainforge-0.3.1.6/chainforge/react-server/build/
--rw-r--r--   0 ianarawjo   (501) staff       (20)     6148 2024-04-26 11:24:08.000000 chainforge-0.3.1.6/chainforge/react-server/build/.DS_Store
--rw-r--r--   0 ianarawjo   (501) staff       (20)      665 2024-04-26 11:25:16.000000 chainforge-0.3.1.6/chainforge/react-server/build/asset-manifest.json
--rw-r--r--   0 ianarawjo   (501) staff       (20)    17470 2024-04-26 11:24:08.000000 chainforge-0.3.1.6/chainforge/react-server/build/favicon.ico
--rw-r--r--   0 ianarawjo   (501) staff       (20)      893 2024-04-26 11:25:16.000000 chainforge-0.3.1.6/chainforge/react-server/build/index.html
--rw-r--r--   0 ianarawjo   (501) staff       (20)    18595 2024-04-26 11:24:08.000000 chainforge-0.3.1.6/chainforge/react-server/build/logo192.png
--rw-r--r--   0 ianarawjo   (501) staff       (20)    18375 2024-04-26 11:24:08.000000 chainforge-0.3.1.6/chainforge/react-server/build/logo512.png
--rw-r--r--   0 ianarawjo   (501) staff       (20)      480 2024-04-26 11:24:08.000000 chainforge-0.3.1.6/chainforge/react-server/build/manifest.json
--rw-r--r--   0 ianarawjo   (501) staff       (20)       67 2024-04-26 11:24:08.000000 chainforge-0.3.1.6/chainforge/react-server/build/robots.txt
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-26 11:25:42.005246 chainforge-0.3.1.6/chainforge/react-server/build/static/
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-26 11:25:42.067465 chainforge-0.3.1.6/chainforge/react-server/build/static/css/
--rw-r--r--   0 ianarawjo   (501) staff       (20)    26801 2024-04-26 11:25:16.000000 chainforge-0.3.1.6/chainforge/react-server/build/static/css/main.ebedcb7f.css
--rw-r--r--   0 ianarawjo   (501) staff       (20)    52155 2024-04-26 11:25:16.000000 chainforge-0.3.1.6/chainforge/react-server/build/static/css/main.ebedcb7f.css.map
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-26 11:25:42.078029 chainforge-0.3.1.6/chainforge/react-server/build/static/js/
--rw-r--r--   0 ianarawjo   (501) staff       (20)     8597 2024-04-26 11:25:16.000000 chainforge-0.3.1.6/chainforge/react-server/build/static/js/477.650352c6.chunk.js
--rw-r--r--   0 ianarawjo   (501) staff       (20)      149 2024-04-26 11:25:16.000000 chainforge-0.3.1.6/chainforge/react-server/build/static/js/477.650352c6.chunk.js.LICENSE.txt
--rw-r--r--   0 ianarawjo   (501) staff       (20)    28263 2024-04-26 11:25:16.000000 chainforge-0.3.1.6/chainforge/react-server/build/static/js/477.650352c6.chunk.js.map
--rw-r--r--   0 ianarawjo   (501) staff       (20)     4603 2024-04-26 11:25:16.000000 chainforge-0.3.1.6/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js
--rw-r--r--   0 ianarawjo   (501) staff       (20)    10597 2024-04-26 11:25:16.000000 chainforge-0.3.1.6/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js.map
--rw-r--r--   0 ianarawjo   (501) staff       (20)  7723930 2024-04-26 11:25:16.000000 chainforge-0.3.1.6/chainforge/react-server/build/static/js/main.c1980c3a.js
--rw-r--r--   0 ianarawjo   (501) staff       (20)     8862 2024-04-26 11:25:16.000000 chainforge-0.3.1.6/chainforge/react-server/build/static/js/main.c1980c3a.js.LICENSE.txt
--rw-r--r--   0 ianarawjo   (501) staff       (20) 13651537 2024-04-26 11:25:16.000000 chainforge-0.3.1.6/chainforge/react-server/build/static/js/main.c1980c3a.js.map
-drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-26 11:25:42.012790 chainforge-0.3.1.6/chainforge.egg-info/
--rw-r--r--   0 ianarawjo   (501) staff       (20)    12297 2024-04-26 11:25:41.000000 chainforge-0.3.1.6/chainforge.egg-info/PKG-INFO
--rw-r--r--   0 ianarawjo   (501) staff       (20)     3389 2024-04-26 11:25:41.000000 chainforge-0.3.1.6/chainforge.egg-info/SOURCES.txt
--rw-r--r--   0 ianarawjo   (501) staff       (20)        1 2024-04-26 11:25:41.000000 chainforge-0.3.1.6/chainforge.egg-info/dependency_links.txt
--rw-r--r--   0 ianarawjo   (501) staff       (20)       51 2024-04-26 11:25:41.000000 chainforge-0.3.1.6/chainforge.egg-info/entry_points.txt
--rw-r--r--   0 ianarawjo   (501) staff       (20)      127 2024-04-26 11:25:41.000000 chainforge-0.3.1.6/chainforge.egg-info/requires.txt
--rw-r--r--   0 ianarawjo   (501) staff       (20)       11 2024-04-26 11:25:41.000000 chainforge-0.3.1.6/chainforge.egg-info/top_level.txt
--rw-r--r--   0 ianarawjo   (501) staff       (20)       38 2024-04-26 11:25:42.100375 chainforge-0.3.1.6/setup.cfg
--rw-r--r--   0 ianarawjo   (501) staff       (20)     1426 2024-04-26 11:23:29.000000 chainforge-0.3.1.6/setup.py
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-28 18:32:18.883138 chainforge-0.3.1.7/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     1067 2023-04-11 20:15:11.000000 chainforge-0.3.1.7/LICENSE.md
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       79 2023-06-03 18:33:55.000000 chainforge-0.3.1.7/MANIFEST.in
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    12297 2024-04-28 18:32:18.882793 chainforge-0.3.1.7/PKG-INFO
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    11612 2024-04-25 16:57:46.000000 chainforge-0.3.1.7/README.md
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-28 18:32:18.799394 chainforge-0.3.1.7/chainforge/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       22 2023-05-18 04:19:30.000000 chainforge-0.3.1.7/chainforge/__init__.py
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     1799 2024-01-08 23:20:01.000000 chainforge-0.3.1.7/chainforge/app.py
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-28 18:32:18.814504 chainforge-0.3.1.7/chainforge/examples/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     8196 2024-03-14 16:05:55.000000 chainforge-0.3.1.7/chainforge/examples/.DS_Store
+-rw-r--r--   0 ianarawjo   (501) staff       (20)   141071 2024-03-15 02:24:15.000000 chainforge-0.3.1.7/chainforge/examples/basic-comparison.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)   128447 2024-03-15 02:24:15.000000 chainforge-0.3.1.7/chainforge/examples/basic-function-calls.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)   144733 2024-03-15 02:24:15.000000 chainforge-0.3.1.7/chainforge/examples/basic-math.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)   237904 2024-03-15 02:24:15.000000 chainforge-0.3.1.7/chainforge/examples/chaining-prompts.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)  1524201 2024-03-15 02:24:15.000000 chainforge-0.3.1.7/chainforge/examples/comparing-system-msg.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     1897 2023-08-27 19:12:06.000000 chainforge-0.3.1.7/chainforge/examples/custom_provider_cohere.py
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-28 18:32:18.846450 chainforge-0.3.1.7/chainforge/examples/oaievals/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    30489 2023-06-28 22:13:17.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/2d_movement.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     5213 2023-06-21 00:14:03.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/adultery_state_laws.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     7931 2023-06-21 00:08:17.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/aime_evaluation.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     4706 2023-06-28 15:51:36.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/algebra-word-problems.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    13381 2023-06-23 13:09:21.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/ambiguous-sentences.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    26494 2023-06-15 18:12:38.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/bitwise.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    14333 2023-06-21 00:14:31.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/born-first.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)   318543 2023-07-08 00:20:04.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/brazilian_laws.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)   117153 2023-06-21 00:07:22.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/chess-piece-count.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    22194 2023-06-15 18:11:11.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/chess.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    24710 2023-06-21 00:15:38.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/compare-countries-area.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     4877 2023-06-21 00:06:47.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/counterfactual-reasoning.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    13384 2023-06-15 18:11:26.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/countries.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     9806 2023-06-15 18:12:13.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/cricket_situations.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     7465 2023-06-17 13:27:04.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/day-of-week-from-date.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    44972 2023-06-21 00:07:37.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/directions.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)   574499 2023-06-21 00:14:41.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/guess-the-singer.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    12595 2023-06-16 13:47:50.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/hebrew-same-noun-gender.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     8975 2023-06-17 13:25:37.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/hindi_words.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    13395 2023-06-17 12:27:51.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/japanese_populer_video_game_title_and_the_publisher.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)   205977 2023-06-17 13:27:42.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/jee-math.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    13967 2023-06-15 18:13:08.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/mate-in-one.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     5198 2023-06-21 00:15:02.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/nepali-song-singer.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     8499 2023-06-16 13:48:40.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/number-reading.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     8232 2023-06-17 13:26:34.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/pure_korean.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    53397 2023-06-17 12:29:15.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/regex-match.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     9520 2023-06-17 13:24:39.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/reverse-string.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    11295 2023-06-28 22:13:45.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/russian_medical.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     6229 2023-06-17 13:26:03.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/shared-borders.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     8339 2023-06-16 16:38:51.000000 chainforge-0.3.1.7/chainforge/examples/oaievals/tetris.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)  1083834 2024-03-15 02:24:15.000000 chainforge-0.3.1.7/chainforge/examples/prompt-injection-test.cforge
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    30113 2024-04-28 18:29:21.000000 chainforge-0.3.1.7/chainforge/flask_app.py
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-28 18:32:18.848211 chainforge-0.3.1.7/chainforge/providers/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)      141 2023-08-27 19:12:06.000000 chainforge-0.3.1.7/chainforge/providers/__init__.py
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     3595 2023-08-27 19:12:06.000000 chainforge-0.3.1.7/chainforge/providers/dalai.py
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-28 18:32:18.849215 chainforge-0.3.1.7/chainforge/providers/dalaipy/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       43 2023-08-27 19:12:06.000000 chainforge-0.3.1.7/chainforge/providers/dalaipy/__init__.py
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     3996 2023-08-27 19:12:06.000000 chainforge-0.3.1.7/chainforge/providers/dalaipy/main.py
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     6126 2024-04-25 16:57:46.000000 chainforge-0.3.1.7/chainforge/providers/protocol.py
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-28 18:32:18.794512 chainforge-0.3.1.7/chainforge/react-server/
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-28 18:32:18.852931 chainforge-0.3.1.7/chainforge/react-server/build/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     6148 2024-04-28 18:30:22.000000 chainforge-0.3.1.7/chainforge/react-server/build/.DS_Store
+-rw-r--r--   0 ianarawjo   (501) staff       (20)      665 2024-04-28 18:31:28.000000 chainforge-0.3.1.7/chainforge/react-server/build/asset-manifest.json
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    17470 2024-04-28 18:30:22.000000 chainforge-0.3.1.7/chainforge/react-server/build/favicon.ico
+-rw-r--r--   0 ianarawjo   (501) staff       (20)      893 2024-04-28 18:31:28.000000 chainforge-0.3.1.7/chainforge/react-server/build/index.html
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    18595 2024-04-28 18:30:22.000000 chainforge-0.3.1.7/chainforge/react-server/build/logo192.png
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    18375 2024-04-28 18:30:22.000000 chainforge-0.3.1.7/chainforge/react-server/build/logo512.png
+-rw-r--r--   0 ianarawjo   (501) staff       (20)      480 2024-04-28 18:30:22.000000 chainforge-0.3.1.7/chainforge/react-server/build/manifest.json
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       67 2024-04-28 18:30:22.000000 chainforge-0.3.1.7/chainforge/react-server/build/robots.txt
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-28 18:32:18.795112 chainforge-0.3.1.7/chainforge/react-server/build/static/
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-28 18:32:18.853703 chainforge-0.3.1.7/chainforge/react-server/build/static/css/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    26801 2024-04-28 18:31:28.000000 chainforge-0.3.1.7/chainforge/react-server/build/static/css/main.ebedcb7f.css
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    52155 2024-04-28 18:31:28.000000 chainforge-0.3.1.7/chainforge/react-server/build/static/css/main.ebedcb7f.css.map
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-28 18:32:18.866005 chainforge-0.3.1.7/chainforge/react-server/build/static/js/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     8597 2024-04-28 18:31:28.000000 chainforge-0.3.1.7/chainforge/react-server/build/static/js/477.650352c6.chunk.js
+-rw-r--r--   0 ianarawjo   (501) staff       (20)      149 2024-04-28 18:31:28.000000 chainforge-0.3.1.7/chainforge/react-server/build/static/js/477.650352c6.chunk.js.LICENSE.txt
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    28263 2024-04-28 18:31:28.000000 chainforge-0.3.1.7/chainforge/react-server/build/static/js/477.650352c6.chunk.js.map
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     4603 2024-04-28 18:31:28.000000 chainforge-0.3.1.7/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    10597 2024-04-28 18:31:28.000000 chainforge-0.3.1.7/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js.map
+-rw-r--r--   0 ianarawjo   (501) staff       (20)  7723930 2024-04-28 18:31:28.000000 chainforge-0.3.1.7/chainforge/react-server/build/static/js/main.c1980c3a.js
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     8862 2024-04-28 18:31:28.000000 chainforge-0.3.1.7/chainforge/react-server/build/static/js/main.c1980c3a.js.LICENSE.txt
+-rw-r--r--   0 ianarawjo   (501) staff       (20) 13651537 2024-04-28 18:31:28.000000 chainforge-0.3.1.7/chainforge/react-server/build/static/js/main.c1980c3a.js.map
+drwxr-xr-x   0 ianarawjo   (501) staff       (20)        0 2024-04-28 18:32:18.801353 chainforge-0.3.1.7/chainforge.egg-info/
+-rw-r--r--   0 ianarawjo   (501) staff       (20)    12297 2024-04-28 18:32:18.000000 chainforge-0.3.1.7/chainforge.egg-info/PKG-INFO
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     3389 2024-04-28 18:32:18.000000 chainforge-0.3.1.7/chainforge.egg-info/SOURCES.txt
+-rw-r--r--   0 ianarawjo   (501) staff       (20)        1 2024-04-28 18:32:18.000000 chainforge-0.3.1.7/chainforge.egg-info/dependency_links.txt
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       51 2024-04-28 18:32:18.000000 chainforge-0.3.1.7/chainforge.egg-info/entry_points.txt
+-rw-r--r--   0 ianarawjo   (501) staff       (20)      127 2024-04-28 18:32:18.000000 chainforge-0.3.1.7/chainforge.egg-info/requires.txt
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       11 2024-04-28 18:32:18.000000 chainforge-0.3.1.7/chainforge.egg-info/top_level.txt
+-rw-r--r--   0 ianarawjo   (501) staff       (20)       38 2024-04-28 18:32:18.883233 chainforge-0.3.1.7/setup.cfg
+-rw-r--r--   0 ianarawjo   (501) staff       (20)     1426 2024-04-28 18:29:30.000000 chainforge-0.3.1.7/setup.py
```

### Comparing `chainforge-0.3.1.6/LICENSE.md` & `chainforge-0.3.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/PKG-INFO` & `chainforge-0.3.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainforge
-Version: 0.3.1.6
+Version: 0.3.1.7
 Summary: A Visual Programming Environment for Prompt Engineering
 Home-page: https://github.com/ianarawjo/ChainForge/
 Author: Ian Arawjo
 License: MIT
 Keywords: prompt engineering LLM response evaluation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `chainforge-0.3.1.6/README.md` & `chainforge-0.3.1.7/README.md`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/app.py` & `chainforge-0.3.1.7/chainforge/app.py`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/.DS_Store` & `chainforge-0.3.1.7/chainforge/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/basic-comparison.cforge` & `chainforge-0.3.1.7/chainforge/examples/basic-comparison.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/basic-function-calls.cforge` & `chainforge-0.3.1.7/chainforge/examples/basic-function-calls.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/basic-math.cforge` & `chainforge-0.3.1.7/chainforge/examples/basic-math.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/chaining-prompts.cforge` & `chainforge-0.3.1.7/chainforge/examples/chaining-prompts.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/comparing-system-msg.cforge` & `chainforge-0.3.1.7/chainforge/examples/comparing-system-msg.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/custom_provider_cohere.py` & `chainforge-0.3.1.7/chainforge/examples/custom_provider_cohere.py`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/2d_movement.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/2d_movement.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/adultery_state_laws.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/adultery_state_laws.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/aime_evaluation.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/aime_evaluation.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/algebra-word-problems.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/algebra-word-problems.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/ambiguous-sentences.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/ambiguous-sentences.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/bitwise.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/bitwise.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/born-first.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/born-first.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/brazilian_laws.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/brazilian_laws.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/chess-piece-count.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/chess-piece-count.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/chess.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/chess.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/compare-countries-area.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/compare-countries-area.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/counterfactual-reasoning.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/counterfactual-reasoning.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/countries.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/countries.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/cricket_situations.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/cricket_situations.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/day-of-week-from-date.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/day-of-week-from-date.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/directions.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/directions.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/guess-the-singer.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/guess-the-singer.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/hebrew-same-noun-gender.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/hebrew-same-noun-gender.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/hindi_words.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/hindi_words.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/japanese_populer_video_game_title_and_the_publisher.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/japanese_populer_video_game_title_and_the_publisher.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/jee-math.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/jee-math.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/mate-in-one.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/mate-in-one.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/nepali-song-singer.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/nepali-song-singer.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/number-reading.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/number-reading.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/pure_korean.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/pure_korean.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/regex-match.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/regex-match.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/reverse-string.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/reverse-string.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/russian_medical.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/russian_medical.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/shared-borders.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/shared-borders.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/oaievals/tetris.cforge` & `chainforge-0.3.1.7/chainforge/examples/oaievals/tetris.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/examples/prompt-injection-test.cforge` & `chainforge-0.3.1.7/chainforge/examples/prompt-injection-test.cforge`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/flask_app.py` & `chainforge-0.3.1.7/chainforge/flask_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,24 +456,25 @@
     return ret
 
 
 @app.route('/app/fetchEnvironAPIKeys', methods=['POST'])
 def fetchEnvironAPIKeys():
     keymap = {
         'OPENAI_API_KEY': 'OpenAI', 
+        'OPENAI_BASE_URL': 'OpenAI_BaseURL',
         'ANTHROPIC_API_KEY': 'Anthropic', 
         'PALM_API_KEY': 'Google', 
         'HUGGINGFACE_API_KEY': 'HuggingFace',
         'AZURE_OPENAI_KEY': 'Azure_OpenAI', 
         'AZURE_OPENAI_ENDPOINT': 'Azure_OpenAI_Endpoint',
         'ALEPH_ALPHA_API_KEY': 'AlephAlpha',
         'AWS_ACCESS_KEY_ID': 'AWS_Access_Key_ID',
         'AWS_SECRET_ACCESS_KEY': 'AWS_Secret_Access_Key',
         'AWS_REGION': 'AWS_Region', 
-        'AWS_SESSION_TOKEN': 'AWS_Session_Token'
+        'AWS_SESSION_TOKEN': 'AWS_Session_Token',
     }
     d = { alias: os.environ.get(key) for key, alias in keymap.items() }
     ret = jsonify(d)
     ret.headers.add('Access-Control-Allow-Origin', '*')
     return ret
```

### Comparing `chainforge-0.3.1.6/chainforge/providers/dalai.py` & `chainforge-0.3.1.7/chainforge/providers/dalai.py`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/providers/dalaipy/main.py` & `chainforge-0.3.1.7/chainforge/providers/dalaipy/main.py`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/providers/protocol.py` & `chainforge-0.3.1.7/chainforge/providers/protocol.py`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/.DS_Store` & `chainforge-0.3.1.7/chainforge/react-server/build/.DS_Store`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/asset-manifest.json` & `chainforge-0.3.1.7/chainforge/react-server/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/favicon.ico` & `chainforge-0.3.1.7/chainforge/react-server/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/index.html` & `chainforge-0.3.1.7/chainforge/react-server/build/index.html`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/logo192.png` & `chainforge-0.3.1.7/chainforge/react-server/build/logo192.png`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/logo512.png` & `chainforge-0.3.1.7/chainforge/react-server/build/logo512.png`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/static/css/main.ebedcb7f.css` & `chainforge-0.3.1.7/chainforge/react-server/build/static/css/main.ebedcb7f.css`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/static/css/main.ebedcb7f.css.map` & `chainforge-0.3.1.7/chainforge/react-server/build/static/css/main.ebedcb7f.css.map`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/static/js/477.650352c6.chunk.js` & `chainforge-0.3.1.7/chainforge/react-server/build/static/js/477.650352c6.chunk.js`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/static/js/477.650352c6.chunk.js.map` & `chainforge-0.3.1.7/chainforge/react-server/build/static/js/477.650352c6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js` & `chainforge-0.3.1.7/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js.map` & `chainforge-0.3.1.7/chainforge/react-server/build/static/js/787.4c72bb55.chunk.js.map`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/static/js/main.c1980c3a.js` & `chainforge-0.3.1.7/chainforge/react-server/build/static/js/main.c1980c3a.js`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/static/js/main.c1980c3a.js.LICENSE.txt` & `chainforge-0.3.1.7/chainforge/react-server/build/static/js/main.c1980c3a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge/react-server/build/static/js/main.c1980c3a.js.map` & `chainforge-0.3.1.7/chainforge/react-server/build/static/js/main.c1980c3a.js.map`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/chainforge.egg-info/PKG-INFO` & `chainforge-0.3.1.7/chainforge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainforge
-Version: 0.3.1.6
+Version: 0.3.1.7
 Summary: A Visual Programming Environment for Prompt Engineering
 Home-page: https://github.com/ianarawjo/ChainForge/
 Author: Ian Arawjo
 License: MIT
 Keywords: prompt engineering LLM response evaluation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `chainforge-0.3.1.6/chainforge.egg-info/SOURCES.txt` & `chainforge-0.3.1.7/chainforge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainforge-0.3.1.6/setup.py` & `chainforge-0.3.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.md', encoding='utf-8') as f:
         return f.read()
 
 setup(
     name='chainforge',
-    version='0.3.1.6',
+    version='0.3.1.7',
     packages=find_packages(),
     author="Ian Arawjo",
     description="A Visual Programming Environment for Prompt Engineering",
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords='prompt engineering LLM response evaluation',
     license="MIT",
```

