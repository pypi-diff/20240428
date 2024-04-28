# Comparing `tmp/pref_voting-1.0.0.tar.gz` & `tmp/pref_voting-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-1.0.0.tar", max compression
+gzip compressed data, was "pref_voting-1.1.0.tar", max compression
```

## Comparing `pref_voting-1.0.0.tar` & `pref_voting-1.1.0.tar`

### file list

```diff
@@ -1,72 +1,73 @@
--rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.0.0/LICENSE
--rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.0.0/README.md
--rw-r--r--   0        0        0       22 2024-04-24 21:49:13.569104 pref_voting-1.0.0/pref_voting/__init__.py
--rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-1.0.0/pref_voting/analysis.py
--rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.0.0/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.0.0/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.0.0/pref_voting/axioms.py
--rw-r--r--   0        0        0    33205 2024-04-09 01:59:48.226095 pref_voting-1.0.0/pref_voting/c1_methods.py
--rw-r--r--   0        0        0    15161 2024-03-15 20:53:44.539281 pref_voting-1.0.0/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    12659 2023-12-07 15:15:32.783919 pref_voting-1.0.0/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.0.0/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.0.0/pref_voting/generate_spatial_profiles.py
--rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.0.0/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-1.0.0/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.0.0/pref_voting/grade_methods.py
--rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.0.0/pref_voting/grade_profiles.py
--rw-r--r--   0        0        0     8068 2024-04-19 01:31:48.812126 pref_voting-1.0.0/pref_voting/helper.py
--rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.0.0/pref_voting/invariance_axioms.py
--rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.0.0/pref_voting/io/__init__.py
--rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.0.0/pref_voting/io/readers.py
--rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.0.0/pref_voting/io/writers.py
--rw-r--r--   0        0        0    90549 2024-04-15 01:51:51.467855 pref_voting-1.0.0/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.0.0/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-1.0.0/pref_voting/mappings.py
--rw-r--r--   0        0        0    70816 2024-04-15 14:41:33.937321 pref_voting-1.0.0/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.0.0/pref_voting/monotonicity_axioms.py
--rw-r--r--   0        0        0    24548 2024-03-16 15:19:40.029463 pref_voting-1.0.0/pref_voting/other_methods.py
--rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.0.0/pref_voting/prob_voting_method.py
--rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.0.0/pref_voting/probabilistic_methods.py
--rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-1.0.0/pref_voting/profiles.py
--rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.0.0/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.0.0/pref_voting/rankings.py
--rw-r--r--   0        0        0    21026 2024-04-09 02:00:24.744126 pref_voting-1.0.0/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.0.0/pref_voting/social_welfare_function.py
--rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.0.0/pref_voting/social_welfare_functions.py
--rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.0.0/pref_voting/spatial_profiles.py
--rw-r--r--   0        0        0    15790 2024-04-24 21:18:21.291486 pref_voting-1.0.0/pref_voting/strategic_axioms.py
--rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.0.0/pref_voting/tests/__init__.py
--rw-r--r--   0        0        0      666 2024-03-02 21:50:31.231806 pref_voting-1.0.0/pref_voting/tests/conftest.py
--rw-r--r--   0        0        0     5062 2024-03-19 01:38:04.296201 pref_voting-1.0.0/pref_voting/tests/test_c1_methods.py
--rw-r--r--   0        0        0     2576 2024-03-19 00:18:02.163482 pref_voting-1.0.0/pref_voting/tests/test_combined_methods.py
--rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.0.0/pref_voting/tests/test_generate_profiles.py
--rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.0.0/pref_voting/tests/test_generate_spatial_profile.py
--rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.0.0/pref_voting/tests/test_io.py
--rw-r--r--   0        0        0     8943 2024-03-17 11:39:53.682951 pref_voting-1.0.0/pref_voting/tests/test_iterative_methods.py
--rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.0.0/pref_voting/tests/test_majority_graph.py
--rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.0.0/pref_voting/tests/test_mapping.py
--rw-r--r--   0        0        0     7265 2024-04-15 14:48:24.940292 pref_voting-1.0.0/pref_voting/tests/test_margin_based_methods.py
--rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.0.0/pref_voting/tests/test_margin_graph.py
--rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.0.0/pref_voting/tests/test_other_methods.py
--rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.0.0/pref_voting/tests/test_prob_voting_method.py
--rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.0.0/pref_voting/tests/test_profile.py
--rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.0.0/pref_voting/tests/test_profile_with_ties.py
--rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.0.0/pref_voting/tests/test_ranking.py
--rw-r--r--   0        0        0     5543 2024-03-19 11:54:18.932325 pref_voting-1.0.0/pref_voting/tests/test_scoring_rules.py
--rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.0.0/pref_voting/tests/test_social_welfare_functions.py
--rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.0.0/pref_voting/tests/test_spatial_profile.py
--rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.0.0/pref_voting/tests/test_support_graph.py
--rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.0.0/pref_voting/tests/test_utility_function.py
--rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.0.0/pref_voting/tests/test_utility_functions.py
--rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.0.0/pref_voting/tests/test_voting_method.py
--rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.0.0/pref_voting/utility_functions.py
--rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.0.0/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-1.0.0/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.0.0/pref_voting/variable_candidate_axioms.py
--rw-r--r--   0        0        0    57504 2024-04-24 21:14:50.598729 pref_voting-1.0.0/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     5566 2023-12-07 15:03:17.438046 pref_voting-1.0.0/pref_voting/voting_method.py
--rw-r--r--   0        0        0      372 2023-11-14 00:06:58.907333 pref_voting-1.0.0/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.0.0/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      760 2024-04-24 21:49:13.568194 pref_voting-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-1.0.0/setup.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.1.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-28 12:21:46.031009 pref_voting-1.1.0/pref_voting/__init__.py
+-rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-1.1.0/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.1.0/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.1.0/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.1.0/pref_voting/axioms.py
+-rw-r--r--   0        0        0    33205 2024-04-09 01:59:48.226095 pref_voting-1.1.0/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0    15161 2024-03-15 20:53:44.539281 pref_voting-1.1.0/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    12659 2023-12-07 15:15:32.783919 pref_voting-1.1.0/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.1.0/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.1.0/pref_voting/generate_spatial_profiles.py
+-rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.1.0/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-1.1.0/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.1.0/pref_voting/grade_methods.py
+-rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.1.0/pref_voting/grade_profiles.py
+-rw-r--r--   0        0        0     8068 2024-04-19 01:31:48.812126 pref_voting-1.1.0/pref_voting/helper.py
+-rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.1.0/pref_voting/invariance_axioms.py
+-rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.1.0/pref_voting/io/__init__.py
+-rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.1.0/pref_voting/io/readers.py
+-rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.1.0/pref_voting/io/writers.py
+-rw-r--r--   0        0        0    90549 2024-04-15 01:51:51.467855 pref_voting-1.1.0/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.1.0/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-1.1.0/pref_voting/mappings.py
+-rw-r--r--   0        0        0    73036 2024-04-27 22:46:59.878102 pref_voting-1.1.0/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    70814 2024-04-27 22:10:28.624211 pref_voting-1.1.0/pref_voting/margin_based_methods_old.py
+-rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.1.0/pref_voting/monotonicity_axioms.py
+-rw-r--r--   0        0        0    24548 2024-03-16 15:19:40.029463 pref_voting-1.1.0/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.1.0/pref_voting/prob_voting_method.py
+-rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.1.0/pref_voting/probabilistic_methods.py
+-rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-1.1.0/pref_voting/profiles.py
+-rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.1.0/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.1.0/pref_voting/rankings.py
+-rw-r--r--   0        0        0    21026 2024-04-09 02:00:24.744126 pref_voting-1.1.0/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.1.0/pref_voting/social_welfare_function.py
+-rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.1.0/pref_voting/social_welfare_functions.py
+-rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.1.0/pref_voting/spatial_profiles.py
+-rw-r--r--   0        0        0    15790 2024-04-24 21:18:21.291486 pref_voting-1.1.0/pref_voting/strategic_axioms.py
+-rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.1.0/pref_voting/tests/__init__.py
+-rw-r--r--   0        0        0      666 2024-03-02 21:50:31.231806 pref_voting-1.1.0/pref_voting/tests/conftest.py
+-rw-r--r--   0        0        0     5062 2024-03-19 01:38:04.296201 pref_voting-1.1.0/pref_voting/tests/test_c1_methods.py
+-rw-r--r--   0        0        0     2576 2024-03-19 00:18:02.163482 pref_voting-1.1.0/pref_voting/tests/test_combined_methods.py
+-rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.1.0/pref_voting/tests/test_generate_profiles.py
+-rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.1.0/pref_voting/tests/test_generate_spatial_profile.py
+-rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.1.0/pref_voting/tests/test_io.py
+-rw-r--r--   0        0        0     8943 2024-03-17 11:39:53.682951 pref_voting-1.1.0/pref_voting/tests/test_iterative_methods.py
+-rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.1.0/pref_voting/tests/test_majority_graph.py
+-rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.1.0/pref_voting/tests/test_mapping.py
+-rw-r--r--   0        0        0    10335 2024-04-28 12:01:51.077156 pref_voting-1.1.0/pref_voting/tests/test_margin_based_methods.py
+-rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.1.0/pref_voting/tests/test_margin_graph.py
+-rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.1.0/pref_voting/tests/test_other_methods.py
+-rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.1.0/pref_voting/tests/test_prob_voting_method.py
+-rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.1.0/pref_voting/tests/test_profile.py
+-rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.1.0/pref_voting/tests/test_profile_with_ties.py
+-rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.1.0/pref_voting/tests/test_ranking.py
+-rw-r--r--   0        0        0     5543 2024-03-19 11:54:18.932325 pref_voting-1.1.0/pref_voting/tests/test_scoring_rules.py
+-rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.1.0/pref_voting/tests/test_social_welfare_functions.py
+-rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.1.0/pref_voting/tests/test_spatial_profile.py
+-rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.1.0/pref_voting/tests/test_support_graph.py
+-rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.1.0/pref_voting/tests/test_utility_function.py
+-rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.1.0/pref_voting/tests/test_utility_functions.py
+-rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.1.0/pref_voting/tests/test_voting_method.py
+-rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.1.0/pref_voting/utility_functions.py
+-rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.1.0/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-1.1.0/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.1.0/pref_voting/variable_candidate_axioms.py
+-rw-r--r--   0        0        0    91053 2024-04-27 11:07:33.697481 pref_voting-1.1.0/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     5566 2023-12-07 15:03:17.438046 pref_voting-1.1.0/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      372 2023-11-14 00:06:58.907333 pref_voting-1.1.0/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.1.0/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      760 2024-04-28 12:21:46.030090 pref_voting-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-1.1.0/setup.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-1.1.0/PKG-INFO
```

### Comparing `pref_voting-1.0.0/LICENSE` & `pref_voting-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/README.md` & `pref_voting-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/analysis.py` & `pref_voting-1.1.0/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/axiom.py` & `pref_voting-1.1.0/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/c1_methods.py` & `pref_voting-1.1.0/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/combined_methods.py` & `pref_voting-1.1.0/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/dominance_axioms.py` & `pref_voting-1.1.0/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/generate_profiles.py` & `pref_voting-1.1.0/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/generate_spatial_profiles.py` & `pref_voting-1.1.0/pref_voting/generate_spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/generate_utility_profiles.py` & `pref_voting-1.1.0/pref_voting/generate_utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-1.1.0/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/grade_methods.py` & `pref_voting-1.1.0/pref_voting/grade_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/grade_profiles.py` & `pref_voting-1.1.0/pref_voting/grade_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/helper.py` & `pref_voting-1.1.0/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/invariance_axioms.py` & `pref_voting-1.1.0/pref_voting/invariance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/io/readers.py` & `pref_voting-1.1.0/pref_voting/io/readers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/io/writers.py` & `pref_voting-1.1.0/pref_voting/io/writers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/iterative_methods.py` & `pref_voting-1.1.0/pref_voting/iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/maj_graph_ex1.png` & `pref_voting-1.1.0/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/mappings.py` & `pref_voting-1.1.0/pref_voting/mappings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/margin_based_methods.py` & `pref_voting-1.1.0/pref_voting/margin_based_methods_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,4013 +414,4013 @@
 000019d0: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
 000019e0: 645f 6d65 7468 6f64 732e 6265 6174 5f70  d_methods.beat_p
 000019f0: 6174 685f 466c 6f79 645f 5761 7273 6861  ath_Floyd_Warsha
 00001a00: 6c6c 602c 203a 6d65 7468 3a60 7072 6566  ll`, :meth:`pref
 00001a10: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
 00001a20: 6173 6564 5f6d 6574 686f 6473 2e62 6561  ased_methods.bea
 00001a30: 745f 7061 7468 5f64 6566 6561 7460 0a0a  t_path_defeat`..
-00001a40: 0a20 2020 203a 4578 616d 706c 653a 200a  .    :Example: .
-00001a50: 0a20 2020 202e 2e20 706c 6f74 3a3a 2020  .    .. plot::  
-00001a60: 6d61 7267 696e 5f67 7261 7068 735f 6578  margin_graphs_ex
-00001a70: 616d 706c 6573 2f6d 675f 6578 5f62 705f  amples/mg_ex_bp_
-00001a80: 7270 2e70 790a 2020 2020 2020 2020 3a63  rp.py.        :c
-00001a90: 6f6e 7465 7874 3a20 7265 7365 7420 200a  ontext: reset  .
-00001aa0: 2020 2020 2020 2020 3a69 6e63 6c75 6465          :include
-00001ab0: 2d73 6f75 7263 653a 2054 7275 650a 0a0a  -source: True...
-00001ac0: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
-00001ad0: 6b3a 3a20 0a0a 2020 2020 2020 2020 6672  k:: ..        fr
-00001ae0: 6f6d 2070 7265 665f 766f 7469 6e67 2e6d  om pref_voting.m
-00001af0: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-00001b00: 6f64 7320 696d 706f 7274 2062 6561 745f  ods import beat_
-00001b10: 7061 7468 0a0a 2020 2020 2020 2020 6265  path..        be
-00001b20: 6174 5f70 6174 682e 6469 7370 6c61 7928  at_path.display(
-00001b30: 6d67 290a 0a0a 2020 2020 2e2e 2065 7865  mg)...    .. exe
-00001b40: 635f 636f 6465 3a3a 200a 2020 2020 2020  c_code:: .      
-00001b50: 2020 3a68 6964 655f 636f 6465 3a0a 0a20    :hide_code:.. 
-00001b60: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
-00001b70: 5f76 6f74 696e 672e 7765 6967 6874 6564  _voting.weighted
-00001b80: 5f6d 616a 6f72 6974 795f 6772 6170 6873  _majority_graphs
-00001b90: 2069 6d70 6f72 7420 4d61 7267 696e 4772   import MarginGr
-00001ba0: 6170 680a 2020 2020 2020 2020 6672 6f6d  aph.        from
-00001bb0: 2070 7265 665f 766f 7469 6e67 2e6d 6172   pref_voting.mar
-00001bc0: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
-00001bd0: 7320 696d 706f 7274 2062 6561 745f 7061  s import beat_pa
-00001be0: 7468 0a20 2020 2020 2020 200a 2020 2020  th.        .    
-00001bf0: 2020 2020 6d67 203d 204d 6172 6769 6e47      mg = MarginG
-00001c00: 7261 7068 285b 302c 2031 2c20 322c 2033  raph([0, 1, 2, 3
-00001c10: 5d2c 205b 2830 2c20 322c 2033 292c 2028  ], [(0, 2, 3), (
-00001c20: 312c 2030 2c20 3529 2c20 2832 2c20 312c  1, 0, 5), (2, 1,
-00001c30: 2035 292c 2028 322c 2033 2c20 3129 2c20   5), (2, 3, 1), 
-00001c40: 2833 2c20 302c 2033 292c 2028 332c 2031  (3, 0, 3), (3, 1
-00001c50: 2c20 3129 5d29 0a20 2020 2020 2020 200a  , 1)]).        .
-00001c60: 2020 2020 2020 2020 6265 6174 5f70 6174          beat_pat
-00001c70: 682e 6469 7370 6c61 7928 6d67 290a 0a0a  h.display(mg)...
-00001c80: 2020 2020 2222 220a 0a20 2020 2063 616e      """..    can
-00001c90: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
-00001ca0: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
-00001cb0: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
-00001cc0: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
-00001cd0: 2020 2020 0a20 2020 2073 7472 656e 6774      .    strengt
-00001ce0: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
-00001cf0: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
-00001d00: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
-00001d10: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
-00001d20: 6e67 7468 5f66 756e 6374 696f 6e0a 2020  ngth_function.  
-00001d30: 2020 0a20 2020 206d 6720 3d20 6765 745f    .    mg = get_
-00001d40: 6d67 2865 6461 7461 2c20 6375 7272 5f63  mg(edata, curr_c
-00001d50: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
-00001d60: 7329 0a20 2020 200a 2020 2020 6265 6174  s).    .    beat
-00001d70: 5f70 6174 6873 5f77 6569 6768 7473 203d  _paths_weights =
-00001d80: 207b 633a 207b 6332 3a30 2066 6f72 2063   {c: {c2:0 for c
-00001d90: 3220 696e 2063 616e 6469 6461 7465 7320  2 in candidates 
-00001da0: 6966 2063 3220 213d 2063 7d20 666f 7220  if c2 != c} for 
-00001db0: 6320 696e 2063 616e 6469 6461 7465 737d  c in candidates}
-00001dc0: 0a20 2020 2066 6f72 2063 2069 6e20 6361  .    for c in ca
-00001dd0: 6e64 6964 6174 6573 3a20 0a20 2020 2020  ndidates: .     
-00001de0: 2020 2066 6f72 206f 7468 6572 5f63 2069     for other_c i
-00001df0: 6e20 6265 6174 5f70 6174 6873 5f77 6569  n beat_paths_wei
-00001e00: 6768 7473 5b63 5d2e 6b65 7973 2829 3a0a  ghts[c].keys():.
-00001e10: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00001e20: 7061 7468 7320 3d20 206c 6973 7428 6e78  paths =  list(nx
-00001e30: 2e61 6c6c 5f73 696d 706c 655f 7061 7468  .all_simple_path
-00001e40: 7328 6d67 2c20 632c 206f 7468 6572 5f63  s(mg, c, other_c
-00001e50: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
-00001e60: 6620 6c65 6e28 616c 6c5f 7061 7468 7329  f len(all_paths)
-00001e70: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
-00001e80: 2020 2020 2020 6265 6174 5f70 6174 6873        beat_paths
-00001e90: 5f77 6569 6768 7473 5b63 5d5b 6f74 6865  _weights[c][othe
-00001ea0: 725f 635d 203d 206d 6178 285b 6d69 6e28  r_c] = max([min(
-00001eb0: 5b73 7472 656e 6774 685f 6675 6e63 7469  [strength_functi
-00001ec0: 6f6e 2870 5b69 5d2c 2070 5b69 2b31 5d29  on(p[i], p[i+1])
-00001ed0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00001ee0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00001ef0: 2830 2c6c 656e 2870 292d 3129 5d29 200a  (0,len(p)-1)]) .
-00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f10: 666f 7220 7020 696e 2061 6c6c 5f70 6174  for p in all_pat
-00001f20: 6873 5d29 0a20 2020 200a 2020 2020 7769  hs]).    .    wi
-00001f30: 6e6e 6572 7320 3d20 6c69 7374 2829 0a20  nners = list(). 
-00001f40: 2020 2066 6f72 2063 2069 6e20 6361 6e64     for c in cand
-00001f50: 6964 6174 6573 3a20 0a20 2020 2020 2020  idates: .       
-00001f60: 2069 6620 616c 6c28 5b62 6561 745f 7061   if all([beat_pa
-00001f70: 7468 735f 7765 6967 6874 735b 635d 5b63  ths_weights[c][c
-00001f80: 325d 203e 3d20 6265 6174 5f70 6174 6873  2] >= beat_paths
-00001f90: 5f77 6569 6768 7473 5b63 325d 5b63 5d20  _weights[c2][c] 
-00001fa0: 666f 7220 6332 2069 6e20 6361 6e64 6964  for c2 in candid
-00001fb0: 6174 6573 2020 6966 2063 3220 213d 2063  ates  if c2 != c
-00001fc0: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-00001fd0: 7769 6e6e 6572 732e 6170 7065 6e64 2863  winners.append(c
-00001fe0: 290a 2020 2020 7265 7475 726e 2073 6f72  ).    return sor
-00001ff0: 7465 6428 6c69 7374 2877 696e 6e65 7273  ted(list(winners
-00002000: 2929 0a0a 0a40 766d 286e 616d 653d 2242  ))...@vm(name="B
-00002010: 6561 7420 5061 7468 2229 0a64 6566 2062  eat Path").def b
-00002020: 6561 745f 7061 7468 5f46 6c6f 7964 5f57  eat_path_Floyd_W
-00002030: 6172 7368 616c 6c28 6564 6174 612c 2063  arshall(edata, c
-00002040: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
-00002050: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
-00002060: 696f 6e20 3d20 4e6f 6e65 293a 2020 200a  ion = None):   .
-00002070: 2020 2020 2222 2241 6e20 696d 706c 656d      """An implem
-00002080: 656e 7461 7469 6f6e 206f 6620 4265 6174  entation of Beat
-00002090: 2050 6174 6820 7573 696e 6720 6120 7661   Path using a va
-000020a0: 7269 6174 696f 6e20 6f66 2074 6865 2046  riation of the F
-000020b0: 6c6f 7964 2d57 6172 7368 616c 6c20 416c  loyd-Warshall Al
-000020c0: 676f 7269 7468 6d0a 2020 2020 5365 6520  gorithm.    See 
-000020d0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-000020e0: 6564 6961 2e6f 7267 2f77 696b 692f 5363  edia.org/wiki/Sc
-000020f0: 6875 6c7a 655f 6d65 7468 6f64 2349 6d70  hulze_method#Imp
-00002100: 6c65 6d65 6e74 6174 696f 6e29 0a20 0a20  lementation). . 
-00002110: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00002120: 2065 6461 7461 2028 5072 6f66 696c 652c   edata (Profile,
-00002130: 2050 726f 6669 6c65 5769 7468 5469 6573   ProfileWithTies
-00002140: 2c20 4d61 7267 696e 4772 6170 6829 3a20  , MarginGraph): 
-00002150: 416e 7920 656c 6563 7469 6f6e 2064 6174  Any election dat
-00002160: 6120 7468 6174 2068 6173 2061 2060 6d61  a that has a `ma
-00002170: 7267 696e 6020 6d65 7468 6f64 2e20 0a20  rgin` method. . 
-00002180: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
-00002190: 7320 284c 6973 745b 696e 745d 2c20 6f70  s (List[int], op
-000021a0: 7469 6f6e 616c 293a 2049 6620 7365 742c  tional): If set,
-000021b0: 2074 6865 6e20 6669 6e64 2074 6865 2077   then find the w
-000021c0: 696e 6e65 7273 2066 6f72 2074 6865 2070  inners for the p
-000021d0: 726f 6669 6c65 2072 6573 7472 6963 7465  rofile restricte
-000021e0: 6420 746f 2074 6865 2063 616e 6469 6461  d to the candida
-000021f0: 7465 7320 696e 2060 6063 7572 725f 6361  tes in ``curr_ca
-00002200: 6e64 7360 600a 2020 2020 2020 2020 7374  nds``.        st
-00002210: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-00002220: 2866 756e 6374 696f 6e2c 206f 7074 696f  (function, optio
-00002230: 6e61 6c29 3a20 5468 6520 7374 7265 6e67  nal): The streng
-00002240: 7468 2066 756e 6374 696f 6e20 746f 2062  th function to b
-00002250: 6520 7573 6564 2074 6f20 6361 6c63 756c  e used to calcul
-00002260: 6174 6520 7468 6520 7374 7265 6e67 7468  ate the strength
-00002270: 206f 6620 6120 7061 7468 2e20 2020 5468   of a path.   Th
-00002280: 6520 6465 6661 756c 7420 6973 2074 6865  e default is the
-00002290: 206d 6172 6769 6e20 6d65 7468 6f64 206f   margin method o
-000022a0: 6620 6060 6564 6174 6160 602e 2020 2054  f ``edata``.   T
-000022b0: 6869 7320 6f6e 6c79 206d 6174 7465 7273  his only matters
-000022c0: 2077 6865 6e20 7468 6520 6261 6c6c 6f74   when the ballot
-000022d0: 7320 6172 6520 6e6f 7420 6c69 6e65 6172  s are not linear
-000022e0: 206f 7264 6572 732e 200a 0a20 2020 2052   orders. ..    R
-000022f0: 6574 7572 6e73 3a20 0a20 2020 2020 2020  eturns: .       
-00002300: 2041 2073 6f72 7465 6420 6c69 7374 206f   A sorted list o
-00002310: 6620 6361 6e64 6964 6174 6573 2e20 0a0a  f candidates. ..
-00002320: 2020 2020 2e2e 2073 6565 616c 736f 3a3a      .. seealso::
-00002330: 0a0a 2020 2020 2020 2020 3a6d 6574 683a  ..        :meth:
-00002340: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
-00002350: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
-00002360: 732e 6265 6174 5f70 6174 6860 2c20 3a6d  s.beat_path`, :m
-00002370: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
-00002380: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-00002390: 7468 6f64 732e 6265 6174 5f70 6174 685f  thods.beat_path_
-000023a0: 6465 6665 6174 600a 0a0a 2020 2020 3a45  defeat`...    :E
-000023b0: 7861 6d70 6c65 3a20 0a0a 2020 2020 2e2e  xample: ..    ..
-000023c0: 2070 6c6f 743a 3a20 206d 6172 6769 6e5f   plot::  margin_
-000023d0: 6772 6170 6873 5f65 7861 6d70 6c65 732f  graphs_examples/
-000023e0: 6d67 5f65 785f 6270 5f72 702e 7079 0a20  mg_ex_bp_rp.py. 
-000023f0: 2020 2020 2020 203a 636f 6e74 6578 743a         :context:
-00002400: 2072 6573 6574 2020 0a20 2020 2020 2020   reset  .       
-00002410: 203a 696e 636c 7564 652d 736f 7572 6365   :include-source
-00002420: 3a20 5472 7565 0a0a 0a20 2020 202e 2e20  : True...    .. 
-00002430: 636f 6465 2d62 6c6f 636b 3a3a 200a 0a20  code-block:: .. 
-00002440: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
-00002450: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
-00002460: 6173 6564 5f6d 6574 686f 6473 2069 6d70  ased_methods imp
-00002470: 6f72 7420 6265 6174 5f70 6174 685f 466c  ort beat_path_Fl
-00002480: 6f79 645f 5761 7273 6861 6c6c 0a0a 2020  oyd_Warshall..  
-00002490: 2020 2020 2020 6265 6174 5f70 6174 682e        beat_path.
-000024a0: 6469 7370 6c61 7928 6d67 290a 2020 2020  display(mg).    
-000024b0: 2020 2020 6265 6174 5f70 6174 685f 466c      beat_path_Fl
-000024c0: 6f79 645f 5761 7273 6861 6c6c 2e64 6973  oyd_Warshall.dis
-000024d0: 706c 6179 286d 6729 0a0a 0a20 2020 202e  play(mg)...    .
-000024e0: 2e20 6578 6563 5f63 6f64 653a 3a20 0a20  . exec_code:: . 
-000024f0: 2020 2020 2020 203a 6869 6465 5f63 6f64         :hide_cod
-00002500: 653a 0a0a 2020 2020 2020 2020 6672 6f6d  e:..        from
-00002510: 2070 7265 665f 766f 7469 6e67 2e77 6569   pref_voting.wei
-00002520: 6768 7465 645f 6d61 6a6f 7269 7479 5f67  ghted_majority_g
-00002530: 7261 7068 7320 696d 706f 7274 204d 6172  raphs import Mar
-00002540: 6769 6e47 7261 7068 0a20 2020 2020 2020  ginGraph.       
-00002550: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
-00002560: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-00002570: 6574 686f 6473 2069 6d70 6f72 7420 6265  ethods import be
-00002580: 6174 5f70 6174 682c 2062 6561 745f 7061  at_path, beat_pa
-00002590: 7468 5f46 6c6f 7964 5f57 6172 7368 616c  th_Floyd_Warshal
-000025a0: 6c0a 2020 2020 2020 2020 0a20 2020 2020  l.        .     
-000025b0: 2020 206d 6720 3d20 4d61 7267 696e 4772     mg = MarginGr
-000025c0: 6170 6828 5b30 2c20 312c 2032 2c20 335d  aph([0, 1, 2, 3]
-000025d0: 2c20 5b28 302c 2032 2c20 3329 2c20 2831  , [(0, 2, 3), (1
-000025e0: 2c20 302c 2035 292c 2028 322c 2031 2c20  , 0, 5), (2, 1, 
-000025f0: 3529 2c20 2832 2c20 332c 2031 292c 2028  5), (2, 3, 1), (
-00002600: 332c 2030 2c20 3329 2c20 2833 2c20 312c  3, 0, 3), (3, 1,
-00002610: 2031 295d 290a 0a20 2020 2020 2020 2062   1)])..        b
-00002620: 6561 745f 7061 7468 2e64 6973 706c 6179  eat_path.display
-00002630: 286d 6729 0a20 2020 2020 2020 2062 6561  (mg).        bea
-00002640: 745f 7061 7468 5f46 6c6f 7964 5f57 6172  t_path_Floyd_War
-00002650: 7368 616c 6c2e 6469 7370 6c61 7928 6d67  shall.display(mg
-00002660: 290a 0a20 2020 2022 2222 0a0a 2020 2020  )..    """..    
-00002670: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
-00002680: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
-00002690: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
-000026a0: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
-000026b0: 6e64 7320 2020 200a 2020 2020 7374 7265  nds    .    stre
-000026c0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-000026d0: 6564 6174 612e 6d61 7267 696e 2069 6620  edata.margin if 
-000026e0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-000026f0: 6e20 6973 204e 6f6e 6520 656c 7365 2073  n is None else s
-00002700: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00002710: 0a20 2020 2020 2020 200a 2020 2020 735f  .        .    s_
-00002720: 6d61 7472 6978 203d 205b 5b2d 6e70 2e69  matrix = [[-np.i
-00002730: 6e66 2066 6f72 205f 2069 6e20 6361 6e64  nf for _ in cand
-00002740: 6964 6174 6573 5d20 666f 7220 5f20 696e  idates] for _ in
-00002750: 2063 616e 6469 6461 7465 735d 0a20 2020   candidates].   
-00002760: 2066 6f72 2063 315f 6964 782c 2063 3120   for c1_idx, c1 
-00002770: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
-00002780: 6469 6461 7465 7329 3a0a 2020 2020 2020  didates):.      
-00002790: 2020 666f 7220 6332 5f69 6478 2c20 6332    for c2_idx, c2
-000027a0: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-000027b0: 6e64 6964 6174 6573 293a 0a20 2020 2020  ndidates):.     
-000027c0: 2020 2020 2020 2069 6620 2865 6461 7461         if (edata
-000027d0: 2e6d 616a 6f72 6974 795f 7072 6566 6572  .majority_prefer
-000027e0: 7328 6331 2c20 6332 2920 6f72 2063 3120  s(c1, c2) or c1 
-000027f0: 3d3d 2063 3229 3a0a 2020 2020 2020 2020  == c2):.        
-00002800: 2020 2020 2020 2020 735f 6d61 7472 6978          s_matrix
-00002810: 5b63 315f 6964 785d 5b63 325f 6964 785d  [c1_idx][c2_idx]
-00002820: 203d 2073 7472 656e 6774 685f 6675 6e63   = strength_func
-00002830: 7469 6f6e 2863 312c 2063 3229 200a 2020  tion(c1, c2) .  
-00002840: 2020 7374 7265 6e67 7468 203d 206c 6973    strength = lis
-00002850: 7428 6d61 7028 6c61 6d62 6461 2069 203a  t(map(lambda i :
-00002860: 206c 6973 7428 6d61 7028 6c61 6d62 6461   list(map(lambda
-00002870: 206a 203a 206a 202c 2069 2929 202c 2073   j : j , i)) , s
-00002880: 5f6d 6174 7269 7829 290a 2020 2020 666f  _matrix)).    fo
-00002890: 7220 695f 6964 782c 2069 2069 6e20 656e  r i_idx, i in en
-000028a0: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
-000028b0: 6573 293a 2020 2020 2020 2020 200a 2020  es):         .  
-000028c0: 2020 2020 2020 666f 7220 6a5f 6964 782c        for j_idx,
-000028d0: 206a 2069 6e20 656e 756d 6572 6174 6528   j in enumerate(
-000028e0: 6361 6e64 6964 6174 6573 293a 200a 2020  candidates): .  
-000028f0: 2020 2020 2020 2020 2020 6966 2069 213d            if i!=
-00002900: 206a 3a0a 2020 2020 2020 2020 2020 2020   j:.            
-00002910: 2020 2020 666f 7220 6b5f 6964 782c 206b      for k_idx, k
-00002920: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-00002930: 6e64 6964 6174 6573 293a 200a 2020 2020  ndidates): .    
-00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002950: 6966 2069 213d 206b 2061 6e64 206a 2021  if i!= k and j !
-00002960: 3d20 6b3a 0a20 2020 2020 2020 2020 2020  = k:.           
-00002970: 2020 2020 2020 2020 2020 2020 2073 7472               str
-00002980: 656e 6774 685b 6a5f 6964 785d 5b6b 5f69  ength[j_idx][k_i
-00002990: 6478 5d20 3d20 6d61 7828 7374 7265 6e67  dx] = max(streng
-000029a0: 7468 5b6a 5f69 6478 5d5b 6b5f 6964 785d  th[j_idx][k_idx]
-000029b0: 2c20 6d69 6e28 7374 7265 6e67 7468 5b6a  , min(strength[j
-000029c0: 5f69 6478 5d5b 695f 6964 785d 2c73 7472  _idx][i_idx],str
-000029d0: 656e 6774 685b 695f 6964 785d 5b6b 5f69  ength[i_idx][k_i
-000029e0: 6478 5d29 290a 2020 2020 7769 6e6e 6572  dx])).    winner
-000029f0: 7320 3d20 7b69 3a54 7275 6520 666f 7220  s = {i:True for 
-00002a00: 6920 696e 2063 616e 6469 6461 7465 737d  i in candidates}
-00002a10: 0a20 2020 2066 6f72 2069 5f69 6478 2c20  .    for i_idx, 
-00002a20: 6920 696e 2065 6e75 6d65 7261 7465 2863  i in enumerate(c
-00002a30: 616e 6469 6461 7465 7329 3a20 0a20 2020  andidates): .   
-00002a40: 2020 2020 2066 6f72 206a 5f69 6478 2c20       for j_idx, 
-00002a50: 6a20 696e 2065 6e75 6d65 7261 7465 2863  j in enumerate(c
-00002a60: 616e 6469 6461 7465 7329 3a0a 2020 2020  andidates):.    
-00002a70: 2020 2020 2020 2020 6966 2069 213d 6a3a          if i!=j:
-00002a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a90: 2069 6620 7374 7265 6e67 7468 5b6a 5f69   if strength[j_i
-00002aa0: 6478 5d5b 695f 6964 785d 203e 2073 7472  dx][i_idx] > str
-00002ab0: 656e 6774 685b 695f 6964 785d 5b6a 5f69  ength[i_idx][j_i
-00002ac0: 6478 5d3a 0a20 2020 2020 2020 2020 2020  dx]:.           
-00002ad0: 2020 2020 2020 2020 2077 696e 6e65 7273           winners
-00002ae0: 5b69 5d20 3d20 4661 6c73 650a 2020 2020  [i] = False.    
-00002af0: 7265 7475 726e 2073 6f72 7465 6428 5b63  return sorted([c
-00002b00: 2066 6f72 2063 2069 6e20 6361 6e64 6964   for c in candid
-00002b10: 6174 6573 2069 6620 7769 6e6e 6572 735b  ates if winners[
-00002b20: 635d 5d29 0a0a 6465 6620 6265 6174 5f70  c]])..def beat_p
-00002b30: 6174 685f 6465 6665 6174 2865 6461 7461  ath_defeat(edata
-00002b40: 2c20 6375 7272 5f63 616e 6473 203d 204e  , curr_cands = N
-00002b50: 6f6e 652c 2073 7472 656e 6774 685f 6675  one, strength_fu
-00002b60: 6e63 7469 6f6e 203d 204e 6f6e 6529 3a20  nction = None): 
-00002b70: 2020 0a20 2020 2022 2222 5265 7475 726e    .    """Return
-00002b80: 7320 7468 6520 6465 6665 6174 2072 656c  s the defeat rel
-00002b90: 6174 696f 6e20 666f 7220 4265 6174 2050  ation for Beat P
-00002ba0: 6174 682e 200a 2020 2020 0a20 2020 2041  ath. .    .    A
-00002bb0: 7267 733a 0a20 2020 2020 2020 2065 6461  rgs:.        eda
-00002bc0: 7461 2028 5072 6f66 696c 652c 2050 726f  ta (Profile, Pro
-00002bd0: 6669 6c65 5769 7468 5469 6573 2c20 4d61  fileWithTies, Ma
-00002be0: 7267 696e 4772 6170 6829 3a20 416e 7920  rginGraph): Any 
-00002bf0: 656c 6563 7469 6f6e 2064 6174 6120 7468  election data th
-00002c00: 6174 2068 6173 2061 2060 6d61 7267 696e  at has a `margin
-00002c10: 6020 6d65 7468 6f64 2e20 0a20 2020 2020  ` method. .     
-00002c20: 2020 2063 7572 725f 6361 6e64 7320 284c     curr_cands (L
-00002c30: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
-00002c40: 616c 293a 2049 6620 7365 742c 2074 6865  al): If set, the
-00002c50: 6e20 6669 6e64 2074 6865 2077 696e 6e65  n find the winne
-00002c60: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
-00002c70: 6c65 2072 6573 7472 6963 7465 6420 746f  le restricted to
-00002c80: 2074 6865 2063 616e 6469 6461 7465 7320   the candidates 
-00002c90: 696e 2060 6063 7572 725f 6361 6e64 7360  in ``curr_cands`
-00002ca0: 600a 2020 2020 2020 2020 7374 7265 6e67  `.        streng
-00002cb0: 7468 5f66 756e 6374 696f 6e20 2866 756e  th_function (fun
-00002cc0: 6374 696f 6e2c 206f 7074 696f 6e61 6c29  ction, optional)
-00002cd0: 3a20 5468 6520 7374 7265 6e67 7468 2066  : The strength f
-00002ce0: 756e 6374 696f 6e20 746f 2062 6520 7573  unction to be us
-00002cf0: 6564 2074 6f20 6361 6c63 756c 6174 6520  ed to calculate 
-00002d00: 7468 6520 7374 7265 6e67 7468 206f 6620  the strength of 
-00002d10: 6120 7061 7468 2e20 2020 5468 6520 6465  a path.   The de
-00002d20: 6661 756c 7420 6973 2074 6865 206d 6172  fault is the mar
-00002d30: 6769 6e20 6d65 7468 6f64 206f 6620 6060  gin method of ``
-00002d40: 6564 6174 6160 602e 2020 2054 6869 7320  edata``.   This 
-00002d50: 6f6e 6c79 206d 6174 7465 7273 2077 6865  only matters whe
-00002d60: 6e20 7468 6520 6261 6c6c 6f74 7320 6172  n the ballots ar
-00002d70: 6520 6e6f 7420 6c69 6e65 6172 206f 7264  e not linear ord
-00002d80: 6572 732e 200a 0a20 2020 2052 6574 7572  ers. ..    Retur
-00002d90: 6e73 3a20 0a20 2020 2020 2020 2041 206e  ns: .        A n
-00002da0: 6574 776f 726b 7820 4469 4772 6170 6820  etworkx DiGraph 
-00002db0: 7265 7072 6573 656e 7469 6e67 2074 6865  representing the
-00002dc0: 2042 6561 7420 5061 7468 2064 6566 6561   Beat Path defea
-00002dd0: 7420 7265 6c61 7469 6f6e 2e20 0a0a 2020  t relation. ..  
-00002de0: 2020 2e2e 2073 6565 616c 736f 3a3a 0a0a    .. seealso::..
-00002df0: 2020 2020 2020 2020 3a6d 6574 683a 6070          :meth:`p
-00002e00: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-00002e10: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-00002e20: 6265 6174 5f70 6174 6860 2c20 3a6d 6574  beat_path`, :met
-00002e30: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
-00002e40: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-00002e50: 6f64 732e 6265 6174 5f70 6174 685f 466c  ods.beat_path_Fl
-00002e60: 6f79 645f 5761 7273 6861 6c6c 600a 0a20  oyd_Warshall`.. 
-00002e70: 2020 203a 4578 616d 706c 653a 200a 0a20     :Example: .. 
-00002e80: 2020 202e 2e20 706c 6f74 3a3a 2020 6d61     .. plot::  ma
-00002e90: 7267 696e 5f67 7261 7068 735f 6578 616d  rgin_graphs_exam
-00002ea0: 706c 6573 2f6d 675f 6578 5f62 705f 6465  ples/mg_ex_bp_de
-00002eb0: 6665 6174 2e70 790a 2020 2020 2020 2020  feat.py.        
-00002ec0: 3a63 6f6e 7465 7874 3a20 7265 7365 7420  :context: reset 
-00002ed0: 200a 2020 2020 2020 2020 3a69 6e63 6c75   .        :inclu
-00002ee0: 6465 2d73 6f75 7263 653a 2054 7275 650a  de-source: True.
-00002ef0: 0a20 2020 2022 2222 0a0a 2020 2020 6361  .    """..    ca
-00002f00: 6e64 6964 6174 6573 203d 2065 6461 7461  ndidates = edata
-00002f10: 2e63 616e 6469 6461 7465 7320 6966 2063  .candidates if c
-00002f20: 7572 725f 6361 6e64 7320 6973 204e 6f6e  urr_cands is Non
-00002f30: 6520 656c 7365 2063 7572 725f 6361 6e64  e else curr_cand
-00002f40: 7320 2020 200a 2020 2020 7374 7265 6e67  s    .    streng
-00002f50: 7468 5f66 756e 6374 696f 6e20 3d20 6564  th_function = ed
-00002f60: 6174 612e 6d61 7267 696e 2069 6620 7374  ata.margin if st
-00002f70: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-00002f80: 6973 204e 6f6e 6520 656c 7365 2073 7472  is None else str
-00002f90: 656e 6774 685f 6675 6e63 7469 6f6e 0a20  ength_function. 
-00002fa0: 2020 2020 2020 200a 2020 2020 735f 6d61         .    s_ma
-00002fb0: 7472 6978 203d 205b 5b2d 6e70 2e69 6e66  trix = [[-np.inf
-00002fc0: 2066 6f72 205f 2069 6e20 6361 6e64 6964   for _ in candid
-00002fd0: 6174 6573 5d20 666f 7220 5f20 696e 2063  ates] for _ in c
-00002fe0: 616e 6469 6461 7465 735d 0a20 2020 2066  andidates].    f
-00002ff0: 6f72 2063 315f 6964 782c 2063 3120 696e  or c1_idx, c1 in
-00003000: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
-00003010: 6461 7465 7329 3a0a 2020 2020 2020 2020  dates):.        
-00003020: 666f 7220 6332 5f69 6478 2c20 6332 2069  for c2_idx, c2 i
-00003030: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
-00003040: 6964 6174 6573 293a 0a20 2020 2020 2020  idates):.       
-00003050: 2020 2020 2069 6620 2865 6461 7461 2e6d       if (edata.m
-00003060: 616a 6f72 6974 795f 7072 6566 6572 7328  ajority_prefers(
-00003070: 6331 2c20 6332 2920 6f72 2063 3120 3d3d  c1, c2) or c1 ==
-00003080: 2063 3229 3a0a 2020 2020 2020 2020 2020   c2):.          
-00003090: 2020 2020 2020 735f 6d61 7472 6978 5b63        s_matrix[c
-000030a0: 315f 6964 785d 5b63 325f 6964 785d 203d  1_idx][c2_idx] =
-000030b0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-000030c0: 6f6e 2863 312c 2063 3229 200a 2020 2020  on(c1, c2) .    
-000030d0: 7374 7265 6e67 7468 203d 206c 6973 7428  strength = list(
-000030e0: 6d61 7028 6c61 6d62 6461 2069 203a 206c  map(lambda i : l
-000030f0: 6973 7428 6d61 7028 6c61 6d62 6461 206a  ist(map(lambda j
-00003100: 203a 206a 202c 2069 2929 202c 2073 5f6d   : j , i)) , s_m
-00003110: 6174 7269 7829 290a 2020 2020 666f 7220  atrix)).    for 
-00003120: 695f 6964 782c 2069 2069 6e20 656e 756d  i_idx, i in enum
-00003130: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
-00003140: 293a 2020 2020 2020 2020 200a 2020 2020  ):         .    
-00003150: 2020 2020 666f 7220 6a5f 6964 782c 206a      for j_idx, j
-00003160: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-00003170: 6e64 6964 6174 6573 293a 200a 2020 2020  ndidates): .    
-00003180: 2020 2020 2020 2020 6966 2069 213d 206a          if i!= j
-00003190: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000031a0: 2020 666f 7220 6b5f 6964 782c 206b 2069    for k_idx, k i
-000031b0: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
-000031c0: 6964 6174 6573 293a 200a 2020 2020 2020  idates): .      
-000031d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000031e0: 2069 213d 206b 2061 6e64 206a 2021 3d20   i!= k and j != 
-000031f0: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
-00003200: 2020 2020 2020 2020 2020 2073 7472 656e             stren
-00003210: 6774 685b 6a5f 6964 785d 5b6b 5f69 6478  gth[j_idx][k_idx
-00003220: 5d20 3d20 6d61 7828 7374 7265 6e67 7468  ] = max(strength
-00003230: 5b6a 5f69 6478 5d5b 6b5f 6964 785d 2c20  [j_idx][k_idx], 
-00003240: 6d69 6e28 7374 7265 6e67 7468 5b6a 5f69  min(strength[j_i
-00003250: 6478 5d5b 695f 6964 785d 2c73 7472 656e  dx][i_idx],stren
-00003260: 6774 685b 695f 6964 785d 5b6b 5f69 6478  gth[i_idx][k_idx
-00003270: 5d29 290a 0a20 2020 2064 6566 6561 745f  ]))..    defeat_
-00003280: 6772 6170 6820 3d20 6e78 2e44 6947 7261  graph = nx.DiGra
-00003290: 7068 2829 0a20 2020 2064 6566 6561 745f  ph().    defeat_
-000032a0: 6772 6170 682e 6164 645f 6e6f 6465 735f  graph.add_nodes_
-000032b0: 6672 6f6d 2863 616e 6469 6461 7465 7329  from(candidates)
-000032c0: 0a20 2020 200a 2020 2020 666f 7220 695f  .    .    for i_
-000032d0: 6964 782c 2069 2069 6e20 656e 756d 6572  idx, i in enumer
-000032e0: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
-000032f0: 200a 2020 2020 2020 2020 666f 7220 6a5f   .        for j_
-00003300: 6964 782c 206a 2069 6e20 656e 756d 6572  idx, j in enumer
-00003310: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
-00003320: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003330: 6921 3d6a 3a0a 2020 2020 2020 2020 2020  i!=j:.          
-00003340: 2020 2020 2020 6966 2073 7472 656e 6774        if strengt
-00003350: 685b 6a5f 6964 785d 5b69 5f69 6478 5d20  h[j_idx][i_idx] 
-00003360: 3e20 7374 7265 6e67 7468 5b69 5f69 6478  > strength[i_idx
-00003370: 5d5b 6a5f 6964 785d 3a0a 2020 2020 2020  ][j_idx]:.      
-00003380: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00003390: 6665 6174 5f67 7261 7068 2e61 6464 5f77  feat_graph.add_w
-000033a0: 6569 6768 7465 645f 6564 6765 735f 6672  eighted_edges_fr
-000033b0: 6f6d 285b 286a 2c69 2c73 5f6d 6174 7269  om([(j,i,s_matri
-000033c0: 785b 6a5f 6964 785d 5b69 5f69 6478 5d29  x[j_idx][i_idx])
-000033d0: 5d29 0a0a 2020 2020 7265 7475 726e 2064  ])..    return d
-000033e0: 6566 6561 745f 6772 6170 680a 2020 2020  efeat_graph.    
-000033f0: 0a64 6566 2068 6173 5f73 7472 6f6e 675f  .def has_strong_
-00003400: 7061 7468 2841 2c20 736f 7572 6365 2c20  path(A, source, 
-00003410: 7461 7267 6574 2c20 6b29 3a0a 2020 2020  target, k):.    
-00003420: 2222 2247 6976 656e 2061 2073 7175 6172  """Given a squar
-00003430: 6520 6d61 7472 6978 2041 2c20 7265 7475  e matrix A, retu
-00003440: 726e 2054 7275 6520 6966 2074 6865 7265  rn True if there
-00003450: 2069 7320 6120 7061 7468 2066 726f 6d20   is a path from 
-00003460: 736f 7572 6365 2074 6f20 7461 7267 6574  source to target
-00003470: 2069 6e20 7468 6520 6173 736f 6369 6174   in the associat
-00003480: 6564 2064 6972 6563 7465 6420 6772 6170  ed directed grap
-00003490: 6820 2020 2020 7768 6572 6520 6561 6368  h     where each
-000034a0: 2065 6467 6520 6861 7320 6120 7765 6967   edge has a weig
-000034b0: 6874 2067 7265 6174 6572 2074 6861 6e20  ht greater than 
-000034c0: 6f72 2065 7175 616c 2074 6f20 6b2c 2061  or equal to k, a
-000034d0: 6e64 2046 616c 7365 206f 7468 6572 7769  nd False otherwi
-000034e0: 7365 2e22 2222 0a20 2020 200a 2020 2020  se.""".    .    
-000034f0: 6e20 3d20 412e 7368 6170 655b 305d 2023  n = A.shape[0] #
-00003500: 2061 7373 756d 6520 4120 6973 2061 2073   assume A is a s
-00003510: 7175 6172 6520 6d61 7472 6978 0a20 2020  quare matrix.   
-00003520: 2076 6973 6974 6564 203d 206e 702e 7a65   visited = np.ze
-00003530: 726f 7328 6e2c 2064 7479 7065 3d62 6f6f  ros(n, dtype=boo
-00003540: 6c29 0a0a 2020 2020 6465 6620 6466 7328  l)..    def dfs(
-00003550: 6e6f 6465 293a 0a20 2020 2020 2020 2069  node):.        i
-00003560: 6620 6e6f 6465 203d 3d20 7461 7267 6574  f node == target
-00003570: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00003580: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-00003590: 2020 7669 7369 7465 645b 6e6f 6465 5d20    visited[node] 
-000035a0: 3d20 5472 7565 0a20 2020 2020 2020 2066  = True.        f
-000035b0: 6f72 206e 6569 6768 626f 722c 2077 6569  or neighbor, wei
-000035c0: 6768 7420 696e 2065 6e75 6d65 7261 7465  ght in enumerate
-000035d0: 2841 5b6e 6f64 652c 203a 5d29 3a0a 2020  (A[node, :]):.  
-000035e0: 2020 2020 2020 2020 2020 6966 2041 5b6e            if A[n
-000035f0: 6f64 655d 5b6e 6569 6768 626f 725d 203e  ode][neighbor] >
-00003600: 2041 5b6e 6569 6768 626f 725d 5b6e 6f64   A[neighbor][nod
-00003610: 655d 2061 6e64 2077 6569 6768 7420 3e3d  e] and weight >=
-00003620: 206b 2061 6e64 206e 6f74 2076 6973 6974   k and not visit
-00003630: 6564 5b6e 6569 6768 626f 725d 3a0a 2020  ed[neighbor]:.  
-00003640: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00003650: 2064 6673 286e 6569 6768 626f 7229 3a0a   dfs(neighbor):.
+00001a40: 2020 2020 3a45 7861 6d70 6c65 3a20 0a0a      :Example: ..
+00001a50: 2020 2020 2e2e 2070 6c6f 743a 3a20 206d      .. plot::  m
+00001a60: 6172 6769 6e5f 6772 6170 6873 5f65 7861  argin_graphs_exa
+00001a70: 6d70 6c65 732f 6d67 5f65 785f 6270 5f72  mples/mg_ex_bp_r
+00001a80: 702e 7079 0a20 2020 2020 2020 203a 636f  p.py.        :co
+00001a90: 6e74 6578 743a 2072 6573 6574 2020 0a20  ntext: reset  . 
+00001aa0: 2020 2020 2020 203a 696e 636c 7564 652d         :include-
+00001ab0: 736f 7572 6365 3a20 5472 7565 0a0a 0a20  source: True... 
+00001ac0: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+00001ad0: 3a3a 200a 0a20 2020 2020 2020 2066 726f  :: ..        fro
+00001ae0: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
+00001af0: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+00001b00: 6473 2069 6d70 6f72 7420 6265 6174 5f70  ds import beat_p
+00001b10: 6174 680a 0a20 2020 2020 2020 2062 6561  ath..        bea
+00001b20: 745f 7061 7468 2e64 6973 706c 6179 286d  t_path.display(m
+00001b30: 6729 0a0a 0a20 2020 202e 2e20 6578 6563  g)...    .. exec
+00001b40: 5f63 6f64 653a 3a20 0a20 2020 2020 2020  _code:: .       
+00001b50: 203a 6869 6465 5f63 6f64 653a 0a0a 2020   :hide_code:..  
+00001b60: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+00001b70: 766f 7469 6e67 2e77 6569 6768 7465 645f  voting.weighted_
+00001b80: 6d61 6a6f 7269 7479 5f67 7261 7068 7320  majority_graphs 
+00001b90: 696d 706f 7274 204d 6172 6769 6e47 7261  import MarginGra
+00001ba0: 7068 0a20 2020 2020 2020 2066 726f 6d20  ph.        from 
+00001bb0: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+00001bc0: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+00001bd0: 2069 6d70 6f72 7420 6265 6174 5f70 6174   import beat_pat
+00001be0: 680a 2020 2020 2020 2020 0a20 2020 2020  h.        .     
+00001bf0: 2020 206d 6720 3d20 4d61 7267 696e 4772     mg = MarginGr
+00001c00: 6170 6828 5b30 2c20 312c 2032 2c20 335d  aph([0, 1, 2, 3]
+00001c10: 2c20 5b28 302c 2032 2c20 3329 2c20 2831  , [(0, 2, 3), (1
+00001c20: 2c20 302c 2035 292c 2028 322c 2031 2c20  , 0, 5), (2, 1, 
+00001c30: 3529 2c20 2832 2c20 332c 2031 292c 2028  5), (2, 3, 1), (
+00001c40: 332c 2030 2c20 3329 2c20 2833 2c20 312c  3, 0, 3), (3, 1,
+00001c50: 2031 295d 290a 2020 2020 2020 2020 0a20   1)]).        . 
+00001c60: 2020 2020 2020 2062 6561 745f 7061 7468         beat_path
+00001c70: 2e64 6973 706c 6179 286d 6729 0a0a 0a20  .display(mg)... 
+00001c80: 2020 2022 2222 0a0a 2020 2020 6361 6e64     """..    cand
+00001c90: 6964 6174 6573 203d 2065 6461 7461 2e63  idates = edata.c
+00001ca0: 616e 6469 6461 7465 7320 6966 2063 7572  andidates if cur
+00001cb0: 725f 6361 6e64 7320 6973 204e 6f6e 6520  r_cands is None 
+00001cc0: 656c 7365 2063 7572 725f 6361 6e64 7320  else curr_cands 
+00001cd0: 2020 200a 2020 2020 7374 7265 6e67 7468     .    strength
+00001ce0: 5f66 756e 6374 696f 6e20 3d20 6564 6174  _function = edat
+00001cf0: 612e 6d61 7267 696e 2069 6620 7374 7265  a.margin if stre
+00001d00: 6e67 7468 5f66 756e 6374 696f 6e20 6973  ngth_function is
+00001d10: 204e 6f6e 6520 656c 7365 2073 7472 656e   None else stren
+00001d20: 6774 685f 6675 6e63 7469 6f6e 0a20 2020  gth_function.   
+00001d30: 200a 2020 2020 6d67 203d 2067 6574 5f6d   .    mg = get_m
+00001d40: 6728 6564 6174 612c 2063 7572 725f 6361  g(edata, curr_ca
+00001d50: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
+00001d60: 290a 2020 2020 0a20 2020 2062 6561 745f  ).    .    beat_
+00001d70: 7061 7468 735f 7765 6967 6874 7320 3d20  paths_weights = 
+00001d80: 7b63 3a20 7b63 323a 3020 666f 7220 6332  {c: {c2:0 for c2
+00001d90: 2069 6e20 6361 6e64 6964 6174 6573 2069   in candidates i
+00001da0: 6620 6332 2021 3d20 637d 2066 6f72 2063  f c2 != c} for c
+00001db0: 2069 6e20 6361 6e64 6964 6174 6573 7d0a   in candidates}.
+00001dc0: 2020 2020 666f 7220 6320 696e 2063 616e      for c in can
+00001dd0: 6469 6461 7465 733a 200a 2020 2020 2020  didates: .      
+00001de0: 2020 666f 7220 6f74 6865 725f 6320 696e    for other_c in
+00001df0: 2062 6561 745f 7061 7468 735f 7765 6967   beat_paths_weig
+00001e00: 6874 735b 635d 2e6b 6579 7328 293a 0a20  hts[c].keys():. 
+00001e10: 2020 2020 2020 2020 2020 2061 6c6c 5f70             all_p
+00001e20: 6174 6873 203d 2020 6c69 7374 286e 782e  aths =  list(nx.
+00001e30: 616c 6c5f 7369 6d70 6c65 5f70 6174 6873  all_simple_paths
+00001e40: 286d 672c 2063 2c20 6f74 6865 725f 6329  (mg, c, other_c)
+00001e50: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00001e60: 206c 656e 2861 6c6c 5f70 6174 6873 2920   len(all_paths) 
+00001e70: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
+00001e80: 2020 2020 2062 6561 745f 7061 7468 735f       beat_paths_
+00001e90: 7765 6967 6874 735b 635d 5b6f 7468 6572  weights[c][other
+00001ea0: 5f63 5d20 3d20 6d61 7828 5b6d 696e 285b  _c] = max([min([
+00001eb0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00001ec0: 6e28 705b 695d 2c20 705b 692b 315d 2920  n(p[i], p[i+1]) 
+00001ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ee0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00001ef0: 302c 6c65 6e28 7029 2d31 295d 2920 0a20  0,len(p)-1)]) . 
+00001f00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00001f10: 6f72 2070 2069 6e20 616c 6c5f 7061 7468  or p in all_path
+00001f20: 735d 290a 2020 2020 0a20 2020 2077 696e  s]).    .    win
+00001f30: 6e65 7273 203d 206c 6973 7428 290a 2020  ners = list().  
+00001f40: 2020 666f 7220 6320 696e 2063 616e 6469    for c in candi
+00001f50: 6461 7465 733a 200a 2020 2020 2020 2020  dates: .        
+00001f60: 6966 2061 6c6c 285b 6265 6174 5f70 6174  if all([beat_pat
+00001f70: 6873 5f77 6569 6768 7473 5b63 5d5b 6332  hs_weights[c][c2
+00001f80: 5d20 3e3d 2062 6561 745f 7061 7468 735f  ] >= beat_paths_
+00001f90: 7765 6967 6874 735b 6332 5d5b 635d 2066  weights[c2][c] f
+00001fa0: 6f72 2063 3220 696e 2063 616e 6469 6461  or c2 in candida
+00001fb0: 7465 7320 2069 6620 6332 2021 3d20 635d  tes  if c2 != c]
+00001fc0: 293a 0a20 2020 2020 2020 2020 2020 2077  ):.            w
+00001fd0: 696e 6e65 7273 2e61 7070 656e 6428 6329  inners.append(c)
+00001fe0: 0a20 2020 2072 6574 7572 6e20 736f 7274  .    return sort
+00001ff0: 6564 286c 6973 7428 7769 6e6e 6572 7329  ed(list(winners)
+00002000: 290a 0a0a 4076 6d28 6e61 6d65 3d22 4265  )...@vm(name="Be
+00002010: 6174 2050 6174 6822 290a 6465 6620 6265  at Path").def be
+00002020: 6174 5f70 6174 685f 466c 6f79 645f 5761  at_path_Floyd_Wa
+00002030: 7273 6861 6c6c 2865 6461 7461 2c20 6375  rshall(edata, cu
+00002040: 7272 5f63 616e 6473 203d 204e 6f6e 652c  rr_cands = None,
+00002050: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00002060: 6f6e 203d 204e 6f6e 6529 3a20 2020 0a20  on = None):   . 
+00002070: 2020 2022 2222 416e 2069 6d70 6c65 6d65     """An impleme
+00002080: 6e74 6174 696f 6e20 6f66 2042 6561 7420  ntation of Beat 
+00002090: 5061 7468 2075 7369 6e67 2061 2076 6172  Path using a var
+000020a0: 6961 7469 6f6e 206f 6620 7468 6520 466c  iation of the Fl
+000020b0: 6f79 642d 5761 7273 6861 6c6c 2041 6c67  oyd-Warshall Alg
+000020c0: 6f72 6974 686d 0a20 2020 2053 6565 2068  orithm.    See h
+000020d0: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+000020e0: 6469 612e 6f72 672f 7769 6b69 2f53 6368  dia.org/wiki/Sch
+000020f0: 756c 7a65 5f6d 6574 686f 6423 496d 706c  ulze_method#Impl
+00002100: 656d 656e 7461 7469 6f6e 290a 200a 2020  ementation). .  
+00002110: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00002120: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
+00002130: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
+00002140: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
+00002150: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
+00002160: 2074 6861 7420 6861 7320 6120 606d 6172   that has a `mar
+00002170: 6769 6e60 206d 6574 686f 642e 200a 2020  gin` method. .  
+00002180: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
+00002190: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
+000021a0: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
+000021b0: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
+000021c0: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
+000021d0: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
+000021e0: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
+000021f0: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
+00002200: 6473 6060 0a20 2020 2020 2020 2073 7472  ds``.        str
+00002210: 656e 6774 685f 6675 6e63 7469 6f6e 2028  ength_function (
+00002220: 6675 6e63 7469 6f6e 2c20 6f70 7469 6f6e  function, option
+00002230: 616c 293a 2054 6865 2073 7472 656e 6774  al): The strengt
+00002240: 6820 6675 6e63 7469 6f6e 2074 6f20 6265  h function to be
+00002250: 2075 7365 6420 746f 2063 616c 6375 6c61   used to calcula
+00002260: 7465 2074 6865 2073 7472 656e 6774 6820  te the strength 
+00002270: 6f66 2061 2070 6174 682e 2020 2054 6865  of a path.   The
+00002280: 2064 6566 6175 6c74 2069 7320 7468 6520   default is the 
+00002290: 6d61 7267 696e 206d 6574 686f 6420 6f66  margin method of
+000022a0: 2060 6065 6461 7461 6060 2e20 2020 5468   ``edata``.   Th
+000022b0: 6973 206f 6e6c 7920 6d61 7474 6572 7320  is only matters 
+000022c0: 7768 656e 2074 6865 2062 616c 6c6f 7473  when the ballots
+000022d0: 2061 7265 206e 6f74 206c 696e 6561 7220   are not linear 
+000022e0: 6f72 6465 7273 2e20 0a0a 2020 2020 5265  orders. ..    Re
+000022f0: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
+00002300: 4120 736f 7274 6564 206c 6973 7420 6f66  A sorted list of
+00002310: 2063 616e 6469 6461 7465 732e 200a 0a20   candidates. .. 
+00002320: 2020 202e 2e20 7365 6561 6c73 6f3a 3a0a     .. seealso::.
+00002330: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
+00002340: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+00002350: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+00002360: 2e62 6561 745f 7061 7468 602c 203a 6d65  .beat_path`, :me
+00002370: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
+00002380: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+00002390: 686f 6473 2e62 6561 745f 7061 7468 5f64  hods.beat_path_d
+000023a0: 6566 6561 7460 0a0a 0a20 2020 203a 4578  efeat`...    :Ex
+000023b0: 616d 706c 653a 200a 0a20 2020 202e 2e20  ample: ..    .. 
+000023c0: 706c 6f74 3a3a 2020 6d61 7267 696e 5f67  plot::  margin_g
+000023d0: 7261 7068 735f 6578 616d 706c 6573 2f6d  raphs_examples/m
+000023e0: 675f 6578 5f62 705f 7270 2e70 790a 2020  g_ex_bp_rp.py.  
+000023f0: 2020 2020 2020 3a63 6f6e 7465 7874 3a20        :context: 
+00002400: 7265 7365 7420 200a 2020 2020 2020 2020  reset  .        
+00002410: 3a69 6e63 6c75 6465 2d73 6f75 7263 653a  :include-source:
+00002420: 2054 7275 650a 0a0a 2020 2020 2e2e 2063   True...    .. c
+00002430: 6f64 652d 626c 6f63 6b3a 3a20 0a0a 2020  ode-block:: ..  
+00002440: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+00002450: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+00002460: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
+00002470: 7274 2062 6561 745f 7061 7468 5f46 6c6f  rt beat_path_Flo
+00002480: 7964 5f57 6172 7368 616c 6c0a 0a20 2020  yd_Warshall..   
+00002490: 2020 2020 2062 6561 745f 7061 7468 2e64       beat_path.d
+000024a0: 6973 706c 6179 286d 6729 0a20 2020 2020  isplay(mg).     
+000024b0: 2020 2062 6561 745f 7061 7468 5f46 6c6f     beat_path_Flo
+000024c0: 7964 5f57 6172 7368 616c 6c2e 6469 7370  yd_Warshall.disp
+000024d0: 6c61 7928 6d67 290a 0a0a 2020 2020 2e2e  lay(mg)...    ..
+000024e0: 2065 7865 635f 636f 6465 3a3a 200a 2020   exec_code:: .  
+000024f0: 2020 2020 2020 3a68 6964 655f 636f 6465        :hide_code
+00002500: 3a0a 0a20 2020 2020 2020 2066 726f 6d20  :..        from 
+00002510: 7072 6566 5f76 6f74 696e 672e 7765 6967  pref_voting.weig
+00002520: 6874 6564 5f6d 616a 6f72 6974 795f 6772  hted_majority_gr
+00002530: 6170 6873 2069 6d70 6f72 7420 4d61 7267  aphs import Marg
+00002540: 696e 4772 6170 680a 2020 2020 2020 2020  inGraph.        
+00002550: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
+00002560: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+00002570: 7468 6f64 7320 696d 706f 7274 2062 6561  thods import bea
+00002580: 745f 7061 7468 2c20 6265 6174 5f70 6174  t_path, beat_pat
+00002590: 685f 466c 6f79 645f 5761 7273 6861 6c6c  h_Floyd_Warshall
+000025a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000025b0: 2020 6d67 203d 204d 6172 6769 6e47 7261    mg = MarginGra
+000025c0: 7068 285b 302c 2031 2c20 322c 2033 5d2c  ph([0, 1, 2, 3],
+000025d0: 205b 2830 2c20 322c 2033 292c 2028 312c   [(0, 2, 3), (1,
+000025e0: 2030 2c20 3529 2c20 2832 2c20 312c 2035   0, 5), (2, 1, 5
+000025f0: 292c 2028 322c 2033 2c20 3129 2c20 2833  ), (2, 3, 1), (3
+00002600: 2c20 302c 2033 292c 2028 332c 2031 2c20  , 0, 3), (3, 1, 
+00002610: 3129 5d29 0a0a 2020 2020 2020 2020 6265  1)])..        be
+00002620: 6174 5f70 6174 682e 6469 7370 6c61 7928  at_path.display(
+00002630: 6d67 290a 2020 2020 2020 2020 6265 6174  mg).        beat
+00002640: 5f70 6174 685f 466c 6f79 645f 5761 7273  _path_Floyd_Wars
+00002650: 6861 6c6c 2e64 6973 706c 6179 286d 6729  hall.display(mg)
+00002660: 0a0a 2020 2020 2222 220a 0a20 2020 2063  ..    """..    c
+00002670: 616e 6469 6461 7465 7320 3d20 6564 6174  andidates = edat
+00002680: 612e 6361 6e64 6964 6174 6573 2069 6620  a.candidates if 
+00002690: 6375 7272 5f63 616e 6473 2069 7320 4e6f  curr_cands is No
+000026a0: 6e65 2065 6c73 6520 6375 7272 5f63 616e  ne else curr_can
+000026b0: 6473 2020 2020 0a20 2020 2073 7472 656e  ds    .    stren
+000026c0: 6774 685f 6675 6e63 7469 6f6e 203d 2065  gth_function = e
+000026d0: 6461 7461 2e6d 6172 6769 6e20 6966 2073  data.margin if s
+000026e0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+000026f0: 2069 7320 4e6f 6e65 2065 6c73 6520 7374   is None else st
+00002700: 7265 6e67 7468 5f66 756e 6374 696f 6e0a  rength_function.
+00002710: 2020 2020 2020 2020 0a20 2020 2073 5f6d          .    s_m
+00002720: 6174 7269 7820 3d20 5b5b 2d6e 702e 696e  atrix = [[-np.in
+00002730: 6620 666f 7220 5f20 696e 2063 616e 6469  f for _ in candi
+00002740: 6461 7465 735d 2066 6f72 205f 2069 6e20  dates] for _ in 
+00002750: 6361 6e64 6964 6174 6573 5d0a 2020 2020  candidates].    
+00002760: 666f 7220 6331 5f69 6478 2c20 6331 2069  for c1_idx, c1 i
+00002770: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
+00002780: 6964 6174 6573 293a 0a20 2020 2020 2020  idates):.       
+00002790: 2066 6f72 2063 325f 6964 782c 2063 3220   for c2_idx, c2 
+000027a0: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+000027b0: 6469 6461 7465 7329 3a0a 2020 2020 2020  didates):.      
+000027c0: 2020 2020 2020 6966 2028 6564 6174 612e        if (edata.
+000027d0: 6d61 6a6f 7269 7479 5f70 7265 6665 7273  majority_prefers
+000027e0: 2863 312c 2063 3229 206f 7220 6331 203d  (c1, c2) or c1 =
+000027f0: 3d20 6332 293a 0a20 2020 2020 2020 2020  = c2):.         
+00002800: 2020 2020 2020 2073 5f6d 6174 7269 785b         s_matrix[
+00002810: 6331 5f69 6478 5d5b 6332 5f69 6478 5d20  c1_idx][c2_idx] 
+00002820: 3d20 7374 7265 6e67 7468 5f66 756e 6374  = strength_funct
+00002830: 696f 6e28 6331 2c20 6332 2920 0a20 2020  ion(c1, c2) .   
+00002840: 2073 7472 656e 6774 6820 3d20 6c69 7374   strength = list
+00002850: 286d 6170 286c 616d 6264 6120 6920 3a20  (map(lambda i : 
+00002860: 6c69 7374 286d 6170 286c 616d 6264 6120  list(map(lambda 
+00002870: 6a20 3a20 6a20 2c20 6929 2920 2c20 735f  j : j , i)) , s_
+00002880: 6d61 7472 6978 2929 0a20 2020 2066 6f72  matrix)).    for
+00002890: 2069 5f69 6478 2c20 6920 696e 2065 6e75   i_idx, i in enu
+000028a0: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
+000028b0: 7329 3a20 2020 2020 2020 2020 0a20 2020  s):         .   
+000028c0: 2020 2020 2066 6f72 206a 5f69 6478 2c20       for j_idx, 
+000028d0: 6a20 696e 2065 6e75 6d65 7261 7465 2863  j in enumerate(c
+000028e0: 616e 6469 6461 7465 7329 3a20 0a20 2020  andidates): .   
+000028f0: 2020 2020 2020 2020 2069 6620 6921 3d20           if i!= 
+00002900: 6a3a 0a20 2020 2020 2020 2020 2020 2020  j:.             
+00002910: 2020 2066 6f72 206b 5f69 6478 2c20 6b20     for k_idx, k 
+00002920: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+00002930: 6469 6461 7465 7329 3a20 0a20 2020 2020  didates): .     
+00002940: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002950: 6620 6921 3d20 6b20 616e 6420 6a20 213d  f i!= k and j !=
+00002960: 206b 3a0a 2020 2020 2020 2020 2020 2020   k:.            
+00002970: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+00002980: 6e67 7468 5b6a 5f69 6478 5d5b 6b5f 6964  ngth[j_idx][k_id
+00002990: 785d 203d 206d 6178 2873 7472 656e 6774  x] = max(strengt
+000029a0: 685b 6a5f 6964 785d 5b6b 5f69 6478 5d2c  h[j_idx][k_idx],
+000029b0: 206d 696e 2873 7472 656e 6774 685b 6a5f   min(strength[j_
+000029c0: 6964 785d 5b69 5f69 6478 5d2c 7374 7265  idx][i_idx],stre
+000029d0: 6e67 7468 5b69 5f69 6478 5d5b 6b5f 6964  ngth[i_idx][k_id
+000029e0: 785d 2929 0a20 2020 2077 696e 6e65 7273  x])).    winners
+000029f0: 203d 207b 693a 5472 7565 2066 6f72 2069   = {i:True for i
+00002a00: 2069 6e20 6361 6e64 6964 6174 6573 7d0a   in candidates}.
+00002a10: 2020 2020 666f 7220 695f 6964 782c 2069      for i_idx, i
+00002a20: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
+00002a30: 6e64 6964 6174 6573 293a 200a 2020 2020  ndidates): .    
+00002a40: 2020 2020 666f 7220 6a5f 6964 782c 206a      for j_idx, j
+00002a50: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
+00002a60: 6e64 6964 6174 6573 293a 0a20 2020 2020  ndidates):.     
+00002a70: 2020 2020 2020 2069 6620 6921 3d6a 3a0a         if i!=j:.
+00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a90: 6966 2073 7472 656e 6774 685b 6a5f 6964  if strength[j_id
+00002aa0: 785d 5b69 5f69 6478 5d20 3e20 7374 7265  x][i_idx] > stre
+00002ab0: 6e67 7468 5b69 5f69 6478 5d5b 6a5f 6964  ngth[i_idx][j_id
+00002ac0: 785d 3a0a 2020 2020 2020 2020 2020 2020  x]:.            
+00002ad0: 2020 2020 2020 2020 7769 6e6e 6572 735b          winners[
+00002ae0: 695d 203d 2046 616c 7365 0a20 2020 2072  i] = False.    r
+00002af0: 6574 7572 6e20 736f 7274 6564 285b 6320  eturn sorted([c 
+00002b00: 666f 7220 6320 696e 2063 616e 6469 6461  for c in candida
+00002b10: 7465 7320 6966 2077 696e 6e65 7273 5b63  tes if winners[c
+00002b20: 5d5d 290a 0a64 6566 2062 6561 745f 7061  ]])..def beat_pa
+00002b30: 7468 5f64 6566 6561 7428 6564 6174 612c  th_defeat(edata,
+00002b40: 2063 7572 725f 6361 6e64 7320 3d20 4e6f   curr_cands = No
+00002b50: 6e65 2c20 7374 7265 6e67 7468 5f66 756e  ne, strength_fun
+00002b60: 6374 696f 6e20 3d20 4e6f 6e65 293a 2020  ction = None):  
+00002b70: 200a 2020 2020 2222 2252 6574 7572 6e73   .    """Returns
+00002b80: 2074 6865 2064 6566 6561 7420 7265 6c61   the defeat rela
+00002b90: 7469 6f6e 2066 6f72 2042 6561 7420 5061  tion for Beat Pa
+00002ba0: 7468 2e20 0a20 2020 200a 2020 2020 4172  th. .    .    Ar
+00002bb0: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
+00002bc0: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
+00002bd0: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
+00002be0: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
+00002bf0: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
+00002c00: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
+00002c10: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
+00002c20: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
+00002c30: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
+00002c40: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
+00002c50: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
+00002c60: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
+00002c70: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
+00002c80: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
+00002c90: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
+00002ca0: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
+00002cb0: 685f 6675 6e63 7469 6f6e 2028 6675 6e63  h_function (func
+00002cc0: 7469 6f6e 2c20 6f70 7469 6f6e 616c 293a  tion, optional):
+00002cd0: 2054 6865 2073 7472 656e 6774 6820 6675   The strength fu
+00002ce0: 6e63 7469 6f6e 2074 6f20 6265 2075 7365  nction to be use
+00002cf0: 6420 746f 2063 616c 6375 6c61 7465 2074  d to calculate t
+00002d00: 6865 2073 7472 656e 6774 6820 6f66 2061  he strength of a
+00002d10: 2070 6174 682e 2020 2054 6865 2064 6566   path.   The def
+00002d20: 6175 6c74 2069 7320 7468 6520 6d61 7267  ault is the marg
+00002d30: 696e 206d 6574 686f 6420 6f66 2060 6065  in method of ``e
+00002d40: 6461 7461 6060 2e20 2020 5468 6973 206f  data``.   This o
+00002d50: 6e6c 7920 6d61 7474 6572 7320 7768 656e  nly matters when
+00002d60: 2074 6865 2062 616c 6c6f 7473 2061 7265   the ballots are
+00002d70: 206e 6f74 206c 696e 6561 7220 6f72 6465   not linear orde
+00002d80: 7273 2e20 0a0a 2020 2020 5265 7475 726e  rs. ..    Return
+00002d90: 733a 200a 2020 2020 2020 2020 4120 6e65  s: .        A ne
+00002da0: 7477 6f72 6b78 2044 6947 7261 7068 2072  tworkx DiGraph r
+00002db0: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+00002dc0: 4265 6174 2050 6174 6820 6465 6665 6174  Beat Path defeat
+00002dd0: 2072 656c 6174 696f 6e2e 200a 0a20 2020   relation. ..   
+00002de0: 202e 2e20 7365 6561 6c73 6f3a 3a0a 0a20   .. seealso::.. 
+00002df0: 2020 2020 2020 203a 6d65 7468 3a60 7072         :meth:`pr
+00002e00: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+00002e10: 5f62 6173 6564 5f6d 6574 686f 6473 2e62  _based_methods.b
+00002e20: 6561 745f 7061 7468 602c 203a 6d65 7468  eat_path`, :meth
+00002e30: 3a60 7072 6566 5f76 6f74 696e 672e 6d61  :`pref_voting.ma
+00002e40: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+00002e50: 6473 2e62 6561 745f 7061 7468 5f46 6c6f  ds.beat_path_Flo
+00002e60: 7964 5f57 6172 7368 616c 6c60 0a0a 2020  yd_Warshall`..  
+00002e70: 2020 3a45 7861 6d70 6c65 3a20 0a0a 2020    :Example: ..  
+00002e80: 2020 2e2e 2070 6c6f 743a 3a20 206d 6172    .. plot::  mar
+00002e90: 6769 6e5f 6772 6170 6873 5f65 7861 6d70  gin_graphs_examp
+00002ea0: 6c65 732f 6d67 5f65 785f 6270 5f64 6566  les/mg_ex_bp_def
+00002eb0: 6561 742e 7079 0a20 2020 2020 2020 203a  eat.py.        :
+00002ec0: 636f 6e74 6578 743a 2072 6573 6574 2020  context: reset  
+00002ed0: 0a20 2020 2020 2020 203a 696e 636c 7564  .        :includ
+00002ee0: 652d 736f 7572 6365 3a20 5472 7565 0a0a  e-source: True..
+00002ef0: 2020 2020 2222 220a 0a20 2020 2063 616e      """..    can
+00002f00: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
+00002f10: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
+00002f20: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
+00002f30: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
+00002f40: 2020 2020 0a20 2020 2073 7472 656e 6774      .    strengt
+00002f50: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
+00002f60: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
+00002f70: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
+00002f80: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
+00002f90: 6e67 7468 5f66 756e 6374 696f 6e0a 2020  ngth_function.  
+00002fa0: 2020 2020 2020 0a20 2020 2073 5f6d 6174        .    s_mat
+00002fb0: 7269 7820 3d20 5b5b 2d6e 702e 696e 6620  rix = [[-np.inf 
+00002fc0: 666f 7220 5f20 696e 2063 616e 6469 6461  for _ in candida
+00002fd0: 7465 735d 2066 6f72 205f 2069 6e20 6361  tes] for _ in ca
+00002fe0: 6e64 6964 6174 6573 5d0a 2020 2020 666f  ndidates].    fo
+00002ff0: 7220 6331 5f69 6478 2c20 6331 2069 6e20  r c1_idx, c1 in 
+00003000: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
+00003010: 6174 6573 293a 0a20 2020 2020 2020 2066  ates):.        f
+00003020: 6f72 2063 325f 6964 782c 2063 3220 696e  or c2_idx, c2 in
+00003030: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
+00003040: 6461 7465 7329 3a0a 2020 2020 2020 2020  dates):.        
+00003050: 2020 2020 6966 2028 6564 6174 612e 6d61      if (edata.ma
+00003060: 6a6f 7269 7479 5f70 7265 6665 7273 2863  jority_prefers(c
+00003070: 312c 2063 3229 206f 7220 6331 203d 3d20  1, c2) or c1 == 
+00003080: 6332 293a 0a20 2020 2020 2020 2020 2020  c2):.           
+00003090: 2020 2020 2073 5f6d 6174 7269 785b 6331       s_matrix[c1
+000030a0: 5f69 6478 5d5b 6332 5f69 6478 5d20 3d20  _idx][c2_idx] = 
+000030b0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+000030c0: 6e28 6331 2c20 6332 2920 0a20 2020 2073  n(c1, c2) .    s
+000030d0: 7472 656e 6774 6820 3d20 6c69 7374 286d  trength = list(m
+000030e0: 6170 286c 616d 6264 6120 6920 3a20 6c69  ap(lambda i : li
+000030f0: 7374 286d 6170 286c 616d 6264 6120 6a20  st(map(lambda j 
+00003100: 3a20 6a20 2c20 6929 2920 2c20 735f 6d61  : j , i)) , s_ma
+00003110: 7472 6978 2929 0a20 2020 2066 6f72 2069  trix)).    for i
+00003120: 5f69 6478 2c20 6920 696e 2065 6e75 6d65  _idx, i in enume
+00003130: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+00003140: 3a20 2020 2020 2020 2020 0a20 2020 2020  :         .     
+00003150: 2020 2066 6f72 206a 5f69 6478 2c20 6a20     for j_idx, j 
+00003160: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+00003170: 6469 6461 7465 7329 3a20 0a20 2020 2020  didates): .     
+00003180: 2020 2020 2020 2069 6620 6921 3d20 6a3a         if i!= j:
+00003190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000031a0: 2066 6f72 206b 5f69 6478 2c20 6b20 696e   for k_idx, k in
+000031b0: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
+000031c0: 6461 7465 7329 3a20 0a20 2020 2020 2020  dates): .       
+000031d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000031e0: 6921 3d20 6b20 616e 6420 6a20 213d 206b  i!= k and j != k
+000031f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003200: 2020 2020 2020 2020 2020 7374 7265 6e67            streng
+00003210: 7468 5b6a 5f69 6478 5d5b 6b5f 6964 785d  th[j_idx][k_idx]
+00003220: 203d 206d 6178 2873 7472 656e 6774 685b   = max(strength[
+00003230: 6a5f 6964 785d 5b6b 5f69 6478 5d2c 206d  j_idx][k_idx], m
+00003240: 696e 2873 7472 656e 6774 685b 6a5f 6964  in(strength[j_id
+00003250: 785d 5b69 5f69 6478 5d2c 7374 7265 6e67  x][i_idx],streng
+00003260: 7468 5b69 5f69 6478 5d5b 6b5f 6964 785d  th[i_idx][k_idx]
+00003270: 2929 0a0a 2020 2020 6465 6665 6174 5f67  ))..    defeat_g
+00003280: 7261 7068 203d 206e 782e 4469 4772 6170  raph = nx.DiGrap
+00003290: 6828 290a 2020 2020 6465 6665 6174 5f67  h().    defeat_g
+000032a0: 7261 7068 2e61 6464 5f6e 6f64 6573 5f66  raph.add_nodes_f
+000032b0: 726f 6d28 6361 6e64 6964 6174 6573 290a  rom(candidates).
+000032c0: 2020 2020 0a20 2020 2066 6f72 2069 5f69      .    for i_i
+000032d0: 6478 2c20 6920 696e 2065 6e75 6d65 7261  dx, i in enumera
+000032e0: 7465 2863 616e 6469 6461 7465 7329 3a20  te(candidates): 
+000032f0: 0a20 2020 2020 2020 2066 6f72 206a 5f69  .        for j_i
+00003300: 6478 2c20 6a20 696e 2065 6e75 6d65 7261  dx, j in enumera
+00003310: 7465 2863 616e 6469 6461 7465 7329 3a0a  te(candidates):.
+00003320: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00003330: 213d 6a3a 0a20 2020 2020 2020 2020 2020  !=j:.           
+00003340: 2020 2020 2069 6620 7374 7265 6e67 7468       if strength
+00003350: 5b6a 5f69 6478 5d5b 695f 6964 785d 203e  [j_idx][i_idx] >
+00003360: 2073 7472 656e 6774 685b 695f 6964 785d   strength[i_idx]
+00003370: 5b6a 5f69 6478 5d3a 0a20 2020 2020 2020  [j_idx]:.       
+00003380: 2020 2020 2020 2020 2020 2020 2064 6566               def
+00003390: 6561 745f 6772 6170 682e 6164 645f 7765  eat_graph.add_we
+000033a0: 6967 6874 6564 5f65 6467 6573 5f66 726f  ighted_edges_fro
+000033b0: 6d28 5b28 6a2c 692c 735f 6d61 7472 6978  m([(j,i,s_matrix
+000033c0: 5b6a 5f69 6478 5d5b 695f 6964 785d 295d  [j_idx][i_idx])]
+000033d0: 290a 0a20 2020 2072 6574 7572 6e20 6465  )..    return de
+000033e0: 6665 6174 5f67 7261 7068 0a20 2020 200a  feat_graph.    .
+000033f0: 6465 6620 6861 735f 7374 726f 6e67 5f70  def has_strong_p
+00003400: 6174 6828 412c 2073 6f75 7263 652c 2074  ath(A, source, t
+00003410: 6172 6765 742c 206b 293a 0a20 2020 2022  arget, k):.    "
+00003420: 2222 4769 7665 6e20 6120 7371 7561 7265  ""Given a square
+00003430: 206d 6174 7269 7820 412c 2072 6574 7572   matrix A, retur
+00003440: 6e20 5472 7565 2069 6620 7468 6572 6520  n True if there 
+00003450: 6973 2061 2070 6174 6820 6672 6f6d 2073  is a path from s
+00003460: 6f75 7263 6520 746f 2074 6172 6765 7420  ource to target 
+00003470: 696e 2074 6865 2061 7373 6f63 6961 7465  in the associate
+00003480: 6420 6469 7265 6374 6564 2067 7261 7068  d directed graph
+00003490: 2020 2020 2077 6865 7265 2065 6163 6820       where each 
+000034a0: 6564 6765 2068 6173 2061 2077 6569 6768  edge has a weigh
+000034b0: 7420 6772 6561 7465 7220 7468 616e 206f  t greater than o
+000034c0: 7220 6571 7561 6c20 746f 206b 2c20 616e  r equal to k, an
+000034d0: 6420 4661 6c73 6520 6f74 6865 7277 6973  d False otherwis
+000034e0: 652e 2222 220a 2020 2020 0a20 2020 206e  e.""".    .    n
+000034f0: 203d 2041 2e73 6861 7065 5b30 5d20 2320   = A.shape[0] # 
+00003500: 6173 7375 6d65 2041 2069 7320 6120 7371  assume A is a sq
+00003510: 7561 7265 206d 6174 7269 780a 2020 2020  uare matrix.    
+00003520: 7669 7369 7465 6420 3d20 6e70 2e7a 6572  visited = np.zer
+00003530: 6f73 286e 2c20 6474 7970 653d 626f 6f6c  os(n, dtype=bool
+00003540: 290a 0a20 2020 2064 6566 2064 6673 286e  )..    def dfs(n
+00003550: 6f64 6529 3a0a 2020 2020 2020 2020 6966  ode):.        if
+00003560: 206e 6f64 6520 3d3d 2074 6172 6765 743a   node == target:
+00003570: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00003580: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+00003590: 2076 6973 6974 6564 5b6e 6f64 655d 203d   visited[node] =
+000035a0: 2054 7275 650a 2020 2020 2020 2020 666f   True.        fo
+000035b0: 7220 6e65 6967 6862 6f72 2c20 7765 6967  r neighbor, weig
+000035c0: 6874 2069 6e20 656e 756d 6572 6174 6528  ht in enumerate(
+000035d0: 415b 6e6f 6465 2c20 3a5d 293a 0a20 2020  A[node, :]):.   
+000035e0: 2020 2020 2020 2020 2069 6620 415b 6e6f           if A[no
+000035f0: 6465 5d5b 6e65 6967 6862 6f72 5d20 3e20  de][neighbor] > 
+00003600: 415b 6e65 6967 6862 6f72 5d5b 6e6f 6465  A[neighbor][node
+00003610: 5d20 616e 6420 7765 6967 6874 203e 3d20  ] and weight >= 
+00003620: 6b20 616e 6420 6e6f 7420 7669 7369 7465  k and not visite
+00003630: 645b 6e65 6967 6862 6f72 5d3a 0a20 2020  d[neighbor]:.   
+00003640: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00003650: 6466 7328 6e65 6967 6862 6f72 293a 0a20  dfs(neighbor):. 
 00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003670: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-00003680: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00003690: 616c 7365 0a0a 2020 2020 7265 7475 726e  alse..    return
-000036a0: 2064 6673 2873 6f75 7263 6529 0a0a 4076   dfs(source)..@v
-000036b0: 6d28 6e61 6d65 3d22 5370 6c69 7420 4379  m(name="Split Cy
-000036c0: 636c 6522 290a 6465 6620 7370 6c69 745f  cle").def split_
-000036d0: 6379 636c 6528 6564 6174 612c 2063 7572  cycle(edata, cur
-000036e0: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
-000036f0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00003700: 6e20 3d20 4e6f 6e65 293a 0a0a 2020 2020  n = None):..    
-00003710: 2222 2241 202a 2a6d 616a 6f72 6974 7920  """A **majority 
-00003720: 6379 636c 652a 2a20 6973 2061 2073 6571  cycle** is a seq
-00003730: 7565 6e63 6520 3a6d 6174 683a 6078 5f31  uence :math:`x_1
-00003740: 2c20 5c6c 646f 7473 202c 785f 6e60 206f  , \ldots ,x_n` o
-00003750: 6620 6469 7374 696e 6374 2063 616e 6469  f distinct candi
-00003760: 6461 7465 7320 7769 7468 203a 6d61 7468  dates with :math
-00003770: 3a60 785f 313d 785f 6e60 2073 7563 6820  :`x_1=x_n` such 
-00003780: 7468 6174 2066 6f72 203a 6d61 7468 3a60  that for :math:`
-00003790: 3120 5c6c 6571 206b 205c 6c65 7120 6e2d  1 \leq k \leq n-
-000037a0: 3160 2c20 203a 6d61 7468 3a60 785f 6b60  1`,  :math:`x_k`
-000037b0: 2069 7320 6d61 6a6f 7269 7479 2070 7265   is majority pre
-000037c0: 6665 7272 6564 2074 6f20 3a6d 6174 683a  ferred to :math:
-000037d0: 6078 5f7b 6b2b 317d 602e 2020 5468 6520  `x_{k+1}`.  The 
-000037e0: 5370 6c69 7420 4379 636c 6520 7769 6e6e  Split Cycle winn
-000037f0: 6572 7320 6172 6520 6465 7465 726d 696e  ers are determin
-00003800: 6564 2061 7320 666f 6c6c 6f77 733a 2020  ed as follows:  
-00003810: 0a20 2020 200a 2020 2020 4966 2063 616e  .    .    If can
-00003820: 6469 6461 7465 2078 2068 6173 2061 2070  didate x has a p
-00003830: 6f73 6974 6976 6520 6d61 7267 696e 206f  ositive margin o
-00003840: 7665 7220 7920 616e 6420 2878 2c79 2920  ver y and (x,y) 
-00003850: 6973 206e 6f74 2074 6865 2077 6561 6b65  is not the weake
-00003860: 7374 2065 6467 6520 696e 2061 2063 7963  st edge in a cyc
-00003870: 6c65 2c20 7468 656e 2078 2064 6566 6561  le, then x defea
-00003880: 7473 2079 2e20 4571 7569 7661 6c65 6e74  ts y. Equivalent
-00003890: 6c79 2c20 6966 2078 2068 6173 2061 2070  ly, if x has a p
-000038a0: 6f73 6974 6976 6520 6d61 7267 696e 206f  ositive margin o
-000038b0: 7665 7220 7920 616e 6420 7468 6572 6520  ver y and there 
-000038c0: 6973 206e 6f20 7061 7468 2066 726f 6d20  is no path from 
-000038d0: 7920 6261 636b 2074 6f20 7820 6f66 2073  y back to x of s
-000038e0: 7472 656e 6774 6820 6174 206c 6561 7374  trength at least
-000038f0: 2074 6865 206d 6172 6769 6e20 6f66 2078   the margin of x
-00003900: 206f 7665 7220 792c 2074 6865 6e20 7820   over y, then x 
-00003910: 6465 6665 6174 7320 792e 200a 2020 2020  defeats y. .    
-00003920: 0a20 2020 2054 6865 2063 616e 6469 6461  .    The candida
-00003930: 7465 7320 7468 6174 2061 7265 2075 6e64  tes that are und
-00003940: 6566 6561 7465 6420 6172 6520 7468 6520  efeated are the 
-00003950: 5370 6c69 7420 4379 636c 6520 7769 6e6e  Split Cycle winn
-00003960: 6572 732e 0a0a 2020 2020 5365 6520 6874  ers...    See ht
-00003970: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003980: 2f65 7061 6375 6974 2f73 706c 6974 6379  /epacuit/splitcy
-00003990: 636c 6520 616e 6420 7468 6520 7061 7065  cle and the pape
-000039a0: 7220 6874 7470 733a 2f2f 6172 7869 762e  r https://arxiv.
-000039b0: 6f72 672f 6162 732f 3230 3034 2e30 3233  org/abs/2004.023
-000039c0: 3530 2066 6f72 206d 6f72 6520 696e 666f  50 for more info
-000039d0: 726d 6174 696f 6e2e 200a 0a20 2020 2041  rmation. ..    A
-000039e0: 7267 733a 0a20 2020 2020 2020 2065 6461  rgs:.        eda
-000039f0: 7461 2028 5072 6f66 696c 652c 2050 726f  ta (Profile, Pro
-00003a00: 6669 6c65 5769 7468 5469 6573 2c20 4d61  fileWithTies, Ma
-00003a10: 7267 696e 4772 6170 6829 3a20 416e 7920  rginGraph): Any 
-00003a20: 656c 6563 7469 6f6e 2064 6174 6120 7468  election data th
-00003a30: 6174 2068 6173 2061 2060 6d61 7267 696e  at has a `margin
-00003a40: 6020 6d65 7468 6f64 2e20 0a20 2020 2020  ` method. .     
-00003a50: 2020 2063 7572 725f 6361 6e64 7320 284c     curr_cands (L
-00003a60: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
-00003a70: 616c 293a 2049 6620 7365 742c 2074 6865  al): If set, the
-00003a80: 6e20 6669 6e64 2074 6865 2077 696e 6e65  n find the winne
-00003a90: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
-00003aa0: 6c65 2072 6573 7472 6963 7465 6420 746f  le restricted to
-00003ab0: 2074 6865 2063 616e 6469 6461 7465 7320   the candidates 
-00003ac0: 696e 2060 6063 7572 725f 6361 6e64 7360  in ``curr_cands`
-00003ad0: 600a 2020 2020 2020 2020 7374 7265 6e67  `.        streng
-00003ae0: 7468 5f66 756e 6374 696f 6e20 2866 756e  th_function (fun
-00003af0: 6374 696f 6e2c 206f 7074 696f 6e61 6c29  ction, optional)
-00003b00: 3a20 5468 6520 7374 7265 6e67 7468 2066  : The strength f
-00003b10: 756e 6374 696f 6e20 746f 2062 6520 7573  unction to be us
-00003b20: 6564 2074 6f20 6361 6c63 756c 6174 6520  ed to calculate 
-00003b30: 7468 6520 7374 7265 6e67 7468 206f 6620  the strength of 
-00003b40: 6120 7061 7468 2e20 2020 5468 6520 6465  a path.   The de
-00003b50: 6661 756c 7420 6973 2074 6865 206d 6172  fault is the mar
-00003b60: 6769 6e20 6d65 7468 6f64 206f 6620 6060  gin method of ``
-00003b70: 6564 6174 6160 602e 2020 2054 6869 7320  edata``.   This 
-00003b80: 6f6e 6c79 206d 6174 7465 7273 2077 6865  only matters whe
-00003b90: 6e20 7468 6520 6261 6c6c 6f74 7320 6172  n the ballots ar
-00003ba0: 6520 6e6f 7420 6c69 6e65 6172 206f 7264  e not linear ord
-00003bb0: 6572 732e 200a 0a20 2020 2052 6574 7572  ers. ..    Retur
-00003bc0: 6e73 3a20 0a20 2020 2020 2020 2041 2073  ns: .        A s
-00003bd0: 6f72 7465 6420 6c69 7374 206f 6620 6361  orted list of ca
-00003be0: 6e64 6964 6174 6573 2e20 0a0a 2020 2020  ndidates. ..    
-00003bf0: 2e2e 2073 6565 616c 736f 3a3a 0a0a 2020  .. seealso::..  
-00003c00: 2020 2020 2020 3a6d 6574 683a 6070 7265        :meth:`pre
-00003c10: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
-00003c20: 6261 7365 645f 6d65 7468 6f64 732e 7370  based_methods.sp
-00003c30: 6c69 745f 6379 636c 655f 466c 6f79 645f  lit_cycle_Floyd_
-00003c40: 5761 7273 6861 6c6c 602c 203a 6d65 7468  Warshall`, :meth
-00003c50: 3a60 7072 6566 5f76 6f74 696e 672e 6d61  :`pref_voting.ma
-00003c60: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-00003c70: 6473 2e73 706c 6974 5f63 7963 6c65 5f64  ds.split_cycle_d
-00003c80: 6566 6561 7460 0a0a 2020 2020 3a45 7861  efeat`..    :Exa
-00003c90: 6d70 6c65 3a20 0a0a 2020 2020 2e2e 2070  mple: ..    .. p
-00003ca0: 6c6f 743a 3a20 206d 6172 6769 6e5f 6772  lot::  margin_gr
-00003cb0: 6170 6873 5f65 7861 6d70 6c65 732f 6d67  aphs_examples/mg
-00003cc0: 5f65 785f 6270 5f72 702e 7079 0a20 2020  _ex_bp_rp.py.   
-00003cd0: 2020 2020 203a 636f 6e74 6578 743a 2072       :context: r
-00003ce0: 6573 6574 2020 0a20 2020 2020 2020 203a  eset  .        :
-00003cf0: 696e 636c 7564 652d 736f 7572 6365 3a20  include-source: 
-00003d00: 5472 7565 0a0a 0a20 2020 202e 2e20 636f  True...    .. co
-00003d10: 6465 2d62 6c6f 636b 3a3a 200a 0a20 2020  de-block:: ..   
-00003d20: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-00003d30: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-00003d40: 6564 5f6d 6574 686f 6473 2069 6d70 6f72  ed_methods impor
-00003d50: 7420 7370 6c69 745f 6379 636c 650a 0a20  t split_cycle.. 
-00003d60: 2020 2020 2020 2073 706c 6974 5f63 7963         split_cyc
-00003d70: 6c65 2e64 6973 706c 6179 286d 6729 0a0a  le.display(mg)..
-00003d80: 0a20 2020 202e 2e20 6578 6563 5f63 6f64  .    .. exec_cod
-00003d90: 653a 3a20 0a20 2020 2020 2020 203a 6869  e:: .        :hi
-00003da0: 6465 5f63 6f64 653a 0a0a 2020 2020 2020  de_code:..      
-00003db0: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
-00003dc0: 6e67 2e77 6569 6768 7465 645f 6d61 6a6f  ng.weighted_majo
-00003dd0: 7269 7479 5f67 7261 7068 7320 696d 706f  rity_graphs impo
-00003de0: 7274 204d 6172 6769 6e47 7261 7068 0a20  rt MarginGraph. 
-00003df0: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
-00003e00: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
-00003e10: 6173 6564 5f6d 6574 686f 6473 2069 6d70  ased_methods imp
-00003e20: 6f72 7420 7370 6c69 745f 6379 636c 650a  ort split_cycle.
-00003e30: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00003e40: 206d 6720 3d20 4d61 7267 696e 4772 6170   mg = MarginGrap
-00003e50: 6828 5b30 2c20 312c 2032 2c20 335d 2c20  h([0, 1, 2, 3], 
-00003e60: 5b28 302c 2032 2c20 3329 2c20 2831 2c20  [(0, 2, 3), (1, 
-00003e70: 302c 2035 292c 2028 322c 2031 2c20 3529  0, 5), (2, 1, 5)
-00003e80: 2c20 2832 2c20 332c 2031 292c 2028 332c  , (2, 3, 1), (3,
-00003e90: 2030 2c20 3329 2c20 2833 2c20 312c 2031   0, 3), (3, 1, 1
-00003ea0: 295d 290a 2020 2020 2020 2020 0a20 2020  )]).        .   
-00003eb0: 2020 2020 2073 706c 6974 5f63 7963 6c65       split_cycle
-00003ec0: 2e64 6973 706c 6179 286d 6729 0a20 2020  .display(mg).   
-00003ed0: 2022 2222 0a20 2020 200a 2020 2020 7374   """.    .    st
-00003ee0: 7265 6e67 7468 5f6d 6174 7269 782c 2063  rength_matrix, c
-00003ef0: 616e 645f 746f 5f63 696e 6465 7820 3d20  and_to_cindex = 
-00003f00: 6564 6174 612e 7374 7265 6e67 7468 5f6d  edata.strength_m
-00003f10: 6174 7269 7828 6375 7272 5f63 616e 6473  atrix(curr_cands
-00003f20: 203d 2063 7572 725f 6361 6e64 732c 2073   = curr_cands, s
-00003f30: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00003f40: 3d73 7472 656e 6774 685f 6675 6e63 7469  =strength_functi
-00003f50: 6f6e 290a 0a20 2020 2063 616e 6469 6461  on)..    candida
-00003f60: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
-00003f70: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
-00003f80: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
-00003f90: 6520 6375 7272 5f63 616e 6473 2020 0a0a  e curr_cands  ..
-00003fa0: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
-00003fb0: 6374 696f 6e20 3d20 6564 6174 612e 6d61  ction = edata.ma
-00003fc0: 7267 696e 2069 6620 7374 7265 6e67 7468  rgin if strength
-00003fd0: 5f66 756e 6374 696f 6e20 6973 204e 6f6e  _function is Non
-00003fe0: 6520 656c 7365 2073 7472 656e 6774 685f  e else strength_
-00003ff0: 6675 6e63 7469 6f6e 200a 0a20 2020 2070  function ..    p
-00004000: 6f74 656e 7469 616c 5f77 696e 6e65 7273  otential_winners
-00004010: 203d 2073 6574 2863 616e 6469 6461 7465   = set(candidate
-00004020: 7329 0a0a 2020 2020 666f 7220 6120 696e  s)..    for a in
-00004030: 2063 616e 6469 6461 7465 733a 0a20 2020   candidates:.   
-00004040: 2020 2020 2066 6f72 2062 2069 6e20 6361       for b in ca
-00004050: 6e64 6964 6174 6573 3a0a 2020 2020 2020  ndidates:.      
-00004060: 2020 2020 2020 6966 2073 7472 656e 6774        if strengt
-00004070: 685f 6675 6e63 7469 6f6e 2862 2c20 6129  h_function(b, a)
-00004080: 203e 2073 7472 656e 6774 685f 6675 6e63   > strength_func
-00004090: 7469 6f6e 2861 2c20 6229 2061 6e64 206e  tion(a, b) and n
-000040a0: 6f74 2068 6173 5f73 7472 6f6e 675f 7061  ot has_strong_pa
-000040b0: 7468 2873 7472 656e 6774 685f 6d61 7472  th(strength_matr
-000040c0: 6978 2c20 6361 6e64 5f74 6f5f 6369 6e64  ix, cand_to_cind
-000040d0: 6578 2861 292c 2063 616e 645f 746f 5f63  ex(a), cand_to_c
-000040e0: 696e 6465 7828 6229 2c20 7374 7265 6e67  index(b), streng
-000040f0: 7468 5f66 756e 6374 696f 6e28 622c 6129  th_function(b,a)
-00004100: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00004110: 2020 2070 6f74 656e 7469 616c 5f77 696e     potential_win
-00004120: 6e65 7273 2e64 6973 6361 7264 2861 290a  ners.discard(a).
-00004130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004140: 6272 6561 6b0a 0a20 2020 2072 6574 7572  break..    retur
-00004150: 6e20 736f 7274 6564 2870 6f74 656e 7469  n sorted(potenti
-00004160: 616c 5f77 696e 6e65 7273 290a 0a0a 4076  al_winners)...@v
-00004170: 6d28 6e61 6d65 3d22 5370 6c69 7420 4379  m(name="Split Cy
-00004180: 636c 6522 290a 6465 6620 7370 6c69 745f  cle").def split_
-00004190: 6379 636c 655f 466c 6f79 645f 5761 7273  cycle_Floyd_Wars
-000041a0: 6861 6c6c 2865 6461 7461 2c20 6375 7272  hall(edata, curr
-000041b0: 5f63 616e 6473 203d 204e 6f6e 652c 2073  _cands = None, s
-000041c0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-000041d0: 203d 204e 6f6e 6529 3a20 2020 0a20 2020   = None):   .   
-000041e0: 2022 2222 416e 2069 6d70 6c65 6d65 6e74   """An implement
-000041f0: 6174 696f 6e20 6f66 2053 706c 6974 2043  ation of Split C
-00004200: 7963 6c65 2062 6173 6564 206f 6e20 7468  ycle based on th
-00004210: 6520 466c 6f79 642d 5761 7273 6861 6c6c  e Floyd-Warshall
-00004220: 2041 6c67 6f72 6974 686d 2e20 0a0a 2020   Algorithm. ..  
-00004230: 2020 5365 6520 6874 7470 733a 2f2f 6769    See https://gi
-00004240: 7468 7562 2e63 6f6d 2f65 7061 6375 6974  thub.com/epacuit
-00004250: 2f73 706c 6974 6379 636c 6520 616e 6420  /splitcycle and 
-00004260: 7468 6520 7061 7065 7220 6874 7470 733a  the paper https:
-00004270: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
-00004280: 3230 3034 2e30 3233 3530 2066 6f72 206d  2004.02350 for m
-00004290: 6f72 6520 696e 666f 726d 6174 696f 6e2e  ore information.
-000042a0: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
-000042b0: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-000042c0: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-000042d0: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-000042e0: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-000042f0: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-00004300: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
-00004310: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
-00004320: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
-00004330: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
-00004340: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
-00004350: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
-00004360: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
-00004370: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
-00004380: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
-00004390: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
-000043a0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-000043b0: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
-000043c0: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
-000043d0: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
-000043e0: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
-000043f0: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
-00004400: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
-00004410: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
-00004420: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
-00004430: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
-00004440: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
-00004450: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
-00004460: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
-00004470: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
-00004480: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
-00004490: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
-000044a0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
-000044b0: 2e20 0a0a 2020 2020 2e2e 2073 6565 616c  . ..    .. seeal
-000044c0: 736f 3a3a 0a0a 2020 2020 2020 2020 3a6d  so::..        :m
-000044d0: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
-000044e0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-000044f0: 7468 6f64 732e 7370 6c69 745f 6379 636c  thods.split_cycl
-00004500: 6560 2c20 3a6d 6574 683a 6070 7265 665f  e`, :meth:`pref_
-00004510: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-00004520: 7365 645f 6d65 7468 6f64 732e 7370 6c69  sed_methods.spli
-00004530: 745f 6379 636c 655f 6465 6665 6174 600a  t_cycle_defeat`.
-00004540: 0a0a 2020 2020 3a45 7861 6d70 6c65 3a20  ..    :Example: 
-00004550: 0a0a 2020 2020 2e2e 2070 6c6f 743a 3a20  ..    .. plot:: 
-00004560: 206d 6172 6769 6e5f 6772 6170 6873 5f65   margin_graphs_e
-00004570: 7861 6d70 6c65 732f 6d67 5f65 785f 6270  xamples/mg_ex_bp
-00004580: 5f72 702e 7079 0a20 2020 2020 2020 203a  _rp.py.        :
-00004590: 636f 6e74 6578 743a 2072 6573 6574 2020  context: reset  
-000045a0: 0a20 2020 2020 2020 203a 696e 636c 7564  .        :includ
-000045b0: 652d 736f 7572 6365 3a20 5472 7565 0a0a  e-source: True..
-000045c0: 0a20 2020 202e 2e20 636f 6465 2d62 6c6f  .    .. code-blo
-000045d0: 636b 3a3a 200a 0a20 2020 2020 2020 2066  ck:: ..        f
-000045e0: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
-000045f0: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-00004600: 686f 6473 2069 6d70 6f72 7420 7370 6c69  hods import spli
-00004610: 745f 6379 636c 652c 2073 706c 6974 5f63  t_cycle, split_c
-00004620: 7963 6c65 5f46 6c6f 7964 5f57 6172 7368  ycle_Floyd_Warsh
-00004630: 616c 6c0a 0a20 2020 2020 2020 2073 706c  all..        spl
-00004640: 6974 5f63 7963 6c65 2e64 6973 706c 6179  it_cycle.display
-00004650: 286d 6729 0a20 2020 2020 2020 2073 706c  (mg).        spl
-00004660: 6974 5f63 7963 6c65 5f46 6c6f 7964 5f57  it_cycle_Floyd_W
-00004670: 6172 7368 616c 6c2e 6469 7370 6c61 7928  arshall.display(
-00004680: 6d67 290a 0a0a 2020 2020 2e2e 2065 7865  mg)...    .. exe
-00004690: 635f 636f 6465 3a3a 200a 2020 2020 2020  c_code:: .      
-000046a0: 2020 3a68 6964 655f 636f 6465 3a0a 0a20    :hide_code:.. 
-000046b0: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
-000046c0: 5f76 6f74 696e 672e 7765 6967 6874 6564  _voting.weighted
-000046d0: 5f6d 616a 6f72 6974 795f 6772 6170 6873  _majority_graphs
-000046e0: 2069 6d70 6f72 7420 4d61 7267 696e 4772   import MarginGr
-000046f0: 6170 680a 2020 2020 2020 2020 6672 6f6d  aph.        from
-00004700: 2070 7265 665f 766f 7469 6e67 2e6d 6172   pref_voting.mar
-00004710: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
-00004720: 7320 696d 706f 7274 2073 706c 6974 5f63  s import split_c
-00004730: 7963 6c65 2c20 7370 6c69 745f 6379 636c  ycle, split_cycl
-00004740: 655f 466c 6f79 645f 5761 7273 6861 6c6c  e_Floyd_Warshall
-00004750: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00004760: 2020 6d67 203d 204d 6172 6769 6e47 7261    mg = MarginGra
-00004770: 7068 285b 302c 2031 2c20 322c 2033 5d2c  ph([0, 1, 2, 3],
-00004780: 205b 2830 2c20 322c 2033 292c 2028 312c   [(0, 2, 3), (1,
-00004790: 2030 2c20 3529 2c20 2832 2c20 312c 2035   0, 5), (2, 1, 5
-000047a0: 292c 2028 322c 2033 2c20 3129 2c20 2833  ), (2, 3, 1), (3
-000047b0: 2c20 302c 2033 292c 2028 332c 2031 2c20  , 0, 3), (3, 1, 
-000047c0: 3129 5d29 0a20 2020 2020 2020 200a 2020  1)]).        .  
-000047d0: 2020 2020 2020 7370 6c69 745f 6379 636c        split_cycl
-000047e0: 652e 6469 7370 6c61 7928 6d67 290a 2020  e.display(mg).  
-000047f0: 2020 2020 2020 7370 6c69 745f 6379 636c        split_cycl
-00004800: 655f 466c 6f79 645f 5761 7273 6861 6c6c  e_Floyd_Warshall
-00004810: 2e64 6973 706c 6179 286d 6729 0a0a 0a20  .display(mg)... 
-00004820: 2020 2022 2222 0a0a 2020 2020 6361 6e64     """..    cand
-00004830: 6964 6174 6573 203d 2065 6461 7461 2e63  idates = edata.c
-00004840: 616e 6469 6461 7465 7320 6966 2063 7572  andidates if cur
-00004850: 725f 6361 6e64 7320 6973 204e 6f6e 6520  r_cands is None 
-00004860: 656c 7365 2063 7572 725f 6361 6e64 7320  else curr_cands 
-00004870: 2020 200a 2020 2020 7374 7265 6e67 7468     .    strength
-00004880: 5f66 756e 6374 696f 6e20 3d20 6564 6174  _function = edat
-00004890: 612e 6d61 7267 696e 2069 6620 7374 7265  a.margin if stre
-000048a0: 6e67 7468 5f66 756e 6374 696f 6e20 6973  ngth_function is
-000048b0: 204e 6f6e 6520 656c 7365 2073 7472 656e   None else stren
-000048c0: 6774 685f 6675 6e63 7469 6f6e 200a 200a  gth_function . .
-000048d0: 2020 2020 7765 616b 5f63 6f6e 646f 7263      weak_condorc
-000048e0: 6574 5f77 696e 6e65 7273 203d 207b 633a  et_winners = {c:
-000048f0: 5472 7565 2066 6f72 2063 2069 6e20 6361  True for c in ca
-00004900: 6e64 6964 6174 6573 7d0a 2020 2020 735f  ndidates}.    s_
-00004910: 6d61 7472 6978 203d 205b 5b2d 6e70 2e69  matrix = [[-np.i
-00004920: 6e66 2066 6f72 205f 2069 6e20 6361 6e64  nf for _ in cand
-00004930: 6964 6174 6573 5d20 666f 7220 5f20 696e  idates] for _ in
-00004940: 2063 616e 6469 6461 7465 735d 0a20 2020   candidates].   
-00004950: 200a 2020 2020 2320 696e 6974 6961 6c69   .    # initiali
-00004960: 7a65 2074 6865 2073 5f6d 6174 7269 780a  ze the s_matrix.
-00004970: 2020 2020 666f 7220 6331 5f69 6478 2c20      for c1_idx, 
-00004980: 6331 2069 6e20 656e 756d 6572 6174 6528  c1 in enumerate(
-00004990: 6361 6e64 6964 6174 6573 293a 0a20 2020  candidates):.   
-000049a0: 2020 2020 2066 6f72 2063 325f 6964 782c       for c2_idx,
-000049b0: 2063 3220 696e 2065 6e75 6d65 7261 7465   c2 in enumerate
-000049c0: 2863 616e 6469 6461 7465 7329 3a0a 2020  (candidates):.  
-000049d0: 2020 2020 2020 2020 2020 6966 2028 6564            if (ed
-000049e0: 6174 612e 6d61 6a6f 7269 7479 5f70 7265  ata.majority_pre
-000049f0: 6665 7273 2863 312c 2063 3229 206f 7220  fers(c1, c2) or 
-00004a00: 6331 203d 3d20 6332 293a 0a20 2020 2020  c1 == c2):.     
-00004a10: 2020 2020 2020 2020 2020 2073 5f6d 6174             s_mat
-00004a20: 7269 785b 6331 5f69 6478 5d5b 6332 5f69  rix[c1_idx][c2_i
-00004a30: 6478 5d20 3d20 7374 7265 6e67 7468 5f66  dx] = strength_f
-00004a40: 756e 6374 696f 6e28 6331 2c20 6332 2920  unction(c1, c2) 
-00004a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004a60: 2077 6561 6b5f 636f 6e64 6f72 6365 745f   weak_condorcet_
-00004a70: 7769 6e6e 6572 735b 6332 5d20 3d20 7765  winners[c2] = we
-00004a80: 616b 5f63 6f6e 646f 7263 6574 5f77 696e  ak_condorcet_win
-00004a90: 6e65 7273 5b63 325d 2061 6e64 2028 6331  ners[c2] and (c1
-00004aa0: 203d 3d20 6332 2920 2320 5765 616b 2043   == c2) # Weak C
-00004ab0: 6f6e 646f 7263 6574 2077 696e 6e65 7273  ondorcet winners
-00004ac0: 2061 7265 2053 706c 6974 2043 7963 6c65   are Split Cycle
-00004ad0: 2077 696e 6e65 7273 0a20 2020 200a 2020   winners.    .  
-00004ae0: 2020 7374 7265 6e67 7468 203d 206c 6973    strength = lis
-00004af0: 7428 6d61 7028 6c61 6d62 6461 2069 203a  t(map(lambda i :
-00004b00: 206c 6973 7428 6d61 7028 6c61 6d62 6461   list(map(lambda
-00004b10: 206a 203a 206a 202c 2069 2929 202c 2073   j : j , i)) , s
-00004b20: 5f6d 6174 7269 7829 290a 2020 2020 666f  _matrix)).    fo
-00004b30: 7220 695f 6964 782c 2069 2069 6e20 656e  r i_idx, i in en
-00004b40: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
-00004b50: 6573 293a 200a 2020 2020 2020 2020 666f  es): .        fo
-00004b60: 7220 6a5f 6964 782c 206a 2069 6e20 656e  r j_idx, j in en
-00004b70: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
-00004b80: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
-00004b90: 2069 6620 6921 3d20 6a3a 0a20 2020 2020   if i!= j:.     
-00004ba0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00004bb0: 7420 7765 616b 5f63 6f6e 646f 7263 6574  t weak_condorcet
-00004bc0: 5f77 696e 6e65 7273 5b6a 5d3a 2023 2077  _winners[j]: # w
-00004bd0: 6561 6b20 436f 6e64 6f72 6365 7420 7769  eak Condorcet wi
-00004be0: 6e6e 6572 7320 6172 6520 5370 6c69 7420  nners are Split 
-00004bf0: 4379 636c 6520 7769 6e6e 6572 730a 2020  Cycle winners.  
+00003670: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
+00003680: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00003690: 6c73 650a 0a20 2020 2072 6574 7572 6e20  lse..    return 
+000036a0: 6466 7328 736f 7572 6365 290a 0a40 766d  dfs(source)..@vm
+000036b0: 286e 616d 653d 2253 706c 6974 2043 7963  (name="Split Cyc
+000036c0: 6c65 2229 0a64 6566 2073 706c 6974 5f63  le").def split_c
+000036d0: 7963 6c65 2865 6461 7461 2c20 6375 7272  ycle(edata, curr
+000036e0: 5f63 616e 6473 203d 204e 6f6e 652c 2073  _cands = None, s
+000036f0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00003700: 203d 204e 6f6e 6529 3a0a 0a20 2020 2022   = None):..    "
+00003710: 2222 4120 2a2a 6d61 6a6f 7269 7479 2063  ""A **majority c
+00003720: 7963 6c65 2a2a 2069 7320 6120 7365 7175  ycle** is a sequ
+00003730: 656e 6365 203a 6d61 7468 3a60 785f 312c  ence :math:`x_1,
+00003740: 205c 6c64 6f74 7320 2c78 5f6e 6020 6f66   \ldots ,x_n` of
+00003750: 2064 6973 7469 6e63 7420 6361 6e64 6964   distinct candid
+00003760: 6174 6573 2077 6974 6820 3a6d 6174 683a  ates with :math:
+00003770: 6078 5f31 3d78 5f6e 6020 7375 6368 2074  `x_1=x_n` such t
+00003780: 6861 7420 666f 7220 3a6d 6174 683a 6031  hat for :math:`1
+00003790: 205c 6c65 7120 6b20 5c6c 6571 206e 2d31   \leq k \leq n-1
+000037a0: 602c 2020 3a6d 6174 683a 6078 5f6b 6020  `,  :math:`x_k` 
+000037b0: 6973 206d 616a 6f72 6974 7920 7072 6566  is majority pref
+000037c0: 6572 7265 6420 746f 203a 6d61 7468 3a60  erred to :math:`
+000037d0: 785f 7b6b 2b31 7d60 2e20 2054 6865 2053  x_{k+1}`.  The S
+000037e0: 706c 6974 2043 7963 6c65 2077 696e 6e65  plit Cycle winne
+000037f0: 7273 2061 7265 2064 6574 6572 6d69 6e65  rs are determine
+00003800: 6420 6173 2066 6f6c 6c6f 7773 3a20 200a  d as follows:  .
+00003810: 2020 2020 0a20 2020 2049 6620 6361 6e64      .    If cand
+00003820: 6964 6174 6520 7820 6861 7320 6120 706f  idate x has a po
+00003830: 7369 7469 7665 206d 6172 6769 6e20 6f76  sitive margin ov
+00003840: 6572 2079 2061 6e64 2028 782c 7929 2069  er y and (x,y) i
+00003850: 7320 6e6f 7420 7468 6520 7765 616b 6573  s not the weakes
+00003860: 7420 6564 6765 2069 6e20 6120 6379 636c  t edge in a cycl
+00003870: 652c 2074 6865 6e20 7820 6465 6665 6174  e, then x defeat
+00003880: 7320 792e 2045 7175 6976 616c 656e 746c  s y. Equivalentl
+00003890: 792c 2069 6620 7820 6861 7320 6120 706f  y, if x has a po
+000038a0: 7369 7469 7665 206d 6172 6769 6e20 6f76  sitive margin ov
+000038b0: 6572 2079 2061 6e64 2074 6865 7265 2069  er y and there i
+000038c0: 7320 6e6f 2070 6174 6820 6672 6f6d 2079  s no path from y
+000038d0: 2062 6163 6b20 746f 2078 206f 6620 7374   back to x of st
+000038e0: 7265 6e67 7468 2061 7420 6c65 6173 7420  rength at least 
+000038f0: 7468 6520 6d61 7267 696e 206f 6620 7820  the margin of x 
+00003900: 6f76 6572 2079 2c20 7468 656e 2078 2064  over y, then x d
+00003910: 6566 6561 7473 2079 2e20 0a20 2020 200a  efeats y. .    .
+00003920: 2020 2020 5468 6520 6361 6e64 6964 6174      The candidat
+00003930: 6573 2074 6861 7420 6172 6520 756e 6465  es that are unde
+00003940: 6665 6174 6564 2061 7265 2074 6865 2053  feated are the S
+00003950: 706c 6974 2043 7963 6c65 2077 696e 6e65  plit Cycle winne
+00003960: 7273 2e0a 0a20 2020 2053 6565 2068 7474  rs...    See htt
+00003970: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00003980: 6570 6163 7569 742f 7370 6c69 7463 7963  epacuit/splitcyc
+00003990: 6c65 2061 6e64 2074 6865 2070 6170 6572  le and the paper
+000039a0: 2068 7474 7073 3a2f 2f61 7278 6976 2e6f   https://arxiv.o
+000039b0: 7267 2f61 6273 2f32 3030 342e 3032 3335  rg/abs/2004.0235
+000039c0: 3020 666f 7220 6d6f 7265 2069 6e66 6f72  0 for more infor
+000039d0: 6d61 7469 6f6e 2e20 0a0a 2020 2020 4172  mation. ..    Ar
+000039e0: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
+000039f0: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
+00003a00: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
+00003a10: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
+00003a20: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
+00003a30: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
+00003a40: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
+00003a50: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
+00003a60: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
+00003a70: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
+00003a80: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
+00003a90: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
+00003aa0: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
+00003ab0: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
+00003ac0: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
+00003ad0: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
+00003ae0: 685f 6675 6e63 7469 6f6e 2028 6675 6e63  h_function (func
+00003af0: 7469 6f6e 2c20 6f70 7469 6f6e 616c 293a  tion, optional):
+00003b00: 2054 6865 2073 7472 656e 6774 6820 6675   The strength fu
+00003b10: 6e63 7469 6f6e 2074 6f20 6265 2075 7365  nction to be use
+00003b20: 6420 746f 2063 616c 6375 6c61 7465 2074  d to calculate t
+00003b30: 6865 2073 7472 656e 6774 6820 6f66 2061  he strength of a
+00003b40: 2070 6174 682e 2020 2054 6865 2064 6566   path.   The def
+00003b50: 6175 6c74 2069 7320 7468 6520 6d61 7267  ault is the marg
+00003b60: 696e 206d 6574 686f 6420 6f66 2060 6065  in method of ``e
+00003b70: 6461 7461 6060 2e20 2020 5468 6973 206f  data``.   This o
+00003b80: 6e6c 7920 6d61 7474 6572 7320 7768 656e  nly matters when
+00003b90: 2074 6865 2062 616c 6c6f 7473 2061 7265   the ballots are
+00003ba0: 206e 6f74 206c 696e 6561 7220 6f72 6465   not linear orde
+00003bb0: 7273 2e20 0a0a 2020 2020 5265 7475 726e  rs. ..    Return
+00003bc0: 733a 200a 2020 2020 2020 2020 4120 736f  s: .        A so
+00003bd0: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
+00003be0: 6469 6461 7465 732e 200a 0a20 2020 202e  didates. ..    .
+00003bf0: 2e20 7365 6561 6c73 6f3a 3a0a 0a20 2020  . seealso::..   
+00003c00: 2020 2020 203a 6d65 7468 3a60 7072 6566       :meth:`pref
+00003c10: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+00003c20: 6173 6564 5f6d 6574 686f 6473 2e73 706c  ased_methods.spl
+00003c30: 6974 5f63 7963 6c65 5f46 6c6f 7964 5f57  it_cycle_Floyd_W
+00003c40: 6172 7368 616c 6c60 2c20 3a6d 6574 683a  arshall`, :meth:
+00003c50: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
+00003c60: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+00003c70: 732e 7370 6c69 745f 6379 636c 655f 6465  s.split_cycle_de
+00003c80: 6665 6174 600a 0a20 2020 203a 4578 616d  feat`..    :Exam
+00003c90: 706c 653a 200a 0a20 2020 202e 2e20 706c  ple: ..    .. pl
+00003ca0: 6f74 3a3a 2020 6d61 7267 696e 5f67 7261  ot::  margin_gra
+00003cb0: 7068 735f 6578 616d 706c 6573 2f6d 675f  phs_examples/mg_
+00003cc0: 6578 5f62 705f 7270 2e70 790a 2020 2020  ex_bp_rp.py.    
+00003cd0: 2020 2020 3a63 6f6e 7465 7874 3a20 7265      :context: re
+00003ce0: 7365 7420 200a 2020 2020 2020 2020 3a69  set  .        :i
+00003cf0: 6e63 6c75 6465 2d73 6f75 7263 653a 2054  nclude-source: T
+00003d00: 7275 650a 0a0a 2020 2020 2e2e 2063 6f64  rue...    .. cod
+00003d10: 652d 626c 6f63 6b3a 3a20 0a0a 2020 2020  e-block:: ..    
+00003d20: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
+00003d30: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+00003d40: 645f 6d65 7468 6f64 7320 696d 706f 7274  d_methods import
+00003d50: 2073 706c 6974 5f63 7963 6c65 0a0a 2020   split_cycle..  
+00003d60: 2020 2020 2020 7370 6c69 745f 6379 636c        split_cycl
+00003d70: 652e 6469 7370 6c61 7928 6d67 290a 0a0a  e.display(mg)...
+00003d80: 2020 2020 2e2e 2065 7865 635f 636f 6465      .. exec_code
+00003d90: 3a3a 200a 2020 2020 2020 2020 3a68 6964  :: .        :hid
+00003da0: 655f 636f 6465 3a0a 0a20 2020 2020 2020  e_code:..       
+00003db0: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
+00003dc0: 672e 7765 6967 6874 6564 5f6d 616a 6f72  g.weighted_major
+00003dd0: 6974 795f 6772 6170 6873 2069 6d70 6f72  ity_graphs impor
+00003de0: 7420 4d61 7267 696e 4772 6170 680a 2020  t MarginGraph.  
+00003df0: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+00003e00: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+00003e10: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
+00003e20: 7274 2073 706c 6974 5f63 7963 6c65 0a20  rt split_cycle. 
+00003e30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003e40: 6d67 203d 204d 6172 6769 6e47 7261 7068  mg = MarginGraph
+00003e50: 285b 302c 2031 2c20 322c 2033 5d2c 205b  ([0, 1, 2, 3], [
+00003e60: 2830 2c20 322c 2033 292c 2028 312c 2030  (0, 2, 3), (1, 0
+00003e70: 2c20 3529 2c20 2832 2c20 312c 2035 292c  , 5), (2, 1, 5),
+00003e80: 2028 322c 2033 2c20 3129 2c20 2833 2c20   (2, 3, 1), (3, 
+00003e90: 302c 2033 292c 2028 332c 2031 2c20 3129  0, 3), (3, 1, 1)
+00003ea0: 5d29 0a20 2020 2020 2020 200a 2020 2020  ]).        .    
+00003eb0: 2020 2020 7370 6c69 745f 6379 636c 652e      split_cycle.
+00003ec0: 6469 7370 6c61 7928 6d67 290a 2020 2020  display(mg).    
+00003ed0: 2222 220a 2020 2020 0a20 2020 2073 7472  """.    .    str
+00003ee0: 656e 6774 685f 6d61 7472 6978 2c20 6361  ength_matrix, ca
+00003ef0: 6e64 5f74 6f5f 6369 6e64 6578 203d 2065  nd_to_cindex = e
+00003f00: 6461 7461 2e73 7472 656e 6774 685f 6d61  data.strength_ma
+00003f10: 7472 6978 2863 7572 725f 6361 6e64 7320  trix(curr_cands 
+00003f20: 3d20 6375 7272 5f63 616e 6473 2c20 7374  = curr_cands, st
+00003f30: 7265 6e67 7468 5f66 756e 6374 696f 6e3d  rength_function=
+00003f40: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00003f50: 6e29 0a0a 2020 2020 6361 6e64 6964 6174  n)..    candidat
+00003f60: 6573 203d 2065 6461 7461 2e63 616e 6469  es = edata.candi
+00003f70: 6461 7465 7320 6966 2063 7572 725f 6361  dates if curr_ca
+00003f80: 6e64 7320 6973 204e 6f6e 6520 656c 7365  nds is None else
+00003f90: 2063 7572 725f 6361 6e64 7320 200a 0a20   curr_cands  .. 
+00003fa0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+00003fb0: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
+00003fc0: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
+00003fd0: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
+00003fe0: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
+00003ff0: 756e 6374 696f 6e20 0a0a 2020 2020 706f  unction ..    po
+00004000: 7465 6e74 6961 6c5f 7769 6e6e 6572 7320  tential_winners 
+00004010: 3d20 7365 7428 6361 6e64 6964 6174 6573  = set(candidates
+00004020: 290a 0a20 2020 2066 6f72 2061 2069 6e20  )..    for a in 
+00004030: 6361 6e64 6964 6174 6573 3a0a 2020 2020  candidates:.    
+00004040: 2020 2020 666f 7220 6220 696e 2063 616e      for b in can
+00004050: 6469 6461 7465 733a 0a20 2020 2020 2020  didates:.       
+00004060: 2020 2020 2069 6620 7374 7265 6e67 7468       if strength
+00004070: 5f66 756e 6374 696f 6e28 622c 2061 2920  _function(b, a) 
+00004080: 3e20 7374 7265 6e67 7468 5f66 756e 6374  > strength_funct
+00004090: 696f 6e28 612c 2062 2920 616e 6420 6e6f  ion(a, b) and no
+000040a0: 7420 6861 735f 7374 726f 6e67 5f70 6174  t has_strong_pat
+000040b0: 6828 7374 7265 6e67 7468 5f6d 6174 7269  h(strength_matri
+000040c0: 782c 2063 616e 645f 746f 5f63 696e 6465  x, cand_to_cinde
+000040d0: 7828 6129 2c20 6361 6e64 5f74 6f5f 6369  x(a), cand_to_ci
+000040e0: 6e64 6578 2862 292c 2073 7472 656e 6774  ndex(b), strengt
+000040f0: 685f 6675 6e63 7469 6f6e 2862 2c61 2929  h_function(b,a))
+00004100: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004110: 2020 706f 7465 6e74 6961 6c5f 7769 6e6e    potential_winn
+00004120: 6572 732e 6469 7363 6172 6428 6129 0a20  ers.discard(a). 
+00004130: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00004140: 7265 616b 0a0a 2020 2020 7265 7475 726e  reak..    return
+00004150: 2073 6f72 7465 6428 706f 7465 6e74 6961   sorted(potentia
+00004160: 6c5f 7769 6e6e 6572 7329 0a0a 0a40 766d  l_winners)...@vm
+00004170: 286e 616d 653d 2253 706c 6974 2043 7963  (name="Split Cyc
+00004180: 6c65 2229 0a64 6566 2073 706c 6974 5f63  le").def split_c
+00004190: 7963 6c65 5f46 6c6f 7964 5f57 6172 7368  ycle_Floyd_Warsh
+000041a0: 616c 6c28 6564 6174 612c 2063 7572 725f  all(edata, curr_
+000041b0: 6361 6e64 7320 3d20 4e6f 6e65 2c20 7374  cands = None, st
+000041c0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+000041d0: 3d20 4e6f 6e65 293a 2020 200a 2020 2020  = None):   .    
+000041e0: 2222 2241 6e20 696d 706c 656d 656e 7461  """An implementa
+000041f0: 7469 6f6e 206f 6620 5370 6c69 7420 4379  tion of Split Cy
+00004200: 636c 6520 6261 7365 6420 6f6e 2074 6865  cle based on the
+00004210: 2046 6c6f 7964 2d57 6172 7368 616c 6c20   Floyd-Warshall 
+00004220: 416c 676f 7269 7468 6d2e 200a 0a20 2020  Algorithm. ..   
+00004230: 2053 6565 2068 7474 7073 3a2f 2f67 6974   See https://git
+00004240: 6875 622e 636f 6d2f 6570 6163 7569 742f  hub.com/epacuit/
+00004250: 7370 6c69 7463 7963 6c65 2061 6e64 2074  splitcycle and t
+00004260: 6865 2070 6170 6572 2068 7474 7073 3a2f  he paper https:/
+00004270: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00004280: 3030 342e 3032 3335 3020 666f 7220 6d6f  004.02350 for mo
+00004290: 7265 2069 6e66 6f72 6d61 7469 6f6e 2e20  re information. 
+000042a0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+000042b0: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
+000042c0: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
+000042d0: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
+000042e0: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
+000042f0: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
+00004300: 606d 6172 6769 6e60 206d 6574 686f 642e  `margin` method.
+00004310: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
+00004320: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
+00004330: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
+00004340: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
+00004350: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
+00004360: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
+00004370: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
+00004380: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
+00004390: 5f63 616e 6473 6060 0a20 2020 2020 2020  _cands``.       
+000043a0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+000043b0: 6f6e 2028 6675 6e63 7469 6f6e 2c20 6f70  on (function, op
+000043c0: 7469 6f6e 616c 293a 2054 6865 2073 7472  tional): The str
+000043d0: 656e 6774 6820 6675 6e63 7469 6f6e 2074  ength function t
+000043e0: 6f20 6265 2075 7365 6420 746f 2063 616c  o be used to cal
+000043f0: 6375 6c61 7465 2074 6865 2073 7472 656e  culate the stren
+00004400: 6774 6820 6f66 2061 2070 6174 682e 2020  gth of a path.  
+00004410: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
+00004420: 7468 6520 6d61 7267 696e 206d 6574 686f  the margin metho
+00004430: 6420 6f66 2060 6065 6461 7461 6060 2e20  d of ``edata``. 
+00004440: 2020 5468 6973 206f 6e6c 7920 6d61 7474    This only matt
+00004450: 6572 7320 7768 656e 2074 6865 2062 616c  ers when the bal
+00004460: 6c6f 7473 2061 7265 206e 6f74 206c 696e  lots are not lin
+00004470: 6561 7220 6f72 6465 7273 2e20 0a0a 2020  ear orders. ..  
+00004480: 2020 5265 7475 726e 733a 200a 2020 2020    Returns: .    
+00004490: 2020 2020 4120 736f 7274 6564 206c 6973      A sorted lis
+000044a0: 7420 6f66 2063 616e 6469 6461 7465 732e  t of candidates.
+000044b0: 200a 0a20 2020 202e 2e20 7365 6561 6c73   ..    .. seeals
+000044c0: 6f3a 3a0a 0a20 2020 2020 2020 203a 6d65  o::..        :me
+000044d0: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
+000044e0: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+000044f0: 686f 6473 2e73 706c 6974 5f63 7963 6c65  hods.split_cycle
+00004500: 602c 203a 6d65 7468 3a60 7072 6566 5f76  `, :meth:`pref_v
+00004510: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
+00004520: 6564 5f6d 6574 686f 6473 2e73 706c 6974  ed_methods.split
+00004530: 5f63 7963 6c65 5f64 6566 6561 7460 0a0a  _cycle_defeat`..
+00004540: 0a20 2020 203a 4578 616d 706c 653a 200a  .    :Example: .
+00004550: 0a20 2020 202e 2e20 706c 6f74 3a3a 2020  .    .. plot::  
+00004560: 6d61 7267 696e 5f67 7261 7068 735f 6578  margin_graphs_ex
+00004570: 616d 706c 6573 2f6d 675f 6578 5f62 705f  amples/mg_ex_bp_
+00004580: 7270 2e70 790a 2020 2020 2020 2020 3a63  rp.py.        :c
+00004590: 6f6e 7465 7874 3a20 7265 7365 7420 200a  ontext: reset  .
+000045a0: 2020 2020 2020 2020 3a69 6e63 6c75 6465          :include
+000045b0: 2d73 6f75 7263 653a 2054 7275 650a 0a0a  -source: True...
+000045c0: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
+000045d0: 6b3a 3a20 0a0a 2020 2020 2020 2020 6672  k:: ..        fr
+000045e0: 6f6d 2070 7265 665f 766f 7469 6e67 2e6d  om pref_voting.m
+000045f0: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+00004600: 6f64 7320 696d 706f 7274 2073 706c 6974  ods import split
+00004610: 5f63 7963 6c65 2c20 7370 6c69 745f 6379  _cycle, split_cy
+00004620: 636c 655f 466c 6f79 645f 5761 7273 6861  cle_Floyd_Warsha
+00004630: 6c6c 0a0a 2020 2020 2020 2020 7370 6c69  ll..        spli
+00004640: 745f 6379 636c 652e 6469 7370 6c61 7928  t_cycle.display(
+00004650: 6d67 290a 2020 2020 2020 2020 7370 6c69  mg).        spli
+00004660: 745f 6379 636c 655f 466c 6f79 645f 5761  t_cycle_Floyd_Wa
+00004670: 7273 6861 6c6c 2e64 6973 706c 6179 286d  rshall.display(m
+00004680: 6729 0a0a 0a20 2020 202e 2e20 6578 6563  g)...    .. exec
+00004690: 5f63 6f64 653a 3a20 0a20 2020 2020 2020  _code:: .       
+000046a0: 203a 6869 6465 5f63 6f64 653a 0a0a 2020   :hide_code:..  
+000046b0: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+000046c0: 766f 7469 6e67 2e77 6569 6768 7465 645f  voting.weighted_
+000046d0: 6d61 6a6f 7269 7479 5f67 7261 7068 7320  majority_graphs 
+000046e0: 696d 706f 7274 204d 6172 6769 6e47 7261  import MarginGra
+000046f0: 7068 0a20 2020 2020 2020 2066 726f 6d20  ph.        from 
+00004700: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+00004710: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+00004720: 2069 6d70 6f72 7420 7370 6c69 745f 6379   import split_cy
+00004730: 636c 652c 2073 706c 6974 5f63 7963 6c65  cle, split_cycle
+00004740: 5f46 6c6f 7964 5f57 6172 7368 616c 6c0a  _Floyd_Warshall.
+00004750: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004760: 206d 6720 3d20 4d61 7267 696e 4772 6170   mg = MarginGrap
+00004770: 6828 5b30 2c20 312c 2032 2c20 335d 2c20  h([0, 1, 2, 3], 
+00004780: 5b28 302c 2032 2c20 3329 2c20 2831 2c20  [(0, 2, 3), (1, 
+00004790: 302c 2035 292c 2028 322c 2031 2c20 3529  0, 5), (2, 1, 5)
+000047a0: 2c20 2832 2c20 332c 2031 292c 2028 332c  , (2, 3, 1), (3,
+000047b0: 2030 2c20 3329 2c20 2833 2c20 312c 2031   0, 3), (3, 1, 1
+000047c0: 295d 290a 2020 2020 2020 2020 0a20 2020  )]).        .   
+000047d0: 2020 2020 2073 706c 6974 5f63 7963 6c65       split_cycle
+000047e0: 2e64 6973 706c 6179 286d 6729 0a20 2020  .display(mg).   
+000047f0: 2020 2020 2073 706c 6974 5f63 7963 6c65       split_cycle
+00004800: 5f46 6c6f 7964 5f57 6172 7368 616c 6c2e  _Floyd_Warshall.
+00004810: 6469 7370 6c61 7928 6d67 290a 0a0a 2020  display(mg)...  
+00004820: 2020 2222 220a 0a20 2020 2063 616e 6469    """..    candi
+00004830: 6461 7465 7320 3d20 6564 6174 612e 6361  dates = edata.ca
+00004840: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
+00004850: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
+00004860: 6c73 6520 6375 7272 5f63 616e 6473 2020  lse curr_cands  
+00004870: 2020 0a20 2020 2073 7472 656e 6774 685f    .    strength_
+00004880: 6675 6e63 7469 6f6e 203d 2065 6461 7461  function = edata
+00004890: 2e6d 6172 6769 6e20 6966 2073 7472 656e  .margin if stren
+000048a0: 6774 685f 6675 6e63 7469 6f6e 2069 7320  gth_function is 
+000048b0: 4e6f 6e65 2065 6c73 6520 7374 7265 6e67  None else streng
+000048c0: 7468 5f66 756e 6374 696f 6e20 0a20 0a20  th_function . . 
+000048d0: 2020 2077 6561 6b5f 636f 6e64 6f72 6365     weak_condorce
+000048e0: 745f 7769 6e6e 6572 7320 3d20 7b63 3a54  t_winners = {c:T
+000048f0: 7275 6520 666f 7220 6320 696e 2063 616e  rue for c in can
+00004900: 6469 6461 7465 737d 0a20 2020 2073 5f6d  didates}.    s_m
+00004910: 6174 7269 7820 3d20 5b5b 2d6e 702e 696e  atrix = [[-np.in
+00004920: 6620 666f 7220 5f20 696e 2063 616e 6469  f for _ in candi
+00004930: 6461 7465 735d 2066 6f72 205f 2069 6e20  dates] for _ in 
+00004940: 6361 6e64 6964 6174 6573 5d0a 2020 2020  candidates].    
+00004950: 0a20 2020 2023 2069 6e69 7469 616c 697a  .    # initializ
+00004960: 6520 7468 6520 735f 6d61 7472 6978 0a20  e the s_matrix. 
+00004970: 2020 2066 6f72 2063 315f 6964 782c 2063     for c1_idx, c
+00004980: 3120 696e 2065 6e75 6d65 7261 7465 2863  1 in enumerate(c
+00004990: 616e 6469 6461 7465 7329 3a0a 2020 2020  andidates):.    
+000049a0: 2020 2020 666f 7220 6332 5f69 6478 2c20      for c2_idx, 
+000049b0: 6332 2069 6e20 656e 756d 6572 6174 6528  c2 in enumerate(
+000049c0: 6361 6e64 6964 6174 6573 293a 0a20 2020  candidates):.   
+000049d0: 2020 2020 2020 2020 2069 6620 2865 6461           if (eda
+000049e0: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+000049f0: 6572 7328 6331 2c20 6332 2920 6f72 2063  ers(c1, c2) or c
+00004a00: 3120 3d3d 2063 3229 3a0a 2020 2020 2020  1 == c2):.      
+00004a10: 2020 2020 2020 2020 2020 735f 6d61 7472            s_matr
+00004a20: 6978 5b63 315f 6964 785d 5b63 325f 6964  ix[c1_idx][c2_id
+00004a30: 785d 203d 2073 7472 656e 6774 685f 6675  x] = strength_fu
+00004a40: 6e63 7469 6f6e 2863 312c 2063 3229 200a  nction(c1, c2) .
+00004a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a60: 7765 616b 5f63 6f6e 646f 7263 6574 5f77  weak_condorcet_w
+00004a70: 696e 6e65 7273 5b63 325d 203d 2077 6561  inners[c2] = wea
+00004a80: 6b5f 636f 6e64 6f72 6365 745f 7769 6e6e  k_condorcet_winn
+00004a90: 6572 735b 6332 5d20 616e 6420 2863 3120  ers[c2] and (c1 
+00004aa0: 3d3d 2063 3229 2023 2057 6561 6b20 436f  == c2) # Weak Co
+00004ab0: 6e64 6f72 6365 7420 7769 6e6e 6572 7320  ndorcet winners 
+00004ac0: 6172 6520 5370 6c69 7420 4379 636c 6520  are Split Cycle 
+00004ad0: 7769 6e6e 6572 730a 2020 2020 0a20 2020  winners.    .   
+00004ae0: 2073 7472 656e 6774 6820 3d20 6c69 7374   strength = list
+00004af0: 286d 6170 286c 616d 6264 6120 6920 3a20  (map(lambda i : 
+00004b00: 6c69 7374 286d 6170 286c 616d 6264 6120  list(map(lambda 
+00004b10: 6a20 3a20 6a20 2c20 6929 2920 2c20 735f  j : j , i)) , s_
+00004b20: 6d61 7472 6978 2929 0a20 2020 2066 6f72  matrix)).    for
+00004b30: 2069 5f69 6478 2c20 6920 696e 2065 6e75   i_idx, i in enu
+00004b40: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
+00004b50: 7329 3a20 0a20 2020 2020 2020 2066 6f72  s): .        for
+00004b60: 206a 5f69 6478 2c20 6a20 696e 2065 6e75   j_idx, j in enu
+00004b70: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
+00004b80: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00004b90: 6966 2069 213d 206a 3a0a 2020 2020 2020  if i!= j:.      
+00004ba0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00004bb0: 2077 6561 6b5f 636f 6e64 6f72 6365 745f   weak_condorcet_
+00004bc0: 7769 6e6e 6572 735b 6a5d 3a20 2320 7765  winners[j]: # we
+00004bd0: 616b 2043 6f6e 646f 7263 6574 2077 696e  ak Condorcet win
+00004be0: 6e65 7273 2061 7265 2053 706c 6974 2043  ners are Split C
+00004bf0: 7963 6c65 2077 696e 6e65 7273 0a20 2020  ycle winners.   
 00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c10: 2020 666f 7220 6b5f 6964 782c 206b 2069    for k_idx, k i
-00004c20: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
-00004c30: 6964 6174 6573 293a 200a 2020 2020 2020  idates): .      
+00004c10: 2066 6f72 206b 5f69 6478 2c20 6b20 696e   for k_idx, k in
+00004c20: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
+00004c30: 6461 7465 7329 3a20 0a20 2020 2020 2020  dates): .       
 00004c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c50: 2020 6966 2069 2021 3d20 6b20 616e 6420    if i != k and 
-00004c60: 6a20 213d 206b 3a0a 2020 2020 2020 2020  j != k:.        
+00004c50: 2069 6620 6920 213d 206b 2061 6e64 206a   if i != k and j
+00004c60: 2021 3d20 6b3a 0a20 2020 2020 2020 2020   != k:.         
 00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c80: 2020 2020 7374 7265 6e67 7468 5b6a 5f69      strength[j_i
-00004c90: 6478 5d5b 6b5f 6964 785d 203d 206d 6178  dx][k_idx] = max
-00004ca0: 2873 7472 656e 6774 685b 6a5f 6964 785d  (strength[j_idx]
-00004cb0: 5b6b 5f69 6478 5d2c 206d 696e 2873 7472  [k_idx], min(str
-00004cc0: 656e 6774 685b 6a5f 6964 785d 5b69 5f69  ength[j_idx][i_i
-00004cd0: 6478 5d2c 7374 7265 6e67 7468 5b69 5f69  dx],strength[i_i
-00004ce0: 6478 5d5b 6b5f 6964 785d 2929 0a20 2020  dx][k_idx])).   
-00004cf0: 2077 696e 6e65 7273 203d 207b 693a 5472   winners = {i:Tr
-00004d00: 7565 2066 6f72 2069 2069 6e20 6361 6e64  ue for i in cand
-00004d10: 6964 6174 6573 7d0a 2020 2020 666f 7220  idates}.    for 
-00004d20: 695f 6964 782c 2069 2069 6e20 656e 756d  i_idx, i in enum
-00004d30: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
-00004d40: 293a 0a20 2020 2020 2020 2066 6f72 206a  ):.        for j
-00004d50: 5f69 6478 2c20 6a20 696e 2065 6e75 6d65  _idx, j in enume
-00004d60: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-00004d70: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00004d80: 2069 2021 3d20 6a3a 0a20 2020 2020 2020   i != j:.       
-00004d90: 2020 2020 2020 2020 2069 6620 735f 6d61           if s_ma
-00004da0: 7472 6978 5b6a 5f69 6478 5d5b 695f 6964  trix[j_idx][i_id
-00004db0: 785d 203e 2073 7472 656e 6774 685b 695f  x] > strength[i_
-00004dc0: 6964 785d 5b6a 5f69 6478 5d3a 2023 2074  idx][j_idx]: # t
-00004dd0: 6865 206d 6169 6e20 6469 6666 6572 656e  he main differen
-00004de0: 6365 2077 6974 6820 4265 6174 2050 6174  ce with Beat Pat
-00004df0: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
-00004e00: 2020 2020 2020 7769 6e6e 6572 735b 695d        winners[i]
-00004e10: 203d 2046 616c 7365 0a20 2020 2072 6574   = False.    ret
-00004e20: 7572 6e20 736f 7274 6564 285b 6320 666f  urn sorted([c fo
-00004e30: 7220 6320 696e 2063 616e 6469 6461 7465  r c in candidate
-00004e40: 7320 6966 2077 696e 6e65 7273 5b63 5d5d  s if winners[c]]
-00004e50: 290a 0a0a 6465 6620 7370 6c69 745f 6379  )...def split_cy
-00004e60: 636c 655f 6465 6665 6174 2865 6461 7461  cle_defeat(edata
-00004e70: 2c20 6375 7272 5f63 616e 6473 203d 204e  , curr_cands = N
-00004e80: 6f6e 652c 2073 7472 656e 6774 685f 6675  one, strength_fu
-00004e90: 6e63 7469 6f6e 203d 204e 6f6e 6529 3a20  nction = None): 
-00004ea0: 2020 0a20 2020 2022 2222 0a20 2020 2052    .    """.    R
-00004eb0: 6574 7572 6e73 2074 6865 2053 706c 6974  eturns the Split
-00004ec0: 2043 7963 6c65 2064 6566 6561 7420 7265   Cycle defeat re
-00004ed0: 6c61 7469 6f6e 2e20 0a0a 2020 2020 5365  lation. ..    Se
-00004ee0: 6520 6874 7470 733a 2f2f 6172 7869 762e  e https://arxiv.
-00004ef0: 6f72 672f 6162 732f 3230 3038 2e30 3834  org/abs/2008.084
-00004f00: 3531 2066 6f72 2061 6e20 6578 7465 6e64  51 for an extend
-00004f10: 6564 2064 6973 6375 7373 696f 6e20 6f66  ed discussion of
-00004f20: 2074 6869 7320 6e6f 7469 6f6e 206f 6620   this notion of 
-00004f30: 6465 6665 6174 2069 6e20 616e 2065 6c65  defeat in an ele
-00004f40: 6374 696f 6e2e 200a 0a20 2020 2041 7267  ction. ..    Arg
-00004f50: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
-00004f60: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
-00004f70: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
-00004f80: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
-00004f90: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
-00004fa0: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
-00004fb0: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
-00004fc0: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
-00004fd0: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
-00004fe0: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
-00004ff0: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
-00005000: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
-00005010: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
-00005020: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
-00005030: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
-00005040: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
-00005050: 2020 2020 2020 2041 206e 6574 776f 726b         A network
-00005060: 7820 4469 4772 6170 6820 7265 7072 6573  x DiGraph repres
-00005070: 656e 7469 6e67 2074 6865 2053 706c 6974  enting the Split
-00005080: 2043 7963 6c65 2064 6566 6561 7420 7265   Cycle defeat re
-00005090: 6c61 7469 6f6e 2e20 0a0a 2020 2020 2e2e  lation. ..    ..
-000050a0: 2073 6565 616c 736f 3a3a 0a0a 2020 2020   seealso::..    
-000050b0: 2020 2020 3a6d 6574 683a 6070 7265 665f      :meth:`pref_
-000050c0: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-000050d0: 7365 645f 6d65 7468 6f64 732e 7370 6c69  sed_methods.spli
-000050e0: 745f 6379 636c 6560 2c20 3a6d 6574 683a  t_cycle`, :meth:
-000050f0: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
-00005100: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
-00005110: 732e 7370 6c69 745f 6379 636c 655f 466c  s.split_cycle_Fl
-00005120: 6f79 645f 5761 7273 6861 6c6c 600a 0a20  oyd_Warshall`.. 
-00005130: 2020 203a 4578 616d 706c 653a 200a 0a20     :Example: .. 
-00005140: 2020 202e 2e20 706c 6f74 3a3a 2020 6d61     .. plot::  ma
-00005150: 7267 696e 5f67 7261 7068 735f 6578 616d  rgin_graphs_exam
-00005160: 706c 6573 2f6d 675f 6578 5f73 635f 6465  ples/mg_ex_sc_de
-00005170: 6665 6174 2e70 790a 2020 2020 2020 2020  feat.py.        
-00005180: 3a63 6f6e 7465 7874 3a20 7265 7365 7420  :context: reset 
-00005190: 200a 2020 2020 2020 2020 3a69 6e63 6c75   .        :inclu
-000051a0: 6465 2d73 6f75 7263 653a 2054 7275 650a  de-source: True.
-000051b0: 0a20 2020 2022 2222 0a0a 2020 2020 6361  .    """..    ca
-000051c0: 6e64 6964 6174 6573 203d 2065 6461 7461  ndidates = edata
-000051d0: 2e63 616e 6469 6461 7465 7320 6966 2063  .candidates if c
-000051e0: 7572 725f 6361 6e64 7320 6973 204e 6f6e  urr_cands is Non
-000051f0: 6520 656c 7365 2063 7572 725f 6361 6e64  e else curr_cand
-00005200: 7320 2020 200a 2020 2020 7374 7265 6e67  s    .    streng
-00005210: 7468 5f66 756e 6374 696f 6e20 3d20 6564  th_function = ed
-00005220: 6174 612e 6d61 7267 696e 2069 6620 7374  ata.margin if st
-00005230: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-00005240: 6973 204e 6f6e 6520 656c 7365 2073 7472  is None else str
-00005250: 656e 6774 685f 6675 6e63 7469 6f6e 200a  ength_function .
-00005260: 200a 2020 2020 7765 616b 5f63 6f6e 646f   .    weak_condo
-00005270: 7263 6574 5f77 696e 6e65 7273 203d 207b  rcet_winners = {
-00005280: 633a 5472 7565 2066 6f72 2063 2069 6e20  c:True for c in 
-00005290: 6361 6e64 6964 6174 6573 7d0a 2020 2020  candidates}.    
-000052a0: 735f 6d61 7472 6978 203d 205b 5b2d 6e70  s_matrix = [[-np
-000052b0: 2e69 6e66 2066 6f72 205f 2069 6e20 6361  .inf for _ in ca
-000052c0: 6e64 6964 6174 6573 5d20 666f 7220 5f20  ndidates] for _ 
-000052d0: 696e 2063 616e 6469 6461 7465 735d 0a20  in candidates]. 
-000052e0: 2020 200a 2020 2020 2320 696e 6974 6961     .    # initia
-000052f0: 6c69 7a65 2074 6865 2073 5f6d 6174 7269  lize the s_matri
-00005300: 780a 2020 2020 666f 7220 6331 5f69 6478  x.    for c1_idx
-00005310: 2c20 6331 2069 6e20 656e 756d 6572 6174  , c1 in enumerat
-00005320: 6528 6361 6e64 6964 6174 6573 293a 0a20  e(candidates):. 
-00005330: 2020 2020 2020 2066 6f72 2063 325f 6964         for c2_id
-00005340: 782c 2063 3220 696e 2065 6e75 6d65 7261  x, c2 in enumera
-00005350: 7465 2863 616e 6469 6461 7465 7329 3a0a  te(candidates):.
-00005360: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00005370: 6564 6174 612e 6d61 6a6f 7269 7479 5f70  edata.majority_p
-00005380: 7265 6665 7273 2863 312c 2063 3229 206f  refers(c1, c2) o
-00005390: 7220 6331 203d 3d20 6332 293a 0a20 2020  r c1 == c2):.   
-000053a0: 2020 2020 2020 2020 2020 2020 2073 5f6d               s_m
-000053b0: 6174 7269 785b 6331 5f69 6478 5d5b 6332  atrix[c1_idx][c2
-000053c0: 5f69 6478 5d20 3d20 7374 7265 6e67 7468  _idx] = strength
-000053d0: 5f66 756e 6374 696f 6e28 6331 2c20 6332  _function(c1, c2
-000053e0: 2920 0a20 2020 2020 2020 2020 2020 2020  ) .             
-000053f0: 2020 2077 6561 6b5f 636f 6e64 6f72 6365     weak_condorce
-00005400: 745f 7769 6e6e 6572 735b 6332 5d20 3d20  t_winners[c2] = 
-00005410: 7765 616b 5f63 6f6e 646f 7263 6574 5f77  weak_condorcet_w
-00005420: 696e 6e65 7273 5b63 325d 2061 6e64 2028  inners[c2] and (
-00005430: 6331 203d 3d20 6332 2920 2320 7765 616b  c1 == c2) # weak
-00005440: 2043 6f6e 646f 7263 6574 2077 696e 6e65   Condorcet winne
-00005450: 7273 2061 7265 2053 706c 6974 2043 7963  rs are Split Cyc
-00005460: 6c65 2077 696e 6e65 7273 0a20 2020 200a  le winners.    .
-00005470: 2020 2020 7374 7265 6e67 7468 203d 206c      strength = l
-00005480: 6973 7428 6d61 7028 6c61 6d62 6461 2069  ist(map(lambda i
-00005490: 203a 206c 6973 7428 6d61 7028 6c61 6d62   : list(map(lamb
-000054a0: 6461 206a 203a 206a 202c 2069 2929 202c  da j : j , i)) ,
-000054b0: 2073 5f6d 6174 7269 7829 290a 2020 2020   s_matrix)).    
-000054c0: 666f 7220 695f 6964 782c 2069 2069 6e20  for i_idx, i in 
-000054d0: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
-000054e0: 6174 6573 293a 200a 2020 2020 2020 2020  ates): .        
-000054f0: 666f 7220 6a5f 6964 782c 206a 2069 6e20  for j_idx, j in 
-00005500: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
-00005510: 6174 6573 293a 0a20 2020 2020 2020 2020  ates):.         
-00005520: 2020 2069 6620 6921 3d20 6a3a 0a20 2020     if i!= j:.   
-00005530: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005540: 6e6f 7420 7765 616b 5f63 6f6e 646f 7263  not weak_condorc
-00005550: 6574 5f77 696e 6e65 7273 5b6a 5d3a 2023  et_winners[j]: #
-00005560: 2077 6561 6b20 436f 6e64 6f72 6365 7420   weak Condorcet 
-00005570: 7769 6e6e 6572 7320 6172 6520 5370 6c69  winners are Spli
-00005580: 7420 4379 636c 6520 7769 6e6e 6572 730a  t Cycle winners.
+00004c80: 2020 2073 7472 656e 6774 685b 6a5f 6964     strength[j_id
+00004c90: 785d 5b6b 5f69 6478 5d20 3d20 6d61 7828  x][k_idx] = max(
+00004ca0: 7374 7265 6e67 7468 5b6a 5f69 6478 5d5b  strength[j_idx][
+00004cb0: 6b5f 6964 785d 2c20 6d69 6e28 7374 7265  k_idx], min(stre
+00004cc0: 6e67 7468 5b6a 5f69 6478 5d5b 695f 6964  ngth[j_idx][i_id
+00004cd0: 785d 2c73 7472 656e 6774 685b 695f 6964  x],strength[i_id
+00004ce0: 785d 5b6b 5f69 6478 5d29 290a 2020 2020  x][k_idx])).    
+00004cf0: 7769 6e6e 6572 7320 3d20 7b69 3a54 7275  winners = {i:Tru
+00004d00: 6520 666f 7220 6920 696e 2063 616e 6469  e for i in candi
+00004d10: 6461 7465 737d 0a20 2020 2066 6f72 2069  dates}.    for i
+00004d20: 5f69 6478 2c20 6920 696e 2065 6e75 6d65  _idx, i in enume
+00004d30: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+00004d40: 3a0a 2020 2020 2020 2020 666f 7220 6a5f  :.        for j_
+00004d50: 6964 782c 206a 2069 6e20 656e 756d 6572  idx, j in enumer
+00004d60: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
+00004d70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00004d80: 6920 213d 206a 3a0a 2020 2020 2020 2020  i != j:.        
+00004d90: 2020 2020 2020 2020 6966 2073 5f6d 6174          if s_mat
+00004da0: 7269 785b 6a5f 6964 785d 5b69 5f69 6478  rix[j_idx][i_idx
+00004db0: 5d20 3e20 7374 7265 6e67 7468 5b69 5f69  ] > strength[i_i
+00004dc0: 6478 5d5b 6a5f 6964 785d 3a20 2320 7468  dx][j_idx]: # th
+00004dd0: 6520 6d61 696e 2064 6966 6665 7265 6e63  e main differenc
+00004de0: 6520 7769 7468 2042 6561 7420 5061 7468  e with Beat Path
+00004df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004e00: 2020 2020 2077 696e 6e65 7273 5b69 5d20       winners[i] 
+00004e10: 3d20 4661 6c73 650a 2020 2020 7265 7475  = False.    retu
+00004e20: 726e 2073 6f72 7465 6428 5b63 2066 6f72  rn sorted([c for
+00004e30: 2063 2069 6e20 6361 6e64 6964 6174 6573   c in candidates
+00004e40: 2069 6620 7769 6e6e 6572 735b 635d 5d29   if winners[c]])
+00004e50: 0a0a 0a64 6566 2073 706c 6974 5f63 7963  ...def split_cyc
+00004e60: 6c65 5f64 6566 6561 7428 6564 6174 612c  le_defeat(edata,
+00004e70: 2063 7572 725f 6361 6e64 7320 3d20 4e6f   curr_cands = No
+00004e80: 6e65 2c20 7374 7265 6e67 7468 5f66 756e  ne, strength_fun
+00004e90: 6374 696f 6e20 3d20 4e6f 6e65 293a 2020  ction = None):  
+00004ea0: 200a 2020 2020 2222 220a 2020 2020 5265   .    """.    Re
+00004eb0: 7475 726e 7320 7468 6520 5370 6c69 7420  turns the Split 
+00004ec0: 4379 636c 6520 6465 6665 6174 2072 656c  Cycle defeat rel
+00004ed0: 6174 696f 6e2e 200a 0a20 2020 2053 6565  ation. ..    See
+00004ee0: 2068 7474 7073 3a2f 2f61 7278 6976 2e6f   https://arxiv.o
+00004ef0: 7267 2f61 6273 2f32 3030 382e 3038 3435  rg/abs/2008.0845
+00004f00: 3120 666f 7220 616e 2065 7874 656e 6465  1 for an extende
+00004f10: 6420 6469 7363 7573 7369 6f6e 206f 6620  d discussion of 
+00004f20: 7468 6973 206e 6f74 696f 6e20 6f66 2064  this notion of d
+00004f30: 6566 6561 7420 696e 2061 6e20 656c 6563  efeat in an elec
+00004f40: 7469 6f6e 2e20 0a0a 2020 2020 4172 6773  tion. ..    Args
+00004f50: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
+00004f60: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
+00004f70: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
+00004f80: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
+00004f90: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
+00004fa0: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
+00004fb0: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
+00004fc0: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
+00004fd0: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
+00004fe0: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
+00004ff0: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
+00005000: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
+00005010: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
+00005020: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
+00005030: 6060 6375 7272 5f63 616e 6473 6060 0a0a  ``curr_cands``..
+00005040: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
+00005050: 2020 2020 2020 4120 6e65 7477 6f72 6b78        A networkx
+00005060: 2044 6947 7261 7068 2072 6570 7265 7365   DiGraph represe
+00005070: 6e74 696e 6720 7468 6520 5370 6c69 7420  nting the Split 
+00005080: 4379 636c 6520 6465 6665 6174 2072 656c  Cycle defeat rel
+00005090: 6174 696f 6e2e 200a 0a20 2020 202e 2e20  ation. ..    .. 
+000050a0: 7365 6561 6c73 6f3a 3a0a 0a20 2020 2020  seealso::..     
+000050b0: 2020 203a 6d65 7468 3a60 7072 6566 5f76     :meth:`pref_v
+000050c0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
+000050d0: 6564 5f6d 6574 686f 6473 2e73 706c 6974  ed_methods.split
+000050e0: 5f63 7963 6c65 602c 203a 6d65 7468 3a60  _cycle`, :meth:`
+000050f0: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+00005100: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+00005110: 2e73 706c 6974 5f63 7963 6c65 5f46 6c6f  .split_cycle_Flo
+00005120: 7964 5f57 6172 7368 616c 6c60 0a0a 2020  yd_Warshall`..  
+00005130: 2020 3a45 7861 6d70 6c65 3a20 0a0a 2020    :Example: ..  
+00005140: 2020 2e2e 2070 6c6f 743a 3a20 206d 6172    .. plot::  mar
+00005150: 6769 6e5f 6772 6170 6873 5f65 7861 6d70  gin_graphs_examp
+00005160: 6c65 732f 6d67 5f65 785f 7363 5f64 6566  les/mg_ex_sc_def
+00005170: 6561 742e 7079 0a20 2020 2020 2020 203a  eat.py.        :
+00005180: 636f 6e74 6578 743a 2072 6573 6574 2020  context: reset  
+00005190: 0a20 2020 2020 2020 203a 696e 636c 7564  .        :includ
+000051a0: 652d 736f 7572 6365 3a20 5472 7565 0a0a  e-source: True..
+000051b0: 2020 2020 2222 220a 0a20 2020 2063 616e      """..    can
+000051c0: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
+000051d0: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
+000051e0: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
+000051f0: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
+00005200: 2020 2020 0a20 2020 2073 7472 656e 6774      .    strengt
+00005210: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
+00005220: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
+00005230: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
+00005240: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
+00005250: 6e67 7468 5f66 756e 6374 696f 6e20 0a20  ngth_function . 
+00005260: 0a20 2020 2077 6561 6b5f 636f 6e64 6f72  .    weak_condor
+00005270: 6365 745f 7769 6e6e 6572 7320 3d20 7b63  cet_winners = {c
+00005280: 3a54 7275 6520 666f 7220 6320 696e 2063  :True for c in c
+00005290: 616e 6469 6461 7465 737d 0a20 2020 2073  andidates}.    s
+000052a0: 5f6d 6174 7269 7820 3d20 5b5b 2d6e 702e  _matrix = [[-np.
+000052b0: 696e 6620 666f 7220 5f20 696e 2063 616e  inf for _ in can
+000052c0: 6469 6461 7465 735d 2066 6f72 205f 2069  didates] for _ i
+000052d0: 6e20 6361 6e64 6964 6174 6573 5d0a 2020  n candidates].  
+000052e0: 2020 0a20 2020 2023 2069 6e69 7469 616c    .    # initial
+000052f0: 697a 6520 7468 6520 735f 6d61 7472 6978  ize the s_matrix
+00005300: 0a20 2020 2066 6f72 2063 315f 6964 782c  .    for c1_idx,
+00005310: 2063 3120 696e 2065 6e75 6d65 7261 7465   c1 in enumerate
+00005320: 2863 616e 6469 6461 7465 7329 3a0a 2020  (candidates):.  
+00005330: 2020 2020 2020 666f 7220 6332 5f69 6478        for c2_idx
+00005340: 2c20 6332 2069 6e20 656e 756d 6572 6174  , c2 in enumerat
+00005350: 6528 6361 6e64 6964 6174 6573 293a 0a20  e(candidates):. 
+00005360: 2020 2020 2020 2020 2020 2069 6620 2865             if (e
+00005370: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
+00005380: 6566 6572 7328 6331 2c20 6332 2920 6f72  efers(c1, c2) or
+00005390: 2063 3120 3d3d 2063 3229 3a0a 2020 2020   c1 == c2):.    
+000053a0: 2020 2020 2020 2020 2020 2020 735f 6d61              s_ma
+000053b0: 7472 6978 5b63 315f 6964 785d 5b63 325f  trix[c1_idx][c2_
+000053c0: 6964 785d 203d 2073 7472 656e 6774 685f  idx] = strength_
+000053d0: 6675 6e63 7469 6f6e 2863 312c 2063 3229  function(c1, c2)
+000053e0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+000053f0: 2020 7765 616b 5f63 6f6e 646f 7263 6574    weak_condorcet
+00005400: 5f77 696e 6e65 7273 5b63 325d 203d 2077  _winners[c2] = w
+00005410: 6561 6b5f 636f 6e64 6f72 6365 745f 7769  eak_condorcet_wi
+00005420: 6e6e 6572 735b 6332 5d20 616e 6420 2863  nners[c2] and (c
+00005430: 3120 3d3d 2063 3229 2023 2077 6561 6b20  1 == c2) # weak 
+00005440: 436f 6e64 6f72 6365 7420 7769 6e6e 6572  Condorcet winner
+00005450: 7320 6172 6520 5370 6c69 7420 4379 636c  s are Split Cycl
+00005460: 6520 7769 6e6e 6572 730a 2020 2020 0a20  e winners.    . 
+00005470: 2020 2073 7472 656e 6774 6820 3d20 6c69     strength = li
+00005480: 7374 286d 6170 286c 616d 6264 6120 6920  st(map(lambda i 
+00005490: 3a20 6c69 7374 286d 6170 286c 616d 6264  : list(map(lambd
+000054a0: 6120 6a20 3a20 6a20 2c20 6929 2920 2c20  a j : j , i)) , 
+000054b0: 735f 6d61 7472 6978 2929 0a20 2020 2066  s_matrix)).    f
+000054c0: 6f72 2069 5f69 6478 2c20 6920 696e 2065  or i_idx, i in e
+000054d0: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
+000054e0: 7465 7329 3a20 0a20 2020 2020 2020 2066  tes): .        f
+000054f0: 6f72 206a 5f69 6478 2c20 6a20 696e 2065  or j_idx, j in e
+00005500: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
+00005510: 7465 7329 3a0a 2020 2020 2020 2020 2020  tes):.          
+00005520: 2020 6966 2069 213d 206a 3a0a 2020 2020    if i!= j:.    
+00005530: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00005540: 6f74 2077 6561 6b5f 636f 6e64 6f72 6365  ot weak_condorce
+00005550: 745f 7769 6e6e 6572 735b 6a5d 3a20 2320  t_winners[j]: # 
+00005560: 7765 616b 2043 6f6e 646f 7263 6574 2077  weak Condorcet w
+00005570: 696e 6e65 7273 2061 7265 2053 706c 6974  inners are Split
+00005580: 2043 7963 6c65 2077 696e 6e65 7273 0a20   Cycle winners. 
 00005590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055a0: 2020 2020 666f 7220 6b5f 6964 782c 206b      for k_idx, k
-000055b0: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-000055c0: 6e64 6964 6174 6573 293a 200a 2020 2020  ndidates): .    
+000055a0: 2020 2066 6f72 206b 5f69 6478 2c20 6b20     for k_idx, k 
+000055b0: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+000055c0: 6469 6461 7465 7329 3a20 0a20 2020 2020  didates): .     
 000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055e0: 2020 2020 6966 2069 2021 3d20 6b20 616e      if i != k an
-000055f0: 6420 6a20 213d 206b 3a0a 2020 2020 2020  d j != k:.      
+000055e0: 2020 2069 6620 6920 213d 206b 2061 6e64     if i != k and
+000055f0: 206a 2021 3d20 6b3a 0a20 2020 2020 2020   j != k:.       
 00005600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005610: 2020 2020 2020 7374 7265 6e67 7468 5b6a        strength[j
-00005620: 5f69 6478 5d5b 6b5f 6964 785d 203d 206d  _idx][k_idx] = m
-00005630: 6178 2873 7472 656e 6774 685b 6a5f 6964  ax(strength[j_id
-00005640: 785d 5b6b 5f69 6478 5d2c 206d 696e 2873  x][k_idx], min(s
-00005650: 7472 656e 6774 685b 6a5f 6964 785d 5b69  trength[j_idx][i
-00005660: 5f69 6478 5d2c 7374 7265 6e67 7468 5b69  _idx],strength[i
-00005670: 5f69 6478 5d5b 6b5f 6964 785d 2929 0a20  _idx][k_idx])). 
-00005680: 0a20 2020 2064 6566 6561 745f 6772 6170  .    defeat_grap
-00005690: 6820 3d20 6e78 2e44 6947 7261 7068 2829  h = nx.DiGraph()
-000056a0: 0a20 2020 2064 6566 6561 745f 6772 6170  .    defeat_grap
-000056b0: 682e 6164 645f 6e6f 6465 735f 6672 6f6d  h.add_nodes_from
-000056c0: 2863 616e 6469 6461 7465 7329 0a0a 2020  (candidates)..  
-000056d0: 2020 666f 7220 695f 6964 782c 2069 2069    for i_idx, i i
-000056e0: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
-000056f0: 6964 6174 6573 293a 0a20 2020 2020 2020  idates):.       
-00005700: 2066 6f72 206a 5f69 6478 2c20 6a20 696e   for j_idx, j in
-00005710: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
-00005720: 6461 7465 7329 3a0a 2020 2020 2020 2020  dates):.        
-00005730: 2020 2020 6966 2069 2021 3d20 6a3a 0a20      if i != j:. 
-00005740: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005750: 6620 735f 6d61 7472 6978 5b6a 5f69 6478  f s_matrix[j_idx
-00005760: 5d5b 695f 6964 785d 203e 2073 7472 656e  ][i_idx] > stren
-00005770: 6774 685b 695f 6964 785d 5b6a 5f69 6478  gth[i_idx][j_idx
-00005780: 5d3a 2023 2074 6865 206d 6169 6e20 6469  ]: # the main di
-00005790: 6666 6572 656e 6365 2077 6974 6820 4265  fference with Be
-000057a0: 6174 2050 6174 680a 2020 2020 2020 2020  at Path.        
-000057b0: 2020 2020 2020 2020 2020 2020 6465 6665              defe
-000057c0: 6174 5f67 7261 7068 2e61 6464 5f77 6569  at_graph.add_wei
-000057d0: 6768 7465 645f 6564 6765 735f 6672 6f6d  ghted_edges_from
-000057e0: 285b 286a 2c69 2c73 5f6d 6174 7269 785b  ([(j,i,s_matrix[
-000057f0: 6a5f 6964 785d 5b69 5f69 6478 5d29 5d29  j_idx][i_idx])])
-00005800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005810: 200a 2020 2020 7265 7475 726e 2064 6566   .    return def
-00005820: 6561 745f 6772 6170 680a 0a0a 0a23 2066  eat_graph....# f
-00005830: 6c61 7474 656e 2061 2032 6420 6c69 7374  latten a 2d list
-00005840: 202d 2074 7572 6e20 6120 3264 206c 6973   - turn a 2d lis
-00005850: 7420 696e 746f 2061 2073 696e 676c 6520  t into a single 
-00005860: 6c69 7374 206f 6620 6974 656d 730a 666c  list of items.fl
-00005870: 6174 7465 6e20 3d20 6c61 6d62 6461 206c  atten = lambda l
-00005880: 3a20 5b69 7465 6d20 666f 7220 7375 626c  : [item for subl
-00005890: 6973 7420 696e 206c 2066 6f72 2069 7465  ist in l for ite
-000058a0: 6d20 696e 2073 7562 6c69 7374 5d0a 0a64  m in sublist]..d
-000058b0: 6566 2064 6f65 735f 6372 6561 7465 5f63  ef does_create_c
-000058c0: 7963 6c65 2867 2c20 6564 6765 293a 0a20  ycle(g, edge):. 
-000058d0: 2020 2027 2727 7265 7475 726e 2054 7275     '''return Tru
-000058e0: 6520 6966 2061 6464 696e 6720 7468 6520  e if adding the 
-000058f0: 6564 6765 2074 6f20 6720 6372 6561 7465  edge to g create
-00005900: 2061 2063 7963 6c65 2e0a 2020 2020 6974   a cycle..    it
-00005910: 2069 7320 6173 7375 6d65 6420 7468 6174   is assumed that
-00005920: 2065 6467 6520 6973 2061 6c72 6561 6479   edge is already
-00005930: 2069 6e20 6727 2727 0a20 2020 2073 6f75   in g'''.    sou
-00005940: 7263 6520 3d20 6564 6765 5b30 5d0a 2020  rce = edge[0].  
-00005950: 2020 7461 7267 6574 203d 2065 6467 655b    target = edge[
-00005960: 315d 0a20 2020 2066 6f72 206e 2069 6e20  1].    for n in 
-00005970: 672e 7072 6564 6563 6573 736f 7273 2873  g.predecessors(s
-00005980: 6f75 7263 6529 3a0a 2020 2020 2020 2020  ource):.        
-00005990: 6966 206e 782e 6861 735f 7061 7468 2867  if nx.has_path(g
-000059a0: 2c20 7461 7267 6574 2c20 6e29 3a20 0a20  , target, n): . 
-000059b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000059c0: 6e20 5472 7565 0a20 2020 2072 6574 7572  n True.    retur
-000059d0: 6e20 4661 6c73 650a 0a40 766d 286e 616d  n False..@vm(nam
-000059e0: 653d 2252 616e 6b65 6420 5061 6972 7322  e="Ranked Pairs"
-000059f0: 290a 6465 6620 7261 6e6b 6564 5f70 6169  ).def ranked_pai
-00005a00: 7273 2865 6461 7461 2c20 6375 7272 5f63  rs(edata, curr_c
-00005a10: 616e 6473 203d 204e 6f6e 652c 2073 7472  ands = None, str
-00005a20: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-00005a30: 204e 6f6e 6529 3a20 2020 0a20 2020 2022   None):   .    "
-00005a40: 2222 0a20 2020 204f 7264 6572 2074 6865  "".    Order the
-00005a50: 2065 6467 6573 2069 6e20 7468 6520 6d61   edges in the ma
-00005a60: 7267 696e 2067 7261 7068 2066 726f 6d20  rgin graph from 
-00005a70: 6c61 7267 6573 7420 746f 2073 6d61 6c6c  largest to small
-00005a80: 6573 7420 616e 6420 6c6f 636b 2074 6865  est and lock the
-00005a90: 6d20 696e 2069 6e20 7468 6174 206f 7264  m in in that ord
-00005aa0: 6572 2c20 736b 6970 7069 6e67 2065 6467  er, skipping edg
-00005ab0: 6573 2074 6861 7420 6372 6561 7465 2061  es that create a
-00005ac0: 2063 7963 6c65 2e20 2049 6620 7468 6572   cycle.  If ther
-00005ad0: 6520 6172 6520 7469 6573 2069 6e20 7468  e are ties in th
-00005ae0: 6520 6d61 7267 696e 732c 2062 7265 616b  e margins, break
-00005af0: 2074 6865 2074 6965 7320 7573 696e 6720   the ties using 
-00005b00: 6120 7469 652d 6272 6561 6b69 6e67 2072  a tie-breaking r
-00005b10: 756c 653a 2061 206c 696e 6561 7220 6f72  ule: a linear or
-00005b20: 6465 7269 6e67 206f 7665 7220 7468 6520  dering over the 
-00005b30: 6564 6765 732e 2020 2041 2063 616e 6469  edges.   A candi
-00005b40: 6461 7465 2069 7320 6120 5261 6e6b 6564  date is a Ranked
-00005b50: 2050 6169 7273 2077 696e 6e65 7220 6966   Pairs winner if
-00005b60: 2069 7420 7769 6e73 2061 6363 6f72 6469   it wins accordi
-00005b70: 6e67 2074 6f20 736f 6d65 2074 6965 2d62  ng to some tie-b
-00005b80: 7265 616b 696e 6720 7275 6c65 2e20 416c  reaking rule. Al
-00005b90: 736f 206b 6e6f 776e 2061 7320 5469 6465  so known as Tide
-00005ba0: 6d61 6e27 7320 5275 6c65 2e0a 0a20 2020  man's Rule...   
-00005bb0: 202e 2e20 7761 726e 696e 673a 3a20 0a20   .. warning:: . 
-00005bc0: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
-00005bd0: 6f64 2063 616e 2074 616b 6520 6120 7665  od can take a ve
-00005be0: 7279 206c 6f6e 6720 7469 6d65 2074 6f20  ry long time to 
-00005bf0: 6669 6e64 2077 696e 6e65 7273 2e20 0a20  find winners. . 
-00005c00: 2020 2020 2020 200a 2020 2020 4172 6773         .    Args
-00005c10: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
-00005c20: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
-00005c30: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
-00005c40: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
-00005c50: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
-00005c60: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
-00005c70: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
-00005c80: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
-00005c90: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
-00005ca0: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
-00005cb0: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
-00005cc0: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
-00005cd0: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
-00005ce0: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
-00005cf0: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
-00005d00: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
-00005d10: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
-00005d20: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
-00005d30: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
-00005d40: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
-00005d50: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
-00005d60: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
-00005d70: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
-00005d80: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
-00005d90: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
-00005da0: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
-00005db0: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
-00005dc0: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
-00005dd0: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
-00005de0: 2e20 0a0a 2020 2020 5265 7475 726e 733a  . ..    Returns:
-00005df0: 200a 2020 2020 2020 2020 4120 736f 7274   .        A sort
-00005e00: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
-00005e10: 6461 7465 732e 200a 0a20 2020 202e 2e20  dates. ..    .. 
-00005e20: 7365 6561 6c73 6f3a 3a0a 0a20 2020 2020  seealso::..     
-00005e30: 2020 203a 6d65 7468 3a60 7072 6566 5f76     :meth:`pref_v
-00005e40: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-00005e50: 6564 5f6d 6574 686f 6473 2e72 616e 6b65  ed_methods.ranke
-00005e60: 645f 7061 6972 735f 7769 7468 5f74 6573  d_pairs_with_tes
-00005e70: 7460 2c20 3a6d 6574 683a 6070 7265 665f  t`, :meth:`pref_
-00005e80: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-00005e90: 7365 645f 6d65 7468 6f64 732e 7261 6e6b  sed_methods.rank
-00005ea0: 6564 5f70 6169 7273 5f7a 7460 2c20 3a6d  ed_pairs_zt`, :m
-00005eb0: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
-00005ec0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-00005ed0: 7468 6f64 732e 7261 6e6b 6564 5f70 6169  thods.ranked_pai
-00005ee0: 7273 5f64 6566 6561 7473 600a 0a20 2020  rs_defeats`..   
-00005ef0: 203a 4578 616d 706c 653a 200a 0a20 2020   :Example: ..   
-00005f00: 202e 2e20 706c 6f74 3a3a 2020 6d61 7267   .. plot::  marg
-00005f10: 696e 5f67 7261 7068 735f 6578 616d 706c  in_graphs_exampl
-00005f20: 6573 2f6d 675f 6578 5f62 705f 7270 2e70  es/mg_ex_bp_rp.p
-00005f30: 790a 2020 2020 2020 2020 3a63 6f6e 7465  y.        :conte
-00005f40: 7874 3a20 7265 7365 7420 200a 2020 2020  xt: reset  .    
-00005f50: 2020 2020 3a69 6e63 6c75 6465 2d73 6f75      :include-sou
-00005f60: 7263 653a 2054 7275 650a 0a0a 2020 2020  rce: True...    
-00005f70: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-00005f80: 0a0a 2020 2020 2020 2020 6672 6f6d 2070  ..        from p
-00005f90: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-00005fa0: 6e5f 6261 7365 645f 6d65 7468 6f64 7320  n_based_methods 
-00005fb0: 696d 706f 7274 2072 616e 6b65 645f 7061  import ranked_pa
-00005fc0: 6972 730a 0a20 2020 2020 2020 2072 616e  irs..        ran
-00005fd0: 6b65 645f 7061 6972 732e 6469 7370 6c61  ked_pairs.displa
-00005fe0: 7928 6d67 290a 0a0a 2020 2020 2e2e 2065  y(mg)...    .. e
-00005ff0: 7865 635f 636f 6465 3a3a 200a 2020 2020  xec_code:: .    
-00006000: 2020 2020 3a68 6964 655f 636f 6465 3a0a      :hide_code:.
-00006010: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
-00006020: 6566 5f76 6f74 696e 672e 7765 6967 6874  ef_voting.weight
-00006030: 6564 5f6d 616a 6f72 6974 795f 6772 6170  ed_majority_grap
-00006040: 6873 2069 6d70 6f72 7420 4d61 7267 696e  hs import Margin
-00006050: 4772 6170 680a 2020 2020 2020 2020 6672  Graph.        fr
-00006060: 6f6d 2070 7265 665f 766f 7469 6e67 2e6d  om pref_voting.m
-00006070: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-00006080: 6f64 7320 696d 706f 7274 2072 616e 6b65  ods import ranke
-00006090: 645f 7061 6972 730a 2020 2020 2020 2020  d_pairs.        
-000060a0: 0a20 2020 2020 2020 206d 6720 3d20 4d61  .        mg = Ma
-000060b0: 7267 696e 4772 6170 6828 5b30 2c20 312c  rginGraph([0, 1,
-000060c0: 2032 2c20 335d 2c20 5b28 302c 2032 2c20   2, 3], [(0, 2, 
-000060d0: 3329 2c20 2831 2c20 302c 2035 292c 2028  3), (1, 0, 5), (
-000060e0: 322c 2031 2c20 3529 2c20 2832 2c20 332c  2, 1, 5), (2, 3,
-000060f0: 2031 292c 2028 332c 2030 2c20 3329 2c20   1), (3, 0, 3), 
-00006100: 2833 2c20 312c 2031 295d 290a 2020 2020  (3, 1, 1)]).    
-00006110: 2020 2020 0a20 2020 2020 2020 2072 616e      .        ran
-00006120: 6b65 645f 7061 6972 732e 6469 7370 6c61  ked_pairs.displa
-00006130: 7928 6d67 290a 0a20 2020 2022 2222 0a20  y(mg)..    """. 
-00006140: 2020 2063 616e 6469 6461 7465 7320 3d20     candidates = 
-00006150: 6564 6174 612e 6361 6e64 6964 6174 6573  edata.candidates
-00006160: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
-00006170: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
-00006180: 5f63 616e 6473 200a 2020 2020 6369 6478  _cands .    cidx
-00006190: 5f74 6f5f 6361 6e64 203d 207b 6369 6478  _to_cand = {cidx
-000061a0: 3a20 6320 666f 7220 6369 6478 2c20 6320  : c for cidx, c 
-000061b0: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
-000061c0: 6469 6461 7465 7329 7d20 200a 2020 2020  didates)}  .    
-000061d0: 6361 6e64 5f74 6f5f 6369 6478 203d 207b  cand_to_cidx = {
-000061e0: 633a 2063 6964 7820 666f 7220 6369 6478  c: cidx for cidx
-000061f0: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
-00006200: 2863 616e 6469 6461 7465 7329 7d20 200a  (candidates)}  .
-00006210: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
-00006220: 6374 696f 6e20 3d20 6564 6174 612e 6d61  ction = edata.ma
-00006230: 7267 696e 2069 6620 7374 7265 6e67 7468  rgin if strength
-00006240: 5f66 756e 6374 696f 6e20 6973 204e 6f6e  _function is Non
-00006250: 6520 656c 7365 2073 7472 656e 6774 685f  e else strength_
-00006260: 6675 6e63 7469 6f6e 2020 2020 0a0a 2020  function    ..  
-00006270: 2020 6377 203d 2065 6461 7461 2e63 6f6e    cw = edata.con
-00006280: 646f 7263 6574 5f77 696e 6e65 7228 6375  dorcet_winner(cu
-00006290: 7272 5f63 616e 6473 3d63 7572 725f 6361  rr_cands=curr_ca
-000062a0: 6e64 7329 0a20 2020 2023 2052 616e 6b65  nds).    # Ranke
-000062b0: 6420 5061 6972 7320 6973 2043 6f6e 646f  d Pairs is Condo
-000062c0: 7263 6574 2063 6f6e 7369 7374 656e 742c  rcet consistent,
-000062d0: 2073 6f20 7369 6d70 6c79 2072 6574 7572   so simply retur
-000062e0: 6e20 7468 6520 436f 6e64 6f72 6365 7420  n the Condorcet 
-000062f0: 7769 6e6e 6572 2069 6620 6578 6973 7473  winner if exists
-00006300: 0a20 2020 2069 6620 6377 2069 7320 6e6f  .    if cw is no
-00006310: 7420 4e6f 6e65 3a20 0a20 2020 2020 2020  t None: .       
-00006320: 2077 696e 6e65 7273 203d 205b 6377 5d0a   winners = [cw].
-00006330: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00006340: 2020 775f 6564 6765 7320 3d20 5b28 6331    w_edges = [(c1
-00006350: 2c20 6332 2c20 7374 7265 6e67 7468 5f66  , c2, strength_f
-00006360: 756e 6374 696f 6e28 6331 2c20 6332 2929  unction(c1, c2))
-00006370: 2066 6f72 2063 3120 696e 2063 616e 6469   for c1 in candi
-00006380: 6461 7465 7320 666f 7220 6332 2069 6e20  dates for c2 in 
-00006390: 6361 6e64 6964 6174 6573 200a 2020 2020  candidates .    
-000063a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000063b0: 6620 6331 2021 3d20 6332 2061 6e64 2028  f c1 != c2 and (
-000063c0: 6564 6174 612e 6d61 6a6f 7269 7479 5f70  edata.majority_p
-000063d0: 7265 6665 7273 2863 312c 2063 3229 206f  refers(c1, c2) o
-000063e0: 7220 6564 6174 612e 6973 5f74 6965 6428  r edata.is_tied(
-000063f0: 6331 2c20 6332 2929 5d0a 2020 2020 2020  c1, c2))].      
-00006400: 2020 7769 6e6e 6572 7320 3d20 6c69 7374    winners = list
-00006410: 2829 2020 200a 2020 2020 2020 2020 6966  ()   .        if
-00006420: 206c 656e 2877 5f65 6467 6573 2920 3e20   len(w_edges) > 
-00006430: 303a 2020 2020 2020 2020 2020 0a20 2020  0:          .   
-00006440: 2020 2020 2020 2020 2073 7472 656e 6774           strengt
-00006450: 6873 203d 2073 6f72 7465 6428 6c69 7374  hs = sorted(list
-00006460: 2873 6574 285b 655b 325d 2066 6f72 2065  (set([e[2] for e
-00006470: 2069 6e20 775f 6564 6765 735d 2929 2c20   in w_edges])), 
-00006480: 7265 7665 7273 653d 5472 7565 290a 2020  reverse=True).  
-00006490: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
-000064a0: 5f65 6467 6573 203d 205b 5b65 2066 6f72  _edges = [[e for
-000064b0: 2065 2069 6e20 775f 6564 6765 7320 6966   e in w_edges if
-000064c0: 2065 5b32 5d20 3d3d 2073 5d20 666f 7220   e[2] == s] for 
-000064d0: 7320 696e 2073 7472 656e 6774 6873 5d0a  s in strengths].
-000064e0: 2020 2020 2020 2020 2020 2020 7462 7320              tbs 
-000064f0: 3d20 7072 6f64 7563 7428 2a5b 7065 726d  = product(*[perm
-00006500: 7574 6174 696f 6e73 2865 6467 6573 2920  utations(edges) 
-00006510: 666f 7220 6564 6765 7320 696e 2073 6f72  for edges in sor
-00006520: 7465 645f 6564 6765 735d 290a 2020 2020  ted_edges]).    
-00006530: 2020 2020 2020 2020 666f 7220 7462 2069          for tb i
-00006540: 6e20 7462 733a 0a20 2020 2020 2020 2020  n tbs:.         
-00006550: 2020 2020 2020 2065 6467 6573 203d 2066         edges = f
-00006560: 6c61 7474 656e 2874 6229 0a20 2020 2020  latten(tb).     
-00006570: 2020 2020 2020 2020 2020 2072 705f 6465             rp_de
-00006580: 6665 6174 203d 2053 504f 286c 656e 2863  feat = SPO(len(c
-00006590: 616e 6469 6461 7465 7329 290a 2020 2020  andidates)).    
-000065a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000065b0: 6530 2c65 312c 7320 696e 2065 6467 6573  e0,e1,s in edges
-000065c0: 3a20 0a20 2020 2020 2020 2020 2020 2020  : .             
-000065d0: 2020 2020 2020 2069 6620 6e6f 7420 7270         if not rp
-000065e0: 5f64 6566 6561 742e 505b 6361 6e64 5f74  _defeat.P[cand_t
-000065f0: 6f5f 6369 6478 5b65 315d 5d5b 6361 6e64  o_cidx[e1]][cand
-00006600: 5f74 6f5f 6369 6478 5b65 305d 5d3a 0a20  _to_cidx[e0]]:. 
+00005610: 2020 2020 2073 7472 656e 6774 685b 6a5f       strength[j_
+00005620: 6964 785d 5b6b 5f69 6478 5d20 3d20 6d61  idx][k_idx] = ma
+00005630: 7828 7374 7265 6e67 7468 5b6a 5f69 6478  x(strength[j_idx
+00005640: 5d5b 6b5f 6964 785d 2c20 6d69 6e28 7374  ][k_idx], min(st
+00005650: 7265 6e67 7468 5b6a 5f69 6478 5d5b 695f  rength[j_idx][i_
+00005660: 6964 785d 2c73 7472 656e 6774 685b 695f  idx],strength[i_
+00005670: 6964 785d 5b6b 5f69 6478 5d29 290a 200a  idx][k_idx])). .
+00005680: 2020 2020 6465 6665 6174 5f67 7261 7068      defeat_graph
+00005690: 203d 206e 782e 4469 4772 6170 6828 290a   = nx.DiGraph().
+000056a0: 2020 2020 6465 6665 6174 5f67 7261 7068      defeat_graph
+000056b0: 2e61 6464 5f6e 6f64 6573 5f66 726f 6d28  .add_nodes_from(
+000056c0: 6361 6e64 6964 6174 6573 290a 0a20 2020  candidates)..   
+000056d0: 2066 6f72 2069 5f69 6478 2c20 6920 696e   for i_idx, i in
+000056e0: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
+000056f0: 6461 7465 7329 3a0a 2020 2020 2020 2020  dates):.        
+00005700: 666f 7220 6a5f 6964 782c 206a 2069 6e20  for j_idx, j in 
+00005710: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
+00005720: 6174 6573 293a 0a20 2020 2020 2020 2020  ates):.         
+00005730: 2020 2069 6620 6920 213d 206a 3a0a 2020     if i != j:.  
+00005740: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005750: 2073 5f6d 6174 7269 785b 6a5f 6964 785d   s_matrix[j_idx]
+00005760: 5b69 5f69 6478 5d20 3e20 7374 7265 6e67  [i_idx] > streng
+00005770: 7468 5b69 5f69 6478 5d5b 6a5f 6964 785d  th[i_idx][j_idx]
+00005780: 3a20 2320 7468 6520 6d61 696e 2064 6966  : # the main dif
+00005790: 6665 7265 6e63 6520 7769 7468 2042 6561  ference with Bea
+000057a0: 7420 5061 7468 0a20 2020 2020 2020 2020  t Path.         
+000057b0: 2020 2020 2020 2020 2020 2064 6566 6561             defea
+000057c0: 745f 6772 6170 682e 6164 645f 7765 6967  t_graph.add_weig
+000057d0: 6874 6564 5f65 6467 6573 5f66 726f 6d28  hted_edges_from(
+000057e0: 5b28 6a2c 692c 735f 6d61 7472 6978 5b6a  [(j,i,s_matrix[j
+000057f0: 5f69 6478 5d5b 695f 6964 785d 295d 290a  _idx][i_idx])]).
+00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005810: 0a20 2020 2072 6574 7572 6e20 6465 6665  .    return defe
+00005820: 6174 5f67 7261 7068 0a0a 0a0a 2320 666c  at_graph....# fl
+00005830: 6174 7465 6e20 6120 3264 206c 6973 7420  atten a 2d list 
+00005840: 2d20 7475 726e 2061 2032 6420 6c69 7374  - turn a 2d list
+00005850: 2069 6e74 6f20 6120 7369 6e67 6c65 206c   into a single l
+00005860: 6973 7420 6f66 2069 7465 6d73 0a66 6c61  ist of items.fla
+00005870: 7474 656e 203d 206c 616d 6264 6120 6c3a  tten = lambda l:
+00005880: 205b 6974 656d 2066 6f72 2073 7562 6c69   [item for subli
+00005890: 7374 2069 6e20 6c20 666f 7220 6974 656d  st in l for item
+000058a0: 2069 6e20 7375 626c 6973 745d 0a0a 6465   in sublist]..de
+000058b0: 6620 646f 6573 5f63 7265 6174 655f 6379  f does_create_cy
+000058c0: 636c 6528 672c 2065 6467 6529 3a0a 2020  cle(g, edge):.  
+000058d0: 2020 2727 2772 6574 7572 6e20 5472 7565    '''return True
+000058e0: 2069 6620 6164 6469 6e67 2074 6865 2065   if adding the e
+000058f0: 6467 6520 746f 2067 2063 7265 6174 6520  dge to g create 
+00005900: 6120 6379 636c 652e 0a20 2020 2069 7420  a cycle..    it 
+00005910: 6973 2061 7373 756d 6564 2074 6861 7420  is assumed that 
+00005920: 6564 6765 2069 7320 616c 7265 6164 7920  edge is already 
+00005930: 696e 2067 2727 270a 2020 2020 736f 7572  in g'''.    sour
+00005940: 6365 203d 2065 6467 655b 305d 0a20 2020  ce = edge[0].   
+00005950: 2074 6172 6765 7420 3d20 6564 6765 5b31   target = edge[1
+00005960: 5d0a 2020 2020 666f 7220 6e20 696e 2067  ].    for n in g
+00005970: 2e70 7265 6465 6365 7373 6f72 7328 736f  .predecessors(so
+00005980: 7572 6365 293a 0a20 2020 2020 2020 2069  urce):.        i
+00005990: 6620 6e78 2e68 6173 5f70 6174 6828 672c  f nx.has_path(g,
+000059a0: 2074 6172 6765 742c 206e 293a 200a 2020   target, n): .  
+000059b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000059c0: 2054 7275 650a 2020 2020 7265 7475 726e   True.    return
+000059d0: 2046 616c 7365 0a0a 4076 6d28 6e61 6d65   False..@vm(name
+000059e0: 3d22 5261 6e6b 6564 2050 6169 7273 2229  ="Ranked Pairs")
+000059f0: 0a64 6566 2072 616e 6b65 645f 7061 6972  .def ranked_pair
+00005a00: 7328 6564 6174 612c 2063 7572 725f 6361  s(edata, curr_ca
+00005a10: 6e64 7320 3d20 4e6f 6e65 2c20 7374 7265  nds = None, stre
+00005a20: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+00005a30: 4e6f 6e65 293a 2020 200a 2020 2020 2222  None):   .    ""
+00005a40: 220a 2020 2020 4f72 6465 7220 7468 6520  ".    Order the 
+00005a50: 6564 6765 7320 696e 2074 6865 206d 6172  edges in the mar
+00005a60: 6769 6e20 6772 6170 6820 6672 6f6d 206c  gin graph from l
+00005a70: 6172 6765 7374 2074 6f20 736d 616c 6c65  argest to smalle
+00005a80: 7374 2061 6e64 206c 6f63 6b20 7468 656d  st and lock them
+00005a90: 2069 6e20 696e 2074 6861 7420 6f72 6465   in in that orde
+00005aa0: 722c 2073 6b69 7070 696e 6720 6564 6765  r, skipping edge
+00005ab0: 7320 7468 6174 2063 7265 6174 6520 6120  s that create a 
+00005ac0: 6379 636c 652e 2020 4966 2074 6865 7265  cycle.  If there
+00005ad0: 2061 7265 2074 6965 7320 696e 2074 6865   are ties in the
+00005ae0: 206d 6172 6769 6e73 2c20 6272 6561 6b20   margins, break 
+00005af0: 7468 6520 7469 6573 2075 7369 6e67 2061  the ties using a
+00005b00: 2074 6965 2d62 7265 616b 696e 6720 7275   tie-breaking ru
+00005b10: 6c65 3a20 6120 6c69 6e65 6172 206f 7264  le: a linear ord
+00005b20: 6572 696e 6720 6f76 6572 2074 6865 2065  ering over the e
+00005b30: 6467 6573 2e20 2020 4120 6361 6e64 6964  dges.   A candid
+00005b40: 6174 6520 6973 2061 2052 616e 6b65 6420  ate is a Ranked 
+00005b50: 5061 6972 7320 7769 6e6e 6572 2069 6620  Pairs winner if 
+00005b60: 6974 2077 696e 7320 6163 636f 7264 696e  it wins accordin
+00005b70: 6720 746f 2073 6f6d 6520 7469 652d 6272  g to some tie-br
+00005b80: 6561 6b69 6e67 2072 756c 652e 2041 6c73  eaking rule. Als
+00005b90: 6f20 6b6e 6f77 6e20 6173 2054 6964 656d  o known as Tidem
+00005ba0: 616e 2773 2052 756c 652e 0a0a 2020 2020  an's Rule...    
+00005bb0: 2e2e 2077 6172 6e69 6e67 3a3a 200a 2020  .. warning:: .  
+00005bc0: 2020 2020 2020 5468 6973 206d 6574 686f        This metho
+00005bd0: 6420 6361 6e20 7461 6b65 2061 2076 6572  d can take a ver
+00005be0: 7920 6c6f 6e67 2074 696d 6520 746f 2066  y long time to f
+00005bf0: 696e 6420 7769 6e6e 6572 732e 200a 2020  ind winners. .  
+00005c00: 2020 2020 2020 0a20 2020 2041 7267 733a        .    Args:
+00005c10: 0a20 2020 2020 2020 2065 6461 7461 2028  .        edata (
+00005c20: 5072 6f66 696c 652c 2050 726f 6669 6c65  Profile, Profile
+00005c30: 5769 7468 5469 6573 2c20 4d61 7267 696e  WithTies, Margin
+00005c40: 4772 6170 6829 3a20 416e 7920 656c 6563  Graph): Any elec
+00005c50: 7469 6f6e 2064 6174 6120 7468 6174 2068  tion data that h
+00005c60: 6173 2061 2060 6d61 7267 696e 6020 6d65  as a `margin` me
+00005c70: 7468 6f64 2e20 0a20 2020 2020 2020 2063  thod. .        c
+00005c80: 7572 725f 6361 6e64 7320 284c 6973 745b  urr_cands (List[
+00005c90: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
+00005ca0: 2049 6620 7365 742c 2074 6865 6e20 6669   If set, then fi
+00005cb0: 6e64 2074 6865 2077 696e 6e65 7273 2066  nd the winners f
+00005cc0: 6f72 2074 6865 2070 726f 6669 6c65 2072  or the profile r
+00005cd0: 6573 7472 6963 7465 6420 746f 2074 6865  estricted to the
+00005ce0: 2063 616e 6469 6461 7465 7320 696e 2060   candidates in `
+00005cf0: 6063 7572 725f 6361 6e64 7360 600a 2020  `curr_cands``.  
+00005d00: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
+00005d10: 756e 6374 696f 6e20 2866 756e 6374 696f  unction (functio
+00005d20: 6e2c 206f 7074 696f 6e61 6c29 3a20 5468  n, optional): Th
+00005d30: 6520 7374 7265 6e67 7468 2066 756e 6374  e strength funct
+00005d40: 696f 6e20 746f 2062 6520 7573 6564 2074  ion to be used t
+00005d50: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
+00005d60: 7374 7265 6e67 7468 206f 6620 6120 7061  strength of a pa
+00005d70: 7468 2e20 2020 5468 6520 6465 6661 756c  th.   The defaul
+00005d80: 7420 6973 2074 6865 206d 6172 6769 6e20  t is the margin 
+00005d90: 6d65 7468 6f64 206f 6620 6060 6564 6174  method of ``edat
+00005da0: 6160 602e 2020 2054 6869 7320 6f6e 6c79  a``.   This only
+00005db0: 206d 6174 7465 7273 2077 6865 6e20 7468   matters when th
+00005dc0: 6520 6261 6c6c 6f74 7320 6172 6520 6e6f  e ballots are no
+00005dd0: 7420 6c69 6e65 6172 206f 7264 6572 732e  t linear orders.
+00005de0: 200a 0a20 2020 2052 6574 7572 6e73 3a20   ..    Returns: 
+00005df0: 0a20 2020 2020 2020 2041 2073 6f72 7465  .        A sorte
+00005e00: 6420 6c69 7374 206f 6620 6361 6e64 6964  d list of candid
+00005e10: 6174 6573 2e20 0a0a 2020 2020 2e2e 2073  ates. ..    .. s
+00005e20: 6565 616c 736f 3a3a 0a0a 2020 2020 2020  eealso::..      
+00005e30: 2020 3a6d 6574 683a 6070 7265 665f 766f    :meth:`pref_vo
+00005e40: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+00005e50: 645f 6d65 7468 6f64 732e 7261 6e6b 6564  d_methods.ranked
+00005e60: 5f70 6169 7273 5f77 6974 685f 7465 7374  _pairs_with_test
+00005e70: 602c 203a 6d65 7468 3a60 7072 6566 5f76  `, :meth:`pref_v
+00005e80: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
+00005e90: 6564 5f6d 6574 686f 6473 2e72 616e 6b65  ed_methods.ranke
+00005ea0: 645f 7061 6972 735f 7a74 602c 203a 6d65  d_pairs_zt`, :me
+00005eb0: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
+00005ec0: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+00005ed0: 686f 6473 2e72 616e 6b65 645f 7061 6972  hods.ranked_pair
+00005ee0: 735f 6465 6665 6174 7360 0a0a 2020 2020  s_defeats`..    
+00005ef0: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
+00005f00: 2e2e 2070 6c6f 743a 3a20 206d 6172 6769  .. plot::  margi
+00005f10: 6e5f 6772 6170 6873 5f65 7861 6d70 6c65  n_graphs_example
+00005f20: 732f 6d67 5f65 785f 6270 5f72 702e 7079  s/mg_ex_bp_rp.py
+00005f30: 0a20 2020 2020 2020 203a 636f 6e74 6578  .        :contex
+00005f40: 743a 2072 6573 6574 2020 0a20 2020 2020  t: reset  .     
+00005f50: 2020 203a 696e 636c 7564 652d 736f 7572     :include-sour
+00005f60: 6365 3a20 5472 7565 0a0a 0a20 2020 202e  ce: True...    .
+00005f70: 2e20 636f 6465 2d62 6c6f 636b 3a3a 200a  . code-block:: .
+00005f80: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
+00005f90: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+00005fa0: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
+00005fb0: 6d70 6f72 7420 7261 6e6b 6564 5f70 6169  mport ranked_pai
+00005fc0: 7273 0a0a 2020 2020 2020 2020 7261 6e6b  rs..        rank
+00005fd0: 6564 5f70 6169 7273 2e64 6973 706c 6179  ed_pairs.display
+00005fe0: 286d 6729 0a0a 0a20 2020 202e 2e20 6578  (mg)...    .. ex
+00005ff0: 6563 5f63 6f64 653a 3a20 0a20 2020 2020  ec_code:: .     
+00006000: 2020 203a 6869 6465 5f63 6f64 653a 0a0a     :hide_code:..
+00006010: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+00006020: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
+00006030: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
+00006040: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
+00006050: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
+00006060: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
+00006070: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+00006080: 6473 2069 6d70 6f72 7420 7261 6e6b 6564  ds import ranked
+00006090: 5f70 6169 7273 0a20 2020 2020 2020 200a  _pairs.        .
+000060a0: 2020 2020 2020 2020 6d67 203d 204d 6172          mg = Mar
+000060b0: 6769 6e47 7261 7068 285b 302c 2031 2c20  ginGraph([0, 1, 
+000060c0: 322c 2033 5d2c 205b 2830 2c20 322c 2033  2, 3], [(0, 2, 3
+000060d0: 292c 2028 312c 2030 2c20 3529 2c20 2832  ), (1, 0, 5), (2
+000060e0: 2c20 312c 2035 292c 2028 322c 2033 2c20  , 1, 5), (2, 3, 
+000060f0: 3129 2c20 2833 2c20 302c 2033 292c 2028  1), (3, 0, 3), (
+00006100: 332c 2031 2c20 3129 5d29 0a20 2020 2020  3, 1, 1)]).     
+00006110: 2020 200a 2020 2020 2020 2020 7261 6e6b     .        rank
+00006120: 6564 5f70 6169 7273 2e64 6973 706c 6179  ed_pairs.display
+00006130: 286d 6729 0a0a 2020 2020 2222 220a 2020  (mg)..    """.  
+00006140: 2020 6361 6e64 6964 6174 6573 203d 2065    candidates = e
+00006150: 6461 7461 2e63 616e 6469 6461 7465 7320  data.candidates 
+00006160: 6966 2063 7572 725f 6361 6e64 7320 6973  if curr_cands is
+00006170: 204e 6f6e 6520 656c 7365 2063 7572 725f   None else curr_
+00006180: 6361 6e64 7320 0a20 2020 2063 6964 785f  cands .    cidx_
+00006190: 746f 5f63 616e 6420 3d20 7b63 6964 783a  to_cand = {cidx:
+000061a0: 2063 2066 6f72 2063 6964 782c 2063 2069   c for cidx, c i
+000061b0: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
+000061c0: 6964 6174 6573 297d 2020 0a20 2020 2063  idates)}  .    c
+000061d0: 616e 645f 746f 5f63 6964 7820 3d20 7b63  and_to_cidx = {c
+000061e0: 3a20 6369 6478 2066 6f72 2063 6964 782c  : cidx for cidx,
+000061f0: 2063 2069 6e20 656e 756d 6572 6174 6528   c in enumerate(
+00006200: 6361 6e64 6964 6174 6573 297d 2020 0a20  candidates)}  . 
+00006210: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+00006220: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
+00006230: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
+00006240: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
+00006250: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
+00006260: 756e 6374 696f 6e20 2020 200a 0a20 2020  unction    ..   
+00006270: 2063 7720 3d20 6564 6174 612e 636f 6e64   cw = edata.cond
+00006280: 6f72 6365 745f 7769 6e6e 6572 2863 7572  orcet_winner(cur
+00006290: 725f 6361 6e64 733d 6375 7272 5f63 616e  r_cands=curr_can
+000062a0: 6473 290a 2020 2020 2320 5261 6e6b 6564  ds).    # Ranked
+000062b0: 2050 6169 7273 2069 7320 436f 6e64 6f72   Pairs is Condor
+000062c0: 6365 7420 636f 6e73 6973 7465 6e74 2c20  cet consistent, 
+000062d0: 736f 2073 696d 706c 7920 7265 7475 726e  so simply return
+000062e0: 2074 6865 2043 6f6e 646f 7263 6574 2077   the Condorcet w
+000062f0: 696e 6e65 7220 6966 2065 7869 7374 730a  inner if exists.
+00006300: 2020 2020 6966 2063 7720 6973 206e 6f74      if cw is not
+00006310: 204e 6f6e 653a 200a 2020 2020 2020 2020   None: .        
+00006320: 7769 6e6e 6572 7320 3d20 5b63 775d 0a20  winners = [cw]. 
+00006330: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00006340: 2077 5f65 6467 6573 203d 205b 2863 312c   w_edges = [(c1,
+00006350: 2063 322c 2073 7472 656e 6774 685f 6675   c2, strength_fu
+00006360: 6e63 7469 6f6e 2863 312c 2063 3229 2920  nction(c1, c2)) 
+00006370: 666f 7220 6331 2069 6e20 6361 6e64 6964  for c1 in candid
+00006380: 6174 6573 2066 6f72 2063 3220 696e 2063  ates for c2 in c
+00006390: 616e 6469 6461 7465 7320 0a20 2020 2020  andidates .     
+000063a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000063b0: 2063 3120 213d 2063 3220 616e 6420 2865   c1 != c2 and (e
+000063c0: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
+000063d0: 6566 6572 7328 6331 2c20 6332 2920 6f72  efers(c1, c2) or
+000063e0: 2065 6461 7461 2e69 735f 7469 6564 2863   edata.is_tied(c
+000063f0: 312c 2063 3229 295d 0a20 2020 2020 2020  1, c2))].       
+00006400: 2077 696e 6e65 7273 203d 206c 6973 7428   winners = list(
+00006410: 2920 2020 0a20 2020 2020 2020 2069 6620  )   .        if 
+00006420: 6c65 6e28 775f 6564 6765 7329 203e 2030  len(w_edges) > 0
+00006430: 3a20 2020 2020 2020 2020 200a 2020 2020  :          .    
+00006440: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+00006450: 7320 3d20 736f 7274 6564 286c 6973 7428  s = sorted(list(
+00006460: 7365 7428 5b65 5b32 5d20 666f 7220 6520  set([e[2] for e 
+00006470: 696e 2077 5f65 6467 6573 5d29 292c 2072  in w_edges])), r
+00006480: 6576 6572 7365 3d54 7275 6529 0a20 2020  everse=True).   
+00006490: 2020 2020 2020 2020 2073 6f72 7465 645f           sorted_
+000064a0: 6564 6765 7320 3d20 5b5b 6520 666f 7220  edges = [[e for 
+000064b0: 6520 696e 2077 5f65 6467 6573 2069 6620  e in w_edges if 
+000064c0: 655b 325d 203d 3d20 735d 2066 6f72 2073  e[2] == s] for s
+000064d0: 2069 6e20 7374 7265 6e67 7468 735d 0a20   in strengths]. 
+000064e0: 2020 2020 2020 2020 2020 2074 6273 203d             tbs =
+000064f0: 2070 726f 6475 6374 282a 5b70 6572 6d75   product(*[permu
+00006500: 7461 7469 6f6e 7328 6564 6765 7329 2066  tations(edges) f
+00006510: 6f72 2065 6467 6573 2069 6e20 736f 7274  or edges in sort
+00006520: 6564 5f65 6467 6573 5d29 0a20 2020 2020  ed_edges]).     
+00006530: 2020 2020 2020 2066 6f72 2074 6220 696e         for tb in
+00006540: 2074 6273 3a0a 2020 2020 2020 2020 2020   tbs:.          
+00006550: 2020 2020 2020 6564 6765 7320 3d20 666c        edges = fl
+00006560: 6174 7465 6e28 7462 290a 2020 2020 2020  atten(tb).      
+00006570: 2020 2020 2020 2020 2020 7270 5f64 6566            rp_def
+00006580: 6561 7420 3d20 5350 4f28 6c65 6e28 6361  eat = SPO(len(ca
+00006590: 6e64 6964 6174 6573 2929 0a20 2020 2020  ndidates)).     
+000065a0: 2020 2020 2020 2020 2020 2066 6f72 2065             for e
+000065b0: 302c 6531 2c73 2069 6e20 6564 6765 733a  0,e1,s in edges:
+000065c0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+000065d0: 2020 2020 2020 6966 206e 6f74 2072 705f        if not rp_
+000065e0: 6465 6665 6174 2e50 5b63 616e 645f 746f  defeat.P[cand_to
+000065f0: 5f63 6964 785b 6531 5d5d 5b63 616e 645f  _cidx[e1]][cand_
+00006600: 746f 5f63 6964 785b 6530 5d5d 3a0a 2020  to_cidx[e0]]:.  
 00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006620: 2020 2020 2020 2072 705f 6465 6665 6174         rp_defeat
-00006630: 2e61 6464 2863 616e 645f 746f 5f63 6964  .add(cand_to_cid
-00006640: 785b 6530 5d2c 6361 6e64 5f74 6f5f 6369  x[e0],cand_to_ci
-00006650: 6478 5b65 315d 290a 2020 2020 2020 2020  dx[e1]).        
-00006660: 2020 2020 2020 2020 7769 6e6e 6572 732e          winners.
-00006670: 6170 7065 6e64 2863 6964 785f 746f 5f63  append(cidx_to_c
-00006680: 616e 645b 7270 5f64 6566 6561 742e 696e  and[rp_defeat.in
-00006690: 6974 6961 6c5f 656c 656d 656e 7473 2829  itial_elements()
-000066a0: 5b30 5d5d 290a 2020 2020 2020 2020 656c  [0]]).        el
-000066b0: 7365 3a20 0a20 2020 2020 2020 2020 2020  se: .           
-000066c0: 2077 696e 6e65 7273 203d 2063 616e 6469   winners = candi
-000066d0: 6461 7465 730a 2020 2020 7265 7475 726e  dates.    return
-000066e0: 2073 6f72 7465 6428 6c69 7374 2873 6574   sorted(list(set
-000066f0: 2877 696e 6e65 7273 2929 290a 0a40 766d  (winners)))..@vm
-00006700: 286e 616d 653d 2252 616e 6b65 6420 5061  (name="Ranked Pa
-00006710: 6972 7322 290a 6465 6620 7261 6e6b 6564  irs").def ranked
-00006720: 5f70 6169 7273 5f77 6974 685f 7465 7374  _pairs_with_test
-00006730: 2865 6461 7461 2c20 6375 7272 5f63 616e  (edata, curr_can
-00006740: 6473 203d 204e 6f6e 652c 2073 7472 656e  ds = None, stren
-00006750: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
-00006760: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
-00006770: 4669 6e64 2074 6865 2052 616e 6b65 6420  Find the Ranked 
-00006780: 5061 6972 7320 7769 6e6e 6572 732c 2062  Pairs winners, b
-00006790: 7574 2069 6e63 6c75 6465 2061 2074 6573  ut include a tes
-000067a0: 7420 746f 2064 6574 6572 6d69 6e65 6420  t to determined 
-000067b0: 6966 2069 7420 7769 6c6c 2074 616b 6520  if it will take 
-000067c0: 746f 6f20 6c6f 6e67 2074 6f20 636f 6d70  too long to comp
-000067d0: 7574 6520 7468 6520 5261 6e6b 6564 2050  ute the Ranked P
-000067e0: 6169 7273 2077 696e 6e65 7273 2e20 4966  airs winners. If
-000067f0: 2074 6865 2063 616c 6375 6c61 7469 6f6e   the calculation
-00006800: 206f 6620 7468 6520 7769 6e6e 6572 7320   of the winners 
-00006810: 7769 6c6c 2074 616b 6520 746f 6f20 6c6f  will take too lo
-00006820: 6e67 2c20 7265 7475 726e 204e 6f6e 652e  ng, return None.
-00006830: 0a0a 2020 2020 2e2e 2069 6d70 6f72 7461  ..    .. importa
-00006840: 6e74 3a3a 0a20 2020 2020 2020 2054 6869  nt::.        Thi
-00006850: 7320 766f 7469 6e67 206d 6574 686f 6420  s voting method 
-00006860: 7468 6174 206d 6967 6874 2072 6574 7572  that might retur
-00006870: 6e20 4e6f 6e65 2072 6174 6865 7220 7468  n None rather th
-00006880: 616e 2061 206c 6973 7420 6f66 2063 616e  an a list of can
-00006890: 6469 6461 7465 732e 2020 0a0a 2020 2020  didates.  ..    
-000068a0: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-000068b0: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-000068c0: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-000068d0: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-000068e0: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-000068f0: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-00006900: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
-00006910: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
-00006920: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
-00006930: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
-00006940: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
-00006950: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
-00006960: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
-00006970: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
-00006980: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
-00006990: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
-000069a0: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
-000069b0: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
-000069c0: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
-000069d0: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
-000069e0: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
-000069f0: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
-00006a00: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
-00006a10: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
-00006a20: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
-00006a30: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
-00006a40: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
-00006a50: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
-00006a60: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
-00006a70: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
-00006a80: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
-00006a90: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
-00006aa0: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
-00006ab0: 202e 2e20 7365 6561 6c73 6f3a 3a0a 0a20   .. seealso::.. 
-00006ac0: 2020 2020 2020 203a 6d65 7468 3a60 7072         :meth:`pr
-00006ad0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-00006ae0: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
-00006af0: 616e 6b65 645f 7061 6972 735f 7769 7468  anked_pairs_with
-00006b00: 5f74 6573 7460 2c20 3a6d 6574 683a 6070  _test`, :meth:`p
-00006b10: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-00006b20: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-00006b30: 7261 6e6b 6564 5f70 6169 7273 5f7a 7460  ranked_pairs_zt`
-00006b40: 2c20 3a6d 6574 683a 6070 7265 665f 766f  , :meth:`pref_vo
-00006b50: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
-00006b60: 645f 6d65 7468 6f64 732e 7261 6e6b 6564  d_methods.ranked
-00006b70: 5f70 6169 7273 5f64 6566 6561 7473 600a  _pairs_defeats`.
-00006b80: 0a20 2020 203a 4578 616d 706c 653a 200a  .    :Example: .
-00006b90: 0a20 2020 202e 2e20 706c 6f74 3a3a 2020  .    .. plot::  
-00006ba0: 6d61 7267 696e 5f67 7261 7068 735f 6578  margin_graphs_ex
-00006bb0: 616d 706c 6573 2f6d 675f 6578 5f72 705f  amples/mg_ex_rp_
-00006bc0: 7769 7468 5f74 6573 742e 7079 0a20 2020  with_test.py.   
-00006bd0: 2020 2020 203a 636f 6e74 6578 743a 2072       :context: r
-00006be0: 6573 6574 2020 0a20 2020 2020 2020 203a  eset  .        :
-00006bf0: 696e 636c 7564 652d 736f 7572 6365 3a20  include-source: 
-00006c00: 5472 7565 0a0a 0a20 2020 202e 2e20 636f  True...    .. co
-00006c10: 6465 2d62 6c6f 636b 3a3a 200a 0a20 2020  de-block:: ..   
-00006c20: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-00006c30: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-00006c40: 6564 5f6d 6574 686f 6473 2069 6d70 6f72  ed_methods impor
-00006c50: 7420 7261 6e6b 6564 5f70 6169 7273 5f77  t ranked_pairs_w
-00006c60: 6974 685f 7465 7374 0a0a 2020 2020 2020  ith_test..      
-00006c70: 2020 7261 6e6b 6564 5f70 6169 7273 5f77    ranked_pairs_w
-00006c80: 6974 685f 7465 7374 2e64 6973 706c 6179  ith_test.display
-00006c90: 286d 6729 0a0a 0a20 2020 202e 2e20 6578  (mg)...    .. ex
-00006ca0: 6563 5f63 6f64 653a 3a20 0a20 2020 2020  ec_code:: .     
-00006cb0: 2020 203a 6869 6465 5f63 6f64 653a 0a0a     :hide_code:..
-00006cc0: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-00006cd0: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
-00006ce0: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
-00006cf0: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
-00006d00: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
-00006d10: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
-00006d20: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-00006d30: 6473 2069 6d70 6f72 7420 7261 6e6b 6564  ds import ranked
-00006d40: 5f70 6169 7273 5f77 6974 685f 7465 7374  _pairs_with_test
-00006d50: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006d60: 2020 6d67 203d 204d 6172 6769 6e47 7261    mg = MarginGra
-00006d70: 7068 285b 302c 2031 2c20 322c 2033 5d2c  ph([0, 1, 2, 3],
-00006d80: 205b 2831 2c20 322c 2032 292c 2028 312c   [(1, 2, 2), (1,
-00006d90: 2033 2c20 3229 2c20 2832 2c20 302c 2032   3, 2), (2, 0, 2
-00006da0: 295d 290a 2020 2020 2020 2020 0a20 2020  )]).        .   
-00006db0: 2020 2020 2072 616e 6b65 645f 7061 6972       ranked_pair
-00006dc0: 735f 7769 7468 5f74 6573 742e 6469 7370  s_with_test.disp
-00006dd0: 6c61 7928 6d67 290a 0a0a 2020 2020 2222  lay(mg)...    ""
-00006de0: 2220 2020 200a 2020 2020 6361 6e64 6964  "    .    candid
-00006df0: 6174 6573 203d 2065 6461 7461 2e63 616e  ates = edata.can
-00006e00: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
-00006e10: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
-00006e20: 7365 2063 7572 725f 6361 6e64 7320 2020  se curr_cands   
-00006e30: 200a 2020 2020 6369 6478 5f74 6f5f 6361   .    cidx_to_ca
-00006e40: 6e64 203d 207b 6369 6478 3a20 6320 666f  nd = {cidx: c fo
-00006e50: 7220 6369 6478 2c20 6320 696e 2065 6e75  r cidx, c in enu
-00006e60: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
-00006e70: 7329 7d20 200a 2020 2020 6361 6e64 5f74  s)}  .    cand_t
-00006e80: 6f5f 6369 6478 203d 207b 633a 2063 6964  o_cidx = {c: cid
-00006e90: 7820 666f 7220 6369 6478 2c20 6320 696e  x for cidx, c in
-00006ea0: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
-00006eb0: 6461 7465 7329 7d20 200a 2020 2020 0a20  dates)}  .    . 
-00006ec0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-00006ed0: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
-00006ee0: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
-00006ef0: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
-00006f00: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
-00006f10: 756e 6374 696f 6e20 2020 0a0a 2020 2020  unction   ..    
-00006f20: 6377 203d 2065 6461 7461 2e63 6f6e 646f  cw = edata.condo
-00006f30: 7263 6574 5f77 696e 6e65 7228 6375 7272  rcet_winner(curr
-00006f40: 5f63 616e 6473 203d 2063 7572 725f 6361  _cands = curr_ca
-00006f50: 6e64 7329 0a20 2020 2023 2052 616e 6b65  nds).    # Ranke
-00006f60: 6420 5061 6972 7320 6973 2043 6f6e 646f  d Pairs is Condo
-00006f70: 7263 6574 2063 6f6e 7369 7374 656e 742c  rcet consistent,
-00006f80: 2073 6f20 7369 6d70 6c79 2072 6574 7572   so simply retur
-00006f90: 6e20 7468 6520 436f 6e64 6f72 6365 7420  n the Condorcet 
-00006fa0: 7769 6e6e 6572 2069 6620 6578 6973 7473  winner if exists
-00006fb0: 0a20 2020 2069 6620 6377 2069 7320 6e6f  .    if cw is no
-00006fc0: 7420 4e6f 6e65 3a20 0a20 2020 2020 2020  t None: .       
-00006fd0: 2077 696e 6e65 7273 203d 205b 6377 5d0a   winners = [cw].
-00006fe0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00006ff0: 2020 775f 6564 6765 7320 3d20 5b28 6331    w_edges = [(c1
-00007000: 2c20 6332 2c20 7374 7265 6e67 7468 5f66  , c2, strength_f
-00007010: 756e 6374 696f 6e28 6331 2c20 6332 2929  unction(c1, c2))
-00007020: 2066 6f72 2063 3120 696e 2063 616e 6469   for c1 in candi
-00007030: 6461 7465 7320 666f 7220 6332 2069 6e20  dates for c2 in 
-00007040: 6361 6e64 6964 6174 6573 200a 2020 2020  candidates .    
-00007050: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00007060: 6620 6331 2021 3d20 6332 2061 6e64 2028  f c1 != c2 and (
-00007070: 6564 6174 612e 6d61 6a6f 7269 7479 5f70  edata.majority_p
-00007080: 7265 6665 7273 2863 312c 2063 3229 206f  refers(c1, c2) o
-00007090: 7220 6564 6174 612e 6973 5f74 6965 6428  r edata.is_tied(
-000070a0: 6331 2c20 6332 2929 5d0a 2020 2020 2020  c1, c2))].      
-000070b0: 2020 7769 6e6e 6572 7320 3d20 6c69 7374    winners = list
-000070c0: 2829 2020 2020 2020 2020 2020 2020 0a20  ()            . 
-000070d0: 2020 2020 2020 2073 7472 656e 6774 6873         strengths
-000070e0: 203d 2073 6f72 7465 6428 6c69 7374 2873   = sorted(list(s
-000070f0: 6574 285b 655b 325d 2066 6f72 2065 2069  et([e[2] for e i
-00007100: 6e20 775f 6564 6765 735d 2929 2c20 7265  n w_edges])), re
-00007110: 7665 7273 653d 5472 7565 290a 2020 2020  verse=True).    
-00007120: 2020 2020 736f 7274 6564 5f65 6467 6573      sorted_edges
-00007130: 203d 205b 5b65 2066 6f72 2065 2069 6e20   = [[e for e in 
-00007140: 775f 6564 6765 7320 6966 2065 5b32 5d20  w_edges if e[2] 
-00007150: 3d3d 2073 5d20 666f 7220 7320 696e 2073  == s] for s in s
-00007160: 7472 656e 6774 6873 5d0a 2020 2020 2020  trengths].      
-00007170: 2020 6966 206e 702e 7072 6f64 285b 6d61    if np.prod([ma
-00007180: 7468 2e66 6163 746f 7269 616c 286c 656e  th.factorial(len
-00007190: 2865 7329 2920 666f 7220 6573 2069 6e20  (es)) for es in 
-000071a0: 736f 7274 6564 5f65 6467 6573 5d29 203e  sorted_edges]) >
-000071b0: 2033 3030 303a 200a 2020 2020 2020 2020   3000: .        
-000071c0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-000071d0: 2020 2020 2020 2020 656c 7365 3a20 0a20          else: . 
-000071e0: 2020 2020 2020 2020 2020 2074 6273 203d             tbs =
-000071f0: 2070 726f 6475 6374 282a 5b70 6572 6d75   product(*[permu
-00007200: 7461 7469 6f6e 7328 6564 6765 7329 2066  tations(edges) f
-00007210: 6f72 2065 6467 6573 2069 6e20 736f 7274  or edges in sort
-00007220: 6564 5f65 6467 6573 5d29 0a20 2020 2020  ed_edges]).     
-00007230: 2020 2020 2020 2066 6f72 2074 6220 696e         for tb in
-00007240: 2074 6273 3a0a 2020 2020 2020 2020 2020   tbs:.          
-00007250: 2020 2020 2020 6564 6765 7320 3d20 666c        edges = fl
-00007260: 6174 7465 6e28 7462 290a 2020 2020 2020  atten(tb).      
-00007270: 2020 2020 2020 2020 2020 7270 5f64 6566            rp_def
-00007280: 6561 7420 3d20 5350 4f28 6c65 6e28 6361  eat = SPO(len(ca
-00007290: 6e64 6964 6174 6573 2929 0a20 2020 2020  ndidates)).     
-000072a0: 2020 2020 2020 2020 2020 2066 6f72 2065             for e
-000072b0: 302c 6531 2c73 2069 6e20 6564 6765 733a  0,e1,s in edges:
-000072c0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-000072d0: 2020 2020 2020 6966 206e 6f74 2072 705f        if not rp_
-000072e0: 6465 6665 6174 2e50 5b63 616e 645f 746f  defeat.P[cand_to
-000072f0: 5f63 6964 785b 6531 5d5d 5b63 616e 645f  _cidx[e1]][cand_
-00007300: 746f 5f63 6964 785b 6530 5d5d 3a0a 2020  to_cidx[e0]]:.  
+00006620: 2020 2020 2020 7270 5f64 6566 6561 742e        rp_defeat.
+00006630: 6164 6428 6361 6e64 5f74 6f5f 6369 6478  add(cand_to_cidx
+00006640: 5b65 305d 2c63 616e 645f 746f 5f63 6964  [e0],cand_to_cid
+00006650: 785b 6531 5d29 0a20 2020 2020 2020 2020  x[e1]).         
+00006660: 2020 2020 2020 2077 696e 6e65 7273 2e61         winners.a
+00006670: 7070 656e 6428 6369 6478 5f74 6f5f 6361  ppend(cidx_to_ca
+00006680: 6e64 5b72 705f 6465 6665 6174 2e69 6e69  nd[rp_defeat.ini
+00006690: 7469 616c 5f65 6c65 6d65 6e74 7328 295b  tial_elements()[
+000066a0: 305d 5d29 0a20 2020 2020 2020 2065 6c73  0]]).        els
+000066b0: 653a 200a 2020 2020 2020 2020 2020 2020  e: .            
+000066c0: 7769 6e6e 6572 7320 3d20 6361 6e64 6964  winners = candid
+000066d0: 6174 6573 0a20 2020 2072 6574 7572 6e20  ates.    return 
+000066e0: 736f 7274 6564 286c 6973 7428 7365 7428  sorted(list(set(
+000066f0: 7769 6e6e 6572 7329 2929 0a0a 4076 6d28  winners)))..@vm(
+00006700: 6e61 6d65 3d22 5261 6e6b 6564 2050 6169  name="Ranked Pai
+00006710: 7273 2229 0a64 6566 2072 616e 6b65 645f  rs").def ranked_
+00006720: 7061 6972 735f 7769 7468 5f74 6573 7428  pairs_with_test(
+00006730: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
+00006740: 7320 3d20 4e6f 6e65 2c20 7374 7265 6e67  s = None, streng
+00006750: 7468 5f66 756e 6374 696f 6e20 3d20 4e6f  th_function = No
+00006760: 6e65 293a 2020 200a 2020 2020 2222 2246  ne):   .    """F
+00006770: 696e 6420 7468 6520 5261 6e6b 6564 2050  ind the Ranked P
+00006780: 6169 7273 2077 696e 6e65 7273 2c20 6275  airs winners, bu
+00006790: 7420 696e 636c 7564 6520 6120 7465 7374  t include a test
+000067a0: 2074 6f20 6465 7465 726d 696e 6564 2069   to determined i
+000067b0: 6620 6974 2077 696c 6c20 7461 6b65 2074  f it will take t
+000067c0: 6f6f 206c 6f6e 6720 746f 2063 6f6d 7075  oo long to compu
+000067d0: 7465 2074 6865 2052 616e 6b65 6420 5061  te the Ranked Pa
+000067e0: 6972 7320 7769 6e6e 6572 732e 2049 6620  irs winners. If 
+000067f0: 7468 6520 6361 6c63 756c 6174 696f 6e20  the calculation 
+00006800: 6f66 2074 6865 2077 696e 6e65 7273 2077  of the winners w
+00006810: 696c 6c20 7461 6b65 2074 6f6f 206c 6f6e  ill take too lon
+00006820: 672c 2072 6574 7572 6e20 4e6f 6e65 2e0a  g, return None..
+00006830: 0a20 2020 202e 2e20 696d 706f 7274 616e  .    .. importan
+00006840: 743a 3a0a 2020 2020 2020 2020 5468 6973  t::.        This
+00006850: 2076 6f74 696e 6720 6d65 7468 6f64 2074   voting method t
+00006860: 6861 7420 6d69 6768 7420 7265 7475 726e  hat might return
+00006870: 204e 6f6e 6520 7261 7468 6572 2074 6861   None rather tha
+00006880: 6e20 6120 6c69 7374 206f 6620 6361 6e64  n a list of cand
+00006890: 6964 6174 6573 2e20 200a 0a20 2020 2041  idates.  ..    A
+000068a0: 7267 733a 0a20 2020 2020 2020 2065 6461  rgs:.        eda
+000068b0: 7461 2028 5072 6f66 696c 652c 2050 726f  ta (Profile, Pro
+000068c0: 6669 6c65 5769 7468 5469 6573 2c20 4d61  fileWithTies, Ma
+000068d0: 7267 696e 4772 6170 6829 3a20 416e 7920  rginGraph): Any 
+000068e0: 656c 6563 7469 6f6e 2064 6174 6120 7468  election data th
+000068f0: 6174 2068 6173 2061 2060 6d61 7267 696e  at has a `margin
+00006900: 6020 6d65 7468 6f64 2e20 0a20 2020 2020  ` method. .     
+00006910: 2020 2063 7572 725f 6361 6e64 7320 284c     curr_cands (L
+00006920: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
+00006930: 616c 293a 2049 6620 7365 742c 2074 6865  al): If set, the
+00006940: 6e20 6669 6e64 2074 6865 2077 696e 6e65  n find the winne
+00006950: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
+00006960: 6c65 2072 6573 7472 6963 7465 6420 746f  le restricted to
+00006970: 2074 6865 2063 616e 6469 6461 7465 7320   the candidates 
+00006980: 696e 2060 6063 7572 725f 6361 6e64 7360  in ``curr_cands`
+00006990: 600a 2020 2020 2020 2020 7374 7265 6e67  `.        streng
+000069a0: 7468 5f66 756e 6374 696f 6e20 2866 756e  th_function (fun
+000069b0: 6374 696f 6e2c 206f 7074 696f 6e61 6c29  ction, optional)
+000069c0: 3a20 5468 6520 7374 7265 6e67 7468 2066  : The strength f
+000069d0: 756e 6374 696f 6e20 746f 2062 6520 7573  unction to be us
+000069e0: 6564 2074 6f20 6361 6c63 756c 6174 6520  ed to calculate 
+000069f0: 7468 6520 7374 7265 6e67 7468 206f 6620  the strength of 
+00006a00: 6120 7061 7468 2e20 2020 5468 6520 6465  a path.   The de
+00006a10: 6661 756c 7420 6973 2074 6865 206d 6172  fault is the mar
+00006a20: 6769 6e20 6d65 7468 6f64 206f 6620 6060  gin method of ``
+00006a30: 6564 6174 6160 602e 2020 2054 6869 7320  edata``.   This 
+00006a40: 6f6e 6c79 206d 6174 7465 7273 2077 6865  only matters whe
+00006a50: 6e20 7468 6520 6261 6c6c 6f74 7320 6172  n the ballots ar
+00006a60: 6520 6e6f 7420 6c69 6e65 6172 206f 7264  e not linear ord
+00006a70: 6572 732e 200a 0a20 2020 2052 6574 7572  ers. ..    Retur
+00006a80: 6e73 3a20 0a20 2020 2020 2020 2041 2073  ns: .        A s
+00006a90: 6f72 7465 6420 6c69 7374 206f 6620 6361  orted list of ca
+00006aa0: 6e64 6964 6174 6573 2e20 0a0a 2020 2020  ndidates. ..    
+00006ab0: 2e2e 2073 6565 616c 736f 3a3a 0a0a 2020  .. seealso::..  
+00006ac0: 2020 2020 2020 3a6d 6574 683a 6070 7265        :meth:`pre
+00006ad0: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+00006ae0: 6261 7365 645f 6d65 7468 6f64 732e 7261  based_methods.ra
+00006af0: 6e6b 6564 5f70 6169 7273 5f77 6974 685f  nked_pairs_with_
+00006b00: 7465 7374 602c 203a 6d65 7468 3a60 7072  test`, :meth:`pr
+00006b10: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+00006b20: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
+00006b30: 616e 6b65 645f 7061 6972 735f 7a74 602c  anked_pairs_zt`,
+00006b40: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
+00006b50: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
+00006b60: 5f6d 6574 686f 6473 2e72 616e 6b65 645f  _methods.ranked_
+00006b70: 7061 6972 735f 6465 6665 6174 7360 0a0a  pairs_defeats`..
+00006b80: 2020 2020 3a45 7861 6d70 6c65 3a20 0a0a      :Example: ..
+00006b90: 2020 2020 2e2e 2070 6c6f 743a 3a20 206d      .. plot::  m
+00006ba0: 6172 6769 6e5f 6772 6170 6873 5f65 7861  argin_graphs_exa
+00006bb0: 6d70 6c65 732f 6d67 5f65 785f 7270 5f77  mples/mg_ex_rp_w
+00006bc0: 6974 685f 7465 7374 2e70 790a 2020 2020  ith_test.py.    
+00006bd0: 2020 2020 3a63 6f6e 7465 7874 3a20 7265      :context: re
+00006be0: 7365 7420 200a 2020 2020 2020 2020 3a69  set  .        :i
+00006bf0: 6e63 6c75 6465 2d73 6f75 7263 653a 2054  nclude-source: T
+00006c00: 7275 650a 0a0a 2020 2020 2e2e 2063 6f64  rue...    .. cod
+00006c10: 652d 626c 6f63 6b3a 3a20 0a0a 2020 2020  e-block:: ..    
+00006c20: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
+00006c30: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+00006c40: 645f 6d65 7468 6f64 7320 696d 706f 7274  d_methods import
+00006c50: 2072 616e 6b65 645f 7061 6972 735f 7769   ranked_pairs_wi
+00006c60: 7468 5f74 6573 740a 0a20 2020 2020 2020  th_test..       
+00006c70: 2072 616e 6b65 645f 7061 6972 735f 7769   ranked_pairs_wi
+00006c80: 7468 5f74 6573 742e 6469 7370 6c61 7928  th_test.display(
+00006c90: 6d67 290a 0a0a 2020 2020 2e2e 2065 7865  mg)...    .. exe
+00006ca0: 635f 636f 6465 3a3a 200a 2020 2020 2020  c_code:: .      
+00006cb0: 2020 3a68 6964 655f 636f 6465 3a0a 0a20    :hide_code:.. 
+00006cc0: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
+00006cd0: 5f76 6f74 696e 672e 7765 6967 6874 6564  _voting.weighted
+00006ce0: 5f6d 616a 6f72 6974 795f 6772 6170 6873  _majority_graphs
+00006cf0: 2069 6d70 6f72 7420 4d61 7267 696e 4772   import MarginGr
+00006d00: 6170 680a 2020 2020 2020 2020 6672 6f6d  aph.        from
+00006d10: 2070 7265 665f 766f 7469 6e67 2e6d 6172   pref_voting.mar
+00006d20: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+00006d30: 7320 696d 706f 7274 2072 616e 6b65 645f  s import ranked_
+00006d40: 7061 6972 735f 7769 7468 5f74 6573 740a  pairs_with_test.
+00006d50: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00006d60: 206d 6720 3d20 4d61 7267 696e 4772 6170   mg = MarginGrap
+00006d70: 6828 5b30 2c20 312c 2032 2c20 335d 2c20  h([0, 1, 2, 3], 
+00006d80: 5b28 312c 2032 2c20 3229 2c20 2831 2c20  [(1, 2, 2), (1, 
+00006d90: 332c 2032 292c 2028 322c 2030 2c20 3229  3, 2), (2, 0, 2)
+00006da0: 5d29 0a20 2020 2020 2020 200a 2020 2020  ]).        .    
+00006db0: 2020 2020 7261 6e6b 6564 5f70 6169 7273      ranked_pairs
+00006dc0: 5f77 6974 685f 7465 7374 2e64 6973 706c  _with_test.displ
+00006dd0: 6179 286d 6729 0a0a 0a20 2020 2022 2222  ay(mg)...    """
+00006de0: 2020 2020 0a20 2020 2063 616e 6469 6461      .    candida
+00006df0: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
+00006e00: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
+00006e10: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
+00006e20: 6520 6375 7272 5f63 616e 6473 2020 2020  e curr_cands    
+00006e30: 0a20 2020 2063 6964 785f 746f 5f63 616e  .    cidx_to_can
+00006e40: 6420 3d20 7b63 6964 783a 2063 2066 6f72  d = {cidx: c for
+00006e50: 2063 6964 782c 2063 2069 6e20 656e 756d   cidx, c in enum
+00006e60: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
+00006e70: 297d 2020 0a20 2020 2063 616e 645f 746f  )}  .    cand_to
+00006e80: 5f63 6964 7820 3d20 7b63 3a20 6369 6478  _cidx = {c: cidx
+00006e90: 2066 6f72 2063 6964 782c 2063 2069 6e20   for cidx, c in 
+00006ea0: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
+00006eb0: 6174 6573 297d 2020 0a20 2020 200a 2020  ates)}  .    .  
+00006ec0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+00006ed0: 696f 6e20 3d20 6564 6174 612e 6d61 7267  ion = edata.marg
+00006ee0: 696e 2069 6620 7374 7265 6e67 7468 5f66  in if strength_f
+00006ef0: 756e 6374 696f 6e20 6973 204e 6f6e 6520  unction is None 
+00006f00: 656c 7365 2073 7472 656e 6774 685f 6675  else strength_fu
+00006f10: 6e63 7469 6f6e 2020 200a 0a20 2020 2063  nction   ..    c
+00006f20: 7720 3d20 6564 6174 612e 636f 6e64 6f72  w = edata.condor
+00006f30: 6365 745f 7769 6e6e 6572 2863 7572 725f  cet_winner(curr_
+00006f40: 6361 6e64 7320 3d20 6375 7272 5f63 616e  cands = curr_can
+00006f50: 6473 290a 2020 2020 2320 5261 6e6b 6564  ds).    # Ranked
+00006f60: 2050 6169 7273 2069 7320 436f 6e64 6f72   Pairs is Condor
+00006f70: 6365 7420 636f 6e73 6973 7465 6e74 2c20  cet consistent, 
+00006f80: 736f 2073 696d 706c 7920 7265 7475 726e  so simply return
+00006f90: 2074 6865 2043 6f6e 646f 7263 6574 2077   the Condorcet w
+00006fa0: 696e 6e65 7220 6966 2065 7869 7374 730a  inner if exists.
+00006fb0: 2020 2020 6966 2063 7720 6973 206e 6f74      if cw is not
+00006fc0: 204e 6f6e 653a 200a 2020 2020 2020 2020   None: .        
+00006fd0: 7769 6e6e 6572 7320 3d20 5b63 775d 0a20  winners = [cw]. 
+00006fe0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00006ff0: 2077 5f65 6467 6573 203d 205b 2863 312c   w_edges = [(c1,
+00007000: 2063 322c 2073 7472 656e 6774 685f 6675   c2, strength_fu
+00007010: 6e63 7469 6f6e 2863 312c 2063 3229 2920  nction(c1, c2)) 
+00007020: 666f 7220 6331 2069 6e20 6361 6e64 6964  for c1 in candid
+00007030: 6174 6573 2066 6f72 2063 3220 696e 2063  ates for c2 in c
+00007040: 616e 6469 6461 7465 7320 0a20 2020 2020  andidates .     
+00007050: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00007060: 2063 3120 213d 2063 3220 616e 6420 2865   c1 != c2 and (e
+00007070: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
+00007080: 6566 6572 7328 6331 2c20 6332 2920 6f72  efers(c1, c2) or
+00007090: 2065 6461 7461 2e69 735f 7469 6564 2863   edata.is_tied(c
+000070a0: 312c 2063 3229 295d 0a20 2020 2020 2020  1, c2))].       
+000070b0: 2077 696e 6e65 7273 203d 206c 6973 7428   winners = list(
+000070c0: 2920 2020 2020 2020 2020 2020 200a 2020  )            .  
+000070d0: 2020 2020 2020 7374 7265 6e67 7468 7320        strengths 
+000070e0: 3d20 736f 7274 6564 286c 6973 7428 7365  = sorted(list(se
+000070f0: 7428 5b65 5b32 5d20 666f 7220 6520 696e  t([e[2] for e in
+00007100: 2077 5f65 6467 6573 5d29 292c 2072 6576   w_edges])), rev
+00007110: 6572 7365 3d54 7275 6529 0a20 2020 2020  erse=True).     
+00007120: 2020 2073 6f72 7465 645f 6564 6765 7320     sorted_edges 
+00007130: 3d20 5b5b 6520 666f 7220 6520 696e 2077  = [[e for e in w
+00007140: 5f65 6467 6573 2069 6620 655b 325d 203d  _edges if e[2] =
+00007150: 3d20 735d 2066 6f72 2073 2069 6e20 7374  = s] for s in st
+00007160: 7265 6e67 7468 735d 0a20 2020 2020 2020  rengths].       
+00007170: 2069 6620 6e70 2e70 726f 6428 5b6d 6174   if np.prod([mat
+00007180: 682e 6661 6374 6f72 6961 6c28 6c65 6e28  h.factorial(len(
+00007190: 6573 2929 2066 6f72 2065 7320 696e 2073  es)) for es in s
+000071a0: 6f72 7465 645f 6564 6765 735d 2920 3e20  orted_edges]) > 
+000071b0: 3330 3030 3a20 0a20 2020 2020 2020 2020  3000: .         
+000071c0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+000071d0: 2020 2020 2020 2065 6c73 653a 200a 2020         else: .  
+000071e0: 2020 2020 2020 2020 2020 7462 7320 3d20            tbs = 
+000071f0: 7072 6f64 7563 7428 2a5b 7065 726d 7574  product(*[permut
+00007200: 6174 696f 6e73 2865 6467 6573 2920 666f  ations(edges) fo
+00007210: 7220 6564 6765 7320 696e 2073 6f72 7465  r edges in sorte
+00007220: 645f 6564 6765 735d 290a 2020 2020 2020  d_edges]).      
+00007230: 2020 2020 2020 666f 7220 7462 2069 6e20        for tb in 
+00007240: 7462 733a 0a20 2020 2020 2020 2020 2020  tbs:.           
+00007250: 2020 2020 2065 6467 6573 203d 2066 6c61       edges = fla
+00007260: 7474 656e 2874 6229 0a20 2020 2020 2020  tten(tb).       
+00007270: 2020 2020 2020 2020 2072 705f 6465 6665           rp_defe
+00007280: 6174 203d 2053 504f 286c 656e 2863 616e  at = SPO(len(can
+00007290: 6469 6461 7465 7329 290a 2020 2020 2020  didates)).      
+000072a0: 2020 2020 2020 2020 2020 666f 7220 6530            for e0
+000072b0: 2c65 312c 7320 696e 2065 6467 6573 3a20  ,e1,s in edges: 
+000072c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000072d0: 2020 2020 2069 6620 6e6f 7420 7270 5f64       if not rp_d
+000072e0: 6566 6561 742e 505b 6361 6e64 5f74 6f5f  efeat.P[cand_to_
+000072f0: 6369 6478 5b65 315d 5d5b 6361 6e64 5f74  cidx[e1]][cand_t
+00007300: 6f5f 6369 6478 5b65 305d 5d3a 0a20 2020  o_cidx[e0]]:.   
 00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007320: 2020 2020 2020 7270 5f64 6566 6561 742e        rp_defeat.
-00007330: 6164 6428 6361 6e64 5f74 6f5f 6369 6478  add(cand_to_cidx
-00007340: 5b65 305d 2c63 616e 645f 746f 5f63 6964  [e0],cand_to_cid
-00007350: 785b 6531 5d29 0a20 2020 2020 2020 2020  x[e1]).         
-00007360: 2020 2020 2020 2077 696e 6e65 7273 2e61         winners.a
-00007370: 7070 656e 6428 6369 6478 5f74 6f5f 6361  ppend(cidx_to_ca
-00007380: 6e64 5b72 705f 6465 6665 6174 2e69 6e69  nd[rp_defeat.ini
-00007390: 7469 616c 5f65 6c65 6d65 6e74 7328 295b  tial_elements()[
-000073a0: 305d 5d29 0a20 2020 2072 6574 7572 6e20  0]]).    return 
-000073b0: 736f 7274 6564 286c 6973 7428 7365 7428  sorted(list(set(
-000073c0: 7769 6e6e 6572 7329 2929 0a0a 6465 6620  winners)))..def 
-000073d0: 7261 6e6b 6564 5f70 6169 7273 5f64 6566  ranked_pairs_def
-000073e0: 6561 7473 2865 6461 7461 2c20 6375 7272  eats(edata, curr
-000073f0: 5f63 616e 6473 203d 204e 6f6e 652c 2073  _cands = None, s
-00007400: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00007410: 203d 204e 6f6e 6529 3a20 2020 0a20 2020   = None):   .   
-00007420: 2022 2222 0a20 2020 2052 6574 7572 6e73   """.    Returns
-00007430: 2074 6865 2052 616e 6b65 6420 5061 6972   the Ranked Pair
-00007440: 7320 6465 6665 6174 2072 656c 6174 696f  s defeat relatio
-00007450: 6e73 2070 726f 6475 6365 6420 6279 2074  ns produced by t
-00007460: 6865 2052 616e 6b65 6420 5061 6972 7320  he Ranked Pairs 
-00007470: 616c 676f 7269 7468 6d2e 200a 0a20 2020  algorithm. ..   
-00007480: 202e 2e20 696d 706f 7274 616e 743a 3a0a   .. important::.
-00007490: 2020 2020 2020 2020 556e 6c69 6b65 2074          Unlike t
-000074a0: 6865 206f 7468 6572 2066 756e 6374 696f  he other functio
-000074b0: 6e73 2074 6861 7420 7265 7475 726e 2061  ns that return a
-000074c0: 2073 696e 676c 6520 6465 6665 6174 2072   single defeat r
-000074d0: 656c 6174 696f 6e2c 2074 6869 7320 7265  elation, this re
-000074e0: 7475 726e 7320 6120 6c69 7374 206f 6620  turns a list of 
-000074f0: 6465 6665 6174 2072 656c 6174 696f 6e73  defeat relations
-00007500: 2e20 0a20 2020 2020 2020 200a 2020 2020  . .        .    
-00007510: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-00007520: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-00007530: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-00007540: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-00007550: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-00007560: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-00007570: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
-00007580: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
-00007590: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
-000075a0: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
-000075b0: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
-000075c0: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
-000075d0: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
-000075e0: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
-000075f0: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
-00007600: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
-00007610: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
-00007620: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
-00007630: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
-00007640: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
-00007650: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
-00007660: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
-00007670: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
-00007680: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
-00007690: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
-000076a0: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
-000076b0: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
-000076c0: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
-000076d0: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
-000076e0: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
-000076f0: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
-00007700: 6e65 7477 6f72 6b78 2044 6947 7261 7068  networkx DiGraph
-00007710: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
-00007720: 6520 5261 6e6b 6564 2050 6169 7273 2064  e Ranked Pairs d
-00007730: 6566 6561 7420 7265 6c61 7469 6f6e 2e20  efeat relation. 
-00007740: 0a0a 2020 2020 2e2e 2073 6565 616c 736f  ..    .. seealso
-00007750: 3a3a 0a0a 2020 2020 2020 2020 3a6d 6574  ::..        :met
-00007760: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
-00007770: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-00007780: 6f64 732e 7261 6e6b 6564 5f70 6169 7273  ods.ranked_pairs
-00007790: 602c 203a 6d65 7468 3a60 7072 6566 5f76  `, :meth:`pref_v
-000077a0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-000077b0: 6564 5f6d 6574 686f 6473 2e72 616e 6b65  ed_methods.ranke
-000077c0: 645f 7061 6972 735f 7769 7468 5f74 6573  d_pairs_with_tes
-000077d0: 7460 0a0a 2020 2020 3a45 7861 6d70 6c65  t`..    :Example
-000077e0: 3a20 0a0a 2020 2020 2e2e 2070 6c6f 743a  : ..    .. plot:
-000077f0: 3a20 206d 6172 6769 6e5f 6772 6170 6873  :  margin_graphs
-00007800: 5f65 7861 6d70 6c65 732f 6d67 5f65 785f  _examples/mg_ex_
-00007810: 7270 5f64 6566 6561 7473 2e70 790a 2020  rp_defeats.py.  
-00007820: 2020 2020 2020 3a63 6f6e 7465 7874 3a20        :context: 
-00007830: 7265 7365 7420 200a 2020 2020 2020 2020  reset  .        
-00007840: 3a69 6e63 6c75 6465 2d73 6f75 7263 653a  :include-source:
-00007850: 2054 7275 650a 0a20 2020 202e 2e20 6578   True..    .. ex
-00007860: 6563 5f63 6f64 653a 3a0a 0a0a 2020 2020  ec_code::...    
-00007870: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
-00007880: 7469 6e67 2e77 6569 6768 7465 645f 6d61  ting.weighted_ma
-00007890: 6a6f 7269 7479 5f67 7261 7068 7320 696d  jority_graphs im
-000078a0: 706f 7274 204d 6172 6769 6e47 7261 7068  port MarginGraph
-000078b0: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
-000078c0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-000078d0: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
-000078e0: 6d70 6f72 7420 7261 6e6b 6564 5f70 6169  mport ranked_pai
-000078f0: 7273 5f64 6566 6561 7473 0a0a 2020 2020  rs_defeats..    
-00007900: 2020 2020 6d67 203d 204d 6172 6769 6e47      mg = MarginG
-00007910: 7261 7068 285b 302c 2031 2c20 322c 2033  raph([0, 1, 2, 3
-00007920: 5d2c 205b 2830 2c20 312c 2031 3029 2c20  ], [(0, 1, 10), 
-00007930: 2830 2c20 322c 2032 292c 2028 312c 2033  (0, 2, 2), (1, 3
-00007940: 2c20 3429 2c20 2832 2c20 312c 2036 292c  , 4), (2, 1, 6),
-00007950: 2028 322c 2033 2c20 3829 2c20 2833 2c20   (2, 3, 8), (3, 
-00007960: 302c 2034 295d 290a 2020 2020 2020 2020  0, 4)]).        
-00007970: 7270 5f64 6566 6561 7473 203d 2072 616e  rp_defeats = ran
-00007980: 6b65 645f 7061 6972 735f 6465 6665 6174  ked_pairs_defeat
-00007990: 7328 6d67 290a 0a20 2020 2020 2020 2066  s(mg)..        f
-000079a0: 6f72 2072 7064 2069 6e20 7270 5f64 6566  or rpd in rp_def
-000079b0: 6561 7473 3a20 0a20 2020 2020 2020 2020  eats: .         
-000079c0: 2020 2070 7269 6e74 2872 7064 2e65 6467     print(rpd.edg
-000079d0: 6573 290a 0a20 2020 2022 2222 0a20 2020  es)..    """.   
-000079e0: 200a 2020 2020 6361 6e64 6964 6174 6573   .    candidates
-000079f0: 203d 2065 6461 7461 2e63 616e 6469 6461   = edata.candida
-00007a00: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
-00007a10: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
-00007a20: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
-00007a30: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-00007a40: 696f 6e20 3d20 6564 6174 612e 6d61 7267  ion = edata.marg
-00007a50: 696e 2069 6620 7374 7265 6e67 7468 5f66  in if strength_f
-00007a60: 756e 6374 696f 6e20 6973 204e 6f6e 6520  unction is None 
-00007a70: 656c 7365 2073 7472 656e 6774 685f 6675  else strength_fu
-00007a80: 6e63 7469 6f6e 2020 2020 0a0a 2020 2020  nction    ..    
-00007a90: 775f 6564 6765 7320 3d20 5b28 6331 2c20  w_edges = [(c1, 
-00007aa0: 6332 2c20 7374 7265 6e67 7468 5f66 756e  c2, strength_fun
-00007ab0: 6374 696f 6e28 6331 2c20 6332 2929 2066  ction(c1, c2)) f
-00007ac0: 6f72 2063 3120 696e 2063 616e 6469 6461  or c1 in candida
-00007ad0: 7465 7320 666f 7220 6332 2069 6e20 6361  tes for c2 in ca
-00007ae0: 6e64 6964 6174 6573 2069 6620 6331 2021  ndidates if c1 !
-00007af0: 3d20 6332 2061 6e64 2028 6564 6174 612e  = c2 and (edata.
-00007b00: 6d61 6a6f 7269 7479 5f70 7265 6665 7273  majority_prefers
-00007b10: 2863 312c 2063 3229 206f 7220 6564 6174  (c1, c2) or edat
-00007b20: 612e 6973 5f74 6965 6428 6331 2c20 6332  a.is_tied(c1, c2
-00007b30: 2929 5d0a 2020 2020 7769 6e6e 6572 7320  ))].    winners 
-00007b40: 3d20 6c69 7374 2829 2020 2020 2020 2020  = list()        
-00007b50: 2020 2020 0a20 2020 2073 7472 656e 6774      .    strengt
-00007b60: 6873 203d 2073 6f72 7465 6428 6c69 7374  hs = sorted(list
-00007b70: 2873 6574 285b 655b 325d 2066 6f72 2065  (set([e[2] for e
-00007b80: 2069 6e20 775f 6564 6765 735d 2929 2c20   in w_edges])), 
-00007b90: 7265 7665 7273 653d 5472 7565 290a 2020  reverse=True).  
-00007ba0: 2020 736f 7274 6564 5f65 6467 6573 203d    sorted_edges =
-00007bb0: 205b 5b65 2066 6f72 2065 2069 6e20 775f   [[e for e in w_
-00007bc0: 6564 6765 7320 6966 2065 5b32 5d20 3d3d  edges if e[2] ==
-00007bd0: 2073 5d20 666f 7220 7320 696e 2073 7472   s] for s in str
-00007be0: 656e 6774 6873 5d0a 2020 2020 7462 7320  engths].    tbs 
-00007bf0: 3d20 7072 6f64 7563 7428 2a5b 7065 726d  = product(*[perm
-00007c00: 7574 6174 696f 6e73 2865 6467 6573 2920  utations(edges) 
-00007c10: 666f 7220 6564 6765 7320 696e 2073 6f72  for edges in sor
-00007c20: 7465 645f 6564 6765 735d 290a 2020 2020  ted_edges]).    
-00007c30: 7270 5f64 6566 6561 7473 203d 206c 6973  rp_defeats = lis
-00007c40: 7428 290a 2020 2020 666f 7220 7462 2069  t().    for tb i
-00007c50: 6e20 7462 733a 0a20 2020 2020 2020 2065  n tbs:.        e
-00007c60: 6467 6573 203d 2066 6c61 7474 656e 2874  dges = flatten(t
-00007c70: 6229 0a20 2020 2020 2020 2072 705f 6465  b).        rp_de
-00007c80: 6665 6174 203d 206e 782e 4469 4772 6170  feat = nx.DiGrap
-00007c90: 6828 2920 0a20 2020 2020 2020 2066 6f72  h() .        for
-00007ca0: 2065 2069 6e20 6564 6765 733a 200a 2020   e in edges: .  
-00007cb0: 2020 2020 2020 2020 2020 7270 5f64 6566            rp_def
-00007cc0: 6561 742e 6164 645f 6564 6765 2865 5b30  eat.add_edge(e[0
-00007cd0: 5d2c 2065 5b31 5d2c 2077 6569 6768 743d  ], e[1], weight=
-00007ce0: 655b 325d 290a 2020 2020 2020 2020 2020  e[2]).          
-00007cf0: 2020 6966 2064 6f65 735f 6372 6561 7465    if does_create
-00007d00: 5f63 7963 6c65 2872 705f 6465 6665 6174  _cycle(rp_defeat
-00007d10: 2c20 6529 3a0a 2020 2020 2020 2020 2020  , e):.          
-00007d20: 2020 2020 2020 7270 5f64 6566 6561 742e        rp_defeat.
-00007d30: 7265 6d6f 7665 5f65 6467 6528 655b 305d  remove_edge(e[0]
-00007d40: 2c20 655b 315d 290a 2020 2020 2020 2020  , e[1]).        
-00007d50: 7270 5f64 6566 6561 7473 2e61 7070 656e  rp_defeats.appen
-00007d60: 6428 7270 5f64 6566 6561 7429 0a20 2020  d(rp_defeat).   
-00007d70: 2020 2020 2077 696e 6e65 7273 2e61 7070       winners.app
-00007d80: 656e 6428 6d61 7869 6d61 6c5f 656c 656d  end(maximal_elem
-00007d90: 656e 7473 2872 705f 6465 6665 6174 295b  ents(rp_defeat)[
-00007da0: 305d 290a 2020 2020 7265 7475 726e 2072  0]).    return r
-00007db0: 705f 6465 6665 6174 730a 0a64 6566 2070  p_defeats..def p
-00007dc0: 6f77 6572 7365 7428 6974 6572 6162 6c65  owerset(iterable
-00007dd0: 293a 0a20 2020 2022 2222 0a20 2020 2052  ):.    """.    R
-00007de0: 6574 7572 6e20 7468 6520 706f 7765 7273  eturn the powers
-00007df0: 6574 206f 6620 6060 6974 6572 6162 6c65  et of ``iterable
-00007e00: 6060 0a0a 2020 2020 706f 7765 7273 6574  ``..    powerset
-00007e10: 285b 312c 322c 335d 2920 2d2d 3e20 2829  ([1,2,3]) --> ()
-00007e20: 2028 312c 2920 2832 2c29 2028 332c 2920   (1,) (2,) (3,) 
-00007e30: 2831 2c32 2920 2831 2c33 2920 2832 2c33  (1,2) (1,3) (2,3
-00007e40: 2920 2831 2c32 2c33 290a 2020 2020 2222  ) (1,2,3).    ""
-00007e50: 220a 2020 2020 7320 3d20 6c69 7374 2869  ".    s = list(i
-00007e60: 7465 7261 626c 6529 0a20 2020 2072 6574  terable).    ret
-00007e70: 7572 6e20 6368 6169 6e2e 6672 6f6d 5f69  urn chain.from_i
-00007e80: 7465 7261 626c 6528 636f 6d62 696e 6174  terable(combinat
-00007e90: 696f 6e73 2873 2c20 7229 2066 6f72 2072  ions(s, r) for r
-00007ea0: 2069 6e20 7261 6e67 6528 6c65 6e28 7329   in range(len(s)
-00007eb0: 2b31 2929 0a0a 0a64 6566 2069 735f 7374  +1))...def is_st
-00007ec0: 6163 6b28 6564 6174 612c 2063 616e 645f  ack(edata, cand_
-00007ed0: 6c69 7374 2c20 6375 7272 5f63 616e 6473  list, curr_cands
-00007ee0: 3d4e 6f6e 6529 3a20 0a20 2020 2022 2222  =None): .    """
-00007ef0: 0a20 2020 2041 202a 2a73 7461 636b 2a2a  .    A **stack**
-00007f00: 2069 7320 6120 6c69 6e65 6172 206f 7264   is a linear ord
-00007f10: 6572 203a 6d61 7468 3a60 4c60 206f 6e20  er :math:`L` on 
-00007f20: 7468 6520 6361 6e64 6964 6174 6520 7375  the candidate su
-00007f30: 6368 2074 6861 7420 666f 7220 616c 6c20  ch that for all 
-00007f40: 6361 6e64 6964 6174 6573 203a 6d61 7468  candidates :math
-00007f50: 3a60 6160 2061 6e64 203a 6d61 7468 3a60  :`a` and :math:`
-00007f60: 6260 2c20 6966 203a 6d61 7468 3a60 614c  b`, if :math:`aL
-00007f70: 6260 2c20 7468 656e 2074 6865 7265 2061  b`, then there a
-00007f80: 7265 2064 6973 7469 6e63 7420 6361 6e64  re distinct cand
-00007f90: 6964 6174 6573 203a 6d61 7468 3a60 785f  idates :math:`x_
-00007fa0: 312c 5c64 6f74 732c 785f 6e60 2077 6974  1,\dots,x_n` wit
-00007fb0: 6820 3a6d 6174 683a 6078 5f31 3d61 6020  h :math:`x_1=a` 
-00007fc0: 616e 6420 3a6d 6174 683a 6078 5f6e 3d62  and :math:`x_n=b
-00007fd0: 6020 7375 6368 2074 6861 7420 3a6d 6174  ` such that :mat
-00007fe0: 683a 6078 5f69 204c 2078 5f7b 692b 317d  h:`x_i L x_{i+1}
-00007ff0: 6020 616e 6420 666f 7220 616c 6c20 3a6d  ` and for all :m
-00008000: 6174 683a 6069 5c69 6e20 5c7b 312c 5c64  ath:`i\in \{1,\d
-00008010: 6f74 732c 206e 2d31 5c7d 602c 2074 6865  ots, n-1\}`, the
-00008020: 206d 6172 6769 6e20 6f66 203a 6d61 7468   margin of :math
-00008030: 3a60 785f 3160 206f 7665 7220 3a6d 6174  :`x_1` over :mat
-00008040: 683a 6078 5f7b 692b 317d 6020 6973 2067  h:`x_{i+1}` is g
-00008050: 7265 6174 6572 2074 6861 6e20 6f72 2065  reater than or e
-00008060: 7175 616c 2074 6f20 7468 6520 6d61 7267  qual to the marg
-00008070: 696e 206f 6620 3a6d 6174 683a 6062 6020  in of :math:`b` 
-00008080: 6f76 6572 203a 6d61 7468 3a60 6160 2e0a  over :math:`a`..
-00008090: 0a20 2020 2054 6869 7320 6465 6669 6e69  .    This defini
-000080a0: 7469 6f6e 2069 7320 6475 6520 746f 205a  tion is due to Z
-000080b0: 6176 6973 7420 616e 6420 5469 6465 6d61  avist and Tidema
-000080c0: 6e20 3139 3839 2c20 616e 6420 6973 2075  n 1989, and is u
-000080d0: 7365 6420 6173 2061 6e20 616c 7465 726e  sed as an altern
-000080e0: 6174 6976 6520 6368 6172 6163 7465 7269  ative characteri
-000080f0: 7a61 7469 6f6e 206f 6620 5261 6e6b 6564  zation of Ranked
-00008100: 2050 6169 7273 3a20 3a6d 6174 683a 6061   Pairs: :math:`a
-00008110: 6020 6973 2061 2052 616e 6b65 6420 5061  ` is a Ranked Pa
-00008120: 6972 7320 7769 6e6e 6572 2069 6620 616e  irs winner if an
-00008130: 6420 6f6e 6c79 2069 6620 3a6d 6174 683a  d only if :math:
-00008140: 6061 6020 6973 2074 6865 206d 6178 696d  `a` is the maxim
-00008150: 756d 2065 6c65 6d65 6e74 206f 6620 736f  um element of so
-00008160: 6d65 2073 7461 636b 2e20 0a0a 2020 2020  me stack. ..    
-00008170: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-00008180: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-00008190: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-000081a0: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-000081b0: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-000081c0: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-000081d0: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
-000081e0: 2020 2020 6361 6e64 5f6c 6973 7420 286c      cand_list (l
-000081f0: 6973 7429 3a20 5468 6520 6c69 7374 206f  ist): The list o
-00008200: 6620 6361 6e64 6964 6174 6573 2074 6861  f candidates tha
-00008210: 7420 6d61 7920 6265 2061 2073 7461 636b  t may be a stack
-00008220: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
-00008230: 6e64 7320 284c 6973 745b 696e 745d 2c20  nds (List[int], 
-00008240: 6f70 7469 6f6e 616c 293a 2049 6620 7365  optional): If se
-00008250: 742c 2074 6865 6e20 6669 6e64 2074 6865  t, then find the
-00008260: 2077 696e 6e65 7273 2066 6f72 2074 6865   winners for the
-00008270: 2070 726f 6669 6c65 2072 6573 7472 6963   profile restric
-00008280: 7465 6420 746f 2074 6865 2063 616e 6469  ted to the candi
-00008290: 6461 7465 7320 696e 2060 6063 7572 725f  dates in ``curr_
-000082a0: 6361 6e64 7360 600a 0a20 2020 2052 6574  cands``..    Ret
-000082b0: 7572 6e73 3a20 0a20 2020 2020 2020 2054  urns: .        T
-000082c0: 7275 6520 6966 2060 6063 616e 645f 6c69  rue if ``cand_li
-000082d0: 7374 6060 2069 7320 6120 7374 6163 6b20  st`` is a stack 
-000082e0: 616e 6420 4661 6c73 6520 6f74 6865 7277  and False otherw
-000082f0: 6973 650a 0a20 2020 203a 4578 616d 706c  ise..    :Exampl
-00008300: 653a 200a 2020 2020 0a20 2020 202e 2e20  e: .    .    .. 
-00008310: 706c 6f74 3a3a 2020 6d61 7267 696e 5f67  plot::  margin_g
-00008320: 7261 7068 735f 6578 616d 706c 6573 2f6d  raphs_examples/m
-00008330: 675f 6578 5f72 705f 7374 6163 6b73 2e70  g_ex_rp_stacks.p
-00008340: 790a 2020 2020 2020 2020 3a63 6f6e 7465  y.        :conte
-00008350: 7874 3a20 7265 7365 7420 200a 2020 2020  xt: reset  .    
-00008360: 2020 2020 3a69 6e63 6c75 6465 2d73 6f75      :include-sou
-00008370: 7263 653a 2054 7275 650a 0a0a 2020 2020  rce: True...    
-00008380: 2e2e 2065 7865 635f 636f 6465 3a3a 0a20  .. exec_code::. 
-00008390: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000083a0: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
-000083b0: 2e77 6569 6768 7465 645f 6d61 6a6f 7269  .weighted_majori
-000083c0: 7479 5f67 7261 7068 7320 696d 706f 7274  ty_graphs import
-000083d0: 204d 6172 6769 6e47 7261 7068 0a20 2020   MarginGraph.   
-000083e0: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-000083f0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-00008400: 6564 5f6d 6574 686f 6473 2069 6d70 6f72  ed_methods impor
-00008410: 7420 6973 5f73 7461 636b 0a20 2020 2020  t is_stack.     
-00008420: 2020 2066 726f 6d20 6974 6572 746f 6f6c     from itertool
-00008430: 7320 696d 706f 7274 2070 6572 6d75 7461  s import permuta
-00008440: 7469 6f6e 730a 2020 2020 2020 2020 0a20  tions.        . 
-00008450: 2020 2020 2020 206d 6720 3d20 4d61 7267         mg = Marg
-00008460: 696e 4772 6170 6828 5b30 2c20 312c 2032  inGraph([0, 1, 2
-00008470: 5d2c 205b 2830 2c20 312c 2032 292c 2028  ], [(0, 1, 2), (
-00008480: 312c 2032 2c20 3429 2c20 2832 2c20 302c  1, 2, 4), (2, 0,
-00008490: 2032 295d 290a 2020 2020 2020 2020 0a20   2)]).        . 
-000084a0: 2020 2020 2020 2066 6f72 2063 6c69 7374         for clist
-000084b0: 2069 6e20 7065 726d 7574 6174 696f 6e73   in permutations
-000084c0: 286d 672e 6361 6e64 6964 6174 6573 293a  (mg.candidates):
-000084d0: 200a 2020 2020 2020 2020 2020 2020 7072   .            pr
-000084e0: 696e 7428 6622 7b63 6c69 7374 7d20 7b27  int(f"{clist} {'
-000084f0: 6973 2720 6966 2069 735f 7374 6163 6b28  is' if is_stack(
-00008500: 6d67 2c20 636c 6973 7429 2065 6c73 6520  mg, clist) else 
-00008510: 2769 7320 6e6f 7427 7d20 6120 7374 6163  'is not'} a stac
-00008520: 6b22 290a 2020 2020 2020 2020 2020 2020  k").            
-00008530: 0a20 2020 2022 2222 0a20 2020 200a 2020  .    """.    .  
-00008540: 2020 6361 6e64 6964 6174 6573 203d 2063    candidates = c
-00008550: 7572 725f 6361 6e64 7320 6966 2063 7572  urr_cands if cur
-00008560: 725f 6361 6e64 7320 6973 206e 6f74 204e  r_cands is not N
-00008570: 6f6e 6520 656c 7365 2065 6461 7461 2e63  one else edata.c
-00008580: 616e 6469 6461 7465 730a 2020 2020 6361  andidates.    ca
-00008590: 6e64 5f70 6169 7273 203d 205b 2861 2c20  nd_pairs = [(a, 
-000085a0: 6229 2069 6620 6361 6e64 5f6c 6973 742e  b) if cand_list.
-000085b0: 696e 6465 7828 6129 203c 2063 616e 645f  index(a) < cand_
-000085c0: 6c69 7374 2e69 6e64 6578 2862 2920 656c  list.index(b) el
-000085d0: 7365 2028 622c 2061 2920 666f 7220 612c  se (b, a) for a,
-000085e0: 2062 2069 6e20 636f 6d62 696e 6174 696f   b in combinatio
-000085f0: 6e73 2863 616e 6469 6461 7465 732c 2032  ns(candidates, 2
-00008600: 295d 0a20 2020 2020 2020 200a 2020 2020  )].        .    
-00008610: 666f 7220 612c 2062 2069 6e20 6361 6e64  for a, b in cand
-00008620: 5f70 6169 7273 3a0a 2020 2020 2020 2020  _pairs:.        
-00008630: 6f74 6865 725f 6361 6e64 7320 3d20 5b63  other_cands = [c
-00008640: 2066 6f72 2063 2069 6e20 6361 6e64 6964   for c in candid
-00008650: 6174 6573 2069 6620 6320 213d 2061 2061  ates if c != a a
-00008660: 6e64 2063 2021 3d20 625d 0a20 2020 2020  nd c != b].     
-00008670: 2020 2066 6f75 6e64 5f70 6174 6820 3d20     found_path = 
-00008680: 4661 6c73 650a 2020 2020 2020 2020 0a20  False.        . 
-00008690: 2020 2020 2020 2073 7562 6c69 7374 203d         sublist =
-000086a0: 2063 616e 645f 6c69 7374 5b63 616e 645f   cand_list[cand_
-000086b0: 6c69 7374 2e69 6e64 6578 2861 2920 2b20  list.index(a) + 
-000086c0: 313a 6361 6e64 5f6c 6973 742e 696e 6465  1:cand_list.inde
-000086d0: 7828 6229 5d0a 2020 2020 2020 2020 0a20  x(b)].        . 
-000086e0: 2020 2020 2020 2066 6f72 2069 6e64 6963         for indic
-000086f0: 6573 2069 6e20 706f 7765 7273 6574 2872  es in powerset(r
-00008700: 616e 6765 286c 656e 2873 7562 6c69 7374  ange(len(sublist
-00008710: 2929 293a 200a 2020 2020 2020 2020 2020  ))): .          
-00008720: 2020 0a20 2020 2020 2020 2020 2020 2070    .            p
-00008730: 6174 6820 3d20 5b61 5d20 2b20 5b73 7562  ath = [a] + [sub
-00008740: 6c69 7374 5b69 5d20 666f 7220 6920 696e  list[i] for i in
-00008750: 2073 6f72 7465 6428 696e 6469 6365 7329   sorted(indices)
-00008760: 5d20 2b20 5b62 5d0a 2020 2020 2020 2020  ] + [b].        
-00008770: 2020 2020 6d61 7267 696e 7320 3d20 5b65      margins = [e
-00008780: 6461 7461 2e6d 6172 6769 6e28 7869 2c20  data.margin(xi, 
-00008790: 7061 7468 5b69 202b 2031 5d29 2066 6f72  path[i + 1]) for
-000087a0: 2069 2c20 7869 2069 6e20 656e 756d 6572   i, xi in enumer
-000087b0: 6174 6528 7061 7468 5b30 3a2d 315d 295d  ate(path[0:-1])]
-000087c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000087d0: 616c 6c28 5b63 616e 645f 6c69 7374 2e69  all([cand_list.i
-000087e0: 6e64 6578 2878 6929 203c 2063 616e 645f  ndex(xi) < cand_
-000087f0: 6c69 7374 2e69 6e64 6578 2870 6174 685b  list.index(path[
-00008800: 692b 315d 2920 666f 7220 692c 2078 6920  i+1]) for i, xi 
-00008810: 696e 2065 6e75 6d65 7261 7465 2870 6174  in enumerate(pat
-00008820: 685b 303a 2d31 5d29 5d29 2061 6e64 2061  h[0:-1])]) and a
-00008830: 6c6c 285b 6d20 3e3d 2065 6461 7461 2e6d  ll([m >= edata.m
-00008840: 6172 6769 6e28 622c 2061 2920 666f 7220  argin(b, a) for 
-00008850: 6d20 696e 206d 6172 6769 6e73 5d29 3a20  m in margins]): 
-00008860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008870: 2066 6f75 6e64 5f70 6174 6820 3d20 5472   found_path = Tr
-00008880: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-00008890: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-000088a0: 2069 6620 6e6f 7420 666f 756e 645f 7061   if not found_pa
-000088b0: 7468 3a20 0a20 2020 2020 2020 2020 2020  th: .           
-000088c0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-000088d0: 2020 7265 7475 726e 2054 7275 650a 0a40    return True..@
-000088e0: 766d 286e 616d 653d 2252 616e 6b65 6420  vm(name="Ranked 
-000088f0: 5061 6972 7322 290a 6465 6620 7261 6e6b  Pairs").def rank
-00008900: 6564 5f70 6169 7273 5f66 726f 6d5f 7374  ed_pairs_from_st
-00008910: 6163 6b73 2865 6461 7461 2c20 6375 7272  acks(edata, curr
-00008920: 5f63 616e 6473 203d 204e 6f6e 6529 3a20  _cands = None): 
-00008930: 0a20 2020 2022 2222 4669 6e64 2074 6865  .    """Find the
-00008940: 2052 616e 6b65 6420 5061 6972 7320 7769   Ranked Pairs wi
-00008950: 6e6e 6572 7320 6279 2069 7465 7261 7469  nners by iterati
-00008960: 6e67 206f 7665 7220 616c 6c20 7065 726d  ng over all perm
-00008970: 7574 6174 696f 6e73 206f 6620 6361 6e64  utations of cand
-00008980: 6964 6174 6573 2028 7265 7374 7269 6374  idates (restrict
-00008990: 6564 2074 6f20 6060 6375 7272 5f63 616e  ed to ``curr_can
-000089a0: 6473 6060 2069 6620 6e6f 7420 4e6f 6e65  ds`` if not None
-000089b0: 292c 2061 6e64 2063 6865 636b 696e 6720  ), and checking 
-000089c0: 6966 2074 6865 206c 6973 7420 6973 2061  if the list is a
-000089d0: 2073 7461 636b 2e20 0a0a 2020 2020 4172   stack. ..    Ar
-000089e0: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
-000089f0: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
-00008a00: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
-00008a10: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
-00008a20: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
-00008a30: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
-00008a40: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
-00008a50: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
-00008a60: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
-00008a70: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
-00008a80: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
-00008a90: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
-00008aa0: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
-00008ab0: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
-00008ac0: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
-00008ad0: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
-00008ae0: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
-00008af0: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
-00008b00: 7465 732e 200a 0a20 2020 202e 2e20 7365  tes. ..    .. se
-00008b10: 6561 6c73 6f3a 3a0a 0a20 2020 2020 2020  ealso::..       
-00008b20: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
-00008b30: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
-00008b40: 5f6d 6574 686f 6473 2e72 616e 6b65 645f  _methods.ranked_
-00008b50: 7061 6972 7360 2c20 3a6d 6574 683a 6070  pairs`, :meth:`p
-00008b60: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-00008b70: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-00008b80: 6973 5f73 7461 636b 600a 0a20 2020 203a  is_stack`..    :
-00008b90: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
-00008ba0: 2e20 706c 6f74 3a3a 2020 6d61 7267 696e  . plot::  margin
-00008bb0: 5f67 7261 7068 735f 6578 616d 706c 6573  _graphs_examples
-00008bc0: 2f6d 675f 6578 5f62 705f 7270 2e70 790a  /mg_ex_bp_rp.py.
-00008bd0: 2020 2020 2020 2020 3a63 6f6e 7465 7874          :context
-00008be0: 3a20 7265 7365 7420 200a 2020 2020 2020  : reset  .      
-00008bf0: 2020 3a69 6e63 6c75 6465 2d73 6f75 7263    :include-sourc
-00008c00: 653a 2054 7275 650a 0a0a 2020 2020 2e2e  e: True...    ..
-00008c10: 2063 6f64 652d 626c 6f63 6b3a 3a20 0a0a   code-block:: ..
-00008c20: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-00008c30: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
-00008c40: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
-00008c50: 706f 7274 2072 616e 6b65 645f 7061 6972  port ranked_pair
-00008c60: 732c 2072 616e 6b65 645f 7061 6972 735f  s, ranked_pairs_
-00008c70: 6672 6f6d 5f73 7461 636b 730a 0a20 2020  from_stacks..   
-00008c80: 2020 2020 2072 616e 6b65 645f 7061 6972       ranked_pair
-00008c90: 732e 6469 7370 6c61 7928 6d67 290a 2020  s.display(mg).  
-00008ca0: 2020 2020 2020 7261 6e6b 6564 5f70 6169        ranked_pai
-00008cb0: 7273 5f66 726f 6d5f 7374 6163 6b73 2e64  rs_from_stacks.d
-00008cc0: 6973 706c 6179 286d 6729 0a0a 0a20 2020  isplay(mg)...   
-00008cd0: 202e 2e20 6578 6563 5f63 6f64 653a 3a20   .. exec_code:: 
-00008ce0: 0a20 2020 2020 2020 203a 6869 6465 5f63  .        :hide_c
-00008cf0: 6f64 653a 0a0a 2020 2020 2020 2020 6672  ode:..        fr
-00008d00: 6f6d 2070 7265 665f 766f 7469 6e67 2e77  om pref_voting.w
-00008d10: 6569 6768 7465 645f 6d61 6a6f 7269 7479  eighted_majority
-00008d20: 5f67 7261 7068 7320 696d 706f 7274 204d  _graphs import M
-00008d30: 6172 6769 6e47 7261 7068 0a20 2020 2020  arginGraph.     
-00008d40: 2020 2066 726f 6d20 7072 6566 5f76 6f74     from pref_vot
-00008d50: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
-00008d60: 5f6d 6574 686f 6473 2069 6d70 6f72 7420  _methods import 
-00008d70: 7261 6e6b 6564 5f70 6169 7273 2c20 7261  ranked_pairs, ra
-00008d80: 6e6b 6564 5f70 6169 7273 5f66 726f 6d5f  nked_pairs_from_
-00008d90: 7374 6163 6b73 0a20 2020 2020 2020 200a  stacks.        .
-00008da0: 2020 2020 2020 2020 6d67 203d 204d 6172          mg = Mar
-00008db0: 6769 6e47 7261 7068 285b 302c 2031 2c20  ginGraph([0, 1, 
-00008dc0: 322c 2033 5d2c 205b 2830 2c20 322c 2033  2, 3], [(0, 2, 3
-00008dd0: 292c 2028 312c 2030 2c20 3529 2c20 2832  ), (1, 0, 5), (2
-00008de0: 2c20 312c 2035 292c 2028 322c 2033 2c20  , 1, 5), (2, 3, 
-00008df0: 3129 2c20 2833 2c20 302c 2033 292c 2028  1), (3, 0, 3), (
-00008e00: 332c 2031 2c20 3129 5d29 0a0a 2020 2020  3, 1, 1)])..    
-00008e10: 2020 2020 7261 6e6b 6564 5f70 6169 7273      ranked_pairs
-00008e20: 2e64 6973 706c 6179 286d 6729 0a20 2020  .display(mg).   
-00008e30: 2020 2020 2072 616e 6b65 645f 7061 6972       ranked_pair
-00008e40: 735f 6672 6f6d 5f73 7461 636b 732e 6469  s_from_stacks.di
-00008e50: 7370 6c61 7928 6d67 290a 0a20 2020 2022  splay(mg)..    "
-00008e60: 2222 2020 2020 0a0a 2020 2020 6361 6e64  ""    ..    cand
-00008e70: 6964 6174 6573 203d 2063 7572 725f 6361  idates = curr_ca
-00008e80: 6e64 7320 6966 2063 7572 725f 6361 6e64  nds if curr_cand
-00008e90: 7320 6973 206e 6f74 204e 6f6e 6520 656c  s is not None el
-00008ea0: 7365 2065 6461 7461 2e63 616e 6469 6461  se edata.candida
-00008eb0: 7465 730a 2020 2020 7769 6e6e 6572 7320  tes.    winners 
-00008ec0: 3d20 6c69 7374 2829 0a20 2020 2066 6f72  = list().    for
-00008ed0: 2063 6c69 7374 2069 6e20 7065 726d 7574   clist in permut
-00008ee0: 6174 696f 6e73 2863 616e 6469 6461 7465  ations(candidate
-00008ef0: 7329 3a20 0a20 2020 2020 2020 2069 7373  s): .        iss
-00008f00: 7461 636b 203d 2069 735f 7374 6163 6b28  tack = is_stack(
-00008f10: 6564 6174 612c 2063 6c69 7374 2c20 6375  edata, clist, cu
-00008f20: 7272 5f63 616e 6473 203d 2063 7572 725f  rr_cands = curr_
-00008f30: 6361 6e64 7329 0a20 2020 2020 2020 2069  cands).        i
-00008f40: 6620 6973 7374 6163 6b3a 200a 2020 2020  f isstack: .    
-00008f50: 2020 2020 2020 2020 7769 6e6e 6572 732e          winners.
-00008f60: 6170 7065 6e64 2863 6c69 7374 5b30 5d29  append(clist[0])
-00008f70: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-00008f80: 2020 7265 7475 726e 2073 6f72 7465 6428    return sorted(
-00008f90: 6c69 7374 2873 6574 2877 696e 6e65 7273  list(set(winners
-00008fa0: 2929 290a 0a40 766d 286e 616d 653d 2252  )))..@vm(name="R
-00008fb0: 616e 6b65 6420 5061 6972 7320 5442 2229  anked Pairs TB")
-00008fc0: 0a64 6566 2072 616e 6b65 645f 7061 6972  .def ranked_pair
-00008fd0: 735f 7462 2865 6461 7461 2c20 6375 7272  s_tb(edata, curr
-00008fe0: 5f63 616e 6473 203d 204e 6f6e 652c 2074  _cands = None, t
-00008ff0: 6965 5f62 7265 616b 6572 203d 204e 6f6e  ie_breaker = Non
-00009000: 652c 2073 7472 656e 6774 685f 6675 6e63  e, strength_func
-00009010: 7469 6f6e 203d 204e 6f6e 6529 3a20 2020  tion = None):   
-00009020: 0a20 2020 2022 2222 0a20 2020 2052 616e  .    """.    Ran
-00009030: 6b65 6420 5061 6972 7320 7769 7468 2061  ked Pairs with a
-00009040: 2066 6978 6564 206c 696e 6561 7220 6f72   fixed linear or
-00009050: 6465 7220 6f6e 2074 6865 2063 616e 6469  der on the candi
-00009060: 6461 7465 7320 746f 2062 7265 616b 2061  dates to break a
-00009070: 6e79 2074 6965 7320 696e 2074 6865 206d  ny ties in the m
-00009080: 6172 6769 6e73 2e20 2020 0a20 2020 2053  argins.   .    S
-00009090: 696e 6365 2074 6865 2074 6965 5f62 7265  ince the tie_bre
-000090a0: 616b 6572 2069 7320 6120 6c69 6e65 6172  aker is a linear
-000090b0: 206f 7264 6572 2c20 7468 6973 206d 6574   order, this met
-000090c0: 686f 6420 6973 2072 6573 6f6c 7574 652e  hod is resolute.
-000090d0: 2020 200a 0a20 2020 2041 7267 733a 0a20     ..    Args:. 
-000090e0: 2020 2020 2020 2065 6461 7461 2028 5072         edata (Pr
-000090f0: 6f66 696c 652c 2050 726f 6669 6c65 5769  ofile, ProfileWi
-00009100: 7468 5469 6573 2c20 4d61 7267 696e 4772  thTies, MarginGr
-00009110: 6170 6829 3a20 416e 7920 656c 6563 7469  aph): Any electi
-00009120: 6f6e 2064 6174 6120 7468 6174 2068 6173  on data that has
-00009130: 2061 2060 6d61 7267 696e 6020 6d65 7468   a `margin` meth
-00009140: 6f64 2e20 0a20 2020 2020 2020 2063 7572  od. .        cur
-00009150: 725f 6361 6e64 7320 284c 6973 745b 696e  r_cands (List[in
-00009160: 745d 2c20 6f70 7469 6f6e 616c 293a 2049  t], optional): I
-00009170: 6620 7365 742c 2074 6865 6e20 6669 6e64  f set, then find
-00009180: 2074 6865 2077 696e 6e65 7273 2066 6f72   the winners for
-00009190: 2074 6865 2070 726f 6669 6c65 2072 6573   the profile res
-000091a0: 7472 6963 7465 6420 746f 2074 6865 2063  tricted to the c
-000091b0: 616e 6469 6461 7465 7320 696e 2060 6063  andidates in ``c
-000091c0: 7572 725f 6361 6e64 7360 600a 2020 2020  urr_cands``.    
-000091d0: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
-000091e0: 6374 696f 6e20 2866 756e 6374 696f 6e2c  ction (function,
-000091f0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
-00009200: 7374 7265 6e67 7468 2066 756e 6374 696f  strength functio
-00009210: 6e20 746f 2062 6520 7573 6564 2074 6f20  n to be used to 
-00009220: 6361 6c63 756c 6174 6520 7468 6520 7374  calculate the st
-00009230: 7265 6e67 7468 206f 6620 6120 7061 7468  rength of a path
-00009240: 2e20 2020 5468 6520 6465 6661 756c 7420  .   The default 
-00009250: 6973 2074 6865 206d 6172 6769 6e20 6d65  is the margin me
-00009260: 7468 6f64 206f 6620 6060 6564 6174 6160  thod of ``edata`
-00009270: 602e 2020 2054 6869 7320 6f6e 6c79 206d  `.   This only m
-00009280: 6174 7465 7273 2077 6865 6e20 7468 6520  atters when the 
-00009290: 6261 6c6c 6f74 7320 6172 6520 6e6f 7420  ballots are not 
-000092a0: 6c69 6e65 6172 206f 7264 6572 732e 200a  linear orders. .
-000092b0: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
-000092c0: 2020 2020 2020 2041 2073 6f72 7465 6420         A sorted 
-000092d0: 6c69 7374 206f 6620 6361 6e64 6964 6174  list of candidat
-000092e0: 6573 2e20 0a0a 2020 2020 2e2e 2073 6565  es. ..    .. see
-000092f0: 616c 736f 3a3a 0a0a 2020 2020 2020 2020  also::..        
-00009300: 3a6d 6574 683a 6070 7265 665f 766f 7469  :meth:`pref_voti
-00009310: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
-00009320: 6d65 7468 6f64 732e 7261 6e6b 6564 5f70  methods.ranked_p
-00009330: 6169 7273 602c 203a 6d65 7468 3a60 7072  airs`, :meth:`pr
-00009340: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-00009350: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
-00009360: 616e 6b65 645f 7061 6972 735f 7769 7468  anked_pairs_with
-00009370: 5f74 6573 7460 2c20 3a6d 6574 683a 6070  _test`, :meth:`p
-00009380: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-00009390: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-000093a0: 7261 6e6b 6564 5f70 6169 7273 5f66 726f  ranked_pairs_fro
-000093b0: 6d5f 7374 6163 6b73 600a 0a20 2020 202e  m_stacks`..    .
-000093c0: 2e20 6578 6563 5f63 6f64 653a 3a0a 0a20  . exec_code::.. 
-000093d0: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
-000093e0: 5f76 6f74 696e 672e 7072 6f66 696c 6573  _voting.profiles
-000093f0: 2069 6d70 6f72 7420 5072 6f66 696c 650a   import Profile.
-00009400: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-00009410: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
-00009420: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
-00009430: 706f 7274 2072 616e 6b65 645f 7061 6972  port ranked_pair
-00009440: 735f 6672 6f6d 5f73 7461 636b 732c 2072  s_from_stacks, r
-00009450: 616e 6b65 645f 7061 6972 735f 7462 2c20  anked_pairs_tb, 
-00009460: 7261 6e6b 6564 5f70 6169 7273 5f7a 740a  ranked_pairs_zt.
-00009470: 0a20 2020 2020 2020 2070 726f 6620 3d20  .        prof = 
-00009480: 5072 6f66 696c 6528 5b5b 322c 2033 2c20  Profile([[2, 3, 
-00009490: 312c 2030 5d2c 205b 302c 2033 2c20 312c  1, 0], [0, 3, 1,
-000094a0: 2032 5d2c 205b 312c 2033 2c20 322c 2030   2], [1, 3, 2, 0
-000094b0: 5d2c 205b 322c 2031 2c20 332c 2030 5d5d  ], [2, 1, 3, 0]]
-000094c0: 2c20 5b31 2c20 312c 2031 2c20 315d 290a  , [1, 1, 1, 1]).
-000094d0: 0a20 2020 2020 2020 2070 726f 662e 6469  .        prof.di
-000094e0: 7370 6c61 7928 290a 0a20 2020 2020 2020  splay()..       
-000094f0: 2072 616e 6b65 645f 7061 6972 735f 6672   ranked_pairs_fr
-00009500: 6f6d 5f73 7461 636b 732e 6469 7370 6c61  om_stacks.displa
-00009510: 7928 7072 6f66 290a 2020 2020 2020 2020  y(prof).        
-00009520: 7261 6e6b 6564 5f70 6169 7273 5f74 622e  ranked_pairs_tb.
-00009530: 6469 7370 6c61 7928 7072 6f66 290a 2020  display(prof).  
-00009540: 2020 2020 2020 7261 6e6b 6564 5f70 6169        ranked_pai
-00009550: 7273 5f74 622e 6469 7370 6c61 7928 7072  rs_tb.display(pr
-00009560: 6f66 2c20 7469 655f 6272 6561 6b65 7220  of, tie_breaker 
-00009570: 3d20 5b33 2c20 322c 2031 2c20 305d 290a  = [3, 2, 1, 0]).
-00009580: 2020 2020 2020 2020 7261 6e6b 6564 5f70          ranked_p
-00009590: 6169 7273 5f7a 742e 6469 7370 6c61 7928  airs_zt.display(
-000095a0: 7072 6f66 290a 0a20 2020 2022 2222 0a0a  prof)..    """..
-000095b0: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
-000095c0: 2065 6461 7461 2e63 616e 6469 6461 7465   edata.candidate
-000095d0: 7320 6966 2063 7572 725f 6361 6e64 7320  s if curr_cands 
-000095e0: 6973 204e 6f6e 6520 656c 7365 2063 7572  is None else cur
-000095f0: 725f 6361 6e64 7320 2020 200a 2020 2020  r_cands    .    
-00009600: 6369 6478 5f74 6f5f 6361 6e64 203d 207b  cidx_to_cand = {
-00009610: 6369 6478 3a20 6320 666f 7220 6369 6478  cidx: c for cidx
-00009620: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
-00009630: 2863 616e 6469 6461 7465 7329 7d20 200a  (candidates)}  .
-00009640: 2020 2020 6361 6e64 5f74 6f5f 6369 6478      cand_to_cidx
-00009650: 203d 207b 633a 2063 6964 7820 666f 7220   = {c: cidx for 
-00009660: 6369 6478 2c20 6320 696e 2065 6e75 6d65  cidx, c in enume
-00009670: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-00009680: 7d20 200a 0a20 2020 2073 7472 656e 6774  }  ..    strengt
-00009690: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
-000096a0: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
-000096b0: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
-000096c0: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
-000096d0: 6e67 7468 5f66 756e 6374 696f 6e0a 2020  ngth_function.  
-000096e0: 2020 0a20 2020 2074 625f 7261 6e6b 696e    .    tb_rankin
-000096f0: 6720 3d20 7469 655f 6272 6561 6b65 7220  g = tie_breaker 
-00009700: 6966 2074 6965 5f62 7265 616b 6572 2069  if tie_breaker i
-00009710: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-00009720: 736f 7274 6564 286c 6973 7428 6361 6e64  sorted(list(cand
-00009730: 6964 6174 6573 2929 0a0a 2020 2020 6377  idates))..    cw
-00009740: 203d 2065 6461 7461 2e63 6f6e 646f 7263   = edata.condorc
-00009750: 6574 5f77 696e 6e65 7228 6375 7272 5f63  et_winner(curr_c
-00009760: 616e 6473 3d63 7572 725f 6361 6e64 7329  ands=curr_cands)
-00009770: 0a20 2020 2023 2052 616e 6b65 6420 5061  .    # Ranked Pa
-00009780: 6972 7320 6973 2043 6f6e 646f 7263 6574  irs is Condorcet
-00009790: 2063 6f6e 7369 7374 656e 742c 2073 6f20   consistent, so 
-000097a0: 7369 6d70 6c79 2072 6574 7572 6e20 7468  simply return th
-000097b0: 6520 436f 6e64 6f72 6365 7420 7769 6e6e  e Condorcet winn
-000097c0: 6572 2069 6620 6578 6973 7473 0a20 2020  er if exists.   
-000097d0: 2069 6620 6377 2069 7320 6e6f 7420 4e6f   if cw is not No
-000097e0: 6e65 3a20 0a20 2020 2020 2020 2077 696e  ne: .        win
-000097f0: 6e65 7273 203d 205b 6377 5d0a 2020 2020  ners = [cw].    
-00009800: 656c 7365 3a0a 2020 2020 2020 2020 775f  else:.        w_
-00009810: 6564 6765 7320 3d20 5b28 6331 2c20 6332  edges = [(c1, c2
-00009820: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
-00009830: 696f 6e28 6331 2c20 6332 2929 2066 6f72  ion(c1, c2)) for
-00009840: 2063 3120 696e 2063 616e 6469 6461 7465   c1 in candidate
-00009850: 7320 666f 7220 6332 2069 6e20 6361 6e64  s for c2 in cand
-00009860: 6964 6174 6573 200a 2020 2020 2020 2020  idates .        
-00009870: 2020 2020 2020 2020 2020 2069 6620 6331             if c1
-00009880: 2021 3d20 6332 2061 6e64 2028 6564 6174   != c2 and (edat
-00009890: 612e 6d61 6a6f 7269 7479 5f70 7265 6665  a.majority_prefe
-000098a0: 7273 2863 312c 2063 3229 206f 7220 6564  rs(c1, c2) or ed
-000098b0: 6174 612e 6973 5f74 6965 6428 6331 2c20  ata.is_tied(c1, 
-000098c0: 6332 2929 5d0a 2020 2020 2020 2020 7769  c2))].        wi
-000098d0: 6e6e 6572 7320 3d20 6c69 7374 2829 2020  nners = list()  
-000098e0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-000098f0: 2020 2073 7472 656e 6774 6873 203d 2073     strengths = s
-00009900: 6f72 7465 6428 6c69 7374 2873 6574 285b  orted(list(set([
-00009910: 655b 325d 2066 6f72 2065 2069 6e20 775f  e[2] for e in w_
-00009920: 6564 6765 735d 2929 2c20 7265 7665 7273  edges])), revers
-00009930: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
-00009940: 0a20 2020 2020 2020 2072 705f 6465 6665  .        rp_defe
-00009950: 6174 203d 2053 504f 286c 656e 2863 616e  at = SPO(len(can
-00009960: 6469 6461 7465 7329 290a 0a20 2020 2020  didates))..     
-00009970: 2020 2066 6f72 2073 2069 6e20 7374 7265     for s in stre
-00009980: 6e67 7468 733a 200a 2020 2020 2020 2020  ngths: .        
-00009990: 2020 2020 6564 6765 7320 3d20 5b65 2066      edges = [e f
-000099a0: 6f72 2065 2069 6e20 775f 6564 6765 7320  or e in w_edges 
-000099b0: 6966 2065 5b32 5d20 3d3d 2073 5d0a 2020  if e[2] == s].  
-000099c0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-000099d0: 2020 2020 2020 2023 2062 7265 616b 2074         # break t
-000099e0: 6965 7320 7573 696e 6720 7468 6520 6c65  ies using the le
-000099f0: 7869 636f 6772 6170 6869 6320 6f72 6465  xicographic orde
-00009a00: 7269 6e67 206f 6e20 7475 706c 6573 2067  ring on tuples g
-00009a10: 6976 656e 2074 625f 7261 6e6b 696e 670a  iven tb_ranking.
-00009a20: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-00009a30: 6564 5f65 6467 6573 203d 2073 6f72 7465  ed_edges = sorte
-00009a40: 6428 6564 6765 732c 206b 6579 203d 206c  d(edges, key = l
-00009a50: 616d 6264 6120 653a 2028 7462 5f72 616e  ambda e: (tb_ran
-00009a60: 6b69 6e67 2e69 6e64 6578 2865 5b30 5d29  king.index(e[0])
-00009a70: 2c20 7462 5f72 616e 6b69 6e67 2e69 6e64  , tb_ranking.ind
-00009a80: 6578 2865 5b31 5d29 292c 2072 6576 6572  ex(e[1])), rever
-00009a90: 7365 3d46 616c 7365 290a 2020 2020 2020  se=False).      
-00009aa0: 2020 2020 2020 666f 7220 6530 2c65 312c        for e0,e1,
-00009ab0: 7320 696e 2065 6467 6573 3a20 0a20 2020  s in edges: .   
-00009ac0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00009ad0: 6e6f 7420 7270 5f64 6566 6561 742e 505b  not rp_defeat.P[
-00009ae0: 6361 6e64 5f74 6f5f 6369 6478 5b65 315d  cand_to_cidx[e1]
-00009af0: 5d5b 6361 6e64 5f74 6f5f 6369 6478 5b65  ][cand_to_cidx[e
-00009b00: 305d 5d3a 0a20 2020 2020 2020 2020 2020  0]]:.           
-00009b10: 2020 2020 2020 2020 2072 705f 6465 6665           rp_defe
-00009b20: 6174 2e61 6464 2863 616e 645f 746f 5f63  at.add(cand_to_c
-00009b30: 6964 785b 6530 5d2c 6361 6e64 5f74 6f5f  idx[e0],cand_to_
-00009b40: 6369 6478 5b65 315d 290a 2020 2020 2020  cidx[e1]).      
-00009b50: 2020 2020 2020 7769 6e6e 6572 732e 6170        winners.ap
-00009b60: 7065 6e64 2863 6964 785f 746f 5f63 616e  pend(cidx_to_can
-00009b70: 645b 7270 5f64 6566 6561 742e 696e 6974  d[rp_defeat.init
-00009b80: 6961 6c5f 656c 656d 656e 7473 2829 5b30  ial_elements()[0
-00009b90: 5d5d 290a 0a20 2020 2072 6574 7572 6e20  ]])..    return 
-00009ba0: 736f 7274 6564 286c 6973 7428 7365 7428  sorted(list(set(
-00009bb0: 7769 6e6e 6572 7329 2929 0a0a 0a40 766d  winners)))...@vm
-00009bc0: 286e 616d 653d 2252 616e 6b65 6420 5061  (name="Ranked Pa
-00009bd0: 6972 7320 5a54 2229 0a64 6566 2072 616e  irs ZT").def ran
-00009be0: 6b65 645f 7061 6972 735f 7a74 2870 726f  ked_pairs_zt(pro
-00009bf0: 6669 6c65 2c20 6375 7272 5f63 616e 6473  file, curr_cands
-00009c00: 203d 204e 6f6e 652c 2073 7472 656e 6774   = None, strengt
-00009c10: 685f 6675 6e63 7469 6f6e 203d 204e 6f6e  h_function = Non
-00009c20: 6529 3a20 2020 0a20 2020 2022 2222 5261  e):   .    """Ra
-00009c30: 6e6b 6564 2070 6169 7273 2077 6865 7265  nked pairs where
-00009c40: 2061 2066 6978 6564 2076 6f74 6572 2062   a fixed voter b
-00009c50: 7265 616b 7320 616e 7920 7469 6573 2069  reaks any ties i
-00009c60: 6e20 7468 6520 6d61 7267 696e 732e 2020  n the margins.  
-00009c70: 4974 2069 7320 616c 7761 7973 2074 6865  It is always the
-00009c80: 2076 6f74 6572 2069 6e20 706f 7369 7469   voter in positi
-00009c90: 6f6e 2030 2074 6861 7420 6272 6561 6b73  on 0 that breaks
-00009ca0: 2074 6865 2074 6965 732e 2020 5369 6e63   the ties.  Sinc
-00009cb0: 6520 766f 7465 7273 2068 6176 6520 7374  e voters have st
-00009cc0: 7269 6374 2070 7265 6665 7265 6e63 6573  rict preferences
-00009cd0: 2c20 7468 6973 206d 6574 686f 6420 6973  , this method is
-00009ce0: 2072 6573 6f6c 7574 652e 2020 5468 6973   resolute.  This
-00009cf0: 2069 7320 6b6e 6f77 6e20 6173 2052 616e   is known as Ran
-00009d00: 6b65 6420 5061 6972 7320 5a54 2c20 666f  ked Pairs ZT, fo
-00009d10: 7220 5a61 7669 7374 2054 6964 656d 616e  r Zavist Tideman
-00009d20: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00009d30: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-00009d40: 696c 6529 3a20 4120 7072 6f66 696c 6520  ile): A profile 
-00009d50: 6f66 206c 696e 6561 7220 6f72 6465 7273  of linear orders
-00009d60: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
-00009d70: 6e64 7320 284c 6973 745b 696e 745d 2c20  nds (List[int], 
-00009d80: 6f70 7469 6f6e 616c 293a 2049 6620 7365  optional): If se
-00009d90: 742c 2074 6865 6e20 6669 6e64 2074 6865  t, then find the
-00009da0: 2077 696e 6e65 7273 2066 6f72 2074 6865   winners for the
-00009db0: 2070 726f 6669 6c65 2072 6573 7472 6963   profile restric
-00009dc0: 7465 6420 746f 2074 6865 2063 616e 6469  ted to the candi
-00009dd0: 6461 7465 7320 696e 2060 6063 7572 725f  dates in ``curr_
-00009de0: 6361 6e64 7360 600a 0a20 2020 2052 6574  cands``..    Ret
-00009df0: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
-00009e00: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
-00009e10: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
-00009e20: 2020 2e2e 2073 6565 616c 736f 3a3a 0a0a    .. seealso::..
-00009e30: 2020 2020 2020 2020 3a6d 6574 683a 6070          :meth:`p
-00009e40: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-00009e50: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-00009e60: 7261 6e6b 6564 5f70 6169 7273 602c 203a  ranked_pairs`, :
-00009e70: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-00009e80: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-00009e90: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
-00009ea0: 6972 735f 7769 7468 5f74 6573 7460 2c20  irs_with_test`, 
-00009eb0: 3a6d 6574 683a 6070 7265 665f 766f 7469  :meth:`pref_voti
-00009ec0: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
-00009ed0: 6d65 7468 6f64 732e 7261 6e6b 6564 5f70  methods.ranked_p
-00009ee0: 6169 7273 5f66 726f 6d5f 7374 6163 6b73  airs_from_stacks
-00009ef0: 600a 0a20 2020 202e 2e20 6578 6563 5f63  `..    .. exec_c
-00009f00: 6f64 653a 3a0a 0a20 2020 2020 2020 2066  ode::..        f
-00009f10: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
-00009f20: 7072 6f66 696c 6573 2069 6d70 6f72 7420  profiles import 
-00009f30: 5072 6f66 696c 650a 2020 2020 2020 2020  Profile.        
-00009f40: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
-00009f50: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-00009f60: 7468 6f64 7320 696d 706f 7274 2072 616e  thods import ran
-00009f70: 6b65 645f 7061 6972 735f 6672 6f6d 5f73  ked_pairs_from_s
-00009f80: 7461 636b 732c 2072 616e 6b65 645f 7061  tacks, ranked_pa
-00009f90: 6972 735f 7462 2c20 7261 6e6b 6564 5f70  irs_tb, ranked_p
-00009fa0: 6169 7273 5f7a 740a 0a20 2020 2020 2020  airs_zt..       
-00009fb0: 2070 726f 6620 3d20 5072 6f66 696c 6528   prof = Profile(
-00009fc0: 5b5b 322c 2033 2c20 312c 2030 5d2c 205b  [[2, 3, 1, 0], [
-00009fd0: 302c 2033 2c20 312c 2032 5d2c 205b 312c  0, 3, 1, 2], [1,
-00009fe0: 2033 2c20 322c 2030 5d2c 205b 322c 2031   3, 2, 0], [2, 1
-00009ff0: 2c20 332c 2030 5d5d 2c20 5b31 2c20 312c  , 3, 0]], [1, 1,
-0000a000: 2031 2c20 315d 290a 0a20 2020 2020 2020   1, 1])..       
-0000a010: 2070 726f 662e 6469 7370 6c61 7928 290a   prof.display().
-0000a020: 0a20 2020 2020 2020 2072 616e 6b65 645f  .        ranked_
-0000a030: 7061 6972 735f 6672 6f6d 5f73 7461 636b  pairs_from_stack
-0000a040: 732e 6469 7370 6c61 7928 7072 6f66 290a  s.display(prof).
-0000a050: 2020 2020 2020 2020 7261 6e6b 6564 5f70          ranked_p
-0000a060: 6169 7273 5f74 622e 6469 7370 6c61 7928  airs_tb.display(
-0000a070: 7072 6f66 290a 2020 2020 2020 2020 7261  prof).        ra
-0000a080: 6e6b 6564 5f70 6169 7273 5f74 622e 6469  nked_pairs_tb.di
-0000a090: 7370 6c61 7928 7072 6f66 2c20 7469 655f  splay(prof, tie_
-0000a0a0: 6272 6561 6b65 7220 3d20 5b33 2c20 322c  breaker = [3, 2,
-0000a0b0: 2031 2c20 305d 290a 2020 2020 2020 2020   1, 0]).        
-0000a0c0: 7261 6e6b 6564 5f70 6169 7273 5f7a 742e  ranked_pairs_zt.
-0000a0d0: 6469 7370 6c61 7928 7072 6f66 290a 0a20  display(prof).. 
-0000a0e0: 2020 200a 2020 2020 2222 220a 2020 2020     .    """.    
-0000a0f0: 6361 6e64 6964 6174 6573 203d 2070 726f  candidates = pro
-0000a100: 6669 6c65 2e63 616e 6469 6461 7465 7320  file.candidates 
-0000a110: 6966 2063 7572 725f 6361 6e64 7320 6973  if curr_cands is
-0000a120: 204e 6f6e 6520 656c 7365 2063 7572 725f   None else curr_
-0000a130: 6361 6e64 7320 2020 200a 2020 2020 0a20  cands    .    . 
-0000a140: 2020 2023 2074 6865 2074 6965 2d62 7265     # the tie-bre
-0000a150: 616b 6572 2069 7320 616c 7761 7973 2074  aker is always t
-0000a160: 6865 2066 6972 7374 2076 6f74 6572 2e20  he first voter. 
-0000a170: 0a20 2020 2074 625f 7261 6e6b 696e 6720  .    tb_ranking 
-0000a180: 3d20 7475 706c 6528 5b63 2066 6f72 2063  = tuple([c for c
-0000a190: 2069 6e20 6c69 7374 2870 726f 6669 6c65   in list(profile
-0000a1a0: 2e5f 7261 6e6b 696e 6773 5b30 5d29 2069  ._rankings[0]) i
-0000a1b0: 6620 6320 696e 2063 616e 6469 6461 7465  f c in candidate
-0000a1c0: 735d 290a 2020 2020 0a20 2020 2072 6574  s]).    .    ret
-0000a1d0: 7572 6e20 7261 6e6b 6564 5f70 6169 7273  urn ranked_pairs
-0000a1e0: 5f74 6228 7072 6f66 696c 652c 2063 7572  _tb(profile, cur
-0000a1f0: 725f 6361 6e64 7320 3d20 6375 7272 5f63  r_cands = curr_c
-0000a200: 616e 6473 2c20 7469 655f 6272 6561 6b65  ands, tie_breake
-0000a210: 7220 3d20 7462 5f72 616e 6b69 6e67 2c20  r = tb_ranking, 
-0000a220: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000a230: 6e20 3d20 7374 7265 6e67 7468 5f66 756e  n = strength_fun
-0000a240: 6374 696f 6e29 0a0a 0a0a 4076 6d28 6e61  ction)....@vm(na
-0000a250: 6d65 3d22 5269 7665 7222 290a 6465 6620  me="River").def 
-0000a260: 7269 7665 7228 6564 6174 612c 2063 7572  river(edata, cur
-0000a270: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
-0000a280: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000a290: 6e20 3d20 4e6f 6e65 293a 2020 200a 2020  n = None):   .  
-0000a2a0: 2020 2222 220a 2020 2020 4f72 6465 7220    """.    Order 
-0000a2b0: 7468 6520 6564 6765 7320 696e 2074 6865  the edges in the
-0000a2c0: 2077 6561 6b20 6d61 7267 696e 2067 7261   weak margin gra
-0000a2d0: 7068 2066 726f 6d20 6c61 7267 6573 7420  ph from largest 
-0000a2e0: 746f 2073 6d61 6c6c 6573 7420 616e 6420  to smallest and 
-0000a2f0: 6c6f 636b 2074 6865 6d20 696e 2069 6e20  lock them in in 
-0000a300: 7468 6174 206f 7264 6572 2c20 736b 6970  that order, skip
-0000a310: 7069 6e67 2065 6467 6573 2074 6861 7420  ping edges that 
-0000a320: 6372 6561 7465 2061 2063 7963 6c65 202a  create a cycle *
-0000a330: 616e 6420 6564 6765 7320 696e 2077 6869  and edges in whi
-0000a340: 6368 2074 6865 7265 2069 7320 616c 7265  ch there is alre
-0000a350: 6164 7920 616e 2065 6467 6520 706f 696e  ady an edge poin
-0000a360: 7469 6e67 2074 6f20 7468 6520 7461 7267  ting to the targ
-0000a370: 6574 2a2e 2020 4272 6561 6b20 7469 6573  et*.  Break ties
-0000a380: 2075 7369 6e67 2061 2074 6965 2d62 7265   using a tie-bre
-0000a390: 616b 696e 6720 206c 696e 6561 7220 6f72  aking  linear or
-0000a3a0: 6465 7269 6e67 206f 7665 7220 7468 6520  dering over the 
-0000a3b0: 6564 6765 732e 2020 4120 6361 6e64 6964  edges.  A candid
-0000a3c0: 6174 6520 6973 2061 2052 6976 6572 2077  ate is a River w
-0000a3d0: 696e 6e65 7220 6966 2069 7420 7769 6e73  inner if it wins
-0000a3e0: 2061 6363 6f72 6469 6e67 2074 6f20 736f   according to so
-0000a3f0: 6d65 2074 6965 2d62 7265 616b 696e 6720  me tie-breaking 
-0000a400: 7275 6c65 2e20 5365 6520 6874 7470 733a  rule. See https:
-0000a410: 2f2f 656c 6563 746f 7769 6b69 2e6f 7267  //electowiki.org
-0000a420: 2f77 696b 692f 5269 7665 722e 0a0a 2020  /wiki/River...  
-0000a430: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000a440: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
-0000a450: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
-0000a460: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
-0000a470: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
-0000a480: 2074 6861 7420 6861 7320 6120 606d 6172   that has a `mar
-0000a490: 6769 6e60 206d 6574 686f 642e 200a 2020  gin` method. .  
-0000a4a0: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
-0000a4b0: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
-0000a4c0: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
-0000a4d0: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
-0000a4e0: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
-0000a4f0: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
-0000a500: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
-0000a510: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
-0000a520: 6473 6060 0a20 2020 2020 2020 2073 7472  ds``.        str
-0000a530: 656e 6774 685f 6675 6e63 7469 6f6e 2028  ength_function (
-0000a540: 6675 6e63 7469 6f6e 2c20 6f70 7469 6f6e  function, option
-0000a550: 616c 293a 2054 6865 2073 7472 656e 6774  al): The strengt
-0000a560: 6820 6675 6e63 7469 6f6e 2074 6f20 6265  h function to be
-0000a570: 2075 7365 6420 746f 2063 616c 6375 6c61   used to calcula
-0000a580: 7465 2074 6865 2073 7472 656e 6774 6820  te the strength 
-0000a590: 6f66 2061 2070 6174 682e 2020 2054 6865  of a path.   The
-0000a5a0: 2064 6566 6175 6c74 2069 7320 7468 6520   default is the 
-0000a5b0: 6d61 7267 696e 206d 6574 686f 6420 6f66  margin method of
-0000a5c0: 2060 6065 6461 7461 6060 2e20 2020 5468   ``edata``.   Th
-0000a5d0: 6973 206f 6e6c 7920 6d61 7474 6572 7320  is only matters 
-0000a5e0: 7768 656e 2074 6865 2062 616c 6c6f 7473  when the ballots
-0000a5f0: 2061 7265 206e 6f74 206c 696e 6561 7220   are not linear 
-0000a600: 6f72 6465 7273 2e20 0a0a 2020 2020 5265  orders. ..    Re
-0000a610: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
-0000a620: 4120 736f 7274 6564 206c 6973 7420 6f66  A sorted list of
-0000a630: 2063 616e 6469 6461 7465 732e 200a 0a20   candidates. .. 
-0000a640: 2020 203a 4578 616d 706c 653a 200a 0a20     :Example: .. 
-0000a650: 2020 202e 2e20 6578 6563 5f63 6f64 653a     .. exec_code:
-0000a660: 3a20 0a0a 2020 2020 2020 2020 6672 6f6d  : ..        from
-0000a670: 2070 7265 665f 766f 7469 6e67 2e77 6569   pref_voting.wei
-0000a680: 6768 7465 645f 6d61 6a6f 7269 7479 5f67  ghted_majority_g
-0000a690: 7261 7068 7320 696d 706f 7274 204d 6172  raphs import Mar
-0000a6a0: 6769 6e47 7261 7068 0a20 2020 2020 2020  ginGraph.       
-0000a6b0: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
-0000a6c0: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-0000a6d0: 6574 686f 6473 2069 6d70 6f72 7420 7269  ethods import ri
-0000a6e0: 7665 722c 2072 616e 6b65 645f 7061 6972  ver, ranked_pair
-0000a6f0: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
-0000a700: 2020 206d 6720 3d20 4d61 7267 696e 4772     mg = MarginGr
-0000a710: 6170 6828 5b30 2c20 312c 2032 2c20 335d  aph([0, 1, 2, 3]
-0000a720: 2c20 5b28 302c 2032 2c20 3229 2c20 2830  , [(0, 2, 2), (0
-0000a730: 2c20 332c 2038 292c 2028 312c 2030 2c20  , 3, 8), (1, 0, 
-0000a740: 3132 292c 2028 322c 2033 2c20 3132 292c  12), (2, 3, 12),
-0000a750: 2028 332c 2031 2c20 3629 5d29 0a0a 2020   (3, 1, 6)])..  
-0000a760: 2020 2020 2020 7261 6e6b 6564 5f70 6169        ranked_pai
-0000a770: 7273 2e64 6973 706c 6179 286d 6729 0a20  rs.display(mg). 
-0000a780: 2020 2020 2020 2072 6976 6572 2e64 6973         river.dis
-0000a790: 706c 6179 286d 6729 0a0a 2020 2020 2222  play(mg)..    ""
-0000a7a0: 220a 2020 2020 6361 6e64 6964 6174 6573  ".    candidates
-0000a7b0: 203d 2065 6461 7461 2e63 616e 6469 6461   = edata.candida
-0000a7c0: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
-0000a7d0: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
-0000a7e0: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
-0000a7f0: 2020 6369 6478 5f74 6f5f 6361 6e64 203d    cidx_to_cand =
-0000a800: 207b 6369 6478 3a20 6320 666f 7220 6369   {cidx: c for ci
-0000a810: 6478 2c20 6320 696e 2065 6e75 6d65 7261  dx, c in enumera
-0000a820: 7465 2863 616e 6469 6461 7465 7329 7d20  te(candidates)} 
-0000a830: 200a 2020 2020 6361 6e64 5f74 6f5f 6369   .    cand_to_ci
-0000a840: 6478 203d 207b 633a 2063 6964 7820 666f  dx = {c: cidx fo
-0000a850: 7220 6369 6478 2c20 6320 696e 2065 6e75  r cidx, c in enu
-0000a860: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
-0000a870: 7329 7d20 200a 0a20 2020 2073 7472 656e  s)}  ..    stren
-0000a880: 6774 685f 6675 6e63 7469 6f6e 203d 2065  gth_function = e
-0000a890: 6461 7461 2e6d 6172 6769 6e20 6966 2073  data.margin if s
-0000a8a0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000a8b0: 2069 7320 4e6f 6e65 2065 6c73 6520 7374   is None else st
-0000a8c0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-0000a8d0: 2020 200a 0a20 2020 2063 7720 3d20 6564     ..    cw = ed
-0000a8e0: 6174 612e 636f 6e64 6f72 6365 745f 7769  ata.condorcet_wi
-0000a8f0: 6e6e 6572 2863 7572 725f 6361 6e64 733d  nner(curr_cands=
-0000a900: 6375 7272 5f63 616e 6473 290a 2020 2020  curr_cands).    
-0000a910: 2320 5261 6e6b 6564 2050 6169 7273 2069  # Ranked Pairs i
-0000a920: 7320 436f 6e64 6f72 6365 7420 636f 6e73  s Condorcet cons
-0000a930: 6973 7465 6e74 2c20 736f 2073 696d 706c  istent, so simpl
-0000a940: 7920 7265 7475 726e 2074 6865 2043 6f6e  y return the Con
-0000a950: 646f 7263 6574 2077 696e 6e65 7220 6966  dorcet winner if
-0000a960: 2065 7869 7374 730a 2020 2020 6966 2063   exists.    if c
-0000a970: 7720 6973 206e 6f74 204e 6f6e 653a 200a  w is not None: .
-0000a980: 2020 2020 2020 2020 7769 6e6e 6572 7320          winners 
-0000a990: 3d20 5b63 775d 0a20 2020 2065 6c73 653a  = [cw].    else:
-0000a9a0: 0a20 2020 2020 2020 2077 5f65 6467 6573  .        w_edges
-0000a9b0: 203d 205b 2863 312c 2063 322c 2073 7472   = [(c1, c2, str
-0000a9c0: 656e 6774 685f 6675 6e63 7469 6f6e 2863  ength_function(c
-0000a9d0: 312c 2063 3229 2920 666f 7220 6331 2069  1, c2)) for c1 i
-0000a9e0: 6e20 6361 6e64 6964 6174 6573 2066 6f72  n candidates for
-0000a9f0: 2063 3220 696e 2063 616e 6469 6461 7465   c2 in candidate
-0000aa00: 7320 0a20 2020 2020 2020 2020 2020 2020  s .             
-0000aa10: 2020 2020 2020 6966 2063 3120 213d 2063        if c1 != c
-0000aa20: 3220 616e 6420 2865 6461 7461 2e6d 616a  2 and (edata.maj
-0000aa30: 6f72 6974 795f 7072 6566 6572 7328 6331  ority_prefers(c1
-0000aa40: 2c20 6332 2920 6f72 2065 6461 7461 2e69  , c2) or edata.i
-0000aa50: 735f 7469 6564 2863 312c 2063 3229 295d  s_tied(c1, c2))]
-0000aa60: 0a20 2020 2020 2020 2077 696e 6e65 7273  .        winners
-0000aa70: 203d 206c 6973 7428 2920 2020 2020 2020   = list()       
-0000aa80: 2020 2020 200a 2020 2020 2020 2020 7374       .        st
-0000aa90: 7265 6e67 7468 7320 3d20 736f 7274 6564  rengths = sorted
-0000aaa0: 286c 6973 7428 7365 7428 5b65 5b32 5d20  (list(set([e[2] 
-0000aab0: 666f 7220 6520 696e 2077 5f65 6467 6573  for e in w_edges
-0000aac0: 5d29 292c 2072 6576 6572 7365 3d54 7275  ])), reverse=Tru
-0000aad0: 6529 0a20 2020 2020 2020 2073 6f72 7465  e).        sorte
-0000aae0: 645f 6564 6765 7320 3d20 5b5b 6520 666f  d_edges = [[e fo
-0000aaf0: 7220 6520 696e 2077 5f65 6467 6573 2069  r e in w_edges i
-0000ab00: 6620 655b 325d 203d 3d20 735d 2066 6f72  f e[2] == s] for
-0000ab10: 2073 2069 6e20 7374 7265 6e67 7468 735d   s in strengths]
-0000ab20: 0a20 2020 2020 2020 2074 6273 203d 2070  .        tbs = p
-0000ab30: 726f 6475 6374 282a 5b70 6572 6d75 7461  roduct(*[permuta
-0000ab40: 7469 6f6e 7328 6564 6765 7329 2066 6f72  tions(edges) for
-0000ab50: 2065 6467 6573 2069 6e20 736f 7274 6564   edges in sorted
-0000ab60: 5f65 6467 6573 5d29 0a20 2020 2020 2020  _edges]).       
-0000ab70: 2066 6f72 2074 6220 696e 2074 6273 3a0a   for tb in tbs:.
-0000ab80: 2020 2020 2020 2020 2020 2020 6564 6765              edge
-0000ab90: 7320 3d20 666c 6174 7465 6e28 7462 290a  s = flatten(tb).
-0000aba0: 2020 2020 2020 2020 2020 2020 7276 5f64              rv_d
-0000abb0: 6566 6561 7420 3d20 5350 4f28 6c65 6e28  efeat = SPO(len(
-0000abc0: 6361 6e64 6964 6174 6573 2929 0a20 2020  candidates)).   
-0000abd0: 2020 2020 2020 2020 2066 6f72 2065 302c           for e0,
-0000abe0: 6531 2c73 2069 6e20 6564 6765 733a 200a  e1,s in edges: .
-0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac00: 6966 206e 6f74 2072 765f 6465 6665 6174  if not rv_defeat
-0000ac10: 2e50 5b63 616e 645f 746f 5f63 6964 785b  .P[cand_to_cidx[
-0000ac20: 6531 5d5d 5b63 616e 645f 746f 5f63 6964  e1]][cand_to_cid
-0000ac30: 785b 6530 5d5d 2061 6e64 206c 656e 2872  x[e0]] and len(r
-0000ac40: 765f 6465 6665 6174 2e70 7265 6473 5b63  v_defeat.preds[c
-0000ac50: 616e 645f 746f 5f63 6964 785b 6531 5d5d  and_to_cidx[e1]]
-0000ac60: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
-0000ac70: 2020 2020 2020 2020 2020 2020 7276 5f64              rv_d
-0000ac80: 6566 6561 742e 6164 6428 6361 6e64 5f74  efeat.add(cand_t
-0000ac90: 6f5f 6369 6478 5b65 305d 2c63 616e 645f  o_cidx[e0],cand_
-0000aca0: 746f 5f63 6964 785b 6531 5d29 0a20 2020  to_cidx[e1]).   
-0000acb0: 2020 2020 2020 2020 2077 696e 6e65 7273           winners
-0000acc0: 2e61 7070 656e 6428 6369 6478 5f74 6f5f  .append(cidx_to_
-0000acd0: 6361 6e64 5b72 765f 6465 6665 6174 2e69  cand[rv_defeat.i
-0000ace0: 6e69 7469 616c 5f65 6c65 6d65 6e74 7328  nitial_elements(
-0000acf0: 295b 305d 5d29 0a0a 2020 2020 7265 7475  )[0]])..    retu
-0000ad00: 726e 2073 6f72 7465 6428 6c69 7374 2873  rn sorted(list(s
-0000ad10: 6574 2877 696e 6e65 7273 2929 290a 0a64  et(winners)))..d
-0000ad20: 6566 2072 6976 6572 5f64 6566 6561 7473  ef river_defeats
-0000ad30: 2865 6461 7461 2c20 6375 7272 5f63 616e  (edata, curr_can
-0000ad40: 6473 203d 204e 6f6e 652c 2073 7472 656e  ds = None, stren
-0000ad50: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
-0000ad60: 6f6e 6529 3a0a 2020 2020 2222 220a 2020  one):.    """.  
-0000ad70: 2020 5265 7475 726e 7320 7468 6520 5269    Returns the Ri
-0000ad80: 7665 7220 6465 6665 6174 2072 656c 6174  ver defeat relat
-0000ad90: 696f 6e73 2070 726f 6475 6365 6420 6279  ions produced by
-0000ada0: 2074 6865 2052 6976 6572 2061 6c67 6f72   the River algor
-0000adb0: 6974 686d 2e0a 0a20 2020 202e 2e20 696d  ithm...    .. im
-0000adc0: 706f 7274 616e 743a 3a0a 2020 2020 2020  portant::.      
-0000add0: 2020 556e 6c69 6b65 2074 6865 206f 7468    Unlike the oth
-0000ade0: 6572 2066 756e 6374 696f 6e73 2074 6861  er functions tha
-0000adf0: 7420 7265 7475 726e 2061 2073 696e 676c  t return a singl
-0000ae00: 6520 6465 6665 6174 2072 656c 6174 696f  e defeat relatio
-0000ae10: 6e2c 2074 6869 7320 7265 7475 726e 7320  n, this returns 
-0000ae20: 6120 6c69 7374 206f 6620 6465 6665 6174  a list of defeat
-0000ae30: 2072 656c 6174 696f 6e73 2e20 0a20 2020   relations. .   
-0000ae40: 2020 2020 200a 2020 2020 4172 6773 3a0a       .    Args:.
-0000ae50: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
-0000ae60: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
-0000ae70: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
-0000ae80: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
-0000ae90: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
-0000aea0: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
-0000aeb0: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
-0000aec0: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
-0000aed0: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
-0000aee0: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
-0000aef0: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
-0000af00: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
-0000af10: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
-0000af20: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
-0000af30: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
-0000af40: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
-0000af50: 6e63 7469 6f6e 2028 6675 6e63 7469 6f6e  nction (function
-0000af60: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-0000af70: 2073 7472 656e 6774 6820 6675 6e63 7469   strength functi
-0000af80: 6f6e 2074 6f20 6265 2075 7365 6420 746f  on to be used to
-0000af90: 2063 616c 6375 6c61 7465 2074 6865 2073   calculate the s
-0000afa0: 7472 656e 6774 6820 6f66 2061 2070 6174  trength of a pat
-0000afb0: 682e 2020 2054 6865 2064 6566 6175 6c74  h.   The default
-0000afc0: 2069 7320 7468 6520 6d61 7267 696e 206d   is the margin m
-0000afd0: 6574 686f 6420 6f66 2060 6065 6461 7461  ethod of ``edata
-0000afe0: 6060 2e20 2020 5468 6973 206f 6e6c 7920  ``.   This only 
-0000aff0: 6d61 7474 6572 7320 7768 656e 2074 6865  matters when the
-0000b000: 2062 616c 6c6f 7473 2061 7265 206e 6f74   ballots are not
-0000b010: 206c 696e 6561 7220 6f72 6465 7273 2e20   linear orders. 
-0000b020: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
-0000b030: 2020 2020 2020 2020 4120 6e65 7477 6f72          A networ
-0000b040: 6b78 2044 6947 7261 7068 2072 6570 7265  kx DiGraph repre
-0000b050: 7365 6e74 696e 6720 7468 6520 5269 7665  senting the Rive
-0000b060: 7220 6465 6665 6174 2072 656c 6174 696f  r defeat relatio
-0000b070: 6e2e 200a 2020 2020 2222 220a 0a20 2020  n. .    """..   
-0000b080: 2063 616e 6469 6461 7465 7320 3d20 6564   candidates = ed
-0000b090: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
-0000b0a0: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
-0000b0b0: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
-0000b0c0: 616e 6473 2020 2020 0a20 2020 2073 7472  ands    .    str
-0000b0d0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-0000b0e0: 2065 6461 7461 2e6d 6172 6769 6e20 6966   edata.margin if
-0000b0f0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000b100: 6f6e 2069 7320 4e6f 6e65 2065 6c73 6520  on is None else 
-0000b110: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000b120: 6e20 2020 200a 0a20 2020 2077 5f65 6467  n    ..    w_edg
-0000b130: 6573 203d 205b 2863 312c 2063 322c 2073  es = [(c1, c2, s
-0000b140: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000b150: 2863 312c 2063 3229 2920 666f 7220 6331  (c1, c2)) for c1
-0000b160: 2069 6e20 6361 6e64 6964 6174 6573 2066   in candidates f
-0000b170: 6f72 2063 3220 696e 2063 616e 6469 6461  or c2 in candida
-0000b180: 7465 7320 6966 2063 3120 213d 2063 3220  tes if c1 != c2 
-0000b190: 616e 6420 2865 6461 7461 2e6d 616a 6f72  and (edata.major
-0000b1a0: 6974 795f 7072 6566 6572 7328 6331 2c20  ity_prefers(c1, 
-0000b1b0: 6332 2920 6f72 2065 6461 7461 2e69 735f  c2) or edata.is_
-0000b1c0: 7469 6564 2863 312c 2063 3229 295d 0a0a  tied(c1, c2))]..
-0000b1d0: 2020 2020 7374 7265 6e67 7468 7320 3d20      strengths = 
-0000b1e0: 736f 7274 6564 286c 6973 7428 7365 7428  sorted(list(set(
-0000b1f0: 5b65 5b32 5d20 666f 7220 6520 696e 2077  [e[2] for e in w
-0000b200: 5f65 6467 6573 5d29 292c 2072 6576 6572  _edges])), rever
-0000b210: 7365 3d54 7275 6529 0a20 2020 2073 6f72  se=True).    sor
-0000b220: 7465 645f 6564 6765 7320 3d20 5b5b 6520  ted_edges = [[e 
-0000b230: 666f 7220 6520 696e 2077 5f65 6467 6573  for e in w_edges
-0000b240: 2069 6620 655b 325d 203d 3d20 735d 2066   if e[2] == s] f
-0000b250: 6f72 2073 2069 6e20 7374 7265 6e67 7468  or s in strength
-0000b260: 735d 0a20 2020 2074 6273 203d 2070 726f  s].    tbs = pro
-0000b270: 6475 6374 282a 5b70 6572 6d75 7461 7469  duct(*[permutati
-0000b280: 6f6e 7328 6564 6765 7329 2066 6f72 2065  ons(edges) for e
-0000b290: 6467 6573 2069 6e20 736f 7274 6564 5f65  dges in sorted_e
-0000b2a0: 6467 6573 5d29 0a0a 2020 2020 7269 7665  dges])..    rive
-0000b2b0: 725f 6465 6665 6174 7320 3d20 6c69 7374  r_defeats = list
-0000b2c0: 2829 0a20 2020 2066 6f72 2074 6220 696e  ().    for tb in
-0000b2d0: 2074 6273 3a0a 2020 2020 2020 2020 6564   tbs:.        ed
-0000b2e0: 6765 7320 3d20 666c 6174 7465 6e28 7462  ges = flatten(tb
-0000b2f0: 290a 2020 2020 2020 2020 7269 7665 725f  ).        river_
-0000b300: 6465 6665 6174 203d 206e 782e 4469 4772  defeat = nx.DiGr
-0000b310: 6170 6828 2920 0a20 2020 2020 2020 2066  aph() .        f
-0000b320: 6f72 2065 2069 6e20 6564 6765 733a 200a  or e in edges: .
-0000b330: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-0000b340: 5b31 5d20 6e6f 7420 696e 2072 6976 6572  [1] not in river
-0000b350: 5f64 6566 6561 742e 6e6f 6465 7320 6f72  _defeat.nodes or
-0000b360: 206c 656e 286c 6973 7428 7269 7665 725f   len(list(river_
-0000b370: 6465 6665 6174 2e69 6e5f 6564 6765 7328  defeat.in_edges(
-0000b380: 655b 315d 2929 2920 3d3d 2030 3a0a 2020  e[1]))) == 0:.  
-0000b390: 2020 2020 2020 2020 2020 2020 2020 7269                ri
-0000b3a0: 7665 725f 6465 6665 6174 2e61 6464 5f65  ver_defeat.add_e
-0000b3b0: 6467 6528 655b 305d 2c20 655b 315d 2c20  dge(e[0], e[1], 
-0000b3c0: 7765 6967 6874 3d65 5b32 5d29 0a20 2020  weight=e[2]).   
-0000b3d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000b3e0: 646f 6573 5f63 7265 6174 655f 6379 636c  does_create_cycl
-0000b3f0: 6528 7269 7665 725f 6465 6665 6174 2c20  e(river_defeat, 
-0000b400: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-0000b410: 2020 2020 2020 2020 7269 7665 725f 6465          river_de
-0000b420: 6665 6174 2e72 656d 6f76 655f 6564 6765  feat.remove_edge
-0000b430: 2865 5b30 5d2c 2065 5b31 5d29 0a20 2020  (e[0], e[1]).   
-0000b440: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-0000b450: 2020 7269 7665 725f 6465 6665 6174 732e    river_defeats.
-0000b460: 6170 7065 6e64 2872 6976 6572 5f64 6566  append(river_def
-0000b470: 6561 7429 0a0a 2020 2020 7265 7475 726e  eat)..    return
-0000b480: 2072 6976 6572 5f64 6566 6561 7473 0a0a   river_defeats..
-0000b490: 4076 6d28 6e61 6d65 3d22 5269 7665 7222  @vm(name="River"
-0000b4a0: 290a 6465 6620 7269 7665 725f 7769 7468  ).def river_with
-0000b4b0: 5f74 6573 7428 6564 6174 612c 2063 7572  _test(edata, cur
-0000b4c0: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
-0000b4d0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000b4e0: 6e20 3d20 4e6f 6e65 293a 2020 200a 2020  n = None):   .  
-0000b4f0: 2020 2222 2246 696e 6420 7468 6520 5269    """Find the Ri
-0000b500: 7665 7220 7769 6e6e 6572 7320 7769 7468  ver winners with
-0000b510: 2061 2074 6573 7420 746f 2064 6574 6572   a test to deter
-0000b520: 6d69 6e65 6420 6966 2069 7420 7769 6c6c  mined if it will
-0000b530: 2074 616b 6520 746f 6f20 6c6f 6e67 2074   take too long t
-0000b540: 6f20 636f 6d70 7574 6520 7468 6520 5269  o compute the Ri
-0000b550: 7665 7220 7769 6e6e 6572 732e 2049 6620  ver winners. If 
-0000b560: 7468 6520 6361 6c63 756c 6174 696f 6e20  the calculation 
-0000b570: 6f66 2074 6865 2077 696e 6e65 7273 2077  of the winners w
-0000b580: 696c 6c20 7461 6b65 2074 6f6f 206c 6f6e  ill take too lon
-0000b590: 672c 2072 6574 7572 6e20 4e6f 6e65 2e20  g, return None. 
-0000b5a0: 0a20 2020 2020 2020 200a 2020 2020 2e2e  .        .    ..
-0000b5b0: 2069 6d70 6f72 7461 6e74 3a3a 0a20 2020   important::.   
-0000b5c0: 2020 2020 2054 6869 7320 766f 7469 6e67       This voting
-0000b5d0: 206d 6574 686f 6420 7468 6174 206d 6967   method that mig
-0000b5e0: 6874 2072 6574 7572 6e20 4e6f 6e65 2072  ht return None r
-0000b5f0: 6174 6865 7220 7468 616e 2061 206c 6973  ather than a lis
-0000b600: 7420 6f66 2063 616e 6469 6461 7465 732e  t of candidates.
-0000b610: 2020 0a0a 2020 2020 4172 6773 3a0a 2020    ..    Args:.  
-0000b620: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
-0000b630: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
-0000b640: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
-0000b650: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
-0000b660: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
-0000b670: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
-0000b680: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
-0000b690: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
-0000b6a0: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
-0000b6b0: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
-0000b6c0: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
-0000b6d0: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
-0000b6e0: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
-0000b6f0: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
-0000b700: 7272 5f63 616e 6473 6060 0a20 2020 2020  rr_cands``.     
-0000b710: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-0000b720: 7469 6f6e 2028 6675 6e63 7469 6f6e 2c20  tion (function, 
-0000b730: 6f70 7469 6f6e 616c 293a 2054 6865 2073  optional): The s
-0000b740: 7472 656e 6774 6820 6675 6e63 7469 6f6e  trength function
-0000b750: 2074 6f20 6265 2075 7365 6420 746f 2063   to be used to c
-0000b760: 616c 6375 6c61 7465 2074 6865 2073 7472  alculate the str
-0000b770: 656e 6774 6820 6f66 2061 2070 6174 682e  ength of a path.
-0000b780: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
-0000b790: 7320 7468 6520 6d61 7267 696e 206d 6574  s the margin met
-0000b7a0: 686f 6420 6f66 2060 6065 6461 7461 6060  hod of ``edata``
-0000b7b0: 2e20 2020 5468 6973 206f 6e6c 7920 6d61  .   This only ma
-0000b7c0: 7474 6572 7320 7768 656e 2074 6865 2062  tters when the b
-0000b7d0: 616c 6c6f 7473 2061 7265 206e 6f74 206c  allots are not l
-0000b7e0: 696e 6561 7220 6f72 6465 7273 2e20 0a0a  inear orders. ..
-0000b7f0: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
-0000b800: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
-0000b810: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
-0000b820: 732e 200a 0a20 2020 202e 2e20 7365 6561  s. ..    .. seea
-0000b830: 6c73 6f3a 3a0a 0a20 2020 2020 2020 203a  lso::..        :
-0000b840: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-0000b850: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-0000b860: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
-0000b870: 6972 735f 7769 7468 5f74 6573 7460 2c20  irs_with_test`, 
-0000b880: 3a6d 6574 683a 6070 7265 665f 766f 7469  :meth:`pref_voti
-0000b890: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
-0000b8a0: 6d65 7468 6f64 732e 7269 7665 7260 0a0a  methods.river`..
-0000b8b0: 0a20 2020 2022 2222 0a20 2020 2063 616e  .    """.    can
-0000b8c0: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
-0000b8d0: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
-0000b8e0: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
-0000b8f0: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
-0000b900: 2020 2020 0a20 2020 2063 6964 785f 746f      .    cidx_to
-0000b910: 5f63 616e 6420 3d20 7b63 6964 783a 2063  _cand = {cidx: c
-0000b920: 2066 6f72 2063 6964 782c 2063 2069 6e20   for cidx, c in 
-0000b930: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
-0000b940: 6174 6573 297d 2020 0a20 2020 2063 616e  ates)}  .    can
-0000b950: 645f 746f 5f63 6964 7820 3d20 7b63 3a20  d_to_cidx = {c: 
-0000b960: 6369 6478 2066 6f72 2063 6964 782c 2063  cidx for cidx, c
-0000b970: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-0000b980: 6e64 6964 6174 6573 297d 2020 0a0a 2020  ndidates)}  ..  
-0000b990: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-0000b9a0: 696f 6e20 3d20 6564 6174 612e 6d61 7267  ion = edata.marg
-0000b9b0: 696e 2069 6620 7374 7265 6e67 7468 5f66  in if strength_f
-0000b9c0: 756e 6374 696f 6e20 6973 204e 6f6e 6520  unction is None 
-0000b9d0: 656c 7365 2073 7472 656e 6774 685f 6675  else strength_fu
-0000b9e0: 6e63 7469 6f6e 2020 2020 0a0a 2020 2020  nction    ..    
-0000b9f0: 6377 203d 2065 6461 7461 2e63 6f6e 646f  cw = edata.condo
-0000ba00: 7263 6574 5f77 696e 6e65 7228 6375 7272  rcet_winner(curr
-0000ba10: 5f63 616e 6473 3d63 7572 725f 6361 6e64  _cands=curr_cand
-0000ba20: 7329 0a20 2020 2023 2052 616e 6b65 6420  s).    # Ranked 
-0000ba30: 5061 6972 7320 6973 2043 6f6e 646f 7263  Pairs is Condorc
-0000ba40: 6574 2063 6f6e 7369 7374 656e 742c 2073  et consistent, s
-0000ba50: 6f20 7369 6d70 6c79 2072 6574 7572 6e20  o simply return 
-0000ba60: 7468 6520 436f 6e64 6f72 6365 7420 7769  the Condorcet wi
-0000ba70: 6e6e 6572 2069 6620 6578 6973 7473 0a20  nner if exists. 
-0000ba80: 2020 2069 6620 6377 2069 7320 6e6f 7420     if cw is not 
-0000ba90: 4e6f 6e65 3a20 0a20 2020 2020 2020 2077  None: .        w
-0000baa0: 696e 6e65 7273 203d 205b 6377 5d0a 2020  inners = [cw].  
-0000bab0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000bac0: 775f 6564 6765 7320 3d20 5b28 6331 2c20  w_edges = [(c1, 
-0000bad0: 6332 2c20 7374 7265 6e67 7468 5f66 756e  c2, strength_fun
-0000bae0: 6374 696f 6e28 6331 2c20 6332 2929 2066  ction(c1, c2)) f
-0000baf0: 6f72 2063 3120 696e 2063 616e 6469 6461  or c1 in candida
-0000bb00: 7465 7320 666f 7220 6332 2069 6e20 6361  tes for c2 in ca
-0000bb10: 6e64 6964 6174 6573 200a 2020 2020 2020  ndidates .      
-0000bb20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000bb30: 6331 2021 3d20 6332 2061 6e64 2028 6564  c1 != c2 and (ed
-0000bb40: 6174 612e 6d61 6a6f 7269 7479 5f70 7265  ata.majority_pre
-0000bb50: 6665 7273 2863 312c 2063 3229 206f 7220  fers(c1, c2) or 
-0000bb60: 6564 6174 612e 6973 5f74 6965 6428 6331  edata.is_tied(c1
-0000bb70: 2c20 6332 2929 5d0a 2020 2020 2020 2020  , c2))].        
-0000bb80: 7769 6e6e 6572 7320 3d20 6c69 7374 2829  winners = list()
-0000bb90: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-0000bba0: 2020 2020 2073 7472 656e 6774 6873 203d       strengths =
-0000bbb0: 2073 6f72 7465 6428 6c69 7374 2873 6574   sorted(list(set
-0000bbc0: 285b 655b 325d 2066 6f72 2065 2069 6e20  ([e[2] for e in 
-0000bbd0: 775f 6564 6765 735d 2929 2c20 7265 7665  w_edges])), reve
-0000bbe0: 7273 653d 5472 7565 290a 2020 2020 2020  rse=True).      
-0000bbf0: 2020 736f 7274 6564 5f65 6467 6573 203d    sorted_edges =
-0000bc00: 205b 5b65 2066 6f72 2065 2069 6e20 775f   [[e for e in w_
-0000bc10: 6564 6765 7320 6966 2065 5b32 5d20 3d3d  edges if e[2] ==
-0000bc20: 2073 5d20 666f 7220 7320 696e 2073 7472   s] for s in str
-0000bc30: 656e 6774 6873 5d0a 2020 2020 2020 2020  engths].        
-0000bc40: 6966 206e 702e 7072 6f64 285b 6d61 7468  if np.prod([math
-0000bc50: 2e66 6163 746f 7269 616c 286c 656e 2865  .factorial(len(e
-0000bc60: 7329 2920 666f 7220 6573 2069 6e20 736f  s)) for es in so
-0000bc70: 7274 6564 5f65 6467 6573 5d29 203e 2033  rted_edges]) > 3
-0000bc80: 3030 303a 200a 2020 2020 2020 2020 2020  000: .          
-0000bc90: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
-0000bca0: 2020 2020 2020 656c 7365 3a20 0a20 2020        else: .   
-0000bcb0: 2020 2020 2020 2020 2074 6273 203d 2070           tbs = p
-0000bcc0: 726f 6475 6374 282a 5b70 6572 6d75 7461  roduct(*[permuta
-0000bcd0: 7469 6f6e 7328 6564 6765 7329 2066 6f72  tions(edges) for
-0000bce0: 2065 6467 6573 2069 6e20 736f 7274 6564   edges in sorted
-0000bcf0: 5f65 6467 6573 5d29 0a20 2020 2020 2020  _edges]).       
-0000bd00: 2020 2020 2066 6f72 2074 6220 696e 2074       for tb in t
-0000bd10: 6273 3a0a 2020 2020 2020 2020 2020 2020  bs:.            
-0000bd20: 2020 2020 6564 6765 7320 3d20 666c 6174      edges = flat
-0000bd30: 7465 6e28 7462 290a 2020 2020 2020 2020  ten(tb).        
-0000bd40: 2020 2020 2020 2020 7276 5f64 6566 6561          rv_defea
-0000bd50: 7420 3d20 5350 4f28 6c65 6e28 6361 6e64  t = SPO(len(cand
-0000bd60: 6964 6174 6573 2929 0a20 2020 2020 2020  idates)).       
-0000bd70: 2020 2020 2020 2020 2066 6f72 2065 302c           for e0,
-0000bd80: 6531 2c73 2069 6e20 6564 6765 733a 200a  e1,s in edges: .
+00007320: 2020 2020 2072 705f 6465 6665 6174 2e61       rp_defeat.a
+00007330: 6464 2863 616e 645f 746f 5f63 6964 785b  dd(cand_to_cidx[
+00007340: 6530 5d2c 6361 6e64 5f74 6f5f 6369 6478  e0],cand_to_cidx
+00007350: 5b65 315d 290a 2020 2020 2020 2020 2020  [e1]).          
+00007360: 2020 2020 2020 7769 6e6e 6572 732e 6170        winners.ap
+00007370: 7065 6e64 2863 6964 785f 746f 5f63 616e  pend(cidx_to_can
+00007380: 645b 7270 5f64 6566 6561 742e 696e 6974  d[rp_defeat.init
+00007390: 6961 6c5f 656c 656d 656e 7473 2829 5b30  ial_elements()[0
+000073a0: 5d5d 290a 2020 2020 7265 7475 726e 2073  ]]).    return s
+000073b0: 6f72 7465 6428 6c69 7374 2873 6574 2877  orted(list(set(w
+000073c0: 696e 6e65 7273 2929 290a 0a64 6566 2072  inners)))..def r
+000073d0: 616e 6b65 645f 7061 6972 735f 6465 6665  anked_pairs_defe
+000073e0: 6174 7328 6564 6174 612c 2063 7572 725f  ats(edata, curr_
+000073f0: 6361 6e64 7320 3d20 4e6f 6e65 2c20 7374  cands = None, st
+00007400: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+00007410: 3d20 4e6f 6e65 293a 2020 200a 2020 2020  = None):   .    
+00007420: 2222 220a 2020 2020 5265 7475 726e 7320  """.    Returns 
+00007430: 7468 6520 5261 6e6b 6564 2050 6169 7273  the Ranked Pairs
+00007440: 2064 6566 6561 7420 7265 6c61 7469 6f6e   defeat relation
+00007450: 7320 7072 6f64 7563 6564 2062 7920 7468  s produced by th
+00007460: 6520 5261 6e6b 6564 2050 6169 7273 2061  e Ranked Pairs a
+00007470: 6c67 6f72 6974 686d 2e20 0a0a 2020 2020  lgorithm. ..    
+00007480: 2e2e 2069 6d70 6f72 7461 6e74 3a3a 0a20  .. important::. 
+00007490: 2020 2020 2020 2055 6e6c 696b 6520 7468         Unlike th
+000074a0: 6520 6f74 6865 7220 6675 6e63 7469 6f6e  e other function
+000074b0: 7320 7468 6174 2072 6574 7572 6e20 6120  s that return a 
+000074c0: 7369 6e67 6c65 2064 6566 6561 7420 7265  single defeat re
+000074d0: 6c61 7469 6f6e 2c20 7468 6973 2072 6574  lation, this ret
+000074e0: 7572 6e73 2061 206c 6973 7420 6f66 2064  urns a list of d
+000074f0: 6566 6561 7420 7265 6c61 7469 6f6e 732e  efeat relations.
+00007500: 200a 2020 2020 2020 2020 0a20 2020 2041   .        .    A
+00007510: 7267 733a 0a20 2020 2020 2020 2065 6461  rgs:.        eda
+00007520: 7461 2028 5072 6f66 696c 652c 2050 726f  ta (Profile, Pro
+00007530: 6669 6c65 5769 7468 5469 6573 2c20 4d61  fileWithTies, Ma
+00007540: 7267 696e 4772 6170 6829 3a20 416e 7920  rginGraph): Any 
+00007550: 656c 6563 7469 6f6e 2064 6174 6120 7468  election data th
+00007560: 6174 2068 6173 2061 2060 6d61 7267 696e  at has a `margin
+00007570: 6020 6d65 7468 6f64 2e20 0a20 2020 2020  ` method. .     
+00007580: 2020 2063 7572 725f 6361 6e64 7320 284c     curr_cands (L
+00007590: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
+000075a0: 616c 293a 2049 6620 7365 742c 2074 6865  al): If set, the
+000075b0: 6e20 6669 6e64 2074 6865 2077 696e 6e65  n find the winne
+000075c0: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
+000075d0: 6c65 2072 6573 7472 6963 7465 6420 746f  le restricted to
+000075e0: 2074 6865 2063 616e 6469 6461 7465 7320   the candidates 
+000075f0: 696e 2060 6063 7572 725f 6361 6e64 7360  in ``curr_cands`
+00007600: 600a 2020 2020 2020 2020 7374 7265 6e67  `.        streng
+00007610: 7468 5f66 756e 6374 696f 6e20 2866 756e  th_function (fun
+00007620: 6374 696f 6e2c 206f 7074 696f 6e61 6c29  ction, optional)
+00007630: 3a20 5468 6520 7374 7265 6e67 7468 2066  : The strength f
+00007640: 756e 6374 696f 6e20 746f 2062 6520 7573  unction to be us
+00007650: 6564 2074 6f20 6361 6c63 756c 6174 6520  ed to calculate 
+00007660: 7468 6520 7374 7265 6e67 7468 206f 6620  the strength of 
+00007670: 6120 7061 7468 2e20 2020 5468 6520 6465  a path.   The de
+00007680: 6661 756c 7420 6973 2074 6865 206d 6172  fault is the mar
+00007690: 6769 6e20 6d65 7468 6f64 206f 6620 6060  gin method of ``
+000076a0: 6564 6174 6160 602e 2020 2054 6869 7320  edata``.   This 
+000076b0: 6f6e 6c79 206d 6174 7465 7273 2077 6865  only matters whe
+000076c0: 6e20 7468 6520 6261 6c6c 6f74 7320 6172  n the ballots ar
+000076d0: 6520 6e6f 7420 6c69 6e65 6172 206f 7264  e not linear ord
+000076e0: 6572 732e 200a 0a20 2020 2052 6574 7572  ers. ..    Retur
+000076f0: 6e73 3a20 0a20 2020 2020 2020 2041 206e  ns: .        A n
+00007700: 6574 776f 726b 7820 4469 4772 6170 6820  etworkx DiGraph 
+00007710: 7265 7072 6573 656e 7469 6e67 2074 6865  representing the
+00007720: 2052 616e 6b65 6420 5061 6972 7320 6465   Ranked Pairs de
+00007730: 6665 6174 2072 656c 6174 696f 6e2e 200a  feat relation. .
+00007740: 0a20 2020 202e 2e20 7365 6561 6c73 6f3a  .    .. seealso:
+00007750: 3a0a 0a20 2020 2020 2020 203a 6d65 7468  :..        :meth
+00007760: 3a60 7072 6566 5f76 6f74 696e 672e 6d61  :`pref_voting.ma
+00007770: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+00007780: 6473 2e72 616e 6b65 645f 7061 6972 7360  ds.ranked_pairs`
+00007790: 2c20 3a6d 6574 683a 6070 7265 665f 766f  , :meth:`pref_vo
+000077a0: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+000077b0: 645f 6d65 7468 6f64 732e 7261 6e6b 6564  d_methods.ranked
+000077c0: 5f70 6169 7273 5f77 6974 685f 7465 7374  _pairs_with_test
+000077d0: 600a 0a20 2020 203a 4578 616d 706c 653a  `..    :Example:
+000077e0: 200a 0a20 2020 202e 2e20 706c 6f74 3a3a   ..    .. plot::
+000077f0: 2020 6d61 7267 696e 5f67 7261 7068 735f    margin_graphs_
+00007800: 6578 616d 706c 6573 2f6d 675f 6578 5f72  examples/mg_ex_r
+00007810: 705f 6465 6665 6174 732e 7079 0a20 2020  p_defeats.py.   
+00007820: 2020 2020 203a 636f 6e74 6578 743a 2072       :context: r
+00007830: 6573 6574 2020 0a20 2020 2020 2020 203a  eset  .        :
+00007840: 696e 636c 7564 652d 736f 7572 6365 3a20  include-source: 
+00007850: 5472 7565 0a0a 2020 2020 2e2e 2065 7865  True..    .. exe
+00007860: 635f 636f 6465 3a3a 0a0a 0a20 2020 2020  c_code::...     
+00007870: 2020 2066 726f 6d20 7072 6566 5f76 6f74     from pref_vot
+00007880: 696e 672e 7765 6967 6874 6564 5f6d 616a  ing.weighted_maj
+00007890: 6f72 6974 795f 6772 6170 6873 2069 6d70  ority_graphs imp
+000078a0: 6f72 7420 4d61 7267 696e 4772 6170 680a  ort MarginGraph.
+000078b0: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+000078c0: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+000078d0: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
+000078e0: 706f 7274 2072 616e 6b65 645f 7061 6972  port ranked_pair
+000078f0: 735f 6465 6665 6174 730a 0a20 2020 2020  s_defeats..     
+00007900: 2020 206d 6720 3d20 4d61 7267 696e 4772     mg = MarginGr
+00007910: 6170 6828 5b30 2c20 312c 2032 2c20 335d  aph([0, 1, 2, 3]
+00007920: 2c20 5b28 302c 2031 2c20 3130 292c 2028  , [(0, 1, 10), (
+00007930: 302c 2032 2c20 3229 2c20 2831 2c20 332c  0, 2, 2), (1, 3,
+00007940: 2034 292c 2028 322c 2031 2c20 3629 2c20   4), (2, 1, 6), 
+00007950: 2832 2c20 332c 2038 292c 2028 332c 2030  (2, 3, 8), (3, 0
+00007960: 2c20 3429 5d29 0a20 2020 2020 2020 2072  , 4)]).        r
+00007970: 705f 6465 6665 6174 7320 3d20 7261 6e6b  p_defeats = rank
+00007980: 6564 5f70 6169 7273 5f64 6566 6561 7473  ed_pairs_defeats
+00007990: 286d 6729 0a0a 2020 2020 2020 2020 666f  (mg)..        fo
+000079a0: 7220 7270 6420 696e 2072 705f 6465 6665  r rpd in rp_defe
+000079b0: 6174 733a 200a 2020 2020 2020 2020 2020  ats: .          
+000079c0: 2020 7072 696e 7428 7270 642e 6564 6765    print(rpd.edge
+000079d0: 7329 0a0a 2020 2020 2222 220a 2020 2020  s)..    """.    
+000079e0: 0a20 2020 2063 616e 6469 6461 7465 7320  .    candidates 
+000079f0: 3d20 6564 6174 612e 6361 6e64 6964 6174  = edata.candidat
+00007a00: 6573 2069 6620 6375 7272 5f63 616e 6473  es if curr_cands
+00007a10: 2069 7320 4e6f 6e65 2065 6c73 6520 6375   is None else cu
+00007a20: 7272 5f63 616e 6473 2020 2020 0a20 2020  rr_cands    .   
+00007a30: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00007a40: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
+00007a50: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
+00007a60: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
+00007a70: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
+00007a80: 6374 696f 6e20 2020 200a 0a20 2020 2077  ction    ..    w
+00007a90: 5f65 6467 6573 203d 205b 2863 312c 2063  _edges = [(c1, c
+00007aa0: 322c 2073 7472 656e 6774 685f 6675 6e63  2, strength_func
+00007ab0: 7469 6f6e 2863 312c 2063 3229 2920 666f  tion(c1, c2)) fo
+00007ac0: 7220 6331 2069 6e20 6361 6e64 6964 6174  r c1 in candidat
+00007ad0: 6573 2066 6f72 2063 3220 696e 2063 616e  es for c2 in can
+00007ae0: 6469 6461 7465 7320 6966 2063 3120 213d  didates if c1 !=
+00007af0: 2063 3220 616e 6420 2865 6461 7461 2e6d   c2 and (edata.m
+00007b00: 616a 6f72 6974 795f 7072 6566 6572 7328  ajority_prefers(
+00007b10: 6331 2c20 6332 2920 6f72 2065 6461 7461  c1, c2) or edata
+00007b20: 2e69 735f 7469 6564 2863 312c 2063 3229  .is_tied(c1, c2)
+00007b30: 295d 0a20 2020 2077 696e 6e65 7273 203d  )].    winners =
+00007b40: 206c 6973 7428 2920 2020 2020 2020 2020   list()         
+00007b50: 2020 200a 2020 2020 7374 7265 6e67 7468     .    strength
+00007b60: 7320 3d20 736f 7274 6564 286c 6973 7428  s = sorted(list(
+00007b70: 7365 7428 5b65 5b32 5d20 666f 7220 6520  set([e[2] for e 
+00007b80: 696e 2077 5f65 6467 6573 5d29 292c 2072  in w_edges])), r
+00007b90: 6576 6572 7365 3d54 7275 6529 0a20 2020  everse=True).   
+00007ba0: 2073 6f72 7465 645f 6564 6765 7320 3d20   sorted_edges = 
+00007bb0: 5b5b 6520 666f 7220 6520 696e 2077 5f65  [[e for e in w_e
+00007bc0: 6467 6573 2069 6620 655b 325d 203d 3d20  dges if e[2] == 
+00007bd0: 735d 2066 6f72 2073 2069 6e20 7374 7265  s] for s in stre
+00007be0: 6e67 7468 735d 0a20 2020 2074 6273 203d  ngths].    tbs =
+00007bf0: 2070 726f 6475 6374 282a 5b70 6572 6d75   product(*[permu
+00007c00: 7461 7469 6f6e 7328 6564 6765 7329 2066  tations(edges) f
+00007c10: 6f72 2065 6467 6573 2069 6e20 736f 7274  or edges in sort
+00007c20: 6564 5f65 6467 6573 5d29 0a20 2020 2072  ed_edges]).    r
+00007c30: 705f 6465 6665 6174 7320 3d20 6c69 7374  p_defeats = list
+00007c40: 2829 0a20 2020 2066 6f72 2074 6220 696e  ().    for tb in
+00007c50: 2074 6273 3a0a 2020 2020 2020 2020 6564   tbs:.        ed
+00007c60: 6765 7320 3d20 666c 6174 7465 6e28 7462  ges = flatten(tb
+00007c70: 290a 2020 2020 2020 2020 7270 5f64 6566  ).        rp_def
+00007c80: 6561 7420 3d20 6e78 2e44 6947 7261 7068  eat = nx.DiGraph
+00007c90: 2829 200a 2020 2020 2020 2020 666f 7220  () .        for 
+00007ca0: 6520 696e 2065 6467 6573 3a20 0a20 2020  e in edges: .   
+00007cb0: 2020 2020 2020 2020 2072 705f 6465 6665           rp_defe
+00007cc0: 6174 2e61 6464 5f65 6467 6528 655b 305d  at.add_edge(e[0]
+00007cd0: 2c20 655b 315d 2c20 7765 6967 6874 3d65  , e[1], weight=e
+00007ce0: 5b32 5d29 0a20 2020 2020 2020 2020 2020  [2]).           
+00007cf0: 2069 6620 646f 6573 5f63 7265 6174 655f   if does_create_
+00007d00: 6379 636c 6528 7270 5f64 6566 6561 742c  cycle(rp_defeat,
+00007d10: 2065 293a 0a20 2020 2020 2020 2020 2020   e):.           
+00007d20: 2020 2020 2072 705f 6465 6665 6174 2e72       rp_defeat.r
+00007d30: 656d 6f76 655f 6564 6765 2865 5b30 5d2c  emove_edge(e[0],
+00007d40: 2065 5b31 5d29 0a20 2020 2020 2020 2072   e[1]).        r
+00007d50: 705f 6465 6665 6174 732e 6170 7065 6e64  p_defeats.append
+00007d60: 2872 705f 6465 6665 6174 290a 2020 2020  (rp_defeat).    
+00007d70: 2020 2020 7769 6e6e 6572 732e 6170 7065      winners.appe
+00007d80: 6e64 286d 6178 696d 616c 5f65 6c65 6d65  nd(maximal_eleme
+00007d90: 6e74 7328 7270 5f64 6566 6561 7429 5b30  nts(rp_defeat)[0
+00007da0: 5d29 0a20 2020 2072 6574 7572 6e20 7270  ]).    return rp
+00007db0: 5f64 6566 6561 7473 0a0a 6465 6620 706f  _defeats..def po
+00007dc0: 7765 7273 6574 2869 7465 7261 626c 6529  werset(iterable)
+00007dd0: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
+00007de0: 7475 726e 2074 6865 2070 6f77 6572 7365  turn the powerse
+00007df0: 7420 6f66 2060 6069 7465 7261 626c 6560  t of ``iterable`
+00007e00: 600a 0a20 2020 2070 6f77 6572 7365 7428  `..    powerset(
+00007e10: 5b31 2c32 2c33 5d29 202d 2d3e 2028 2920  [1,2,3]) --> () 
+00007e20: 2831 2c29 2028 322c 2920 2833 2c29 2028  (1,) (2,) (3,) (
+00007e30: 312c 3229 2028 312c 3329 2028 322c 3329  1,2) (1,3) (2,3)
+00007e40: 2028 312c 322c 3329 0a20 2020 2022 2222   (1,2,3).    """
+00007e50: 0a20 2020 2073 203d 206c 6973 7428 6974  .    s = list(it
+00007e60: 6572 6162 6c65 290a 2020 2020 7265 7475  erable).    retu
+00007e70: 726e 2063 6861 696e 2e66 726f 6d5f 6974  rn chain.from_it
+00007e80: 6572 6162 6c65 2863 6f6d 6269 6e61 7469  erable(combinati
+00007e90: 6f6e 7328 732c 2072 2920 666f 7220 7220  ons(s, r) for r 
+00007ea0: 696e 2072 616e 6765 286c 656e 2873 292b  in range(len(s)+
+00007eb0: 3129 290a 0a0a 6465 6620 6973 5f73 7461  1))...def is_sta
+00007ec0: 636b 2865 6461 7461 2c20 6361 6e64 5f6c  ck(edata, cand_l
+00007ed0: 6973 742c 2063 7572 725f 6361 6e64 733d  ist, curr_cands=
+00007ee0: 4e6f 6e65 293a 200a 2020 2020 2222 220a  None): .    """.
+00007ef0: 2020 2020 4120 2a2a 7374 6163 6b2a 2a20      A **stack** 
+00007f00: 6973 2061 206c 696e 6561 7220 6f72 6465  is a linear orde
+00007f10: 7220 3a6d 6174 683a 604c 6020 6f6e 2074  r :math:`L` on t
+00007f20: 6865 2063 616e 6469 6461 7465 2073 7563  he candidate suc
+00007f30: 6820 7468 6174 2066 6f72 2061 6c6c 2063  h that for all c
+00007f40: 616e 6469 6461 7465 7320 3a6d 6174 683a  andidates :math:
+00007f50: 6061 6020 616e 6420 3a6d 6174 683a 6062  `a` and :math:`b
+00007f60: 602c 2069 6620 3a6d 6174 683a 6061 4c62  `, if :math:`aLb
+00007f70: 602c 2074 6865 6e20 7468 6572 6520 6172  `, then there ar
+00007f80: 6520 6469 7374 696e 6374 2063 616e 6469  e distinct candi
+00007f90: 6461 7465 7320 3a6d 6174 683a 6078 5f31  dates :math:`x_1
+00007fa0: 2c5c 646f 7473 2c78 5f6e 6020 7769 7468  ,\dots,x_n` with
+00007fb0: 203a 6d61 7468 3a60 785f 313d 6160 2061   :math:`x_1=a` a
+00007fc0: 6e64 203a 6d61 7468 3a60 785f 6e3d 6260  nd :math:`x_n=b`
+00007fd0: 2073 7563 6820 7468 6174 203a 6d61 7468   such that :math
+00007fe0: 3a60 785f 6920 4c20 785f 7b69 2b31 7d60  :`x_i L x_{i+1}`
+00007ff0: 2061 6e64 2066 6f72 2061 6c6c 203a 6d61   and for all :ma
+00008000: 7468 3a60 695c 696e 205c 7b31 2c5c 646f  th:`i\in \{1,\do
+00008010: 7473 2c20 6e2d 315c 7d60 2c20 7468 6520  ts, n-1\}`, the 
+00008020: 6d61 7267 696e 206f 6620 3a6d 6174 683a  margin of :math:
+00008030: 6078 5f31 6020 6f76 6572 203a 6d61 7468  `x_1` over :math
+00008040: 3a60 785f 7b69 2b31 7d60 2069 7320 6772  :`x_{i+1}` is gr
+00008050: 6561 7465 7220 7468 616e 206f 7220 6571  eater than or eq
+00008060: 7561 6c20 746f 2074 6865 206d 6172 6769  ual to the margi
+00008070: 6e20 6f66 203a 6d61 7468 3a60 6260 206f  n of :math:`b` o
+00008080: 7665 7220 3a6d 6174 683a 6061 602e 0a0a  ver :math:`a`...
+00008090: 2020 2020 5468 6973 2064 6566 696e 6974      This definit
+000080a0: 696f 6e20 6973 2064 7565 2074 6f20 5a61  ion is due to Za
+000080b0: 7669 7374 2061 6e64 2054 6964 656d 616e  vist and Tideman
+000080c0: 2031 3938 392c 2061 6e64 2069 7320 7573   1989, and is us
+000080d0: 6564 2061 7320 616e 2061 6c74 6572 6e61  ed as an alterna
+000080e0: 7469 7665 2063 6861 7261 6374 6572 697a  tive characteriz
+000080f0: 6174 696f 6e20 6f66 2052 616e 6b65 6420  ation of Ranked 
+00008100: 5061 6972 733a 203a 6d61 7468 3a60 6160  Pairs: :math:`a`
+00008110: 2069 7320 6120 5261 6e6b 6564 2050 6169   is a Ranked Pai
+00008120: 7273 2077 696e 6e65 7220 6966 2061 6e64  rs winner if and
+00008130: 206f 6e6c 7920 6966 203a 6d61 7468 3a60   only if :math:`
+00008140: 6160 2069 7320 7468 6520 6d61 7869 6d75  a` is the maximu
+00008150: 6d20 656c 656d 656e 7420 6f66 2073 6f6d  m element of som
+00008160: 6520 7374 6163 6b2e 200a 0a20 2020 2041  e stack. ..    A
+00008170: 7267 733a 0a20 2020 2020 2020 2065 6461  rgs:.        eda
+00008180: 7461 2028 5072 6f66 696c 652c 2050 726f  ta (Profile, Pro
+00008190: 6669 6c65 5769 7468 5469 6573 2c20 4d61  fileWithTies, Ma
+000081a0: 7267 696e 4772 6170 6829 3a20 416e 7920  rginGraph): Any 
+000081b0: 656c 6563 7469 6f6e 2064 6174 6120 7468  election data th
+000081c0: 6174 2068 6173 2061 2060 6d61 7267 696e  at has a `margin
+000081d0: 6020 6d65 7468 6f64 2e20 0a20 2020 2020  ` method. .     
+000081e0: 2020 2063 616e 645f 6c69 7374 2028 6c69     cand_list (li
+000081f0: 7374 293a 2054 6865 206c 6973 7420 6f66  st): The list of
+00008200: 2063 616e 6469 6461 7465 7320 7468 6174   candidates that
+00008210: 206d 6179 2062 6520 6120 7374 6163 6b0a   may be a stack.
+00008220: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
+00008230: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
+00008240: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
+00008250: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
+00008260: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
+00008270: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
+00008280: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
+00008290: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
+000082a0: 616e 6473 6060 0a0a 2020 2020 5265 7475  ands``..    Retu
+000082b0: 726e 733a 200a 2020 2020 2020 2020 5472  rns: .        Tr
+000082c0: 7565 2069 6620 6060 6361 6e64 5f6c 6973  ue if ``cand_lis
+000082d0: 7460 6020 6973 2061 2073 7461 636b 2061  t`` is a stack a
+000082e0: 6e64 2046 616c 7365 206f 7468 6572 7769  nd False otherwi
+000082f0: 7365 0a0a 2020 2020 3a45 7861 6d70 6c65  se..    :Example
+00008300: 3a20 0a20 2020 200a 2020 2020 2e2e 2070  : .    .    .. p
+00008310: 6c6f 743a 3a20 206d 6172 6769 6e5f 6772  lot::  margin_gr
+00008320: 6170 6873 5f65 7861 6d70 6c65 732f 6d67  aphs_examples/mg
+00008330: 5f65 785f 7270 5f73 7461 636b 732e 7079  _ex_rp_stacks.py
+00008340: 0a20 2020 2020 2020 203a 636f 6e74 6578  .        :contex
+00008350: 743a 2072 6573 6574 2020 0a20 2020 2020  t: reset  .     
+00008360: 2020 203a 696e 636c 7564 652d 736f 7572     :include-sour
+00008370: 6365 3a20 5472 7565 0a0a 0a20 2020 202e  ce: True...    .
+00008380: 2e20 6578 6563 5f63 6f64 653a 3a0a 2020  . exec_code::.  
+00008390: 2020 2020 2020 0a20 2020 2020 2020 2066        .        f
+000083a0: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
+000083b0: 7765 6967 6874 6564 5f6d 616a 6f72 6974  weighted_majorit
+000083c0: 795f 6772 6170 6873 2069 6d70 6f72 7420  y_graphs import 
+000083d0: 4d61 7267 696e 4772 6170 680a 2020 2020  MarginGraph.    
+000083e0: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
+000083f0: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+00008400: 645f 6d65 7468 6f64 7320 696d 706f 7274  d_methods import
+00008410: 2069 735f 7374 6163 6b0a 2020 2020 2020   is_stack.      
+00008420: 2020 6672 6f6d 2069 7465 7274 6f6f 6c73    from itertools
+00008430: 2069 6d70 6f72 7420 7065 726d 7574 6174   import permutat
+00008440: 696f 6e73 0a20 2020 2020 2020 200a 2020  ions.        .  
+00008450: 2020 2020 2020 6d67 203d 204d 6172 6769        mg = Margi
+00008460: 6e47 7261 7068 285b 302c 2031 2c20 325d  nGraph([0, 1, 2]
+00008470: 2c20 5b28 302c 2031 2c20 3229 2c20 2831  , [(0, 1, 2), (1
+00008480: 2c20 322c 2034 292c 2028 322c 2030 2c20  , 2, 4), (2, 0, 
+00008490: 3229 5d29 0a20 2020 2020 2020 200a 2020  2)]).        .  
+000084a0: 2020 2020 2020 666f 7220 636c 6973 7420        for clist 
+000084b0: 696e 2070 6572 6d75 7461 7469 6f6e 7328  in permutations(
+000084c0: 6d67 2e63 616e 6469 6461 7465 7329 3a20  mg.candidates): 
+000084d0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+000084e0: 6e74 2866 227b 636c 6973 747d 207b 2769  nt(f"{clist} {'i
+000084f0: 7327 2069 6620 6973 5f73 7461 636b 286d  s' if is_stack(m
+00008500: 672c 2063 6c69 7374 2920 656c 7365 2027  g, clist) else '
+00008510: 6973 206e 6f74 277d 2061 2073 7461 636b  is not'} a stack
+00008520: 2229 0a20 2020 2020 2020 2020 2020 200a  ").            .
+00008530: 2020 2020 2222 220a 2020 2020 0a20 2020      """.    .   
+00008540: 2063 616e 6469 6461 7465 7320 3d20 6375   candidates = cu
+00008550: 7272 5f63 616e 6473 2069 6620 6375 7272  rr_cands if curr
+00008560: 5f63 616e 6473 2069 7320 6e6f 7420 4e6f  _cands is not No
+00008570: 6e65 2065 6c73 6520 6564 6174 612e 6361  ne else edata.ca
+00008580: 6e64 6964 6174 6573 0a20 2020 2063 616e  ndidates.    can
+00008590: 645f 7061 6972 7320 3d20 5b28 612c 2062  d_pairs = [(a, b
+000085a0: 2920 6966 2063 616e 645f 6c69 7374 2e69  ) if cand_list.i
+000085b0: 6e64 6578 2861 2920 3c20 6361 6e64 5f6c  ndex(a) < cand_l
+000085c0: 6973 742e 696e 6465 7828 6229 2065 6c73  ist.index(b) els
+000085d0: 6520 2862 2c20 6129 2066 6f72 2061 2c20  e (b, a) for a, 
+000085e0: 6220 696e 2063 6f6d 6269 6e61 7469 6f6e  b in combination
+000085f0: 7328 6361 6e64 6964 6174 6573 2c20 3229  s(candidates, 2)
+00008600: 5d0a 2020 2020 2020 2020 0a20 2020 2066  ].        .    f
+00008610: 6f72 2061 2c20 6220 696e 2063 616e 645f  or a, b in cand_
+00008620: 7061 6972 733a 0a20 2020 2020 2020 206f  pairs:.        o
+00008630: 7468 6572 5f63 616e 6473 203d 205b 6320  ther_cands = [c 
+00008640: 666f 7220 6320 696e 2063 616e 6469 6461  for c in candida
+00008650: 7465 7320 6966 2063 2021 3d20 6120 616e  tes if c != a an
+00008660: 6420 6320 213d 2062 5d0a 2020 2020 2020  d c != b].      
+00008670: 2020 666f 756e 645f 7061 7468 203d 2046    found_path = F
+00008680: 616c 7365 0a20 2020 2020 2020 200a 2020  alse.        .  
+00008690: 2020 2020 2020 7375 626c 6973 7420 3d20        sublist = 
+000086a0: 6361 6e64 5f6c 6973 745b 6361 6e64 5f6c  cand_list[cand_l
+000086b0: 6973 742e 696e 6465 7828 6129 202b 2031  ist.index(a) + 1
+000086c0: 3a63 616e 645f 6c69 7374 2e69 6e64 6578  :cand_list.index
+000086d0: 2862 295d 0a20 2020 2020 2020 200a 2020  (b)].        .  
+000086e0: 2020 2020 2020 666f 7220 696e 6469 6365        for indice
+000086f0: 7320 696e 2070 6f77 6572 7365 7428 7261  s in powerset(ra
+00008700: 6e67 6528 6c65 6e28 7375 626c 6973 7429  nge(len(sublist)
+00008710: 2929 3a20 0a20 2020 2020 2020 2020 2020  )): .           
+00008720: 200a 2020 2020 2020 2020 2020 2020 7061   .            pa
+00008730: 7468 203d 205b 615d 202b 205b 7375 626c  th = [a] + [subl
+00008740: 6973 745b 695d 2066 6f72 2069 2069 6e20  ist[i] for i in 
+00008750: 736f 7274 6564 2869 6e64 6963 6573 295d  sorted(indices)]
+00008760: 202b 205b 625d 0a20 2020 2020 2020 2020   + [b].         
+00008770: 2020 206d 6172 6769 6e73 203d 205b 6564     margins = [ed
+00008780: 6174 612e 6d61 7267 696e 2878 692c 2070  ata.margin(xi, p
+00008790: 6174 685b 6920 2b20 315d 2920 666f 7220  ath[i + 1]) for 
+000087a0: 692c 2078 6920 696e 2065 6e75 6d65 7261  i, xi in enumera
+000087b0: 7465 2870 6174 685b 303a 2d31 5d29 5d0a  te(path[0:-1])].
+000087c0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+000087d0: 6c6c 285b 6361 6e64 5f6c 6973 742e 696e  ll([cand_list.in
+000087e0: 6465 7828 7869 2920 3c20 6361 6e64 5f6c  dex(xi) < cand_l
+000087f0: 6973 742e 696e 6465 7828 7061 7468 5b69  ist.index(path[i
+00008800: 2b31 5d29 2066 6f72 2069 2c20 7869 2069  +1]) for i, xi i
+00008810: 6e20 656e 756d 6572 6174 6528 7061 7468  n enumerate(path
+00008820: 5b30 3a2d 315d 295d 2920 616e 6420 616c  [0:-1])]) and al
+00008830: 6c28 5b6d 203e 3d20 6564 6174 612e 6d61  l([m >= edata.ma
+00008840: 7267 696e 2862 2c20 6129 2066 6f72 206d  rgin(b, a) for m
+00008850: 2069 6e20 6d61 7267 696e 735d 293a 200a   in margins]): .
+00008860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008870: 666f 756e 645f 7061 7468 203d 2054 7275  found_path = Tru
+00008880: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00008890: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+000088a0: 6966 206e 6f74 2066 6f75 6e64 5f70 6174  if not found_pat
+000088b0: 683a 200a 2020 2020 2020 2020 2020 2020  h: .            
+000088c0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+000088d0: 2072 6574 7572 6e20 5472 7565 0a0a 4076   return True..@v
+000088e0: 6d28 6e61 6d65 3d22 5261 6e6b 6564 2050  m(name="Ranked P
+000088f0: 6169 7273 2229 0a64 6566 2072 616e 6b65  airs").def ranke
+00008900: 645f 7061 6972 735f 6672 6f6d 5f73 7461  d_pairs_from_sta
+00008910: 636b 7328 6564 6174 612c 2063 7572 725f  cks(edata, curr_
+00008920: 6361 6e64 7320 3d20 4e6f 6e65 293a 200a  cands = None): .
+00008930: 2020 2020 2222 2246 696e 6420 7468 6520      """Find the 
+00008940: 5261 6e6b 6564 2050 6169 7273 2077 696e  Ranked Pairs win
+00008950: 6e65 7273 2062 7920 6974 6572 6174 696e  ners by iteratin
+00008960: 6720 6f76 6572 2061 6c6c 2070 6572 6d75  g over all permu
+00008970: 7461 7469 6f6e 7320 6f66 2063 616e 6469  tations of candi
+00008980: 6461 7465 7320 2872 6573 7472 6963 7465  dates (restricte
+00008990: 6420 746f 2060 6063 7572 725f 6361 6e64  d to ``curr_cand
+000089a0: 7360 6020 6966 206e 6f74 204e 6f6e 6529  s`` if not None)
+000089b0: 2c20 616e 6420 6368 6563 6b69 6e67 2069  , and checking i
+000089c0: 6620 7468 6520 6c69 7374 2069 7320 6120  f the list is a 
+000089d0: 7374 6163 6b2e 200a 0a20 2020 2041 7267  stack. ..    Arg
+000089e0: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
+000089f0: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
+00008a00: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
+00008a10: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
+00008a20: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
+00008a30: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
+00008a40: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
+00008a50: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
+00008a60: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
+00008a70: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
+00008a80: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
+00008a90: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
+00008aa0: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
+00008ab0: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
+00008ac0: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
+00008ad0: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
+00008ae0: 2020 2020 2020 2041 2073 6f72 7465 6420         A sorted 
+00008af0: 6c69 7374 206f 6620 6361 6e64 6964 6174  list of candidat
+00008b00: 6573 2e20 0a0a 2020 2020 2e2e 2073 6565  es. ..    .. see
+00008b10: 616c 736f 3a3a 0a0a 2020 2020 2020 2020  also::..        
+00008b20: 3a6d 6574 683a 6070 7265 665f 766f 7469  :meth:`pref_voti
+00008b30: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
+00008b40: 6d65 7468 6f64 732e 7261 6e6b 6564 5f70  methods.ranked_p
+00008b50: 6169 7273 602c 203a 6d65 7468 3a60 7072  airs`, :meth:`pr
+00008b60: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+00008b70: 5f62 6173 6564 5f6d 6574 686f 6473 2e69  _based_methods.i
+00008b80: 735f 7374 6163 6b60 0a0a 2020 2020 3a45  s_stack`..    :E
+00008b90: 7861 6d70 6c65 3a20 0a0a 2020 2020 2e2e  xample: ..    ..
+00008ba0: 2070 6c6f 743a 3a20 206d 6172 6769 6e5f   plot::  margin_
+00008bb0: 6772 6170 6873 5f65 7861 6d70 6c65 732f  graphs_examples/
+00008bc0: 6d67 5f65 785f 6270 5f72 702e 7079 0a20  mg_ex_bp_rp.py. 
+00008bd0: 2020 2020 2020 203a 636f 6e74 6578 743a         :context:
+00008be0: 2072 6573 6574 2020 0a20 2020 2020 2020   reset  .       
+00008bf0: 203a 696e 636c 7564 652d 736f 7572 6365   :include-source
+00008c00: 3a20 5472 7565 0a0a 0a20 2020 202e 2e20  : True...    .. 
+00008c10: 636f 6465 2d62 6c6f 636b 3a3a 200a 0a20  code-block:: .. 
+00008c20: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
+00008c30: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+00008c40: 6173 6564 5f6d 6574 686f 6473 2069 6d70  ased_methods imp
+00008c50: 6f72 7420 7261 6e6b 6564 5f70 6169 7273  ort ranked_pairs
+00008c60: 2c20 7261 6e6b 6564 5f70 6169 7273 5f66  , ranked_pairs_f
+00008c70: 726f 6d5f 7374 6163 6b73 0a0a 2020 2020  rom_stacks..    
+00008c80: 2020 2020 7261 6e6b 6564 5f70 6169 7273      ranked_pairs
+00008c90: 2e64 6973 706c 6179 286d 6729 0a20 2020  .display(mg).   
+00008ca0: 2020 2020 2072 616e 6b65 645f 7061 6972       ranked_pair
+00008cb0: 735f 6672 6f6d 5f73 7461 636b 732e 6469  s_from_stacks.di
+00008cc0: 7370 6c61 7928 6d67 290a 0a0a 2020 2020  splay(mg)...    
+00008cd0: 2e2e 2065 7865 635f 636f 6465 3a3a 200a  .. exec_code:: .
+00008ce0: 2020 2020 2020 2020 3a68 6964 655f 636f          :hide_co
+00008cf0: 6465 3a0a 0a20 2020 2020 2020 2066 726f  de:..        fro
+00008d00: 6d20 7072 6566 5f76 6f74 696e 672e 7765  m pref_voting.we
+00008d10: 6967 6874 6564 5f6d 616a 6f72 6974 795f  ighted_majority_
+00008d20: 6772 6170 6873 2069 6d70 6f72 7420 4d61  graphs import Ma
+00008d30: 7267 696e 4772 6170 680a 2020 2020 2020  rginGraph.      
+00008d40: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
+00008d50: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
+00008d60: 6d65 7468 6f64 7320 696d 706f 7274 2072  methods import r
+00008d70: 616e 6b65 645f 7061 6972 732c 2072 616e  anked_pairs, ran
+00008d80: 6b65 645f 7061 6972 735f 6672 6f6d 5f73  ked_pairs_from_s
+00008d90: 7461 636b 730a 2020 2020 2020 2020 0a20  tacks.        . 
+00008da0: 2020 2020 2020 206d 6720 3d20 4d61 7267         mg = Marg
+00008db0: 696e 4772 6170 6828 5b30 2c20 312c 2032  inGraph([0, 1, 2
+00008dc0: 2c20 335d 2c20 5b28 302c 2032 2c20 3329  , 3], [(0, 2, 3)
+00008dd0: 2c20 2831 2c20 302c 2035 292c 2028 322c  , (1, 0, 5), (2,
+00008de0: 2031 2c20 3529 2c20 2832 2c20 332c 2031   1, 5), (2, 3, 1
+00008df0: 292c 2028 332c 2030 2c20 3329 2c20 2833  ), (3, 0, 3), (3
+00008e00: 2c20 312c 2031 295d 290a 0a20 2020 2020  , 1, 1)])..     
+00008e10: 2020 2072 616e 6b65 645f 7061 6972 732e     ranked_pairs.
+00008e20: 6469 7370 6c61 7928 6d67 290a 2020 2020  display(mg).    
+00008e30: 2020 2020 7261 6e6b 6564 5f70 6169 7273      ranked_pairs
+00008e40: 5f66 726f 6d5f 7374 6163 6b73 2e64 6973  _from_stacks.dis
+00008e50: 706c 6179 286d 6729 0a0a 2020 2020 2222  play(mg)..    ""
+00008e60: 2220 2020 200a 0a20 2020 2063 616e 6469  "    ..    candi
+00008e70: 6461 7465 7320 3d20 6375 7272 5f63 616e  dates = curr_can
+00008e80: 6473 2069 6620 6375 7272 5f63 616e 6473  ds if curr_cands
+00008e90: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
+00008ea0: 6520 6564 6174 612e 6361 6e64 6964 6174  e edata.candidat
+00008eb0: 6573 0a20 2020 2077 696e 6e65 7273 203d  es.    winners =
+00008ec0: 206c 6973 7428 290a 2020 2020 666f 7220   list().    for 
+00008ed0: 636c 6973 7420 696e 2070 6572 6d75 7461  clist in permuta
+00008ee0: 7469 6f6e 7328 6361 6e64 6964 6174 6573  tions(candidates
+00008ef0: 293a 200a 2020 2020 2020 2020 6973 7374  ): .        isst
+00008f00: 6163 6b20 3d20 6973 5f73 7461 636b 2865  ack = is_stack(e
+00008f10: 6461 7461 2c20 636c 6973 742c 2063 7572  data, clist, cur
+00008f20: 725f 6361 6e64 7320 3d20 6375 7272 5f63  r_cands = curr_c
+00008f30: 616e 6473 290a 2020 2020 2020 2020 6966  ands).        if
+00008f40: 2069 7373 7461 636b 3a20 0a20 2020 2020   isstack: .     
+00008f50: 2020 2020 2020 2077 696e 6e65 7273 2e61         winners.a
+00008f60: 7070 656e 6428 636c 6973 745b 305d 290a  ppend(clist[0]).
+00008f70: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00008f80: 2072 6574 7572 6e20 736f 7274 6564 286c   return sorted(l
+00008f90: 6973 7428 7365 7428 7769 6e6e 6572 7329  ist(set(winners)
+00008fa0: 2929 0a0a 4076 6d28 6e61 6d65 3d22 5261  ))..@vm(name="Ra
+00008fb0: 6e6b 6564 2050 6169 7273 2054 4222 290a  nked Pairs TB").
+00008fc0: 6465 6620 7261 6e6b 6564 5f70 6169 7273  def ranked_pairs
+00008fd0: 5f74 6228 6564 6174 612c 2063 7572 725f  _tb(edata, curr_
+00008fe0: 6361 6e64 7320 3d20 4e6f 6e65 2c20 7469  cands = None, ti
+00008ff0: 655f 6272 6561 6b65 7220 3d20 4e6f 6e65  e_breaker = None
+00009000: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+00009010: 696f 6e20 3d20 4e6f 6e65 293a 2020 200a  ion = None):   .
+00009020: 2020 2020 2222 220a 2020 2020 5261 6e6b      """.    Rank
+00009030: 6564 2050 6169 7273 2077 6974 6820 6120  ed Pairs with a 
+00009040: 6669 7865 6420 6c69 6e65 6172 206f 7264  fixed linear ord
+00009050: 6572 206f 6e20 7468 6520 6361 6e64 6964  er on the candid
+00009060: 6174 6573 2074 6f20 6272 6561 6b20 616e  ates to break an
+00009070: 7920 7469 6573 2069 6e20 7468 6520 6d61  y ties in the ma
+00009080: 7267 696e 732e 2020 200a 2020 2020 5369  rgins.   .    Si
+00009090: 6e63 6520 7468 6520 7469 655f 6272 6561  nce the tie_brea
+000090a0: 6b65 7220 6973 2061 206c 696e 6561 7220  ker is a linear 
+000090b0: 6f72 6465 722c 2074 6869 7320 6d65 7468  order, this meth
+000090c0: 6f64 2069 7320 7265 736f 6c75 7465 2e20  od is resolute. 
+000090d0: 2020 0a0a 2020 2020 4172 6773 3a0a 2020    ..    Args:.  
+000090e0: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
+000090f0: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
+00009100: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
+00009110: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
+00009120: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
+00009130: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
+00009140: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
+00009150: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
+00009160: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
+00009170: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
+00009180: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
+00009190: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
+000091a0: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
+000091b0: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
+000091c0: 7272 5f63 616e 6473 6060 0a20 2020 2020  rr_cands``.     
+000091d0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+000091e0: 7469 6f6e 2028 6675 6e63 7469 6f6e 2c20  tion (function, 
+000091f0: 6f70 7469 6f6e 616c 293a 2054 6865 2073  optional): The s
+00009200: 7472 656e 6774 6820 6675 6e63 7469 6f6e  trength function
+00009210: 2074 6f20 6265 2075 7365 6420 746f 2063   to be used to c
+00009220: 616c 6375 6c61 7465 2074 6865 2073 7472  alculate the str
+00009230: 656e 6774 6820 6f66 2061 2070 6174 682e  ength of a path.
+00009240: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
+00009250: 7320 7468 6520 6d61 7267 696e 206d 6574  s the margin met
+00009260: 686f 6420 6f66 2060 6065 6461 7461 6060  hod of ``edata``
+00009270: 2e20 2020 5468 6973 206f 6e6c 7920 6d61  .   This only ma
+00009280: 7474 6572 7320 7768 656e 2074 6865 2062  tters when the b
+00009290: 616c 6c6f 7473 2061 7265 206e 6f74 206c  allots are not l
+000092a0: 696e 6561 7220 6f72 6465 7273 2e20 0a0a  inear orders. ..
+000092b0: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
+000092c0: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
+000092d0: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
+000092e0: 732e 200a 0a20 2020 202e 2e20 7365 6561  s. ..    .. seea
+000092f0: 6c73 6f3a 3a0a 0a20 2020 2020 2020 203a  lso::..        :
+00009300: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
+00009310: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
+00009320: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
+00009330: 6972 7360 2c20 3a6d 6574 683a 6070 7265  irs`, :meth:`pre
+00009340: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+00009350: 6261 7365 645f 6d65 7468 6f64 732e 7261  based_methods.ra
+00009360: 6e6b 6564 5f70 6169 7273 5f77 6974 685f  nked_pairs_with_
+00009370: 7465 7374 602c 203a 6d65 7468 3a60 7072  test`, :meth:`pr
+00009380: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+00009390: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
+000093a0: 616e 6b65 645f 7061 6972 735f 6672 6f6d  anked_pairs_from
+000093b0: 5f73 7461 636b 7360 0a0a 2020 2020 2e2e  _stacks`..    ..
+000093c0: 2065 7865 635f 636f 6465 3a3a 0a0a 2020   exec_code::..  
+000093d0: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+000093e0: 766f 7469 6e67 2e70 726f 6669 6c65 7320  voting.profiles 
+000093f0: 696d 706f 7274 2050 726f 6669 6c65 0a20  import Profile. 
+00009400: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
+00009410: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+00009420: 6173 6564 5f6d 6574 686f 6473 2069 6d70  ased_methods imp
+00009430: 6f72 7420 7261 6e6b 6564 5f70 6169 7273  ort ranked_pairs
+00009440: 5f66 726f 6d5f 7374 6163 6b73 2c20 7261  _from_stacks, ra
+00009450: 6e6b 6564 5f70 6169 7273 5f74 622c 2072  nked_pairs_tb, r
+00009460: 616e 6b65 645f 7061 6972 735f 7a74 0a0a  anked_pairs_zt..
+00009470: 2020 2020 2020 2020 7072 6f66 203d 2050          prof = P
+00009480: 726f 6669 6c65 285b 5b32 2c20 332c 2031  rofile([[2, 3, 1
+00009490: 2c20 305d 2c20 5b30 2c20 332c 2031 2c20  , 0], [0, 3, 1, 
+000094a0: 325d 2c20 5b31 2c20 332c 2032 2c20 305d  2], [1, 3, 2, 0]
+000094b0: 2c20 5b32 2c20 312c 2033 2c20 305d 5d2c  , [2, 1, 3, 0]],
+000094c0: 205b 312c 2031 2c20 312c 2031 5d29 0a0a   [1, 1, 1, 1])..
+000094d0: 2020 2020 2020 2020 7072 6f66 2e64 6973          prof.dis
+000094e0: 706c 6179 2829 0a0a 2020 2020 2020 2020  play()..        
+000094f0: 7261 6e6b 6564 5f70 6169 7273 5f66 726f  ranked_pairs_fro
+00009500: 6d5f 7374 6163 6b73 2e64 6973 706c 6179  m_stacks.display
+00009510: 2870 726f 6629 0a20 2020 2020 2020 2072  (prof).        r
+00009520: 616e 6b65 645f 7061 6972 735f 7462 2e64  anked_pairs_tb.d
+00009530: 6973 706c 6179 2870 726f 6629 0a20 2020  isplay(prof).   
+00009540: 2020 2020 2072 616e 6b65 645f 7061 6972       ranked_pair
+00009550: 735f 7462 2e64 6973 706c 6179 2870 726f  s_tb.display(pro
+00009560: 662c 2074 6965 5f62 7265 616b 6572 203d  f, tie_breaker =
+00009570: 205b 332c 2032 2c20 312c 2030 5d29 0a20   [3, 2, 1, 0]). 
+00009580: 2020 2020 2020 2072 616e 6b65 645f 7061         ranked_pa
+00009590: 6972 735f 7a74 2e64 6973 706c 6179 2870  irs_zt.display(p
+000095a0: 726f 6629 0a0a 2020 2020 2222 220a 0a20  rof)..    """.. 
+000095b0: 2020 2063 616e 6469 6461 7465 7320 3d20     candidates = 
+000095c0: 6564 6174 612e 6361 6e64 6964 6174 6573  edata.candidates
+000095d0: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
+000095e0: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
+000095f0: 5f63 616e 6473 2020 2020 0a20 2020 2063  _cands    .    c
+00009600: 6964 785f 746f 5f63 616e 6420 3d20 7b63  idx_to_cand = {c
+00009610: 6964 783a 2063 2066 6f72 2063 6964 782c  idx: c for cidx,
+00009620: 2063 2069 6e20 656e 756d 6572 6174 6528   c in enumerate(
+00009630: 6361 6e64 6964 6174 6573 297d 2020 0a20  candidates)}  . 
+00009640: 2020 2063 616e 645f 746f 5f63 6964 7820     cand_to_cidx 
+00009650: 3d20 7b63 3a20 6369 6478 2066 6f72 2063  = {c: cidx for c
+00009660: 6964 782c 2063 2069 6e20 656e 756d 6572  idx, c in enumer
+00009670: 6174 6528 6361 6e64 6964 6174 6573 297d  ate(candidates)}
+00009680: 2020 0a0a 2020 2020 7374 7265 6e67 7468    ..    strength
+00009690: 5f66 756e 6374 696f 6e20 3d20 6564 6174  _function = edat
+000096a0: 612e 6d61 7267 696e 2069 6620 7374 7265  a.margin if stre
+000096b0: 6e67 7468 5f66 756e 6374 696f 6e20 6973  ngth_function is
+000096c0: 204e 6f6e 6520 656c 7365 2073 7472 656e   None else stren
+000096d0: 6774 685f 6675 6e63 7469 6f6e 0a20 2020  gth_function.   
+000096e0: 200a 2020 2020 7462 5f72 616e 6b69 6e67   .    tb_ranking
+000096f0: 203d 2074 6965 5f62 7265 616b 6572 2069   = tie_breaker i
+00009700: 6620 7469 655f 6272 6561 6b65 7220 6973  f tie_breaker is
+00009710: 206e 6f74 204e 6f6e 6520 656c 7365 2073   not None else s
+00009720: 6f72 7465 6428 6c69 7374 2863 616e 6469  orted(list(candi
+00009730: 6461 7465 7329 290a 0a20 2020 2063 7720  dates))..    cw 
+00009740: 3d20 6564 6174 612e 636f 6e64 6f72 6365  = edata.condorce
+00009750: 745f 7769 6e6e 6572 2863 7572 725f 6361  t_winner(curr_ca
+00009760: 6e64 733d 6375 7272 5f63 616e 6473 290a  nds=curr_cands).
+00009770: 2020 2020 2320 5261 6e6b 6564 2050 6169      # Ranked Pai
+00009780: 7273 2069 7320 436f 6e64 6f72 6365 7420  rs is Condorcet 
+00009790: 636f 6e73 6973 7465 6e74 2c20 736f 2073  consistent, so s
+000097a0: 696d 706c 7920 7265 7475 726e 2074 6865  imply return the
+000097b0: 2043 6f6e 646f 7263 6574 2077 696e 6e65   Condorcet winne
+000097c0: 7220 6966 2065 7869 7374 730a 2020 2020  r if exists.    
+000097d0: 6966 2063 7720 6973 206e 6f74 204e 6f6e  if cw is not Non
+000097e0: 653a 200a 2020 2020 2020 2020 7769 6e6e  e: .        winn
+000097f0: 6572 7320 3d20 5b63 775d 0a20 2020 2065  ers = [cw].    e
+00009800: 6c73 653a 0a20 2020 2020 2020 2077 5f65  lse:.        w_e
+00009810: 6467 6573 203d 205b 2863 312c 2063 322c  dges = [(c1, c2,
+00009820: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00009830: 6f6e 2863 312c 2063 3229 2920 666f 7220  on(c1, c2)) for 
+00009840: 6331 2069 6e20 6361 6e64 6964 6174 6573  c1 in candidates
+00009850: 2066 6f72 2063 3220 696e 2063 616e 6469   for c2 in candi
+00009860: 6461 7465 7320 0a20 2020 2020 2020 2020  dates .         
+00009870: 2020 2020 2020 2020 2020 6966 2063 3120            if c1 
+00009880: 213d 2063 3220 616e 6420 2865 6461 7461  != c2 and (edata
+00009890: 2e6d 616a 6f72 6974 795f 7072 6566 6572  .majority_prefer
+000098a0: 7328 6331 2c20 6332 2920 6f72 2065 6461  s(c1, c2) or eda
+000098b0: 7461 2e69 735f 7469 6564 2863 312c 2063  ta.is_tied(c1, c
+000098c0: 3229 295d 0a20 2020 2020 2020 2077 696e  2))].        win
+000098d0: 6e65 7273 203d 206c 6973 7428 2920 2020  ners = list()   
+000098e0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+000098f0: 2020 7374 7265 6e67 7468 7320 3d20 736f    strengths = so
+00009900: 7274 6564 286c 6973 7428 7365 7428 5b65  rted(list(set([e
+00009910: 5b32 5d20 666f 7220 6520 696e 2077 5f65  [2] for e in w_e
+00009920: 6467 6573 5d29 292c 2072 6576 6572 7365  dges])), reverse
+00009930: 3d54 7275 6529 0a20 2020 2020 2020 200a  =True).        .
+00009940: 2020 2020 2020 2020 7270 5f64 6566 6561          rp_defea
+00009950: 7420 3d20 5350 4f28 6c65 6e28 6361 6e64  t = SPO(len(cand
+00009960: 6964 6174 6573 2929 0a0a 2020 2020 2020  idates))..      
+00009970: 2020 666f 7220 7320 696e 2073 7472 656e    for s in stren
+00009980: 6774 6873 3a20 0a20 2020 2020 2020 2020  gths: .         
+00009990: 2020 2065 6467 6573 203d 205b 6520 666f     edges = [e fo
+000099a0: 7220 6520 696e 2077 5f65 6467 6573 2069  r e in w_edges i
+000099b0: 6620 655b 325d 203d 3d20 735d 0a20 2020  f e[2] == s].   
+000099c0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+000099d0: 2020 2020 2020 2320 6272 6561 6b20 7469        # break ti
+000099e0: 6573 2075 7369 6e67 2074 6865 206c 6578  es using the lex
+000099f0: 6963 6f67 7261 7068 6963 206f 7264 6572  icographic order
+00009a00: 696e 6720 6f6e 2074 7570 6c65 7320 6769  ing on tuples gi
+00009a10: 7665 6e20 7462 5f72 616e 6b69 6e67 0a20  ven tb_ranking. 
+00009a20: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
+00009a30: 645f 6564 6765 7320 3d20 736f 7274 6564  d_edges = sorted
+00009a40: 2865 6467 6573 2c20 6b65 7920 3d20 6c61  (edges, key = la
+00009a50: 6d62 6461 2065 3a20 2874 625f 7261 6e6b  mbda e: (tb_rank
+00009a60: 696e 672e 696e 6465 7828 655b 305d 292c  ing.index(e[0]),
+00009a70: 2074 625f 7261 6e6b 696e 672e 696e 6465   tb_ranking.inde
+00009a80: 7828 655b 315d 2929 2c20 7265 7665 7273  x(e[1])), revers
+00009a90: 653d 4661 6c73 6529 0a20 2020 2020 2020  e=False).       
+00009aa0: 2020 2020 2066 6f72 2065 302c 6531 2c73       for e0,e1,s
+00009ab0: 2069 6e20 6564 6765 733a 200a 2020 2020   in edges: .    
+00009ac0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00009ad0: 6f74 2072 705f 6465 6665 6174 2e50 5b63  ot rp_defeat.P[c
+00009ae0: 616e 645f 746f 5f63 6964 785b 6531 5d5d  and_to_cidx[e1]]
+00009af0: 5b63 616e 645f 746f 5f63 6964 785b 6530  [cand_to_cidx[e0
+00009b00: 5d5d 3a0a 2020 2020 2020 2020 2020 2020  ]]:.            
+00009b10: 2020 2020 2020 2020 7270 5f64 6566 6561          rp_defea
+00009b20: 742e 6164 6428 6361 6e64 5f74 6f5f 6369  t.add(cand_to_ci
+00009b30: 6478 5b65 305d 2c63 616e 645f 746f 5f63  dx[e0],cand_to_c
+00009b40: 6964 785b 6531 5d29 0a20 2020 2020 2020  idx[e1]).       
+00009b50: 2020 2020 2077 696e 6e65 7273 2e61 7070       winners.app
+00009b60: 656e 6428 6369 6478 5f74 6f5f 6361 6e64  end(cidx_to_cand
+00009b70: 5b72 705f 6465 6665 6174 2e69 6e69 7469  [rp_defeat.initi
+00009b80: 616c 5f65 6c65 6d65 6e74 7328 295b 305d  al_elements()[0]
+00009b90: 5d29 0a0a 2020 2020 7265 7475 726e 2073  ])..    return s
+00009ba0: 6f72 7465 6428 6c69 7374 2873 6574 2877  orted(list(set(w
+00009bb0: 696e 6e65 7273 2929 290a 0a0a 4076 6d28  inners)))...@vm(
+00009bc0: 6e61 6d65 3d22 5261 6e6b 6564 2050 6169  name="Ranked Pai
+00009bd0: 7273 205a 5422 290a 6465 6620 7261 6e6b  rs ZT").def rank
+00009be0: 6564 5f70 6169 7273 5f7a 7428 7072 6f66  ed_pairs_zt(prof
+00009bf0: 696c 652c 2063 7572 725f 6361 6e64 7320  ile, curr_cands 
+00009c00: 3d20 4e6f 6e65 2c20 7374 7265 6e67 7468  = None, strength
+00009c10: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
+00009c20: 293a 2020 200a 2020 2020 2222 2252 616e  ):   .    """Ran
+00009c30: 6b65 6420 7061 6972 7320 7768 6572 6520  ked pairs where 
+00009c40: 6120 6669 7865 6420 766f 7465 7220 6272  a fixed voter br
+00009c50: 6561 6b73 2061 6e79 2074 6965 7320 696e  eaks any ties in
+00009c60: 2074 6865 206d 6172 6769 6e73 2e20 2049   the margins.  I
+00009c70: 7420 6973 2061 6c77 6179 7320 7468 6520  t is always the 
+00009c80: 766f 7465 7220 696e 2070 6f73 6974 696f  voter in positio
+00009c90: 6e20 3020 7468 6174 2062 7265 616b 7320  n 0 that breaks 
+00009ca0: 7468 6520 7469 6573 2e20 2053 696e 6365  the ties.  Since
+00009cb0: 2076 6f74 6572 7320 6861 7665 2073 7472   voters have str
+00009cc0: 6963 7420 7072 6566 6572 656e 6365 732c  ict preferences,
+00009cd0: 2074 6869 7320 6d65 7468 6f64 2069 7320   this method is 
+00009ce0: 7265 736f 6c75 7465 2e20 2054 6869 7320  resolute.  This 
+00009cf0: 6973 206b 6e6f 776e 2061 7320 5261 6e6b  is known as Rank
+00009d00: 6564 2050 6169 7273 205a 542c 2066 6f72  ed Pairs ZT, for
+00009d10: 205a 6176 6973 7420 5469 6465 6d61 6e2e   Zavist Tideman.
+00009d20: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00009d30: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
+00009d40: 6c65 293a 2041 2070 726f 6669 6c65 206f  le): A profile o
+00009d50: 6620 6c69 6e65 6172 206f 7264 6572 730a  f linear orders.
+00009d60: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
+00009d70: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
+00009d80: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
+00009d90: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
+00009da0: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
+00009db0: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
+00009dc0: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
+00009dd0: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
+00009de0: 616e 6473 6060 0a0a 2020 2020 5265 7475  ands``..    Retu
+00009df0: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
+00009e00: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
+00009e10: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
+00009e20: 202e 2e20 7365 6561 6c73 6f3a 3a0a 0a20   .. seealso::.. 
+00009e30: 2020 2020 2020 203a 6d65 7468 3a60 7072         :meth:`pr
+00009e40: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+00009e50: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
+00009e60: 616e 6b65 645f 7061 6972 7360 2c20 3a6d  anked_pairs`, :m
+00009e70: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
+00009e80: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+00009e90: 7468 6f64 732e 7261 6e6b 6564 5f70 6169  thods.ranked_pai
+00009ea0: 7273 5f77 6974 685f 7465 7374 602c 203a  rs_with_test`, :
+00009eb0: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
+00009ec0: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
+00009ed0: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
+00009ee0: 6972 735f 6672 6f6d 5f73 7461 636b 7360  irs_from_stacks`
+00009ef0: 0a0a 2020 2020 2e2e 2065 7865 635f 636f  ..    .. exec_co
+00009f00: 6465 3a3a 0a0a 2020 2020 2020 2020 6672  de::..        fr
+00009f10: 6f6d 2070 7265 665f 766f 7469 6e67 2e70  om pref_voting.p
+00009f20: 726f 6669 6c65 7320 696d 706f 7274 2050  rofiles import P
+00009f30: 726f 6669 6c65 0a20 2020 2020 2020 2066  rofile.        f
+00009f40: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
+00009f50: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+00009f60: 686f 6473 2069 6d70 6f72 7420 7261 6e6b  hods import rank
+00009f70: 6564 5f70 6169 7273 5f66 726f 6d5f 7374  ed_pairs_from_st
+00009f80: 6163 6b73 2c20 7261 6e6b 6564 5f70 6169  acks, ranked_pai
+00009f90: 7273 5f74 622c 2072 616e 6b65 645f 7061  rs_tb, ranked_pa
+00009fa0: 6972 735f 7a74 0a0a 2020 2020 2020 2020  irs_zt..        
+00009fb0: 7072 6f66 203d 2050 726f 6669 6c65 285b  prof = Profile([
+00009fc0: 5b32 2c20 332c 2031 2c20 305d 2c20 5b30  [2, 3, 1, 0], [0
+00009fd0: 2c20 332c 2031 2c20 325d 2c20 5b31 2c20  , 3, 1, 2], [1, 
+00009fe0: 332c 2032 2c20 305d 2c20 5b32 2c20 312c  3, 2, 0], [2, 1,
+00009ff0: 2033 2c20 305d 5d2c 205b 312c 2031 2c20   3, 0]], [1, 1, 
+0000a000: 312c 2031 5d29 0a0a 2020 2020 2020 2020  1, 1])..        
+0000a010: 7072 6f66 2e64 6973 706c 6179 2829 0a0a  prof.display()..
+0000a020: 2020 2020 2020 2020 7261 6e6b 6564 5f70          ranked_p
+0000a030: 6169 7273 5f66 726f 6d5f 7374 6163 6b73  airs_from_stacks
+0000a040: 2e64 6973 706c 6179 2870 726f 6629 0a20  .display(prof). 
+0000a050: 2020 2020 2020 2072 616e 6b65 645f 7061         ranked_pa
+0000a060: 6972 735f 7462 2e64 6973 706c 6179 2870  irs_tb.display(p
+0000a070: 726f 6629 0a20 2020 2020 2020 2072 616e  rof).        ran
+0000a080: 6b65 645f 7061 6972 735f 7462 2e64 6973  ked_pairs_tb.dis
+0000a090: 706c 6179 2870 726f 662c 2074 6965 5f62  play(prof, tie_b
+0000a0a0: 7265 616b 6572 203d 205b 332c 2032 2c20  reaker = [3, 2, 
+0000a0b0: 312c 2030 5d29 0a20 2020 2020 2020 2072  1, 0]).        r
+0000a0c0: 616e 6b65 645f 7061 6972 735f 7a74 2e64  anked_pairs_zt.d
+0000a0d0: 6973 706c 6179 2870 726f 6629 0a0a 2020  isplay(prof)..  
+0000a0e0: 2020 0a20 2020 2022 2222 0a20 2020 2063    .    """.    c
+0000a0f0: 616e 6469 6461 7465 7320 3d20 7072 6f66  andidates = prof
+0000a100: 696c 652e 6361 6e64 6964 6174 6573 2069  ile.candidates i
+0000a110: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
+0000a120: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
+0000a130: 616e 6473 2020 2020 0a20 2020 200a 2020  ands    .    .  
+0000a140: 2020 2320 7468 6520 7469 652d 6272 6561    # the tie-brea
+0000a150: 6b65 7220 6973 2061 6c77 6179 7320 7468  ker is always th
+0000a160: 6520 6669 7273 7420 766f 7465 722e 200a  e first voter. .
+0000a170: 2020 2020 7462 5f72 616e 6b69 6e67 203d      tb_ranking =
+0000a180: 2074 7570 6c65 285b 6320 666f 7220 6320   tuple([c for c 
+0000a190: 696e 206c 6973 7428 7072 6f66 696c 652e  in list(profile.
+0000a1a0: 5f72 616e 6b69 6e67 735b 305d 2920 6966  _rankings[0]) if
+0000a1b0: 2063 2069 6e20 6361 6e64 6964 6174 6573   c in candidates
+0000a1c0: 5d29 0a20 2020 200a 2020 2020 7265 7475  ]).    .    retu
+0000a1d0: 726e 2072 616e 6b65 645f 7061 6972 735f  rn ranked_pairs_
+0000a1e0: 7462 2870 726f 6669 6c65 2c20 6375 7272  tb(profile, curr
+0000a1f0: 5f63 616e 6473 203d 2063 7572 725f 6361  _cands = curr_ca
+0000a200: 6e64 732c 2074 6965 5f62 7265 616b 6572  nds, tie_breaker
+0000a210: 203d 2074 625f 7261 6e6b 696e 672c 2073   = tb_ranking, s
+0000a220: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000a230: 203d 2073 7472 656e 6774 685f 6675 6e63   = strength_func
+0000a240: 7469 6f6e 290a 0a0a 0a40 766d 286e 616d  tion)....@vm(nam
+0000a250: 653d 2252 6976 6572 2229 0a64 6566 2072  e="River").def r
+0000a260: 6976 6572 2865 6461 7461 2c20 6375 7272  iver(edata, curr
+0000a270: 5f63 616e 6473 203d 204e 6f6e 652c 2073  _cands = None, s
+0000a280: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000a290: 203d 204e 6f6e 6529 3a20 2020 0a20 2020   = None):   .   
+0000a2a0: 2022 2222 0a20 2020 204f 7264 6572 2074   """.    Order t
+0000a2b0: 6865 2065 6467 6573 2069 6e20 7468 6520  he edges in the 
+0000a2c0: 7765 616b 206d 6172 6769 6e20 6772 6170  weak margin grap
+0000a2d0: 6820 6672 6f6d 206c 6172 6765 7374 2074  h from largest t
+0000a2e0: 6f20 736d 616c 6c65 7374 2061 6e64 206c  o smallest and l
+0000a2f0: 6f63 6b20 7468 656d 2069 6e20 696e 2074  ock them in in t
+0000a300: 6861 7420 6f72 6465 722c 2073 6b69 7070  hat order, skipp
+0000a310: 696e 6720 6564 6765 7320 7468 6174 2063  ing edges that c
+0000a320: 7265 6174 6520 6120 6379 636c 6520 2a61  reate a cycle *a
+0000a330: 6e64 2065 6467 6573 2069 6e20 7768 6963  nd edges in whic
+0000a340: 6820 7468 6572 6520 6973 2061 6c72 6561  h there is alrea
+0000a350: 6479 2061 6e20 6564 6765 2070 6f69 6e74  dy an edge point
+0000a360: 696e 6720 746f 2074 6865 2074 6172 6765  ing to the targe
+0000a370: 742a 2e20 2042 7265 616b 2074 6965 7320  t*.  Break ties 
+0000a380: 7573 696e 6720 6120 7469 652d 6272 6561  using a tie-brea
+0000a390: 6b69 6e67 2020 6c69 6e65 6172 206f 7264  king  linear ord
+0000a3a0: 6572 696e 6720 6f76 6572 2074 6865 2065  ering over the e
+0000a3b0: 6467 6573 2e20 2041 2063 616e 6469 6461  dges.  A candida
+0000a3c0: 7465 2069 7320 6120 5269 7665 7220 7769  te is a River wi
+0000a3d0: 6e6e 6572 2069 6620 6974 2077 696e 7320  nner if it wins 
+0000a3e0: 6163 636f 7264 696e 6720 746f 2073 6f6d  according to som
+0000a3f0: 6520 7469 652d 6272 6561 6b69 6e67 2072  e tie-breaking r
+0000a400: 756c 652e 2053 6565 2068 7474 7073 3a2f  ule. See https:/
+0000a410: 2f65 6c65 6374 6f77 696b 692e 6f72 672f  /electowiki.org/
+0000a420: 7769 6b69 2f52 6976 6572 2e0a 0a20 2020  wiki/River...   
+0000a430: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
+0000a440: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
+0000a450: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
+0000a460: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
+0000a470: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
+0000a480: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
+0000a490: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
+0000a4a0: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
+0000a4b0: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
+0000a4c0: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
+0000a4d0: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
+0000a4e0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
+0000a4f0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
+0000a500: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
+0000a510: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
+0000a520: 7360 600a 2020 2020 2020 2020 7374 7265  s``.        stre
+0000a530: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
+0000a540: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
+0000a550: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
+0000a560: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
+0000a570: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
+0000a580: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
+0000a590: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
+0000a5a0: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
+0000a5b0: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
+0000a5c0: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
+0000a5d0: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
+0000a5e0: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
+0000a5f0: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
+0000a600: 7264 6572 732e 200a 0a20 2020 2052 6574  rders. ..    Ret
+0000a610: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
+0000a620: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
+0000a630: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
+0000a640: 2020 3a45 7861 6d70 6c65 3a20 0a0a 2020    :Example: ..  
+0000a650: 2020 2e2e 2065 7865 635f 636f 6465 3a3a    .. exec_code::
+0000a660: 200a 0a20 2020 2020 2020 2066 726f 6d20   ..        from 
+0000a670: 7072 6566 5f76 6f74 696e 672e 7765 6967  pref_voting.weig
+0000a680: 6874 6564 5f6d 616a 6f72 6974 795f 6772  hted_majority_gr
+0000a690: 6170 6873 2069 6d70 6f72 7420 4d61 7267  aphs import Marg
+0000a6a0: 696e 4772 6170 680a 2020 2020 2020 2020  inGraph.        
+0000a6b0: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
+0000a6c0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+0000a6d0: 7468 6f64 7320 696d 706f 7274 2072 6976  thods import riv
+0000a6e0: 6572 2c20 7261 6e6b 6564 5f70 6169 7273  er, ranked_pairs
+0000a6f0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+0000a700: 2020 6d67 203d 204d 6172 6769 6e47 7261    mg = MarginGra
+0000a710: 7068 285b 302c 2031 2c20 322c 2033 5d2c  ph([0, 1, 2, 3],
+0000a720: 205b 2830 2c20 322c 2032 292c 2028 302c   [(0, 2, 2), (0,
+0000a730: 2033 2c20 3829 2c20 2831 2c20 302c 2031   3, 8), (1, 0, 1
+0000a740: 3229 2c20 2832 2c20 332c 2031 3229 2c20  2), (2, 3, 12), 
+0000a750: 2833 2c20 312c 2036 295d 290a 0a20 2020  (3, 1, 6)])..   
+0000a760: 2020 2020 2072 616e 6b65 645f 7061 6972       ranked_pair
+0000a770: 732e 6469 7370 6c61 7928 6d67 290a 2020  s.display(mg).  
+0000a780: 2020 2020 2020 7269 7665 722e 6469 7370        river.disp
+0000a790: 6c61 7928 6d67 290a 0a20 2020 2022 2222  lay(mg)..    """
+0000a7a0: 0a20 2020 2063 616e 6469 6461 7465 7320  .    candidates 
+0000a7b0: 3d20 6564 6174 612e 6361 6e64 6964 6174  = edata.candidat
+0000a7c0: 6573 2069 6620 6375 7272 5f63 616e 6473  es if curr_cands
+0000a7d0: 2069 7320 4e6f 6e65 2065 6c73 6520 6375   is None else cu
+0000a7e0: 7272 5f63 616e 6473 2020 2020 0a20 2020  rr_cands    .   
+0000a7f0: 2063 6964 785f 746f 5f63 616e 6420 3d20   cidx_to_cand = 
+0000a800: 7b63 6964 783a 2063 2066 6f72 2063 6964  {cidx: c for cid
+0000a810: 782c 2063 2069 6e20 656e 756d 6572 6174  x, c in enumerat
+0000a820: 6528 6361 6e64 6964 6174 6573 297d 2020  e(candidates)}  
+0000a830: 0a20 2020 2063 616e 645f 746f 5f63 6964  .    cand_to_cid
+0000a840: 7820 3d20 7b63 3a20 6369 6478 2066 6f72  x = {c: cidx for
+0000a850: 2063 6964 782c 2063 2069 6e20 656e 756d   cidx, c in enum
+0000a860: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
+0000a870: 297d 2020 0a0a 2020 2020 7374 7265 6e67  )}  ..    streng
+0000a880: 7468 5f66 756e 6374 696f 6e20 3d20 6564  th_function = ed
+0000a890: 6174 612e 6d61 7267 696e 2069 6620 7374  ata.margin if st
+0000a8a0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+0000a8b0: 6973 204e 6f6e 6520 656c 7365 2073 7472  is None else str
+0000a8c0: 656e 6774 685f 6675 6e63 7469 6f6e 2020  ength_function  
+0000a8d0: 2020 0a0a 2020 2020 6377 203d 2065 6461    ..    cw = eda
+0000a8e0: 7461 2e63 6f6e 646f 7263 6574 5f77 696e  ta.condorcet_win
+0000a8f0: 6e65 7228 6375 7272 5f63 616e 6473 3d63  ner(curr_cands=c
+0000a900: 7572 725f 6361 6e64 7329 0a20 2020 2023  urr_cands).    #
+0000a910: 2052 616e 6b65 6420 5061 6972 7320 6973   Ranked Pairs is
+0000a920: 2043 6f6e 646f 7263 6574 2063 6f6e 7369   Condorcet consi
+0000a930: 7374 656e 742c 2073 6f20 7369 6d70 6c79  stent, so simply
+0000a940: 2072 6574 7572 6e20 7468 6520 436f 6e64   return the Cond
+0000a950: 6f72 6365 7420 7769 6e6e 6572 2069 6620  orcet winner if 
+0000a960: 6578 6973 7473 0a20 2020 2069 6620 6377  exists.    if cw
+0000a970: 2069 7320 6e6f 7420 4e6f 6e65 3a20 0a20   is not None: . 
+0000a980: 2020 2020 2020 2077 696e 6e65 7273 203d         winners =
+0000a990: 205b 6377 5d0a 2020 2020 656c 7365 3a0a   [cw].    else:.
+0000a9a0: 2020 2020 2020 2020 775f 6564 6765 7320          w_edges 
+0000a9b0: 3d20 5b28 6331 2c20 6332 2c20 7374 7265  = [(c1, c2, stre
+0000a9c0: 6e67 7468 5f66 756e 6374 696f 6e28 6331  ngth_function(c1
+0000a9d0: 2c20 6332 2929 2066 6f72 2063 3120 696e  , c2)) for c1 in
+0000a9e0: 2063 616e 6469 6461 7465 7320 666f 7220   candidates for 
+0000a9f0: 6332 2069 6e20 6361 6e64 6964 6174 6573  c2 in candidates
+0000aa00: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0000aa10: 2020 2020 2069 6620 6331 2021 3d20 6332       if c1 != c2
+0000aa20: 2061 6e64 2028 6564 6174 612e 6d61 6a6f   and (edata.majo
+0000aa30: 7269 7479 5f70 7265 6665 7273 2863 312c  rity_prefers(c1,
+0000aa40: 2063 3229 206f 7220 6564 6174 612e 6973   c2) or edata.is
+0000aa50: 5f74 6965 6428 6331 2c20 6332 2929 5d0a  _tied(c1, c2))].
+0000aa60: 2020 2020 2020 2020 7769 6e6e 6572 7320          winners 
+0000aa70: 3d20 6c69 7374 2829 2020 2020 2020 2020  = list()        
+0000aa80: 2020 2020 0a20 2020 2020 2020 2073 7472      .        str
+0000aa90: 656e 6774 6873 203d 2073 6f72 7465 6428  engths = sorted(
+0000aaa0: 6c69 7374 2873 6574 285b 655b 325d 2066  list(set([e[2] f
+0000aab0: 6f72 2065 2069 6e20 775f 6564 6765 735d  or e in w_edges]
+0000aac0: 2929 2c20 7265 7665 7273 653d 5472 7565  )), reverse=True
+0000aad0: 290a 2020 2020 2020 2020 736f 7274 6564  ).        sorted
+0000aae0: 5f65 6467 6573 203d 205b 5b65 2066 6f72  _edges = [[e for
+0000aaf0: 2065 2069 6e20 775f 6564 6765 7320 6966   e in w_edges if
+0000ab00: 2065 5b32 5d20 3d3d 2073 5d20 666f 7220   e[2] == s] for 
+0000ab10: 7320 696e 2073 7472 656e 6774 6873 5d0a  s in strengths].
+0000ab20: 2020 2020 2020 2020 7462 7320 3d20 7072          tbs = pr
+0000ab30: 6f64 7563 7428 2a5b 7065 726d 7574 6174  oduct(*[permutat
+0000ab40: 696f 6e73 2865 6467 6573 2920 666f 7220  ions(edges) for 
+0000ab50: 6564 6765 7320 696e 2073 6f72 7465 645f  edges in sorted_
+0000ab60: 6564 6765 735d 290a 2020 2020 2020 2020  edges]).        
+0000ab70: 666f 7220 7462 2069 6e20 7462 733a 0a20  for tb in tbs:. 
+0000ab80: 2020 2020 2020 2020 2020 2065 6467 6573             edges
+0000ab90: 203d 2066 6c61 7474 656e 2874 6229 0a20   = flatten(tb). 
+0000aba0: 2020 2020 2020 2020 2020 2072 765f 6465             rv_de
+0000abb0: 6665 6174 203d 2053 504f 286c 656e 2863  feat = SPO(len(c
+0000abc0: 616e 6469 6461 7465 7329 290a 2020 2020  andidates)).    
+0000abd0: 2020 2020 2020 2020 666f 7220 6530 2c65          for e0,e
+0000abe0: 312c 7320 696e 2065 6467 6573 3a20 0a20  1,s in edges: . 
+0000abf0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000ac00: 6620 6e6f 7420 7276 5f64 6566 6561 742e  f not rv_defeat.
+0000ac10: 505b 6361 6e64 5f74 6f5f 6369 6478 5b65  P[cand_to_cidx[e
+0000ac20: 315d 5d5b 6361 6e64 5f74 6f5f 6369 6478  1]][cand_to_cidx
+0000ac30: 5b65 305d 5d20 616e 6420 6c65 6e28 7276  [e0]] and len(rv
+0000ac40: 5f64 6566 6561 742e 7072 6564 735b 6361  _defeat.preds[ca
+0000ac50: 6e64 5f74 6f5f 6369 6478 5b65 315d 5d29  nd_to_cidx[e1]])
+0000ac60: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+0000ac70: 2020 2020 2020 2020 2020 2072 765f 6465             rv_de
+0000ac80: 6665 6174 2e61 6464 2863 616e 645f 746f  feat.add(cand_to
+0000ac90: 5f63 6964 785b 6530 5d2c 6361 6e64 5f74  _cidx[e0],cand_t
+0000aca0: 6f5f 6369 6478 5b65 315d 290a 2020 2020  o_cidx[e1]).    
+0000acb0: 2020 2020 2020 2020 7769 6e6e 6572 732e          winners.
+0000acc0: 6170 7065 6e64 2863 6964 785f 746f 5f63  append(cidx_to_c
+0000acd0: 616e 645b 7276 5f64 6566 6561 742e 696e  and[rv_defeat.in
+0000ace0: 6974 6961 6c5f 656c 656d 656e 7473 2829  itial_elements()
+0000acf0: 5b30 5d5d 290a 0a20 2020 2072 6574 7572  [0]])..    retur
+0000ad00: 6e20 736f 7274 6564 286c 6973 7428 7365  n sorted(list(se
+0000ad10: 7428 7769 6e6e 6572 7329 2929 0a0a 6465  t(winners)))..de
+0000ad20: 6620 7269 7665 725f 6465 6665 6174 7328  f river_defeats(
+0000ad30: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
+0000ad40: 7320 3d20 4e6f 6e65 2c20 7374 7265 6e67  s = None, streng
+0000ad50: 7468 5f66 756e 6374 696f 6e20 3d20 4e6f  th_function = No
+0000ad60: 6e65 293a 0a20 2020 2022 2222 0a20 2020  ne):.    """.   
+0000ad70: 2052 6574 7572 6e73 2074 6865 2052 6976   Returns the Riv
+0000ad80: 6572 2064 6566 6561 7420 7265 6c61 7469  er defeat relati
+0000ad90: 6f6e 7320 7072 6f64 7563 6564 2062 7920  ons produced by 
+0000ada0: 7468 6520 5269 7665 7220 616c 676f 7269  the River algori
+0000adb0: 7468 6d2e 0a0a 2020 2020 2e2e 2069 6d70  thm...    .. imp
+0000adc0: 6f72 7461 6e74 3a3a 0a20 2020 2020 2020  ortant::.       
+0000add0: 2055 6e6c 696b 6520 7468 6520 6f74 6865   Unlike the othe
+0000ade0: 7220 6675 6e63 7469 6f6e 7320 7468 6174  r functions that
+0000adf0: 2072 6574 7572 6e20 6120 7369 6e67 6c65   return a single
+0000ae00: 2064 6566 6561 7420 7265 6c61 7469 6f6e   defeat relation
+0000ae10: 2c20 7468 6973 2072 6574 7572 6e73 2061  , this returns a
+0000ae20: 206c 6973 7420 6f66 2064 6566 6561 7420   list of defeat 
+0000ae30: 7265 6c61 7469 6f6e 732e 200a 2020 2020  relations. .    
+0000ae40: 2020 2020 0a20 2020 2041 7267 733a 0a20      .    Args:. 
+0000ae50: 2020 2020 2020 2065 6461 7461 2028 5072         edata (Pr
+0000ae60: 6f66 696c 652c 2050 726f 6669 6c65 5769  ofile, ProfileWi
+0000ae70: 7468 5469 6573 2c20 4d61 7267 696e 4772  thTies, MarginGr
+0000ae80: 6170 6829 3a20 416e 7920 656c 6563 7469  aph): Any electi
+0000ae90: 6f6e 2064 6174 6120 7468 6174 2068 6173  on data that has
+0000aea0: 2061 2060 6d61 7267 696e 6020 6d65 7468   a `margin` meth
+0000aeb0: 6f64 2e20 0a20 2020 2020 2020 2063 7572  od. .        cur
+0000aec0: 725f 6361 6e64 7320 284c 6973 745b 696e  r_cands (List[in
+0000aed0: 745d 2c20 6f70 7469 6f6e 616c 293a 2049  t], optional): I
+0000aee0: 6620 7365 742c 2074 6865 6e20 6669 6e64  f set, then find
+0000aef0: 2074 6865 2077 696e 6e65 7273 2066 6f72   the winners for
+0000af00: 2074 6865 2070 726f 6669 6c65 2072 6573   the profile res
+0000af10: 7472 6963 7465 6420 746f 2074 6865 2063  tricted to the c
+0000af20: 616e 6469 6461 7465 7320 696e 2060 6063  andidates in ``c
+0000af30: 7572 725f 6361 6e64 7360 600a 2020 2020  urr_cands``.    
+0000af40: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+0000af50: 6374 696f 6e20 2866 756e 6374 696f 6e2c  ction (function,
+0000af60: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+0000af70: 7374 7265 6e67 7468 2066 756e 6374 696f  strength functio
+0000af80: 6e20 746f 2062 6520 7573 6564 2074 6f20  n to be used to 
+0000af90: 6361 6c63 756c 6174 6520 7468 6520 7374  calculate the st
+0000afa0: 7265 6e67 7468 206f 6620 6120 7061 7468  rength of a path
+0000afb0: 2e20 2020 5468 6520 6465 6661 756c 7420  .   The default 
+0000afc0: 6973 2074 6865 206d 6172 6769 6e20 6d65  is the margin me
+0000afd0: 7468 6f64 206f 6620 6060 6564 6174 6160  thod of ``edata`
+0000afe0: 602e 2020 2054 6869 7320 6f6e 6c79 206d  `.   This only m
+0000aff0: 6174 7465 7273 2077 6865 6e20 7468 6520  atters when the 
+0000b000: 6261 6c6c 6f74 7320 6172 6520 6e6f 7420  ballots are not 
+0000b010: 6c69 6e65 6172 206f 7264 6572 732e 200a  linear orders. .
+0000b020: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
+0000b030: 2020 2020 2020 2041 206e 6574 776f 726b         A network
+0000b040: 7820 4469 4772 6170 6820 7265 7072 6573  x DiGraph repres
+0000b050: 656e 7469 6e67 2074 6865 2052 6976 6572  enting the River
+0000b060: 2064 6566 6561 7420 7265 6c61 7469 6f6e   defeat relation
+0000b070: 2e20 0a20 2020 2022 2222 0a0a 2020 2020  . .    """..    
+0000b080: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
+0000b090: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
+0000b0a0: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
+0000b0b0: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
+0000b0c0: 6e64 7320 2020 200a 2020 2020 7374 7265  nds    .    stre
+0000b0d0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+0000b0e0: 6564 6174 612e 6d61 7267 696e 2069 6620  edata.margin if 
+0000b0f0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+0000b100: 6e20 6973 204e 6f6e 6520 656c 7365 2073  n is None else s
+0000b110: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000b120: 2020 2020 0a0a 2020 2020 775f 6564 6765      ..    w_edge
+0000b130: 7320 3d20 5b28 6331 2c20 6332 2c20 7374  s = [(c1, c2, st
+0000b140: 7265 6e67 7468 5f66 756e 6374 696f 6e28  rength_function(
+0000b150: 6331 2c20 6332 2929 2066 6f72 2063 3120  c1, c2)) for c1 
+0000b160: 696e 2063 616e 6469 6461 7465 7320 666f  in candidates fo
+0000b170: 7220 6332 2069 6e20 6361 6e64 6964 6174  r c2 in candidat
+0000b180: 6573 2069 6620 6331 2021 3d20 6332 2061  es if c1 != c2 a
+0000b190: 6e64 2028 6564 6174 612e 6d61 6a6f 7269  nd (edata.majori
+0000b1a0: 7479 5f70 7265 6665 7273 2863 312c 2063  ty_prefers(c1, c
+0000b1b0: 3229 206f 7220 6564 6174 612e 6973 5f74  2) or edata.is_t
+0000b1c0: 6965 6428 6331 2c20 6332 2929 5d0a 0a20  ied(c1, c2))].. 
+0000b1d0: 2020 2073 7472 656e 6774 6873 203d 2073     strengths = s
+0000b1e0: 6f72 7465 6428 6c69 7374 2873 6574 285b  orted(list(set([
+0000b1f0: 655b 325d 2066 6f72 2065 2069 6e20 775f  e[2] for e in w_
+0000b200: 6564 6765 735d 2929 2c20 7265 7665 7273  edges])), revers
+0000b210: 653d 5472 7565 290a 2020 2020 736f 7274  e=True).    sort
+0000b220: 6564 5f65 6467 6573 203d 205b 5b65 2066  ed_edges = [[e f
+0000b230: 6f72 2065 2069 6e20 775f 6564 6765 7320  or e in w_edges 
+0000b240: 6966 2065 5b32 5d20 3d3d 2073 5d20 666f  if e[2] == s] fo
+0000b250: 7220 7320 696e 2073 7472 656e 6774 6873  r s in strengths
+0000b260: 5d0a 2020 2020 7462 7320 3d20 7072 6f64  ].    tbs = prod
+0000b270: 7563 7428 2a5b 7065 726d 7574 6174 696f  uct(*[permutatio
+0000b280: 6e73 2865 6467 6573 2920 666f 7220 6564  ns(edges) for ed
+0000b290: 6765 7320 696e 2073 6f72 7465 645f 6564  ges in sorted_ed
+0000b2a0: 6765 735d 290a 0a20 2020 2072 6976 6572  ges])..    river
+0000b2b0: 5f64 6566 6561 7473 203d 206c 6973 7428  _defeats = list(
+0000b2c0: 290a 2020 2020 666f 7220 7462 2069 6e20  ).    for tb in 
+0000b2d0: 7462 733a 0a20 2020 2020 2020 2065 6467  tbs:.        edg
+0000b2e0: 6573 203d 2066 6c61 7474 656e 2874 6229  es = flatten(tb)
+0000b2f0: 0a20 2020 2020 2020 2072 6976 6572 5f64  .        river_d
+0000b300: 6566 6561 7420 3d20 6e78 2e44 6947 7261  efeat = nx.DiGra
+0000b310: 7068 2829 200a 2020 2020 2020 2020 666f  ph() .        fo
+0000b320: 7220 6520 696e 2065 6467 6573 3a20 0a20  r e in edges: . 
+0000b330: 2020 2020 2020 2020 2020 2069 6620 655b             if e[
+0000b340: 315d 206e 6f74 2069 6e20 7269 7665 725f  1] not in river_
+0000b350: 6465 6665 6174 2e6e 6f64 6573 206f 7220  defeat.nodes or 
+0000b360: 6c65 6e28 6c69 7374 2872 6976 6572 5f64  len(list(river_d
+0000b370: 6566 6561 742e 696e 5f65 6467 6573 2865  efeat.in_edges(e
+0000b380: 5b31 5d29 2929 203d 3d20 303a 0a20 2020  [1]))) == 0:.   
+0000b390: 2020 2020 2020 2020 2020 2020 2072 6976               riv
+0000b3a0: 6572 5f64 6566 6561 742e 6164 645f 6564  er_defeat.add_ed
+0000b3b0: 6765 2865 5b30 5d2c 2065 5b31 5d2c 2077  ge(e[0], e[1], w
+0000b3c0: 6569 6768 743d 655b 325d 290a 2020 2020  eight=e[2]).    
+0000b3d0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+0000b3e0: 6f65 735f 6372 6561 7465 5f63 7963 6c65  oes_create_cycle
+0000b3f0: 2872 6976 6572 5f64 6566 6561 742c 2065  (river_defeat, e
+0000b400: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000b410: 2020 2020 2020 2072 6976 6572 5f64 6566         river_def
+0000b420: 6561 742e 7265 6d6f 7665 5f65 6467 6528  eat.remove_edge(
+0000b430: 655b 305d 2c20 655b 315d 290a 2020 2020  e[0], e[1]).    
+0000b440: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0000b450: 2072 6976 6572 5f64 6566 6561 7473 2e61   river_defeats.a
+0000b460: 7070 656e 6428 7269 7665 725f 6465 6665  ppend(river_defe
+0000b470: 6174 290a 0a20 2020 2072 6574 7572 6e20  at)..    return 
+0000b480: 7269 7665 725f 6465 6665 6174 730a 0a40  river_defeats..@
+0000b490: 766d 286e 616d 653d 2252 6976 6572 2229  vm(name="River")
+0000b4a0: 0a64 6566 2072 6976 6572 5f77 6974 685f  .def river_with_
+0000b4b0: 7465 7374 2865 6461 7461 2c20 6375 7272  test(edata, curr
+0000b4c0: 5f63 616e 6473 203d 204e 6f6e 652c 2073  _cands = None, s
+0000b4d0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000b4e0: 203d 204e 6f6e 6529 3a20 2020 0a20 2020   = None):   .   
+0000b4f0: 2022 2222 4669 6e64 2074 6865 2052 6976   """Find the Riv
+0000b500: 6572 2077 696e 6e65 7273 2077 6974 6820  er winners with 
+0000b510: 6120 7465 7374 2074 6f20 6465 7465 726d  a test to determ
+0000b520: 696e 6564 2069 6620 6974 2077 696c 6c20  ined if it will 
+0000b530: 7461 6b65 2074 6f6f 206c 6f6e 6720 746f  take too long to
+0000b540: 2063 6f6d 7075 7465 2074 6865 2052 6976   compute the Riv
+0000b550: 6572 2077 696e 6e65 7273 2e20 4966 2074  er winners. If t
+0000b560: 6865 2063 616c 6375 6c61 7469 6f6e 206f  he calculation o
+0000b570: 6620 7468 6520 7769 6e6e 6572 7320 7769  f the winners wi
+0000b580: 6c6c 2074 616b 6520 746f 6f20 6c6f 6e67  ll take too long
+0000b590: 2c20 7265 7475 726e 204e 6f6e 652e 200a  , return None. .
+0000b5a0: 2020 2020 2020 2020 0a20 2020 202e 2e20          .    .. 
+0000b5b0: 696d 706f 7274 616e 743a 3a0a 2020 2020  important::.    
+0000b5c0: 2020 2020 5468 6973 2076 6f74 696e 6720      This voting 
+0000b5d0: 6d65 7468 6f64 2074 6861 7420 6d69 6768  method that migh
+0000b5e0: 7420 7265 7475 726e 204e 6f6e 6520 7261  t return None ra
+0000b5f0: 7468 6572 2074 6861 6e20 6120 6c69 7374  ther than a list
+0000b600: 206f 6620 6361 6e64 6964 6174 6573 2e20   of candidates. 
+0000b610: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
+0000b620: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
+0000b630: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
+0000b640: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
+0000b650: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
+0000b660: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
+0000b670: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
+0000b680: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
+0000b690: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
+0000b6a0: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+0000b6b0: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
+0000b6c0: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
+0000b6d0: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
+0000b6e0: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
+0000b6f0: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
+0000b700: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
+0000b710: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+0000b720: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
+0000b730: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
+0000b740: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
+0000b750: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
+0000b760: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
+0000b770: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
+0000b780: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
+0000b790: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
+0000b7a0: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
+0000b7b0: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
+0000b7c0: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
+0000b7d0: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
+0000b7e0: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
+0000b7f0: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+0000b800: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
+0000b810: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
+0000b820: 2e20 0a0a 2020 2020 2e2e 2073 6565 616c  . ..    .. seeal
+0000b830: 736f 3a3a 0a0a 2020 2020 2020 2020 3a6d  so::..        :m
+0000b840: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
+0000b850: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+0000b860: 7468 6f64 732e 7261 6e6b 6564 5f70 6169  thods.ranked_pai
+0000b870: 7273 5f77 6974 685f 7465 7374 602c 203a  rs_with_test`, :
+0000b880: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
+0000b890: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
+0000b8a0: 6574 686f 6473 2e72 6976 6572 600a 0a0a  ethods.river`...
+0000b8b0: 2020 2020 2222 220a 2020 2020 6361 6e64      """.    cand
+0000b8c0: 6964 6174 6573 203d 2065 6461 7461 2e63  idates = edata.c
+0000b8d0: 616e 6469 6461 7465 7320 6966 2063 7572  andidates if cur
+0000b8e0: 725f 6361 6e64 7320 6973 204e 6f6e 6520  r_cands is None 
+0000b8f0: 656c 7365 2063 7572 725f 6361 6e64 7320  else curr_cands 
+0000b900: 2020 200a 2020 2020 6369 6478 5f74 6f5f     .    cidx_to_
+0000b910: 6361 6e64 203d 207b 6369 6478 3a20 6320  cand = {cidx: c 
+0000b920: 666f 7220 6369 6478 2c20 6320 696e 2065  for cidx, c in e
+0000b930: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
+0000b940: 7465 7329 7d20 200a 2020 2020 6361 6e64  tes)}  .    cand
+0000b950: 5f74 6f5f 6369 6478 203d 207b 633a 2063  _to_cidx = {c: c
+0000b960: 6964 7820 666f 7220 6369 6478 2c20 6320  idx for cidx, c 
+0000b970: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+0000b980: 6469 6461 7465 7329 7d20 200a 0a20 2020  didates)}  ..   
+0000b990: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000b9a0: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
+0000b9b0: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
+0000b9c0: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
+0000b9d0: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
+0000b9e0: 6374 696f 6e20 2020 200a 0a20 2020 2063  ction    ..    c
+0000b9f0: 7720 3d20 6564 6174 612e 636f 6e64 6f72  w = edata.condor
+0000ba00: 6365 745f 7769 6e6e 6572 2863 7572 725f  cet_winner(curr_
+0000ba10: 6361 6e64 733d 6375 7272 5f63 616e 6473  cands=curr_cands
+0000ba20: 290a 2020 2020 2320 5261 6e6b 6564 2050  ).    # Ranked P
+0000ba30: 6169 7273 2069 7320 436f 6e64 6f72 6365  airs is Condorce
+0000ba40: 7420 636f 6e73 6973 7465 6e74 2c20 736f  t consistent, so
+0000ba50: 2073 696d 706c 7920 7265 7475 726e 2074   simply return t
+0000ba60: 6865 2043 6f6e 646f 7263 6574 2077 696e  he Condorcet win
+0000ba70: 6e65 7220 6966 2065 7869 7374 730a 2020  ner if exists.  
+0000ba80: 2020 6966 2063 7720 6973 206e 6f74 204e    if cw is not N
+0000ba90: 6f6e 653a 200a 2020 2020 2020 2020 7769  one: .        wi
+0000baa0: 6e6e 6572 7320 3d20 5b63 775d 0a20 2020  nners = [cw].   
+0000bab0: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
+0000bac0: 5f65 6467 6573 203d 205b 2863 312c 2063  _edges = [(c1, c
+0000bad0: 322c 2073 7472 656e 6774 685f 6675 6e63  2, strength_func
+0000bae0: 7469 6f6e 2863 312c 2063 3229 2920 666f  tion(c1, c2)) fo
+0000baf0: 7220 6331 2069 6e20 6361 6e64 6964 6174  r c1 in candidat
+0000bb00: 6573 2066 6f72 2063 3220 696e 2063 616e  es for c2 in can
+0000bb10: 6469 6461 7465 7320 0a20 2020 2020 2020  didates .       
+0000bb20: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+0000bb30: 3120 213d 2063 3220 616e 6420 2865 6461  1 != c2 and (eda
+0000bb40: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+0000bb50: 6572 7328 6331 2c20 6332 2920 6f72 2065  ers(c1, c2) or e
+0000bb60: 6461 7461 2e69 735f 7469 6564 2863 312c  data.is_tied(c1,
+0000bb70: 2063 3229 295d 0a20 2020 2020 2020 2077   c2))].        w
+0000bb80: 696e 6e65 7273 203d 206c 6973 7428 2920  inners = list() 
+0000bb90: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+0000bba0: 2020 2020 7374 7265 6e67 7468 7320 3d20      strengths = 
+0000bbb0: 736f 7274 6564 286c 6973 7428 7365 7428  sorted(list(set(
+0000bbc0: 5b65 5b32 5d20 666f 7220 6520 696e 2077  [e[2] for e in w
+0000bbd0: 5f65 6467 6573 5d29 292c 2072 6576 6572  _edges])), rever
+0000bbe0: 7365 3d54 7275 6529 0a20 2020 2020 2020  se=True).       
+0000bbf0: 2073 6f72 7465 645f 6564 6765 7320 3d20   sorted_edges = 
+0000bc00: 5b5b 6520 666f 7220 6520 696e 2077 5f65  [[e for e in w_e
+0000bc10: 6467 6573 2069 6620 655b 325d 203d 3d20  dges if e[2] == 
+0000bc20: 735d 2066 6f72 2073 2069 6e20 7374 7265  s] for s in stre
+0000bc30: 6e67 7468 735d 0a20 2020 2020 2020 2069  ngths].        i
+0000bc40: 6620 6e70 2e70 726f 6428 5b6d 6174 682e  f np.prod([math.
+0000bc50: 6661 6374 6f72 6961 6c28 6c65 6e28 6573  factorial(len(es
+0000bc60: 2929 2066 6f72 2065 7320 696e 2073 6f72  )) for es in sor
+0000bc70: 7465 645f 6564 6765 735d 2920 3e20 3330  ted_edges]) > 30
+0000bc80: 3030 3a20 0a20 2020 2020 2020 2020 2020  00: .           
+0000bc90: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
+0000bca0: 2020 2020 2065 6c73 653a 200a 2020 2020       else: .    
+0000bcb0: 2020 2020 2020 2020 7462 7320 3d20 7072          tbs = pr
+0000bcc0: 6f64 7563 7428 2a5b 7065 726d 7574 6174  oduct(*[permutat
+0000bcd0: 696f 6e73 2865 6467 6573 2920 666f 7220  ions(edges) for 
+0000bce0: 6564 6765 7320 696e 2073 6f72 7465 645f  edges in sorted_
+0000bcf0: 6564 6765 735d 290a 2020 2020 2020 2020  edges]).        
+0000bd00: 2020 2020 666f 7220 7462 2069 6e20 7462      for tb in tb
+0000bd10: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000bd20: 2020 2065 6467 6573 203d 2066 6c61 7474     edges = flatt
+0000bd30: 656e 2874 6229 0a20 2020 2020 2020 2020  en(tb).         
+0000bd40: 2020 2020 2020 2072 765f 6465 6665 6174         rv_defeat
+0000bd50: 203d 2053 504f 286c 656e 2863 616e 6469   = SPO(len(candi
+0000bd60: 6461 7465 7329 290a 2020 2020 2020 2020  dates)).        
+0000bd70: 2020 2020 2020 2020 666f 7220 6530 2c65          for e0,e
+0000bd80: 312c 7320 696e 2065 6467 6573 3a20 0a20  1,s in edges: . 
 0000bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bda0: 2020 2020 6966 206e 6f74 2072 765f 6465      if not rv_de
-0000bdb0: 6665 6174 2e50 5b63 616e 645f 746f 5f63  feat.P[cand_to_c
-0000bdc0: 6964 785b 6531 5d5d 5b63 616e 645f 746f  idx[e1]][cand_to
-0000bdd0: 5f63 6964 785b 6530 5d5d 2061 6e64 206c  _cidx[e0]] and l
-0000bde0: 656e 2872 765f 6465 6665 6174 2e70 7265  en(rv_defeat.pre
-0000bdf0: 6473 5b63 616e 645f 746f 5f63 6964 785b  ds[cand_to_cidx[
-0000be00: 6531 5d5d 2920 3d3d 2030 3a0a 2020 2020  e1]]) == 0:.    
+0000bda0: 2020 2069 6620 6e6f 7420 7276 5f64 6566     if not rv_def
+0000bdb0: 6561 742e 505b 6361 6e64 5f74 6f5f 6369  eat.P[cand_to_ci
+0000bdc0: 6478 5b65 315d 5d5b 6361 6e64 5f74 6f5f  dx[e1]][cand_to_
+0000bdd0: 6369 6478 5b65 305d 5d20 616e 6420 6c65  cidx[e0]] and le
+0000bde0: 6e28 7276 5f64 6566 6561 742e 7072 6564  n(rv_defeat.pred
+0000bdf0: 735b 6361 6e64 5f74 6f5f 6369 6478 5b65  s[cand_to_cidx[e
+0000be00: 315d 5d29 203d 3d20 303a 0a20 2020 2020  1]]) == 0:.     
 0000be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be20: 2020 2020 7276 5f64 6566 6561 742e 6164      rv_defeat.ad
-0000be30: 6428 6361 6e64 5f74 6f5f 6369 6478 5b65  d(cand_to_cidx[e
-0000be40: 305d 2c63 616e 645f 746f 5f63 6964 785b  0],cand_to_cidx[
-0000be50: 6531 5d29 0a20 2020 2020 2020 2020 2020  e1]).           
-0000be60: 2020 2020 2077 696e 6e65 7273 2e61 7070       winners.app
-0000be70: 656e 6428 6369 6478 5f74 6f5f 6361 6e64  end(cidx_to_cand
-0000be80: 5b72 765f 6465 6665 6174 2e69 6e69 7469  [rv_defeat.initi
-0000be90: 616c 5f65 6c65 6d65 6e74 7328 295b 305d  al_elements()[0]
-0000bea0: 5d29 0a20 2020 2072 6574 7572 6e20 736f  ]).    return so
-0000beb0: 7274 6564 286c 6973 7428 7365 7428 7769  rted(list(set(wi
-0000bec0: 6e6e 6572 7329 2929 0a0a 0a40 766d 286e  nners)))...@vm(n
-0000bed0: 616d 653d 2252 6976 6572 2054 4222 290a  ame="River TB").
-0000bee0: 6465 6620 7269 7665 725f 7462 2865 6461  def river_tb(eda
-0000bef0: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
-0000bf00: 204e 6f6e 652c 2074 6965 5f62 7265 616b   None, tie_break
-0000bf10: 6572 203d 204e 6f6e 652c 2073 7472 656e  er = None, stren
-0000bf20: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
-0000bf30: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
-0000bf40: 0a20 2020 2052 6976 6572 2077 6974 6820  .    River with 
-0000bf50: 6120 6669 7865 6420 6c69 6e65 6172 206f  a fixed linear o
-0000bf60: 7264 6572 206f 6e20 7468 6520 6361 6e64  rder on the cand
-0000bf70: 6964 6174 6573 2074 6f20 6272 6561 6b20  idates to break 
-0000bf80: 616e 7920 7469 6573 2069 6e20 7468 6520  any ties in the 
-0000bf90: 6d61 7267 696e 732e 2020 5369 6e63 6520  margins.  Since 
-0000bfa0: 7468 6520 7469 655f 6272 6561 6b65 7220  the tie_breaker 
-0000bfb0: 6973 2061 206c 696e 6561 7220 6f72 6465  is a linear orde
-0000bfc0: 722c 2074 6869 7320 6d65 7468 6f64 2069  r, this method i
-0000bfd0: 7320 7265 736f 6c75 7465 2e20 2020 0a0a  s resolute.   ..
-0000bfe0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000bff0: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
-0000c000: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
-0000c010: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
-0000c020: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
-0000c030: 7461 2074 6861 7420 6861 7320 6120 606d  ta that has a `m
-0000c040: 6172 6769 6e60 206d 6574 686f 642e 200a  argin` method. .
-0000c050: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
-0000c060: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
-0000c070: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
-0000c080: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
-0000c090: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
-0000c0a0: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
-0000c0b0: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
-0000c0c0: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
-0000c0d0: 616e 6473 6060 0a20 2020 2020 2020 2074  ands``.        t
-0000c0e0: 6965 5f62 7265 616b 6572 2028 4c69 7374  ie_breaker (List
-0000c0f0: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
-0000c100: 3a20 4120 6c69 6e65 6172 206f 7264 6572  : A linear order
-0000c110: 206f 6e20 7468 6520 6361 6e64 6964 6174   on the candidat
-0000c120: 6573 2e20 2049 6620 6e6f 7420 7365 742c  es.  If not set,
-0000c130: 2074 6865 6e20 7468 6520 6361 6e64 6964   then the candid
-0000c140: 6174 6573 2061 7265 2073 6f72 7465 6420  ates are sorted 
-0000c150: 696e 2061 7363 656e 6469 6e67 206f 7264  in ascending ord
-0000c160: 6572 2e0a 2020 2020 2020 2020 7374 7265  er..        stre
-0000c170: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
-0000c180: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
-0000c190: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
-0000c1a0: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
-0000c1b0: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
-0000c1c0: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
-0000c1d0: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
-0000c1e0: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
-0000c1f0: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
-0000c200: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
-0000c210: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
-0000c220: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
-0000c230: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
-0000c240: 7264 6572 732e 200a 0a20 2020 2052 6574  rders. ..    Ret
-0000c250: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
-0000c260: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
-0000c270: 6361 6e64 6964 6174 6573 2e20 0a0a 0a20  candidates. ... 
-0000c280: 2020 2022 2222 0a20 2020 2063 616e 6469     """.    candi
-0000c290: 6461 7465 7320 3d20 6564 6174 612e 6361  dates = edata.ca
-0000c2a0: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
-0000c2b0: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
-0000c2c0: 6c73 6520 6375 7272 5f63 616e 6473 2020  lse curr_cands  
-0000c2d0: 2020 0a20 2020 2063 6964 785f 746f 5f63    .    cidx_to_c
-0000c2e0: 616e 6420 3d20 7b63 6964 783a 2063 2066  and = {cidx: c f
-0000c2f0: 6f72 2063 6964 782c 2063 2069 6e20 656e  or cidx, c in en
-0000c300: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
-0000c310: 6573 297d 2020 0a20 2020 2063 616e 645f  es)}  .    cand_
-0000c320: 746f 5f63 6964 7820 3d20 7b63 3a20 6369  to_cidx = {c: ci
-0000c330: 6478 2066 6f72 2063 6964 782c 2063 2069  dx for cidx, c i
-0000c340: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
-0000c350: 6964 6174 6573 297d 2020 0a20 2020 2073  idates)}  .    s
-0000c360: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000c370: 203d 2065 6461 7461 2e6d 6172 6769 6e20   = edata.margin 
-0000c380: 6966 2073 7472 656e 6774 685f 6675 6e63  if strength_func
-0000c390: 7469 6f6e 2069 7320 4e6f 6e65 2065 6c73  tion is None els
-0000c3a0: 6520 7374 7265 6e67 7468 5f66 756e 6374  e strength_funct
-0000c3b0: 696f 6e20 2020 200a 0a20 2020 2074 625f  ion    ..    tb_
-0000c3c0: 7261 6e6b 696e 6720 3d20 7469 655f 6272  ranking = tie_br
-0000c3d0: 6561 6b65 7220 6966 2074 6965 5f62 7265  eaker if tie_bre
-0000c3e0: 616b 6572 2069 7320 6e6f 7420 4e6f 6e65  aker is not None
-0000c3f0: 2065 6c73 6520 736f 7274 6564 286c 6973   else sorted(lis
-0000c400: 7428 6361 6e64 6964 6174 6573 2929 0a0a  t(candidates))..
-0000c410: 2020 2020 6377 203d 2065 6461 7461 2e63      cw = edata.c
-0000c420: 6f6e 646f 7263 6574 5f77 696e 6e65 7228  ondorcet_winner(
-0000c430: 6375 7272 5f63 616e 6473 3d63 7572 725f  curr_cands=curr_
-0000c440: 6361 6e64 7329 0a20 2020 2023 2052 6976  cands).    # Riv
-0000c450: 6572 2069 7320 436f 6e64 6f72 6365 7420  er is Condorcet 
-0000c460: 636f 6e73 6973 7465 6e74 2c20 736f 2073  consistent, so s
-0000c470: 696d 706c 7920 7265 7475 726e 2074 6865  imply return the
-0000c480: 2043 6f6e 646f 7263 6574 2077 696e 6e65   Condorcet winne
-0000c490: 7220 6966 2065 7869 7374 730a 2020 2020  r if exists.    
-0000c4a0: 6966 2063 7720 6973 206e 6f74 204e 6f6e  if cw is not Non
-0000c4b0: 653a 200a 2020 2020 2020 2020 7769 6e6e  e: .        winn
-0000c4c0: 6572 7320 3d20 5b63 775d 0a20 2020 2065  ers = [cw].    e
-0000c4d0: 6c73 653a 0a20 2020 2020 2020 2077 5f65  lse:.        w_e
-0000c4e0: 6467 6573 203d 205b 2863 312c 2063 322c  dges = [(c1, c2,
-0000c4f0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000c500: 6f6e 2863 312c 2063 3229 2920 666f 7220  on(c1, c2)) for 
-0000c510: 6331 2069 6e20 6361 6e64 6964 6174 6573  c1 in candidates
-0000c520: 2066 6f72 2063 3220 696e 2063 616e 6469   for c2 in candi
-0000c530: 6461 7465 7320 6966 2063 3120 213d 2063  dates if c1 != c
-0000c540: 3220 616e 6420 2865 6461 7461 2e6d 616a  2 and (edata.maj
-0000c550: 6f72 6974 795f 7072 6566 6572 7328 6331  ority_prefers(c1
-0000c560: 2c20 6332 2920 6f72 2065 6461 7461 2e69  , c2) or edata.i
-0000c570: 735f 7469 6564 2863 312c 2063 3229 295d  s_tied(c1, c2))]
-0000c580: 0a20 2020 2020 2020 2077 696e 6e65 7273  .        winners
-0000c590: 203d 206c 6973 7428 2920 200a 2020 2020   = list()  .    
-0000c5a0: 2020 2020 7374 7265 6e67 7468 7320 3d20      strengths = 
-0000c5b0: 736f 7274 6564 286c 6973 7428 7365 7428  sorted(list(set(
-0000c5c0: 5b65 5b32 5d20 666f 7220 6520 696e 2077  [e[2] for e in w
-0000c5d0: 5f65 6467 6573 5d29 292c 2072 6576 6572  _edges])), rever
-0000c5e0: 7365 3d54 7275 6529 0a0a 2020 2020 2020  se=True)..      
-0000c5f0: 2020 7276 5f64 6566 6561 7420 3d20 5350    rv_defeat = SP
-0000c600: 4f28 6c65 6e28 6361 6e64 6964 6174 6573  O(len(candidates
-0000c610: 2929 0a0a 2020 2020 2020 2020 666f 7220  ))..        for 
-0000c620: 7320 696e 2073 7472 656e 6774 6873 3a20  s in strengths: 
-0000c630: 0a20 2020 2020 2020 2020 2020 2065 6467  .            edg
-0000c640: 6573 203d 205b 6520 666f 7220 6520 696e  es = [e for e in
-0000c650: 2077 5f65 6467 6573 2069 6620 655b 325d   w_edges if e[2]
-0000c660: 203d 3d20 735d 0a20 2020 2020 2020 2020   == s].         
-0000c670: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-0000c680: 2320 6272 6561 6b20 7469 6573 2075 7369  # break ties usi
-0000c690: 6e67 2074 6865 206c 6578 6963 6f67 7261  ng the lexicogra
-0000c6a0: 7068 6963 206f 7264 6572 696e 6720 6f6e  phic ordering on
-0000c6b0: 2074 7570 6c65 7320 6769 7665 6e20 7462   tuples given tb
-0000c6c0: 5f72 616e 6b69 6e67 0a20 2020 2020 2020  _ranking.       
-0000c6d0: 2020 2020 2073 6f72 7465 645f 6564 6765       sorted_edge
-0000c6e0: 7320 3d20 736f 7274 6564 2865 6467 6573  s = sorted(edges
-0000c6f0: 2c20 6b65 7920 3d20 6c61 6d62 6461 2065  , key = lambda e
-0000c700: 3a20 2874 625f 7261 6e6b 696e 672e 696e  : (tb_ranking.in
-0000c710: 6465 7828 655b 305d 292c 2074 625f 7261  dex(e[0]), tb_ra
-0000c720: 6e6b 696e 672e 696e 6465 7828 655b 315d  nking.index(e[1]
-0000c730: 2929 2c20 7265 7665 7273 653d 4661 6c73  )), reverse=Fals
-0000c740: 6529 0a20 2020 2020 2020 2020 2020 2066  e).            f
-0000c750: 6f72 2065 302c 6531 2c73 2069 6e20 736f  or e0,e1,s in so
-0000c760: 7274 6564 5f65 6467 6573 3a20 0a20 2020  rted_edges: .   
-0000c770: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000c780: 6e6f 7420 7276 5f64 6566 6561 742e 505b  not rv_defeat.P[
-0000c790: 6361 6e64 5f74 6f5f 6369 6478 5b65 315d  cand_to_cidx[e1]
-0000c7a0: 5d5b 6361 6e64 5f74 6f5f 6369 6478 5b65  ][cand_to_cidx[e
-0000c7b0: 305d 5d20 616e 6420 6c65 6e28 7276 5f64  0]] and len(rv_d
-0000c7c0: 6566 6561 742e 7072 6564 735b 6361 6e64  efeat.preds[cand
-0000c7d0: 5f74 6f5f 6369 6478 5b65 315d 5d29 203d  _to_cidx[e1]]) =
-0000c7e0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-0000c7f0: 2020 2020 2020 2020 2072 765f 6465 6665           rv_defe
-0000c800: 6174 2e61 6464 2863 616e 645f 746f 5f63  at.add(cand_to_c
-0000c810: 6964 785b 6530 5d2c 6361 6e64 5f74 6f5f  idx[e0],cand_to_
-0000c820: 6369 6478 5b65 315d 290a 2020 2020 2020  cidx[e1]).      
-0000c830: 2020 2020 2020 7769 6e6e 6572 732e 6170        winners.ap
-0000c840: 7065 6e64 2863 6964 785f 746f 5f63 616e  pend(cidx_to_can
-0000c850: 645b 7276 5f64 6566 6561 742e 696e 6974  d[rv_defeat.init
-0000c860: 6961 6c5f 656c 656d 656e 7473 2829 5b30  ial_elements()[0
-0000c870: 5d5d 290a 2020 2020 7265 7475 726e 2073  ]]).    return s
-0000c880: 6f72 7465 6428 6c69 7374 2873 6574 2877  orted(list(set(w
-0000c890: 696e 6e65 7273 2929 290a 0a0a 4076 6d28  inners)))...@vm(
-0000c8a0: 6e61 6d65 3d22 5269 7665 7220 5a54 2229  name="River ZT")
-0000c8b0: 0a64 6566 2072 6976 6572 5f7a 7428 7072  .def river_zt(pr
-0000c8c0: 6f66 696c 652c 2063 7572 725f 6361 6e64  ofile, curr_cand
-0000c8d0: 7320 3d20 4e6f 6e65 2c20 7374 7265 6e67  s = None, streng
-0000c8e0: 7468 5f66 756e 6374 696f 6e20 3d20 4e6f  th_function = No
-0000c8f0: 6e65 293a 2020 200a 2020 2020 2222 2252  ne):   .    """R
-0000c900: 6976 6572 2077 6865 7265 2061 2066 6978  iver where a fix
-0000c910: 6564 2076 6f74 6572 2062 7265 616b 7320  ed voter breaks 
-0000c920: 616e 7920 7469 6573 2069 6e20 7468 6520  any ties in the 
-0000c930: 6d61 7267 696e 732e 2020 4974 2069 7320  margins.  It is 
-0000c940: 616c 7761 7973 2074 6865 2076 6f74 6572  always the voter
-0000c950: 2069 6e20 706f 7369 7469 6f6e 2030 2074   in position 0 t
-0000c960: 6861 7420 6272 6561 6b73 2074 6865 2074  hat breaks the t
-0000c970: 6965 732e 2020 5369 6e63 6520 766f 7465  ies.  Since vote
-0000c980: 7273 2068 6176 6520 7374 7269 6374 2070  rs have strict p
-0000c990: 7265 6665 7265 6e63 6573 2c20 7468 6973  references, this
-0000c9a0: 206d 6574 686f 6420 6973 2072 6573 6f6c   method is resol
-0000c9b0: 7574 652e 2020 0a0a 2020 2020 4172 6773  ute.  ..    Args
-0000c9c0: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
-0000c9d0: 2850 726f 6669 6c65 293a 2041 2070 726f  (Profile): A pro
-0000c9e0: 6669 6c65 206f 6620 6c69 6e65 6172 206f  file of linear o
-0000c9f0: 7264 6572 730a 2020 2020 2020 2020 6375  rders.        cu
-0000ca00: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
-0000ca10: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
-0000ca20: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
-0000ca30: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
-0000ca40: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
-0000ca50: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
-0000ca60: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
-0000ca70: 6375 7272 5f63 616e 6473 6060 0a0a 2020  curr_cands``..  
-0000ca80: 2020 5265 7475 726e 733a 200a 2020 2020    Returns: .    
-0000ca90: 2020 2020 4120 736f 7274 6564 206c 6973      A sorted lis
-0000caa0: 7420 6f66 2063 616e 6469 6461 7465 732e  t of candidates.
-0000cab0: 200a 0a20 2020 202e 2e20 7365 6561 6c73   ..    .. seeals
-0000cac0: 6f3a 3a0a 0a20 2020 2020 2020 203a 6d65  o::..        :me
-0000cad0: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
-0000cae0: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-0000caf0: 686f 6473 2e72 6976 6572 602c 203a 6d65  hods.river`, :me
-0000cb00: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
-0000cb10: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-0000cb20: 686f 6473 2e72 6976 6572 5f77 6974 685f  hods.river_with_
-0000cb30: 7465 7374 602c 203a 6d65 7468 3a60 7072  test`, :meth:`pr
-0000cb40: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-0000cb50: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
-0000cb60: 616e 6b65 645f 7061 6972 7360 0a0a 2020  anked_pairs`..  
-0000cb70: 2020 0a20 2020 2022 2222 0a20 2020 2063    .    """.    c
-0000cb80: 616e 6469 6461 7465 7320 3d20 7072 6f66  andidates = prof
-0000cb90: 696c 652e 6361 6e64 6964 6174 6573 2069  ile.candidates i
-0000cba0: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
-0000cbb0: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
-0000cbc0: 616e 6473 2020 2020 0a20 2020 200a 2020  ands    .    .  
-0000cbd0: 2020 2320 7468 6520 7469 652d 6272 6561    # the tie-brea
-0000cbe0: 6b65 7220 6973 2061 6c77 6179 7320 7468  ker is always th
-0000cbf0: 6520 6669 7273 7420 766f 7465 722e 200a  e first voter. .
-0000cc00: 2020 2020 7462 5f72 616e 6b69 6e67 203d      tb_ranking =
-0000cc10: 2074 7570 6c65 285b 6320 666f 7220 6320   tuple([c for c 
-0000cc20: 696e 206c 6973 7428 7072 6f66 696c 652e  in list(profile.
-0000cc30: 5f72 616e 6b69 6e67 735b 305d 2920 6966  _rankings[0]) if
-0000cc40: 2063 2069 6e20 6361 6e64 6964 6174 6573   c in candidates
-0000cc50: 5d29 0a20 2020 200a 2020 2020 7265 7475  ]).    .    retu
-0000cc60: 726e 2072 6976 6572 5f74 6228 7072 6f66  rn river_tb(prof
-0000cc70: 696c 652c 2063 7572 725f 6361 6e64 7320  ile, curr_cands 
-0000cc80: 3d20 6375 7272 5f63 616e 6473 2c20 7469  = curr_cands, ti
-0000cc90: 655f 6272 6561 6b65 7220 3d20 7462 5f72  e_breaker = tb_r
-0000cca0: 616e 6b69 6e67 2c20 7374 7265 6e67 7468  anking, strength
-0000ccb0: 5f66 756e 6374 696f 6e20 3d20 7374 7265  _function = stre
-0000ccc0: 6e67 7468 5f66 756e 6374 696f 6e29 0a20  ngth_function). 
-0000ccd0: 2020 200a 0a23 2053 696d 706c 6520 5374     ..# Simple St
-0000cce0: 6162 6c65 2056 6f74 696e 6720 0a64 6566  able Voting .def
-0000ccf0: 205f 7369 6d70 6c65 5f73 7461 626c 655f   _simple_stable_
-0000cd00: 766f 7469 6e67 2863 7572 725f 6361 6e64  voting(curr_cand
-0000cd10: 732c 200a 2020 2020 2020 2020 2020 2020  s, .            
-0000cd20: 2020 2020 2020 2020 2020 2020 2020 736f                so
-0000cd30: 7274 6564 5f6d 6174 6368 6573 2c0a 2020  rted_matches,.  
+0000be20: 2020 2072 765f 6465 6665 6174 2e61 6464     rv_defeat.add
+0000be30: 2863 616e 645f 746f 5f63 6964 785b 6530  (cand_to_cidx[e0
+0000be40: 5d2c 6361 6e64 5f74 6f5f 6369 6478 5b65  ],cand_to_cidx[e
+0000be50: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
+0000be60: 2020 2020 7769 6e6e 6572 732e 6170 7065      winners.appe
+0000be70: 6e64 2863 6964 785f 746f 5f63 616e 645b  nd(cidx_to_cand[
+0000be80: 7276 5f64 6566 6561 742e 696e 6974 6961  rv_defeat.initia
+0000be90: 6c5f 656c 656d 656e 7473 2829 5b30 5d5d  l_elements()[0]]
+0000bea0: 290a 2020 2020 7265 7475 726e 2073 6f72  ).    return sor
+0000beb0: 7465 6428 6c69 7374 2873 6574 2877 696e  ted(list(set(win
+0000bec0: 6e65 7273 2929 290a 0a0a 4076 6d28 6e61  ners)))...@vm(na
+0000bed0: 6d65 3d22 5269 7665 7220 5442 2229 0a64  me="River TB").d
+0000bee0: 6566 2072 6976 6572 5f74 6228 6564 6174  ef river_tb(edat
+0000bef0: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
+0000bf00: 4e6f 6e65 2c20 7469 655f 6272 6561 6b65  None, tie_breake
+0000bf10: 7220 3d20 4e6f 6e65 2c20 7374 7265 6e67  r = None, streng
+0000bf20: 7468 5f66 756e 6374 696f 6e20 3d20 4e6f  th_function = No
+0000bf30: 6e65 293a 2020 200a 2020 2020 2222 220a  ne):   .    """.
+0000bf40: 2020 2020 5269 7665 7220 7769 7468 2061      River with a
+0000bf50: 2066 6978 6564 206c 696e 6561 7220 6f72   fixed linear or
+0000bf60: 6465 7220 6f6e 2074 6865 2063 616e 6469  der on the candi
+0000bf70: 6461 7465 7320 746f 2062 7265 616b 2061  dates to break a
+0000bf80: 6e79 2074 6965 7320 696e 2074 6865 206d  ny ties in the m
+0000bf90: 6172 6769 6e73 2e20 2053 696e 6365 2074  argins.  Since t
+0000bfa0: 6865 2074 6965 5f62 7265 616b 6572 2069  he tie_breaker i
+0000bfb0: 7320 6120 6c69 6e65 6172 206f 7264 6572  s a linear order
+0000bfc0: 2c20 7468 6973 206d 6574 686f 6420 6973  , this method is
+0000bfd0: 2072 6573 6f6c 7574 652e 2020 200a 0a20   resolute.   .. 
+0000bfe0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000bff0: 2065 6461 7461 2028 5072 6f66 696c 652c   edata (Profile,
+0000c000: 2050 726f 6669 6c65 5769 7468 5469 6573   ProfileWithTies
+0000c010: 2c20 4d61 7267 696e 4772 6170 6829 3a20  , MarginGraph): 
+0000c020: 416e 7920 656c 6563 7469 6f6e 2064 6174  Any election dat
+0000c030: 6120 7468 6174 2068 6173 2061 2060 6d61  a that has a `ma
+0000c040: 7267 696e 6020 6d65 7468 6f64 2e20 0a20  rgin` method. . 
+0000c050: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
+0000c060: 7320 284c 6973 745b 696e 745d 2c20 6f70  s (List[int], op
+0000c070: 7469 6f6e 616c 293a 2049 6620 7365 742c  tional): If set,
+0000c080: 2074 6865 6e20 6669 6e64 2074 6865 2077   then find the w
+0000c090: 696e 6e65 7273 2066 6f72 2074 6865 2070  inners for the p
+0000c0a0: 726f 6669 6c65 2072 6573 7472 6963 7465  rofile restricte
+0000c0b0: 6420 746f 2074 6865 2063 616e 6469 6461  d to the candida
+0000c0c0: 7465 7320 696e 2060 6063 7572 725f 6361  tes in ``curr_ca
+0000c0d0: 6e64 7360 600a 2020 2020 2020 2020 7469  nds``.        ti
+0000c0e0: 655f 6272 6561 6b65 7220 284c 6973 745b  e_breaker (List[
+0000c0f0: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
+0000c100: 2041 206c 696e 6561 7220 6f72 6465 7220   A linear order 
+0000c110: 6f6e 2074 6865 2063 616e 6469 6461 7465  on the candidate
+0000c120: 732e 2020 4966 206e 6f74 2073 6574 2c20  s.  If not set, 
+0000c130: 7468 656e 2074 6865 2063 616e 6469 6461  then the candida
+0000c140: 7465 7320 6172 6520 736f 7274 6564 2069  tes are sorted i
+0000c150: 6e20 6173 6365 6e64 696e 6720 6f72 6465  n ascending orde
+0000c160: 722e 0a20 2020 2020 2020 2073 7472 656e  r..        stren
+0000c170: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
+0000c180: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
+0000c190: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
+0000c1a0: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
+0000c1b0: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
+0000c1c0: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
+0000c1d0: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
+0000c1e0: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
+0000c1f0: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
+0000c200: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
+0000c210: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
+0000c220: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
+0000c230: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
+0000c240: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
+0000c250: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
+0000c260: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
+0000c270: 616e 6469 6461 7465 732e 200a 0a0a 2020  andidates. ...  
+0000c280: 2020 2222 220a 2020 2020 6361 6e64 6964    """.    candid
+0000c290: 6174 6573 203d 2065 6461 7461 2e63 616e  ates = edata.can
+0000c2a0: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
+0000c2b0: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
+0000c2c0: 7365 2063 7572 725f 6361 6e64 7320 2020  se curr_cands   
+0000c2d0: 200a 2020 2020 6369 6478 5f74 6f5f 6361   .    cidx_to_ca
+0000c2e0: 6e64 203d 207b 6369 6478 3a20 6320 666f  nd = {cidx: c fo
+0000c2f0: 7220 6369 6478 2c20 6320 696e 2065 6e75  r cidx, c in enu
+0000c300: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
+0000c310: 7329 7d20 200a 2020 2020 6361 6e64 5f74  s)}  .    cand_t
+0000c320: 6f5f 6369 6478 203d 207b 633a 2063 6964  o_cidx = {c: cid
+0000c330: 7820 666f 7220 6369 6478 2c20 6320 696e  x for cidx, c in
+0000c340: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
+0000c350: 6461 7465 7329 7d20 200a 2020 2020 7374  dates)}  .    st
+0000c360: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+0000c370: 3d20 6564 6174 612e 6d61 7267 696e 2069  = edata.margin i
+0000c380: 6620 7374 7265 6e67 7468 5f66 756e 6374  f strength_funct
+0000c390: 696f 6e20 6973 204e 6f6e 6520 656c 7365  ion is None else
+0000c3a0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000c3b0: 6f6e 2020 2020 0a0a 2020 2020 7462 5f72  on    ..    tb_r
+0000c3c0: 616e 6b69 6e67 203d 2074 6965 5f62 7265  anking = tie_bre
+0000c3d0: 616b 6572 2069 6620 7469 655f 6272 6561  aker if tie_brea
+0000c3e0: 6b65 7220 6973 206e 6f74 204e 6f6e 6520  ker is not None 
+0000c3f0: 656c 7365 2073 6f72 7465 6428 6c69 7374  else sorted(list
+0000c400: 2863 616e 6469 6461 7465 7329 290a 0a20  (candidates)).. 
+0000c410: 2020 2063 7720 3d20 6564 6174 612e 636f     cw = edata.co
+0000c420: 6e64 6f72 6365 745f 7769 6e6e 6572 2863  ndorcet_winner(c
+0000c430: 7572 725f 6361 6e64 733d 6375 7272 5f63  urr_cands=curr_c
+0000c440: 616e 6473 290a 2020 2020 2320 5269 7665  ands).    # Rive
+0000c450: 7220 6973 2043 6f6e 646f 7263 6574 2063  r is Condorcet c
+0000c460: 6f6e 7369 7374 656e 742c 2073 6f20 7369  onsistent, so si
+0000c470: 6d70 6c79 2072 6574 7572 6e20 7468 6520  mply return the 
+0000c480: 436f 6e64 6f72 6365 7420 7769 6e6e 6572  Condorcet winner
+0000c490: 2069 6620 6578 6973 7473 0a20 2020 2069   if exists.    i
+0000c4a0: 6620 6377 2069 7320 6e6f 7420 4e6f 6e65  f cw is not None
+0000c4b0: 3a20 0a20 2020 2020 2020 2077 696e 6e65  : .        winne
+0000c4c0: 7273 203d 205b 6377 5d0a 2020 2020 656c  rs = [cw].    el
+0000c4d0: 7365 3a0a 2020 2020 2020 2020 775f 6564  se:.        w_ed
+0000c4e0: 6765 7320 3d20 5b28 6331 2c20 6332 2c20  ges = [(c1, c2, 
+0000c4f0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+0000c500: 6e28 6331 2c20 6332 2929 2066 6f72 2063  n(c1, c2)) for c
+0000c510: 3120 696e 2063 616e 6469 6461 7465 7320  1 in candidates 
+0000c520: 666f 7220 6332 2069 6e20 6361 6e64 6964  for c2 in candid
+0000c530: 6174 6573 2069 6620 6331 2021 3d20 6332  ates if c1 != c2
+0000c540: 2061 6e64 2028 6564 6174 612e 6d61 6a6f   and (edata.majo
+0000c550: 7269 7479 5f70 7265 6665 7273 2863 312c  rity_prefers(c1,
+0000c560: 2063 3229 206f 7220 6564 6174 612e 6973   c2) or edata.is
+0000c570: 5f74 6965 6428 6331 2c20 6332 2929 5d0a  _tied(c1, c2))].
+0000c580: 2020 2020 2020 2020 7769 6e6e 6572 7320          winners 
+0000c590: 3d20 6c69 7374 2829 2020 0a20 2020 2020  = list()  .     
+0000c5a0: 2020 2073 7472 656e 6774 6873 203d 2073     strengths = s
+0000c5b0: 6f72 7465 6428 6c69 7374 2873 6574 285b  orted(list(set([
+0000c5c0: 655b 325d 2066 6f72 2065 2069 6e20 775f  e[2] for e in w_
+0000c5d0: 6564 6765 735d 2929 2c20 7265 7665 7273  edges])), revers
+0000c5e0: 653d 5472 7565 290a 0a20 2020 2020 2020  e=True)..       
+0000c5f0: 2072 765f 6465 6665 6174 203d 2053 504f   rv_defeat = SPO
+0000c600: 286c 656e 2863 616e 6469 6461 7465 7329  (len(candidates)
+0000c610: 290a 0a20 2020 2020 2020 2066 6f72 2073  )..        for s
+0000c620: 2069 6e20 7374 7265 6e67 7468 733a 200a   in strengths: .
+0000c630: 2020 2020 2020 2020 2020 2020 6564 6765              edge
+0000c640: 7320 3d20 5b65 2066 6f72 2065 2069 6e20  s = [e for e in 
+0000c650: 775f 6564 6765 7320 6966 2065 5b32 5d20  w_edges if e[2] 
+0000c660: 3d3d 2073 5d0a 2020 2020 2020 2020 2020  == s].          
+0000c670: 2020 0a20 2020 2020 2020 2020 2020 2023    .            #
+0000c680: 2062 7265 616b 2074 6965 7320 7573 696e   break ties usin
+0000c690: 6720 7468 6520 6c65 7869 636f 6772 6170  g the lexicograp
+0000c6a0: 6869 6320 6f72 6465 7269 6e67 206f 6e20  hic ordering on 
+0000c6b0: 7475 706c 6573 2067 6976 656e 2074 625f  tuples given tb_
+0000c6c0: 7261 6e6b 696e 670a 2020 2020 2020 2020  ranking.        
+0000c6d0: 2020 2020 736f 7274 6564 5f65 6467 6573      sorted_edges
+0000c6e0: 203d 2073 6f72 7465 6428 6564 6765 732c   = sorted(edges,
+0000c6f0: 206b 6579 203d 206c 616d 6264 6120 653a   key = lambda e:
+0000c700: 2028 7462 5f72 616e 6b69 6e67 2e69 6e64   (tb_ranking.ind
+0000c710: 6578 2865 5b30 5d29 2c20 7462 5f72 616e  ex(e[0]), tb_ran
+0000c720: 6b69 6e67 2e69 6e64 6578 2865 5b31 5d29  king.index(e[1])
+0000c730: 292c 2072 6576 6572 7365 3d46 616c 7365  ), reverse=False
+0000c740: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0000c750: 7220 6530 2c65 312c 7320 696e 2073 6f72  r e0,e1,s in sor
+0000c760: 7465 645f 6564 6765 733a 200a 2020 2020  ted_edges: .    
+0000c770: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000c780: 6f74 2072 765f 6465 6665 6174 2e50 5b63  ot rv_defeat.P[c
+0000c790: 616e 645f 746f 5f63 6964 785b 6531 5d5d  and_to_cidx[e1]]
+0000c7a0: 5b63 616e 645f 746f 5f63 6964 785b 6530  [cand_to_cidx[e0
+0000c7b0: 5d5d 2061 6e64 206c 656e 2872 765f 6465  ]] and len(rv_de
+0000c7c0: 6665 6174 2e70 7265 6473 5b63 616e 645f  feat.preds[cand_
+0000c7d0: 746f 5f63 6964 785b 6531 5d5d 2920 3d3d  to_cidx[e1]]) ==
+0000c7e0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0000c7f0: 2020 2020 2020 2020 7276 5f64 6566 6561          rv_defea
+0000c800: 742e 6164 6428 6361 6e64 5f74 6f5f 6369  t.add(cand_to_ci
+0000c810: 6478 5b65 305d 2c63 616e 645f 746f 5f63  dx[e0],cand_to_c
+0000c820: 6964 785b 6531 5d29 0a20 2020 2020 2020  idx[e1]).       
+0000c830: 2020 2020 2077 696e 6e65 7273 2e61 7070       winners.app
+0000c840: 656e 6428 6369 6478 5f74 6f5f 6361 6e64  end(cidx_to_cand
+0000c850: 5b72 765f 6465 6665 6174 2e69 6e69 7469  [rv_defeat.initi
+0000c860: 616c 5f65 6c65 6d65 6e74 7328 295b 305d  al_elements()[0]
+0000c870: 5d29 0a20 2020 2072 6574 7572 6e20 736f  ]).    return so
+0000c880: 7274 6564 286c 6973 7428 7365 7428 7769  rted(list(set(wi
+0000c890: 6e6e 6572 7329 2929 0a0a 0a40 766d 286e  nners)))...@vm(n
+0000c8a0: 616d 653d 2252 6976 6572 205a 5422 290a  ame="River ZT").
+0000c8b0: 6465 6620 7269 7665 725f 7a74 2870 726f  def river_zt(pro
+0000c8c0: 6669 6c65 2c20 6375 7272 5f63 616e 6473  file, curr_cands
+0000c8d0: 203d 204e 6f6e 652c 2073 7472 656e 6774   = None, strengt
+0000c8e0: 685f 6675 6e63 7469 6f6e 203d 204e 6f6e  h_function = Non
+0000c8f0: 6529 3a20 2020 0a20 2020 2022 2222 5269  e):   .    """Ri
+0000c900: 7665 7220 7768 6572 6520 6120 6669 7865  ver where a fixe
+0000c910: 6420 766f 7465 7220 6272 6561 6b73 2061  d voter breaks a
+0000c920: 6e79 2074 6965 7320 696e 2074 6865 206d  ny ties in the m
+0000c930: 6172 6769 6e73 2e20 2049 7420 6973 2061  argins.  It is a
+0000c940: 6c77 6179 7320 7468 6520 766f 7465 7220  lways the voter 
+0000c950: 696e 2070 6f73 6974 696f 6e20 3020 7468  in position 0 th
+0000c960: 6174 2062 7265 616b 7320 7468 6520 7469  at breaks the ti
+0000c970: 6573 2e20 2053 696e 6365 2076 6f74 6572  es.  Since voter
+0000c980: 7320 6861 7665 2073 7472 6963 7420 7072  s have strict pr
+0000c990: 6566 6572 656e 6365 732c 2074 6869 7320  eferences, this 
+0000c9a0: 6d65 7468 6f64 2069 7320 7265 736f 6c75  method is resolu
+0000c9b0: 7465 2e20 200a 0a20 2020 2041 7267 733a  te.  ..    Args:
+0000c9c0: 0a20 2020 2020 2020 2065 6461 7461 2028  .        edata (
+0000c9d0: 5072 6f66 696c 6529 3a20 4120 7072 6f66  Profile): A prof
+0000c9e0: 696c 6520 6f66 206c 696e 6561 7220 6f72  ile of linear or
+0000c9f0: 6465 7273 0a20 2020 2020 2020 2063 7572  ders.        cur
+0000ca00: 725f 6361 6e64 7320 284c 6973 745b 696e  r_cands (List[in
+0000ca10: 745d 2c20 6f70 7469 6f6e 616c 293a 2049  t], optional): I
+0000ca20: 6620 7365 742c 2074 6865 6e20 6669 6e64  f set, then find
+0000ca30: 2074 6865 2077 696e 6e65 7273 2066 6f72   the winners for
+0000ca40: 2074 6865 2070 726f 6669 6c65 2072 6573   the profile res
+0000ca50: 7472 6963 7465 6420 746f 2074 6865 2063  tricted to the c
+0000ca60: 616e 6469 6461 7465 7320 696e 2060 6063  andidates in ``c
+0000ca70: 7572 725f 6361 6e64 7360 600a 0a20 2020  urr_cands``..   
+0000ca80: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
+0000ca90: 2020 2041 2073 6f72 7465 6420 6c69 7374     A sorted list
+0000caa0: 206f 6620 6361 6e64 6964 6174 6573 2e20   of candidates. 
+0000cab0: 0a0a 2020 2020 2e2e 2073 6565 616c 736f  ..    .. seealso
+0000cac0: 3a3a 0a0a 2020 2020 2020 2020 3a6d 6574  ::..        :met
+0000cad0: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
+0000cae0: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+0000caf0: 6f64 732e 7269 7665 7260 2c20 3a6d 6574  ods.river`, :met
+0000cb00: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
+0000cb10: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+0000cb20: 6f64 732e 7269 7665 725f 7769 7468 5f74  ods.river_with_t
+0000cb30: 6573 7460 2c20 3a6d 6574 683a 6070 7265  est`, :meth:`pre
+0000cb40: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+0000cb50: 6261 7365 645f 6d65 7468 6f64 732e 7261  based_methods.ra
+0000cb60: 6e6b 6564 5f70 6169 7273 600a 0a20 2020  nked_pairs`..   
+0000cb70: 200a 2020 2020 2222 220a 2020 2020 6361   .    """.    ca
+0000cb80: 6e64 6964 6174 6573 203d 2070 726f 6669  ndidates = profi
+0000cb90: 6c65 2e63 616e 6469 6461 7465 7320 6966  le.candidates if
+0000cba0: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
+0000cbb0: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
+0000cbc0: 6e64 7320 2020 200a 2020 2020 0a20 2020  nds    .    .   
+0000cbd0: 2023 2074 6865 2074 6965 2d62 7265 616b   # the tie-break
+0000cbe0: 6572 2069 7320 616c 7761 7973 2074 6865  er is always the
+0000cbf0: 2066 6972 7374 2076 6f74 6572 2e20 0a20   first voter. . 
+0000cc00: 2020 2074 625f 7261 6e6b 696e 6720 3d20     tb_ranking = 
+0000cc10: 7475 706c 6528 5b63 2066 6f72 2063 2069  tuple([c for c i
+0000cc20: 6e20 6c69 7374 2870 726f 6669 6c65 2e5f  n list(profile._
+0000cc30: 7261 6e6b 696e 6773 5b30 5d29 2069 6620  rankings[0]) if 
+0000cc40: 6320 696e 2063 616e 6469 6461 7465 735d  c in candidates]
+0000cc50: 290a 2020 2020 0a20 2020 2072 6574 7572  ).    .    retur
+0000cc60: 6e20 7269 7665 725f 7462 2870 726f 6669  n river_tb(profi
+0000cc70: 6c65 2c20 6375 7272 5f63 616e 6473 203d  le, curr_cands =
+0000cc80: 2063 7572 725f 6361 6e64 732c 2074 6965   curr_cands, tie
+0000cc90: 5f62 7265 616b 6572 203d 2074 625f 7261  _breaker = tb_ra
+0000cca0: 6e6b 696e 672c 2073 7472 656e 6774 685f  nking, strength_
+0000ccb0: 6675 6e63 7469 6f6e 203d 2073 7472 656e  function = stren
+0000ccc0: 6774 685f 6675 6e63 7469 6f6e 290a 2020  gth_function).  
+0000ccd0: 2020 0a0a 2320 5369 6d70 6c65 2053 7461    ..# Simple Sta
+0000cce0: 626c 6520 566f 7469 6e67 200a 6465 6620  ble Voting .def 
+0000ccf0: 5f73 696d 706c 655f 7374 6162 6c65 5f76  _simple_stable_v
+0000cd00: 6f74 696e 6728 6375 7272 5f63 616e 6473  oting(curr_cands
+0000cd10: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
+0000cd20: 2020 2020 2020 2020 2020 2020 2073 6f72               sor
+0000cd30: 7465 645f 6d61 7463 6865 732c 0a20 2020  ted_matches,.   
 0000cd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd50: 2020 2020 2020 2020 6d65 6d5f 7376 5f77          mem_sv_w
-0000cd60: 696e 6e65 7273 293a 0a20 2020 2027 2727  inners):.    '''
-0000cd70: 0a20 2020 2044 6574 6572 6d69 6e65 2074  .    Determine t
-0000cd80: 6865 2053 696d 706c 6520 5374 6162 6c65  he Simple Stable
-0000cd90: 2056 6f74 696e 6720 7769 6e6e 6572 7320   Voting winners 
-0000cda0: 7768 696c 6520 6b65 6570 696e 6720 7472  while keeping tr
-0000cdb0: 6163 6b20 0a20 2020 206f 6620 7468 6520  ack .    of the 
-0000cdc0: 7769 6e6e 6572 7320 696e 2061 6e79 2073  winners in any s
-0000cdd0: 7562 7072 6f66 696c 6573 2063 6865 636b  ubprofiles check
-0000cde0: 6564 2064 7572 696e 6720 636f 6d70 7574  ed during comput
-0000cdf0: 6174 696f 6e2e 200a 2020 2020 2727 270a  ation. .    '''.
-0000ce00: 2020 2020 0a20 2020 2073 765f 7769 6e6e      .    sv_winn
-0000ce10: 6572 7320 3d20 6c69 7374 2829 0a20 2020  ers = list().   
-0000ce20: 2020 2020 200a 2020 2020 6966 206c 656e       .    if len
-0000ce30: 2863 7572 725f 6361 6e64 7329 203d 3d20  (curr_cands) == 
-0000ce40: 313a 200a 2020 2020 2020 2020 6d65 6d5f  1: .        mem_
-0000ce50: 7376 5f77 696e 6e65 7273 5b74 7570 6c65  sv_winners[tuple
-0000ce60: 2863 7572 725f 6361 6e64 7329 5d20 3d20  (curr_cands)] = 
-0000ce70: 6375 7272 5f63 616e 6473 0a20 2020 2020  curr_cands.     
-0000ce80: 2020 2072 6574 7572 6e20 6375 7272 5f63     return curr_c
-0000ce90: 616e 6473 2c20 6d65 6d5f 7376 5f77 696e  ands, mem_sv_win
-0000cea0: 6e65 7273 0a20 2020 200a 2020 2020 6d61  ners.    .    ma
-0000ceb0: 7267 696e 5f77 6974 6e65 7373 696e 675f  rgin_witnessing_
-0000cec0: 7769 6e20 3d20 2d6d 6174 682e 696e 660a  win = -math.inf.
-0000ced0: 0a20 2020 2066 6f72 2061 2c20 622c 2073  .    for a, b, s
-0000cee0: 2069 6e20 736f 7274 6564 5f6d 6174 6368   in sorted_match
-0000cef0: 6573 3a0a 2020 2020 2020 2020 6966 2073  es:.        if s
-0000cf00: 203c 206d 6172 6769 6e5f 7769 746e 6573   < margin_witnes
-0000cf10: 7369 6e67 5f77 696e 3a20 0a20 2020 2020  sing_win: .     
-0000cf20: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-0000cf30: 2020 2020 2069 6620 6120 6e6f 7420 696e       if a not in
-0000cf40: 2073 765f 7769 6e6e 6572 733a 200a 2020   sv_winners: .  
-0000cf50: 2020 2020 2020 2020 2020 6361 6e64 735f            cands_
-0000cf60: 6d69 6e75 735f 6220 3d20 5b63 2066 6f72  minus_b = [c for
-0000cf70: 2063 2069 6e20 6375 7272 5f63 616e 6473   c in curr_cands
-0000cf80: 2069 6620 6320 213d 2062 5d0a 2020 2020   if c != b].    
-0000cf90: 2020 2020 2020 2020 6361 6e64 735f 6d69          cands_mi
-0000cfa0: 6e75 735f 625f 6b65 7920 3d20 7475 706c  nus_b_key = tupl
-0000cfb0: 6528 736f 7274 6564 2863 616e 6473 5f6d  e(sorted(cands_m
-0000cfc0: 696e 7573 5f62 2929 0a20 2020 2020 2020  inus_b)).       
-0000cfd0: 2020 2020 2069 6620 6361 6e64 735f 6d69       if cands_mi
-0000cfe0: 6e75 735f 625f 6b65 7920 6e6f 7420 696e  nus_b_key not in
-0000cff0: 206d 656d 5f73 765f 7769 6e6e 6572 732e   mem_sv_winners.
-0000d000: 6b65 7973 2829 3a20 0a20 2020 2020 2020  keys(): .       
-0000d010: 2020 2020 2020 2020 2077 732c 206d 656d           ws, mem
-0000d020: 5f73 765f 7769 6e6e 6572 7320 3d20 5f73  _sv_winners = _s
-0000d030: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
-0000d040: 696e 6728 6375 7272 5f63 616e 6473 203d  ing(curr_cands =
-0000d050: 2063 616e 6473 5f6d 696e 7573 5f62 2c0a   cands_minus_b,.
+0000cd50: 2020 2020 2020 206d 656d 5f73 765f 7769         mem_sv_wi
+0000cd60: 6e6e 6572 7329 3a0a 2020 2020 2727 270a  nners):.    '''.
+0000cd70: 2020 2020 4465 7465 726d 696e 6520 7468      Determine th
+0000cd80: 6520 5369 6d70 6c65 2053 7461 626c 6520  e Simple Stable 
+0000cd90: 566f 7469 6e67 2077 696e 6e65 7273 2077  Voting winners w
+0000cda0: 6869 6c65 206b 6565 7069 6e67 2074 7261  hile keeping tra
+0000cdb0: 636b 200a 2020 2020 6f66 2074 6865 2077  ck .    of the w
+0000cdc0: 696e 6e65 7273 2069 6e20 616e 7920 7375  inners in any su
+0000cdd0: 6270 726f 6669 6c65 7320 6368 6563 6b65  bprofiles checke
+0000cde0: 6420 6475 7269 6e67 2063 6f6d 7075 7461  d during computa
+0000cdf0: 7469 6f6e 2e20 0a20 2020 2027 2727 0a20  tion. .    '''. 
+0000ce00: 2020 200a 2020 2020 7376 5f77 696e 6e65     .    sv_winne
+0000ce10: 7273 203d 206c 6973 7428 290a 2020 2020  rs = list().    
+0000ce20: 2020 2020 0a20 2020 2069 6620 6c65 6e28      .    if len(
+0000ce30: 6375 7272 5f63 616e 6473 2920 3d3d 2031  curr_cands) == 1
+0000ce40: 3a20 0a20 2020 2020 2020 206d 656d 5f73  : .        mem_s
+0000ce50: 765f 7769 6e6e 6572 735b 7475 706c 6528  v_winners[tuple(
+0000ce60: 6375 7272 5f63 616e 6473 295d 203d 2063  curr_cands)] = c
+0000ce70: 7572 725f 6361 6e64 730a 2020 2020 2020  urr_cands.      
+0000ce80: 2020 7265 7475 726e 2063 7572 725f 6361    return curr_ca
+0000ce90: 6e64 732c 206d 656d 5f73 765f 7769 6e6e  nds, mem_sv_winn
+0000cea0: 6572 730a 2020 2020 0a20 2020 206d 6172  ers.    .    mar
+0000ceb0: 6769 6e5f 7769 746e 6573 7369 6e67 5f77  gin_witnessing_w
+0000cec0: 696e 203d 202d 6d61 7468 2e69 6e66 0a0a  in = -math.inf..
+0000ced0: 2020 2020 666f 7220 612c 2062 2c20 7320      for a, b, s 
+0000cee0: 696e 2073 6f72 7465 645f 6d61 7463 6865  in sorted_matche
+0000cef0: 733a 0a20 2020 2020 2020 2069 6620 7320  s:.        if s 
+0000cf00: 3c20 6d61 7267 696e 5f77 6974 6e65 7373  < margin_witness
+0000cf10: 696e 675f 7769 6e3a 200a 2020 2020 2020  ing_win: .      
+0000cf20: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
+0000cf30: 2020 2020 6966 2061 206e 6f74 2069 6e20      if a not in 
+0000cf40: 7376 5f77 696e 6e65 7273 3a20 0a20 2020  sv_winners: .   
+0000cf50: 2020 2020 2020 2020 2063 616e 6473 5f6d           cands_m
+0000cf60: 696e 7573 5f62 203d 205b 6320 666f 7220  inus_b = [c for 
+0000cf70: 6320 696e 2063 7572 725f 6361 6e64 7320  c in curr_cands 
+0000cf80: 6966 2063 2021 3d20 625d 0a20 2020 2020  if c != b].     
+0000cf90: 2020 2020 2020 2063 616e 6473 5f6d 696e         cands_min
+0000cfa0: 7573 5f62 5f6b 6579 203d 2074 7570 6c65  us_b_key = tuple
+0000cfb0: 2873 6f72 7465 6428 6361 6e64 735f 6d69  (sorted(cands_mi
+0000cfc0: 6e75 735f 6229 290a 2020 2020 2020 2020  nus_b)).        
+0000cfd0: 2020 2020 6966 2063 616e 6473 5f6d 696e      if cands_min
+0000cfe0: 7573 5f62 5f6b 6579 206e 6f74 2069 6e20  us_b_key not in 
+0000cff0: 6d65 6d5f 7376 5f77 696e 6e65 7273 2e6b  mem_sv_winners.k
+0000d000: 6579 7328 293a 200a 2020 2020 2020 2020  eys(): .        
+0000d010: 2020 2020 2020 2020 7773 2c20 6d65 6d5f          ws, mem_
+0000d020: 7376 5f77 696e 6e65 7273 203d 205f 7369  sv_winners = _si
+0000d030: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
+0000d040: 6e67 2863 7572 725f 6361 6e64 7320 3d20  ng(curr_cands = 
+0000d050: 6361 6e64 735f 6d69 6e75 735f 622c 0a20  cands_minus_b,. 
 0000d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d090: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
-0000d0a0: 645f 6d61 7463 6865 7320 3d20 5b28 612c  d_matches = [(a,
-0000d0b0: 2063 2c20 7329 2066 6f72 2061 2c20 632c   c, s) for a, c,
-0000d0c0: 2073 2069 6e20 736f 7274 6564 5f6d 6174   s in sorted_mat
-0000d0d0: 6368 6573 2069 6620 6120 213d 2062 2061  ches if a != b a
-0000d0e0: 6e64 2063 2021 3d20 625d 2c0a 2020 2020  nd c != b],.    
+0000d090: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
+0000d0a0: 5f6d 6174 6368 6573 203d 205b 2861 2c20  _matches = [(a, 
+0000d0b0: 632c 2073 2920 666f 7220 612c 2063 2c20  c, s) for a, c, 
+0000d0c0: 7320 696e 2073 6f72 7465 645f 6d61 7463  s in sorted_matc
+0000d0d0: 6865 7320 6966 2061 2021 3d20 6220 616e  hes if a != b an
+0000d0e0: 6420 6320 213d 2062 5d2c 0a20 2020 2020  d c != b],.     
 0000d0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d120: 2020 2020 2020 206d 656d 5f73 765f 7769         mem_sv_wi
-0000d130: 6e6e 6572 7320 3d20 6d65 6d5f 7376 5f77  nners = mem_sv_w
-0000d140: 696e 6e65 7273 290a 2020 2020 2020 2020  inners).        
-0000d150: 2020 2020 2020 2020 6d65 6d5f 7376 5f77          mem_sv_w
-0000d160: 696e 6e65 7273 5b63 616e 6473 5f6d 696e  inners[cands_min
-0000d170: 7573 5f62 5f6b 6579 5d20 3d20 7773 0a20  us_b_key] = ws. 
-0000d180: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000d190: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0000d1a0: 2020 7773 203d 206d 656d 5f73 765f 7769    ws = mem_sv_wi
-0000d1b0: 6e6e 6572 735b 6361 6e64 735f 6d69 6e75  nners[cands_minu
-0000d1c0: 735f 625f 6b65 795d 0a20 2020 2020 2020  s_b_key].       
-0000d1d0: 2020 2020 2069 6620 6120 696e 2077 733a       if a in ws:
-0000d1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d1f0: 2073 765f 7769 6e6e 6572 732e 6170 7065   sv_winners.appe
-0000d200: 6e64 2861 290a 2020 2020 2020 2020 2020  nd(a).          
-0000d210: 2020 2020 2020 6d61 7267 696e 5f77 6974        margin_wit
-0000d220: 6e65 7373 696e 675f 7769 6e20 3d20 730a  nessing_win = s.
-0000d230: 0a20 2020 2072 6574 7572 6e20 7376 5f77  .    return sv_w
-0000d240: 696e 6e65 7273 2c20 6d65 6d5f 7376 5f77  inners, mem_sv_w
-0000d250: 696e 6e65 7273 0a20 2020 200a 4076 6d28  inners.    .@vm(
-0000d260: 6e61 6d65 203d 2022 5369 6d70 6c65 2053  name = "Simple S
-0000d270: 7461 626c 6520 566f 7469 6e67 2229 0a64  table Voting").d
-0000d280: 6566 2073 696d 706c 655f 7374 6162 6c65  ef simple_stable
-0000d290: 5f76 6f74 696e 6728 6564 6174 612c 2063  _voting(edata, c
-0000d2a0: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
-0000d2b0: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
-0000d2c0: 696f 6e20 3d20 4e6f 6e65 293a 200a 2020  ion = None): .  
-0000d2d0: 2020 2222 2249 6d70 6c65 6d65 6e74 6174    """Implementat
-0000d2e0: 696f 6e20 6f66 2053 696d 706c 6520 5374  ion of Simple St
-0000d2f0: 6162 6c65 2056 6f74 696e 6720 6672 6f6d  able Voting from
-0000d300: 2068 7474 7073 3a2f 2f61 7278 6976 2e6f   https://arxiv.o
-0000d310: 7267 2f61 6273 2f32 3130 382e 3030 3534  rg/abs/2108.0054
-0000d320: 322e 200a 0a20 2020 2053 696d 706c 6520  2. ..    Simple 
-0000d330: 5374 6162 6c65 2056 6f74 696e 6720 6973  Stable Voting is
-0000d340: 2061 2072 6563 7572 7369 7665 2076 6f74   a recursive vot
-0000d350: 696e 6720 6d65 7468 6f64 2064 6566 696e  ing method defin
-0000d360: 6564 2061 7320 666f 6c6c 6f77 733a 200a  ed as follows: .
-0000d370: 0a20 2020 2031 2e20 4966 2074 6865 7265  .    1. If there
-0000d380: 2069 7320 6f6e 6c79 206f 6e65 2063 616e   is only one can
-0000d390: 6469 6461 7465 2069 6e20 7468 6520 7072  didate in the pr
-0000d3a0: 6f66 696c 652c 2074 6865 6e20 7468 6174  ofile, then that
-0000d3b0: 2063 616e 6469 6461 7465 2069 7320 7468   candidate is th
-0000d3c0: 6520 7769 6e6e 6572 2e20 0a20 2020 2032  e winner. .    2
-0000d3d0: 2e20 4f72 6465 7220 7468 6520 7061 6972  . Order the pair
-0000d3e0: 7320 3a6d 6174 683a 6028 612c 6229 6020  s :math:`(a,b)` 
-0000d3f0: 6f66 2063 616e 6469 6461 7465 7320 6672  of candidates fr
-0000d400: 6f6d 206c 6172 6765 7374 2074 6f20 736d  om largest to sm
-0000d410: 616c 6c65 7374 2076 616c 7565 206f 6620  allest value of 
-0000d420: 7468 6520 6d61 7267 696e 206f 6620 3a6d  the margin of :m
-0000d430: 6174 683a 6061 6020 6f76 6572 203a 6d61  ath:`a` over :ma
-0000d440: 7468 3a60 6260 2c20 616e 6420 6465 636c  th:`b`, and decl
-0000d450: 6172 6520 6173 2053 696d 706c 6520 5374  are as Simple St
-0000d460: 6162 6c65 2056 6f74 696e 6720 7769 6e6e  able Voting winn
-0000d470: 6572 7320 7468 6520 6361 6e64 6964 6174  ers the candidat
-0000d480: 6528 7329 203a 6d61 7468 3a60 6160 2066  e(s) :math:`a` f
-0000d490: 726f 6d20 7468 6520 6561 726c 6965 7374  rom the earliest
-0000d4a0: 2070 6169 7228 7329 203a 6d61 7468 3a60   pair(s) :math:`
-0000d4b0: 2861 2c62 2960 2073 7563 6820 7468 6174  (a,b)` such that
-0000d4c0: 203a 6d61 7468 3a60 6160 2069 7320 6120   :math:`a` is a 
-0000d4d0: 5369 6d70 6c65 2053 7461 626c 6520 566f  Simple Stable Vo
-0000d4e0: 7469 6e67 2077 696e 6e65 7220 696e 2074  ting winner in t
-0000d4f0: 6865 2065 6c65 6374 696f 6e20 7769 7468  he election with
-0000d500: 6f75 7420 3a6d 6174 683a 6062 602e 200a  out :math:`b`. .
-0000d510: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-0000d520: 2020 2065 6461 7461 2028 5072 6f66 696c     edata (Profil
-0000d530: 652c 2050 726f 6669 6c65 5769 7468 5469  e, ProfileWithTi
-0000d540: 6573 2c20 4d61 7267 696e 4772 6170 6829  es, MarginGraph)
-0000d550: 3a20 416e 7920 656c 6563 7469 6f6e 2064  : Any election d
-0000d560: 6174 6120 7468 6174 2068 6173 2061 2060  ata that has a `
-0000d570: 6d61 7267 696e 6020 6d65 7468 6f64 2e20  margin` method. 
-0000d580: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
-0000d590: 6e64 7320 284c 6973 745b 696e 745d 2c20  nds (List[int], 
-0000d5a0: 6f70 7469 6f6e 616c 293a 2049 6620 7365  optional): If se
-0000d5b0: 742c 2074 6865 6e20 6669 6e64 2074 6865  t, then find the
-0000d5c0: 2077 696e 6e65 7273 2066 6f72 2074 6865   winners for the
-0000d5d0: 2070 726f 6669 6c65 2072 6573 7472 6963   profile restric
-0000d5e0: 7465 6420 746f 2074 6865 2063 616e 6469  ted to the candi
-0000d5f0: 6461 7465 7320 696e 2060 6063 7572 725f  dates in ``curr_
-0000d600: 6361 6e64 7360 600a 2020 2020 2020 2020  cands``.        
-0000d610: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000d620: 6e20 2866 756e 6374 696f 6e2c 206f 7074  n (function, opt
-0000d630: 696f 6e61 6c29 3a20 5468 6520 7374 7265  ional): The stre
-0000d640: 6e67 7468 2066 756e 6374 696f 6e20 746f  ngth function to
-0000d650: 2062 6520 7573 6564 2074 6f20 6361 6c63   be used to calc
-0000d660: 756c 6174 6520 7468 6520 7374 7265 6e67  ulate the streng
-0000d670: 7468 206f 6620 6120 7061 7468 2e20 2020  th of a path.   
-0000d680: 5468 6520 6465 6661 756c 7420 6973 2074  The default is t
-0000d690: 6865 206d 6172 6769 6e20 6d65 7468 6f64  he margin method
-0000d6a0: 206f 6620 6060 6564 6174 6160 602e 2020   of ``edata``.  
-0000d6b0: 2054 6869 7320 6f6e 6c79 206d 6174 7465   This only matte
-0000d6c0: 7273 2077 6865 6e20 7468 6520 6261 6c6c  rs when the ball
-0000d6d0: 6f74 7320 6172 6520 6e6f 7420 6c69 6e65  ots are not line
-0000d6e0: 6172 206f 7264 6572 732e 200a 0a20 2020  ar orders. ..   
-0000d6f0: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
-0000d700: 2020 2041 2073 6f72 7465 6420 6c69 7374     A sorted list
-0000d710: 206f 6620 6361 6e64 6964 6174 6573 2e20   of candidates. 
-0000d720: 0a0a 2020 2020 2e2e 2073 6565 616c 736f  ..    .. seealso
-0000d730: 3a3a 0a0a 2020 2020 2020 2020 3a6d 6574  ::..        :met
-0000d740: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
-0000d750: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-0000d760: 6f64 732e 7369 6d70 6c65 5f73 7461 626c  ods.simple_stabl
-0000d770: 655f 766f 7469 6e67 5f66 6173 7465 7260  e_voting_faster`
-0000d780: 2c20 3a6d 6574 683a 6070 7265 665f 766f  , :meth:`pref_vo
-0000d790: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
-0000d7a0: 645f 6d65 7468 6f64 732e 7374 6162 6c65  d_methods.stable
-0000d7b0: 5f76 6f74 696e 6760 0a0a 0a20 2020 203a  _voting`...    :
-0000d7c0: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
-0000d7d0: 2e20 6578 6563 5f63 6f64 653a 3a0a 0a20  . exec_code::.. 
-0000d7e0: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
-0000d7f0: 5f76 6f74 696e 672e 7765 6967 6874 6564  _voting.weighted
-0000d800: 5f6d 616a 6f72 6974 795f 6772 6170 6873  _majority_graphs
-0000d810: 2069 6d70 6f72 7420 4d61 7267 696e 4772   import MarginGr
-0000d820: 6170 680a 2020 2020 2020 2020 6672 6f6d  aph.        from
-0000d830: 2070 7265 665f 766f 7469 6e67 2e6d 6172   pref_voting.mar
-0000d840: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
-0000d850: 7320 696d 706f 7274 2073 696d 706c 655f  s import simple_
-0000d860: 7374 6162 6c65 5f76 6f74 696e 670a 0a20  stable_voting.. 
-0000d870: 2020 2020 2020 206d 6720 3d20 4d61 7267         mg = Marg
-0000d880: 696e 4772 6170 6828 5b30 2c20 312c 2032  inGraph([0, 1, 2
-0000d890: 2c20 335d 2c20 5b28 302c 2033 2c20 3829  , 3], [(0, 3, 8)
-0000d8a0: 2c20 2831 2c20 302c 2031 3029 2c20 2832  , (1, 0, 10), (2
-0000d8b0: 2c20 302c 2034 292c 2028 322c 2031 2c20  , 0, 4), (2, 1, 
-0000d8c0: 3829 2c20 2833 2c20 312c 2038 295d 290a  8), (3, 1, 8)]).
-0000d8d0: 0a20 2020 2020 2020 2073 696d 706c 655f  .        simple_
-0000d8e0: 7374 6162 6c65 5f76 6f74 696e 672e 6469  stable_voting.di
-0000d8f0: 7370 6c61 7928 6d67 290a 0a20 2020 2022  splay(mg)..    "
-0000d900: 2222 0a20 2020 200a 2020 2020 6375 7272  "".    .    curr
-0000d910: 5f63 616e 6473 203d 2065 6461 7461 2e63  _cands = edata.c
-0000d920: 616e 6469 6461 7465 7320 6966 2063 7572  andidates if cur
-0000d930: 725f 6361 6e64 7320 6973 204e 6f6e 6520  r_cands is None 
-0000d940: 656c 7365 2063 7572 725f 6361 6e64 730a  else curr_cands.
-0000d950: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
-0000d960: 6374 696f 6e20 3d20 6564 6174 612e 6d61  ction = edata.ma
-0000d970: 7267 696e 2069 6620 7374 7265 6e67 7468  rgin if strength
-0000d980: 5f66 756e 6374 696f 6e20 6973 204e 6f6e  _function is Non
-0000d990: 6520 656c 7365 2073 7472 656e 6774 685f  e else strength_
-0000d9a0: 6675 6e63 7469 6f6e 2020 0a0a 2020 2020  function  ..    
-0000d9b0: 6d61 7463 6865 7320 3d20 5b28 612c 2062  matches = [(a, b
-0000d9c0: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
-0000d9d0: 696f 6e28 612c 2062 2929 2066 6f72 2061  ion(a, b)) for a
-0000d9e0: 2069 6e20 6375 7272 5f63 616e 6473 2066   in curr_cands f
-0000d9f0: 6f72 2062 2069 6e20 6375 7272 5f63 616e  or b in curr_can
-0000da00: 6473 2069 6620 6120 213d 2062 5d0a 2020  ds if a != b].  
-0000da10: 2020 736f 7274 6564 5f6d 6174 6368 6573    sorted_matches
-0000da20: 203d 2073 6f72 7465 6428 6d61 7463 6865   = sorted(matche
-0000da30: 732c 2072 6576 6572 7365 3d54 7275 652c  s, reverse=True,
-0000da40: 206b 6579 3d6c 616d 6264 6120 6d5f 775f   key=lambda m_w_
-0000da50: 7765 6967 6874 3a20 6d5f 775f 7765 6967  weight: m_w_weig
-0000da60: 6874 5b32 5d29 0a20 2020 200a 2020 2020  ht[2]).    .    
-0000da70: 7265 7475 726e 2073 6f72 7465 6428 5f73  return sorted(_s
-0000da80: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
-0000da90: 696e 6728 6375 7272 5f63 616e 6473 203d  ing(curr_cands =
-0000daa0: 2063 7572 725f 6361 6e64 732c 200a 2020   curr_cands, .  
+0000d120: 2020 2020 2020 6d65 6d5f 7376 5f77 696e        mem_sv_win
+0000d130: 6e65 7273 203d 206d 656d 5f73 765f 7769  ners = mem_sv_wi
+0000d140: 6e6e 6572 7329 0a20 2020 2020 2020 2020  nners).         
+0000d150: 2020 2020 2020 206d 656d 5f73 765f 7769         mem_sv_wi
+0000d160: 6e6e 6572 735b 6361 6e64 735f 6d69 6e75  nners[cands_minu
+0000d170: 735f 625f 6b65 795d 203d 2077 730a 2020  s_b_key] = ws.  
+0000d180: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
+0000d190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d1a0: 2077 7320 3d20 6d65 6d5f 7376 5f77 696e   ws = mem_sv_win
+0000d1b0: 6e65 7273 5b63 616e 6473 5f6d 696e 7573  ners[cands_minus
+0000d1c0: 5f62 5f6b 6579 5d0a 2020 2020 2020 2020  _b_key].        
+0000d1d0: 2020 2020 6966 2061 2069 6e20 7773 3a0a      if a in ws:.
+0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1f0: 7376 5f77 696e 6e65 7273 2e61 7070 656e  sv_winners.appen
+0000d200: 6428 6129 0a20 2020 2020 2020 2020 2020  d(a).           
+0000d210: 2020 2020 206d 6172 6769 6e5f 7769 746e       margin_witn
+0000d220: 6573 7369 6e67 5f77 696e 203d 2073 0a0a  essing_win = s..
+0000d230: 2020 2020 7265 7475 726e 2073 765f 7769      return sv_wi
+0000d240: 6e6e 6572 732c 206d 656d 5f73 765f 7769  nners, mem_sv_wi
+0000d250: 6e6e 6572 730a 2020 2020 0a40 766d 286e  nners.    .@vm(n
+0000d260: 616d 6520 3d20 2253 696d 706c 6520 5374  ame = "Simple St
+0000d270: 6162 6c65 2056 6f74 696e 6722 290a 6465  able Voting").de
+0000d280: 6620 7369 6d70 6c65 5f73 7461 626c 655f  f simple_stable_
+0000d290: 766f 7469 6e67 2865 6461 7461 2c20 6375  voting(edata, cu
+0000d2a0: 7272 5f63 616e 6473 203d 204e 6f6e 652c  rr_cands = None,
+0000d2b0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000d2c0: 6f6e 203d 204e 6f6e 6529 3a20 0a20 2020  on = None): .   
+0000d2d0: 2022 2222 496d 706c 656d 656e 7461 7469   """Implementati
+0000d2e0: 6f6e 206f 6620 5369 6d70 6c65 2053 7461  on of Simple Sta
+0000d2f0: 626c 6520 566f 7469 6e67 2066 726f 6d20  ble Voting from 
+0000d300: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+0000d310: 672f 6162 732f 3231 3038 2e30 3035 3432  g/abs/2108.00542
+0000d320: 2e20 0a0a 2020 2020 5369 6d70 6c65 2053  . ..    Simple S
+0000d330: 7461 626c 6520 566f 7469 6e67 2069 7320  table Voting is 
+0000d340: 6120 7265 6375 7273 6976 6520 766f 7469  a recursive voti
+0000d350: 6e67 206d 6574 686f 6420 6465 6669 6e65  ng method define
+0000d360: 6420 6173 2066 6f6c 6c6f 7773 3a20 0a0a  d as follows: ..
+0000d370: 2020 2020 312e 2049 6620 7468 6572 6520      1. If there 
+0000d380: 6973 206f 6e6c 7920 6f6e 6520 6361 6e64  is only one cand
+0000d390: 6964 6174 6520 696e 2074 6865 2070 726f  idate in the pro
+0000d3a0: 6669 6c65 2c20 7468 656e 2074 6861 7420  file, then that 
+0000d3b0: 6361 6e64 6964 6174 6520 6973 2074 6865  candidate is the
+0000d3c0: 2077 696e 6e65 722e 200a 2020 2020 322e   winner. .    2.
+0000d3d0: 204f 7264 6572 2074 6865 2070 6169 7273   Order the pairs
+0000d3e0: 203a 6d61 7468 3a60 2861 2c62 2960 206f   :math:`(a,b)` o
+0000d3f0: 6620 6361 6e64 6964 6174 6573 2066 726f  f candidates fro
+0000d400: 6d20 6c61 7267 6573 7420 746f 2073 6d61  m largest to sma
+0000d410: 6c6c 6573 7420 7661 6c75 6520 6f66 2074  llest value of t
+0000d420: 6865 206d 6172 6769 6e20 6f66 203a 6d61  he margin of :ma
+0000d430: 7468 3a60 6160 206f 7665 7220 3a6d 6174  th:`a` over :mat
+0000d440: 683a 6062 602c 2061 6e64 2064 6563 6c61  h:`b`, and decla
+0000d450: 7265 2061 7320 5369 6d70 6c65 2053 7461  re as Simple Sta
+0000d460: 626c 6520 566f 7469 6e67 2077 696e 6e65  ble Voting winne
+0000d470: 7273 2074 6865 2063 616e 6469 6461 7465  rs the candidate
+0000d480: 2873 2920 3a6d 6174 683a 6061 6020 6672  (s) :math:`a` fr
+0000d490: 6f6d 2074 6865 2065 6172 6c69 6573 7420  om the earliest 
+0000d4a0: 7061 6972 2873 2920 3a6d 6174 683a 6028  pair(s) :math:`(
+0000d4b0: 612c 6229 6020 7375 6368 2074 6861 7420  a,b)` such that 
+0000d4c0: 3a6d 6174 683a 6061 6020 6973 2061 2053  :math:`a` is a S
+0000d4d0: 696d 706c 6520 5374 6162 6c65 2056 6f74  imple Stable Vot
+0000d4e0: 696e 6720 7769 6e6e 6572 2069 6e20 7468  ing winner in th
+0000d4f0: 6520 656c 6563 7469 6f6e 2077 6974 686f  e election witho
+0000d500: 7574 203a 6d61 7468 3a60 6260 2e20 0a0a  ut :math:`b`. ..
+0000d510: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000d520: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
+0000d530: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
+0000d540: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
+0000d550: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
+0000d560: 7461 2074 6861 7420 6861 7320 6120 606d  ta that has a `m
+0000d570: 6172 6769 6e60 206d 6574 686f 642e 200a  argin` method. .
+0000d580: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
+0000d590: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
+0000d5a0: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
+0000d5b0: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
+0000d5c0: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
+0000d5d0: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
+0000d5e0: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
+0000d5f0: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
+0000d600: 616e 6473 6060 0a20 2020 2020 2020 2073  ands``.        s
+0000d610: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000d620: 2028 6675 6e63 7469 6f6e 2c20 6f70 7469   (function, opti
+0000d630: 6f6e 616c 293a 2054 6865 2073 7472 656e  onal): The stren
+0000d640: 6774 6820 6675 6e63 7469 6f6e 2074 6f20  gth function to 
+0000d650: 6265 2075 7365 6420 746f 2063 616c 6375  be used to calcu
+0000d660: 6c61 7465 2074 6865 2073 7472 656e 6774  late the strengt
+0000d670: 6820 6f66 2061 2070 6174 682e 2020 2054  h of a path.   T
+0000d680: 6865 2064 6566 6175 6c74 2069 7320 7468  he default is th
+0000d690: 6520 6d61 7267 696e 206d 6574 686f 6420  e margin method 
+0000d6a0: 6f66 2060 6065 6461 7461 6060 2e20 2020  of ``edata``.   
+0000d6b0: 5468 6973 206f 6e6c 7920 6d61 7474 6572  This only matter
+0000d6c0: 7320 7768 656e 2074 6865 2062 616c 6c6f  s when the ballo
+0000d6d0: 7473 2061 7265 206e 6f74 206c 696e 6561  ts are not linea
+0000d6e0: 7220 6f72 6465 7273 2e20 0a0a 2020 2020  r orders. ..    
+0000d6f0: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
+0000d700: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
+0000d710: 6f66 2063 616e 6469 6461 7465 732e 200a  of candidates. .
+0000d720: 0a20 2020 202e 2e20 7365 6561 6c73 6f3a  .    .. seealso:
+0000d730: 3a0a 0a20 2020 2020 2020 203a 6d65 7468  :..        :meth
+0000d740: 3a60 7072 6566 5f76 6f74 696e 672e 6d61  :`pref_voting.ma
+0000d750: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+0000d760: 6473 2e73 696d 706c 655f 7374 6162 6c65  ds.simple_stable
+0000d770: 5f76 6f74 696e 675f 6661 7374 6572 602c  _voting_faster`,
+0000d780: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
+0000d790: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
+0000d7a0: 5f6d 6574 686f 6473 2e73 7461 626c 655f  _methods.stable_
+0000d7b0: 766f 7469 6e67 600a 0a0a 2020 2020 3a45  voting`...    :E
+0000d7c0: 7861 6d70 6c65 3a20 0a0a 2020 2020 2e2e  xample: ..    ..
+0000d7d0: 2065 7865 635f 636f 6465 3a3a 0a0a 2020   exec_code::..  
+0000d7e0: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+0000d7f0: 766f 7469 6e67 2e77 6569 6768 7465 645f  voting.weighted_
+0000d800: 6d61 6a6f 7269 7479 5f67 7261 7068 7320  majority_graphs 
+0000d810: 696d 706f 7274 204d 6172 6769 6e47 7261  import MarginGra
+0000d820: 7068 0a20 2020 2020 2020 2066 726f 6d20  ph.        from 
+0000d830: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+0000d840: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+0000d850: 2069 6d70 6f72 7420 7369 6d70 6c65 5f73   import simple_s
+0000d860: 7461 626c 655f 766f 7469 6e67 0a0a 2020  table_voting..  
+0000d870: 2020 2020 2020 6d67 203d 204d 6172 6769        mg = Margi
+0000d880: 6e47 7261 7068 285b 302c 2031 2c20 322c  nGraph([0, 1, 2,
+0000d890: 2033 5d2c 205b 2830 2c20 332c 2038 292c   3], [(0, 3, 8),
+0000d8a0: 2028 312c 2030 2c20 3130 292c 2028 322c   (1, 0, 10), (2,
+0000d8b0: 2030 2c20 3429 2c20 2832 2c20 312c 2038   0, 4), (2, 1, 8
+0000d8c0: 292c 2028 332c 2031 2c20 3829 5d29 0a0a  ), (3, 1, 8)])..
+0000d8d0: 2020 2020 2020 2020 7369 6d70 6c65 5f73          simple_s
+0000d8e0: 7461 626c 655f 766f 7469 6e67 2e64 6973  table_voting.dis
+0000d8f0: 706c 6179 286d 6729 0a0a 2020 2020 2222  play(mg)..    ""
+0000d900: 220a 2020 2020 0a20 2020 2063 7572 725f  ".    .    curr_
+0000d910: 6361 6e64 7320 3d20 6564 6174 612e 6361  cands = edata.ca
+0000d920: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
+0000d930: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
+0000d940: 6c73 6520 6375 7272 5f63 616e 6473 0a20  lse curr_cands. 
+0000d950: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+0000d960: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
+0000d970: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
+0000d980: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
+0000d990: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
+0000d9a0: 756e 6374 696f 6e20 200a 0a20 2020 206d  unction  ..    m
+0000d9b0: 6174 6368 6573 203d 205b 2861 2c20 622c  atches = [(a, b,
+0000d9c0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000d9d0: 6f6e 2861 2c20 6229 2920 666f 7220 6120  on(a, b)) for a 
+0000d9e0: 696e 2063 7572 725f 6361 6e64 7320 666f  in curr_cands fo
+0000d9f0: 7220 6220 696e 2063 7572 725f 6361 6e64  r b in curr_cand
+0000da00: 7320 6966 2061 2021 3d20 625d 0a20 2020  s if a != b].   
+0000da10: 2073 6f72 7465 645f 6d61 7463 6865 7320   sorted_matches 
+0000da20: 3d20 736f 7274 6564 286d 6174 6368 6573  = sorted(matches
+0000da30: 2c20 7265 7665 7273 653d 5472 7565 2c20  , reverse=True, 
+0000da40: 6b65 793d 6c61 6d62 6461 206d 5f77 5f77  key=lambda m_w_w
+0000da50: 6569 6768 743a 206d 5f77 5f77 6569 6768  eight: m_w_weigh
+0000da60: 745b 325d 290a 2020 2020 0a20 2020 2072  t[2]).    .    r
+0000da70: 6574 7572 6e20 736f 7274 6564 285f 7369  eturn sorted(_si
+0000da80: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
+0000da90: 6e67 2863 7572 725f 6361 6e64 7320 3d20  ng(curr_cands = 
+0000daa0: 6375 7272 5f63 616e 6473 2c20 0a20 2020  curr_cands, .   
 0000dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dad0: 2020 2020 2020 736f 7274 6564 5f6d 6174        sorted_mat
-0000dae0: 6368 6573 203d 2073 6f72 7465 645f 6d61  ches = sorted_ma
-0000daf0: 7463 6865 732c 0a20 2020 2020 2020 2020  tches,.         
+0000dad0: 2020 2020 2073 6f72 7465 645f 6d61 7463       sorted_matc
+0000dae0: 6865 7320 3d20 736f 7274 6564 5f6d 6174  hes = sorted_mat
+0000daf0: 6368 6573 2c0a 2020 2020 2020 2020 2020  ches,.          
 0000db00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db10: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000db20: 656d 5f73 765f 7769 6e6e 6572 7320 3d20  em_sv_winners = 
-0000db30: 7b7d 295b 305d 290a 0a40 766d 286e 616d  {})[0])..@vm(nam
-0000db40: 6520 3d20 2253 696d 706c 6520 5374 6162  e = "Simple Stab
-0000db50: 6c65 2056 6f74 696e 6722 290a 6465 6620  le Voting").def 
-0000db60: 7369 6d70 6c65 5f73 7461 626c 655f 766f  simple_stable_vo
-0000db70: 7469 6e67 5f66 6173 7465 7228 6564 6174  ting_faster(edat
-0000db80: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
-0000db90: 4e6f 6e65 2c20 7374 7265 6e67 7468 5f66  None, strength_f
-0000dba0: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
-0000dbb0: 200a 2020 2020 2222 2253 696d 706c 6520   .    """Simple 
-0000dbc0: 5374 6162 6c65 2056 6f74 696e 6720 6973  Stable Voting is
-0000dbd0: 2043 6f6e 646f 7263 6574 2063 6f6e 7369   Condorcet consi
-0000dbe0: 7374 656e 742e 2020 2049 7420 6973 2066  stent.   It is f
-0000dbf0: 6173 7465 7220 746f 2073 6b69 7020 6578  aster to skip ex
-0000dc00: 6563 7574 696e 6720 7468 6520 7265 6375  ecuting the recu
-0000dc10: 7273 6976 6520 616c 676f 7269 7468 6d20  rsive algorithm 
-0000dc20: 7768 656e 2074 6865 7265 2069 7320 6120  when there is a 
-0000dc30: 436f 6e64 6f72 6365 7420 7769 6e6e 6572  Condorcet winner
-0000dc40: 4669 7273 7420 6368 6563 6b20 6966 2074  First check if t
-0000dc50: 6865 7265 2069 7320 6120 436f 6e64 6f72  here is a Condor
-0000dc60: 6365 7420 7769 6e6e 6572 2e20 2049 6620  cet winner.  If 
-0000dc70: 736f 2c20 7265 7475 726e 2074 6865 2043  so, return the C
-0000dc80: 6f6e 646f 7263 6574 2077 696e 6e65 722c  ondorcet winner,
-0000dc90: 206f 7468 6572 7769 7365 2066 696e 6420   otherwise find 
-0000dca0: 7468 6520 5369 6d70 6c65 2053 7461 626c  the Simple Stabl
-0000dcb0: 6520 566f 7469 6e67 2077 696e 6e65 7220  e Voting winner 
-0000dcc0: 7573 696e 6720 5f73 696d 706c 655f 7374  using _simple_st
-0000dcd0: 6162 6c65 5f76 6f74 696e 670a 0a20 2020  able_voting..   
-0000dce0: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
-0000dcf0: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
-0000dd00: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
-0000dd10: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
-0000dd20: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
-0000dd30: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
-0000dd40: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
-0000dd50: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-0000dd60: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-0000dd70: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-0000dd80: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-0000dd90: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-0000dda0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-0000ddb0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-0000ddc0: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-0000ddd0: 7360 600a 2020 2020 2020 2020 7374 7265  s``.        stre
-0000dde0: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
-0000ddf0: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
-0000de00: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
-0000de10: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
-0000de20: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
-0000de30: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
-0000de40: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
-0000de50: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
-0000de60: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
-0000de70: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
-0000de80: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
-0000de90: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
-0000dea0: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
-0000deb0: 7264 6572 732e 200a 0a20 2020 2052 6574  rders. ..    Ret
-0000dec0: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
-0000ded0: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
-0000dee0: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
-0000def0: 2020 2e2e 2073 6565 616c 736f 3a3a 0a0a    .. seealso::..
-0000df00: 2020 2020 2020 2020 3a6d 6574 683a 6070          :meth:`p
-0000df10: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-0000df20: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-0000df30: 7369 6d70 6c65 5f73 7461 626c 655f 766f  simple_stable_vo
-0000df40: 7469 6e67 602c 203a 6d65 7468 3a60 7072  ting`, :meth:`pr
-0000df50: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-0000df60: 5f62 6173 6564 5f6d 6574 686f 6473 2e73  _based_methods.s
-0000df70: 7461 626c 655f 766f 7469 6e67 600a 0a0a  table_voting`...
-0000df80: 2020 2020 3a45 7861 6d70 6c65 3a20 0a0a      :Example: ..
-0000df90: 2020 2020 2e2e 2065 7865 635f 636f 6465      .. exec_code
-0000dfa0: 3a3a 0a0a 2020 2020 2020 2020 6672 6f6d  ::..        from
-0000dfb0: 2070 7265 665f 766f 7469 6e67 2e77 6569   pref_voting.wei
-0000dfc0: 6768 7465 645f 6d61 6a6f 7269 7479 5f67  ghted_majority_g
-0000dfd0: 7261 7068 7320 696d 706f 7274 204d 6172  raphs import Mar
-0000dfe0: 6769 6e47 7261 7068 0a20 2020 2020 2020  ginGraph.       
-0000dff0: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
-0000e000: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-0000e010: 6574 686f 6473 2069 6d70 6f72 7420 7369  ethods import si
-0000e020: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
-0000e030: 6e67 2c20 7369 6d70 6c65 5f73 7461 626c  ng, simple_stabl
-0000e040: 655f 766f 7469 6e67 5f66 6173 7465 720a  e_voting_faster.
-0000e050: 0a20 2020 2020 2020 206d 6720 3d20 4d61  .        mg = Ma
-0000e060: 7267 696e 4772 6170 6828 5b30 2c20 312c  rginGraph([0, 1,
-0000e070: 2032 2c20 335d 2c20 5b28 302c 2033 2c20   2, 3], [(0, 3, 
-0000e080: 3829 2c20 2831 2c20 302c 2031 3029 2c20  8), (1, 0, 10), 
-0000e090: 2832 2c20 302c 2034 292c 2028 322c 2031  (2, 0, 4), (2, 1
-0000e0a0: 2c20 3829 2c20 2833 2c20 312c 2038 295d  , 8), (3, 1, 8)]
-0000e0b0: 290a 0a20 2020 2020 2020 2073 696d 706c  )..        simpl
-0000e0c0: 655f 7374 6162 6c65 5f76 6f74 696e 675f  e_stable_voting_
-0000e0d0: 6661 7374 6572 2e64 6973 706c 6179 286d  faster.display(m
-0000e0e0: 6729 0a20 2020 2020 2020 2073 696d 706c  g).        simpl
-0000e0f0: 655f 7374 6162 6c65 5f76 6f74 696e 672e  e_stable_voting.
-0000e100: 6469 7370 6c61 7928 6d67 290a 0a20 2020  display(mg)..   
-0000e110: 2022 2222 0a20 2020 200a 2020 2020 6377   """.    .    cw
-0000e120: 203d 2065 6461 7461 2e63 6f6e 646f 7263   = edata.condorc
-0000e130: 6574 5f77 696e 6e65 7228 6375 7272 5f63  et_winner(curr_c
-0000e140: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
-0000e150: 7329 0a20 2020 2069 6620 6377 2069 7320  s).    if cw is 
-0000e160: 6e6f 7420 4e6f 6e65 3a20 0a20 2020 2020  not None: .     
-0000e170: 2020 2072 6574 7572 6e20 5b63 775d 0a20     return [cw]. 
-0000e180: 2020 2065 6c73 653a 200a 2020 2020 2020     else: .      
-0000e190: 2020 6375 7272 5f63 616e 6473 203d 2065    curr_cands = e
-0000e1a0: 6461 7461 2e63 616e 6469 6461 7465 7320  data.candidates 
-0000e1b0: 6966 2063 7572 725f 6361 6e64 7320 6973  if curr_cands is
-0000e1c0: 204e 6f6e 6520 656c 7365 2063 7572 725f   None else curr_
-0000e1d0: 6361 6e64 730a 2020 2020 2020 2020 7374  cands.        st
-0000e1e0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-0000e1f0: 3d20 6564 6174 612e 6d61 7267 696e 2069  = edata.margin i
-0000e200: 6620 7374 7265 6e67 7468 5f66 756e 6374  f strength_funct
-0000e210: 696f 6e20 6973 204e 6f6e 6520 656c 7365  ion is None else
-0000e220: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000e230: 6f6e 2020 0a0a 2020 2020 2020 2020 6d61  on  ..        ma
-0000e240: 7463 6865 7320 3d20 5b28 612c 2062 2c20  tches = [(a, b, 
-0000e250: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000e260: 6e28 612c 2062 2929 2066 6f72 2061 2069  n(a, b)) for a i
-0000e270: 6e20 6375 7272 5f63 616e 6473 2066 6f72  n curr_cands for
-0000e280: 2062 2069 6e20 6375 7272 5f63 616e 6473   b in curr_cands
-0000e290: 2069 6620 6120 213d 2062 5d0a 2020 2020   if a != b].    
-0000e2a0: 2020 2020 736f 7274 6564 5f6d 6174 6368      sorted_match
-0000e2b0: 6573 203d 2073 6f72 7465 6428 6d61 7463  es = sorted(matc
-0000e2c0: 6865 732c 2072 6576 6572 7365 3d54 7275  hes, reverse=Tru
-0000e2d0: 652c 206b 6579 3d6c 616d 6264 6120 6d5f  e, key=lambda m_
-0000e2e0: 775f 7765 6967 6874 3a20 6d5f 775f 7765  w_weight: m_w_we
-0000e2f0: 6967 6874 5b32 5d29 0a20 2020 200a 2020  ight[2]).    .  
-0000e300: 2020 2020 2020 7265 7475 726e 2073 6f72        return sor
-0000e310: 7465 6428 5f73 696d 706c 655f 7374 6162  ted(_simple_stab
-0000e320: 6c65 5f76 6f74 696e 6728 6375 7272 5f63  le_voting(curr_c
-0000e330: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
-0000e340: 732c 200a 2020 2020 2020 2020 2020 2020  s, .            
+0000db10: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0000db20: 6d5f 7376 5f77 696e 6e65 7273 203d 207b  m_sv_winners = {
+0000db30: 7d29 5b30 5d29 0a0a 4076 6d28 6e61 6d65  })[0])..@vm(name
+0000db40: 203d 2022 5369 6d70 6c65 2053 7461 626c   = "Simple Stabl
+0000db50: 6520 566f 7469 6e67 2229 0a64 6566 2073  e Voting").def s
+0000db60: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
+0000db70: 696e 675f 6661 7374 6572 2865 6461 7461  ing_faster(edata
+0000db80: 2c20 6375 7272 5f63 616e 6473 203d 204e  , curr_cands = N
+0000db90: 6f6e 652c 2073 7472 656e 6774 685f 6675  one, strength_fu
+0000dba0: 6e63 7469 6f6e 203d 204e 6f6e 6529 3a20  nction = None): 
+0000dbb0: 0a20 2020 2022 2222 5369 6d70 6c65 2053  .    """Simple S
+0000dbc0: 7461 626c 6520 566f 7469 6e67 2069 7320  table Voting is 
+0000dbd0: 436f 6e64 6f72 6365 7420 636f 6e73 6973  Condorcet consis
+0000dbe0: 7465 6e74 2e20 2020 4974 2069 7320 6661  tent.   It is fa
+0000dbf0: 7374 6572 2074 6f20 736b 6970 2065 7865  ster to skip exe
+0000dc00: 6375 7469 6e67 2074 6865 2072 6563 7572  cuting the recur
+0000dc10: 7369 7665 2061 6c67 6f72 6974 686d 2077  sive algorithm w
+0000dc20: 6865 6e20 7468 6572 6520 6973 2061 2043  hen there is a C
+0000dc30: 6f6e 646f 7263 6574 2077 696e 6e65 7246  ondorcet winnerF
+0000dc40: 6972 7374 2063 6865 636b 2069 6620 7468  irst check if th
+0000dc50: 6572 6520 6973 2061 2043 6f6e 646f 7263  ere is a Condorc
+0000dc60: 6574 2077 696e 6e65 722e 2020 4966 2073  et winner.  If s
+0000dc70: 6f2c 2072 6574 7572 6e20 7468 6520 436f  o, return the Co
+0000dc80: 6e64 6f72 6365 7420 7769 6e6e 6572 2c20  ndorcet winner, 
+0000dc90: 6f74 6865 7277 6973 6520 6669 6e64 2074  otherwise find t
+0000dca0: 6865 2053 696d 706c 6520 5374 6162 6c65  he Simple Stable
+0000dcb0: 2056 6f74 696e 6720 7769 6e6e 6572 2075   Voting winner u
+0000dcc0: 7369 6e67 205f 7369 6d70 6c65 5f73 7461  sing _simple_sta
+0000dcd0: 626c 655f 766f 7469 6e67 0a0a 2020 2020  ble_voting..    
+0000dce0: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
+0000dcf0: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
+0000dd00: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
+0000dd10: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
+0000dd20: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
+0000dd30: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
+0000dd40: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
+0000dd50: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
+0000dd60: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
+0000dd70: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
+0000dd80: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
+0000dd90: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
+0000dda0: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
+0000ddb0: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
+0000ddc0: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
+0000ddd0: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
+0000dde0: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
+0000ddf0: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
+0000de00: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
+0000de10: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
+0000de20: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
+0000de30: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
+0000de40: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
+0000de50: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
+0000de60: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
+0000de70: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
+0000de80: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
+0000de90: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
+0000dea0: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
+0000deb0: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
+0000dec0: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
+0000ded0: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
+0000dee0: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
+0000def0: 202e 2e20 7365 6561 6c73 6f3a 3a0a 0a20   .. seealso::.. 
+0000df00: 2020 2020 2020 203a 6d65 7468 3a60 7072         :meth:`pr
+0000df10: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+0000df20: 5f62 6173 6564 5f6d 6574 686f 6473 2e73  _based_methods.s
+0000df30: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
+0000df40: 696e 6760 2c20 3a6d 6574 683a 6070 7265  ing`, :meth:`pre
+0000df50: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+0000df60: 6261 7365 645f 6d65 7468 6f64 732e 7374  based_methods.st
+0000df70: 6162 6c65 5f76 6f74 696e 6760 0a0a 0a20  able_voting`... 
+0000df80: 2020 203a 4578 616d 706c 653a 200a 0a20     :Example: .. 
+0000df90: 2020 202e 2e20 6578 6563 5f63 6f64 653a     .. exec_code:
+0000dfa0: 3a0a 0a20 2020 2020 2020 2066 726f 6d20  :..        from 
+0000dfb0: 7072 6566 5f76 6f74 696e 672e 7765 6967  pref_voting.weig
+0000dfc0: 6874 6564 5f6d 616a 6f72 6974 795f 6772  hted_majority_gr
+0000dfd0: 6170 6873 2069 6d70 6f72 7420 4d61 7267  aphs import Marg
+0000dfe0: 696e 4772 6170 680a 2020 2020 2020 2020  inGraph.        
+0000dff0: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
+0000e000: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+0000e010: 7468 6f64 7320 696d 706f 7274 2073 696d  thods import sim
+0000e020: 706c 655f 7374 6162 6c65 5f76 6f74 696e  ple_stable_votin
+0000e030: 672c 2073 696d 706c 655f 7374 6162 6c65  g, simple_stable
+0000e040: 5f76 6f74 696e 675f 6661 7374 6572 0a0a  _voting_faster..
+0000e050: 2020 2020 2020 2020 6d67 203d 204d 6172          mg = Mar
+0000e060: 6769 6e47 7261 7068 285b 302c 2031 2c20  ginGraph([0, 1, 
+0000e070: 322c 2033 5d2c 205b 2830 2c20 332c 2038  2, 3], [(0, 3, 8
+0000e080: 292c 2028 312c 2030 2c20 3130 292c 2028  ), (1, 0, 10), (
+0000e090: 322c 2030 2c20 3429 2c20 2832 2c20 312c  2, 0, 4), (2, 1,
+0000e0a0: 2038 292c 2028 332c 2031 2c20 3829 5d29   8), (3, 1, 8)])
+0000e0b0: 0a0a 2020 2020 2020 2020 7369 6d70 6c65  ..        simple
+0000e0c0: 5f73 7461 626c 655f 766f 7469 6e67 5f66  _stable_voting_f
+0000e0d0: 6173 7465 722e 6469 7370 6c61 7928 6d67  aster.display(mg
+0000e0e0: 290a 2020 2020 2020 2020 7369 6d70 6c65  ).        simple
+0000e0f0: 5f73 7461 626c 655f 766f 7469 6e67 2e64  _stable_voting.d
+0000e100: 6973 706c 6179 286d 6729 0a0a 2020 2020  isplay(mg)..    
+0000e110: 2222 220a 2020 2020 0a20 2020 2063 7720  """.    .    cw 
+0000e120: 3d20 6564 6174 612e 636f 6e64 6f72 6365  = edata.condorce
+0000e130: 745f 7769 6e6e 6572 2863 7572 725f 6361  t_winner(curr_ca
+0000e140: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
+0000e150: 290a 2020 2020 6966 2063 7720 6973 206e  ).    if cw is n
+0000e160: 6f74 204e 6f6e 653a 200a 2020 2020 2020  ot None: .      
+0000e170: 2020 7265 7475 726e 205b 6377 5d0a 2020    return [cw].  
+0000e180: 2020 656c 7365 3a20 0a20 2020 2020 2020    else: .       
+0000e190: 2063 7572 725f 6361 6e64 7320 3d20 6564   curr_cands = ed
+0000e1a0: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
+0000e1b0: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
+0000e1c0: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
+0000e1d0: 616e 6473 0a20 2020 2020 2020 2073 7472  ands.        str
+0000e1e0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+0000e1f0: 2065 6461 7461 2e6d 6172 6769 6e20 6966   edata.margin if
+0000e200: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000e210: 6f6e 2069 7320 4e6f 6e65 2065 6c73 6520  on is None else 
+0000e220: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+0000e230: 6e20 200a 0a20 2020 2020 2020 206d 6174  n  ..        mat
+0000e240: 6368 6573 203d 205b 2861 2c20 622c 2073  ches = [(a, b, s
+0000e250: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000e260: 2861 2c20 6229 2920 666f 7220 6120 696e  (a, b)) for a in
+0000e270: 2063 7572 725f 6361 6e64 7320 666f 7220   curr_cands for 
+0000e280: 6220 696e 2063 7572 725f 6361 6e64 7320  b in curr_cands 
+0000e290: 6966 2061 2021 3d20 625d 0a20 2020 2020  if a != b].     
+0000e2a0: 2020 2073 6f72 7465 645f 6d61 7463 6865     sorted_matche
+0000e2b0: 7320 3d20 736f 7274 6564 286d 6174 6368  s = sorted(match
+0000e2c0: 6573 2c20 7265 7665 7273 653d 5472 7565  es, reverse=True
+0000e2d0: 2c20 6b65 793d 6c61 6d62 6461 206d 5f77  , key=lambda m_w
+0000e2e0: 5f77 6569 6768 743a 206d 5f77 5f77 6569  _weight: m_w_wei
+0000e2f0: 6768 745b 325d 290a 2020 2020 0a20 2020  ght[2]).    .   
+0000e300: 2020 2020 2072 6574 7572 6e20 736f 7274       return sort
+0000e310: 6564 285f 7369 6d70 6c65 5f73 7461 626c  ed(_simple_stabl
+0000e320: 655f 766f 7469 6e67 2863 7572 725f 6361  e_voting(curr_ca
+0000e330: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
+0000e340: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
 0000e350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e370: 736f 7274 6564 5f6d 6174 6368 6573 203d  sorted_matches =
-0000e380: 2073 6f72 7465 645f 6d61 7463 6865 732c   sorted_matches,
-0000e390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e360: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e370: 6f72 7465 645f 6d61 7463 6865 7320 3d20  orted_matches = 
+0000e380: 736f 7274 6564 5f6d 6174 6368 6573 2c0a  sorted_matches,.
+0000e390: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3b0: 2020 2020 2020 2020 2020 2020 206d 656d               mem
-0000e3c0: 5f73 765f 7769 6e6e 6572 7320 3d20 7b7d  _sv_winners = {}
-0000e3d0: 295b 305d 290a 0a20 2020 200a 6465 6620  )[0])..    .def 
-0000e3e0: 5f73 7461 626c 655f 766f 7469 6e67 2865  _stable_voting(e
-0000e3f0: 6461 7461 2c20 0a20 2020 2020 2020 2020  data, .         
-0000e400: 2020 2020 2020 2020 2020 6375 7272 5f63            curr_c
-0000e410: 616e 6473 2c0a 2020 2020 2020 2020 2020  ands,.          
-0000e420: 2020 2020 2020 2020 2073 7472 656e 6774           strengt
-0000e430: 685f 6675 6e63 7469 6f6e 2c0a 2020 2020  h_function,.    
-0000e440: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e450: 6f72 7465 645f 6d61 7463 6865 732c 0a20  orted_matches,. 
+0000e3b0: 2020 2020 2020 2020 2020 2020 6d65 6d5f              mem_
+0000e3c0: 7376 5f77 696e 6e65 7273 203d 207b 7d29  sv_winners = {})
+0000e3d0: 5b30 5d29 0a0a 2020 2020 0a64 6566 205f  [0])..    .def _
+0000e3e0: 7374 6162 6c65 5f76 6f74 696e 6728 6564  stable_voting(ed
+0000e3f0: 6174 612c 200a 2020 2020 2020 2020 2020  ata, .          
+0000e400: 2020 2020 2020 2020 2063 7572 725f 6361           curr_ca
+0000e410: 6e64 732c 0a20 2020 2020 2020 2020 2020  nds,.           
+0000e420: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+0000e430: 5f66 756e 6374 696f 6e2c 0a20 2020 2020  _function,.     
+0000e440: 2020 2020 2020 2020 2020 2020 2020 736f                so
+0000e450: 7274 6564 5f6d 6174 6368 6573 2c0a 2020  rted_matches,.  
 0000e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e470: 2020 6d65 6d5f 7376 5f77 696e 6e65 7273    mem_sv_winners
-0000e480: 293a 200a 2020 2020 2727 270a 2020 2020  ): .    '''.    
-0000e490: 4465 7465 726d 696e 6520 7468 6520 5374  Determine the St
-0000e4a0: 6162 6c65 2056 6f74 696e 6720 7769 6e6e  able Voting winn
-0000e4b0: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
-0000e4c0: 696c 6520 7768 696c 6520 6b65 6570 696e  ile while keepin
-0000e4d0: 6720 7472 6163 6b20 6f66 2074 6865 2077  g track of the w
-0000e4e0: 696e 6e65 7273 2069 6e20 616e 7920 7375  inners in any su
-0000e4f0: 6270 726f 6669 6c65 7320 6368 6563 6b65  bprofiles checke
-0000e500: 6420 6475 7269 6e67 2063 6f6d 7075 7461  d during computa
-0000e510: 7469 6f6e 2e20 0a20 2020 2027 2727 0a20  tion. .    '''. 
-0000e520: 2020 200a 2020 2020 7376 5f77 696e 6e65     .    sv_winne
-0000e530: 7273 203d 206c 6973 7428 290a 2020 2020  rs = list().    
-0000e540: 0a20 2020 2075 6e64 6566 6561 7465 645f  .    undefeated_
-0000e550: 6361 6e64 6964 6174 6573 203d 2073 706c  candidates = spl
-0000e560: 6974 5f63 7963 6c65 2865 6461 7461 2c20  it_cycle(edata, 
-0000e570: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
-0000e580: 725f 6361 6e64 732c 2073 7472 656e 6774  r_cands, strengt
-0000e590: 685f 6675 6e63 7469 6f6e 203d 2073 7472  h_function = str
-0000e5a0: 656e 6774 685f 6675 6e63 7469 6f6e 290a  ength_function).
-0000e5b0: 0a20 2020 2069 6620 6c65 6e28 6375 7272  .    if len(curr
-0000e5c0: 5f63 616e 6473 2920 3d3d 2031 3a20 0a20  _cands) == 1: . 
-0000e5d0: 2020 2020 2020 206d 656d 5f73 765f 7769         mem_sv_wi
-0000e5e0: 6e6e 6572 735b 7475 706c 6528 6375 7272  nners[tuple(curr
-0000e5f0: 5f63 616e 6473 295d 203d 2063 7572 725f  _cands)] = curr_
-0000e600: 6361 6e64 730a 2020 2020 2020 2020 7265  cands.        re
-0000e610: 7475 726e 2063 7572 725f 6361 6e64 732c  turn curr_cands,
-0000e620: 206d 656d 5f73 765f 7769 6e6e 6572 730a   mem_sv_winners.
-0000e630: 2020 2020 0a20 2020 206d 6172 6769 6e5f      .    margin_
-0000e640: 7769 746e 6573 7369 6e67 5f77 696e 203d  witnessing_win =
-0000e650: 202d 6d61 7468 2e69 6e66 0a0a 2020 2020   -math.inf..    
-0000e660: 666f 7220 612c 2062 2c20 7320 696e 2073  for a, b, s in s
-0000e670: 6f72 7465 645f 6d61 7463 6865 733a 0a20  orted_matches:. 
-0000e680: 2020 2020 2020 2069 6620 7320 3c20 6d61         if s < ma
-0000e690: 7267 696e 5f77 6974 6e65 7373 696e 675f  rgin_witnessing_
-0000e6a0: 7769 6e3a 200a 2020 2020 2020 2020 2020  win: .          
-0000e6b0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-0000e6c0: 6966 2061 2069 6e20 756e 6465 6665 6174  if a in undefeat
-0000e6d0: 6564 5f63 616e 6469 6461 7465 7320 616e  ed_candidates an
-0000e6e0: 6420 6120 6e6f 7420 696e 2073 765f 7769  d a not in sv_wi
-0000e6f0: 6e6e 6572 733a 200a 2020 2020 2020 2020  nners: .        
-0000e700: 2020 2020 6361 6e64 735f 6d69 6e75 735f      cands_minus_
-0000e710: 6220 3d20 5b63 2066 6f72 2063 2069 6e20  b = [c for c in 
-0000e720: 6375 7272 5f63 616e 6473 2069 6620 6320  curr_cands if c 
-0000e730: 213d 2062 5d0a 2020 2020 2020 2020 2020  != b].          
-0000e740: 2020 6361 6e64 735f 6d69 6e75 735f 625f    cands_minus_b_
-0000e750: 6b65 7920 3d20 7475 706c 6528 736f 7274  key = tuple(sort
-0000e760: 6564 2863 616e 6473 5f6d 696e 7573 5f62  ed(cands_minus_b
-0000e770: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
-0000e780: 6620 6361 6e64 735f 6d69 6e75 735f 625f  f cands_minus_b_
-0000e790: 6b65 7920 6e6f 7420 696e 206d 656d 5f73  key not in mem_s
-0000e7a0: 765f 7769 6e6e 6572 732e 6b65 7973 2829  v_winners.keys()
-0000e7b0: 3a20 0a20 2020 2020 2020 2020 2020 2020  : .             
-0000e7c0: 2020 2077 732c 206d 656d 5f73 765f 7769     ws, mem_sv_wi
-0000e7d0: 6e6e 6572 7320 3d20 5f73 7461 626c 655f  nners = _stable_
-0000e7e0: 766f 7469 6e67 2865 6461 7461 2c0a 2020  voting(edata,.  
+0000e470: 206d 656d 5f73 765f 7769 6e6e 6572 7329   mem_sv_winners)
+0000e480: 3a20 0a20 2020 2027 2727 0a20 2020 2044  : .    '''.    D
+0000e490: 6574 6572 6d69 6e65 2074 6865 2053 7461  etermine the Sta
+0000e4a0: 626c 6520 566f 7469 6e67 2077 696e 6e65  ble Voting winne
+0000e4b0: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
+0000e4c0: 6c65 2077 6869 6c65 206b 6565 7069 6e67  le while keeping
+0000e4d0: 2074 7261 636b 206f 6620 7468 6520 7769   track of the wi
+0000e4e0: 6e6e 6572 7320 696e 2061 6e79 2073 7562  nners in any sub
+0000e4f0: 7072 6f66 696c 6573 2063 6865 636b 6564  profiles checked
+0000e500: 2064 7572 696e 6720 636f 6d70 7574 6174   during computat
+0000e510: 696f 6e2e 200a 2020 2020 2727 270a 2020  ion. .    '''.  
+0000e520: 2020 0a20 2020 2073 765f 7769 6e6e 6572    .    sv_winner
+0000e530: 7320 3d20 6c69 7374 2829 0a20 2020 200a  s = list().    .
+0000e540: 2020 2020 756e 6465 6665 6174 6564 5f63      undefeated_c
+0000e550: 616e 6469 6461 7465 7320 3d20 7370 6c69  andidates = spli
+0000e560: 745f 6379 636c 6528 6564 6174 612c 2063  t_cycle(edata, c
+0000e570: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
+0000e580: 5f63 616e 6473 2c20 7374 7265 6e67 7468  _cands, strength
+0000e590: 5f66 756e 6374 696f 6e20 3d20 7374 7265  _function = stre
+0000e5a0: 6e67 7468 5f66 756e 6374 696f 6e29 0a0a  ngth_function)..
+0000e5b0: 2020 2020 6966 206c 656e 2863 7572 725f      if len(curr_
+0000e5c0: 6361 6e64 7329 203d 3d20 313a 200a 2020  cands) == 1: .  
+0000e5d0: 2020 2020 2020 6d65 6d5f 7376 5f77 696e        mem_sv_win
+0000e5e0: 6e65 7273 5b74 7570 6c65 2863 7572 725f  ners[tuple(curr_
+0000e5f0: 6361 6e64 7329 5d20 3d20 6375 7272 5f63  cands)] = curr_c
+0000e600: 616e 6473 0a20 2020 2020 2020 2072 6574  ands.        ret
+0000e610: 7572 6e20 6375 7272 5f63 616e 6473 2c20  urn curr_cands, 
+0000e620: 6d65 6d5f 7376 5f77 696e 6e65 7273 0a20  mem_sv_winners. 
+0000e630: 2020 200a 2020 2020 6d61 7267 696e 5f77     .    margin_w
+0000e640: 6974 6e65 7373 696e 675f 7769 6e20 3d20  itnessing_win = 
+0000e650: 2d6d 6174 682e 696e 660a 0a20 2020 2066  -math.inf..    f
+0000e660: 6f72 2061 2c20 622c 2073 2069 6e20 736f  or a, b, s in so
+0000e670: 7274 6564 5f6d 6174 6368 6573 3a0a 2020  rted_matches:.  
+0000e680: 2020 2020 2020 6966 2073 203c 206d 6172        if s < mar
+0000e690: 6769 6e5f 7769 746e 6573 7369 6e67 5f77  gin_witnessing_w
+0000e6a0: 696e 3a20 0a20 2020 2020 2020 2020 2020  in: .           
+0000e6b0: 2062 7265 616b 0a20 2020 2020 2020 2069   break.        i
+0000e6c0: 6620 6120 696e 2075 6e64 6566 6561 7465  f a in undefeate
+0000e6d0: 645f 6361 6e64 6964 6174 6573 2061 6e64  d_candidates and
+0000e6e0: 2061 206e 6f74 2069 6e20 7376 5f77 696e   a not in sv_win
+0000e6f0: 6e65 7273 3a20 0a20 2020 2020 2020 2020  ners: .         
+0000e700: 2020 2063 616e 6473 5f6d 696e 7573 5f62     cands_minus_b
+0000e710: 203d 205b 6320 666f 7220 6320 696e 2063   = [c for c in c
+0000e720: 7572 725f 6361 6e64 7320 6966 2063 2021  urr_cands if c !
+0000e730: 3d20 625d 0a20 2020 2020 2020 2020 2020  = b].           
+0000e740: 2063 616e 6473 5f6d 696e 7573 5f62 5f6b   cands_minus_b_k
+0000e750: 6579 203d 2074 7570 6c65 2873 6f72 7465  ey = tuple(sorte
+0000e760: 6428 6361 6e64 735f 6d69 6e75 735f 6229  d(cands_minus_b)
+0000e770: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000e780: 2063 616e 6473 5f6d 696e 7573 5f62 5f6b   cands_minus_b_k
+0000e790: 6579 206e 6f74 2069 6e20 6d65 6d5f 7376  ey not in mem_sv
+0000e7a0: 5f77 696e 6e65 7273 2e6b 6579 7328 293a  _winners.keys():
+0000e7b0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0000e7c0: 2020 7773 2c20 6d65 6d5f 7376 5f77 696e    ws, mem_sv_win
+0000e7d0: 6e65 7273 203d 205f 7374 6162 6c65 5f76  ners = _stable_v
+0000e7e0: 6f74 696e 6728 6564 6174 612c 0a20 2020  oting(edata,.   
 0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e820: 2020 6375 7272 5f63 616e 6473 203d 2063    curr_cands = c
-0000e830: 616e 6473 5f6d 696e 7573 5f62 2c0a 2020  ands_minus_b,.  
+0000e820: 2063 7572 725f 6361 6e64 7320 3d20 6361   curr_cands = ca
+0000e830: 6e64 735f 6d69 6e75 735f 622c 0a20 2020  nds_minus_b,.   
 0000e840: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e870: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-0000e880: 696f 6e20 3d20 7374 7265 6e67 7468 5f66  ion = strength_f
-0000e890: 756e 6374 696f 6e2c 0a20 2020 2020 2020  unction,.       
+0000e870: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000e880: 6f6e 203d 2073 7472 656e 6774 685f 6675  on = strength_fu
+0000e890: 6e63 7469 6f6e 2c0a 2020 2020 2020 2020  nction,.        
 0000e8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8c0: 2020 2020 2020 2020 2020 2020 2073 6f72               sor
-0000e8d0: 7465 645f 6d61 7463 6865 7320 3d20 5b28  ted_matches = [(
-0000e8e0: 612c 2063 2c20 7329 2066 6f72 2061 2c20  a, c, s) for a, 
-0000e8f0: 632c 2073 2069 6e20 736f 7274 6564 5f6d  c, s in sorted_m
-0000e900: 6174 6368 6573 2069 6620 6120 213d 2062  atches if a != b
-0000e910: 2061 6e64 2063 2021 3d20 625d 2c0a 2020   and c != b],.  
+0000e8c0: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+0000e8d0: 6564 5f6d 6174 6368 6573 203d 205b 2861  ed_matches = [(a
+0000e8e0: 2c20 632c 2073 2920 666f 7220 612c 2063  , c, s) for a, c
+0000e8f0: 2c20 7320 696e 2073 6f72 7465 645f 6d61  , s in sorted_ma
+0000e900: 7463 6865 7320 6966 2061 2021 3d20 6220  tches if a != b 
+0000e910: 616e 6420 6320 213d 2062 5d2c 0a20 2020  and c != b],.   
 0000e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e950: 2020 6d65 6d5f 7376 5f77 696e 6e65 7273    mem_sv_winners
-0000e960: 203d 206d 656d 5f73 765f 7769 6e6e 6572   = mem_sv_winner
-0000e970: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-0000e980: 2020 206d 656d 5f73 765f 7769 6e6e 6572     mem_sv_winner
-0000e990: 735b 6361 6e64 735f 6d69 6e75 735f 625f  s[cands_minus_b_
-0000e9a0: 6b65 795d 203d 2077 730a 2020 2020 2020  key] = ws.      
-0000e9b0: 2020 2020 2020 656c 7365 3a20 0a20 2020        else: .   
-0000e9c0: 2020 2020 2020 2020 2020 2020 2077 7320               ws 
-0000e9d0: 3d20 6d65 6d5f 7376 5f77 696e 6e65 7273  = mem_sv_winners
-0000e9e0: 5b63 616e 6473 5f6d 696e 7573 5f62 5f6b  [cands_minus_b_k
-0000e9f0: 6579 5d0a 2020 2020 2020 2020 2020 2020  ey].            
-0000ea00: 6966 2061 2069 6e20 7773 3a0a 2020 2020  if a in ws:.    
-0000ea10: 2020 2020 2020 2020 2020 2020 7376 5f77              sv_w
-0000ea20: 696e 6e65 7273 2e61 7070 656e 6428 6129  inners.append(a)
-0000ea30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ea40: 206d 6172 6769 6e5f 7769 746e 6573 7369   margin_witnessi
-0000ea50: 6e67 5f77 696e 203d 2073 0a20 2020 2020  ng_win = s.     
-0000ea60: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-0000ea70: 7265 7475 726e 2073 765f 7769 6e6e 6572  return sv_winner
-0000ea80: 732c 206d 656d 5f73 765f 7769 6e6e 6572  s, mem_sv_winner
-0000ea90: 730a 2020 2020 2020 2020 0a40 766d 286e  s.        .@vm(n
-0000eaa0: 616d 6520 3d20 2253 7461 626c 6520 566f  ame = "Stable Vo
-0000eab0: 7469 6e67 2229 0a64 6566 2073 7461 626c  ting").def stabl
-0000eac0: 655f 766f 7469 6e67 2865 6461 7461 2c20  e_voting(edata, 
-0000ead0: 6375 7272 5f63 616e 6473 203d 204e 6f6e  curr_cands = Non
-0000eae0: 652c 2073 7472 656e 6774 685f 6675 6e63  e, strength_func
-0000eaf0: 7469 6f6e 203d 204e 6f6e 6529 3a20 0a20  tion = None): . 
-0000eb00: 2020 2022 2222 496d 706c 656d 656e 7461     """Implementa
-0000eb10: 7469 6f6e 206f 6620 2053 7461 626c 6520  tion of  Stable 
-0000eb20: 566f 7469 6e67 2066 726f 6d20 6874 7470  Voting from http
-0000eb30: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-0000eb40: 732f 3231 3038 2e30 3035 3432 2e20 0a0a  s/2108.00542. ..
-0000eb50: 2020 2020 5374 6162 6c65 2056 6f74 696e      Stable Votin
-0000eb60: 6720 6973 2061 2072 6563 7572 7369 7665  g is a recursive
-0000eb70: 2076 6f74 696e 6720 6d65 7468 6f64 2064   voting method d
-0000eb80: 6566 696e 6564 2061 7320 666f 6c6c 6f77  efined as follow
-0000eb90: 733a 200a 0a20 2020 2031 2e20 2049 6620  s: ..    1.  If 
-0000eba0: 7468 6572 6520 6973 206f 6e6c 7920 6f6e  there is only on
-0000ebb0: 6520 6361 6e64 6964 6174 6520 696e 2074  e candidate in t
-0000ebc0: 6865 2070 726f 6669 6c65 2c20 7468 656e  he profile, then
-0000ebd0: 2074 6861 7420 6361 6e64 6964 6174 6520   that candidate 
-0000ebe0: 6973 2074 6865 2077 696e 6e65 722e 200a  is the winner. .
-0000ebf0: 2020 2020 322e 204f 7264 6572 2074 6865      2. Order the
-0000ec00: 2070 6169 7273 203a 6d61 7468 3a60 2861   pairs :math:`(a
-0000ec10: 2c62 2960 206f 6620 6361 6e64 6964 6174  ,b)` of candidat
-0000ec20: 6573 2066 726f 6d20 6c61 7267 6573 7420  es from largest 
-0000ec30: 746f 2073 6d61 6c6c 6573 7420 7661 6c75  to smallest valu
-0000ec40: 6520 6f66 2074 6865 206d 6172 6769 6e20  e of the margin 
-0000ec50: 6f66 203a 6d61 7468 3a60 6160 206f 7665  of :math:`a` ove
-0000ec60: 7220 3a6d 6174 683a 6062 6020 7375 6368  r :math:`b` such
-0000ec70: 2074 6861 7420 3a6d 6174 683a 6061 6020   that :math:`a` 
-0000ec80: 6973 2075 6e64 6566 6561 7465 6420 6163  is undefeated ac
-0000ec90: 636f 7264 696e 6720 746f 2053 706c 6974  cording to Split
-0000eca0: 2043 7963 6c65 2c20 616e 6420 6465 636c   Cycle, and decl
-0000ecb0: 6172 6520 6173 2053 7461 626c 6520 566f  are as Stable Vo
-0000ecc0: 7469 6e67 2077 696e 6e65 7273 2074 6865  ting winners the
-0000ecd0: 2063 616e 6469 6461 7465 2873 2920 3a6d   candidate(s) :m
-0000ece0: 6174 683a 6061 6020 6672 6f6d 2074 6865  ath:`a` from the
-0000ecf0: 2065 6172 6c69 6573 7420 7061 6972 2873   earliest pair(s
-0000ed00: 2920 3a6d 6174 683a 6028 612c 6229 6020  ) :math:`(a,b)` 
-0000ed10: 7375 6368 2074 6861 7420 3a6d 6174 683a  such that :math:
-0000ed20: 6061 6020 6973 2061 2053 696d 706c 6520  `a` is a Simple 
-0000ed30: 5374 6162 6c65 2056 6f74 696e 6720 7769  Stable Voting wi
-0000ed40: 6e6e 6572 2069 6e20 7468 6520 656c 6563  nner in the elec
-0000ed50: 7469 6f6e 2077 6974 686f 7574 203a 6d61  tion without :ma
-0000ed60: 7468 3a60 6260 2e20 0a0a 2020 2020 4172  th:`b`. ..    Ar
-0000ed70: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
-0000ed80: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
-0000ed90: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
-0000eda0: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
-0000edb0: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
-0000edc0: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
-0000edd0: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
-0000ede0: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
-0000edf0: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
-0000ee00: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
-0000ee10: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
-0000ee20: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
-0000ee30: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
-0000ee40: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
-0000ee50: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
-0000ee60: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
-0000ee70: 685f 6675 6e63 7469 6f6e 2028 6675 6e63  h_function (func
-0000ee80: 7469 6f6e 2c20 6f70 7469 6f6e 616c 293a  tion, optional):
-0000ee90: 2054 6865 2073 7472 656e 6774 6820 6675   The strength fu
-0000eea0: 6e63 7469 6f6e 2074 6f20 6265 2075 7365  nction to be use
-0000eeb0: 6420 746f 2063 616c 6375 6c61 7465 2074  d to calculate t
-0000eec0: 6865 2073 7472 656e 6774 6820 6f66 2061  he strength of a
-0000eed0: 2070 6174 682e 2020 2054 6865 2064 6566   path.   The def
-0000eee0: 6175 6c74 2069 7320 7468 6520 6d61 7267  ault is the marg
-0000eef0: 696e 206d 6574 686f 6420 6f66 2060 6065  in method of ``e
-0000ef00: 6461 7461 6060 2e20 2020 5468 6973 206f  data``.   This o
-0000ef10: 6e6c 7920 6d61 7474 6572 7320 7768 656e  nly matters when
-0000ef20: 2074 6865 2062 616c 6c6f 7473 2061 7265   the ballots are
-0000ef30: 206e 6f74 206c 696e 6561 7220 6f72 6465   not linear orde
-0000ef40: 7273 2e20 0a0a 2020 2020 5265 7475 726e  rs. ..    Return
-0000ef50: 733a 200a 2020 2020 2020 2020 4120 736f  s: .        A so
-0000ef60: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
-0000ef70: 6469 6461 7465 732e 200a 0a20 2020 202e  didates. ..    .
-0000ef80: 2e20 7365 6561 6c73 6f3a 3a0a 0a20 2020  . seealso::..   
-0000ef90: 2020 2020 203a 6d65 7468 3a60 7072 6566       :meth:`pref
-0000efa0: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
-0000efb0: 6173 6564 5f6d 6574 686f 6473 2e73 696d  ased_methods.sim
-0000efc0: 706c 655f 7374 6162 6c65 5f66 6173 7465  ple_stable_faste
-0000efd0: 7260 2c20 3a6d 6574 683a 6070 7265 665f  r`, :meth:`pref_
-0000efe0: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-0000eff0: 7365 645f 6d65 7468 6f64 732e 7369 6d70  sed_methods.simp
-0000f000: 6c65 5f73 7461 626c 655f 766f 7469 6e67  le_stable_voting
-0000f010: 600a 0a0a 2020 2020 3a45 7861 6d70 6c65  `...    :Example
-0000f020: 3a20 0a0a 2020 2020 2e2e 2065 7865 635f  : ..    .. exec_
-0000f030: 636f 6465 3a3a 0a0a 2020 2020 2020 2020  code::..        
-0000f040: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
-0000f050: 2e77 6569 6768 7465 645f 6d61 6a6f 7269  .weighted_majori
-0000f060: 7479 5f67 7261 7068 7320 696d 706f 7274  ty_graphs import
-0000f070: 204d 6172 6769 6e47 7261 7068 0a20 2020   MarginGraph.   
-0000f080: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-0000f090: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-0000f0a0: 6564 5f6d 6574 686f 6473 2069 6d70 6f72  ed_methods impor
-0000f0b0: 7420 7374 6162 6c65 5f76 6f74 696e 670a  t stable_voting.
-0000f0c0: 0a20 2020 2020 2020 206d 6720 3d20 4d61  .        mg = Ma
-0000f0d0: 7267 696e 4772 6170 6828 5b30 2c20 312c  rginGraph([0, 1,
-0000f0e0: 2032 2c20 335d 2c20 5b28 302c 2033 2c20   2, 3], [(0, 3, 
-0000f0f0: 3829 2c20 2831 2c20 302c 2031 3029 2c20  8), (1, 0, 10), 
-0000f100: 2832 2c20 302c 2034 292c 2028 322c 2031  (2, 0, 4), (2, 1
-0000f110: 2c20 3829 2c20 2833 2c20 312c 2038 295d  , 8), (3, 1, 8)]
-0000f120: 290a 0a20 2020 2020 2020 2073 7461 626c  )..        stabl
-0000f130: 655f 766f 7469 6e67 2e64 6973 706c 6179  e_voting.display
-0000f140: 286d 6729 0a0a 2020 2020 2222 220a 0a20  (mg)..    """.. 
-0000f150: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
-0000f160: 6564 6174 612e 6361 6e64 6964 6174 6573  edata.candidates
-0000f170: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
-0000f180: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
-0000f190: 5f63 616e 6473 0a20 2020 2073 7472 656e  _cands.    stren
-0000f1a0: 6774 685f 6675 6e63 7469 6f6e 203d 2065  gth_function = e
-0000f1b0: 6461 7461 2e6d 6172 6769 6e20 6966 2073  data.margin if s
-0000f1c0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000f1d0: 2069 7320 4e6f 6e65 2065 6c73 6520 7374   is None else st
-0000f1e0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-0000f1f0: 200a 0a20 2020 206d 6174 6368 6573 203d   ..    matches =
-0000f200: 205b 2861 2c20 622c 2073 7472 656e 6774   [(a, b, strengt
-0000f210: 685f 6675 6e63 7469 6f6e 2861 2c20 6229  h_function(a, b)
-0000f220: 2920 666f 7220 6120 696e 2063 7572 725f  ) for a in curr_
-0000f230: 6361 6e64 7320 666f 7220 6220 696e 2063  cands for b in c
-0000f240: 7572 725f 6361 6e64 7320 6966 2061 2021  urr_cands if a !
-0000f250: 3d20 625d 0a20 2020 2073 6f72 7465 645f  = b].    sorted_
-0000f260: 6d61 7463 6865 7320 3d20 736f 7274 6564  matches = sorted
-0000f270: 286d 6174 6368 6573 2c20 7265 7665 7273  (matches, revers
-0000f280: 653d 5472 7565 2c20 6b65 793d 6c61 6d62  e=True, key=lamb
-0000f290: 6461 206d 5f77 5f77 6569 6768 743a 206d  da m_w_weight: m
-0000f2a0: 5f77 5f77 6569 6768 745b 325d 290a 0a20  _w_weight[2]).. 
-0000f2b0: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
-0000f2c0: 285f 7374 6162 6c65 5f76 6f74 696e 6728  (_stable_voting(
-0000f2d0: 6564 6174 612c 200a 2020 2020 2020 2020  edata, .        
+0000e950: 206d 656d 5f73 765f 7769 6e6e 6572 7320   mem_sv_winners 
+0000e960: 3d20 6d65 6d5f 7376 5f77 696e 6e65 7273  = mem_sv_winners
+0000e970: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e980: 2020 6d65 6d5f 7376 5f77 696e 6e65 7273    mem_sv_winners
+0000e990: 5b63 616e 6473 5f6d 696e 7573 5f62 5f6b  [cands_minus_b_k
+0000e9a0: 6579 5d20 3d20 7773 0a20 2020 2020 2020  ey] = ws.       
+0000e9b0: 2020 2020 2065 6c73 653a 200a 2020 2020       else: .    
+0000e9c0: 2020 2020 2020 2020 2020 2020 7773 203d              ws =
+0000e9d0: 206d 656d 5f73 765f 7769 6e6e 6572 735b   mem_sv_winners[
+0000e9e0: 6361 6e64 735f 6d69 6e75 735f 625f 6b65  cands_minus_b_ke
+0000e9f0: 795d 0a20 2020 2020 2020 2020 2020 2069  y].            i
+0000ea00: 6620 6120 696e 2077 733a 0a20 2020 2020  f a in ws:.     
+0000ea10: 2020 2020 2020 2020 2020 2073 765f 7769             sv_wi
+0000ea20: 6e6e 6572 732e 6170 7065 6e64 2861 290a  nners.append(a).
+0000ea30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea40: 6d61 7267 696e 5f77 6974 6e65 7373 696e  margin_witnessin
+0000ea50: 675f 7769 6e20 3d20 730a 2020 2020 2020  g_win = s.      
+0000ea60: 2020 2020 2020 2020 2020 0a20 2020 2072            .    r
+0000ea70: 6574 7572 6e20 7376 5f77 696e 6e65 7273  eturn sv_winners
+0000ea80: 2c20 6d65 6d5f 7376 5f77 696e 6e65 7273  , mem_sv_winners
+0000ea90: 0a20 2020 2020 2020 200a 4076 6d28 6e61  .        .@vm(na
+0000eaa0: 6d65 203d 2022 5374 6162 6c65 2056 6f74  me = "Stable Vot
+0000eab0: 696e 6722 290a 6465 6620 7374 6162 6c65  ing").def stable
+0000eac0: 5f76 6f74 696e 6728 6564 6174 612c 2063  _voting(edata, c
+0000ead0: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
+0000eae0: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+0000eaf0: 696f 6e20 3d20 4e6f 6e65 293a 200a 2020  ion = None): .  
+0000eb00: 2020 2222 2249 6d70 6c65 6d65 6e74 6174    """Implementat
+0000eb10: 696f 6e20 6f66 2020 5374 6162 6c65 2056  ion of  Stable V
+0000eb20: 6f74 696e 6720 6672 6f6d 2068 7474 7073  oting from https
+0000eb30: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
+0000eb40: 2f32 3130 382e 3030 3534 322e 200a 0a20  /2108.00542. .. 
+0000eb50: 2020 2053 7461 626c 6520 566f 7469 6e67     Stable Voting
+0000eb60: 2069 7320 6120 7265 6375 7273 6976 6520   is a recursive 
+0000eb70: 766f 7469 6e67 206d 6574 686f 6420 6465  voting method de
+0000eb80: 6669 6e65 6420 6173 2066 6f6c 6c6f 7773  fined as follows
+0000eb90: 3a20 0a0a 2020 2020 312e 2020 4966 2074  : ..    1.  If t
+0000eba0: 6865 7265 2069 7320 6f6e 6c79 206f 6e65  here is only one
+0000ebb0: 2063 616e 6469 6461 7465 2069 6e20 7468   candidate in th
+0000ebc0: 6520 7072 6f66 696c 652c 2074 6865 6e20  e profile, then 
+0000ebd0: 7468 6174 2063 616e 6469 6461 7465 2069  that candidate i
+0000ebe0: 7320 7468 6520 7769 6e6e 6572 2e20 0a20  s the winner. . 
+0000ebf0: 2020 2032 2e20 4f72 6465 7220 7468 6520     2. Order the 
+0000ec00: 7061 6972 7320 3a6d 6174 683a 6028 612c  pairs :math:`(a,
+0000ec10: 6229 6020 6f66 2063 616e 6469 6461 7465  b)` of candidate
+0000ec20: 7320 6672 6f6d 206c 6172 6765 7374 2074  s from largest t
+0000ec30: 6f20 736d 616c 6c65 7374 2076 616c 7565  o smallest value
+0000ec40: 206f 6620 7468 6520 6d61 7267 696e 206f   of the margin o
+0000ec50: 6620 3a6d 6174 683a 6061 6020 6f76 6572  f :math:`a` over
+0000ec60: 203a 6d61 7468 3a60 6260 2073 7563 6820   :math:`b` such 
+0000ec70: 7468 6174 203a 6d61 7468 3a60 6160 2069  that :math:`a` i
+0000ec80: 7320 756e 6465 6665 6174 6564 2061 6363  s undefeated acc
+0000ec90: 6f72 6469 6e67 2074 6f20 5370 6c69 7420  ording to Split 
+0000eca0: 4379 636c 652c 2061 6e64 2064 6563 6c61  Cycle, and decla
+0000ecb0: 7265 2061 7320 5374 6162 6c65 2056 6f74  re as Stable Vot
+0000ecc0: 696e 6720 7769 6e6e 6572 7320 7468 6520  ing winners the 
+0000ecd0: 6361 6e64 6964 6174 6528 7329 203a 6d61  candidate(s) :ma
+0000ece0: 7468 3a60 6160 2066 726f 6d20 7468 6520  th:`a` from the 
+0000ecf0: 6561 726c 6965 7374 2070 6169 7228 7329  earliest pair(s)
+0000ed00: 203a 6d61 7468 3a60 2861 2c62 2960 2073   :math:`(a,b)` s
+0000ed10: 7563 6820 7468 6174 203a 6d61 7468 3a60  uch that :math:`
+0000ed20: 6160 2069 7320 6120 5369 6d70 6c65 2053  a` is a Simple S
+0000ed30: 7461 626c 6520 566f 7469 6e67 2077 696e  table Voting win
+0000ed40: 6e65 7220 696e 2074 6865 2065 6c65 6374  ner in the elect
+0000ed50: 696f 6e20 7769 7468 6f75 7420 3a6d 6174  ion without :mat
+0000ed60: 683a 6062 602e 200a 0a20 2020 2041 7267  h:`b`. ..    Arg
+0000ed70: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
+0000ed80: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
+0000ed90: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
+0000eda0: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
+0000edb0: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
+0000edc0: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
+0000edd0: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
+0000ede0: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
+0000edf0: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
+0000ee00: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
+0000ee10: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
+0000ee20: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
+0000ee30: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
+0000ee40: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
+0000ee50: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
+0000ee60: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+0000ee70: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
+0000ee80: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
+0000ee90: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
+0000eea0: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
+0000eeb0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+0000eec0: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
+0000eed0: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
+0000eee0: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
+0000eef0: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
+0000ef00: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
+0000ef10: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
+0000ef20: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
+0000ef30: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
+0000ef40: 732e 200a 0a20 2020 2052 6574 7572 6e73  s. ..    Returns
+0000ef50: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
+0000ef60: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
+0000ef70: 6964 6174 6573 2e20 0a0a 2020 2020 2e2e  idates. ..    ..
+0000ef80: 2073 6565 616c 736f 3a3a 0a0a 2020 2020   seealso::..    
+0000ef90: 2020 2020 3a6d 6574 683a 6070 7265 665f      :meth:`pref_
+0000efa0: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+0000efb0: 7365 645f 6d65 7468 6f64 732e 7369 6d70  sed_methods.simp
+0000efc0: 6c65 5f73 7461 626c 655f 6661 7374 6572  le_stable_faster
+0000efd0: 602c 203a 6d65 7468 3a60 7072 6566 5f76  `, :meth:`pref_v
+0000efe0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
+0000eff0: 6564 5f6d 6574 686f 6473 2e73 696d 706c  ed_methods.simpl
+0000f000: 655f 7374 6162 6c65 5f76 6f74 696e 6760  e_stable_voting`
+0000f010: 0a0a 0a20 2020 203a 4578 616d 706c 653a  ...    :Example:
+0000f020: 200a 0a20 2020 202e 2e20 6578 6563 5f63   ..    .. exec_c
+0000f030: 6f64 653a 3a0a 0a20 2020 2020 2020 2066  ode::..        f
+0000f040: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
+0000f050: 7765 6967 6874 6564 5f6d 616a 6f72 6974  weighted_majorit
+0000f060: 795f 6772 6170 6873 2069 6d70 6f72 7420  y_graphs import 
+0000f070: 4d61 7267 696e 4772 6170 680a 2020 2020  MarginGraph.    
+0000f080: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
+0000f090: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+0000f0a0: 645f 6d65 7468 6f64 7320 696d 706f 7274  d_methods import
+0000f0b0: 2073 7461 626c 655f 766f 7469 6e67 0a0a   stable_voting..
+0000f0c0: 2020 2020 2020 2020 6d67 203d 204d 6172          mg = Mar
+0000f0d0: 6769 6e47 7261 7068 285b 302c 2031 2c20  ginGraph([0, 1, 
+0000f0e0: 322c 2033 5d2c 205b 2830 2c20 332c 2038  2, 3], [(0, 3, 8
+0000f0f0: 292c 2028 312c 2030 2c20 3130 292c 2028  ), (1, 0, 10), (
+0000f100: 322c 2030 2c20 3429 2c20 2832 2c20 312c  2, 0, 4), (2, 1,
+0000f110: 2038 292c 2028 332c 2031 2c20 3829 5d29   8), (3, 1, 8)])
+0000f120: 0a0a 2020 2020 2020 2020 7374 6162 6c65  ..        stable
+0000f130: 5f76 6f74 696e 672e 6469 7370 6c61 7928  _voting.display(
+0000f140: 6d67 290a 0a20 2020 2022 2222 0a0a 2020  mg)..    """..  
+0000f150: 2020 6375 7272 5f63 616e 6473 203d 2065    curr_cands = e
+0000f160: 6461 7461 2e63 616e 6469 6461 7465 7320  data.candidates 
+0000f170: 6966 2063 7572 725f 6361 6e64 7320 6973  if curr_cands is
+0000f180: 204e 6f6e 6520 656c 7365 2063 7572 725f   None else curr_
+0000f190: 6361 6e64 730a 2020 2020 7374 7265 6e67  cands.    streng
+0000f1a0: 7468 5f66 756e 6374 696f 6e20 3d20 6564  th_function = ed
+0000f1b0: 6174 612e 6d61 7267 696e 2069 6620 7374  ata.margin if st
+0000f1c0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+0000f1d0: 6973 204e 6f6e 6520 656c 7365 2073 7472  is None else str
+0000f1e0: 656e 6774 685f 6675 6e63 7469 6f6e 2020  ength_function  
+0000f1f0: 0a0a 2020 2020 6d61 7463 6865 7320 3d20  ..    matches = 
+0000f200: 5b28 612c 2062 2c20 7374 7265 6e67 7468  [(a, b, strength
+0000f210: 5f66 756e 6374 696f 6e28 612c 2062 2929  _function(a, b))
+0000f220: 2066 6f72 2061 2069 6e20 6375 7272 5f63   for a in curr_c
+0000f230: 616e 6473 2066 6f72 2062 2069 6e20 6375  ands for b in cu
+0000f240: 7272 5f63 616e 6473 2069 6620 6120 213d  rr_cands if a !=
+0000f250: 2062 5d0a 2020 2020 736f 7274 6564 5f6d   b].    sorted_m
+0000f260: 6174 6368 6573 203d 2073 6f72 7465 6428  atches = sorted(
+0000f270: 6d61 7463 6865 732c 2072 6576 6572 7365  matches, reverse
+0000f280: 3d54 7275 652c 206b 6579 3d6c 616d 6264  =True, key=lambd
+0000f290: 6120 6d5f 775f 7765 6967 6874 3a20 6d5f  a m_w_weight: m_
+0000f2a0: 775f 7765 6967 6874 5b32 5d29 0a0a 2020  w_weight[2])..  
+0000f2b0: 2020 7265 7475 726e 2073 6f72 7465 6428    return sorted(
+0000f2c0: 5f73 7461 626c 655f 766f 7469 6e67 2865  _stable_voting(e
+0000f2d0: 6461 7461 2c20 0a20 2020 2020 2020 2020  data, .         
 0000f2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2f0: 2020 2020 2020 2020 2063 7572 725f 6361           curr_ca
-0000f300: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
-0000f310: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
+0000f2f0: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
+0000f300: 6473 203d 2063 7572 725f 6361 6e64 732c  ds = curr_cands,
+0000f310: 200a 2020 2020 2020 2020 2020 2020 2020   .              
 0000f320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f330: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
-0000f340: 6374 696f 6e20 3d20 7374 7265 6e67 7468  ction = strength
-0000f350: 5f66 756e 6374 696f 6e2c 0a20 2020 2020  _function,.     
+0000f330: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+0000f340: 7469 6f6e 203d 2073 7472 656e 6774 685f  tion = strength_
+0000f350: 6675 6e63 7469 6f6e 2c0a 2020 2020 2020  function,.      
 0000f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f370: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-0000f380: 6564 5f6d 6174 6368 6573 203d 2073 6f72  ed_matches = sor
-0000f390: 7465 645f 6d61 7463 6865 732c 0a20 2020  ted_matches,.   
+0000f370: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
+0000f380: 645f 6d61 7463 6865 7320 3d20 736f 7274  d_matches = sort
+0000f390: 6564 5f6d 6174 6368 6573 2c0a 2020 2020  ed_matches,.    
 0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3b0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-0000f3c0: 6d5f 7376 5f77 696e 6e65 7273 203d 207b  m_sv_winners = {
-0000f3d0: 7d29 5b30 5d29 0a0a 4076 6d28 6e61 6d65  })[0])..@vm(name
-0000f3e0: 203d 2022 5374 6162 6c65 2056 6f74 696e   = "Stable Votin
-0000f3f0: 6722 290a 6465 6620 7374 6162 6c65 5f76  g").def stable_v
-0000f400: 6f74 696e 675f 6661 7374 6572 2865 6461  oting_faster(eda
-0000f410: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
-0000f420: 204e 6f6e 652c 2073 7472 656e 6774 685f   None, strength_
-0000f430: 6675 6e63 7469 6f6e 203d 204e 6f6e 6529  function = None)
-0000f440: 3a20 0a20 2020 2022 2222 0a20 2020 2053  : .    """.    S
-0000f450: 7461 626c 6520 566f 7469 6e67 2069 7320  table Voting is 
-0000f460: 436f 6e64 6f72 6365 7420 636f 6e73 6973  Condorcet consis
-0000f470: 7465 6e74 2e20 2020 4974 2069 7320 6661  tent.   It is fa
-0000f480: 7374 6572 2074 6f20 736b 6970 2065 7865  ster to skip exe
-0000f490: 6375 7469 6e67 2074 6865 2072 6563 7572  cuting the recur
-0000f4a0: 7369 7665 2061 6c67 6f72 6974 686d 2077  sive algorithm w
-0000f4b0: 6865 6e20 7468 6572 6520 6973 2061 2043  hen there is a C
-0000f4c0: 6f6e 646f 7263 6574 2077 696e 6e65 722e  ondorcet winner.
-0000f4d0: 2020 0a0a 2020 2020 4172 6773 3a0a 2020    ..    Args:.  
-0000f4e0: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
-0000f4f0: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
-0000f500: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
-0000f510: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
-0000f520: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
-0000f530: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
-0000f540: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
-0000f550: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
-0000f560: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
-0000f570: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
-0000f580: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
-0000f590: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
-0000f5a0: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
-0000f5b0: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
-0000f5c0: 7272 5f63 616e 6473 6060 0a20 2020 2020  rr_cands``.     
-0000f5d0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-0000f5e0: 7469 6f6e 2028 6675 6e63 7469 6f6e 2c20  tion (function, 
-0000f5f0: 6f70 7469 6f6e 616c 293a 2054 6865 2073  optional): The s
-0000f600: 7472 656e 6774 6820 6675 6e63 7469 6f6e  trength function
-0000f610: 2074 6f20 6265 2075 7365 6420 746f 2063   to be used to c
-0000f620: 616c 6375 6c61 7465 2074 6865 2073 7472  alculate the str
-0000f630: 656e 6774 6820 6f66 2061 2070 6174 682e  ength of a path.
-0000f640: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
-0000f650: 7320 7468 6520 6d61 7267 696e 206d 6574  s the margin met
-0000f660: 686f 6420 6f66 2060 6065 6461 7461 6060  hod of ``edata``
-0000f670: 2e20 2020 5468 6973 206f 6e6c 7920 6d61  .   This only ma
-0000f680: 7474 6572 7320 7768 656e 2074 6865 2062  tters when the b
-0000f690: 616c 6c6f 7473 2061 7265 206e 6f74 206c  allots are not l
-0000f6a0: 696e 6561 7220 6f72 6465 7273 2e20 0a0a  inear orders. ..
-0000f6b0: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
-0000f6c0: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
-0000f6d0: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
-0000f6e0: 732e 200a 0a20 2020 202e 2e20 7365 6561  s. ..    .. seea
-0000f6f0: 6c73 6f3a 3a0a 0a20 2020 2020 2020 203a  lso::..        :
-0000f700: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-0000f710: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-0000f720: 6574 686f 6473 2e73 696d 706c 655f 7374  ethods.simple_st
-0000f730: 6162 6c65 5f76 6f74 696e 6760 2c20 3a6d  able_voting`, :m
-0000f740: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
-0000f750: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-0000f760: 7468 6f64 732e 7374 6162 6c65 5f76 6f74  thods.stable_vot
-0000f770: 696e 6760 0a0a 0a20 2020 203a 4578 616d  ing`...    :Exam
-0000f780: 706c 653a 200a 0a20 2020 202e 2e20 6578  ple: ..    .. ex
-0000f790: 6563 5f63 6f64 653a 3a0a 0a20 2020 2020  ec_code::..     
-0000f7a0: 2020 2066 726f 6d20 7072 6566 5f76 6f74     from pref_vot
-0000f7b0: 696e 672e 7765 6967 6874 6564 5f6d 616a  ing.weighted_maj
-0000f7c0: 6f72 6974 795f 6772 6170 6873 2069 6d70  ority_graphs imp
-0000f7d0: 6f72 7420 4d61 7267 696e 4772 6170 680a  ort MarginGraph.
-0000f7e0: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-0000f7f0: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
-0000f800: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
-0000f810: 706f 7274 2073 7461 626c 655f 766f 7469  port stable_voti
-0000f820: 6e67 2c20 7374 6162 6c65 5f76 6f74 696e  ng, stable_votin
-0000f830: 675f 6661 7374 6572 0a0a 2020 2020 2020  g_faster..      
-0000f840: 2020 6d67 203d 204d 6172 6769 6e47 7261    mg = MarginGra
-0000f850: 7068 285b 302c 2031 2c20 322c 2033 5d2c  ph([0, 1, 2, 3],
-0000f860: 205b 2830 2c20 332c 2038 292c 2028 312c   [(0, 3, 8), (1,
-0000f870: 2030 2c20 3130 292c 2028 322c 2030 2c20   0, 10), (2, 0, 
-0000f880: 3429 2c20 2832 2c20 312c 2038 292c 2028  4), (2, 1, 8), (
-0000f890: 332c 2031 2c20 3829 5d29 0a0a 2020 2020  3, 1, 8)])..    
-0000f8a0: 2020 2020 7374 6162 6c65 5f76 6f74 696e      stable_votin
-0000f8b0: 675f 6661 7374 6572 2e64 6973 706c 6179  g_faster.display
-0000f8c0: 286d 6729 0a20 2020 2020 2020 2073 7461  (mg).        sta
-0000f8d0: 626c 655f 766f 7469 6e67 2e64 6973 706c  ble_voting.displ
-0000f8e0: 6179 286d 6729 0a0a 0a20 2020 2022 2222  ay(mg)...    """
-0000f8f0: 0a20 2020 2063 7720 3d20 6564 6174 612e  .    cw = edata.
-0000f900: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
-0000f910: 2863 7572 725f 6361 6e64 7320 3d20 6375  (curr_cands = cu
-0000f920: 7272 5f63 616e 6473 290a 2020 2020 6966  rr_cands).    if
-0000f930: 2063 7720 6973 206e 6f74 204e 6f6e 653a   cw is not None:
-0000f940: 200a 2020 2020 2020 2020 7265 7475 726e   .        return
-0000f950: 205b 6377 5d0a 2020 2020 656c 7365 3a20   [cw].    else: 
-0000f960: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
-0000f970: 6e64 7320 3d20 6564 6174 612e 6361 6e64  nds = edata.cand
-0000f980: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
-0000f990: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
-0000f9a0: 6520 6375 7272 5f63 616e 6473 0a20 2020  e curr_cands.   
-0000f9b0: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
-0000f9c0: 6e63 7469 6f6e 203d 2065 6461 7461 2e6d  nction = edata.m
-0000f9d0: 6172 6769 6e20 6966 2073 7472 656e 6774  argin if strengt
-0000f9e0: 685f 6675 6e63 7469 6f6e 2069 7320 4e6f  h_function is No
-0000f9f0: 6e65 2065 6c73 6520 7374 7265 6e67 7468  ne else strength
-0000fa00: 5f66 756e 6374 696f 6e20 200a 0a20 2020  _function  ..   
-0000fa10: 2020 2020 206d 6174 6368 6573 203d 205b       matches = [
-0000fa20: 2861 2c20 622c 2073 7472 656e 6774 685f  (a, b, strength_
-0000fa30: 6675 6e63 7469 6f6e 2861 2c20 6229 2920  function(a, b)) 
-0000fa40: 666f 7220 6120 696e 2063 7572 725f 6361  for a in curr_ca
-0000fa50: 6e64 7320 666f 7220 6220 696e 2063 7572  nds for b in cur
-0000fa60: 725f 6361 6e64 7320 6966 2061 2021 3d20  r_cands if a != 
-0000fa70: 625d 0a20 2020 2020 2020 2073 6f72 7465  b].        sorte
-0000fa80: 645f 6d61 7463 6865 7320 3d20 736f 7274  d_matches = sort
-0000fa90: 6564 286d 6174 6368 6573 2c20 7265 7665  ed(matches, reve
-0000faa0: 7273 653d 5472 7565 2c20 6b65 793d 6c61  rse=True, key=la
-0000fab0: 6d62 6461 206d 5f77 5f77 6569 6768 743a  mbda m_w_weight:
-0000fac0: 206d 5f77 5f77 6569 6768 745b 325d 290a   m_w_weight[2]).
-0000fad0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000fae0: 736f 7274 6564 285f 7374 6162 6c65 5f76  sorted(_stable_v
-0000faf0: 6f74 696e 6728 6564 6174 612c 200a 2020  oting(edata, .  
+0000f3b0: 2020 2020 2020 2020 2020 2020 206d 656d               mem
+0000f3c0: 5f73 765f 7769 6e6e 6572 7320 3d20 7b7d  _sv_winners = {}
+0000f3d0: 295b 305d 290a 0a40 766d 286e 616d 6520  )[0])..@vm(name 
+0000f3e0: 3d20 2253 7461 626c 6520 566f 7469 6e67  = "Stable Voting
+0000f3f0: 2229 0a64 6566 2073 7461 626c 655f 766f  ").def stable_vo
+0000f400: 7469 6e67 5f66 6173 7465 7228 6564 6174  ting_faster(edat
+0000f410: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
+0000f420: 4e6f 6e65 2c20 7374 7265 6e67 7468 5f66  None, strength_f
+0000f430: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
+0000f440: 200a 2020 2020 2222 220a 2020 2020 5374   .    """.    St
+0000f450: 6162 6c65 2056 6f74 696e 6720 6973 2043  able Voting is C
+0000f460: 6f6e 646f 7263 6574 2063 6f6e 7369 7374  ondorcet consist
+0000f470: 656e 742e 2020 2049 7420 6973 2066 6173  ent.   It is fas
+0000f480: 7465 7220 746f 2073 6b69 7020 6578 6563  ter to skip exec
+0000f490: 7574 696e 6720 7468 6520 7265 6375 7273  uting the recurs
+0000f4a0: 6976 6520 616c 676f 7269 7468 6d20 7768  ive algorithm wh
+0000f4b0: 656e 2074 6865 7265 2069 7320 6120 436f  en there is a Co
+0000f4c0: 6e64 6f72 6365 7420 7769 6e6e 6572 2e20  ndorcet winner. 
+0000f4d0: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
+0000f4e0: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
+0000f4f0: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
+0000f500: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
+0000f510: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
+0000f520: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
+0000f530: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
+0000f540: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
+0000f550: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
+0000f560: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+0000f570: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
+0000f580: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
+0000f590: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
+0000f5a0: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
+0000f5b0: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
+0000f5c0: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
+0000f5d0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+0000f5e0: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
+0000f5f0: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
+0000f600: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
+0000f610: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
+0000f620: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
+0000f630: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
+0000f640: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
+0000f650: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
+0000f660: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
+0000f670: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
+0000f680: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
+0000f690: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
+0000f6a0: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
+0000f6b0: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+0000f6c0: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
+0000f6d0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
+0000f6e0: 2e20 0a0a 2020 2020 2e2e 2073 6565 616c  . ..    .. seeal
+0000f6f0: 736f 3a3a 0a0a 2020 2020 2020 2020 3a6d  so::..        :m
+0000f700: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
+0000f710: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+0000f720: 7468 6f64 732e 7369 6d70 6c65 5f73 7461  thods.simple_sta
+0000f730: 626c 655f 766f 7469 6e67 602c 203a 6d65  ble_voting`, :me
+0000f740: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
+0000f750: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+0000f760: 686f 6473 2e73 7461 626c 655f 766f 7469  hods.stable_voti
+0000f770: 6e67 600a 0a0a 2020 2020 3a45 7861 6d70  ng`...    :Examp
+0000f780: 6c65 3a20 0a0a 2020 2020 2e2e 2065 7865  le: ..    .. exe
+0000f790: 635f 636f 6465 3a3a 0a0a 2020 2020 2020  c_code::..      
+0000f7a0: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
+0000f7b0: 6e67 2e77 6569 6768 7465 645f 6d61 6a6f  ng.weighted_majo
+0000f7c0: 7269 7479 5f67 7261 7068 7320 696d 706f  rity_graphs impo
+0000f7d0: 7274 204d 6172 6769 6e47 7261 7068 0a20  rt MarginGraph. 
+0000f7e0: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
+0000f7f0: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+0000f800: 6173 6564 5f6d 6574 686f 6473 2069 6d70  ased_methods imp
+0000f810: 6f72 7420 7374 6162 6c65 5f76 6f74 696e  ort stable_votin
+0000f820: 672c 2073 7461 626c 655f 766f 7469 6e67  g, stable_voting
+0000f830: 5f66 6173 7465 720a 0a20 2020 2020 2020  _faster..       
+0000f840: 206d 6720 3d20 4d61 7267 696e 4772 6170   mg = MarginGrap
+0000f850: 6828 5b30 2c20 312c 2032 2c20 335d 2c20  h([0, 1, 2, 3], 
+0000f860: 5b28 302c 2033 2c20 3829 2c20 2831 2c20  [(0, 3, 8), (1, 
+0000f870: 302c 2031 3029 2c20 2832 2c20 302c 2034  0, 10), (2, 0, 4
+0000f880: 292c 2028 322c 2031 2c20 3829 2c20 2833  ), (2, 1, 8), (3
+0000f890: 2c20 312c 2038 295d 290a 0a20 2020 2020  , 1, 8)])..     
+0000f8a0: 2020 2073 7461 626c 655f 766f 7469 6e67     stable_voting
+0000f8b0: 5f66 6173 7465 722e 6469 7370 6c61 7928  _faster.display(
+0000f8c0: 6d67 290a 2020 2020 2020 2020 7374 6162  mg).        stab
+0000f8d0: 6c65 5f76 6f74 696e 672e 6469 7370 6c61  le_voting.displa
+0000f8e0: 7928 6d67 290a 0a0a 2020 2020 2222 220a  y(mg)...    """.
+0000f8f0: 2020 2020 6377 203d 2065 6461 7461 2e63      cw = edata.c
+0000f900: 6f6e 646f 7263 6574 5f77 696e 6e65 7228  ondorcet_winner(
+0000f910: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
+0000f920: 725f 6361 6e64 7329 0a20 2020 2069 6620  r_cands).    if 
+0000f930: 6377 2069 7320 6e6f 7420 4e6f 6e65 3a20  cw is not None: 
+0000f940: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000f950: 5b63 775d 0a20 2020 2065 6c73 653a 200a  [cw].    else: .
+0000f960: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
+0000f970: 6473 203d 2065 6461 7461 2e63 616e 6469  ds = edata.candi
+0000f980: 6461 7465 7320 6966 2063 7572 725f 6361  dates if curr_ca
+0000f990: 6e64 7320 6973 204e 6f6e 6520 656c 7365  nds is None else
+0000f9a0: 2063 7572 725f 6361 6e64 730a 2020 2020   curr_cands.    
+0000f9b0: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+0000f9c0: 6374 696f 6e20 3d20 6564 6174 612e 6d61  ction = edata.ma
+0000f9d0: 7267 696e 2069 6620 7374 7265 6e67 7468  rgin if strength
+0000f9e0: 5f66 756e 6374 696f 6e20 6973 204e 6f6e  _function is Non
+0000f9f0: 6520 656c 7365 2073 7472 656e 6774 685f  e else strength_
+0000fa00: 6675 6e63 7469 6f6e 2020 0a0a 2020 2020  function  ..    
+0000fa10: 2020 2020 6d61 7463 6865 7320 3d20 5b28      matches = [(
+0000fa20: 612c 2062 2c20 7374 7265 6e67 7468 5f66  a, b, strength_f
+0000fa30: 756e 6374 696f 6e28 612c 2062 2929 2066  unction(a, b)) f
+0000fa40: 6f72 2061 2069 6e20 6375 7272 5f63 616e  or a in curr_can
+0000fa50: 6473 2066 6f72 2062 2069 6e20 6375 7272  ds for b in curr
+0000fa60: 5f63 616e 6473 2069 6620 6120 213d 2062  _cands if a != b
+0000fa70: 5d0a 2020 2020 2020 2020 736f 7274 6564  ].        sorted
+0000fa80: 5f6d 6174 6368 6573 203d 2073 6f72 7465  _matches = sorte
+0000fa90: 6428 6d61 7463 6865 732c 2072 6576 6572  d(matches, rever
+0000faa0: 7365 3d54 7275 652c 206b 6579 3d6c 616d  se=True, key=lam
+0000fab0: 6264 6120 6d5f 775f 7765 6967 6874 3a20  bda m_w_weight: 
+0000fac0: 6d5f 775f 7765 6967 6874 5b32 5d29 0a0a  m_w_weight[2])..
+0000fad0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000fae0: 6f72 7465 6428 5f73 7461 626c 655f 766f  orted(_stable_vo
+0000faf0: 7469 6e67 2865 6461 7461 2c20 0a20 2020  ting(edata, .   
 0000fb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000fb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb20: 2020 6375 7272 5f63 616e 6473 203d 2063    curr_cands = c
-0000fb30: 7572 725f 6361 6e64 732c 200a 2020 2020  urr_cands, .    
+0000fb20: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
+0000fb30: 7272 5f63 616e 6473 2c20 0a20 2020 2020  rr_cands, .     
 0000fb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb60: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000fb70: 6e20 3d20 7374 7265 6e67 7468 5f66 756e  n = strength_fun
-0000fb80: 6374 696f 6e2c 0a20 2020 2020 2020 2020  ction,.         
+0000fb50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fb60: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000fb70: 203d 2073 7472 656e 6774 685f 6675 6e63   = strength_func
+0000fb80: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
 0000fb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fba0: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
-0000fbb0: 645f 6d61 7463 6865 7320 3d20 736f 7274  d_matches = sort
-0000fbc0: 6564 5f6d 6174 6368 6573 2c0a 2020 2020  ed_matches,.    
+0000fba0: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
+0000fbb0: 5f6d 6174 6368 6573 203d 2073 6f72 7465  _matches = sorte
+0000fbc0: 645f 6d61 7463 6865 732c 0a20 2020 2020  d_matches,.     
 0000fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbf0: 6d65 6d5f 7376 5f77 696e 6e65 7273 203d  mem_sv_winners =
-0000fc00: 207b 7d29 5b30 5d29 0a0a 0a0a 2323 2053   {})[0])....## S
-0000fc10: 6c61 7465 720a 230a 0a0a 0a0a 4076 6d28  later.#.....@vm(
-0000fc20: 6e61 6d65 3d22 4573 7365 6e74 6961 6c20  name="Essential 
-0000fc30: 5365 7422 290a 6465 6620 6573 7365 6e74  Set").def essent
-0000fc40: 6961 6c28 6564 6174 612c 2063 7572 725f  ial(edata, curr_
-0000fc50: 6361 6e64 7320 3d20 4e6f 6e65 2c20 7468  cands = None, th
-0000fc60: 7265 7368 6f6c 6420 3d20 302e 3030 3030  reshold = 0.0000
-0000fc70: 3030 3129 3a20 0a20 2020 2022 2222 5468  001): .    """Th
-0000fc80: 6520 4573 7365 6e74 6961 6c20 5365 7420  e Essential Set 
-0000fc90: 6973 2074 6865 2073 7570 706f 7274 206f  is the support o
-0000fca0: 6620 7468 6520 2863 686f 7365 6e29 2043  f the (chosen) C
-0000fcb0: 3220 6d61 7869 6d61 6c20 6c6f 7474 6572  2 maximal lotter
-0000fcc0: 792e 0a0a 2020 2020 4172 6773 3a0a 2020  y...    Args:.  
-0000fcd0: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
-0000fce0: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
-0000fcf0: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
-0000fd00: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
-0000fd10: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
-0000fd20: 6120 606d 6172 6769 6e5f 6d61 7472 6978  a `margin_matrix
-0000fd30: 6020 6174 7472 6962 7574 652e 0a20 2020  ` attribute..   
-0000fd40: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-0000fd50: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-0000fd60: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-0000fd70: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-0000fd80: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-0000fd90: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-0000fda0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-0000fdb0: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-0000fdc0: 7360 600a 0a20 2020 2052 6574 7572 6e73  s``..    Returns
-0000fdd0: 3a0a 2020 2020 2020 2020 4120 736f 7274  :.        A sort
-0000fde0: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
-0000fdf0: 6461 7465 732e 0a0a 2020 2020 2222 220a  dates...    """.
-0000fe00: 2020 2020 6d6c 203d 206d 6178 696d 616c      ml = maximal
-0000fe10: 5f6c 6f74 7465 7279 2865 6461 7461 2c20  _lottery(edata, 
-0000fe20: 6375 7272 5f63 616e 6473 3d63 7572 725f  curr_cands=curr_
-0000fe30: 6361 6e64 7329 0a0a 2020 2020 7265 7475  cands)..    retu
-0000fe40: 726e 2073 6f72 7465 6428 5b63 2066 6f72  rn sorted([c for
-0000fe50: 2063 2069 6e20 6d6c 2e6b 6579 7328 2920   c in ml.keys() 
-0000fe60: 6966 206d 6c5b 635d 203e 2074 6872 6573  if ml[c] > thres
-0000fe70: 686f 6c64 5d29 0a0a 4076 6d28 6e61 6d65  hold])..@vm(name
-0000fe80: 3d22 5765 6967 6874 6564 2043 6f76 6572  ="Weighted Cover
-0000fe90: 696e 6722 290a 6465 6620 7765 6967 6874  ing").def weight
-0000fea0: 6564 5f63 6f76 6572 696e 6728 6564 6174  ed_covering(edat
-0000feb0: 612c 2063 7572 725f 6361 6e64 733d 4e6f  a, curr_cands=No
-0000fec0: 6e65 293a 200a 2020 2020 2222 2241 6363  ne): .    """Acc
-0000fed0: 6f72 6469 6e67 2074 6f20 5765 6967 6874  ording to Weight
-0000fee0: 6564 2043 6f76 6572 696e 672c 2078 2064  ed Covering, x d
-0000fef0: 6566 6561 7473 2079 2069 6620 7468 6520  efeats y if the 
-0000ff00: 6d61 7267 696e 206f 6620 7820 6f76 6572  margin of x over
-0000ff10: 2079 2069 7320 706f 7369 7469 7665 2061   y is positive a
-0000ff20: 6e64 2066 6f72 2065 7665 7279 206f 7468  nd for every oth
-0000ff30: 6572 207a 2c20 7468 6520 6d61 7267 696e  er z, the margin
-0000ff40: 206f 6620 7820 6f76 6572 207a 2069 7320   of x over z is 
-0000ff50: 6772 6561 7465 7220 7468 616e 206f 7220  greater than or 
-0000ff60: 6571 7561 6c20 746f 2074 6865 206d 6172  equal to the mar
-0000ff70: 6769 6e20 6f66 2079 206f 7665 7220 7a2e  gin of y over z.
-0000ff80: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
-0000ff90: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-0000ffa0: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-0000ffb0: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-0000ffc0: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-0000ffd0: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-0000ffe0: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
-0000fff0: 2e0a 2020 2020 2020 2020 6375 7272 5f63  ..        curr_c
-00010000: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
-00010010: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
-00010020: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
-00010030: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
-00010040: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
-00010050: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
-00010060: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
-00010070: 5f63 616e 6473 6060 0a0a 2020 2020 5265  _cands``..    Re
-00010080: 7475 726e 733a 0a20 2020 2020 2020 2041  turns:.        A
-00010090: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
-000100a0: 6361 6e64 6964 6174 6573 2e0a 0a20 2020  candidates...   
-000100b0: 202e 2e20 6e6f 7465 3a3a 0a20 2020 2020   .. note::.     
-000100c0: 2020 2053 6565 2c20 652e 672e 2c20 4268     See, e.g., Bh
-000100d0: 6173 6b61 7220 4475 7474 6120 616e 6420  askar Dutta and 
-000100e0: 4a65 616e 2d46 7261 6e63 6f69 7320 4c61  Jean-Francois La
-000100f0: 736c 6965 722c 2022 436f 6d70 6172 6973  slier, "Comparis
-00010100: 6f6e 2066 756e 6374 696f 6e73 2061 6e64  on functions and
-00010110: 2063 686f 6963 6520 636f 7272 6573 706f   choice correspo
-00010120: 6e64 656e 6365 732c 2220 536f 6369 616c  ndences," Social
-00010130: 2043 686f 6963 6520 616e 6420 5765 6c66   Choice and Welf
-00010140: 6172 652c 2031 363a 3531 33e2 8093 3533  are, 16:513...53
-00010150: 322c 2031 3939 392c 2064 6f69 3a31 302e  2, 1999, doi:10.
-00010160: 3130 3037 2f73 3030 3335 3530 3035 3031  1007/s0035500501
-00010170: 3538 2c20 616e 6420 5261 75cc 816c 2050  58, and Rau..l P
-00010180: 65cc 8172 657a 2d46 6572 6e61 cc81 6e64  e..rez-Ferna..nd
-00010190: 657a 2061 6e64 2042 6572 6e61 7264 2044  ez and Bernard D
-000101a0: 6520 4261 6574 732c 2022 5468 6520 7375  e Baets, "The su
-000101b0: 7065 7263 6f76 6572 696e 6720 7265 6c61  percovering rela
-000101c0: 7469 6f6e 2c20 7468 6520 7061 6972 7769  tion, the pairwi
-000101d0: 7365 2077 696e 6e65 722c 2061 6e64 206d  se winner, and m
-000101e0: 6f72 6520 6d69 7373 696e 6720 6c69 6e6b  ore missing link
-000101f0: 7320 6265 7477 6565 6e20 426f 7264 6120  s between Borda 
-00010200: 616e 6420 436f 6e64 6f72 6365 742c 2220  and Condorcet," 
-00010210: 536f 6369 616c 2043 686f 6963 6520 616e  Social Choice an
-00010220: 6420 5765 6c66 6172 652c 2035 303a 3332  d Welfare, 50:32
-00010230: 39e2 8093 3335 322c 2032 3031 382c 2064  9...352, 2018, d
-00010240: 6f69 3a31 302e 3130 3037 2f73 3030 3335  oi:10.1007/s0035
-00010250: 352d 3031 372d 3130 3836 2d30 2e0a 2020  5-017-1086-0..  
-00010260: 2020 2222 220a 0a20 2020 2063 616e 6469    """..    candi
-00010270: 6461 7465 7320 3d20 6564 6174 612e 6361  dates = edata.ca
-00010280: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
-00010290: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
-000102a0: 6c73 6520 6375 7272 5f63 616e 6473 0a0a  lse curr_cands..
-000102b0: 2020 2020 646f 6d20 3d20 7b63 3a20 7365      dom = {c: se
-000102c0: 7428 6564 6174 612e 646f 6d69 6e61 746f  t(edata.dominato
-000102d0: 7273 2863 2c20 6375 7272 5f63 616e 6473  rs(c, curr_cands
-000102e0: 203d 2063 7572 725f 6361 6e64 7329 2920   = curr_cands)) 
-000102f0: 666f 7220 6320 696e 2063 616e 6469 6461  for c in candida
-00010300: 7465 737d 0a20 2020 2075 635f 7365 7420  tes}.    uc_set 
-00010310: 3d20 6c69 7374 2829 0a0a 2020 2020 666f  = list()..    fo
-00010320: 7220 7920 696e 2063 616e 6469 6461 7465  r y in candidate
-00010330: 733a 0a20 2020 2020 2020 2069 735f 696e  s:.        is_in
-00010340: 5f75 6373 203d 2054 7275 650a 2020 2020  _ucs = True.    
-00010350: 2020 2020 666f 7220 7820 696e 2065 6461      for x in eda
-00010360: 7461 2e64 6f6d 696e 6174 6f72 7328 792c  ta.dominators(y,
-00010370: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
-00010380: 7272 5f63 616e 6473 293a 0a20 2020 2020  rr_cands):.     
-00010390: 2020 2020 2020 2023 2063 6865 636b 2069         # check i
-000103a0: 6620 7920 636f 7665 7273 2078 2c20 692e  f y covers x, i.
-000103b0: 652e 2c20 666f 7220 6576 6572 7920 7a2c  e., for every z,
-000103c0: 206d 6172 6769 6e28 782c 207a 2920 3e3d   margin(x, z) >=
-000103d0: 206d 6172 6769 6e28 792c 207a 290a 2020   margin(y, z).  
-000103e0: 2020 2020 2020 2020 2020 636f 7665 7273            covers
-000103f0: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00010400: 2020 2020 666f 7220 7a20 696e 2063 616e      for z in can
-00010410: 6469 6461 7465 733a 0a20 2020 2020 2020  didates:.       
-00010420: 2020 2020 2020 2020 2069 6620 6564 6174           if edat
-00010430: 612e 6d61 7267 696e 2878 2c20 7a29 203c  a.margin(x, z) <
-00010440: 2065 6461 7461 2e6d 6172 6769 6e28 792c   edata.margin(y,
-00010450: 207a 293a 0a20 2020 2020 2020 2020 2020   z):.           
-00010460: 2020 2020 2020 2020 2063 6f76 6572 7320           covers 
-00010470: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00010480: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00010490: 6b0a 2020 2020 2020 2020 2020 0a20 2020  k.          .   
-000104a0: 2020 2020 2020 2020 2069 6620 636f 7665           if cove
-000104b0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-000104c0: 2020 2020 6973 5f69 6e5f 7563 7320 3d20      is_in_ucs = 
-000104d0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-000104e0: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-000104f0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00010500: 2020 2020 2069 6620 6973 5f69 6e5f 7563       if is_in_uc
-00010510: 733a 0a20 2020 2020 2020 2020 2020 2075  s:.            u
-00010520: 635f 7365 742e 6170 7065 6e64 2879 290a  c_set.append(y).
-00010530: 0a20 2020 2072 6574 7572 6e20 736f 7274  .    return sort
-00010540: 6564 2875 635f 7365 7429 0a0a 4076 6d28  ed(uc_set)..@vm(
-00010550: 6e61 6d65 203d 2022 4c6f 7373 2d54 7269  name = "Loss-Tri
-00010560: 6d6d 6572 2056 6f74 696e 6722 290a 6465  mmer Voting").de
-00010570: 6620 6c6f 7373 5f74 7269 6d6d 6572 2865  f loss_trimmer(e
-00010580: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
-00010590: 203d 204e 6f6e 6529 3a0a 2020 2020 2222   = None):.    ""
-000105a0: 2249 7465 7261 7469 7665 6c79 2065 6c69  "Iteratively eli
-000105b0: 6d69 6e61 7465 2074 6865 2063 616e 6469  minate the candi
-000105c0: 6461 7465 2077 6974 6820 7468 6520 6c61  date with the la
-000105d0: 7267 6573 7420 7375 6d20 6f66 206d 6172  rgest sum of mar
-000105e0: 6769 6e73 206f 6620 6c6f 7373 2075 6e74  gins of loss unt
-000105f0: 696c 2061 2043 6f6e 646f 7263 6574 2077  il a Condorcet w
-00010600: 696e 6e65 7220 6973 2066 6f75 6e64 2e20  inner is found. 
-00010610: 496e 2074 6869 7320 7665 7273 696f 6e20  In this version 
-00010620: 6f66 2074 6865 206d 6574 686f 642c 2070  of the method, p
-00010630: 6172 616c 6c65 6c2d 756e 6976 6572 7365  arallel-universe
-00010640: 2074 6965 6272 6561 6b69 6e67 2069 7320   tiebreaking is 
-00010650: 7573 6564 2069 6620 7468 6572 6520 6172  used if there ar
-00010660: 6520 6d75 6c74 6970 6c65 2063 616e 6469  e multiple candi
-00010670: 6461 7465 7320 7769 7468 2074 6865 206c  dates with the l
-00010680: 6172 6765 7374 2073 756d 206f 6620 6d61  argest sum of ma
-00010690: 7267 696e 7320 6f66 206c 6f73 732e 0a0a  rgins of loss...
-000106a0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000106b0: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
-000106c0: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
-000106d0: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
-000106e0: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
-000106f0: 7461 2074 6861 7420 6861 7320 6120 6d61  ta that has a ma
-00010700: 7267 696e 206d 6574 686f 642e 0a20 2020  rgin method..   
-00010710: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-00010720: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-00010730: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-00010740: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-00010750: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-00010760: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-00010770: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-00010780: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-00010790: 7360 600a 0a20 2020 2052 6574 7572 6e73  s``..    Returns
-000107a0: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
-000107b0: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
-000107c0: 6964 6174 6573 0a0a 2020 2020 2e2e 206e  idates..    .. n
-000107d0: 6f74 653a 3a0a 2020 2020 2020 2020 4d65  ote::.        Me
-000107e0: 7468 6f64 2070 726f 706f 7365 6420 6279  thod proposed by
-000107f0: 2052 6963 6861 7264 2042 2e20 4461 726c   Richard B. Darl
-00010800: 696e 6774 6f6e 2069 6e20 2254 6865 2043  ington in "The C
-00010810: 6173 6520 666f 7220 7468 6520 4c6f 7373  ase for the Loss
-00010820: 2d54 7269 6d6d 6572 2056 6f74 696e 6720  -Trimmer Voting 
-00010830: 5379 7374 656d 2e22 0a0a 2020 2020 2222  System."..    ""
-00010840: 220a 0a20 2020 2063 7572 725f 6361 6e64  "..    curr_cand
-00010850: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-00010860: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-00010870: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-00010880: 6375 7272 5f63 616e 6473 0a0a 2020 2020  curr_cands..    
-00010890: 7765 616b 5f63 7720 3d20 6564 6174 612e  weak_cw = edata.
-000108a0: 7765 616b 5f63 6f6e 646f 7263 6574 5f77  weak_condorcet_w
-000108b0: 696e 6e65 7228 6375 7272 5f63 616e 6473  inner(curr_cands
-000108c0: 203d 2063 7572 725f 6361 6e64 7329 0a20   = curr_cands). 
-000108d0: 2020 2023 2049 6620 7468 6572 6520 6172     # If there ar
-000108e0: 6520 7765 616b 2043 6f6e 646f 7263 6574  e weak Condorcet
-000108f0: 2077 696e 6e65 7273 2c20 7265 7475 726e   winners, return
-00010900: 2074 686f 7365 2063 616e 6469 6461 7465   those candidate
-00010910: 730a 2020 2020 6966 2065 6461 7461 2e77  s.    if edata.w
-00010920: 6561 6b5f 636f 6e64 6f72 6365 745f 7769  eak_condorcet_wi
-00010930: 6e6e 6572 2863 7572 725f 6361 6e64 7320  nner(curr_cands 
-00010940: 3d20 6375 7272 5f63 616e 6473 2920 6973  = curr_cands) is
-00010950: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00010960: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
-00010970: 2877 6561 6b5f 6377 290a 2020 2020 0a20  (weak_cw).    . 
-00010980: 2020 2023 204f 7468 6572 7769 7365 2c20     # Otherwise, 
-00010990: 6361 6c63 756c 6174 6520 7468 6520 7375  calculate the su
-000109a0: 6d20 6f66 206d 6172 6769 6e73 206f 6620  m of margins of 
-000109b0: 6c6f 7373 2066 6f72 2065 6163 6820 6361  loss for each ca
-000109c0: 6e64 6964 6174 650a 2020 2020 7375 6d5f  ndidate.    sum_
-000109d0: 6f66 5f6d 6172 6769 6e73 5f6f 665f 6c6f  of_margins_of_lo
-000109e0: 7373 203d 207b 6361 6e64 3a20 7375 6d28  ss = {cand: sum(
-000109f0: 5b65 6461 7461 2e6d 6172 6769 6e28 6f74  [edata.margin(ot
-00010a00: 6865 725f 6361 6e64 2c20 6361 6e64 2920  her_cand, cand) 
-00010a10: 666f 7220 6f74 6865 725f 6361 6e64 2069  for other_cand i
-00010a20: 6e20 6375 7272 5f63 616e 6473 2069 6620  n curr_cands if 
-00010a30: 6564 6174 612e 6d61 7267 696e 286f 7468  edata.margin(oth
-00010a40: 6572 5f63 616e 642c 2063 616e 6429 203e  er_cand, cand) >
-00010a50: 2030 5d29 2066 6f72 2063 616e 6420 696e   0]) for cand in
-00010a60: 2063 7572 725f 6361 6e64 737d 0a0a 2020   curr_cands}..  
-00010a70: 2020 2320 4669 6e64 2074 6865 2063 616e    # Find the can
-00010a80: 6469 6461 7465 7320 7769 7468 2074 6865  didates with the
-00010a90: 206c 6172 6765 7374 2073 756d 206f 6620   largest sum of 
-00010aa0: 6d61 7267 696e 7320 6f66 206c 6f73 730a  margins of loss.
-00010ab0: 2020 2020 6d61 785f 7375 6d5f 6f66 5f6d      max_sum_of_m
-00010ac0: 6172 6769 6e73 5f6f 665f 6c6f 7373 203d  argins_of_loss =
-00010ad0: 206d 6178 2873 756d 5f6f 665f 6d61 7267   max(sum_of_marg
-00010ae0: 696e 735f 6f66 5f6c 6f73 732e 7661 6c75  ins_of_loss.valu
-00010af0: 6573 2829 290a 2020 2020 6269 6767 6573  es()).    bigges
-00010b00: 745f 6c6f 7365 7273 203d 205b 6361 6e64  t_losers = [cand
-00010b10: 2066 6f72 2063 616e 6420 696e 2063 7572   for cand in cur
-00010b20: 725f 6361 6e64 7320 6966 2073 756d 5f6f  r_cands if sum_o
-00010b30: 665f 6d61 7267 696e 735f 6f66 5f6c 6f73  f_margins_of_los
-00010b40: 735b 6361 6e64 5d20 3d3d 206d 6178 5f73  s[cand] == max_s
-00010b50: 756d 5f6f 665f 6d61 7267 696e 735f 6f66  um_of_margins_of
-00010b60: 5f6c 6f73 735d 0a0a 2020 2020 7769 6e6e  _loss]..    winn
-00010b70: 6572 7320 3d20 5b5d 0a0a 2020 2020 2320  ers = []..    # 
-00010b80: 466f 7220 6561 6368 2062 6967 6765 7374  For each biggest
-00010b90: 206c 6f73 6572 2c20 6361 6c63 756c 6174   loser, calculat
-00010ba0: 6520 7468 6520 7769 6e6e 6572 7320 6166  e the winners af
-00010bb0: 7465 7220 7265 6d6f 7669 6e67 2074 6861  ter removing tha
-00010bc0: 7420 6361 6e64 6964 6174 652e 2054 6865  t candidate. The
-00010bd0: 2075 6e69 6f6e 206f 6620 7468 6573 6520   union of these 
-00010be0: 7365 7473 2069 7320 7468 6520 7365 7420  sets is the set 
-00010bf0: 6f66 2077 696e 6e65 7273 2e0a 2020 2020  of winners..    
-00010c00: 666f 7220 626c 2069 6e20 6269 6767 6573  for bl in bigges
-00010c10: 745f 6c6f 7365 7273 3a0a 2020 2020 2020  t_losers:.      
-00010c20: 2020 7769 6e6e 6572 735f 7769 7468 6f75    winners_withou
-00010c30: 745f 626c 203d 206c 6f73 735f 7472 696d  t_bl = loss_trim
-00010c40: 6d65 7228 6564 6174 612c 2063 7572 725f  mer(edata, curr_
-00010c50: 6361 6e64 7320 3d20 5b63 616e 6420 666f  cands = [cand fo
-00010c60: 7220 6361 6e64 2069 6e20 6375 7272 5f63  r cand in curr_c
-00010c70: 616e 6473 2069 6620 6361 6e64 2021 3d20  ands if cand != 
-00010c80: 626c 5d29 0a20 2020 2020 2020 2077 696e  bl]).        win
-00010c90: 6e65 7273 202b 3d20 7769 6e6e 6572 735f  ners += winners_
-00010ca0: 7769 7468 6f75 745f 626c 0a0a 2020 2020  without_bl..    
-00010cb0: 7265 7475 726e 2073 6f72 7465 6428 6c69  return sorted(li
-00010cc0: 7374 2873 6574 2877 696e 6e65 7273 2929  st(set(winners))
-00010cd0: 290a 0a0a 6465 6620 6469 7374 616e 6365  )...def distance
-00010ce0: 5f74 6f5f 6d61 7267 696e 5f67 7261 7068  _to_margin_graph
-00010cf0: 2865 6461 7461 2c20 7265 6c2c 2065 7870  (edata, rel, exp
-00010d00: 203d 2031 2c20 6375 7272 5f63 616e 6473   = 1, curr_cands
-00010d10: 203d 204e 6f6e 6529 3a20 0a20 2020 2022   = None): .    "
-00010d20: 2222 0a20 2020 2043 616c 6375 6c61 7465  "".    Calculate
-00010d30: 2074 6865 2064 6973 7461 6e63 6520 6f66   the distance of
-00010d40: 2060 6072 656c 6060 2028 6120 7265 6c61   ``rel`` (a rela
-00010d50: 7469 6f6e 2920 746f 2074 6865 206d 616a  tion) to the maj
-00010d60: 6f72 6974 7920 6772 6170 6820 6f66 2060  ority graph of `
-00010d70: 6065 6461 7461 6060 2e20 0a20 2020 2022  `edata``. .    "
-00010d80: 2222 0a20 2020 2063 616e 6469 6461 7465  "".    candidate
-00010d90: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-00010da0: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-00010db0: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-00010dc0: 6375 7272 5f63 616e 6473 0a20 2020 200a  curr_cands.    .
-00010dd0: 2020 2020 6966 2074 7970 6528 6564 6174      if type(edat
-00010de0: 6129 203d 3d20 4d61 6a6f 7269 7479 4772  a) == MajorityGr
-00010df0: 6170 6820 616e 6420 6578 7020 3d3d 2030  aph and exp == 0
-00010e00: 3a0a 2020 2020 2020 2020 2320 6966 2065  :.        # if e
-00010e10: 6461 7461 2069 7320 6120 4d61 6a6f 7269  data is a Majori
-00010e20: 7479 4772 6170 682c 2077 6520 6e65 6564  tyGraph, we need
-00010e30: 2074 6f20 6164 6420 6d61 7267 696e 7320   to add margins 
-00010e40: 666f 7220 7468 6520 666f 6c6c 6f77 696e  for the followin
-00010e50: 6720 636f 6465 2074 6f20 776f 726b 2e20  g code to work. 
-00010e60: 2054 6865 206d 6172 6769 6e73 2064 6f20   The margins do 
-00010e70: 6e6f 7420 6d61 7474 6572 2077 6865 6e20  not matter when 
-00010e80: 6578 703d 3d30 2e20 2020 0a20 2020 2020  exp==0.   .     
-00010e90: 2020 2065 6461 7461 203d 204d 6172 6769     edata = Margi
-00010ea0: 6e47 7261 7068 2863 616e 6469 6461 7465  nGraph(candidate
-00010eb0: 732c 205b 2863 312c 2063 322c 2031 2920  s, [(c1, c2, 1) 
-00010ec0: 666f 7220 6331 2c20 6332 2069 6e20 6564  for c1, c2 in ed
-00010ed0: 6174 612e 6564 6765 7320 6966 2028 6331  ata.edges if (c1
-00010ee0: 2069 6e20 6361 6e64 6964 6174 6573 2061   in candidates a
-00010ef0: 6e64 2063 3220 696e 2063 616e 6469 6461  nd c2 in candida
-00010f00: 7465 7329 5d29 0a20 2020 2070 656e 616c  tes)]).    penal
-00010f10: 7479 203d 2030 0a20 2020 2066 6f72 2061  ty = 0.    for a
-00010f20: 2c62 2069 6e20 636f 6d62 696e 6174 696f  ,b in combinatio
-00010f30: 6e73 2863 616e 6469 6461 7465 732c 2032  ns(candidates, 2
-00010f40: 293a 200a 2020 2020 2020 2020 6966 2065  ): .        if e
-00010f50: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
-00010f60: 6566 6572 7328 612c 2062 2920 616e 6420  efers(a, b) and 
-00010f70: 2862 2c61 2920 696e 2072 656c 3a20 0a20  (b,a) in rel: . 
-00010f80: 2020 2020 2020 2020 2020 2070 656e 616c             penal
-00010f90: 7479 202b 3d20 2865 6461 7461 2e6d 6172  ty += (edata.mar
-00010fa0: 6769 6e28 612c 2062 2920 2a2a 2065 7870  gin(a, b) ** exp
-00010fb0: 290a 2020 2020 2020 2020 656c 6966 2065  ).        elif e
-00010fc0: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
-00010fd0: 6566 6572 7328 622c 2061 2920 616e 6420  efers(b, a) and 
-00010fe0: 2861 2c62 2920 696e 2072 656c 3a20 0a20  (a,b) in rel: . 
-00010ff0: 2020 2020 2020 2020 2020 2070 656e 616c             penal
-00011000: 7479 202b 3d20 2865 6461 7461 2e6d 6172  ty += (edata.mar
-00011010: 6769 6e28 622c 2061 2920 2a2a 2065 7870  gin(b, a) ** exp
-00011020: 290a 2020 2020 2020 2020 656c 6966 2065  ).        elif e
-00011030: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
-00011040: 6566 6572 7328 612c 2062 2920 616e 6420  efers(a, b) and 
-00011050: 2861 2c62 2920 6e6f 7420 696e 2072 656c  (a,b) not in rel
-00011060: 2061 6e64 2028 622c 6129 206e 6f74 2069   and (b,a) not i
-00011070: 6e20 7265 6c3a 200a 2020 2020 2020 2020  n rel: .        
-00011080: 2020 2020 7065 6e61 6c74 7920 2b3d 2028      penalty += (
-00011090: 6564 6174 612e 6d61 7267 696e 2861 2c20  edata.margin(a, 
-000110a0: 6229 202a 2a20 6578 7029 202f 2032 200a  b) ** exp) / 2 .
-000110b0: 2020 2020 2020 2020 656c 6966 2065 6461          elif eda
-000110c0: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
-000110d0: 6572 7328 622c 2061 2920 616e 6420 2861  ers(b, a) and (a
-000110e0: 2c62 2920 6e6f 7420 696e 2072 656c 2061  ,b) not in rel a
-000110f0: 6e64 2028 622c 6129 206e 6f74 2069 6e20  nd (b,a) not in 
-00011100: 7265 6c3a 200a 2020 2020 2020 2020 2020  rel: .          
-00011110: 2020 7065 6e61 6c74 7920 2b3d 2028 6564    penalty += (ed
-00011120: 6174 612e 6d61 7267 696e 2862 2c20 6129  ata.margin(b, a)
-00011130: 202a 2a20 6578 7029 2020 2f20 320a 2020   ** exp)  / 2.  
-00011140: 2020 7265 7475 726e 2070 656e 616c 7479    return penalty
-00011150: 0a0a 0a6d 675f 766d 7320 3d20 5b0a 2020  ...mg_vms = [.  
-00011160: 2020 6d69 6e69 6d61 782c 200a 2020 2020    minimax, .    
-00011170: 7370 6c69 745f 6379 636c 652c 0a20 2020  split_cycle,.   
-00011180: 2023 7370 6c69 745f 6379 636c 655f 466c   #split_cycle_Fl
-00011190: 6f79 645f 5761 7273 6861 6c6c 2c0a 2020  oyd_Warshall,.  
-000111a0: 2020 2362 6561 745f 7061 7468 2c0a 2020    #beat_path,.  
-000111b0: 2020 6265 6174 5f70 6174 685f 466c 6f79    beat_path_Floy
-000111c0: 645f 5761 7273 6861 6c6c 2c0a 2020 2020  d_Warshall,.    
-000111d0: 2372 616e 6b65 645f 7061 6972 732c 0a20  #ranked_pairs,. 
-000111e0: 2020 2023 7261 6e6b 6564 5f70 6169 7273     #ranked_pairs
-000111f0: 5f77 6974 685f 7465 7374 2c0a 2020 2020  _with_test,.    
-00011200: 7261 6e6b 6564 5f70 6169 7273 5f7a 742c  ranked_pairs_zt,
-00011210: 0a20 2020 2072 616e 6b65 645f 7061 6972  .    ranked_pair
-00011220: 735f 7462 2c0a 2020 2020 2372 6976 6572  s_tb,.    #river
-00011230: 2c0a 2020 2020 2372 6976 6572 5f77 6974  ,.    #river_wit
-00011240: 685f 7465 7374 2c20 0a20 2020 2073 696d  h_test, .    sim
-00011250: 706c 655f 7374 6162 6c65 5f76 6f74 696e  ple_stable_votin
-00011260: 672c 0a20 2020 2023 7369 6d70 6c65 5f73  g,.    #simple_s
-00011270: 7461 626c 655f 766f 7469 6e67 5f66 6173  table_voting_fas
-00011280: 7465 722c 0a20 2020 2073 7461 626c 655f  ter,.    stable_
-00011290: 766f 7469 6e67 2c0a 2020 2020 2373 7461  voting,.    #sta
-000112a0: 626c 655f 766f 7469 6e67 5f66 6173 7465  ble_voting_faste
-000112b0: 722c 0a20 2020 2065 7373 656e 7469 616c  r,.    essential
-000112c0: 2c0a 2020 2020 7765 6967 6874 6564 5f63  ,.    weighted_c
-000112d0: 6f76 6572 696e 672c 0a20 2020 206c 6f73  overing,.    los
-000112e0: 735f 7472 696d 6d65 720a 5d0a 0a0a 6d67  s_trimmer.]...mg
-000112f0: 5f76 6d73 5f61 6c6c 203d 205b 0a20 2020  _vms_all = [.   
-00011300: 206d 696e 696d 6178 2c20 0a20 2020 2073   minimax, .    s
-00011310: 706c 6974 5f63 7963 6c65 2c0a 2020 2020  plit_cycle,.    
-00011320: 7370 6c69 745f 6379 636c 655f 466c 6f79  split_cycle_Floy
-00011330: 645f 5761 7273 6861 6c6c 2c0a 2020 2020  d_Warshall,.    
-00011340: 6265 6174 5f70 6174 682c 0a20 2020 2062  beat_path,.    b
-00011350: 6561 745f 7061 7468 5f46 6c6f 7964 5f57  eat_path_Floyd_W
-00011360: 6172 7368 616c 6c2c 0a20 2020 2072 616e  arshall,.    ran
-00011370: 6b65 645f 7061 6972 732c 0a20 2020 2072  ked_pairs,.    r
-00011380: 616e 6b65 645f 7061 6972 735f 7769 7468  anked_pairs_with
-00011390: 5f74 6573 742c 0a20 2020 2072 616e 6b65  _test,.    ranke
-000113a0: 645f 7061 6972 735f 7a74 2c0a 2020 2020  d_pairs_zt,.    
-000113b0: 7261 6e6b 6564 5f70 6169 7273 5f74 622c  ranked_pairs_tb,
-000113c0: 0a20 2020 2072 616e 6b65 645f 7061 6972  .    ranked_pair
-000113d0: 735f 6672 6f6d 5f73 7461 636b 732c 0a20  s_from_stacks,. 
-000113e0: 2020 2072 6976 6572 2c0a 2020 2020 7269     river,.    ri
-000113f0: 7665 725f 7769 7468 5f74 6573 742c 200a  ver_with_test, .
-00011400: 2020 2020 7369 6d70 6c65 5f73 7461 626c      simple_stabl
-00011410: 655f 766f 7469 6e67 2c0a 2020 2020 7369  e_voting,.    si
-00011420: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
-00011430: 6e67 5f66 6173 7465 722c 0a20 2020 2073  ng_faster,.    s
-00011440: 7461 626c 655f 766f 7469 6e67 2c0a 2020  table_voting,.  
-00011450: 2020 7374 6162 6c65 5f76 6f74 696e 675f    stable_voting_
-00011460: 6661 7374 6572 2c0a 2020 2020 6573 7365  faster,.    esse
-00011470: 6e74 6961 6c2c 0a20 2020 2077 6569 6768  ntial,.    weigh
-00011480: 7465 645f 636f 7665 7269 6e67 2c0a 2020  ted_covering,.  
-00011490: 2020 6c6f 7373 5f74 7269 6d6d 6572 0a5d    loss_trimmer.]
+0000fbe0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000fbf0: 656d 5f73 765f 7769 6e6e 6572 7320 3d20  em_sv_winners = 
+0000fc00: 7b7d 295b 305d 290a 0a0a 0a23 2320 536c  {})[0])....## Sl
+0000fc10: 6174 6572 0a23 0a0a 0a0a 4076 6d28 6e61  ater.#....@vm(na
+0000fc20: 6d65 3d22 4573 7365 6e74 6961 6c20 5365  me="Essential Se
+0000fc30: 7422 290a 6465 6620 6573 7365 6e74 6961  t").def essentia
+0000fc40: 6c28 6564 6174 612c 2063 7572 725f 6361  l(edata, curr_ca
+0000fc50: 6e64 7320 3d20 4e6f 6e65 2c20 7468 7265  nds = None, thre
+0000fc60: 7368 6f6c 6420 3d20 302e 3030 3030 3030  shold = 0.000000
+0000fc70: 3129 3a20 0a20 2020 2022 2222 5468 6520  1): .    """The 
+0000fc80: 4573 7365 6e74 6961 6c20 5365 7420 6973  Essential Set is
+0000fc90: 2074 6865 2073 7570 706f 7274 206f 6620   the support of 
+0000fca0: 7468 6520 2863 686f 7365 6e29 2043 3220  the (chosen) C2 
+0000fcb0: 6d61 7869 6d61 6c20 6c6f 7474 6572 792e  maximal lottery.
+0000fcc0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+0000fcd0: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
+0000fce0: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
+0000fcf0: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
+0000fd00: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
+0000fd10: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
+0000fd20: 606d 6172 6769 6e5f 6d61 7472 6978 6020  `margin_matrix` 
+0000fd30: 6174 7472 6962 7574 652e 0a20 2020 2020  attribute..     
+0000fd40: 2020 2063 7572 725f 6361 6e64 7320 284c     curr_cands (L
+0000fd50: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
+0000fd60: 616c 293a 2049 6620 7365 742c 2074 6865  al): If set, the
+0000fd70: 6e20 6669 6e64 2074 6865 2077 696e 6e65  n find the winne
+0000fd80: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
+0000fd90: 6c65 2072 6573 7472 6963 7465 6420 746f  le restricted to
+0000fda0: 2074 6865 2063 616e 6469 6461 7465 7320   the candidates 
+0000fdb0: 696e 2060 6063 7572 725f 6361 6e64 7360  in ``curr_cands`
+0000fdc0: 600a 0a20 2020 2052 6574 7572 6e73 3a0a  `..    Returns:.
+0000fdd0: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
+0000fde0: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
+0000fdf0: 7465 732e 0a0a 2020 2020 2222 220a 2020  tes...    """.  
+0000fe00: 2020 6d6c 203d 206d 6178 696d 616c 5f6c    ml = maximal_l
+0000fe10: 6f74 7465 7279 2865 6461 7461 2c20 6375  ottery(edata, cu
+0000fe20: 7272 5f63 616e 6473 3d63 7572 725f 6361  rr_cands=curr_ca
+0000fe30: 6e64 7329 0a0a 2020 2020 7265 7475 726e  nds)..    return
+0000fe40: 2073 6f72 7465 6428 5b63 2066 6f72 2063   sorted([c for c
+0000fe50: 2069 6e20 6d6c 2e6b 6579 7328 2920 6966   in ml.keys() if
+0000fe60: 206d 6c5b 635d 203e 2074 6872 6573 686f   ml[c] > thresho
+0000fe70: 6c64 5d29 0a0a 4076 6d28 6e61 6d65 3d22  ld])..@vm(name="
+0000fe80: 5765 6967 6874 6564 2043 6f76 6572 696e  Weighted Coverin
+0000fe90: 6722 290a 6465 6620 7765 6967 6874 6564  g").def weighted
+0000fea0: 5f63 6f76 6572 696e 6728 6564 6174 612c  _covering(edata,
+0000feb0: 2063 7572 725f 6361 6e64 733d 4e6f 6e65   curr_cands=None
+0000fec0: 293a 200a 2020 2020 2222 2241 6363 6f72  ): .    """Accor
+0000fed0: 6469 6e67 2074 6f20 5765 6967 6874 6564  ding to Weighted
+0000fee0: 2043 6f76 6572 696e 672c 2078 2064 6566   Covering, x def
+0000fef0: 6561 7473 2079 2069 6620 7468 6520 6d61  eats y if the ma
+0000ff00: 7267 696e 206f 6620 7820 6f76 6572 2079  rgin of x over y
+0000ff10: 2069 7320 706f 7369 7469 7665 2061 6e64   is positive and
+0000ff20: 2066 6f72 2065 7665 7279 206f 7468 6572   for every other
+0000ff30: 207a 2c20 7468 6520 6d61 7267 696e 206f   z, the margin o
+0000ff40: 6620 7820 6f76 6572 207a 2069 7320 6772  f x over z is gr
+0000ff50: 6561 7465 7220 7468 616e 206f 7220 6571  eater than or eq
+0000ff60: 7561 6c20 746f 2074 6865 206d 6172 6769  ual to the margi
+0000ff70: 6e20 6f66 2079 206f 7665 7220 7a2e 200a  n of y over z. .
+0000ff80: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+0000ff90: 2020 2065 6461 7461 2028 5072 6f66 696c     edata (Profil
+0000ffa0: 652c 2050 726f 6669 6c65 5769 7468 5469  e, ProfileWithTi
+0000ffb0: 6573 2c20 4d61 7267 696e 4772 6170 6829  es, MarginGraph)
+0000ffc0: 3a20 416e 7920 656c 6563 7469 6f6e 2064  : Any election d
+0000ffd0: 6174 6120 7468 6174 2068 6173 2061 2060  ata that has a `
+0000ffe0: 6d61 7267 696e 6020 6d65 7468 6f64 2e0a  margin` method..
+0000fff0: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
+00010000: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
+00010010: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
+00010020: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
+00010030: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
+00010040: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
+00010050: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
+00010060: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
+00010070: 616e 6473 6060 0a0a 2020 2020 5265 7475  ands``..    Retu
+00010080: 726e 733a 0a20 2020 2020 2020 2041 2073  rns:.        A s
+00010090: 6f72 7465 6420 6c69 7374 206f 6620 6361  orted list of ca
+000100a0: 6e64 6964 6174 6573 2e0a 0a20 2020 202e  ndidates...    .
+000100b0: 2e20 6e6f 7465 3a3a 0a20 2020 2020 2020  . note::.       
+000100c0: 2053 6565 2c20 652e 672e 2c20 4268 6173   See, e.g., Bhas
+000100d0: 6b61 7220 4475 7474 6120 616e 6420 4a65  kar Dutta and Je
+000100e0: 616e 2d46 7261 6e63 6f69 7320 4c61 736c  an-Francois Lasl
+000100f0: 6965 722c 2022 436f 6d70 6172 6973 6f6e  ier, "Comparison
+00010100: 2066 756e 6374 696f 6e73 2061 6e64 2063   functions and c
+00010110: 686f 6963 6520 636f 7272 6573 706f 6e64  hoice correspond
+00010120: 656e 6365 732c 2220 536f 6369 616c 2043  ences," Social C
+00010130: 686f 6963 6520 616e 6420 5765 6c66 6172  hoice and Welfar
+00010140: 652c 2031 363a 3531 33e2 8093 3533 322c  e, 16:513...532,
+00010150: 2031 3939 392c 2064 6f69 3a31 302e 3130   1999, doi:10.10
+00010160: 3037 2f73 3030 3335 3530 3035 3031 3538  07/s003550050158
+00010170: 2c20 616e 6420 5261 75cc 816c 2050 65cc  , and Rau..l Pe.
+00010180: 8172 657a 2d46 6572 6e61 cc81 6e64 657a  .rez-Ferna..ndez
+00010190: 2061 6e64 2042 6572 6e61 7264 2044 6520   and Bernard De 
+000101a0: 4261 6574 732c 2022 5468 6520 7375 7065  Baets, "The supe
+000101b0: 7263 6f76 6572 696e 6720 7265 6c61 7469  rcovering relati
+000101c0: 6f6e 2c20 7468 6520 7061 6972 7769 7365  on, the pairwise
+000101d0: 2077 696e 6e65 722c 2061 6e64 206d 6f72   winner, and mor
+000101e0: 6520 6d69 7373 696e 6720 6c69 6e6b 7320  e missing links 
+000101f0: 6265 7477 6565 6e20 426f 7264 6120 616e  between Borda an
+00010200: 6420 436f 6e64 6f72 6365 742c 2220 536f  d Condorcet," So
+00010210: 6369 616c 2043 686f 6963 6520 616e 6420  cial Choice and 
+00010220: 5765 6c66 6172 652c 2035 303a 3332 39e2  Welfare, 50:329.
+00010230: 8093 3335 322c 2032 3031 382c 2064 6f69  ..352, 2018, doi
+00010240: 3a31 302e 3130 3037 2f73 3030 3335 352d  :10.1007/s00355-
+00010250: 3031 372d 3130 3836 2d30 2e0a 2020 2020  017-1086-0..    
+00010260: 2222 220a 0a20 2020 2063 616e 6469 6461  """..    candida
+00010270: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
+00010280: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
+00010290: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
+000102a0: 6520 6375 7272 5f63 616e 6473 0a0a 2020  e curr_cands..  
+000102b0: 2020 646f 6d20 3d20 7b63 3a20 7365 7428    dom = {c: set(
+000102c0: 6564 6174 612e 646f 6d69 6e61 746f 7273  edata.dominators
+000102d0: 2863 2c20 6375 7272 5f63 616e 6473 203d  (c, curr_cands =
+000102e0: 2063 7572 725f 6361 6e64 7329 2920 666f   curr_cands)) fo
+000102f0: 7220 6320 696e 2063 616e 6469 6461 7465  r c in candidate
+00010300: 737d 0a20 2020 2075 635f 7365 7420 3d20  s}.    uc_set = 
+00010310: 6c69 7374 2829 0a0a 2020 2020 666f 7220  list()..    for 
+00010320: 7920 696e 2063 616e 6469 6461 7465 733a  y in candidates:
+00010330: 0a20 2020 2020 2020 2069 735f 696e 5f75  .        is_in_u
+00010340: 6373 203d 2054 7275 650a 2020 2020 2020  cs = True.      
+00010350: 2020 666f 7220 7820 696e 2065 6461 7461    for x in edata
+00010360: 2e64 6f6d 696e 6174 6f72 7328 792c 2063  .dominators(y, c
+00010370: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
+00010380: 5f63 616e 6473 293a 0a20 2020 2020 2020  _cands):.       
+00010390: 2020 2020 2023 2063 6865 636b 2069 6620       # check if 
+000103a0: 7920 636f 7665 7273 2078 2c20 692e 652e  y covers x, i.e.
+000103b0: 2c20 666f 7220 6576 6572 7920 7a2c 206d  , for every z, m
+000103c0: 6172 6769 6e28 782c 207a 2920 3e3d 206d  argin(x, z) >= m
+000103d0: 6172 6769 6e28 792c 207a 290a 2020 2020  argin(y, z).    
+000103e0: 2020 2020 2020 2020 636f 7665 7273 203d          covers =
+000103f0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+00010400: 2020 666f 7220 7a20 696e 2063 616e 6469    for z in candi
+00010410: 6461 7465 733a 0a20 2020 2020 2020 2020  dates:.         
+00010420: 2020 2020 2020 2069 6620 6564 6174 612e         if edata.
+00010430: 6d61 7267 696e 2878 2c20 7a29 203c 2065  margin(x, z) < e
+00010440: 6461 7461 2e6d 6172 6769 6e28 792c 207a  data.margin(y, z
+00010450: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00010460: 2020 2020 2020 2063 6f76 6572 7320 3d20         covers = 
+00010470: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00010480: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+00010490: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+000104a0: 2020 2020 2020 2069 6620 636f 7665 7273         if covers
+000104b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000104c0: 2020 6973 5f69 6e5f 7563 7320 3d20 4661    is_in_ucs = Fa
+000104d0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+000104e0: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+000104f0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00010500: 2020 2069 6620 6973 5f69 6e5f 7563 733a     if is_in_ucs:
+00010510: 0a20 2020 2020 2020 2020 2020 2075 635f  .            uc_
+00010520: 7365 742e 6170 7065 6e64 2879 290a 0a20  set.append(y).. 
+00010530: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
+00010540: 2875 635f 7365 7429 0a0a 4076 6d28 6e61  (uc_set)..@vm(na
+00010550: 6d65 203d 2022 4c6f 7373 2d54 7269 6d6d  me = "Loss-Trimm
+00010560: 6572 2056 6f74 696e 6722 290a 6465 6620  er Voting").def 
+00010570: 6c6f 7373 5f74 7269 6d6d 6572 2865 6461  loss_trimmer(eda
+00010580: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
+00010590: 204e 6f6e 6529 3a0a 2020 2020 2222 2249   None):.    """I
+000105a0: 7465 7261 7469 7665 6c79 2065 6c69 6d69  teratively elimi
+000105b0: 6e61 7465 2074 6865 2063 616e 6469 6461  nate the candida
+000105c0: 7465 2077 6974 6820 7468 6520 6c61 7267  te with the larg
+000105d0: 6573 7420 7375 6d20 6f66 206d 6172 6769  est sum of margi
+000105e0: 6e73 206f 6620 6c6f 7373 2075 6e74 696c  ns of loss until
+000105f0: 2061 2043 6f6e 646f 7263 6574 2077 696e   a Condorcet win
+00010600: 6e65 7220 6973 2066 6f75 6e64 2e20 496e  ner is found. In
+00010610: 2074 6869 7320 7665 7273 696f 6e20 6f66   this version of
+00010620: 2074 6865 206d 6574 686f 642c 2070 6172   the method, par
+00010630: 616c 6c65 6c2d 756e 6976 6572 7365 2074  allel-universe t
+00010640: 6965 6272 6561 6b69 6e67 2069 7320 7573  iebreaking is us
+00010650: 6564 2069 6620 7468 6572 6520 6172 6520  ed if there are 
+00010660: 6d75 6c74 6970 6c65 2063 616e 6469 6461  multiple candida
+00010670: 7465 7320 7769 7468 2074 6865 206c 6172  tes with the lar
+00010680: 6765 7374 2073 756d 206f 6620 6d61 7267  gest sum of marg
+00010690: 696e 7320 6f66 206c 6f73 732e 0a0a 2020  ins of loss...  
+000106a0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000106b0: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
+000106c0: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
+000106d0: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
+000106e0: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
+000106f0: 2074 6861 7420 6861 7320 6120 6d61 7267   that has a marg
+00010700: 696e 206d 6574 686f 642e 0a20 2020 2020  in method..     
+00010710: 2020 2063 7572 725f 6361 6e64 7320 284c     curr_cands (L
+00010720: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
+00010730: 616c 293a 2049 6620 7365 742c 2074 6865  al): If set, the
+00010740: 6e20 6669 6e64 2074 6865 2077 696e 6e65  n find the winne
+00010750: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
+00010760: 6c65 2072 6573 7472 6963 7465 6420 746f  le restricted to
+00010770: 2074 6865 2063 616e 6469 6461 7465 7320   the candidates 
+00010780: 696e 2060 6063 7572 725f 6361 6e64 7360  in ``curr_cands`
+00010790: 600a 0a20 2020 2052 6574 7572 6e73 3a20  `..    Returns: 
+000107a0: 0a20 2020 2020 2020 2041 2073 6f72 7465  .        A sorte
+000107b0: 6420 6c69 7374 206f 6620 6361 6e64 6964  d list of candid
+000107c0: 6174 6573 0a0a 2020 2020 2e2e 206e 6f74  ates..    .. not
+000107d0: 653a 3a0a 2020 2020 2020 2020 4d65 7468  e::.        Meth
+000107e0: 6f64 2070 726f 706f 7365 6420 6279 2052  od proposed by R
+000107f0: 6963 6861 7264 2042 2e20 4461 726c 696e  ichard B. Darlin
+00010800: 6774 6f6e 2069 6e20 2254 6865 2043 6173  gton in "The Cas
+00010810: 6520 666f 7220 7468 6520 4c6f 7373 2d54  e for the Loss-T
+00010820: 7269 6d6d 6572 2056 6f74 696e 6720 5379  rimmer Voting Sy
+00010830: 7374 656d 2e22 0a0a 2020 2020 2222 220a  stem."..    """.
+00010840: 0a20 2020 2063 7572 725f 6361 6e64 7320  .    curr_cands 
+00010850: 3d20 6564 6174 612e 6361 6e64 6964 6174  = edata.candidat
+00010860: 6573 2069 6620 6375 7272 5f63 616e 6473  es if curr_cands
+00010870: 2069 7320 4e6f 6e65 2065 6c73 6520 6375   is None else cu
+00010880: 7272 5f63 616e 6473 0a0a 2020 2020 7765  rr_cands..    we
+00010890: 616b 5f63 7720 3d20 6564 6174 612e 7765  ak_cw = edata.we
+000108a0: 616b 5f63 6f6e 646f 7263 6574 5f77 696e  ak_condorcet_win
+000108b0: 6e65 7228 6375 7272 5f63 616e 6473 203d  ner(curr_cands =
+000108c0: 2063 7572 725f 6361 6e64 7329 0a20 2020   curr_cands).   
+000108d0: 2023 2049 6620 7468 6572 6520 6172 6520   # If there are 
+000108e0: 7765 616b 2043 6f6e 646f 7263 6574 2077  weak Condorcet w
+000108f0: 696e 6e65 7273 2c20 7265 7475 726e 2074  inners, return t
+00010900: 686f 7365 2063 616e 6469 6461 7465 730a  hose candidates.
+00010910: 2020 2020 6966 2065 6461 7461 2e77 6561      if edata.wea
+00010920: 6b5f 636f 6e64 6f72 6365 745f 7769 6e6e  k_condorcet_winn
+00010930: 6572 2863 7572 725f 6361 6e64 7320 3d20  er(curr_cands = 
+00010940: 6375 7272 5f63 616e 6473 2920 6973 206e  curr_cands) is n
+00010950: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00010960: 2072 6574 7572 6e20 736f 7274 6564 2877   return sorted(w
+00010970: 6561 6b5f 6377 290a 2020 2020 0a20 2020  eak_cw).    .   
+00010980: 2023 204f 7468 6572 7769 7365 2c20 6361   # Otherwise, ca
+00010990: 6c63 756c 6174 6520 7468 6520 7375 6d20  lculate the sum 
+000109a0: 6f66 206d 6172 6769 6e73 206f 6620 6c6f  of margins of lo
+000109b0: 7373 2066 6f72 2065 6163 6820 6361 6e64  ss for each cand
+000109c0: 6964 6174 650a 2020 2020 7375 6d5f 6f66  idate.    sum_of
+000109d0: 5f6d 6172 6769 6e73 5f6f 665f 6c6f 7373  _margins_of_loss
+000109e0: 203d 207b 6361 6e64 3a20 7375 6d28 5b65   = {cand: sum([e
+000109f0: 6461 7461 2e6d 6172 6769 6e28 6f74 6865  data.margin(othe
+00010a00: 725f 6361 6e64 2c20 6361 6e64 2920 666f  r_cand, cand) fo
+00010a10: 7220 6f74 6865 725f 6361 6e64 2069 6e20  r other_cand in 
+00010a20: 6375 7272 5f63 616e 6473 2069 6620 6564  curr_cands if ed
+00010a30: 6174 612e 6d61 7267 696e 286f 7468 6572  ata.margin(other
+00010a40: 5f63 616e 642c 2063 616e 6429 203e 2030  _cand, cand) > 0
+00010a50: 5d29 2066 6f72 2063 616e 6420 696e 2063  ]) for cand in c
+00010a60: 7572 725f 6361 6e64 737d 0a0a 2020 2020  urr_cands}..    
+00010a70: 2320 4669 6e64 2074 6865 2063 616e 6469  # Find the candi
+00010a80: 6461 7465 7320 7769 7468 2074 6865 206c  dates with the l
+00010a90: 6172 6765 7374 2073 756d 206f 6620 6d61  argest sum of ma
+00010aa0: 7267 696e 7320 6f66 206c 6f73 730a 2020  rgins of loss.  
+00010ab0: 2020 6d61 785f 7375 6d5f 6f66 5f6d 6172    max_sum_of_mar
+00010ac0: 6769 6e73 5f6f 665f 6c6f 7373 203d 206d  gins_of_loss = m
+00010ad0: 6178 2873 756d 5f6f 665f 6d61 7267 696e  ax(sum_of_margin
+00010ae0: 735f 6f66 5f6c 6f73 732e 7661 6c75 6573  s_of_loss.values
+00010af0: 2829 290a 2020 2020 6269 6767 6573 745f  ()).    biggest_
+00010b00: 6c6f 7365 7273 203d 205b 6361 6e64 2066  losers = [cand f
+00010b10: 6f72 2063 616e 6420 696e 2063 7572 725f  or cand in curr_
+00010b20: 6361 6e64 7320 6966 2073 756d 5f6f 665f  cands if sum_of_
+00010b30: 6d61 7267 696e 735f 6f66 5f6c 6f73 735b  margins_of_loss[
+00010b40: 6361 6e64 5d20 3d3d 206d 6178 5f73 756d  cand] == max_sum
+00010b50: 5f6f 665f 6d61 7267 696e 735f 6f66 5f6c  _of_margins_of_l
+00010b60: 6f73 735d 0a0a 2020 2020 7769 6e6e 6572  oss]..    winner
+00010b70: 7320 3d20 5b5d 0a0a 2020 2020 2320 466f  s = []..    # Fo
+00010b80: 7220 6561 6368 2062 6967 6765 7374 206c  r each biggest l
+00010b90: 6f73 6572 2c20 6361 6c63 756c 6174 6520  oser, calculate 
+00010ba0: 7468 6520 7769 6e6e 6572 7320 6166 7465  the winners afte
+00010bb0: 7220 7265 6d6f 7669 6e67 2074 6861 7420  r removing that 
+00010bc0: 6361 6e64 6964 6174 652e 2054 6865 2075  candidate. The u
+00010bd0: 6e69 6f6e 206f 6620 7468 6573 6520 7365  nion of these se
+00010be0: 7473 2069 7320 7468 6520 7365 7420 6f66  ts is the set of
+00010bf0: 2077 696e 6e65 7273 2e0a 2020 2020 666f   winners..    fo
+00010c00: 7220 626c 2069 6e20 6269 6767 6573 745f  r bl in biggest_
+00010c10: 6c6f 7365 7273 3a0a 2020 2020 2020 2020  losers:.        
+00010c20: 7769 6e6e 6572 735f 7769 7468 6f75 745f  winners_without_
+00010c30: 626c 203d 206c 6f73 735f 7472 696d 6d65  bl = loss_trimme
+00010c40: 7228 6564 6174 612c 2063 7572 725f 6361  r(edata, curr_ca
+00010c50: 6e64 7320 3d20 5b63 616e 6420 666f 7220  nds = [cand for 
+00010c60: 6361 6e64 2069 6e20 6375 7272 5f63 616e  cand in curr_can
+00010c70: 6473 2069 6620 6361 6e64 2021 3d20 626c  ds if cand != bl
+00010c80: 5d29 0a20 2020 2020 2020 2077 696e 6e65  ]).        winne
+00010c90: 7273 202b 3d20 7769 6e6e 6572 735f 7769  rs += winners_wi
+00010ca0: 7468 6f75 745f 626c 0a0a 2020 2020 7265  thout_bl..    re
+00010cb0: 7475 726e 2073 6f72 7465 6428 6c69 7374  turn sorted(list
+00010cc0: 2873 6574 2877 696e 6e65 7273 2929 290a  (set(winners))).
+00010cd0: 0a0a 6465 6620 6469 7374 616e 6365 5f74  ..def distance_t
+00010ce0: 6f5f 6d61 7267 696e 5f67 7261 7068 2865  o_margin_graph(e
+00010cf0: 6461 7461 2c20 7265 6c2c 2065 7870 203d  data, rel, exp =
+00010d00: 2031 2c20 6375 7272 5f63 616e 6473 203d   1, curr_cands =
+00010d10: 204e 6f6e 6529 3a20 0a20 2020 2022 2222   None): .    """
+00010d20: 0a20 2020 2043 616c 6375 6c61 7465 2074  .    Calculate t
+00010d30: 6865 2064 6973 7461 6e63 6520 6f66 2060  he distance of `
+00010d40: 6072 656c 6060 2028 6120 7265 6c61 7469  `rel`` (a relati
+00010d50: 6f6e 2920 746f 2074 6865 206d 616a 6f72  on) to the major
+00010d60: 6974 7920 6772 6170 6820 6f66 2060 6065  ity graph of ``e
+00010d70: 6461 7461 6060 2e20 0a20 2020 2022 2222  data``. .    """
+00010d80: 0a20 2020 2063 616e 6469 6461 7465 7320  .    candidates 
+00010d90: 3d20 6564 6174 612e 6361 6e64 6964 6174  = edata.candidat
+00010da0: 6573 2069 6620 6375 7272 5f63 616e 6473  es if curr_cands
+00010db0: 2069 7320 4e6f 6e65 2065 6c73 6520 6375   is None else cu
+00010dc0: 7272 5f63 616e 6473 0a20 2020 200a 2020  rr_cands.    .  
+00010dd0: 2020 6966 2074 7970 6528 6564 6174 6129    if type(edata)
+00010de0: 203d 3d20 4d61 6a6f 7269 7479 4772 6170   == MajorityGrap
+00010df0: 6820 616e 6420 6578 7020 3d3d 2030 3a0a  h and exp == 0:.
+00010e00: 2020 2020 2020 2020 2320 6966 2065 6461          # if eda
+00010e10: 7461 2069 7320 6120 4d61 6a6f 7269 7479  ta is a Majority
+00010e20: 4772 6170 682c 2077 6520 6e65 6564 2074  Graph, we need t
+00010e30: 6f20 6164 6420 6d61 7267 696e 7320 666f  o add margins fo
+00010e40: 7220 7468 6520 666f 6c6c 6f77 696e 6720  r the following 
+00010e50: 636f 6465 2074 6f20 776f 726b 2e20 2054  code to work.  T
+00010e60: 6865 206d 6172 6769 6e73 2064 6f20 6e6f  he margins do no
+00010e70: 7420 6d61 7474 6572 2077 6865 6e20 6578  t matter when ex
+00010e80: 703d 3d30 2e20 2020 0a20 2020 2020 2020  p==0.   .       
+00010e90: 2065 6461 7461 203d 204d 6172 6769 6e47   edata = MarginG
+00010ea0: 7261 7068 2863 616e 6469 6461 7465 732c  raph(candidates,
+00010eb0: 205b 2863 312c 2063 322c 2031 2920 666f   [(c1, c2, 1) fo
+00010ec0: 7220 6331 2c20 6332 2069 6e20 6564 6174  r c1, c2 in edat
+00010ed0: 612e 6564 6765 7320 6966 2028 6331 2069  a.edges if (c1 i
+00010ee0: 6e20 6361 6e64 6964 6174 6573 2061 6e64  n candidates and
+00010ef0: 2063 3220 696e 2063 616e 6469 6461 7465   c2 in candidate
+00010f00: 7329 5d29 0a20 2020 2070 656e 616c 7479  s)]).    penalty
+00010f10: 203d 2030 0a20 2020 2066 6f72 2061 2c62   = 0.    for a,b
+00010f20: 2069 6e20 636f 6d62 696e 6174 696f 6e73   in combinations
+00010f30: 2863 616e 6469 6461 7465 732c 2032 293a  (candidates, 2):
+00010f40: 200a 2020 2020 2020 2020 6966 2065 6461   .        if eda
+00010f50: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+00010f60: 6572 7328 612c 2062 2920 616e 6420 2862  ers(a, b) and (b
+00010f70: 2c61 2920 696e 2072 656c 3a20 0a20 2020  ,a) in rel: .   
+00010f80: 2020 2020 2020 2020 2070 656e 616c 7479           penalty
+00010f90: 202b 3d20 2865 6461 7461 2e6d 6172 6769   += (edata.margi
+00010fa0: 6e28 612c 2062 2920 2a2a 2065 7870 290a  n(a, b) ** exp).
+00010fb0: 2020 2020 2020 2020 656c 6966 2065 6461          elif eda
+00010fc0: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+00010fd0: 6572 7328 622c 2061 2920 616e 6420 2861  ers(b, a) and (a
+00010fe0: 2c62 2920 696e 2072 656c 3a20 0a20 2020  ,b) in rel: .   
+00010ff0: 2020 2020 2020 2020 2070 656e 616c 7479           penalty
+00011000: 202b 3d20 2865 6461 7461 2e6d 6172 6769   += (edata.margi
+00011010: 6e28 622c 2061 2920 2a2a 2065 7870 290a  n(b, a) ** exp).
+00011020: 2020 2020 2020 2020 656c 6966 2065 6461          elif eda
+00011030: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+00011040: 6572 7328 612c 2062 2920 616e 6420 2861  ers(a, b) and (a
+00011050: 2c62 2920 6e6f 7420 696e 2072 656c 2061  ,b) not in rel a
+00011060: 6e64 2028 622c 6129 206e 6f74 2069 6e20  nd (b,a) not in 
+00011070: 7265 6c3a 200a 2020 2020 2020 2020 2020  rel: .          
+00011080: 2020 7065 6e61 6c74 7920 2b3d 2028 6564    penalty += (ed
+00011090: 6174 612e 6d61 7267 696e 2861 2c20 6229  ata.margin(a, b)
+000110a0: 202a 2a20 6578 7029 202f 2032 200a 2020   ** exp) / 2 .  
+000110b0: 2020 2020 2020 656c 6966 2065 6461 7461        elif edata
+000110c0: 2e6d 616a 6f72 6974 795f 7072 6566 6572  .majority_prefer
+000110d0: 7328 622c 2061 2920 616e 6420 2861 2c62  s(b, a) and (a,b
+000110e0: 2920 6e6f 7420 696e 2072 656c 2061 6e64  ) not in rel and
+000110f0: 2028 622c 6129 206e 6f74 2069 6e20 7265   (b,a) not in re
+00011100: 6c3a 200a 2020 2020 2020 2020 2020 2020  l: .            
+00011110: 7065 6e61 6c74 7920 2b3d 2028 6564 6174  penalty += (edat
+00011120: 612e 6d61 7267 696e 2862 2c20 6129 202a  a.margin(b, a) *
+00011130: 2a20 6578 7029 2020 2f20 320a 2020 2020  * exp)  / 2.    
+00011140: 7265 7475 726e 2070 656e 616c 7479 0a0a  return penalty..
+00011150: 0a6d 675f 766d 7320 3d20 5b0a 2020 2020  .mg_vms = [.    
+00011160: 6d69 6e69 6d61 782c 200a 2020 2020 7370  minimax, .    sp
+00011170: 6c69 745f 6379 636c 652c 0a20 2020 2023  lit_cycle,.    #
+00011180: 7370 6c69 745f 6379 636c 655f 466c 6f79  split_cycle_Floy
+00011190: 645f 5761 7273 6861 6c6c 2c0a 2020 2020  d_Warshall,.    
+000111a0: 2362 6561 745f 7061 7468 2c0a 2020 2020  #beat_path,.    
+000111b0: 6265 6174 5f70 6174 685f 466c 6f79 645f  beat_path_Floyd_
+000111c0: 5761 7273 6861 6c6c 2c0a 2020 2020 2372  Warshall,.    #r
+000111d0: 616e 6b65 645f 7061 6972 732c 0a20 2020  anked_pairs,.   
+000111e0: 2023 7261 6e6b 6564 5f70 6169 7273 5f77   #ranked_pairs_w
+000111f0: 6974 685f 7465 7374 2c0a 2020 2020 7261  ith_test,.    ra
+00011200: 6e6b 6564 5f70 6169 7273 5f7a 742c 0a20  nked_pairs_zt,. 
+00011210: 2020 2072 616e 6b65 645f 7061 6972 735f     ranked_pairs_
+00011220: 7462 2c0a 2020 2020 2372 6976 6572 2c0a  tb,.    #river,.
+00011230: 2020 2020 2372 6976 6572 5f77 6974 685f      #river_with_
+00011240: 7465 7374 2c20 0a20 2020 2073 696d 706c  test, .    simpl
+00011250: 655f 7374 6162 6c65 5f76 6f74 696e 672c  e_stable_voting,
+00011260: 0a20 2020 2023 7369 6d70 6c65 5f73 7461  .    #simple_sta
+00011270: 626c 655f 766f 7469 6e67 5f66 6173 7465  ble_voting_faste
+00011280: 722c 0a20 2020 2073 7461 626c 655f 766f  r,.    stable_vo
+00011290: 7469 6e67 2c0a 2020 2020 2373 7461 626c  ting,.    #stabl
+000112a0: 655f 766f 7469 6e67 5f66 6173 7465 722c  e_voting_faster,
+000112b0: 0a20 2020 2065 7373 656e 7469 616c 2c0a  .    essential,.
+000112c0: 2020 2020 7765 6967 6874 6564 5f63 6f76      weighted_cov
+000112d0: 6572 696e 672c 0a20 2020 206c 6f73 735f  ering,.    loss_
+000112e0: 7472 696d 6d65 720a 5d0a 0a0a 6d67 5f76  trimmer.]...mg_v
+000112f0: 6d73 5f61 6c6c 203d 205b 0a20 2020 206d  ms_all = [.    m
+00011300: 696e 696d 6178 2c20 0a20 2020 2073 706c  inimax, .    spl
+00011310: 6974 5f63 7963 6c65 2c0a 2020 2020 7370  it_cycle,.    sp
+00011320: 6c69 745f 6379 636c 655f 466c 6f79 645f  lit_cycle_Floyd_
+00011330: 5761 7273 6861 6c6c 2c0a 2020 2020 6265  Warshall,.    be
+00011340: 6174 5f70 6174 682c 0a20 2020 2062 6561  at_path,.    bea
+00011350: 745f 7061 7468 5f46 6c6f 7964 5f57 6172  t_path_Floyd_War
+00011360: 7368 616c 6c2c 0a20 2020 2072 616e 6b65  shall,.    ranke
+00011370: 645f 7061 6972 732c 0a20 2020 2072 616e  d_pairs,.    ran
+00011380: 6b65 645f 7061 6972 735f 7769 7468 5f74  ked_pairs_with_t
+00011390: 6573 742c 0a20 2020 2072 616e 6b65 645f  est,.    ranked_
+000113a0: 7061 6972 735f 7a74 2c0a 2020 2020 7261  pairs_zt,.    ra
+000113b0: 6e6b 6564 5f70 6169 7273 5f74 622c 0a20  nked_pairs_tb,. 
+000113c0: 2020 2072 616e 6b65 645f 7061 6972 735f     ranked_pairs_
+000113d0: 6672 6f6d 5f73 7461 636b 732c 0a20 2020  from_stacks,.   
+000113e0: 2072 6976 6572 2c0a 2020 2020 7269 7665   river,.    rive
+000113f0: 725f 7769 7468 5f74 6573 742c 200a 2020  r_with_test, .  
+00011400: 2020 7369 6d70 6c65 5f73 7461 626c 655f    simple_stable_
+00011410: 766f 7469 6e67 2c0a 2020 2020 7369 6d70  voting,.    simp
+00011420: 6c65 5f73 7461 626c 655f 766f 7469 6e67  le_stable_voting
+00011430: 5f66 6173 7465 722c 0a20 2020 2073 7461  _faster,.    sta
+00011440: 626c 655f 766f 7469 6e67 2c0a 2020 2020  ble_voting,.    
+00011450: 7374 6162 6c65 5f76 6f74 696e 675f 6661  stable_voting_fa
+00011460: 7374 6572 2c0a 2020 2020 6573 7365 6e74  ster,.    essent
+00011470: 6961 6c2c 0a20 2020 2077 6569 6768 7465  ial,.    weighte
+00011480: 645f 636f 7665 7269 6e67 2c0a 2020 2020  d_covering,.    
+00011490: 6c6f 7373 5f74 7269 6d6d 6572 0a5d       loss_trimmer.]
```

### Comparing `pref_voting-1.0.0/pref_voting/monotonicity_axioms.py` & `pref_voting-1.1.0/pref_voting/monotonicity_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/other_methods.py` & `pref_voting-1.1.0/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/prob_voting_method.py` & `pref_voting-1.1.0/pref_voting/prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/probabilistic_methods.py` & `pref_voting-1.1.0/pref_voting/probabilistic_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/profiles.py` & `pref_voting-1.1.0/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/profiles_with_ties.py` & `pref_voting-1.1.0/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/rankings.py` & `pref_voting-1.1.0/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/scoring_methods.py` & `pref_voting-1.1.0/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/social_welfare_function.py` & `pref_voting-1.1.0/pref_voting/social_welfare_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/spatial_profiles.py` & `pref_voting-1.1.0/pref_voting/spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/strategic_axioms.py` & `pref_voting-1.1.0/pref_voting/strategic_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/conftest.py` & `pref_voting-1.1.0/pref_voting/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_c1_methods.py` & `pref_voting-1.1.0/pref_voting/tests/test_c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_combined_methods.py` & `pref_voting-1.1.0/pref_voting/tests/test_combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_generate_profiles.py` & `pref_voting-1.1.0/pref_voting/tests/test_generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_generate_spatial_profile.py` & `pref_voting-1.1.0/pref_voting/tests/test_generate_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_io.py` & `pref_voting-1.1.0/pref_voting/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_iterative_methods.py` & `pref_voting-1.1.0/pref_voting/tests/test_iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_majority_graph.py` & `pref_voting-1.1.0/pref_voting/tests/test_majority_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_mapping.py` & `pref_voting-1.1.0/pref_voting/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_margin_graph.py` & `pref_voting-1.1.0/pref_voting/tests/test_margin_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_other_methods.py` & `pref_voting-1.1.0/pref_voting/tests/test_other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_prob_voting_method.py` & `pref_voting-1.1.0/pref_voting/tests/test_prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_profile.py` & `pref_voting-1.1.0/pref_voting/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_profile_with_ties.py` & `pref_voting-1.1.0/pref_voting/tests/test_profile_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_ranking.py` & `pref_voting-1.1.0/pref_voting/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_scoring_rules.py` & `pref_voting-1.1.0/pref_voting/tests/test_scoring_rules.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_social_welfare_functions.py` & `pref_voting-1.1.0/pref_voting/tests/test_social_welfare_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_spatial_profile.py` & `pref_voting-1.1.0/pref_voting/tests/test_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_support_graph.py` & `pref_voting-1.1.0/pref_voting/tests/test_support_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_utility_function.py` & `pref_voting-1.1.0/pref_voting/tests/test_utility_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_utility_functions.py` & `pref_voting-1.1.0/pref_voting/tests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/tests/test_voting_method.py` & `pref_voting-1.1.0/pref_voting/tests/test_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/utility_functions.py` & `pref_voting-1.1.0/pref_voting/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/utility_methods.py` & `pref_voting-1.1.0/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/utility_profiles.py` & `pref_voting-1.1.0/pref_voting/utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/variable_candidate_axioms.py` & `pref_voting-1.1.0/pref_voting/variable_candidate_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/variable_voter_axioms.py` & `pref_voting-1.1.0/pref_voting/variable_voter_axioms.py`

 * *Files 25% similar despite different names*

```diff
@@ -270,15 +270,15 @@
     if require_uniquely_weighted and not prof.is_uniquely_weighted():
         return False
 
     if violation_type == "Removal":
         if uniform_coalition:
             for loser in losers:
 
-                relevant_ranking_types = [r for r in prof.ranking_types if r[0] == loser and prof.rankings.count(r) >= coalition_size]
+                relevant_ranking_types = [r for r in prof.ranking_types if prof.rankings.count(r) >= coalition_size]
 
                 for r in relevant_ranking_types:
 
                     rankings = prof.rankings
 
                     for i in range(coalition_size):
                         rankings.remove(r) # remove coalition_size-many tokens of the type of ranking
@@ -298,14 +298,15 @@
 
                     if require_uniquely_weighted and not prof2.is_uniquely_weighted():
                         continue
                     
                     if loser in winners2:
 
                         if verbose:
+                            prof = prof.anonymize()
                             if coalition_size == 1:
                                 print(f"{loser} loses in the full profile, but {loser} is a winner after removing voter with the ranking {str(r)}:")
                             else:
                                 print(f"{loser} loses in the full profile, but {loser} is a winner after removing {coalition_size} voters with the ranking {str(r)}:")
                             print("")
                             print("Full profile:")
                             prof.display()
@@ -313,19 +314,19 @@
                             prof.display_margin_graph()
                             vm.display(prof)
                             print("")
                             if coalition_size == 1:
                                 print(f"Profile with voter removed:")
                             else:
                                 print(f"Profile with {coalition_size} voters removed:")
-                            anonprof2 = prof2.anonymize()
-                            anonprof2.display()
-                            print(anonprof2.description())
-                            anonprof2.display_margin_graph()
-                            vm.display(anonprof2)
+                            prof2 = prof2.anonymize()
+                            prof2.display()
+                            print(prof2.description())
+                            prof2.display_margin_graph()
+                            vm.display(prof2)
                             print("")
                         return True
                     
             if check_probabilities:
                 for winner in winners:
 
                     relevant_ranking_types = [r for r in prof.ranking_types if r[0] == winner and prof.rankings.count(r) >= coalition_size]
@@ -352,14 +353,15 @@
 
                         if require_uniquely_weighted and not prof2.is_uniquely_weighted():
                             continue
                         
                         if winner in winners2 and len(winners) > len(winners2):
 
                             if verbose:
+                                prof = prof.anonymize()
                                 if coalition_size == 1:
                                     print(f"{winner} has a higher probability of winning after removing voter with the ranking {str(r)}:")
                                 else:
                                     print(f"{winner} has a higher probability of winning after removing removing {coalition_size} voters with the ranking {str(r)}:")
                                 print("")
                                 print("Full profile:")
                                 prof.display()
@@ -367,19 +369,19 @@
                                 prof.display_margin_graph()
                                 vm.display(prof)
                                 print("")
                                 if coalition_size == 1:
                                     print(f"Profile with voter removed:")
                                 else:
                                     print(f"Profile with {coalition_size} voters removed:")
-                                anonprof2 = prof2.anonymize()
-                                anonprof2.display()
-                                print(anonprof2.description())
-                                anonprof2.display_margin_graph()
-                                vm.display(anonprof2)
+                                prof2 = prof2.anonymize()
+                                prof2.display()
+                                print(prof2.description())
+                                prof2.display_margin_graph()
+                                vm.display(prof2)
                                 print("")
                             return True
 
         
         if not uniform_coalition:
             for loser in losers:
 
@@ -409,28 +411,29 @@
 
                     if require_uniquely_weighted and not prof2.is_uniquely_weighted():
                         continue
                     
                     if loser in winners2:
 
                         if verbose:
+                            prof = prof.anonymize()
                             print(f"{loser} loses in the full profile, but {loser} is a winner after removing a {coalition_size}-voter coalition with the rankings {[str(r) for r in coalition_rankings]} and counts {coalition_rankings_counts}:")
                             print("")
                             print("Full profile:")
                             prof.display()
                             print(prof.description())
                             prof.display_margin_graph()
                             vm.display(prof)
                             print("")
                             print(f"Profile with coalition removed:")
-                            anonprof2 = prof2.anonymize()
-                            anonprof2.display()
-                            print(anonprof2.description())
-                            anonprof2.display_margin_graph()
-                            vm.display(anonprof2)
+                            prof2 = prof2.anonymize()
+                            prof2.display()
+                            print(prof2.description())
+                            prof2.display_margin_graph()
+                            vm.display(prof2)
                             print("")
                         return True
                     
             if check_probabilities:
                 for winner in winners:
 
                     relevant_ranking_types = [r for r in prof.ranking_types if r[0] == winner]
@@ -459,28 +462,29 @@
 
                         if require_uniquely_weighted and not prof2.is_uniquely_weighted():
                             continue
                         
                         if winner in winners2 and len(winners) > len(winners2):
 
                             if verbose:
+                                prof = prof.anonymize()
                                 print(f"{winner} has a higher probability of winning after removing a {coalition_size}-voter coalition with the rankings {[str(r) for r in coalition_rankings]} and counts {coalition_rankings_counts}:")
                                 print("")
                                 print("Full profile:")
                                 prof.display()
                                 print(prof.description())
                                 prof.display_margin_graph()
                                 vm.display(prof)
                                 print("")
                                 print(f"Profile with coalition removed:")
-                                anonprof2 = prof2.anonymize()
-                                anonprof2.display()
-                                print(anonprof2.description())
-                                anonprof2.display_margin_graph()
-                                vm.display(anonprof2)
+                                prof2 = prof2.anonymize()
+                                prof2.display()
+                                print(prof2.description())
+                                prof2.display_margin_graph()
+                                vm.display(prof2)
                                 print("")
                             return True
     
     return False
                     
 def find_all_positive_involvement_violations(prof, vm, verbose=False, violation_type="Removal", coalition_size = 1, uniform_coalition = True, require_resoluteness = False, require_uniquely_weighted = False, check_probabilities = False):
     """
@@ -545,14 +549,15 @@
 
                     if require_uniquely_weighted and not prof2.is_uniquely_weighted():
                         continue
 
                     if loser in winners2:
                         witnesses.append((loser, [r], [coalition_size]))
                         if verbose:
+                            prof = prof.anonymize()
                             if coalition_size == 1:
                                 print(f"{loser} loses in the full profile, but {loser} is a winner after removing voter with the ranking {str(r)}:")
                             else:
                                 print(f"{loser} loses in the full profile, but {loser} is a winner after removing {coalition_size} voters with the ranking {str(r)}:")
                             print("")
                             print("Full profile")
                             prof.display()
@@ -560,19 +565,19 @@
                             prof.display_margin_graph()
                             vm.display(prof)
                             print("")
                             if coalition_size == 1:
                                 print(f"Profile with voter removed:")
                             else:
                                 print(f"Profile with {coalition_size} voters removed:")
-                            anonprof2 = prof2.anonymize()
-                            anonprof2.display()
-                            print(anonprof2.description())
-                            anonprof2.display_margin_graph()
-                            vm.display(anonprof2)
+                            prof2 = prof2.anonymize()
+                            prof2.display()
+                            print(prof2.description())
+                            prof2.display_margin_graph()
+                            vm.display(prof2)
                             print("")
             
             if check_probabilities:
                 for winner in winners:
                     relevant_ranking_types = [r for r in prof.ranking_types if r[0] == winner and prof.rankings.count(r) >= coalition_size]
 
                     for r in relevant_ranking_types:
@@ -597,14 +602,15 @@
 
                         if require_uniquely_weighted and not prof2.is_uniquely_weighted():
                             continue
 
                         if winner in winners2 and len(winners) > len(winners2):
                             witnesses.append((winner, [r], [coalition_size]))
                             if verbose:
+                                prof = prof.anonymize()
                                 if coalition_size == 1:
                                     print(f"{winner} has a higher probability of winning after removing voter with the ranking {str(r)}:")
                                 else:
                                     print(f"{winner} has a higher probability of winning after removing {coalition_size} voters with the ranking {str(r)}:")
                                 print("")
                                 print("Full profile")
                                 prof.display()
@@ -612,19 +618,19 @@
                                 prof.display_margin_graph()
                                 vm.display(prof)
                                 print("")
                                 if coalition_size == 1:
                                     print(f"Profile with voter removed:")
                                 else:
                                     print(f"Profile with {coalition_size} voters removed:")
-                                anonprof2 = prof2.anonymize()
-                                anonprof2.display()
-                                print(anonprof2.description())
-                                anonprof2.display_margin_graph()
-                                vm.display(anonprof2)
+                                prof2 = prof2.anonymize()
+                                prof2.display()
+                                print(prof2.description())
+                                prof2.display_margin_graph()
+                                vm.display(prof2)
                                 print("")
 
 
         if not uniform_coalition:
             for loser in losers:
                 relevant_ranking_types = [r for r in prof.ranking_types if r[0] == loser]
                 relevant_ranking_types_counts = [prof.rankings.count(r) for r in relevant_ranking_types]
@@ -652,28 +658,29 @@
 
                     if require_uniquely_weighted and not prof2.is_uniquely_weighted():
                         continue
 
                     if loser in winners2:
                         witnesses.append((loser, coalition_rankings, coalition_rankings_counts))
                         if verbose:
+                            prof = prof.anonymize()
                             print(f"{loser} loses in the full profile, but {loser} is a winner after removing a {coalition_size}-voter coalition with the rankings {[str(r) for r in coalition_rankings]} and counts {coalition_rankings_counts}:")
                             print("")
                             print("Full profile")
                             prof.display()
                             print(prof.description())
                             prof.display_margin_graph()
                             vm.display(prof)
                             print("")
                             print(f"Profile with coalition removed:")
-                            anonprof2 = prof2.anonymize()
-                            anonprof2.display()
-                            print(anonprof2.description())
-                            anonprof2.display_margin_graph()
-                            vm.display(anonprof2)
+                            prof2 = prof2.anonymize()
+                            prof2.display()
+                            print(prof2.description())
+                            prof2.display_margin_graph()
+                            vm.display(prof2)
                             print("")
 
             if check_probabilities:
                 for winner in winners:
                     relevant_ranking_types = [r for r in prof.ranking_types if r[0] == winner]
                     relevant_ranking_types_counts = [prof.rankings.count(r) for r in relevant_ranking_types]
 
@@ -700,28 +707,29 @@
 
                         if require_uniquely_weighted and not prof2.is_uniquely_weighted():
                             continue
 
                         if winner in winners2 and len(winners) > len(winners2):
                             witnesses.append((winner, coalition_rankings, coalition_rankings_counts))
                             if verbose:
+                                prof = prof.anonymize()
                                 print(f"{winner} has a higher probability of winning after removing a {coalition_size}-voter coalition with the rankings {[str(r) for r in coalition_rankings]} and counts {coalition_rankings_counts}:")
                                 print("")
                                 print("Full profile")
                                 prof.display()
                                 print(prof.description())
                                 prof.display_margin_graph()
                                 vm.display(prof)
                                 print("")
                                 print(f"Profile with coalition removed:")
-                                anonprof2 = prof2.anonymize()
-                                anonprof2.display()
-                                print(anonprof2.description())
-                                anonprof2.display_margin_graph()
-                                vm.display(anonprof2)
+                                prof2 = prof2.anonymize()
+                                prof2.display()
+                                print(prof2.description())
+                                prof2.display_margin_graph()
+                                vm.display(prof2)
                                 print("")
         
     return witnesses
 
 positive_involvement = Axiom(
     "Positive Involvement",
     has_violation = has_positive_involvement_violation,
@@ -755,28 +763,29 @@
                     if isinstance(prof,ProfileWithTies):
                         prof2 = ProfileWithTies(rankings, candidates = prof.candidates)
                         if prof.using_extended_strict_preference:
                             prof2.use_extended_strict_preference()
 
                     if winner not in vm(prof2):
                         if verbose:
+                            prof = prof.anonymize()
                             print(f"{winner} wins in the full profile, but {winner} is a loser after removing a voter with the ranking {str(r)}:")
                             print("")
                             print("Full profile")
                             prof.display()
                             print(prof.description())
                             prof.display_margin_graph()
                             vm.display(prof)
                             print("")
                             print("Profile with voter removed")
-                            anonprof2 = prof2.anonymize()
-                            anonprof2.display()
-                            print(anonprof2.description())
-                            anonprof2.display_margin_graph()
-                            vm.display(anonprof2)
+                            prof2 = prof2.anonymize()
+                            prof2.display()
+                            print(prof2.description())
+                            prof2.display_margin_graph()
+                            vm.display(prof2)
                             print("")
                         return True
                     
 def find_all_negative_involvement_violations(prof, vm, verbose=False, violation_type="Removal"):
     """
     If violation_type = "Removal", returns a list of pairs (winner,ranking) such that removing a voter with the given ranking causes the winner to lose, witnessing a violation of negative involvement.
     
@@ -807,28 +816,29 @@
                         prof2 = ProfileWithTies(rankings, candidates = prof.candidates)
                         if prof.using_extended_strict_preference:
                             prof2.use_extended_strict_preference()
 
                     if winner not in vm(prof2):
                         witnesses.append((winner, r))
                         if verbose:
+                            prof = prof.anonymize()
                             print(f"{winner} wins in the full profile, but {winner} is a loser after removing a voter with the ranking {str(r)}:")
                             print("")
                             print("Full profile")
                             prof.display()
                             print(prof.description())
                             prof.display_margin_graph()
                             vm.display(prof)
                             print("")
                             print("Profile with voter removed")
-                            anonprof2 = prof2.anonymize()
-                            anonprof2.display()
-                            print(anonprof2.description())
-                            anonprof2.display_margin_graph()
-                            vm.display(anonprof2)
+                            prof2 = prof2.anonymize()
+                            prof2.display()
+                            print(prof2.description())
+                            prof2.display_margin_graph()
+                            vm.display(prof2)
                             print("")
     return witnesses
 
 negative_involvement = Axiom(
     "Negative Involvement",
     has_violation = has_negative_involvement_violation,
     find_all_violations = find_all_negative_involvement_violations, 
@@ -872,28 +882,29 @@
                     rankings = prof.rankings
                     rankings.remove(r) # remove the first token of the type of ranking
                     
                     prof2 = Profile(rankings)
 
                     if loser in vm(prof2):
                         if verbose:
+                            prof = prof.anonymize()
                             print(f"{loser} loses in the full profile, but {loser} is a winner after removing a voter with the ranking {rl}:")
                             print("")
                             print("Full profile")
                             prof.display()
                             print(prof.description())
                             prof.display_margin_graph()
                             vm.display(prof)
                             print("")
                             print("Profile with voter removed")
-                            anonprof2 = prof2.anonymize()
-                            anonprof2.display()
-                            print(anonprof2.description())
-                            anonprof2.display_margin_graph()
-                            vm.display(anonprof2)
+                            prof2 = prof2.anonymize()
+                            prof2.display()
+                            print(prof2.description())
+                            prof2.display_margin_graph()
+                            vm.display(prof2)
                             print("")
                         return True
                     
 def find_all_tolerant_positive_involvement_violations(prof, vm, verbose=False, violation_type="Removal"):
     """
     If violation_type = "Removal", returns a list of pairs (loser,ranking) such that removing a voter with the given ranking causes the loser to win, witnessing a violation of tolerant positive involvement.
     
@@ -931,28 +942,29 @@
                     rankings.remove(r) # remove the first token of the type of ranking
                     
                     prof2 = Profile(rankings)
 
                     if loser in vm(prof2):
                         witnesses.append((loser, r))
                         if verbose:
+                            prof = prof.anonymize()
                             print(f"{loser} loses in the full profile, but {loser} is a winner after removing a voter with the ranking {str(r)}:")
                             print("")
                             print("Full profile")
                             prof.display()
                             print(prof.description())
                             prof.display_margin_graph()
                             vm.display(prof)
                             print("")
                             print("Profile with voter removed")
-                            anonprof2 = prof2.anonymize()
-                            anonprof2.display()
-                            print(anonprof2.description())
-                            anonprof2.display_margin_graph()
-                            vm.display(anonprof2)
+                            prof2 = prof2.anonymize()
+                            prof2.display()
+                            print(prof2.description())
+                            prof2.display_margin_graph()
+                            vm.display(prof2)
                             print("")
     return witnesses
                     
 tolerant_positive_involvement = Axiom(
     "Tolerant Positive Involvement",
     has_violation = has_tolerant_positive_involvement_violation,
     find_all_violations = find_all_tolerant_positive_involvement_violations, 
@@ -997,48 +1009,48 @@
         new_ws = vm(new_prof)
 
         if require_resoluteness == True and len(new_ws) > 1:
             continue
 
         if w not in new_ws:
             if verbose:
-
+                prof = prof.anonymize()
+                new_prof = new_prof.anonymize()
                 print(f"Violation of Bullet Vote Positive Involvement for {vm.name}")
                 print("Original profile:")
                 prof.display()
                 print(prof.description())
                 prof.display_margin_graph()
                 vm.display(prof)
-
                 print("New profile:")
                 new_prof.display()
                 print(new_prof.description())
                 new_prof.display_margin_graph()
                 vm.display(new_prof)
                 print("")
 
             return True
         
         if check_probabilities and len(new_ws) > len(ws):
 
             if verbose:
-                    
-                    print(f"Violation of Probabilistic Bullet Vote Positive Involvement for {vm.name}")
-                    print("Original profile:")
-                    prof.display()
-                    print(prof.description())
-                    prof.display_margin_graph()
-                    vm.display(prof)
-    
-                    print("New profile:")
-                    new_prof.display()
-                    print(new_prof.description())
-                    new_prof.display_margin_graph()
-                    vm.display(new_prof)
-                    print("")
+                prof = prof.anonymize()
+                new_prof = new_prof.anonymize()
+                print(f"Violation of Probabilistic Bullet Vote Positive Involvement for {vm.name}")
+                print("Original profile:")
+                prof.display()
+                print(prof.description())
+                prof.display_margin_graph()
+                vm.display(prof)
+                print("New profile:")
+                new_prof.display()
+                print(new_prof.description())
+                new_prof.display_margin_graph()
+                vm.display(new_prof)
+                print("")
 
             return True
         
     return False
 
 def find_all_bullet_vote_positive_involvement_violations(prof, vm, verbose=False, coalition_size = 1, require_resoluteness = False, require_uniquely_weighted = False, check_probabilities = False):
     """
@@ -1081,59 +1093,671 @@
         new_ws = vm(new_prof)
 
         if require_resoluteness == True and len(new_ws) > 1:
             continue
 
         if w not in new_ws:
             if verbose:
-                
+                prof = prof.anonymize()
+                new_prof = new_prof.anonymize()
                 print(f"Violation of Bullet Vote Positive Involvement for {vm.name}")
                 print("Original profile:")
                 prof.display()
                 print(prof.description())
                 prof.display_margin_graph()
                 vm.display(prof)
-
                 print("New profile:")
                 new_prof.display()
                 print(new_prof.description())
                 new_prof.display_margin_graph()
                 vm.display(new_prof)
                 print("")
 
             violations.append(w)
 
         if check_probabilities and len(new_ws) > len(ws):
                 
                 if verbose:
-                        
-                        print(f"Violation of Probabilistic Bullet Vote Positive Involvement for {vm.name}")
-                        print("Original profile:")
-                        prof.display()
-                        print(prof.description())
-                        prof.display_margin_graph()
-                        vm.display(prof)
-        
-                        print("New profile:")
-                        new_prof.display()
-                        print(new_prof.description())
-                        new_prof.display_margin_graph()
-                        vm.display(new_prof)
-                        print("")
+                    prof = prof.anonymize()
+                    new_prof = new_prof.anonymize()
+                    print(f"Violation of Probabilistic Bullet Vote Positive Involvement for {vm.name}")
+                    print("Original profile:")
+                    prof.display()
+                    print(prof.description())
+                    prof.display_margin_graph()
+                    vm.display(prof)
+                    print("New profile:")
+                    new_prof.display()
+                    print(new_prof.description())
+                    new_prof.display_margin_graph()
+                    vm.display(new_prof)
+                    print("")
     
                 violations.append(w)
         
     return violations
 
 bullet_vote_positive_involvement = Axiom(
     "Bullet Vote Positive Involvement",
     has_violation = has_bullet_vote_positive_involvement_violation,
     find_all_violations = find_all_bullet_vote_positive_involvement_violations, 
 )
 
+def has_participation_violation(prof, vm, verbose = False, violation_type = "Removal", coalition_size = 1, uniform_coalition = True, set_preference = "single-winner"):
+    """
+    If violation_type = "Removal", returns True if removing some voter(s) from prof changes the vm winning set such that the (each) voter prefers the new winner(s) to the original winner(s), according to the set_preference relation.
+
+    If violation_type = "Addition", returns True if adding some voter(s) from prof changes the vm winning set such that the (each) voter prefers the original winner(s) to the new winner(s), according to the set_preference relation.
+
+    If coalition_size > 1, checks for a violation involving a coalition of voters acting together.
+
+    If uniform_coalition = True, all voters in the coalition must have the same ranking.
+
+    If set_preference = "single-winner", a voter prefers a set A of candidates to a set B of candidates if A and B are singletons and the voter ranks the candidate in A above the candidate in B.
+
+    If set_preference = "weak-dominance", a voter prefers a set A to a set B if in their sincere ranking, all candidates in A are weakly above all candidates in B and some candidate in A is strictly above some candidate in B.
+
+    If set_preference = "optimist", a voter prefers a set A to a set B if in their sincere ranking, their favorite from A is above their favorite from B.
+
+    If set_preference = "pessimist", a voter prefers a set A to a set B if in their sincere ranking, their least favorite from A is above their least favorite from B.
+    
+    Args:
+        prof: a Profile or ProfileWithTies object.
+        vm (VotingMethod): A voting method to test.
+        verbose (bool, default=False): If a violation is found, display the violation.
+        violation_type: default is "Removal"
+        coalition_size: default is 1
+        uniform_coalition: default is True
+        set_preference: default is "single-winner". Other options are "weak-dominance", "optimist", and "pessimist".
+        
+    Returns:
+        Result of the test (bool): Returns True if there is a violation and False otherwise.
+
+    """
+    
+    winners = vm(prof)
+
+    if isinstance(prof,ProfileWithTies):
+        prof.use_extended_strict_preference()
+
+    found_manipulator = False
+
+    ranking_types = prof.ranking_types
+
+    ws = vm(prof)
+
+    if set_preference == "single-winner":
+        if len(ws) > 1:
+            return False
+        
+    if uniform_coalition:
+        
+        if violation_type == "Removal":
+
+            relevant_ranking_types = [r for r in prof.ranking_types if prof.rankings.count(r) >= coalition_size]
+
+            for r in relevant_ranking_types:
+                if not found_manipulator:
+
+                    ranking_tokens = [r for r in prof.rankings]
+
+                    for i in range(coalition_size):
+                        ranking_tokens.remove(r) # remove coalition_size-many tokens of the type of ranking
+
+                    if isinstance(prof,Profile):
+
+                        new_prof = Profile(ranking_tokens)
+                        new_ws = vm(new_prof)
+
+                        old_winner_to_compare = None
+                        new_winner_to_compare = None
+
+                        if set_preference == "single-winner" and len(new_ws) == 1:
+
+                            old_winner_to_compare = ws[0]
+                            new_winner_to_compare = new_ws[0] 
+                        
+                        elif set_preference == "weak-dominance":
+                            r_as_ranking = Ranking({c: i for i, c in enumerate(r)})
+                        
+                        elif set_preference == "optimist":
+                                
+                            old_winner_to_compare = [cand for cand in r if cand in ws][0]
+                            new_winner_to_compare = [cand for cand in r if cand in new_ws][0]
+
+                        elif set_preference == "pessimist":
+                            
+                            old_winner_to_compare = [cand for cand in r if cand in ws][-1] 
+                            new_winner_to_compare = [cand for cand in r if cand in new_ws][-1]
+
+                        if old_winner_to_compare is not None and r.index(old_winner_to_compare) > r.index(new_winner_to_compare) or (set_preference == "weak-dominance" and r_as_ranking.weak_dom(new_ws,ws)):
+                            
+                            found_manipulator = True
+
+                            if verbose:
+                                prof = prof.anonymize()
+                                new_prof = new_prof.anonymize()
+                                print(f"Violation of Participation for {vm.name} under the {set_preference} set preference.")
+                                if coalition_size == 1:
+                                    print(f"A voter with the ranking {r} can benefit by abstaining.")
+                                else:
+                                    print(f"{coalition_size} voters with the ranking {r} can benefit by jointly abstaining.")
+                                print("")
+                                print("Original Profile:")
+                                prof.display()
+                                print(prof.description())
+                                print("")
+                                vm.display(prof)
+                                prof.display_margin_graph()
+                                print("")
+                                if coalition_size == 1:
+                                    print("Profile if the voter abstains:")
+                                else:
+                                    print("Profile if the voters abstain:")
+                                new_prof.display()
+                                print(new_prof.description())
+                                print("")
+                                vm.display(new_prof)
+                                new_prof.display_margin_graph()
+
+                    if isinstance(prof,ProfileWithTies):
+                        r_dict = r.rmap
+
+                        new_prof = ProfileWithTies(ranking_tokens, candidates = prof.candidates)
+                        new_prof.use_extended_strict_preference()
+                        new_ws = vm(new_prof)
+
+                        ranked_old_winners = [c for c in ws if c in r_dict.keys()]
+                        ranked_new_winners = [c for c in new_ws if c in r_dict.keys()]
+
+                        rank_of_old_winner_to_compare = None
+                        rank_of_new_winner_to_compare = None
+
+                        if set_preference == "single-winner" and len(new_ws) == 1:
+
+                            rank_of_old_winner_to_compare = r_dict[ws[0]] if ranked_old_winners else math.inf
+                            rank_of_new_winner_to_compare = r_dict[new_ws[0]] if ranked_new_winners else math.inf
+                        
+                        elif set_preference == "optimist":
+
+                            rank_of_old_winner_to_compare = min([r_dict[c] for c in ranked_old_winners]) if ranked_old_winners else math.inf
+                            rank_of_new_winner_to_compare = min([r_dict[c] for c in ranked_new_winners]) if ranked_new_winners else math.inf
+
+                        elif set_preference == "pessimist":
+
+                            rank_of_old_winner_to_compare = max([r_dict[c] for c in ranked_old_winners]) if ranked_old_winners == ws else math.inf
+                            rank_of_new_winner_to_compare = max([r_dict[c] for c in ranked_new_winners]) if ranked_new_winners == new_ws else math.inf
+
+                        if rank_of_old_winner_to_compare is not None and rank_of_old_winner_to_compare > rank_of_new_winner_to_compare or (set_preference == "weak-dominance" and r.weak_dom(new_ws,ws,use_extended_preferences=True)):
+                            
+                            found_manipulator = True
+
+                            if verbose:
+                                prof = prof.anonymize()
+                                new_prof = new_prof.anonymize()
+                                print(f"Violation of Participation for {vm.name} under the {set_preference} set preference.")
+                                if coalition_size == 1:
+                                    print(f"A voter with the ranking {r} can benefit by abstaining.")
+                                else:
+                                    print(f"{coalition_size} voters with the ranking {r} can benefit by jointly abstaining.")
+                                print("")
+                                print("Original Profile:")
+                                prof.display()
+                                print(prof.description())
+                                print("")
+                                vm.display(prof)
+                                prof.display_margin_graph()
+                                print("")
+                                if coalition_size == 1:
+                                    print("Profile if the voter abstains:")
+                                else:
+                                    print("Profile if the voters abstain:")
+                                new_prof.display()
+                                print(new_prof.description())
+                                print("")
+                                vm.display(new_prof)
+                                new_prof.display_margin_graph()
+
+        if violation_type == "Addition":
+
+            if isinstance(prof,Profile):
+
+                for new_r in permutations(prof.candidates):
+                    if not found_manipulator:
+
+                        new_ranking_tokens = [r for r in prof.rankings]
+
+                        for i in range(coalition_size):
+                            new_ranking_tokens.append(new_r)
+
+                        new_prof = Profile(new_ranking_tokens)
+                        new_ws = vm(new_prof)
+
+                        old_winner_to_compare = None
+                        new_winner_to_compare = None
+
+                        if set_preference == "single-winner" and len(new_ws) == 1:
+
+                            old_winner_to_compare = ws[0]
+                            new_winner_to_compare = new_ws[0] 
+                        
+                        elif set_preference == "weak-dominance":
+                            new_r_as_ranking = Ranking({c: i for i, c in enumerate(new_r)})
+                        
+                        elif set_preference == "optimist":
+                                
+                            old_winner_to_compare = [cand for cand in r if cand in ws][0]
+                            new_winner_to_compare = [cand for cand in r if cand in new_ws][0]
+
+                        elif set_preference == "pessimist":
+                            
+                            old_winner_to_compare = [cand for cand in r if cand in ws][-1] 
+                            new_winner_to_compare = [cand for cand in r if cand in new_ws][-1]
+
+                        if old_winner_to_compare is not None and new_r.index(old_winner_to_compare) < new_r.index(new_winner_to_compare) or (set_preference == "weak-dominance" and new_r_as_ranking.weak_dom(ws,new_ws)):
+                            
+                            found_manipulator = True
+
+                            if verbose:
+                                prof = prof.anonymize()
+                                new_prof = new_prof.anonymize()
+                                print(f"Violation of Participation for {vm.name} under the {set_preference} set preference.")
+                                if coalition_size == 1:
+                                    print(f"A new voter who joins with the ranking {new_r} will wish they had abstained.")
+                                else:
+                                    print(f"{coalition_size} new voters who join with the ranking {new_r} will wish they had jointly abstained.")
+                                print("")
+                                print("Original Profile without voter(s):")
+                                prof.display()
+                                print(prof.description())
+                                print("")
+                                vm.display(prof)
+                                prof.display_margin_graph()
+                                print("")
+                                print("New Profile with voter(s) added:")
+                                new_prof.display()
+                                print(new_prof.description())
+                                print("")
+                                vm.display(new_prof)
+                                new_prof.display_margin_graph()
+
+            if isinstance(prof,ProfileWithTies):
+
+                for _new_r in weak_orders(prof.candidates):
+                    new_r = Ranking(_new_r)
+                    new_r_dict = new_r.rmap
+
+                    if not found_manipulator:
+
+                        new_ranking_tokens = [r for r in prof.rankings] 
+
+                        for i in range(coalition_size):
+                            new_ranking_tokens.append(new_r)
+
+                        new_prof = ProfileWithTies(new_ranking_tokens, candidates = prof.candidates)
+                        new_prof.use_extended_strict_preference()
+                        new_ws = vm(new_prof)
+
+                        ranked_old_winners = [c for c in ws if c in new_r_dict.keys()]
+                        ranked_new_winners = [c for c in new_ws if c in new_r_dict.keys()]
+
+                        rank_of_old_winner_to_compare = None
+                        rank_of_new_winner_to_compare = None
+
+                        if set_preference == "single-winner" and len(new_ws) == 1:
+
+                            rank_of_old_winner_to_compare = new_r_dict[ws[0]] if ranked_old_winners else math.inf
+                            rank_of_new_winner_to_compare = new_r_dict[new_ws[0]] if ranked_new_winners else math.inf
+                        
+                        elif set_preference == "optimist":
+
+                            rank_of_old_winner_to_compare = min([new_r_dict[c] for c in ranked_old_winners]) if ranked_old_winners else math.inf
+                            rank_of_new_winner_to_compare = min([new_r_dict[c] for c in ranked_new_winners]) if ranked_new_winners else math.inf
+
+                        elif set_preference == "pessimist":
+
+                            rank_of_old_winner_to_compare = max([new_r_dict[c] for c in ranked_old_winners]) if ranked_old_winners == ws else math.inf
+                            rank_of_new_winner_to_compare = max([new_r_dict[c] for c in ranked_new_winners]) if ranked_new_winners == new_ws else math.inf
+
+                        if rank_of_old_winner_to_compare is not None and rank_of_old_winner_to_compare < rank_of_new_winner_to_compare or (set_preference == "weak-dominance" and r.weak_dom(ws,new_ws,use_extended_preferences=True)):
+                            
+                            found_manipulator = True
+
+                            if verbose:
+                                prof = prof.anonymize()
+                                new_prof = new_prof.anonymize()
+                                print(f"Violation of Participation for {vm.name} under the {set_preference} set preference.")
+                                if coalition_size == 1:
+                                    print(f"A new voter who joins with the ranking {new_r} will wish they had abstained.")
+                                else:
+                                    print(f"{coalition_size} new voters who join with the ranking {new_r} will wish they had jointly abstained.")
+                                print("")
+                                print("Original Profile without voter(s):")
+                                prof.display()
+                                print(prof.description())
+                                print("")
+                                vm.display(prof)
+                                prof.display_margin_graph()
+                                print("")
+                                print("New Profile with voter(s) added:")
+                                new_prof.display()
+                                print(new_prof.description())
+                                print("")
+                                vm.display(new_prof)
+                                new_prof.display_margin_graph()
+            
+    return found_manipulator
+
+def find_all_participation_violations(prof, vm, verbose = False, violation_type = "Removal", coalition_size = 1, uniform_coalition = True, set_preference = "single-winner"):
+    """
+    Returns a list of tuples (preferred_winners, dispreferred_winners, ranking) witnessing violations of participation.
+
+    If violation_type = "Removal", returns a list of tuples (preferred_winners, dispreferred_winners, ranking) such that removing coalition_size-many voters with the given ranking changes the winning set from the preferred_winners to the dispreferred_winners, according to the set_preference relation.
+
+    If violation_type = "Addition", returns a list of tuples (preferred_winners, dispreferred_winners, ranking) such that adding coalition_size-many voters with the given ranking changes the winning set from the preferred_winners to the dispreferred_winners, according to the set_preference relation.
+
+    If coalition_size > 1, checks for a violation involving a coalition of voters acting together.
+
+    If uniform_coalition = True, all voters in the coalition must have the same ranking.
+
+    If set_preference = "single-winner", a voter prefers a set A of candidates to a set B of candidates if A and B are singletons and the voter ranks the candidate in A above the candidate in B.
+
+    If set_preference = "weak-dominance", a voter prefers a set A to a set B if in their sincere ranking, all candidates in A are weakly above all candidates in B and some candidate in A is strictly above some candidate in B.
+
+    If set_preference = "optimist", a voter prefers a set A to a set B if in their sincere ranking, their favorite from A is above their favorite from B.
+
+    If set_preference = "pessimist", a voter prefers a set A to a set B if in their sincere ranking, their least favorite from A is above their least favorite from B.
+
+    Args:
+        prof: a Profile or ProfileWithTies object.
+        vm (VotingMethod): A voting method to test.
+        verbose (bool, default=False): If a violation is found, display the violation.
+        violation_type: default is "Removal"
+        coalition_size: default is 1
+        uniform_coalition: default is True
+        set_preference: default is "single-winner". Other options are "weak-dominance", "optimist", and "pessimist".
+
+    Returns:
+        A List of tuples (preferred_winners, dispreferred_winners, ranking) witnessing violations of participation.
+    """
+
+    violations = list()
+
+    winners = vm(prof)
+
+    if isinstance(prof,ProfileWithTies):
+        prof.use_extended_strict_preference()
+
+    ranking_types = prof.ranking_types
+
+    ws = vm(prof)
+
+    if set_preference == "single-winner":
+        if len(ws) > 1:
+            return False
+        
+    if uniform_coalition:
+        
+        if violation_type == "Removal":
+
+            relevant_ranking_types = [r for r in prof.ranking_types if prof.rankings.count(r) >= coalition_size]
+
+            for r in relevant_ranking_types:
+                ranking_tokens = [r for r in prof.rankings]
+
+                for i in range(coalition_size):
+                    ranking_tokens.remove(r) # remove coalition_size-many tokens of the type of ranking
+
+                if isinstance(prof,Profile):
+
+                    new_prof = Profile(ranking_tokens)
+                    new_ws = vm(new_prof)
+
+                    old_winner_to_compare = None
+                    new_winner_to_compare = None
+
+                    if set_preference == "single-winner" and len(new_ws) == 1:
+
+                        old_winner_to_compare = ws[0]
+                        new_winner_to_compare = new_ws[0] 
+                    
+                    elif set_preference == "weak-dominance":
+                        r_as_ranking = Ranking({c: i for i, c in enumerate(r)})
+                    
+                    elif set_preference == "optimist":
+                            
+                        old_winner_to_compare = [cand for cand in r if cand in ws][0]
+                        new_winner_to_compare = [cand for cand in r if cand in new_ws][0]
+
+                    elif set_preference == "pessimist":
+                        
+                        old_winner_to_compare = [cand for cand in r if cand in ws][-1] 
+                        new_winner_to_compare = [cand for cand in r if cand in new_ws][-1]
+
+                    if old_winner_to_compare is not None and r.index(old_winner_to_compare) > r.index(new_winner_to_compare) or (set_preference == "weak-dominance" and r_as_ranking.weak_dom(new_ws,ws)):
+                        
+                        violations.append((ws, new_ws, r))
+
+                        if verbose:
+                            prof = prof.anonymize()
+                            new_prof = new_prof.anonymize()
+                            print(f"Violation of Participation for {vm.name} under the {set_preference} set preference.")
+                            if coalition_size == 1:
+                                print(f"A voter with the ranking {r} can benefit by abstaining.")
+                            else:
+                                print(f"{coalition_size} voters with the ranking {r} can benefit by jointly abstaining.")
+                            print("")
+                            print("Original Profile:")
+                            prof.display()
+                            print(prof.description())
+                            print("")
+                            vm.display(prof)
+                            prof.display_margin_graph()
+                            print("")
+                            if coalition_size == 1:
+                                print("Profile if the voter abstains:")
+
+                            else:
+                                print("Profile if the voters abstain:")
+                            new_prof.display()
+                            print(new_prof.description())
+                            print("")
+                            vm.display(new_prof)
+                            new_prof.display_margin_graph()
+
+                if isinstance(prof,ProfileWithTies):
+                    r_dict = r.rmap
+
+                    new_prof = ProfileWithTies(ranking_tokens, candidates = prof.candidates)
+                    new_prof.use_extended_strict_preference()
+                    new_ws = vm(new_prof)
+
+                    ranked_old_winners = [c for c in ws if c in r_dict.keys()]
+                    ranked_new_winners = [c for c in new_ws if c in r_dict.keys()]
+
+                    rank_of_old_winner_to_compare = None
+                    rank_of_new_winner_to_compare = None
+
+                    if set_preference == "single-winner" and len(new_ws) == 1:
+
+                        rank_of_old_winner_to_compare = r_dict[ws[0]] if ranked_old_winners else math.inf
+                        rank_of_new_winner_to_compare = r_dict[new_ws[0]] if ranked_new_winners else math.inf
+                    
+                    elif set_preference == "optimist":
+
+                        rank_of_old_winner_to_compare = min([r_dict[c] for c in ranked_old_winners]) if ranked_old_winners else math.inf
+                        rank_of_new_winner_to_compare = min([r_dict[c] for c in ranked_new_winners]) if ranked_new_winners else math.inf
+
+                    elif set_preference == "pessimist":
+
+                        rank_of_old_winner_to_compare = max([r_dict[c] for c in ranked_old_winners]) if ranked_old_winners == ws else math.inf
+                        rank_of_new_winner_to_compare = max([r_dict[c] for c in ranked_new_winners]) if ranked_new_winners == new_ws else math.inf
+
+                    if rank_of_old_winner_to_compare is not None and rank_of_old_winner_to_compare > rank_of_new_winner_to_compare or (set_preference == "weak-dominance" and r.weak_dom(new_ws,ws,use_extended_preferences=True)):
+                        
+                        violations.append((ws, new_ws, r_dict))
+
+                        if verbose:
+                            prof = prof.anonymize()
+                            new_prof = new_prof.anonymize()
+                            print(f"Violation of Participation for {vm.name} under the {set_preference} set preference.")
+                            if coalition_size == 1:
+                                print(f"A voter with the ranking {r} can benefit by abstaining.")
+                            else:
+                                print(f"{coalition_size} voters with the ranking {r} can benefit by jointly abstaining.")
+                            print("")
+                            print("Original Profile:")
+                            prof.display()
+                            print(prof.description())
+                            print("")
+                            vm.display(prof)
+                            prof.display_margin_graph()
+                            print("")
+                            if coalition_size == 1:
+                                print("Profile if the voter abstains:")
+                            else:
+                                print("Profile if the voters abstain:")
+                            new_prof.display()
+                            print(new_prof.description())
+                            print("")
+                            vm.display(new_prof)
+                            new_prof
+
+        if violation_type == "Addition":
+
+            if isinstance(prof,Profile):
+
+                for new_r in permutations(prof.candidates):
+                    new_ranking_tokens = [r for r in prof.rankings]
+
+                    for i in range(coalition_size):
+                        new_ranking_tokens.append(new_r)
+
+                    new_prof = Profile(new_ranking_tokens)
+                    new_ws = vm(new_prof)
+
+                    old_winner_to_compare = None
+                    new_winner_to_compare = None
+
+                    if set_preference == "single-winner" and len(new_ws) == 1:
+
+                        old_winner_to_compare = ws[0]
+                        new_winner_to_compare = new_ws[0] 
+                    
+                    elif set_preference == "weak-dominance":
+                        new_r_as_ranking = Ranking({c: i for i, c in enumerate(new_r)})
+                    
+                    elif set_preference == "optimist":
+                            
+                        old_winner_to_compare = [cand for cand in r if cand in ws][0]
+                        new_winner_to_compare = [cand for cand in r if cand in new_ws][0]
+
+                    elif set_preference == "pessimist":
+                        
+                        old_winner_to_compare = [cand for cand in r if cand in ws][-1] 
+                        new_winner_to_compare = [cand for cand in r if cand in new_ws][-1]
+
+                    if old_winner_to_compare is not None and new_r.index(old_winner_to_compare) < new_r.index(new_winner_to_compare) or (set_preference == "weak-dominance" and new_r_as_ranking.weak_dom(ws,new_ws)):
+                        
+                        violations.append((ws, new_ws, new_r))
+
+                        if verbose:
+                            prof = prof.anonymize()
+                            new_prof = new_prof.anonymize()
+                            print(f"Violation of Participation for {vm.name} under the {set_preference} set preference.")
+                            if coalition_size == 1:
+                                print(f"A new voter who joins with the ranking {new_r} will wish they had abstained.")
+                            else:
+                                print(f"{coalition_size} new voters who join with the ranking {new_r} will wish they had jointly abstained.")
+                            print("")
+                            print("Original Profile without voter(s):")
+                            prof.display()
+                            print(prof.description())
+                            print("")
+                            vm.display(prof)
+                            prof.display_margin_graph()
+                            print("")
+                            print("New Profile with voter(s) added:")
+                            new_prof.display()
+                            print(new_prof.description())
+                            print("")
+                            vm.display(new_prof)
+                            new_prof.display_margin_graph()
+
+            if isinstance(prof,ProfileWithTies):
+                
+                    for _new_r in weak_orders(prof.candidates):
+                        new_r = Ranking(_new_r)
+                        new_r_dict = new_r.rmap
+    
+                        new_ranking_tokens = [r for r in prof.rankings] 
+    
+                        for i in range(coalition_size):
+                            new_ranking_tokens.append(new_r)
+    
+                        new_prof = ProfileWithTies(new_ranking_tokens, candidates = prof.candidates)
+                        new_prof.use_extended_strict_preference()
+                        new_ws = vm(new_prof)
+    
+                        ranked_old_winners = [c for c in ws if c in new_r_dict.keys()]
+                        ranked_new_winners = [c for c in new_ws if c in new_r_dict.keys()]
+    
+                        rank_of_old_winner_to_compare = None
+                        rank_of_new_winner_to_compare = None
+    
+                        if set_preference == "single-winner" and len(new_ws) == 1:
+    
+                            rank_of_old_winner_to_compare = new_r_dict[ws[0]] if ranked_old_winners else math.inf
+                            rank_of_new_winner_to_compare = new_r_dict[new_ws[0]] if ranked_new_winners else math.inf
+                        
+                        elif set_preference == "optimist":
+    
+                            rank_of_old_winner_to_compare = min([new_r_dict[c] for c in ranked_old_winners]) if ranked_old_winners else math.inf
+                            rank_of_new_winner_to_compare = min([new_r_dict[c] for c in ranked_new_winners]) if ranked_new_winners else math.inf
+    
+                        elif set_preference == "pessimist":
+    
+                            rank_of_old_winner_to_compare = max([new_r_dict[c] for c in ranked_old_winners]) if ranked_old_winners == ws else math.inf
+                            rank_of_new_winner_to_compare = max([new_r_dict[c] for c in ranked_new_winners]) if ranked_new_winners == new_ws else math.inf
+    
+                        if rank_of_old_winner_to_compare is not None and rank_of_old_winner_to_compare < rank_of_new_winner_to_compare or (set_preference == "weak-dominance" and r.weak_dom(ws,new_ws,use_extended_preferences=True)):
+                            
+                            violations.append((ws, new_ws, new_r_dict))
+    
+                            if verbose:
+                                prof = prof.anonymize()
+                                new_prof = new_prof.anonymize()
+                                print(f"Violation of Participation for {vm.name} under the {set_preference} set preference.")
+                                if coalition_size == 1:
+                                    print(f"A new voter who joins with the ranking {new_r} will wish they had abstained.")
+                                else:
+                                    print(f"{coalition_size} new voters who join with the ranking {new_r} will wish they had jointly abstained.")
+                                print("")
+                                print(" Original Profile without voter(s):")
+                                prof.display()
+                                print(prof.description())
+                                print("")
+                                vm.display(prof)
+                                prof.display_margin_graph()
+                                print("")
+                                print("New Profile with voter(s) added:")
+                                new_prof.display()
+                                print(new_prof.description())
+                                print("")
+                                vm.display(new_prof)
+                                new_prof.display_margin_graph()
+
+    return violations
+
+participation = Axiom(
+    "Participation",
+    has_violation = has_participation_violation,
+    find_all_violations = find_all_participation_violations, 
+)
+
 def has_single_voter_resolvability_violation(prof, vm, verbose=False):
     """
     If prof is a Profile, returns True if there are multiple vm winners in prof and for one such winner A, there is no linear ballot that can be added to prof to make A the unique winner.
 
     If prof is a ProfileWithTies, returns True if there are multiple vm winners in prof and for one such winner A, there is no Ranking (allowing ties) that can be added to prof to make A the unique winner. 
 
     Args:
@@ -1170,14 +1794,15 @@
                     if vm(new_prof) == [winner]:
                         found_voter_to_add = True
                         break
         
             if not found_voter_to_add:
 
                 if verbose:
+                    prof = prof.anonymize()
                     if isinstance(prof,Profile):
                         print(f"Violation of Single-Voter Resolvability for {vm.name}: cannot make {winner} the unique winner by adding a linear ballot.")
                     if isinstance(prof,ProfileWithTies):
                         print(f"Violation of Single-Voter Resolvability for {vm.name}: cannot make {winner} the unique winner by adding a Ranking.")
                     print("")
                     print("Profile:")
                     prof.display()
@@ -1233,14 +1858,15 @@
                     if vm(new_prof) == [winner]:
                         found_voter_to_add = True
                         break
         
             if not found_voter_to_add:
 
                 if verbose:
+                    prof = prof.anonymize()
                     if isinstance(prof,Profile):
                         print(f"Violation of Single-Voter Resolvability for {vm.name}: cannot make {winner} the unique winner by adding a linear ballot.")
                     if isinstance(prof,ProfileWithTies):
                         print(f"Violation of Single-Voter Resolvability for {vm.name}: cannot make {winner} the unique winner by adding a Ranking.")
                     print("")
                     print("Profile:")
                     prof.display()
@@ -1262,9 +1888,10 @@
 
 variable_voter_axioms = [
     reinforcement,
     positive_involvement,
     negative_involvement,
     tolerant_positive_involvement,
     bullet_vote_positive_involvement,
+    participation,
     single_voter_resolvability,
 ]
```

### Comparing `pref_voting-1.0.0/pref_voting/voting_method.py` & `pref_voting-1.1.0/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pref_voting/weighted_majority_graphs.py` & `pref_voting-1.1.0/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.0.0/pyproject.toml` & `pref_voting-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "1.0.0"
+version = "1.1.0"
 description = "pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-1.0.0/setup.py` & `pref_voting-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'prefsampling>=0.1.16,<0.2.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': 'pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.',
     'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n\n## Documentation\n\nOnline documentation is available at [https://pref-voting.readthedocs.io](https://pref-voting.readthedocs.io).\n\n## Example Usage\n\nA profile (of linear orders over the candidates) is created by initializing a `Profile` class object.  Simply provide a list of rankings (each ranking is a tuple of numbers) and a list giving the number of voters with each ranking:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [\n    (0, 1, 2, 3), \n    (2, 3, 1, 0), \n    (3, 1, 2, 0), \n    (1, 2, 0, 3), \n    (1, 3, 2, 0)]\n\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function `generate_profile` is used to generate a profile for a given number of candidates and voters:  \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\nTo use one of the many voting methods, import the function from `pref_voting.voting_methods` and apply it to the profile: \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\nfrom pref_voting.voting_methods import *\n\nprof = generate_profile(3, 4)\nsplit_cycle(prof) # returns the sorted list of winning candidates\nsplit_cycle.display(prof) # display the winning candidates\n\n```\n\n## Questions?\n\nFeel free to [send an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
```

### Comparing `pref_voting-1.0.0/PKG-INFO` & `pref_voting-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 1.0.0
+Version: 1.1.0
 Summary: pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

