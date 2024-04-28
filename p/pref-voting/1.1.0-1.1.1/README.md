# Comparing `tmp/pref_voting-1.1.0.tar.gz` & `tmp/pref_voting-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-1.1.0.tar", max compression
+gzip compressed data, was "pref_voting-1.1.1.tar", max compression
```

## Comparing `pref_voting-1.1.0.tar` & `pref_voting-1.1.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.1.0/LICENSE
--rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.1.0/README.md
--rw-r--r--   0        0        0       22 2024-04-28 12:21:46.031009 pref_voting-1.1.0/pref_voting/__init__.py
--rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-1.1.0/pref_voting/analysis.py
--rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.1.0/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.1.0/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.1.0/pref_voting/axioms.py
--rw-r--r--   0        0        0    33205 2024-04-09 01:59:48.226095 pref_voting-1.1.0/pref_voting/c1_methods.py
--rw-r--r--   0        0        0    15161 2024-03-15 20:53:44.539281 pref_voting-1.1.0/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    12659 2023-12-07 15:15:32.783919 pref_voting-1.1.0/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.1.0/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.1.0/pref_voting/generate_spatial_profiles.py
--rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.1.0/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-1.1.0/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.1.0/pref_voting/grade_methods.py
--rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.1.0/pref_voting/grade_profiles.py
--rw-r--r--   0        0        0     8068 2024-04-19 01:31:48.812126 pref_voting-1.1.0/pref_voting/helper.py
--rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.1.0/pref_voting/invariance_axioms.py
--rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.1.0/pref_voting/io/__init__.py
--rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.1.0/pref_voting/io/readers.py
--rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.1.0/pref_voting/io/writers.py
--rw-r--r--   0        0        0    90549 2024-04-15 01:51:51.467855 pref_voting-1.1.0/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.1.0/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-1.1.0/pref_voting/mappings.py
--rw-r--r--   0        0        0    73036 2024-04-27 22:46:59.878102 pref_voting-1.1.0/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    70814 2024-04-27 22:10:28.624211 pref_voting-1.1.0/pref_voting/margin_based_methods_old.py
--rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.1.0/pref_voting/monotonicity_axioms.py
--rw-r--r--   0        0        0    24548 2024-03-16 15:19:40.029463 pref_voting-1.1.0/pref_voting/other_methods.py
--rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.1.0/pref_voting/prob_voting_method.py
--rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.1.0/pref_voting/probabilistic_methods.py
--rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-1.1.0/pref_voting/profiles.py
--rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.1.0/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.1.0/pref_voting/rankings.py
--rw-r--r--   0        0        0    21026 2024-04-09 02:00:24.744126 pref_voting-1.1.0/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.1.0/pref_voting/social_welfare_function.py
--rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.1.0/pref_voting/social_welfare_functions.py
--rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.1.0/pref_voting/spatial_profiles.py
--rw-r--r--   0        0        0    15790 2024-04-24 21:18:21.291486 pref_voting-1.1.0/pref_voting/strategic_axioms.py
--rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.1.0/pref_voting/tests/__init__.py
--rw-r--r--   0        0        0      666 2024-03-02 21:50:31.231806 pref_voting-1.1.0/pref_voting/tests/conftest.py
--rw-r--r--   0        0        0     5062 2024-03-19 01:38:04.296201 pref_voting-1.1.0/pref_voting/tests/test_c1_methods.py
--rw-r--r--   0        0        0     2576 2024-03-19 00:18:02.163482 pref_voting-1.1.0/pref_voting/tests/test_combined_methods.py
--rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.1.0/pref_voting/tests/test_generate_profiles.py
--rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.1.0/pref_voting/tests/test_generate_spatial_profile.py
--rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.1.0/pref_voting/tests/test_io.py
--rw-r--r--   0        0        0     8943 2024-03-17 11:39:53.682951 pref_voting-1.1.0/pref_voting/tests/test_iterative_methods.py
--rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.1.0/pref_voting/tests/test_majority_graph.py
--rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.1.0/pref_voting/tests/test_mapping.py
--rw-r--r--   0        0        0    10335 2024-04-28 12:01:51.077156 pref_voting-1.1.0/pref_voting/tests/test_margin_based_methods.py
--rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.1.0/pref_voting/tests/test_margin_graph.py
--rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.1.0/pref_voting/tests/test_other_methods.py
--rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.1.0/pref_voting/tests/test_prob_voting_method.py
--rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.1.0/pref_voting/tests/test_profile.py
--rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.1.0/pref_voting/tests/test_profile_with_ties.py
--rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.1.0/pref_voting/tests/test_ranking.py
--rw-r--r--   0        0        0     5543 2024-03-19 11:54:18.932325 pref_voting-1.1.0/pref_voting/tests/test_scoring_rules.py
--rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.1.0/pref_voting/tests/test_social_welfare_functions.py
--rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.1.0/pref_voting/tests/test_spatial_profile.py
--rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.1.0/pref_voting/tests/test_support_graph.py
--rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.1.0/pref_voting/tests/test_utility_function.py
--rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.1.0/pref_voting/tests/test_utility_functions.py
--rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.1.0/pref_voting/tests/test_voting_method.py
--rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.1.0/pref_voting/utility_functions.py
--rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.1.0/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-1.1.0/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.1.0/pref_voting/variable_candidate_axioms.py
--rw-r--r--   0        0        0    91053 2024-04-27 11:07:33.697481 pref_voting-1.1.0/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     5566 2023-12-07 15:03:17.438046 pref_voting-1.1.0/pref_voting/voting_method.py
--rw-r--r--   0        0        0      372 2023-11-14 00:06:58.907333 pref_voting-1.1.0/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.1.0/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      760 2024-04-28 12:21:46.030090 pref_voting-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-1.1.0/setup.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.1.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-28 12:44:16.209666 pref_voting-1.1.1/pref_voting/__init__.py
+-rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-1.1.1/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.1.1/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.1.1/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.1.1/pref_voting/axioms.py
+-rw-r--r--   0        0        0    33205 2024-04-09 01:59:48.226095 pref_voting-1.1.1/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0    15161 2024-03-15 20:53:44.539281 pref_voting-1.1.1/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    12659 2023-12-07 15:15:32.783919 pref_voting-1.1.1/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.1.1/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.1.1/pref_voting/generate_spatial_profiles.py
+-rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.1.1/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-1.1.1/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.1.1/pref_voting/grade_methods.py
+-rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.1.1/pref_voting/grade_profiles.py
+-rw-r--r--   0        0        0     8068 2024-04-19 01:31:48.812126 pref_voting-1.1.1/pref_voting/helper.py
+-rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.1.1/pref_voting/invariance_axioms.py
+-rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.1.1/pref_voting/io/__init__.py
+-rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.1.1/pref_voting/io/readers.py
+-rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.1.1/pref_voting/io/writers.py
+-rw-r--r--   0        0        0    90549 2024-04-15 01:51:51.467855 pref_voting-1.1.1/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.1.1/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-1.1.1/pref_voting/mappings.py
+-rw-r--r--   0        0        0    72109 2024-04-28 12:38:37.443651 pref_voting-1.1.1/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    70814 2024-04-27 22:10:28.624211 pref_voting-1.1.1/pref_voting/margin_based_methods_old.py
+-rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.1.1/pref_voting/monotonicity_axioms.py
+-rw-r--r--   0        0        0    24548 2024-03-16 15:19:40.029463 pref_voting-1.1.1/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.1.1/pref_voting/prob_voting_method.py
+-rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.1.1/pref_voting/probabilistic_methods.py
+-rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-1.1.1/pref_voting/profiles.py
+-rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.1.1/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.1.1/pref_voting/rankings.py
+-rw-r--r--   0        0        0    21026 2024-04-09 02:00:24.744126 pref_voting-1.1.1/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.1.1/pref_voting/social_welfare_function.py
+-rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.1.1/pref_voting/social_welfare_functions.py
+-rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.1.1/pref_voting/spatial_profiles.py
+-rw-r--r--   0        0        0    15790 2024-04-24 21:18:21.291486 pref_voting-1.1.1/pref_voting/strategic_axioms.py
+-rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.1.1/pref_voting/tests/__init__.py
+-rw-r--r--   0        0        0      666 2024-03-02 21:50:31.231806 pref_voting-1.1.1/pref_voting/tests/conftest.py
+-rw-r--r--   0        0        0     5062 2024-03-19 01:38:04.296201 pref_voting-1.1.1/pref_voting/tests/test_c1_methods.py
+-rw-r--r--   0        0        0     2576 2024-03-19 00:18:02.163482 pref_voting-1.1.1/pref_voting/tests/test_combined_methods.py
+-rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.1.1/pref_voting/tests/test_generate_profiles.py
+-rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.1.1/pref_voting/tests/test_generate_spatial_profile.py
+-rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.1.1/pref_voting/tests/test_io.py
+-rw-r--r--   0        0        0     8943 2024-03-17 11:39:53.682951 pref_voting-1.1.1/pref_voting/tests/test_iterative_methods.py
+-rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.1.1/pref_voting/tests/test_majority_graph.py
+-rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.1.1/pref_voting/tests/test_mapping.py
+-rw-r--r--   0        0        0    10335 2024-04-28 12:01:51.077156 pref_voting-1.1.1/pref_voting/tests/test_margin_based_methods.py
+-rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.1.1/pref_voting/tests/test_margin_graph.py
+-rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.1.1/pref_voting/tests/test_other_methods.py
+-rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.1.1/pref_voting/tests/test_prob_voting_method.py
+-rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.1.1/pref_voting/tests/test_profile.py
+-rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.1.1/pref_voting/tests/test_profile_with_ties.py
+-rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.1.1/pref_voting/tests/test_ranking.py
+-rw-r--r--   0        0        0     5543 2024-03-19 11:54:18.932325 pref_voting-1.1.1/pref_voting/tests/test_scoring_rules.py
+-rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.1.1/pref_voting/tests/test_social_welfare_functions.py
+-rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.1.1/pref_voting/tests/test_spatial_profile.py
+-rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.1.1/pref_voting/tests/test_support_graph.py
+-rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.1.1/pref_voting/tests/test_utility_function.py
+-rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.1.1/pref_voting/tests/test_utility_functions.py
+-rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.1.1/pref_voting/tests/test_voting_method.py
+-rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.1.1/pref_voting/utility_functions.py
+-rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.1.1/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-1.1.1/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.1.1/pref_voting/variable_candidate_axioms.py
+-rw-r--r--   0        0        0    91094 2024-04-28 12:43:02.289288 pref_voting-1.1.1/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     5566 2023-12-07 15:03:17.438046 pref_voting-1.1.1/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      372 2023-11-14 00:06:58.907333 pref_voting-1.1.1/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.1.1/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      760 2024-04-28 12:44:16.208500 pref_voting-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-1.1.1/setup.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-1.1.1/PKG-INFO
```

### Comparing `pref_voting-1.1.0/LICENSE` & `pref_voting-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/README.md` & `pref_voting-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/analysis.py` & `pref_voting-1.1.1/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/axiom.py` & `pref_voting-1.1.1/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/c1_methods.py` & `pref_voting-1.1.1/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/combined_methods.py` & `pref_voting-1.1.1/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/dominance_axioms.py` & `pref_voting-1.1.1/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/generate_profiles.py` & `pref_voting-1.1.1/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/generate_spatial_profiles.py` & `pref_voting-1.1.1/pref_voting/generate_spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/generate_utility_profiles.py` & `pref_voting-1.1.1/pref_voting/generate_utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-1.1.1/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/grade_methods.py` & `pref_voting-1.1.1/pref_voting/grade_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/grade_profiles.py` & `pref_voting-1.1.1/pref_voting/grade_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/helper.py` & `pref_voting-1.1.1/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/invariance_axioms.py` & `pref_voting-1.1.1/pref_voting/invariance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/io/readers.py` & `pref_voting-1.1.1/pref_voting/io/readers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/io/writers.py` & `pref_voting-1.1.1/pref_voting/io/writers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/iterative_methods.py` & `pref_voting-1.1.1/pref_voting/iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/maj_graph_ex1.png` & `pref_voting-1.1.1/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/mappings.py` & `pref_voting-1.1.1/pref_voting/mappings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/margin_based_methods.py` & `pref_voting-1.1.1/pref_voting/margin_based_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1638,2928 +1638,2870 @@
 00006650: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
 00006660: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
 00006670: 725f 6361 6e64 7360 600a 0a20 2020 2052  r_cands``..    R
 00006680: 6574 7572 6e73 3a20 0a20 2020 2020 2020  eturns: .       
 00006690: 2041 2073 6f72 7465 6420 6c69 7374 206f   A sorted list o
 000066a0: 6620 6361 6e64 6964 6174 6573 2e20 0a0a  f candidates. ..
 000066b0: 2020 2020 2e2e 2073 6565 616c 736f 3a3a      .. seealso::
-000066c0: 0a0a 2020 2020 2020 2020 3a6d 6574 683a  ..        :meth:
-000066d0: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
-000066e0: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
-000066f0: 732e 7261 6e6b 6564 5f70 6169 7273 602c  s.ranked_pairs`,
-00006700: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
-00006710: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
-00006720: 5f6d 6574 686f 6473 2e69 735f 7374 6163  _methods.is_stac
-00006730: 6b60 0a0a 2020 2020 3a45 7861 6d70 6c65  k`..    :Example
-00006740: 3a20 0a0a 2020 2020 2e2e 2070 6c6f 743a  : ..    .. plot:
-00006750: 3a20 206d 6172 6769 6e5f 6772 6170 6873  :  margin_graphs
-00006760: 5f65 7861 6d70 6c65 732f 6d67 5f65 785f  _examples/mg_ex_
-00006770: 6270 5f72 702e 7079 0a20 2020 2020 2020  bp_rp.py.       
-00006780: 203a 636f 6e74 6578 743a 2072 6573 6574   :context: reset
-00006790: 2020 0a20 2020 2020 2020 203a 696e 636c    .        :incl
-000067a0: 7564 652d 736f 7572 6365 3a20 5472 7565  ude-source: True
-000067b0: 0a0a 0a20 2020 202e 2e20 636f 6465 2d62  ...    .. code-b
-000067c0: 6c6f 636b 3a3a 200a 0a20 2020 2020 2020  lock:: ..       
-000067d0: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
-000067e0: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-000067f0: 6574 686f 6473 2069 6d70 6f72 7420 7261  ethods import ra
-00006800: 6e6b 6564 5f70 6169 7273 2c20 7261 6e6b  nked_pairs, rank
-00006810: 6564 5f70 6169 7273 5f66 726f 6d5f 7374  ed_pairs_from_st
-00006820: 6163 6b73 0a0a 2020 2020 2020 2020 7261  acks..        ra
-00006830: 6e6b 6564 5f70 6169 7273 2e64 6973 706c  nked_pairs.displ
-00006840: 6179 286d 6729 0a20 2020 2020 2020 2072  ay(mg).        r
-00006850: 616e 6b65 645f 7061 6972 735f 6672 6f6d  anked_pairs_from
-00006860: 5f73 7461 636b 732e 6469 7370 6c61 7928  _stacks.display(
-00006870: 6d67 290a 0a0a 2020 2020 2e2e 2065 7865  mg)...    .. exe
-00006880: 635f 636f 6465 3a3a 200a 2020 2020 2020  c_code:: .      
-00006890: 2020 3a68 6964 655f 636f 6465 3a0a 0a20    :hide_code:.. 
-000068a0: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
-000068b0: 5f76 6f74 696e 672e 7765 6967 6874 6564  _voting.weighted
-000068c0: 5f6d 616a 6f72 6974 795f 6772 6170 6873  _majority_graphs
-000068d0: 2069 6d70 6f72 7420 4d61 7267 696e 4772   import MarginGr
-000068e0: 6170 680a 2020 2020 2020 2020 6672 6f6d  aph.        from
-000068f0: 2070 7265 665f 766f 7469 6e67 2e6d 6172   pref_voting.mar
-00006900: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
-00006910: 7320 696d 706f 7274 2072 616e 6b65 645f  s import ranked_
-00006920: 7061 6972 732c 2072 616e 6b65 645f 7061  pairs, ranked_pa
-00006930: 6972 735f 6672 6f6d 5f73 7461 636b 730a  irs_from_stacks.
-00006940: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006950: 206d 6720 3d20 4d61 7267 696e 4772 6170   mg = MarginGrap
-00006960: 6828 5b30 2c20 312c 2032 2c20 335d 2c20  h([0, 1, 2, 3], 
-00006970: 5b28 302c 2032 2c20 3329 2c20 2831 2c20  [(0, 2, 3), (1, 
-00006980: 302c 2035 292c 2028 322c 2031 2c20 3529  0, 5), (2, 1, 5)
-00006990: 2c20 2832 2c20 332c 2031 292c 2028 332c  , (2, 3, 1), (3,
-000069a0: 2030 2c20 3329 2c20 2833 2c20 312c 2031   0, 3), (3, 1, 1
-000069b0: 295d 290a 0a20 2020 2020 2020 2072 616e  )])..        ran
-000069c0: 6b65 645f 7061 6972 732e 6469 7370 6c61  ked_pairs.displa
-000069d0: 7928 6d67 290a 2020 2020 2020 2020 7261  y(mg).        ra
-000069e0: 6e6b 6564 5f70 6169 7273 5f66 726f 6d5f  nked_pairs_from_
-000069f0: 7374 6163 6b73 2e64 6973 706c 6179 286d  stacks.display(m
-00006a00: 6729 0a0a 2020 2020 2222 2220 2020 200a  g)..    """    .
-00006a10: 0a20 2020 2063 616e 6469 6461 7465 7320  .    candidates 
-00006a20: 3d20 6375 7272 5f63 616e 6473 2069 6620  = curr_cands if 
-00006a30: 6375 7272 5f63 616e 6473 2069 7320 6e6f  curr_cands is no
-00006a40: 7420 4e6f 6e65 2065 6c73 6520 6564 6174  t None else edat
-00006a50: 612e 6361 6e64 6964 6174 6573 0a20 2020  a.candidates.   
-00006a60: 2077 696e 6e65 7273 203d 206c 6973 7428   winners = list(
-00006a70: 290a 2020 2020 666f 7220 636c 6973 7420  ).    for clist 
-00006a80: 696e 2070 6572 6d75 7461 7469 6f6e 7328  in permutations(
-00006a90: 6361 6e64 6964 6174 6573 293a 200a 2020  candidates): .  
-00006aa0: 2020 2020 2020 6973 7374 6163 6b20 3d20        isstack = 
-00006ab0: 6973 5f73 7461 636b 2865 6461 7461 2c20  is_stack(edata, 
-00006ac0: 636c 6973 742c 2063 7572 725f 6361 6e64  clist, curr_cand
-00006ad0: 7320 3d20 6375 7272 5f63 616e 6473 290a  s = curr_cands).
-00006ae0: 2020 2020 2020 2020 6966 2069 7373 7461          if issta
-00006af0: 636b 3a20 0a20 2020 2020 2020 2020 2020  ck: .           
-00006b00: 2077 696e 6e65 7273 2e61 7070 656e 6428   winners.append(
-00006b10: 636c 6973 745b 305d 290a 2020 2020 2020  clist[0]).      
-00006b20: 2020 2020 2020 0a20 2020 2072 6574 7572        .    retur
-00006b30: 6e20 736f 7274 6564 286c 6973 7428 7365  n sorted(list(se
-00006b40: 7428 7769 6e6e 6572 7329 2929 0a0a 6465  t(winners)))..de
-00006b50: 6620 5f72 616e 6b65 645f 7061 6972 735f  f _ranked_pairs_
-00006b60: 6261 7369 6328 0a20 2020 2065 6461 7461  basic(.    edata
-00006b70: 2c20 0a20 2020 2063 7572 725f 6361 6e64  , .    curr_cand
-00006b80: 7320 3d20 4e6f 6e65 2c20 0a20 2020 2073  s = None, .    s
-00006b90: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00006ba0: 203d 204e 6f6e 6529 3a20 2020 0a20 2020   = None):   .   
-00006bb0: 2022 2222 416e 2069 6d70 6c65 6d65 6e74   """An implement
-00006bc0: 6174 696f 6e20 6f66 2052 616e 6b65 6420  ation of Ranked 
-00006bd0: 5061 6972 7320 7468 6174 2075 7365 7320  Pairs that uses 
-00006be0: 6120 6261 7369 6320 616c 676f 7269 7468  a basic algorith
-00006bf0: 6d2e 200a 2020 2020 2222 220a 2020 2020  m. .    """.    
-00006c00: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
-00006c10: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
-00006c20: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
-00006c30: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
-00006c40: 6e64 7320 0a20 2020 2063 6964 785f 746f  nds .    cidx_to
-00006c50: 5f63 616e 6420 3d20 7b63 6964 783a 2063  _cand = {cidx: c
-00006c60: 2066 6f72 2063 6964 782c 2063 2069 6e20   for cidx, c in 
-00006c70: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
-00006c80: 6174 6573 297d 2020 0a20 2020 2063 616e  ates)}  .    can
-00006c90: 645f 746f 5f63 6964 7820 3d20 7b63 3a20  d_to_cidx = {c: 
-00006ca0: 6369 6478 2066 6f72 2063 6964 782c 2063  cidx for cidx, c
-00006cb0: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-00006cc0: 6e64 6964 6174 6573 297d 2020 0a20 2020  ndidates)}  .   
-00006cd0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00006ce0: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
-00006cf0: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
-00006d00: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
-00006d10: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
-00006d20: 6374 696f 6e20 2020 200a 0a20 2020 2063  ction    ..    c
-00006d30: 7720 3d20 6564 6174 612e 636f 6e64 6f72  w = edata.condor
-00006d40: 6365 745f 7769 6e6e 6572 2863 7572 725f  cet_winner(curr_
-00006d50: 6361 6e64 733d 6375 7272 5f63 616e 6473  cands=curr_cands
-00006d60: 290a 2020 2020 2320 5261 6e6b 6564 2050  ).    # Ranked P
-00006d70: 6169 7273 2069 7320 436f 6e64 6f72 6365  airs is Condorce
-00006d80: 7420 636f 6e73 6973 7465 6e74 2c20 736f  t consistent, so
-00006d90: 2073 696d 706c 7920 7265 7475 726e 2074   simply return t
-00006da0: 6865 2043 6f6e 646f 7263 6574 2077 696e  he Condorcet win
-00006db0: 6e65 7220 6966 2065 7869 7374 730a 2020  ner if exists.  
-00006dc0: 2020 6966 2063 7720 6973 206e 6f74 204e    if cw is not N
-00006dd0: 6f6e 653a 200a 2020 2020 2020 2020 7769  one: .        wi
-00006de0: 6e6e 6572 7320 3d20 5b63 775d 0a20 2020  nners = [cw].   
-00006df0: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
-00006e00: 5f65 6467 6573 203d 205b 2863 312c 2063  _edges = [(c1, c
-00006e10: 322c 2073 7472 656e 6774 685f 6675 6e63  2, strength_func
-00006e20: 7469 6f6e 2863 312c 2063 3229 2920 666f  tion(c1, c2)) fo
-00006e30: 7220 6331 2069 6e20 6361 6e64 6964 6174  r c1 in candidat
-00006e40: 6573 2066 6f72 2063 3220 696e 2063 616e  es for c2 in can
-00006e50: 6469 6461 7465 7320 0a20 2020 2020 2020  didates .       
-00006e60: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00006e70: 3120 213d 2063 3220 616e 6420 2865 6461  1 != c2 and (eda
-00006e80: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
-00006e90: 6572 7328 6331 2c20 6332 2920 6f72 2065  ers(c1, c2) or e
-00006ea0: 6461 7461 2e69 735f 7469 6564 2863 312c  data.is_tied(c1,
-00006eb0: 2063 3229 295d 0a20 2020 2020 2020 2077   c2))].        w
-00006ec0: 696e 6e65 7273 203d 206c 6973 7428 2920  inners = list() 
-00006ed0: 2020 0a20 2020 2020 2020 2069 6620 6c65    .        if le
-00006ee0: 6e28 775f 6564 6765 7329 203e 2030 3a20  n(w_edges) > 0: 
-00006ef0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00006f00: 2020 2020 2020 7374 7265 6e67 7468 7320        strengths 
-00006f10: 3d20 736f 7274 6564 286c 6973 7428 7365  = sorted(list(se
-00006f20: 7428 5b65 5b32 5d20 666f 7220 6520 696e  t([e[2] for e in
-00006f30: 2077 5f65 6467 6573 5d29 292c 2072 6576   w_edges])), rev
-00006f40: 6572 7365 3d54 7275 6529 0a20 2020 2020  erse=True).     
-00006f50: 2020 2020 2020 2073 6f72 7465 645f 6564         sorted_ed
-00006f60: 6765 7320 3d20 5b5b 6520 666f 7220 6520  ges = [[e for e 
-00006f70: 696e 2077 5f65 6467 6573 2069 6620 655b  in w_edges if e[
-00006f80: 325d 203d 3d20 735d 2066 6f72 2073 2069  2] == s] for s i
-00006f90: 6e20 7374 7265 6e67 7468 735d 0a20 2020  n strengths].   
-00006fa0: 2020 2020 2020 2020 2074 6273 203d 2070           tbs = p
-00006fb0: 726f 6475 6374 282a 5b70 6572 6d75 7461  roduct(*[permuta
-00006fc0: 7469 6f6e 7328 6564 6765 7329 2066 6f72  tions(edges) for
-00006fd0: 2065 6467 6573 2069 6e20 736f 7274 6564   edges in sorted
-00006fe0: 5f65 6467 6573 5d29 0a20 2020 2020 2020  _edges]).       
-00006ff0: 2020 2020 2066 6f72 2074 6220 696e 2074       for tb in t
-00007000: 6273 3a0a 2020 2020 2020 2020 2020 2020  bs:.            
-00007010: 2020 2020 6564 6765 7320 3d20 666c 6174      edges = flat
-00007020: 7465 6e28 7462 290a 2020 2020 2020 2020  ten(tb).        
-00007030: 2020 2020 2020 2020 7270 5f64 6566 6561          rp_defea
-00007040: 7420 3d20 5350 4f28 6c65 6e28 6361 6e64  t = SPO(len(cand
-00007050: 6964 6174 6573 2929 0a20 2020 2020 2020  idates)).       
-00007060: 2020 2020 2020 2020 2066 6f72 2065 302c           for e0,
-00007070: 6531 2c73 2069 6e20 6564 6765 733a 200a  e1,s in edges: .
-00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007090: 2020 2020 6966 206e 6f74 2072 705f 6465      if not rp_de
-000070a0: 6665 6174 2e50 5b63 616e 645f 746f 5f63  feat.P[cand_to_c
-000070b0: 6964 785b 6531 5d5d 5b63 616e 645f 746f  idx[e1]][cand_to
-000070c0: 5f63 6964 785b 6530 5d5d 3a0a 2020 2020  _cidx[e0]]:.    
-000070d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070e0: 2020 2020 7270 5f64 6566 6561 742e 6164      rp_defeat.ad
-000070f0: 6428 6361 6e64 5f74 6f5f 6369 6478 5b65  d(cand_to_cidx[e
-00007100: 305d 2c63 616e 645f 746f 5f63 6964 785b  0],cand_to_cidx[
-00007110: 6531 5d29 0a20 2020 2020 2020 2020 2020  e1]).           
-00007120: 2020 2020 2077 696e 6e65 7273 2e61 7070       winners.app
-00007130: 656e 6428 6369 6478 5f74 6f5f 6361 6e64  end(cidx_to_cand
-00007140: 5b72 705f 6465 6665 6174 2e69 6e69 7469  [rp_defeat.initi
-00007150: 616c 5f65 6c65 6d65 6e74 7328 295b 305d  al_elements()[0]
-00007160: 5d29 0a20 2020 2020 2020 2065 6c73 653a  ]).        else:
-00007170: 200a 2020 2020 2020 2020 2020 2020 7769   .            wi
-00007180: 6e6e 6572 7320 3d20 6361 6e64 6964 6174  nners = candidat
-00007190: 6573 0a20 2020 2072 6574 7572 6e20 736f  es.    return so
-000071a0: 7274 6564 286c 6973 7428 7365 7428 7769  rted(list(set(wi
-000071b0: 6e6e 6572 7329 2929 0a0a 0a40 766d 286e  nners)))...@vm(n
-000071c0: 616d 653d 2252 616e 6b65 6420 5061 6972  ame="Ranked Pair
-000071d0: 7322 290a 6465 6620 7261 6e6b 6564 5f70  s").def ranked_p
-000071e0: 6169 7273 280a 2020 2020 6564 6174 612c  airs(.    edata,
-000071f0: 200a 2020 2020 6375 7272 5f63 616e 6473   .    curr_cands
-00007200: 3d4e 6f6e 652c 200a 2020 2020 7374 7265  =None, .    stre
-00007210: 6e67 7468 5f66 756e 6374 696f 6e3d 4e6f  ngth_function=No
-00007220: 6e65 2c20 0a20 2020 2061 6c67 6f72 6974  ne, .    algorit
-00007230: 686d 3d27 6261 7369 6327 293a 2020 200a  hm='basic'):   .
-00007240: 2020 2020 2222 220a 2020 2020 4f72 6465      """.    Orde
-00007250: 7220 7468 6520 6564 6765 7320 696e 2074  r the edges in t
-00007260: 6865 206d 6172 6769 6e20 6772 6170 6820  he margin graph 
-00007270: 6672 6f6d 206c 6172 6765 7374 2074 6f20  from largest to 
-00007280: 736d 616c 6c65 7374 2061 6e64 206c 6f63  smallest and loc
-00007290: 6b20 7468 656d 2069 6e20 696e 2074 6861  k them in in tha
-000072a0: 7420 6f72 6465 722c 2073 6b69 7070 696e  t order, skippin
-000072b0: 6720 6564 6765 7320 7468 6174 2063 7265  g edges that cre
-000072c0: 6174 6520 6120 6379 636c 652e 2020 4966  ate a cycle.  If
-000072d0: 2074 6865 7265 2061 7265 2074 6965 7320   there are ties 
-000072e0: 696e 2074 6865 206d 6172 6769 6e73 2c20  in the margins, 
-000072f0: 6272 6561 6b20 7468 6520 7469 6573 2075  break the ties u
-00007300: 7369 6e67 2061 2074 6965 2d62 7265 616b  sing a tie-break
-00007310: 696e 6720 7275 6c65 3a20 6120 6c69 6e65  ing rule: a line
-00007320: 6172 206f 7264 6572 696e 6720 6f76 6572  ar ordering over
-00007330: 2074 6865 2065 6467 6573 2e20 2020 4120   the edges.   A 
-00007340: 6361 6e64 6964 6174 6520 6973 2061 2052  candidate is a R
-00007350: 616e 6b65 6420 5061 6972 7320 7769 6e6e  anked Pairs winn
-00007360: 6572 2069 6620 6974 2077 696e 7320 6163  er if it wins ac
-00007370: 636f 7264 696e 6720 746f 2073 6f6d 6520  cording to some 
-00007380: 7469 652d 6272 6561 6b69 6e67 2072 756c  tie-breaking rul
-00007390: 652e 2041 6c73 6f20 6b6e 6f77 6e20 6173  e. Also known as
-000073a0: 2054 6964 656d 616e 2773 2052 756c 652e   Tideman's Rule.
-000073b0: 0a0a 2020 2020 2e2e 2077 6172 6e69 6e67  ..    .. warning
-000073c0: 3a3a 200a 2020 2020 2020 2020 5468 6973  :: .        This
-000073d0: 206d 6574 686f 6420 6361 6e20 7461 6b65   method can take
-000073e0: 2061 2076 6572 7920 6c6f 6e67 2074 696d   a very long tim
-000073f0: 6520 746f 2066 696e 6420 7769 6e6e 6572  e to find winner
-00007400: 732e 200a 2020 2020 2020 2020 0a20 2020  s. .        .   
-00007410: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
-00007420: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
-00007430: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
-00007440: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
-00007450: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
-00007460: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
-00007470: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
-00007480: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-00007490: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-000074a0: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-000074b0: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-000074c0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-000074d0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-000074e0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-000074f0: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-00007500: 7360 600a 2020 2020 2020 2020 7374 7265  s``.        stre
-00007510: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
-00007520: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
-00007530: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
-00007540: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
-00007550: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
-00007560: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
-00007570: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
-00007580: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
-00007590: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
-000075a0: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
-000075b0: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
-000075c0: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
-000075d0: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
-000075e0: 7264 6572 732e 200a 2020 2020 2020 2020  rders. .        
-000075f0: 616c 676f 7269 7468 6d20 2873 7472 2c20  algorithm (str, 
-00007600: 6f70 7469 6f6e 616c 293a 2053 7065 6369  optional): Speci
-00007610: 6679 2077 6869 6368 2061 6c67 6f72 6974  fy which algorit
-00007620: 686d 2074 6f20 7573 652e 2020 4f70 7469  hm to use.  Opti
-00007630: 6f6e 7320 6172 6520 2762 6173 6963 2720  ons are 'basic' 
-00007640: 2874 6865 2064 6566 6175 6c74 2920 616e  (the default) an
-00007650: 6420 2766 726f 6d5f 7374 6163 6b73 272e  d 'from_stacks'.
-00007660: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
-00007670: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
-00007680: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
-00007690: 7465 732e 200a 0a20 2020 202e 2e20 7365  tes. ..    .. se
-000076a0: 6561 6c73 6f3a 3a0a 0a20 2020 2020 2020  ealso::..       
-000076b0: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
-000076c0: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
-000076d0: 5f6d 6574 686f 6473 2e72 616e 6b65 645f  _methods.ranked_
-000076e0: 7061 6972 735f 7769 7468 5f74 6573 7460  pairs_with_test`
-000076f0: 2c20 3a6d 6574 683a 6070 7265 665f 766f  , :meth:`pref_vo
-00007700: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
-00007710: 645f 6d65 7468 6f64 732e 7261 6e6b 6564  d_methods.ranked
-00007720: 5f70 6169 7273 5f7a 7460 2c20 3a6d 6574  _pairs_zt`, :met
-00007730: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
-00007740: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-00007750: 6f64 732e 7261 6e6b 6564 5f70 6169 7273  ods.ranked_pairs
-00007760: 5f64 6566 6561 7473 600a 0a20 2020 203a  _defeats`..    :
-00007770: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
-00007780: 2e20 706c 6f74 3a3a 2020 6d61 7267 696e  . plot::  margin
-00007790: 5f67 7261 7068 735f 6578 616d 706c 6573  _graphs_examples
-000077a0: 2f6d 675f 6578 5f62 705f 7270 2e70 790a  /mg_ex_bp_rp.py.
-000077b0: 2020 2020 2020 2020 3a63 6f6e 7465 7874          :context
-000077c0: 3a20 7265 7365 7420 200a 2020 2020 2020  : reset  .      
-000077d0: 2020 3a69 6e63 6c75 6465 2d73 6f75 7263    :include-sourc
-000077e0: 653a 2054 7275 650a 0a0a 2020 2020 2e2e  e: True...    ..
-000077f0: 2063 6f64 652d 626c 6f63 6b3a 3a20 0a0a   code-block:: ..
-00007800: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-00007810: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
-00007820: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
-00007830: 706f 7274 2072 616e 6b65 645f 7061 6972  port ranked_pair
-00007840: 730a 0a20 2020 2020 2020 2072 616e 6b65  s..        ranke
-00007850: 645f 7061 6972 732e 6469 7370 6c61 7928  d_pairs.display(
-00007860: 6d67 290a 2020 2020 2020 2020 7261 6e6b  mg).        rank
-00007870: 6564 5f70 6169 7273 2e64 6973 706c 6179  ed_pairs.display
-00007880: 286d 672c 2061 6c67 6f72 6974 686d 3d27  (mg, algorithm='
-00007890: 6261 7369 6327 2920 0a20 2020 2020 2020  basic') .       
-000078a0: 2072 616e 6b65 645f 7061 6972 732e 6469   ranked_pairs.di
-000078b0: 7370 6c61 7928 6d67 2c20 616c 676f 7269  splay(mg, algori
-000078c0: 7468 6d3d 2766 726f 6d5f 7374 6163 6b73  thm='from_stacks
-000078d0: 2729 2020 2020 0a0a 0a20 2020 202e 2e20  ')    ...    .. 
-000078e0: 6578 6563 5f63 6f64 653a 3a20 0a20 2020  exec_code:: .   
-000078f0: 2020 2020 203a 6869 6465 5f63 6f64 653a       :hide_code:
-00007900: 0a0a 2020 2020 2020 2020 6672 6f6d 2070  ..        from p
-00007910: 7265 665f 766f 7469 6e67 2e77 6569 6768  ref_voting.weigh
-00007920: 7465 645f 6d61 6a6f 7269 7479 5f67 7261  ted_majority_gra
-00007930: 7068 7320 696d 706f 7274 204d 6172 6769  phs import Margi
-00007940: 6e47 7261 7068 0a20 2020 2020 2020 2066  nGraph.        f
-00007950: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
-00007960: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-00007970: 686f 6473 2069 6d70 6f72 7420 7261 6e6b  hods import rank
-00007980: 6564 5f70 6169 7273 0a20 2020 2020 2020  ed_pairs.       
-00007990: 200a 2020 2020 2020 2020 6d67 203d 204d   .        mg = M
-000079a0: 6172 6769 6e47 7261 7068 285b 302c 2031  arginGraph([0, 1
-000079b0: 2c20 322c 2033 5d2c 205b 2830 2c20 322c  , 2, 3], [(0, 2,
-000079c0: 2033 292c 2028 312c 2030 2c20 3529 2c20   3), (1, 0, 5), 
-000079d0: 2832 2c20 312c 2035 292c 2028 322c 2033  (2, 1, 5), (2, 3
-000079e0: 2c20 3129 2c20 2833 2c20 302c 2033 292c  , 1), (3, 0, 3),
-000079f0: 2028 332c 2031 2c20 3129 5d29 0a20 2020   (3, 1, 1)]).   
-00007a00: 2020 2020 200a 2020 2020 2020 2020 7261       .        ra
-00007a10: 6e6b 6564 5f70 6169 7273 2e64 6973 706c  nked_pairs.displ
-00007a20: 6179 286d 6729 0a20 2020 2020 2020 2072  ay(mg).        r
-00007a30: 616e 6b65 645f 7061 6972 732e 6469 7370  anked_pairs.disp
-00007a40: 6c61 7928 6d67 2c20 616c 676f 7269 7468  lay(mg, algorith
-00007a50: 6d3d 2762 6173 6963 2729 0a20 2020 2020  m='basic').     
-00007a60: 2020 2072 616e 6b65 645f 7061 6972 732e     ranked_pairs.
-00007a70: 6469 7370 6c61 7928 6d67 2c20 616c 676f  display(mg, algo
-00007a80: 7269 7468 6d3d 2766 726f 6d5f 7374 6163  rithm='from_stac
-00007a90: 6b73 2729 0a0a 2020 2020 2222 220a 0a20  ks')..    """.. 
-00007aa0: 2020 2069 6620 616c 676f 7269 7468 6d20     if algorithm 
-00007ab0: 3d3d 2027 6261 7369 6327 3a0a 2020 2020  == 'basic':.    
-00007ac0: 2020 2020 7265 7475 726e 205f 7261 6e6b      return _rank
-00007ad0: 6564 5f70 6169 7273 5f62 6173 6963 2865  ed_pairs_basic(e
-00007ae0: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
-00007af0: 203d 2063 7572 725f 6361 6e64 732c 2073   = curr_cands, s
-00007b00: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00007b10: 203d 2073 7472 656e 6774 685f 6675 6e63   = strength_func
-00007b20: 7469 6f6e 290a 2020 2020 656c 6966 2061  tion).    elif a
-00007b30: 6c67 6f72 6974 686d 203d 3d20 2766 726f  lgorithm == 'fro
-00007b40: 6d5f 7374 6163 6b73 273a 0a20 2020 2020  m_stacks':.     
-00007b50: 2020 2072 6574 7572 6e20 5f72 616e 6b65     return _ranke
-00007b60: 645f 7061 6972 735f 6672 6f6d 5f73 7461  d_pairs_from_sta
-00007b70: 636b 7328 6564 6174 612c 2063 7572 725f  cks(edata, curr_
-00007b80: 6361 6e64 7320 3d20 6375 7272 5f63 616e  cands = curr_can
-00007b90: 6473 290a 2020 2020 656c 7365 3a0a 2020  ds).    else:.  
-00007ba0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00007bb0: 6545 7272 6f72 2822 496e 7661 6c69 6420  eError("Invalid 
-00007bc0: 616c 676f 7269 7468 6d20 7370 6563 6966  algorithm specif
-00007bd0: 6965 642e 2229 0a0a 0a40 766d 286e 616d  ied.")...@vm(nam
-00007be0: 653d 2252 616e 6b65 6420 5061 6972 7322  e="Ranked Pairs"
-00007bf0: 290a 6465 6620 7261 6e6b 6564 5f70 6169  ).def ranked_pai
-00007c00: 7273 5f77 6974 685f 7465 7374 2865 6461  rs_with_test(eda
-00007c10: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
-00007c20: 204e 6f6e 652c 2073 7472 656e 6774 685f   None, strength_
-00007c30: 6675 6e63 7469 6f6e 203d 204e 6f6e 6529  function = None)
-00007c40: 3a20 2020 0a20 2020 2022 2222 4669 6e64  :   .    """Find
-00007c50: 2074 6865 2052 616e 6b65 6420 5061 6972   the Ranked Pair
-00007c60: 7320 7769 6e6e 6572 732c 2062 7574 2069  s winners, but i
-00007c70: 6e63 6c75 6465 2061 2074 6573 7420 746f  nclude a test to
-00007c80: 2064 6574 6572 6d69 6e65 6420 6966 2069   determined if i
-00007c90: 7420 7769 6c6c 2074 616b 6520 746f 6f20  t will take too 
-00007ca0: 6c6f 6e67 2074 6f20 636f 6d70 7574 6520  long to compute 
-00007cb0: 7468 6520 5261 6e6b 6564 2050 6169 7273  the Ranked Pairs
-00007cc0: 2077 696e 6e65 7273 2e20 4966 2074 6865   winners. If the
-00007cd0: 2063 616c 6375 6c61 7469 6f6e 206f 6620   calculation of 
-00007ce0: 7468 6520 7769 6e6e 6572 7320 7769 6c6c  the winners will
-00007cf0: 2074 616b 6520 746f 6f20 6c6f 6e67 2c20   take too long, 
-00007d00: 7265 7475 726e 204e 6f6e 652e 0a0a 2020  return None...  
-00007d10: 2020 2e2e 2069 6d70 6f72 7461 6e74 3a3a    .. important::
-00007d20: 0a20 2020 2020 2020 2054 6869 7320 766f  .        This vo
-00007d30: 7469 6e67 206d 6574 686f 6420 7468 6174  ting method that
-00007d40: 206d 6967 6874 2072 6574 7572 6e20 4e6f   might return No
-00007d50: 6e65 2072 6174 6865 7220 7468 616e 2061  ne rather than a
-00007d60: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
-00007d70: 7465 732e 2020 0a0a 2020 2020 4172 6773  tes.  ..    Args
-00007d80: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
-00007d90: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
-00007da0: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
-00007db0: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
-00007dc0: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
-00007dd0: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
-00007de0: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
-00007df0: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
-00007e00: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
-00007e10: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
-00007e20: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
-00007e30: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
-00007e40: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
-00007e50: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
-00007e60: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
-00007e70: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
-00007e80: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
-00007e90: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
-00007ea0: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
-00007eb0: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
-00007ec0: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
-00007ed0: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
-00007ee0: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
-00007ef0: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
-00007f00: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
-00007f10: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
-00007f20: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
-00007f30: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
-00007f40: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
-00007f50: 2e20 0a0a 2020 2020 5265 7475 726e 733a  . ..    Returns:
-00007f60: 200a 2020 2020 2020 2020 4120 736f 7274   .        A sort
-00007f70: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
-00007f80: 6461 7465 732e 200a 0a20 2020 202e 2e20  dates. ..    .. 
-00007f90: 7365 6561 6c73 6f3a 3a0a 0a20 2020 2020  seealso::..     
-00007fa0: 2020 203a 6d65 7468 3a60 7072 6566 5f76     :meth:`pref_v
-00007fb0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-00007fc0: 6564 5f6d 6574 686f 6473 2e72 616e 6b65  ed_methods.ranke
-00007fd0: 645f 7061 6972 735f 7769 7468 5f74 6573  d_pairs_with_tes
-00007fe0: 7460 2c20 3a6d 6574 683a 6070 7265 665f  t`, :meth:`pref_
-00007ff0: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-00008000: 7365 645f 6d65 7468 6f64 732e 7261 6e6b  sed_methods.rank
-00008010: 6564 5f70 6169 7273 5f7a 7460 2c20 3a6d  ed_pairs_zt`, :m
-00008020: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
-00008030: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-00008040: 7468 6f64 732e 7261 6e6b 6564 5f70 6169  thods.ranked_pai
-00008050: 7273 5f64 6566 6561 7473 600a 0a20 2020  rs_defeats`..   
-00008060: 203a 4578 616d 706c 653a 200a 0a20 2020   :Example: ..   
-00008070: 202e 2e20 706c 6f74 3a3a 2020 6d61 7267   .. plot::  marg
-00008080: 696e 5f67 7261 7068 735f 6578 616d 706c  in_graphs_exampl
-00008090: 6573 2f6d 675f 6578 5f72 705f 7769 7468  es/mg_ex_rp_with
-000080a0: 5f74 6573 742e 7079 0a20 2020 2020 2020  _test.py.       
-000080b0: 203a 636f 6e74 6578 743a 2072 6573 6574   :context: reset
-000080c0: 2020 0a20 2020 2020 2020 203a 696e 636c    .        :incl
-000080d0: 7564 652d 736f 7572 6365 3a20 5472 7565  ude-source: True
-000080e0: 0a0a 0a20 2020 202e 2e20 636f 6465 2d62  ...    .. code-b
-000080f0: 6c6f 636b 3a3a 200a 0a20 2020 2020 2020  lock:: ..       
-00008100: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
-00008110: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-00008120: 6574 686f 6473 2069 6d70 6f72 7420 7261  ethods import ra
-00008130: 6e6b 6564 5f70 6169 7273 5f77 6974 685f  nked_pairs_with_
-00008140: 7465 7374 0a0a 2020 2020 2020 2020 7261  test..        ra
-00008150: 6e6b 6564 5f70 6169 7273 5f77 6974 685f  nked_pairs_with_
-00008160: 7465 7374 2e64 6973 706c 6179 286d 6729  test.display(mg)
-00008170: 0a0a 0a20 2020 202e 2e20 6578 6563 5f63  ...    .. exec_c
-00008180: 6f64 653a 3a20 0a20 2020 2020 2020 203a  ode:: .        :
-00008190: 6869 6465 5f63 6f64 653a 0a0a 2020 2020  hide_code:..    
-000081a0: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
-000081b0: 7469 6e67 2e77 6569 6768 7465 645f 6d61  ting.weighted_ma
-000081c0: 6a6f 7269 7479 5f67 7261 7068 7320 696d  jority_graphs im
-000081d0: 706f 7274 204d 6172 6769 6e47 7261 7068  port MarginGraph
-000081e0: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
-000081f0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-00008200: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
-00008210: 6d70 6f72 7420 7261 6e6b 6564 5f70 6169  mport ranked_pai
-00008220: 7273 5f77 6974 685f 7465 7374 0a20 2020  rs_with_test.   
-00008230: 2020 2020 200a 2020 2020 2020 2020 6d67       .        mg
-00008240: 203d 204d 6172 6769 6e47 7261 7068 285b   = MarginGraph([
-00008250: 302c 2031 2c20 322c 2033 5d2c 205b 2831  0, 1, 2, 3], [(1
-00008260: 2c20 322c 2032 292c 2028 312c 2033 2c20  , 2, 2), (1, 3, 
-00008270: 3229 2c20 2832 2c20 302c 2032 295d 290a  2), (2, 0, 2)]).
-00008280: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00008290: 2072 616e 6b65 645f 7061 6972 735f 7769   ranked_pairs_wi
-000082a0: 7468 5f74 6573 742e 6469 7370 6c61 7928  th_test.display(
-000082b0: 6d67 290a 0a0a 2020 2020 2222 2220 2020  mg)...    """   
-000082c0: 200a 2020 2020 6361 6e64 6964 6174 6573   .    candidates
-000082d0: 203d 2065 6461 7461 2e63 616e 6469 6461   = edata.candida
-000082e0: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
-000082f0: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
-00008300: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
-00008310: 2020 6369 6478 5f74 6f5f 6361 6e64 203d    cidx_to_cand =
-00008320: 207b 6369 6478 3a20 6320 666f 7220 6369   {cidx: c for ci
-00008330: 6478 2c20 6320 696e 2065 6e75 6d65 7261  dx, c in enumera
-00008340: 7465 2863 616e 6469 6461 7465 7329 7d20  te(candidates)} 
-00008350: 200a 2020 2020 6361 6e64 5f74 6f5f 6369   .    cand_to_ci
-00008360: 6478 203d 207b 633a 2063 6964 7820 666f  dx = {c: cidx fo
-00008370: 7220 6369 6478 2c20 6320 696e 2065 6e75  r cidx, c in enu
-00008380: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
-00008390: 7329 7d20 200a 2020 2020 0a20 2020 2073  s)}  .    .    s
-000083a0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-000083b0: 203d 2065 6461 7461 2e6d 6172 6769 6e20   = edata.margin 
-000083c0: 6966 2073 7472 656e 6774 685f 6675 6e63  if strength_func
-000083d0: 7469 6f6e 2069 7320 4e6f 6e65 2065 6c73  tion is None els
-000083e0: 6520 7374 7265 6e67 7468 5f66 756e 6374  e strength_funct
-000083f0: 696f 6e20 2020 0a0a 2020 2020 6377 203d  ion   ..    cw =
-00008400: 2065 6461 7461 2e63 6f6e 646f 7263 6574   edata.condorcet
-00008410: 5f77 696e 6e65 7228 6375 7272 5f63 616e  _winner(curr_can
-00008420: 6473 203d 2063 7572 725f 6361 6e64 7329  ds = curr_cands)
-00008430: 0a20 2020 2023 2052 616e 6b65 6420 5061  .    # Ranked Pa
-00008440: 6972 7320 6973 2043 6f6e 646f 7263 6574  irs is Condorcet
-00008450: 2063 6f6e 7369 7374 656e 742c 2073 6f20   consistent, so 
-00008460: 7369 6d70 6c79 2072 6574 7572 6e20 7468  simply return th
-00008470: 6520 436f 6e64 6f72 6365 7420 7769 6e6e  e Condorcet winn
-00008480: 6572 2069 6620 6578 6973 7473 0a20 2020  er if exists.   
-00008490: 2069 6620 6377 2069 7320 6e6f 7420 4e6f   if cw is not No
-000084a0: 6e65 3a20 0a20 2020 2020 2020 2077 696e  ne: .        win
-000084b0: 6e65 7273 203d 205b 6377 5d0a 2020 2020  ners = [cw].    
-000084c0: 656c 7365 3a0a 2020 2020 2020 2020 775f  else:.        w_
-000084d0: 6564 6765 7320 3d20 5b28 6331 2c20 6332  edges = [(c1, c2
-000084e0: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
-000084f0: 696f 6e28 6331 2c20 6332 2929 2066 6f72  ion(c1, c2)) for
-00008500: 2063 3120 696e 2063 616e 6469 6461 7465   c1 in candidate
-00008510: 7320 666f 7220 6332 2069 6e20 6361 6e64  s for c2 in cand
-00008520: 6964 6174 6573 200a 2020 2020 2020 2020  idates .        
-00008530: 2020 2020 2020 2020 2020 2069 6620 6331             if c1
-00008540: 2021 3d20 6332 2061 6e64 2028 6564 6174   != c2 and (edat
-00008550: 612e 6d61 6a6f 7269 7479 5f70 7265 6665  a.majority_prefe
-00008560: 7273 2863 312c 2063 3229 206f 7220 6564  rs(c1, c2) or ed
-00008570: 6174 612e 6973 5f74 6965 6428 6331 2c20  ata.is_tied(c1, 
-00008580: 6332 2929 5d0a 2020 2020 2020 2020 7769  c2))].        wi
-00008590: 6e6e 6572 7320 3d20 6c69 7374 2829 2020  nners = list()  
-000085a0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-000085b0: 2020 2073 7472 656e 6774 6873 203d 2073     strengths = s
-000085c0: 6f72 7465 6428 6c69 7374 2873 6574 285b  orted(list(set([
-000085d0: 655b 325d 2066 6f72 2065 2069 6e20 775f  e[2] for e in w_
-000085e0: 6564 6765 735d 2929 2c20 7265 7665 7273  edges])), revers
-000085f0: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
-00008600: 736f 7274 6564 5f65 6467 6573 203d 205b  sorted_edges = [
-00008610: 5b65 2066 6f72 2065 2069 6e20 775f 6564  [e for e in w_ed
-00008620: 6765 7320 6966 2065 5b32 5d20 3d3d 2073  ges if e[2] == s
-00008630: 5d20 666f 7220 7320 696e 2073 7472 656e  ] for s in stren
-00008640: 6774 6873 5d0a 2020 2020 2020 2020 6966  gths].        if
-00008650: 206e 702e 7072 6f64 285b 6d61 7468 2e66   np.prod([math.f
-00008660: 6163 746f 7269 616c 286c 656e 2865 7329  actorial(len(es)
-00008670: 2920 666f 7220 6573 2069 6e20 736f 7274  ) for es in sort
-00008680: 6564 5f65 6467 6573 5d29 203e 2033 3030  ed_edges]) > 300
-00008690: 303a 200a 2020 2020 2020 2020 2020 2020  0: .            
-000086a0: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
-000086b0: 2020 2020 656c 7365 3a20 0a20 2020 2020      else: .     
-000086c0: 2020 2020 2020 2074 6273 203d 2070 726f         tbs = pro
-000086d0: 6475 6374 282a 5b70 6572 6d75 7461 7469  duct(*[permutati
-000086e0: 6f6e 7328 6564 6765 7329 2066 6f72 2065  ons(edges) for e
-000086f0: 6467 6573 2069 6e20 736f 7274 6564 5f65  dges in sorted_e
-00008700: 6467 6573 5d29 0a20 2020 2020 2020 2020  dges]).         
-00008710: 2020 2066 6f72 2074 6220 696e 2074 6273     for tb in tbs
-00008720: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008730: 2020 6564 6765 7320 3d20 666c 6174 7465    edges = flatte
-00008740: 6e28 7462 290a 2020 2020 2020 2020 2020  n(tb).          
-00008750: 2020 2020 2020 7270 5f64 6566 6561 7420        rp_defeat 
-00008760: 3d20 5350 4f28 6c65 6e28 6361 6e64 6964  = SPO(len(candid
-00008770: 6174 6573 2929 0a20 2020 2020 2020 2020  ates)).         
-00008780: 2020 2020 2020 2066 6f72 2065 302c 6531         for e0,e1
-00008790: 2c73 2069 6e20 6564 6765 733a 200a 2020  ,s in edges: .  
-000087a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087b0: 2020 6966 206e 6f74 2072 705f 6465 6665    if not rp_defe
-000087c0: 6174 2e50 5b63 616e 645f 746f 5f63 6964  at.P[cand_to_cid
-000087d0: 785b 6531 5d5d 5b63 616e 645f 746f 5f63  x[e1]][cand_to_c
-000087e0: 6964 785b 6530 5d5d 3a0a 2020 2020 2020  idx[e0]]:.      
-000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008800: 2020 7270 5f64 6566 6561 742e 6164 6428    rp_defeat.add(
-00008810: 6361 6e64 5f74 6f5f 6369 6478 5b65 305d  cand_to_cidx[e0]
-00008820: 2c63 616e 645f 746f 5f63 6964 785b 6531  ,cand_to_cidx[e1
-00008830: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00008840: 2020 2077 696e 6e65 7273 2e61 7070 656e     winners.appen
-00008850: 6428 6369 6478 5f74 6f5f 6361 6e64 5b72  d(cidx_to_cand[r
-00008860: 705f 6465 6665 6174 2e69 6e69 7469 616c  p_defeat.initial
-00008870: 5f65 6c65 6d65 6e74 7328 295b 305d 5d29  _elements()[0]])
-00008880: 0a20 2020 2072 6574 7572 6e20 736f 7274  .    return sort
-00008890: 6564 286c 6973 7428 7365 7428 7769 6e6e  ed(list(set(winn
-000088a0: 6572 7329 2929 0a0a 6465 6620 7261 6e6b  ers)))..def rank
-000088b0: 6564 5f70 6169 7273 5f64 6566 6561 7473  ed_pairs_defeats
-000088c0: 2865 6461 7461 2c20 6375 7272 5f63 616e  (edata, curr_can
-000088d0: 6473 203d 204e 6f6e 652c 2073 7472 656e  ds = None, stren
-000088e0: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
-000088f0: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
-00008900: 0a20 2020 2052 6574 7572 6e73 2074 6865  .    Returns the
-00008910: 2052 616e 6b65 6420 5061 6972 7320 6465   Ranked Pairs de
-00008920: 6665 6174 2072 656c 6174 696f 6e73 2070  feat relations p
-00008930: 726f 6475 6365 6420 6279 2074 6865 2052  roduced by the R
-00008940: 616e 6b65 6420 5061 6972 7320 616c 676f  anked Pairs algo
-00008950: 7269 7468 6d2e 200a 0a20 2020 202e 2e20  rithm. ..    .. 
-00008960: 696d 706f 7274 616e 743a 3a0a 2020 2020  important::.    
-00008970: 2020 2020 556e 6c69 6b65 2074 6865 206f      Unlike the o
-00008980: 7468 6572 2066 756e 6374 696f 6e73 2074  ther functions t
-00008990: 6861 7420 7265 7475 726e 2061 2073 696e  hat return a sin
-000089a0: 676c 6520 6465 6665 6174 2072 656c 6174  gle defeat relat
-000089b0: 696f 6e2c 2074 6869 7320 7265 7475 726e  ion, this return
-000089c0: 7320 6120 6c69 7374 206f 6620 6465 6665  s a list of defe
-000089d0: 6174 2072 656c 6174 696f 6e73 2e20 0a20  at relations. . 
-000089e0: 2020 2020 2020 200a 2020 2020 4172 6773         .    Args
-000089f0: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
-00008a00: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
-00008a10: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
-00008a20: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
-00008a30: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
-00008a40: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
-00008a50: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
-00008a60: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
-00008a70: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
-00008a80: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
-00008a90: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
-00008aa0: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
-00008ab0: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
-00008ac0: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
-00008ad0: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
-00008ae0: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
-00008af0: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
-00008b00: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
-00008b10: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
-00008b20: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
-00008b30: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
-00008b40: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
-00008b50: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
-00008b60: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
-00008b70: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
-00008b80: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
-00008b90: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
-00008ba0: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
-00008bb0: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
-00008bc0: 2e20 0a0a 2020 2020 5265 7475 726e 733a  . ..    Returns:
-00008bd0: 200a 2020 2020 2020 2020 4120 6e65 7477   .        A netw
-00008be0: 6f72 6b78 2044 6947 7261 7068 2072 6570  orkx DiGraph rep
-00008bf0: 7265 7365 6e74 696e 6720 7468 6520 5261  resenting the Ra
-00008c00: 6e6b 6564 2050 6169 7273 2064 6566 6561  nked Pairs defea
-00008c10: 7420 7265 6c61 7469 6f6e 2e20 0a0a 2020  t relation. ..  
-00008c20: 2020 2e2e 2073 6565 616c 736f 3a3a 0a0a    .. seealso::..
-00008c30: 2020 2020 2020 2020 3a6d 6574 683a 6070          :meth:`p
-00008c40: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-00008c50: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-00008c60: 7261 6e6b 6564 5f70 6169 7273 602c 203a  ranked_pairs`, :
-00008c70: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-00008c80: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-00008c90: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
-00008ca0: 6972 735f 7769 7468 5f74 6573 7460 0a0a  irs_with_test`..
-00008cb0: 2020 2020 3a45 7861 6d70 6c65 3a20 0a0a      :Example: ..
-00008cc0: 2020 2020 2e2e 2070 6c6f 743a 3a20 206d      .. plot::  m
-00008cd0: 6172 6769 6e5f 6772 6170 6873 5f65 7861  argin_graphs_exa
-00008ce0: 6d70 6c65 732f 6d67 5f65 785f 7270 5f64  mples/mg_ex_rp_d
-00008cf0: 6566 6561 7473 2e70 790a 2020 2020 2020  efeats.py.      
-00008d00: 2020 3a63 6f6e 7465 7874 3a20 7265 7365    :context: rese
-00008d10: 7420 200a 2020 2020 2020 2020 3a69 6e63  t  .        :inc
-00008d20: 6c75 6465 2d73 6f75 7263 653a 2054 7275  lude-source: Tru
-00008d30: 650a 0a20 2020 202e 2e20 6578 6563 5f63  e..    .. exec_c
-00008d40: 6f64 653a 3a0a 0a0a 2020 2020 2020 2020  ode::...        
-00008d50: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
-00008d60: 2e77 6569 6768 7465 645f 6d61 6a6f 7269  .weighted_majori
-00008d70: 7479 5f67 7261 7068 7320 696d 706f 7274  ty_graphs import
-00008d80: 204d 6172 6769 6e47 7261 7068 0a20 2020   MarginGraph.   
-00008d90: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-00008da0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-00008db0: 6564 5f6d 6574 686f 6473 2069 6d70 6f72  ed_methods impor
-00008dc0: 7420 7261 6e6b 6564 5f70 6169 7273 5f64  t ranked_pairs_d
-00008dd0: 6566 6561 7473 0a0a 2020 2020 2020 2020  efeats..        
-00008de0: 6d67 203d 204d 6172 6769 6e47 7261 7068  mg = MarginGraph
-00008df0: 285b 302c 2031 2c20 322c 2033 5d2c 205b  ([0, 1, 2, 3], [
-00008e00: 2830 2c20 312c 2031 3029 2c20 2830 2c20  (0, 1, 10), (0, 
-00008e10: 322c 2032 292c 2028 312c 2033 2c20 3429  2, 2), (1, 3, 4)
-00008e20: 2c20 2832 2c20 312c 2036 292c 2028 322c  , (2, 1, 6), (2,
-00008e30: 2033 2c20 3829 2c20 2833 2c20 302c 2034   3, 8), (3, 0, 4
-00008e40: 295d 290a 2020 2020 2020 2020 7270 5f64  )]).        rp_d
-00008e50: 6566 6561 7473 203d 2072 616e 6b65 645f  efeats = ranked_
-00008e60: 7061 6972 735f 6465 6665 6174 7328 6d67  pairs_defeats(mg
-00008e70: 290a 0a20 2020 2020 2020 2066 6f72 2072  )..        for r
-00008e80: 7064 2069 6e20 7270 5f64 6566 6561 7473  pd in rp_defeats
-00008e90: 3a20 0a20 2020 2020 2020 2020 2020 2070  : .            p
-00008ea0: 7269 6e74 2872 7064 2e65 6467 6573 290a  rint(rpd.edges).
-00008eb0: 0a20 2020 2022 2222 0a20 2020 200a 2020  .    """.    .  
-00008ec0: 2020 6361 6e64 6964 6174 6573 203d 2065    candidates = e
-00008ed0: 6461 7461 2e63 616e 6469 6461 7465 7320  data.candidates 
-00008ee0: 6966 2063 7572 725f 6361 6e64 7320 6973  if curr_cands is
-00008ef0: 204e 6f6e 6520 656c 7365 2063 7572 725f   None else curr_
-00008f00: 6361 6e64 7320 2020 200a 2020 2020 7374  cands    .    st
-00008f10: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-00008f20: 3d20 6564 6174 612e 6d61 7267 696e 2069  = edata.margin i
-00008f30: 6620 7374 7265 6e67 7468 5f66 756e 6374  f strength_funct
-00008f40: 696f 6e20 6973 204e 6f6e 6520 656c 7365  ion is None else
-00008f50: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00008f60: 6f6e 2020 2020 0a0a 2020 2020 775f 6564  on    ..    w_ed
-00008f70: 6765 7320 3d20 5b28 6331 2c20 6332 2c20  ges = [(c1, c2, 
-00008f80: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00008f90: 6e28 6331 2c20 6332 2929 2066 6f72 2063  n(c1, c2)) for c
-00008fa0: 3120 696e 2063 616e 6469 6461 7465 7320  1 in candidates 
-00008fb0: 666f 7220 6332 2069 6e20 6361 6e64 6964  for c2 in candid
-00008fc0: 6174 6573 2069 6620 6331 2021 3d20 6332  ates if c1 != c2
-00008fd0: 2061 6e64 2028 6564 6174 612e 6d61 6a6f   and (edata.majo
-00008fe0: 7269 7479 5f70 7265 6665 7273 2863 312c  rity_prefers(c1,
-00008ff0: 2063 3229 206f 7220 6564 6174 612e 6973   c2) or edata.is
-00009000: 5f74 6965 6428 6331 2c20 6332 2929 5d0a  _tied(c1, c2))].
-00009010: 2020 2020 7769 6e6e 6572 7320 3d20 6c69      winners = li
-00009020: 7374 2829 2020 2020 2020 2020 2020 2020  st()            
-00009030: 0a20 2020 2073 7472 656e 6774 6873 203d  .    strengths =
-00009040: 2073 6f72 7465 6428 6c69 7374 2873 6574   sorted(list(set
-00009050: 285b 655b 325d 2066 6f72 2065 2069 6e20  ([e[2] for e in 
-00009060: 775f 6564 6765 735d 2929 2c20 7265 7665  w_edges])), reve
-00009070: 7273 653d 5472 7565 290a 2020 2020 736f  rse=True).    so
-00009080: 7274 6564 5f65 6467 6573 203d 205b 5b65  rted_edges = [[e
-00009090: 2066 6f72 2065 2069 6e20 775f 6564 6765   for e in w_edge
-000090a0: 7320 6966 2065 5b32 5d20 3d3d 2073 5d20  s if e[2] == s] 
-000090b0: 666f 7220 7320 696e 2073 7472 656e 6774  for s in strengt
-000090c0: 6873 5d0a 2020 2020 7462 7320 3d20 7072  hs].    tbs = pr
-000090d0: 6f64 7563 7428 2a5b 7065 726d 7574 6174  oduct(*[permutat
-000090e0: 696f 6e73 2865 6467 6573 2920 666f 7220  ions(edges) for 
-000090f0: 6564 6765 7320 696e 2073 6f72 7465 645f  edges in sorted_
-00009100: 6564 6765 735d 290a 2020 2020 7270 5f64  edges]).    rp_d
-00009110: 6566 6561 7473 203d 206c 6973 7428 290a  efeats = list().
-00009120: 2020 2020 666f 7220 7462 2069 6e20 7462      for tb in tb
-00009130: 733a 0a20 2020 2020 2020 2065 6467 6573  s:.        edges
-00009140: 203d 2066 6c61 7474 656e 2874 6229 0a20   = flatten(tb). 
-00009150: 2020 2020 2020 2072 705f 6465 6665 6174         rp_defeat
-00009160: 203d 206e 782e 4469 4772 6170 6828 2920   = nx.DiGraph() 
-00009170: 0a20 2020 2020 2020 2066 6f72 2065 2069  .        for e i
-00009180: 6e20 6564 6765 733a 200a 2020 2020 2020  n edges: .      
-00009190: 2020 2020 2020 7270 5f64 6566 6561 742e        rp_defeat.
-000091a0: 6164 645f 6564 6765 2865 5b30 5d2c 2065  add_edge(e[0], e
-000091b0: 5b31 5d2c 2077 6569 6768 743d 655b 325d  [1], weight=e[2]
-000091c0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-000091d0: 2064 6f65 735f 6372 6561 7465 5f63 7963   does_create_cyc
-000091e0: 6c65 2872 705f 6465 6665 6174 2c20 6529  le(rp_defeat, e)
-000091f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009200: 2020 7270 5f64 6566 6561 742e 7265 6d6f    rp_defeat.remo
-00009210: 7665 5f65 6467 6528 655b 305d 2c20 655b  ve_edge(e[0], e[
-00009220: 315d 290a 2020 2020 2020 2020 7270 5f64  1]).        rp_d
-00009230: 6566 6561 7473 2e61 7070 656e 6428 7270  efeats.append(rp
-00009240: 5f64 6566 6561 7429 0a20 2020 2020 2020  _defeat).       
-00009250: 2077 696e 6e65 7273 2e61 7070 656e 6428   winners.append(
-00009260: 6d61 7869 6d61 6c5f 656c 656d 656e 7473  maximal_elements
-00009270: 2872 705f 6465 6665 6174 295b 305d 290a  (rp_defeat)[0]).
-00009280: 2020 2020 7265 7475 726e 2072 705f 6465      return rp_de
-00009290: 6665 6174 730a 0a0a 4076 6d28 6e61 6d65  feats...@vm(name
-000092a0: 3d22 5261 6e6b 6564 2050 6169 7273 2054  ="Ranked Pairs T
-000092b0: 4222 290a 6465 6620 7261 6e6b 6564 5f70  B").def ranked_p
-000092c0: 6169 7273 5f74 6228 0a20 2020 2065 6461  airs_tb(.    eda
-000092d0: 7461 2c20 0a20 2020 2063 7572 725f 6361  ta, .    curr_ca
-000092e0: 6e64 7320 3d20 4e6f 6e65 2c20 0a20 2020  nds = None, .   
-000092f0: 2074 6965 5f62 7265 616b 6572 203d 204e   tie_breaker = N
-00009300: 6f6e 652c 200a 2020 2020 7374 7265 6e67  one, .    streng
-00009310: 7468 5f66 756e 6374 696f 6e20 3d20 4e6f  th_function = No
-00009320: 6e65 293a 2020 200a 2020 2020 2222 220a  ne):   .    """.
-00009330: 2020 2020 5261 6e6b 6564 2050 6169 7273      Ranked Pairs
-00009340: 2077 6974 6820 6120 6669 7865 6420 6c69   with a fixed li
-00009350: 6e65 6172 206f 7264 6572 206f 6e20 7468  near order on th
-00009360: 6520 6361 6e64 6964 6174 6573 2074 6f20  e candidates to 
-00009370: 6272 6561 6b20 616e 7920 7469 6573 2069  break any ties i
-00009380: 6e20 7468 6520 6d61 7267 696e 732e 2020  n the margins.  
-00009390: 200a 2020 2020 5369 6e63 6520 7468 6520   .    Since the 
-000093a0: 7469 655f 6272 6561 6b65 7220 6973 2061  tie_breaker is a
-000093b0: 206c 696e 6561 7220 6f72 6465 722c 2074   linear order, t
-000093c0: 6869 7320 6d65 7468 6f64 2069 7320 7265  his method is re
-000093d0: 736f 6c75 7465 2e20 2020 0a0a 2020 2020  solute.   ..    
-000093e0: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-000093f0: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-00009400: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-00009410: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-00009420: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-00009430: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-00009440: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
-00009450: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
-00009460: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
-00009470: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
-00009480: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
-00009490: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
-000094a0: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
-000094b0: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
-000094c0: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
-000094d0: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
-000094e0: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
-000094f0: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
-00009500: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
-00009510: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
-00009520: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
-00009530: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
-00009540: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
-00009550: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
-00009560: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
-00009570: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
-00009580: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
-00009590: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
-000095a0: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
-000095b0: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
-000095c0: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
-000095d0: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
-000095e0: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
-000095f0: 202e 2e20 7365 6561 6c73 6f3a 3a0a 0a20   .. seealso::.. 
-00009600: 2020 2020 2020 203a 6d65 7468 3a60 7072         :meth:`pr
-00009610: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-00009620: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
-00009630: 616e 6b65 645f 7061 6972 7360 2c20 3a6d  anked_pairs`, :m
-00009640: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
-00009650: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-00009660: 7468 6f64 732e 7261 6e6b 6564 5f70 6169  thods.ranked_pai
-00009670: 7273 5f77 6974 685f 7465 7374 602c 203a  rs_with_test`, :
-00009680: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-00009690: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-000096a0: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
-000096b0: 6972 735f 6672 6f6d 5f73 7461 636b 7360  irs_from_stacks`
-000096c0: 0a0a 2020 2020 2e2e 2065 7865 635f 636f  ..    .. exec_co
-000096d0: 6465 3a3a 0a0a 2020 2020 2020 2020 6672  de::..        fr
-000096e0: 6f6d 2070 7265 665f 766f 7469 6e67 2e70  om pref_voting.p
-000096f0: 726f 6669 6c65 7320 696d 706f 7274 2050  rofiles import P
-00009700: 726f 6669 6c65 0a20 2020 2020 2020 2066  rofile.        f
-00009710: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
-00009720: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-00009730: 686f 6473 2069 6d70 6f72 7420 7261 6e6b  hods import rank
-00009740: 6564 5f70 6169 7273 5f66 726f 6d5f 7374  ed_pairs_from_st
-00009750: 6163 6b73 2c20 7261 6e6b 6564 5f70 6169  acks, ranked_pai
-00009760: 7273 5f74 622c 2072 616e 6b65 645f 7061  rs_tb, ranked_pa
-00009770: 6972 735f 7a74 0a0a 2020 2020 2020 2020  irs_zt..        
-00009780: 7072 6f66 203d 2050 726f 6669 6c65 285b  prof = Profile([
-00009790: 5b32 2c20 332c 2031 2c20 305d 2c20 5b30  [2, 3, 1, 0], [0
-000097a0: 2c20 332c 2031 2c20 325d 2c20 5b31 2c20  , 3, 1, 2], [1, 
-000097b0: 332c 2032 2c20 305d 2c20 5b32 2c20 312c  3, 2, 0], [2, 1,
-000097c0: 2033 2c20 305d 5d2c 205b 312c 2031 2c20   3, 0]], [1, 1, 
-000097d0: 312c 2031 5d29 0a0a 2020 2020 2020 2020  1, 1])..        
-000097e0: 7072 6f66 2e64 6973 706c 6179 2829 0a0a  prof.display()..
-000097f0: 2020 2020 2020 2020 7261 6e6b 6564 5f70          ranked_p
-00009800: 6169 7273 5f66 726f 6d5f 7374 6163 6b73  airs_from_stacks
-00009810: 2e64 6973 706c 6179 2870 726f 6629 0a20  .display(prof). 
-00009820: 2020 2020 2020 2072 616e 6b65 645f 7061         ranked_pa
-00009830: 6972 735f 7462 2e64 6973 706c 6179 2870  irs_tb.display(p
-00009840: 726f 6629 0a20 2020 2020 2020 2072 616e  rof).        ran
-00009850: 6b65 645f 7061 6972 735f 7462 2e64 6973  ked_pairs_tb.dis
-00009860: 706c 6179 2870 726f 662c 2074 6965 5f62  play(prof, tie_b
-00009870: 7265 616b 6572 203d 205b 332c 2032 2c20  reaker = [3, 2, 
-00009880: 312c 2030 5d29 0a20 2020 2020 2020 2072  1, 0]).        r
-00009890: 616e 6b65 645f 7061 6972 735f 7a74 2e64  anked_pairs_zt.d
-000098a0: 6973 706c 6179 2870 726f 6629 0a0a 2020  isplay(prof)..  
-000098b0: 2020 2222 220a 0a20 2020 2063 616e 6469    """..    candi
-000098c0: 6461 7465 7320 3d20 6564 6174 612e 6361  dates = edata.ca
-000098d0: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
-000098e0: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
-000098f0: 6c73 6520 6375 7272 5f63 616e 6473 2020  lse curr_cands  
-00009900: 2020 0a20 2020 2063 6964 785f 746f 5f63    .    cidx_to_c
-00009910: 616e 6420 3d20 7b63 6964 783a 2063 2066  and = {cidx: c f
-00009920: 6f72 2063 6964 782c 2063 2069 6e20 656e  or cidx, c in en
-00009930: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
-00009940: 6573 297d 2020 0a20 2020 2063 616e 645f  es)}  .    cand_
-00009950: 746f 5f63 6964 7820 3d20 7b63 3a20 6369  to_cidx = {c: ci
-00009960: 6478 2066 6f72 2063 6964 782c 2063 2069  dx for cidx, c i
-00009970: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
-00009980: 6964 6174 6573 297d 2020 0a0a 2020 2020  idates)}  ..    
-00009990: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-000099a0: 6e20 3d20 6564 6174 612e 6d61 7267 696e  n = edata.margin
-000099b0: 2069 6620 7374 7265 6e67 7468 5f66 756e   if strength_fun
-000099c0: 6374 696f 6e20 6973 204e 6f6e 6520 656c  ction is None el
-000099d0: 7365 2073 7472 656e 6774 685f 6675 6e63  se strength_func
-000099e0: 7469 6f6e 0a20 2020 200a 2020 2020 7462  tion.    .    tb
-000099f0: 5f72 616e 6b69 6e67 203d 2074 6965 5f62  _ranking = tie_b
-00009a00: 7265 616b 6572 2069 6620 7469 655f 6272  reaker if tie_br
-00009a10: 6561 6b65 7220 6973 206e 6f74 204e 6f6e  eaker is not Non
-00009a20: 6520 656c 7365 2073 6f72 7465 6428 6c69  e else sorted(li
-00009a30: 7374 2863 616e 6469 6461 7465 7329 290a  st(candidates)).
-00009a40: 0a20 2020 2063 7720 3d20 6564 6174 612e  .    cw = edata.
-00009a50: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
-00009a60: 2863 7572 725f 6361 6e64 733d 6375 7272  (curr_cands=curr
-00009a70: 5f63 616e 6473 290a 2020 2020 2320 5261  _cands).    # Ra
-00009a80: 6e6b 6564 2050 6169 7273 2069 7320 436f  nked Pairs is Co
-00009a90: 6e64 6f72 6365 7420 636f 6e73 6973 7465  ndorcet consiste
-00009aa0: 6e74 2c20 736f 2073 696d 706c 7920 7265  nt, so simply re
-00009ab0: 7475 726e 2074 6865 2043 6f6e 646f 7263  turn the Condorc
-00009ac0: 6574 2077 696e 6e65 7220 6966 2065 7869  et winner if exi
-00009ad0: 7374 730a 2020 2020 6966 2063 7720 6973  sts.    if cw is
-00009ae0: 206e 6f74 204e 6f6e 653a 200a 2020 2020   not None: .    
-00009af0: 2020 2020 7769 6e6e 6572 7320 3d20 5b63      winners = [c
-00009b00: 775d 0a20 2020 2065 6c73 653a 0a20 2020  w].    else:.   
-00009b10: 2020 2020 2077 5f65 6467 6573 203d 205b       w_edges = [
-00009b20: 2863 312c 2063 322c 2073 7472 656e 6774  (c1, c2, strengt
-00009b30: 685f 6675 6e63 7469 6f6e 2863 312c 2063  h_function(c1, c
-00009b40: 3229 2920 666f 7220 6331 2069 6e20 6361  2)) for c1 in ca
-00009b50: 6e64 6964 6174 6573 2066 6f72 2063 3220  ndidates for c2 
-00009b60: 696e 2063 616e 6469 6461 7465 7320 0a20  in candidates . 
-00009b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b80: 2020 6966 2063 3120 213d 2063 3220 616e    if c1 != c2 an
-00009b90: 6420 2865 6461 7461 2e6d 616a 6f72 6974  d (edata.majorit
-00009ba0: 795f 7072 6566 6572 7328 6331 2c20 6332  y_prefers(c1, c2
-00009bb0: 2920 6f72 2065 6461 7461 2e69 735f 7469  ) or edata.is_ti
-00009bc0: 6564 2863 312c 2063 3229 295d 0a20 2020  ed(c1, c2))].   
-00009bd0: 2020 2020 2077 696e 6e65 7273 203d 206c       winners = l
-00009be0: 6973 7428 2920 2020 2020 2020 2020 2020  ist()           
-00009bf0: 200a 2020 2020 2020 2020 7374 7265 6e67   .        streng
-00009c00: 7468 7320 3d20 736f 7274 6564 286c 6973  ths = sorted(lis
-00009c10: 7428 7365 7428 5b65 5b32 5d20 666f 7220  t(set([e[2] for 
-00009c20: 6520 696e 2077 5f65 6467 6573 5d29 292c  e in w_edges])),
-00009c30: 2072 6576 6572 7365 3d54 7275 6529 0a20   reverse=True). 
-00009c40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00009c50: 7270 5f64 6566 6561 7420 3d20 5350 4f28  rp_defeat = SPO(
-00009c60: 6c65 6e28 6361 6e64 6964 6174 6573 2929  len(candidates))
-00009c70: 0a0a 2020 2020 2020 2020 666f 7220 7320  ..        for s 
-00009c80: 696e 2073 7472 656e 6774 6873 3a20 0a20  in strengths: . 
-00009c90: 2020 2020 2020 2020 2020 2065 6467 6573             edges
-00009ca0: 203d 205b 6520 666f 7220 6520 696e 2077   = [e for e in w
-00009cb0: 5f65 6467 6573 2069 6620 655b 325d 203d  _edges if e[2] =
-00009cc0: 3d20 735d 0a20 2020 2020 2020 2020 2020  = s].           
-00009cd0: 200a 2020 2020 2020 2020 2020 2020 2320   .            # 
-00009ce0: 6272 6561 6b20 7469 6573 2075 7369 6e67  break ties using
-00009cf0: 2074 6865 206c 6578 6963 6f67 7261 7068   the lexicograph
-00009d00: 6963 206f 7264 6572 696e 6720 6f6e 2074  ic ordering on t
-00009d10: 7570 6c65 7320 6769 7665 6e20 7462 5f72  uples given tb_r
-00009d20: 616e 6b69 6e67 0a20 2020 2020 2020 2020  anking.         
-00009d30: 2020 2073 6f72 7465 645f 6564 6765 7320     sorted_edges 
-00009d40: 3d20 736f 7274 6564 2865 6467 6573 2c20  = sorted(edges, 
-00009d50: 6b65 7920 3d20 6c61 6d62 6461 2065 3a20  key = lambda e: 
-00009d60: 2874 625f 7261 6e6b 696e 672e 696e 6465  (tb_ranking.inde
-00009d70: 7828 655b 305d 292c 2074 625f 7261 6e6b  x(e[0]), tb_rank
-00009d80: 696e 672e 696e 6465 7828 655b 315d 2929  ing.index(e[1]))
-00009d90: 2c20 7265 7665 7273 653d 4661 6c73 6529  , reverse=False)
-00009da0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00009db0: 2065 302c 6531 2c73 2069 6e20 6564 6765   e0,e1,s in edge
-00009dc0: 733a 200a 2020 2020 2020 2020 2020 2020  s: .            
-00009dd0: 2020 2020 6966 206e 6f74 2072 705f 6465      if not rp_de
-00009de0: 6665 6174 2e50 5b63 616e 645f 746f 5f63  feat.P[cand_to_c
-00009df0: 6964 785b 6531 5d5d 5b63 616e 645f 746f  idx[e1]][cand_to
-00009e00: 5f63 6964 785b 6530 5d5d 3a0a 2020 2020  _cidx[e0]]:.    
-00009e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e20: 7270 5f64 6566 6561 742e 6164 6428 6361  rp_defeat.add(ca
-00009e30: 6e64 5f74 6f5f 6369 6478 5b65 305d 2c63  nd_to_cidx[e0],c
-00009e40: 616e 645f 746f 5f63 6964 785b 6531 5d29  and_to_cidx[e1])
-00009e50: 0a20 2020 2020 2020 2020 2020 2077 696e  .            win
-00009e60: 6e65 7273 2e61 7070 656e 6428 6369 6478  ners.append(cidx
-00009e70: 5f74 6f5f 6361 6e64 5b72 705f 6465 6665  _to_cand[rp_defe
-00009e80: 6174 2e69 6e69 7469 616c 5f65 6c65 6d65  at.initial_eleme
-00009e90: 6e74 7328 295b 305d 5d29 0a0a 2020 2020  nts()[0]])..    
-00009ea0: 7265 7475 726e 2073 6f72 7465 6428 6c69  return sorted(li
-00009eb0: 7374 2873 6574 2877 696e 6e65 7273 2929  st(set(winners))
-00009ec0: 290a 0a0a 4076 6d28 6e61 6d65 3d22 5261  )...@vm(name="Ra
-00009ed0: 6e6b 6564 2050 6169 7273 205a 5422 290a  nked Pairs ZT").
-00009ee0: 6465 6620 7261 6e6b 6564 5f70 6169 7273  def ranked_pairs
-00009ef0: 5f7a 7428 0a20 2020 2070 726f 6669 6c65  _zt(.    profile
-00009f00: 2c20 0a20 2020 2063 7572 725f 6361 6e64  , .    curr_cand
-00009f10: 7320 3d20 4e6f 6e65 2c20 0a20 2020 2073  s = None, .    s
-00009f20: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00009f30: 203d 204e 6f6e 6529 3a20 2020 0a20 2020   = None):   .   
-00009f40: 2022 2222 5261 6e6b 6564 2070 6169 7273   """Ranked pairs
-00009f50: 2077 6865 7265 2061 2066 6978 6564 2076   where a fixed v
-00009f60: 6f74 6572 2062 7265 616b 7320 616e 7920  oter breaks any 
-00009f70: 7469 6573 2069 6e20 7468 6520 6d61 7267  ties in the marg
-00009f80: 696e 732e 2020 4974 2069 7320 616c 7761  ins.  It is alwa
-00009f90: 7973 2074 6865 2076 6f74 6572 2069 6e20  ys the voter in 
-00009fa0: 706f 7369 7469 6f6e 2030 2074 6861 7420  position 0 that 
-00009fb0: 6272 6561 6b73 2074 6865 2074 6965 732e  breaks the ties.
-00009fc0: 2020 5369 6e63 6520 766f 7465 7273 2068    Since voters h
-00009fd0: 6176 6520 7374 7269 6374 2070 7265 6665  ave strict prefe
-00009fe0: 7265 6e63 6573 2c20 7468 6973 206d 6574  rences, this met
-00009ff0: 686f 6420 6973 2072 6573 6f6c 7574 652e  hod is resolute.
-0000a000: 2020 5468 6973 2069 7320 6b6e 6f77 6e20    This is known 
-0000a010: 6173 2052 616e 6b65 6420 5061 6972 7320  as Ranked Pairs 
-0000a020: 5a54 2c20 666f 7220 5a61 7669 7374 2054  ZT, for Zavist T
-0000a030: 6964 656d 616e 2e0a 0a20 2020 2041 7267  ideman...    Arg
-0000a040: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
-0000a050: 2028 5072 6f66 696c 6529 3a20 4120 7072   (Profile): A pr
-0000a060: 6f66 696c 6520 6f66 206c 696e 6561 7220  ofile of linear 
-0000a070: 6f72 6465 7273 0a20 2020 2020 2020 2063  orders.        c
-0000a080: 7572 725f 6361 6e64 7320 284c 6973 745b  urr_cands (List[
-0000a090: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
-0000a0a0: 2049 6620 7365 742c 2074 6865 6e20 6669   If set, then fi
-0000a0b0: 6e64 2074 6865 2077 696e 6e65 7273 2066  nd the winners f
-0000a0c0: 6f72 2074 6865 2070 726f 6669 6c65 2072  or the profile r
-0000a0d0: 6573 7472 6963 7465 6420 746f 2074 6865  estricted to the
-0000a0e0: 2063 616e 6469 6461 7465 7320 696e 2060   candidates in `
-0000a0f0: 6063 7572 725f 6361 6e64 7360 600a 0a20  `curr_cands``.. 
-0000a100: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
-0000a110: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
-0000a120: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
-0000a130: 2e20 0a0a 2020 2020 2e2e 2073 6565 616c  . ..    .. seeal
-0000a140: 736f 3a3a 0a0a 2020 2020 2020 2020 3a6d  so::..        :m
-0000a150: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
-0000a160: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-0000a170: 7468 6f64 732e 7261 6e6b 6564 5f70 6169  thods.ranked_pai
-0000a180: 7273 602c 203a 6d65 7468 3a60 7072 6566  rs`, :meth:`pref
-0000a190: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
-0000a1a0: 6173 6564 5f6d 6574 686f 6473 2e72 616e  ased_methods.ran
-0000a1b0: 6b65 645f 7061 6972 735f 7769 7468 5f74  ked_pairs_with_t
-0000a1c0: 6573 7460 2c20 3a6d 6574 683a 6070 7265  est`, :meth:`pre
-0000a1d0: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
-0000a1e0: 6261 7365 645f 6d65 7468 6f64 732e 7261  based_methods.ra
-0000a1f0: 6e6b 6564 5f70 6169 7273 5f66 726f 6d5f  nked_pairs_from_
-0000a200: 7374 6163 6b73 600a 0a20 2020 202e 2e20  stacks`..    .. 
-0000a210: 6578 6563 5f63 6f64 653a 3a0a 0a20 2020  exec_code::..   
-0000a220: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-0000a230: 6f74 696e 672e 7072 6f66 696c 6573 2069  oting.profiles i
-0000a240: 6d70 6f72 7420 5072 6f66 696c 650a 2020  mport Profile.  
-0000a250: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
-0000a260: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-0000a270: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
-0000a280: 7274 2072 616e 6b65 645f 7061 6972 735f  rt ranked_pairs_
-0000a290: 6672 6f6d 5f73 7461 636b 732c 2072 616e  from_stacks, ran
-0000a2a0: 6b65 645f 7061 6972 735f 7462 2c20 7261  ked_pairs_tb, ra
-0000a2b0: 6e6b 6564 5f70 6169 7273 5f7a 740a 0a20  nked_pairs_zt.. 
-0000a2c0: 2020 2020 2020 2070 726f 6620 3d20 5072         prof = Pr
-0000a2d0: 6f66 696c 6528 5b5b 322c 2033 2c20 312c  ofile([[2, 3, 1,
-0000a2e0: 2030 5d2c 205b 302c 2033 2c20 312c 2032   0], [0, 3, 1, 2
-0000a2f0: 5d2c 205b 312c 2033 2c20 322c 2030 5d2c  ], [1, 3, 2, 0],
-0000a300: 205b 322c 2031 2c20 332c 2030 5d5d 2c20   [2, 1, 3, 0]], 
-0000a310: 5b31 2c20 312c 2031 2c20 315d 290a 0a20  [1, 1, 1, 1]).. 
-0000a320: 2020 2020 2020 2070 726f 662e 6469 7370         prof.disp
-0000a330: 6c61 7928 290a 0a20 2020 2020 2020 2072  lay()..        r
-0000a340: 616e 6b65 645f 7061 6972 735f 6672 6f6d  anked_pairs_from
-0000a350: 5f73 7461 636b 732e 6469 7370 6c61 7928  _stacks.display(
-0000a360: 7072 6f66 290a 2020 2020 2020 2020 7261  prof).        ra
-0000a370: 6e6b 6564 5f70 6169 7273 5f74 622e 6469  nked_pairs_tb.di
-0000a380: 7370 6c61 7928 7072 6f66 290a 2020 2020  splay(prof).    
-0000a390: 2020 2020 7261 6e6b 6564 5f70 6169 7273      ranked_pairs
-0000a3a0: 5f74 622e 6469 7370 6c61 7928 7072 6f66  _tb.display(prof
-0000a3b0: 2c20 7469 655f 6272 6561 6b65 7220 3d20  , tie_breaker = 
-0000a3c0: 5b33 2c20 322c 2031 2c20 305d 290a 2020  [3, 2, 1, 0]).  
-0000a3d0: 2020 2020 2020 7261 6e6b 6564 5f70 6169        ranked_pai
-0000a3e0: 7273 5f7a 742e 6469 7370 6c61 7928 7072  rs_zt.display(pr
-0000a3f0: 6f66 290a 0a20 2020 200a 2020 2020 2222  of)..    .    ""
-0000a400: 220a 2020 2020 6361 6e64 6964 6174 6573  ".    candidates
-0000a410: 203d 2070 726f 6669 6c65 2e63 616e 6469   = profile.candi
-0000a420: 6461 7465 7320 6966 2063 7572 725f 6361  dates if curr_ca
-0000a430: 6e64 7320 6973 204e 6f6e 6520 656c 7365  nds is None else
-0000a440: 2063 7572 725f 6361 6e64 7320 2020 200a   curr_cands    .
-0000a450: 2020 2020 0a20 2020 2023 2074 6865 2074      .    # the t
-0000a460: 6965 2d62 7265 616b 6572 2069 7320 616c  ie-breaker is al
-0000a470: 7761 7973 2074 6865 2066 6972 7374 2076  ways the first v
-0000a480: 6f74 6572 2e20 0a20 2020 2074 625f 7261  oter. .    tb_ra
-0000a490: 6e6b 696e 6720 3d20 7475 706c 6528 5b63  nking = tuple([c
-0000a4a0: 2066 6f72 2063 2069 6e20 6c69 7374 2870   for c in list(p
-0000a4b0: 726f 6669 6c65 2e5f 7261 6e6b 696e 6773  rofile._rankings
-0000a4c0: 5b30 5d29 2069 6620 6320 696e 2063 616e  [0]) if c in can
-0000a4d0: 6469 6461 7465 735d 290a 2020 2020 0a20  didates]).    . 
-0000a4e0: 2020 2072 6574 7572 6e20 7261 6e6b 6564     return ranked
-0000a4f0: 5f70 6169 7273 5f74 6228 7072 6f66 696c  _pairs_tb(profil
-0000a500: 652c 2063 7572 725f 6361 6e64 7320 3d20  e, curr_cands = 
-0000a510: 6375 7272 5f63 616e 6473 2c20 7469 655f  curr_cands, tie_
-0000a520: 6272 6561 6b65 7220 3d20 7462 5f72 616e  breaker = tb_ran
-0000a530: 6b69 6e67 2c20 7374 7265 6e67 7468 5f66  king, strength_f
-0000a540: 756e 6374 696f 6e20 3d20 7374 7265 6e67  unction = streng
-0000a550: 7468 5f66 756e 6374 696f 6e29 0a0a 0a40  th_function)...@
-0000a560: 766d 286e 616d 653d 2252 6976 6572 2229  vm(name="River")
-0000a570: 0a64 6566 2072 6976 6572 2865 6461 7461  .def river(edata
-0000a580: 2c20 6375 7272 5f63 616e 6473 203d 204e  , curr_cands = N
-0000a590: 6f6e 652c 2073 7472 656e 6774 685f 6675  one, strength_fu
-0000a5a0: 6e63 7469 6f6e 203d 204e 6f6e 6529 3a20  nction = None): 
-0000a5b0: 2020 0a20 2020 2022 2222 0a20 2020 204f    .    """.    O
-0000a5c0: 7264 6572 2074 6865 2065 6467 6573 2069  rder the edges i
-0000a5d0: 6e20 7468 6520 7765 616b 206d 6172 6769  n the weak margi
-0000a5e0: 6e20 6772 6170 6820 6672 6f6d 206c 6172  n graph from lar
-0000a5f0: 6765 7374 2074 6f20 736d 616c 6c65 7374  gest to smallest
-0000a600: 2061 6e64 206c 6f63 6b20 7468 656d 2069   and lock them i
-0000a610: 6e20 696e 2074 6861 7420 6f72 6465 722c  n in that order,
-0000a620: 2073 6b69 7070 696e 6720 6564 6765 7320   skipping edges 
-0000a630: 7468 6174 2063 7265 6174 6520 6120 6379  that create a cy
-0000a640: 636c 6520 2a61 6e64 2065 6467 6573 2069  cle *and edges i
-0000a650: 6e20 7768 6963 6820 7468 6572 6520 6973  n which there is
-0000a660: 2061 6c72 6561 6479 2061 6e20 6564 6765   already an edge
-0000a670: 2070 6f69 6e74 696e 6720 746f 2074 6865   pointing to the
-0000a680: 2074 6172 6765 742a 2e20 2042 7265 616b   target*.  Break
-0000a690: 2074 6965 7320 7573 696e 6720 6120 7469   ties using a ti
-0000a6a0: 652d 6272 6561 6b69 6e67 2020 6c69 6e65  e-breaking  line
-0000a6b0: 6172 206f 7264 6572 696e 6720 6f76 6572  ar ordering over
-0000a6c0: 2074 6865 2065 6467 6573 2e20 2041 2063   the edges.  A c
-0000a6d0: 616e 6469 6461 7465 2069 7320 6120 5269  andidate is a Ri
-0000a6e0: 7665 7220 7769 6e6e 6572 2069 6620 6974  ver winner if it
-0000a6f0: 2077 696e 7320 6163 636f 7264 696e 6720   wins according 
-0000a700: 746f 2073 6f6d 6520 7469 652d 6272 6561  to some tie-brea
-0000a710: 6b69 6e67 2072 756c 652e 2053 6565 2068  king rule. See h
-0000a720: 7474 7073 3a2f 2f65 6c65 6374 6f77 696b  ttps://electowik
-0000a730: 692e 6f72 672f 7769 6b69 2f52 6976 6572  i.org/wiki/River
-0000a740: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-0000a750: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-0000a760: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-0000a770: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-0000a780: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-0000a790: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-0000a7a0: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
-0000a7b0: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
-0000a7c0: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
-0000a7d0: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
-0000a7e0: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
-0000a7f0: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
-0000a800: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
-0000a810: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
-0000a820: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
-0000a830: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
-0000a840: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-0000a850: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
-0000a860: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
-0000a870: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
-0000a880: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
-0000a890: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
-0000a8a0: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
-0000a8b0: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
-0000a8c0: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
-0000a8d0: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
-0000a8e0: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
-0000a8f0: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
-0000a900: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
-0000a910: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
-0000a920: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
-0000a930: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
-0000a940: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
-0000a950: 2e20 0a0a 2020 2020 3a45 7861 6d70 6c65  . ..    :Example
-0000a960: 3a20 0a0a 2020 2020 2e2e 2065 7865 635f  : ..    .. exec_
-0000a970: 636f 6465 3a3a 200a 0a20 2020 2020 2020  code:: ..       
-0000a980: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
-0000a990: 672e 7765 6967 6874 6564 5f6d 616a 6f72  g.weighted_major
-0000a9a0: 6974 795f 6772 6170 6873 2069 6d70 6f72  ity_graphs impor
-0000a9b0: 7420 4d61 7267 696e 4772 6170 680a 2020  t MarginGraph.  
-0000a9c0: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
-0000a9d0: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-0000a9e0: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
-0000a9f0: 7274 2072 6976 6572 2c20 7261 6e6b 6564  rt river, ranked
-0000aa00: 5f70 6169 7273 0a20 2020 2020 2020 200a  _pairs.        .
-0000aa10: 2020 2020 2020 2020 6d67 203d 204d 6172          mg = Mar
-0000aa20: 6769 6e47 7261 7068 285b 302c 2031 2c20  ginGraph([0, 1, 
-0000aa30: 322c 2033 5d2c 205b 2830 2c20 322c 2032  2, 3], [(0, 2, 2
-0000aa40: 292c 2028 302c 2033 2c20 3829 2c20 2831  ), (0, 3, 8), (1
-0000aa50: 2c20 302c 2031 3229 2c20 2832 2c20 332c  , 0, 12), (2, 3,
-0000aa60: 2031 3229 2c20 2833 2c20 312c 2036 295d   12), (3, 1, 6)]
-0000aa70: 290a 0a20 2020 2020 2020 2072 616e 6b65  )..        ranke
-0000aa80: 645f 7061 6972 732e 6469 7370 6c61 7928  d_pairs.display(
-0000aa90: 6d67 290a 2020 2020 2020 2020 7269 7665  mg).        rive
-0000aaa0: 722e 6469 7370 6c61 7928 6d67 290a 0a20  r.display(mg).. 
-0000aab0: 2020 2022 2222 0a20 2020 2063 616e 6469     """.    candi
-0000aac0: 6461 7465 7320 3d20 6564 6174 612e 6361  dates = edata.ca
-0000aad0: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
-0000aae0: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
-0000aaf0: 6c73 6520 6375 7272 5f63 616e 6473 2020  lse curr_cands  
-0000ab00: 2020 0a20 2020 2063 6964 785f 746f 5f63    .    cidx_to_c
-0000ab10: 616e 6420 3d20 7b63 6964 783a 2063 2066  and = {cidx: c f
-0000ab20: 6f72 2063 6964 782c 2063 2069 6e20 656e  or cidx, c in en
-0000ab30: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
-0000ab40: 6573 297d 2020 0a20 2020 2063 616e 645f  es)}  .    cand_
-0000ab50: 746f 5f63 6964 7820 3d20 7b63 3a20 6369  to_cidx = {c: ci
-0000ab60: 6478 2066 6f72 2063 6964 782c 2063 2069  dx for cidx, c i
-0000ab70: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
-0000ab80: 6964 6174 6573 297d 2020 0a0a 2020 2020  idates)}  ..    
-0000ab90: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000aba0: 6e20 3d20 6564 6174 612e 6d61 7267 696e  n = edata.margin
-0000abb0: 2069 6620 7374 7265 6e67 7468 5f66 756e   if strength_fun
-0000abc0: 6374 696f 6e20 6973 204e 6f6e 6520 656c  ction is None el
-0000abd0: 7365 2073 7472 656e 6774 685f 6675 6e63  se strength_func
-0000abe0: 7469 6f6e 2020 2020 0a0a 2020 2020 6377  tion    ..    cw
-0000abf0: 203d 2065 6461 7461 2e63 6f6e 646f 7263   = edata.condorc
-0000ac00: 6574 5f77 696e 6e65 7228 6375 7272 5f63  et_winner(curr_c
-0000ac10: 616e 6473 3d63 7572 725f 6361 6e64 7329  ands=curr_cands)
-0000ac20: 0a20 2020 2023 2052 616e 6b65 6420 5061  .    # Ranked Pa
-0000ac30: 6972 7320 6973 2043 6f6e 646f 7263 6574  irs is Condorcet
-0000ac40: 2063 6f6e 7369 7374 656e 742c 2073 6f20   consistent, so 
-0000ac50: 7369 6d70 6c79 2072 6574 7572 6e20 7468  simply return th
-0000ac60: 6520 436f 6e64 6f72 6365 7420 7769 6e6e  e Condorcet winn
-0000ac70: 6572 2069 6620 6578 6973 7473 0a20 2020  er if exists.   
-0000ac80: 2069 6620 6377 2069 7320 6e6f 7420 4e6f   if cw is not No
-0000ac90: 6e65 3a20 0a20 2020 2020 2020 2077 696e  ne: .        win
-0000aca0: 6e65 7273 203d 205b 6377 5d0a 2020 2020  ners = [cw].    
-0000acb0: 656c 7365 3a0a 2020 2020 2020 2020 775f  else:.        w_
-0000acc0: 6564 6765 7320 3d20 5b28 6331 2c20 6332  edges = [(c1, c2
-0000acd0: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
-0000ace0: 696f 6e28 6331 2c20 6332 2929 2066 6f72  ion(c1, c2)) for
-0000acf0: 2063 3120 696e 2063 616e 6469 6461 7465   c1 in candidate
-0000ad00: 7320 666f 7220 6332 2069 6e20 6361 6e64  s for c2 in cand
-0000ad10: 6964 6174 6573 200a 2020 2020 2020 2020  idates .        
-0000ad20: 2020 2020 2020 2020 2020 2069 6620 6331             if c1
-0000ad30: 2021 3d20 6332 2061 6e64 2028 6564 6174   != c2 and (edat
-0000ad40: 612e 6d61 6a6f 7269 7479 5f70 7265 6665  a.majority_prefe
-0000ad50: 7273 2863 312c 2063 3229 206f 7220 6564  rs(c1, c2) or ed
-0000ad60: 6174 612e 6973 5f74 6965 6428 6331 2c20  ata.is_tied(c1, 
-0000ad70: 6332 2929 5d0a 2020 2020 2020 2020 7769  c2))].        wi
-0000ad80: 6e6e 6572 7320 3d20 6c69 7374 2829 2020  nners = list()  
-0000ad90: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-0000ada0: 2020 2073 7472 656e 6774 6873 203d 2073     strengths = s
-0000adb0: 6f72 7465 6428 6c69 7374 2873 6574 285b  orted(list(set([
-0000adc0: 655b 325d 2066 6f72 2065 2069 6e20 775f  e[2] for e in w_
-0000add0: 6564 6765 735d 2929 2c20 7265 7665 7273  edges])), revers
-0000ade0: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
-0000adf0: 736f 7274 6564 5f65 6467 6573 203d 205b  sorted_edges = [
-0000ae00: 5b65 2066 6f72 2065 2069 6e20 775f 6564  [e for e in w_ed
-0000ae10: 6765 7320 6966 2065 5b32 5d20 3d3d 2073  ges if e[2] == s
-0000ae20: 5d20 666f 7220 7320 696e 2073 7472 656e  ] for s in stren
-0000ae30: 6774 6873 5d0a 2020 2020 2020 2020 7462  gths].        tb
-0000ae40: 7320 3d20 7072 6f64 7563 7428 2a5b 7065  s = product(*[pe
-0000ae50: 726d 7574 6174 696f 6e73 2865 6467 6573  rmutations(edges
-0000ae60: 2920 666f 7220 6564 6765 7320 696e 2073  ) for edges in s
-0000ae70: 6f72 7465 645f 6564 6765 735d 290a 2020  orted_edges]).  
-0000ae80: 2020 2020 2020 666f 7220 7462 2069 6e20        for tb in 
-0000ae90: 7462 733a 0a20 2020 2020 2020 2020 2020  tbs:.           
-0000aea0: 2065 6467 6573 203d 2066 6c61 7474 656e   edges = flatten
-0000aeb0: 2874 6229 0a20 2020 2020 2020 2020 2020  (tb).           
-0000aec0: 2072 765f 6465 6665 6174 203d 2053 504f   rv_defeat = SPO
-0000aed0: 286c 656e 2863 616e 6469 6461 7465 7329  (len(candidates)
-0000aee0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-0000aef0: 7220 6530 2c65 312c 7320 696e 2065 6467  r e0,e1,s in edg
-0000af00: 6573 3a20 0a20 2020 2020 2020 2020 2020  es: .           
-0000af10: 2020 2020 2069 6620 6e6f 7420 7276 5f64       if not rv_d
-0000af20: 6566 6561 742e 505b 6361 6e64 5f74 6f5f  efeat.P[cand_to_
-0000af30: 6369 6478 5b65 315d 5d5b 6361 6e64 5f74  cidx[e1]][cand_t
-0000af40: 6f5f 6369 6478 5b65 305d 5d20 616e 6420  o_cidx[e0]] and 
-0000af50: 6c65 6e28 7276 5f64 6566 6561 742e 7072  len(rv_defeat.pr
-0000af60: 6564 735b 6361 6e64 5f74 6f5f 6369 6478  eds[cand_to_cidx
-0000af70: 5b65 315d 5d29 203d 3d20 303a 0a20 2020  [e1]]) == 0:.   
-0000af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af90: 2072 765f 6465 6665 6174 2e61 6464 2863   rv_defeat.add(c
-0000afa0: 616e 645f 746f 5f63 6964 785b 6530 5d2c  and_to_cidx[e0],
-0000afb0: 6361 6e64 5f74 6f5f 6369 6478 5b65 315d  cand_to_cidx[e1]
-0000afc0: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
-0000afd0: 6e6e 6572 732e 6170 7065 6e64 2863 6964  nners.append(cid
-0000afe0: 785f 746f 5f63 616e 645b 7276 5f64 6566  x_to_cand[rv_def
-0000aff0: 6561 742e 696e 6974 6961 6c5f 656c 656d  eat.initial_elem
-0000b000: 656e 7473 2829 5b30 5d5d 290a 0a20 2020  ents()[0]])..   
-0000b010: 2072 6574 7572 6e20 736f 7274 6564 286c   return sorted(l
-0000b020: 6973 7428 7365 7428 7769 6e6e 6572 7329  ist(set(winners)
-0000b030: 2929 0a0a 6465 6620 7269 7665 725f 6465  ))..def river_de
-0000b040: 6665 6174 7328 6564 6174 612c 2063 7572  feats(edata, cur
-0000b050: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
-0000b060: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000b070: 6e20 3d20 4e6f 6e65 293a 0a20 2020 2022  n = None):.    "
-0000b080: 2222 0a20 2020 2052 6574 7572 6e73 2074  "".    Returns t
-0000b090: 6865 2052 6976 6572 2064 6566 6561 7420  he River defeat 
-0000b0a0: 7265 6c61 7469 6f6e 7320 7072 6f64 7563  relations produc
-0000b0b0: 6564 2062 7920 7468 6520 5269 7665 7220  ed by the River 
-0000b0c0: 616c 676f 7269 7468 6d2e 0a0a 2020 2020  algorithm...    
-0000b0d0: 2e2e 2069 6d70 6f72 7461 6e74 3a3a 0a20  .. important::. 
-0000b0e0: 2020 2020 2020 2055 6e6c 696b 6520 7468         Unlike th
-0000b0f0: 6520 6f74 6865 7220 6675 6e63 7469 6f6e  e other function
-0000b100: 7320 7468 6174 2072 6574 7572 6e20 6120  s that return a 
-0000b110: 7369 6e67 6c65 2064 6566 6561 7420 7265  single defeat re
-0000b120: 6c61 7469 6f6e 2c20 7468 6973 2072 6574  lation, this ret
-0000b130: 7572 6e73 2061 206c 6973 7420 6f66 2064  urns a list of d
-0000b140: 6566 6561 7420 7265 6c61 7469 6f6e 732e  efeat relations.
-0000b150: 200a 2020 2020 2020 2020 0a20 2020 2041   .        .    A
-0000b160: 7267 733a 0a20 2020 2020 2020 2065 6461  rgs:.        eda
-0000b170: 7461 2028 5072 6f66 696c 652c 2050 726f  ta (Profile, Pro
-0000b180: 6669 6c65 5769 7468 5469 6573 2c20 4d61  fileWithTies, Ma
-0000b190: 7267 696e 4772 6170 6829 3a20 416e 7920  rginGraph): Any 
-0000b1a0: 656c 6563 7469 6f6e 2064 6174 6120 7468  election data th
-0000b1b0: 6174 2068 6173 2061 2060 6d61 7267 696e  at has a `margin
-0000b1c0: 6020 6d65 7468 6f64 2e20 0a20 2020 2020  ` method. .     
-0000b1d0: 2020 2063 7572 725f 6361 6e64 7320 284c     curr_cands (L
-0000b1e0: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
-0000b1f0: 616c 293a 2049 6620 7365 742c 2074 6865  al): If set, the
-0000b200: 6e20 6669 6e64 2074 6865 2077 696e 6e65  n find the winne
-0000b210: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
-0000b220: 6c65 2072 6573 7472 6963 7465 6420 746f  le restricted to
-0000b230: 2074 6865 2063 616e 6469 6461 7465 7320   the candidates 
-0000b240: 696e 2060 6063 7572 725f 6361 6e64 7360  in ``curr_cands`
-0000b250: 600a 2020 2020 2020 2020 7374 7265 6e67  `.        streng
-0000b260: 7468 5f66 756e 6374 696f 6e20 2866 756e  th_function (fun
-0000b270: 6374 696f 6e2c 206f 7074 696f 6e61 6c29  ction, optional)
-0000b280: 3a20 5468 6520 7374 7265 6e67 7468 2066  : The strength f
-0000b290: 756e 6374 696f 6e20 746f 2062 6520 7573  unction to be us
-0000b2a0: 6564 2074 6f20 6361 6c63 756c 6174 6520  ed to calculate 
-0000b2b0: 7468 6520 7374 7265 6e67 7468 206f 6620  the strength of 
-0000b2c0: 6120 7061 7468 2e20 2020 5468 6520 6465  a path.   The de
-0000b2d0: 6661 756c 7420 6973 2074 6865 206d 6172  fault is the mar
-0000b2e0: 6769 6e20 6d65 7468 6f64 206f 6620 6060  gin method of ``
-0000b2f0: 6564 6174 6160 602e 2020 2054 6869 7320  edata``.   This 
-0000b300: 6f6e 6c79 206d 6174 7465 7273 2077 6865  only matters whe
-0000b310: 6e20 7468 6520 6261 6c6c 6f74 7320 6172  n the ballots ar
-0000b320: 6520 6e6f 7420 6c69 6e65 6172 206f 7264  e not linear ord
-0000b330: 6572 732e 200a 0a20 2020 2052 6574 7572  ers. ..    Retur
-0000b340: 6e73 3a20 0a20 2020 2020 2020 2041 206e  ns: .        A n
-0000b350: 6574 776f 726b 7820 4469 4772 6170 6820  etworkx DiGraph 
-0000b360: 7265 7072 6573 656e 7469 6e67 2074 6865  representing the
-0000b370: 2052 6976 6572 2064 6566 6561 7420 7265   River defeat re
-0000b380: 6c61 7469 6f6e 2e20 0a20 2020 2022 2222  lation. .    """
-0000b390: 0a0a 2020 2020 6361 6e64 6964 6174 6573  ..    candidates
-0000b3a0: 203d 2065 6461 7461 2e63 616e 6469 6461   = edata.candida
-0000b3b0: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
-0000b3c0: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
-0000b3d0: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
-0000b3e0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-0000b3f0: 696f 6e20 3d20 6564 6174 612e 6d61 7267  ion = edata.marg
-0000b400: 696e 2069 6620 7374 7265 6e67 7468 5f66  in if strength_f
-0000b410: 756e 6374 696f 6e20 6973 204e 6f6e 6520  unction is None 
-0000b420: 656c 7365 2073 7472 656e 6774 685f 6675  else strength_fu
-0000b430: 6e63 7469 6f6e 2020 2020 0a0a 2020 2020  nction    ..    
-0000b440: 775f 6564 6765 7320 3d20 5b28 6331 2c20  w_edges = [(c1, 
-0000b450: 6332 2c20 7374 7265 6e67 7468 5f66 756e  c2, strength_fun
-0000b460: 6374 696f 6e28 6331 2c20 6332 2929 2066  ction(c1, c2)) f
-0000b470: 6f72 2063 3120 696e 2063 616e 6469 6461  or c1 in candida
-0000b480: 7465 7320 666f 7220 6332 2069 6e20 6361  tes for c2 in ca
-0000b490: 6e64 6964 6174 6573 2069 6620 6331 2021  ndidates if c1 !
-0000b4a0: 3d20 6332 2061 6e64 2028 6564 6174 612e  = c2 and (edata.
-0000b4b0: 6d61 6a6f 7269 7479 5f70 7265 6665 7273  majority_prefers
-0000b4c0: 2863 312c 2063 3229 206f 7220 6564 6174  (c1, c2) or edat
-0000b4d0: 612e 6973 5f74 6965 6428 6331 2c20 6332  a.is_tied(c1, c2
-0000b4e0: 2929 5d0a 0a20 2020 2073 7472 656e 6774  ))]..    strengt
-0000b4f0: 6873 203d 2073 6f72 7465 6428 6c69 7374  hs = sorted(list
-0000b500: 2873 6574 285b 655b 325d 2066 6f72 2065  (set([e[2] for e
-0000b510: 2069 6e20 775f 6564 6765 735d 2929 2c20   in w_edges])), 
-0000b520: 7265 7665 7273 653d 5472 7565 290a 2020  reverse=True).  
-0000b530: 2020 736f 7274 6564 5f65 6467 6573 203d    sorted_edges =
-0000b540: 205b 5b65 2066 6f72 2065 2069 6e20 775f   [[e for e in w_
-0000b550: 6564 6765 7320 6966 2065 5b32 5d20 3d3d  edges if e[2] ==
-0000b560: 2073 5d20 666f 7220 7320 696e 2073 7472   s] for s in str
-0000b570: 656e 6774 6873 5d0a 2020 2020 7462 7320  engths].    tbs 
-0000b580: 3d20 7072 6f64 7563 7428 2a5b 7065 726d  = product(*[perm
-0000b590: 7574 6174 696f 6e73 2865 6467 6573 2920  utations(edges) 
-0000b5a0: 666f 7220 6564 6765 7320 696e 2073 6f72  for edges in sor
-0000b5b0: 7465 645f 6564 6765 735d 290a 0a20 2020  ted_edges])..   
-0000b5c0: 2072 6976 6572 5f64 6566 6561 7473 203d   river_defeats =
-0000b5d0: 206c 6973 7428 290a 2020 2020 666f 7220   list().    for 
-0000b5e0: 7462 2069 6e20 7462 733a 0a20 2020 2020  tb in tbs:.     
-0000b5f0: 2020 2065 6467 6573 203d 2066 6c61 7474     edges = flatt
-0000b600: 656e 2874 6229 0a20 2020 2020 2020 2072  en(tb).        r
-0000b610: 6976 6572 5f64 6566 6561 7420 3d20 6e78  iver_defeat = nx
-0000b620: 2e44 6947 7261 7068 2829 200a 2020 2020  .DiGraph() .    
-0000b630: 2020 2020 666f 7220 6520 696e 2065 6467      for e in edg
-0000b640: 6573 3a20 0a20 2020 2020 2020 2020 2020  es: .           
-0000b650: 2069 6620 655b 315d 206e 6f74 2069 6e20   if e[1] not in 
-0000b660: 7269 7665 725f 6465 6665 6174 2e6e 6f64  river_defeat.nod
-0000b670: 6573 206f 7220 6c65 6e28 6c69 7374 2872  es or len(list(r
-0000b680: 6976 6572 5f64 6566 6561 742e 696e 5f65  iver_defeat.in_e
-0000b690: 6467 6573 2865 5b31 5d29 2929 203d 3d20  dges(e[1]))) == 
-0000b6a0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-0000b6b0: 2020 2072 6976 6572 5f64 6566 6561 742e     river_defeat.
-0000b6c0: 6164 645f 6564 6765 2865 5b30 5d2c 2065  add_edge(e[0], e
-0000b6d0: 5b31 5d2c 2077 6569 6768 743d 655b 325d  [1], weight=e[2]
-0000b6e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000b6f0: 2020 6966 2064 6f65 735f 6372 6561 7465    if does_create
-0000b700: 5f63 7963 6c65 2872 6976 6572 5f64 6566  _cycle(river_def
-0000b710: 6561 742c 2065 293a 0a20 2020 2020 2020  eat, e):.       
-0000b720: 2020 2020 2020 2020 2020 2020 2072 6976               riv
-0000b730: 6572 5f64 6566 6561 742e 7265 6d6f 7665  er_defeat.remove
-0000b740: 5f65 6467 6528 655b 305d 2c20 655b 315d  _edge(e[0], e[1]
-0000b750: 290a 2020 2020 2020 2020 2020 2020 0a20  ).            . 
-0000b760: 2020 2020 2020 2072 6976 6572 5f64 6566         river_def
-0000b770: 6561 7473 2e61 7070 656e 6428 7269 7665  eats.append(rive
-0000b780: 725f 6465 6665 6174 290a 0a20 2020 2072  r_defeat)..    r
-0000b790: 6574 7572 6e20 7269 7665 725f 6465 6665  eturn river_defe
-0000b7a0: 6174 730a 0a40 766d 286e 616d 653d 2252  ats..@vm(name="R
-0000b7b0: 6976 6572 2229 0a64 6566 2072 6976 6572  iver").def river
-0000b7c0: 5f77 6974 685f 7465 7374 2865 6461 7461  _with_test(edata
-0000b7d0: 2c20 6375 7272 5f63 616e 6473 203d 204e  , curr_cands = N
-0000b7e0: 6f6e 652c 2073 7472 656e 6774 685f 6675  one, strength_fu
-0000b7f0: 6e63 7469 6f6e 203d 204e 6f6e 6529 3a20  nction = None): 
-0000b800: 2020 0a20 2020 2022 2222 4669 6e64 2074    .    """Find t
-0000b810: 6865 2052 6976 6572 2077 696e 6e65 7273  he River winners
-0000b820: 2077 6974 6820 6120 7465 7374 2074 6f20   with a test to 
-0000b830: 6465 7465 726d 696e 6564 2069 6620 6974  determined if it
-0000b840: 2077 696c 6c20 7461 6b65 2074 6f6f 206c   will take too l
-0000b850: 6f6e 6720 746f 2063 6f6d 7075 7465 2074  ong to compute t
-0000b860: 6865 2052 6976 6572 2077 696e 6e65 7273  he River winners
-0000b870: 2e20 4966 2074 6865 2063 616c 6375 6c61  . If the calcula
-0000b880: 7469 6f6e 206f 6620 7468 6520 7769 6e6e  tion of the winn
-0000b890: 6572 7320 7769 6c6c 2074 616b 6520 746f  ers will take to
-0000b8a0: 6f20 6c6f 6e67 2c20 7265 7475 726e 204e  o long, return N
-0000b8b0: 6f6e 652e 200a 2020 2020 2020 2020 0a20  one. .        . 
-0000b8c0: 2020 202e 2e20 696d 706f 7274 616e 743a     .. important:
-0000b8d0: 3a0a 2020 2020 2020 2020 5468 6973 2076  :.        This v
-0000b8e0: 6f74 696e 6720 6d65 7468 6f64 2074 6861  oting method tha
-0000b8f0: 7420 6d69 6768 7420 7265 7475 726e 204e  t might return N
-0000b900: 6f6e 6520 7261 7468 6572 2074 6861 6e20  one rather than 
-0000b910: 6120 6c69 7374 206f 6620 6361 6e64 6964  a list of candid
-0000b920: 6174 6573 2e20 200a 0a20 2020 2041 7267  ates.  ..    Arg
-0000b930: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
-0000b940: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
-0000b950: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
-0000b960: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
-0000b970: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
-0000b980: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
-0000b990: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
-0000b9a0: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
-0000b9b0: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
-0000b9c0: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
-0000b9d0: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
-0000b9e0: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
-0000b9f0: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
-0000ba00: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
-0000ba10: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
-0000ba20: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
-0000ba30: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
-0000ba40: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
-0000ba50: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
-0000ba60: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
-0000ba70: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
-0000ba80: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
-0000ba90: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
-0000baa0: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
-0000bab0: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
-0000bac0: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
-0000bad0: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
-0000bae0: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
-0000baf0: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
-0000bb00: 732e 200a 0a20 2020 2052 6574 7572 6e73  s. ..    Returns
-0000bb10: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
-0000bb20: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
-0000bb30: 6964 6174 6573 2e20 0a0a 2020 2020 2e2e  idates. ..    ..
-0000bb40: 2073 6565 616c 736f 3a3a 0a0a 2020 2020   seealso::..    
-0000bb50: 2020 2020 3a6d 6574 683a 6070 7265 665f      :meth:`pref_
-0000bb60: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-0000bb70: 7365 645f 6d65 7468 6f64 732e 7261 6e6b  sed_methods.rank
-0000bb80: 6564 5f70 6169 7273 5f77 6974 685f 7465  ed_pairs_with_te
-0000bb90: 7374 602c 203a 6d65 7468 3a60 7072 6566  st`, :meth:`pref
-0000bba0: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
-0000bbb0: 6173 6564 5f6d 6574 686f 6473 2e72 6976  ased_methods.riv
-0000bbc0: 6572 600a 0a20 2020 2022 2222 0a20 2020  er`..    """.   
-0000bbd0: 2063 616e 6469 6461 7465 7320 3d20 6564   candidates = ed
-0000bbe0: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
-0000bbf0: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
-0000bc00: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
-0000bc10: 616e 6473 2020 2020 0a20 2020 2063 6964  ands    .    cid
-0000bc20: 785f 746f 5f63 616e 6420 3d20 7b63 6964  x_to_cand = {cid
-0000bc30: 783a 2063 2066 6f72 2063 6964 782c 2063  x: c for cidx, c
-0000bc40: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-0000bc50: 6e64 6964 6174 6573 297d 2020 0a20 2020  ndidates)}  .   
-0000bc60: 2063 616e 645f 746f 5f63 6964 7820 3d20   cand_to_cidx = 
-0000bc70: 7b63 3a20 6369 6478 2066 6f72 2063 6964  {c: cidx for cid
-0000bc80: 782c 2063 2069 6e20 656e 756d 6572 6174  x, c in enumerat
-0000bc90: 6528 6361 6e64 6964 6174 6573 297d 2020  e(candidates)}  
-0000bca0: 0a0a 2020 2020 7374 7265 6e67 7468 5f66  ..    strength_f
-0000bcb0: 756e 6374 696f 6e20 3d20 6564 6174 612e  unction = edata.
-0000bcc0: 6d61 7267 696e 2069 6620 7374 7265 6e67  margin if streng
-0000bcd0: 7468 5f66 756e 6374 696f 6e20 6973 204e  th_function is N
-0000bce0: 6f6e 6520 656c 7365 2073 7472 656e 6774  one else strengt
-0000bcf0: 685f 6675 6e63 7469 6f6e 2020 2020 0a0a  h_function    ..
-0000bd00: 2020 2020 6377 203d 2065 6461 7461 2e63      cw = edata.c
-0000bd10: 6f6e 646f 7263 6574 5f77 696e 6e65 7228  ondorcet_winner(
-0000bd20: 6375 7272 5f63 616e 6473 3d63 7572 725f  curr_cands=curr_
-0000bd30: 6361 6e64 7329 0a20 2020 2023 2052 616e  cands).    # Ran
-0000bd40: 6b65 6420 5061 6972 7320 6973 2043 6f6e  ked Pairs is Con
-0000bd50: 646f 7263 6574 2063 6f6e 7369 7374 656e  dorcet consisten
-0000bd60: 742c 2073 6f20 7369 6d70 6c79 2072 6574  t, so simply ret
-0000bd70: 7572 6e20 7468 6520 436f 6e64 6f72 6365  urn the Condorce
-0000bd80: 7420 7769 6e6e 6572 2069 6620 6578 6973  t winner if exis
-0000bd90: 7473 0a20 2020 2069 6620 6377 2069 7320  ts.    if cw is 
-0000bda0: 6e6f 7420 4e6f 6e65 3a20 0a20 2020 2020  not None: .     
-0000bdb0: 2020 2077 696e 6e65 7273 203d 205b 6377     winners = [cw
-0000bdc0: 5d0a 2020 2020 656c 7365 3a0a 2020 2020  ].    else:.    
-0000bdd0: 2020 2020 775f 6564 6765 7320 3d20 5b28      w_edges = [(
-0000bde0: 6331 2c20 6332 2c20 7374 7265 6e67 7468  c1, c2, strength
-0000bdf0: 5f66 756e 6374 696f 6e28 6331 2c20 6332  _function(c1, c2
-0000be00: 2929 2066 6f72 2063 3120 696e 2063 616e  )) for c1 in can
-0000be10: 6469 6461 7465 7320 666f 7220 6332 2069  didates for c2 i
-0000be20: 6e20 6361 6e64 6964 6174 6573 200a 2020  n candidates .  
-0000be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be40: 2069 6620 6331 2021 3d20 6332 2061 6e64   if c1 != c2 and
-0000be50: 2028 6564 6174 612e 6d61 6a6f 7269 7479   (edata.majority
-0000be60: 5f70 7265 6665 7273 2863 312c 2063 3229  _prefers(c1, c2)
-0000be70: 206f 7220 6564 6174 612e 6973 5f74 6965   or edata.is_tie
-0000be80: 6428 6331 2c20 6332 2929 5d0a 2020 2020  d(c1, c2))].    
-0000be90: 2020 2020 7769 6e6e 6572 7320 3d20 6c69      winners = li
-0000bea0: 7374 2829 2020 2020 2020 2020 2020 2020  st()            
-0000beb0: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
-0000bec0: 6873 203d 2073 6f72 7465 6428 6c69 7374  hs = sorted(list
-0000bed0: 2873 6574 285b 655b 325d 2066 6f72 2065  (set([e[2] for e
-0000bee0: 2069 6e20 775f 6564 6765 735d 2929 2c20   in w_edges])), 
-0000bef0: 7265 7665 7273 653d 5472 7565 290a 2020  reverse=True).  
-0000bf00: 2020 2020 2020 736f 7274 6564 5f65 6467        sorted_edg
-0000bf10: 6573 203d 205b 5b65 2066 6f72 2065 2069  es = [[e for e i
-0000bf20: 6e20 775f 6564 6765 7320 6966 2065 5b32  n w_edges if e[2
-0000bf30: 5d20 3d3d 2073 5d20 666f 7220 7320 696e  ] == s] for s in
-0000bf40: 2073 7472 656e 6774 6873 5d0a 2020 2020   strengths].    
-0000bf50: 2020 2020 6966 206e 702e 7072 6f64 285b      if np.prod([
-0000bf60: 6d61 7468 2e66 6163 746f 7269 616c 286c  math.factorial(l
-0000bf70: 656e 2865 7329 2920 666f 7220 6573 2069  en(es)) for es i
-0000bf80: 6e20 736f 7274 6564 5f65 6467 6573 5d29  n sorted_edges])
-0000bf90: 203e 2033 3030 303a 200a 2020 2020 2020   > 3000: .      
-0000bfa0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-0000bfb0: 650a 2020 2020 2020 2020 656c 7365 3a20  e.        else: 
-0000bfc0: 0a20 2020 2020 2020 2020 2020 2074 6273  .            tbs
-0000bfd0: 203d 2070 726f 6475 6374 282a 5b70 6572   = product(*[per
-0000bfe0: 6d75 7461 7469 6f6e 7328 6564 6765 7329  mutations(edges)
-0000bff0: 2066 6f72 2065 6467 6573 2069 6e20 736f   for edges in so
-0000c000: 7274 6564 5f65 6467 6573 5d29 0a20 2020  rted_edges]).   
-0000c010: 2020 2020 2020 2020 2066 6f72 2074 6220           for tb 
-0000c020: 696e 2074 6273 3a0a 2020 2020 2020 2020  in tbs:.        
-0000c030: 2020 2020 2020 2020 6564 6765 7320 3d20          edges = 
-0000c040: 666c 6174 7465 6e28 7462 290a 2020 2020  flatten(tb).    
-0000c050: 2020 2020 2020 2020 2020 2020 7276 5f64              rv_d
-0000c060: 6566 6561 7420 3d20 5350 4f28 6c65 6e28  efeat = SPO(len(
-0000c070: 6361 6e64 6964 6174 6573 2929 0a20 2020  candidates)).   
-0000c080: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000c090: 2065 302c 6531 2c73 2069 6e20 6564 6765   e0,e1,s in edge
-0000c0a0: 733a 200a 2020 2020 2020 2020 2020 2020  s: .            
-0000c0b0: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-0000c0c0: 765f 6465 6665 6174 2e50 5b63 616e 645f  v_defeat.P[cand_
-0000c0d0: 746f 5f63 6964 785b 6531 5d5d 5b63 616e  to_cidx[e1]][can
-0000c0e0: 645f 746f 5f63 6964 785b 6530 5d5d 2061  d_to_cidx[e0]] a
-0000c0f0: 6e64 206c 656e 2872 765f 6465 6665 6174  nd len(rv_defeat
-0000c100: 2e70 7265 6473 5b63 616e 645f 746f 5f63  .preds[cand_to_c
-0000c110: 6964 785b 6531 5d5d 2920 3d3d 2030 3a0a  idx[e1]]) == 0:.
-0000c120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c130: 2020 2020 2020 2020 7276 5f64 6566 6561          rv_defea
-0000c140: 742e 6164 6428 6361 6e64 5f74 6f5f 6369  t.add(cand_to_ci
-0000c150: 6478 5b65 305d 2c63 616e 645f 746f 5f63  dx[e0],cand_to_c
-0000c160: 6964 785b 6531 5d29 0a20 2020 2020 2020  idx[e1]).       
-0000c170: 2020 2020 2020 2020 2077 696e 6e65 7273           winners
-0000c180: 2e61 7070 656e 6428 6369 6478 5f74 6f5f  .append(cidx_to_
-0000c190: 6361 6e64 5b72 765f 6465 6665 6174 2e69  cand[rv_defeat.i
-0000c1a0: 6e69 7469 616c 5f65 6c65 6d65 6e74 7328  nitial_elements(
-0000c1b0: 295b 305d 5d29 0a20 2020 2072 6574 7572  )[0]]).    retur
-0000c1c0: 6e20 736f 7274 6564 286c 6973 7428 7365  n sorted(list(se
-0000c1d0: 7428 7769 6e6e 6572 7329 2929 0a0a 4076  t(winners)))..@v
-0000c1e0: 6d28 6e61 6d65 3d22 5269 7665 7220 5442  m(name="River TB
-0000c1f0: 2229 0a64 6566 2072 6976 6572 5f74 6228  ").def river_tb(
-0000c200: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
-0000c210: 7320 3d20 4e6f 6e65 2c20 7469 655f 6272  s = None, tie_br
-0000c220: 6561 6b65 7220 3d20 4e6f 6e65 2c20 7374  eaker = None, st
-0000c230: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-0000c240: 3d20 4e6f 6e65 293a 2020 200a 2020 2020  = None):   .    
-0000c250: 2222 220a 2020 2020 5269 7665 7220 7769  """.    River wi
-0000c260: 7468 2061 2066 6978 6564 206c 696e 6561  th a fixed linea
-0000c270: 7220 6f72 6465 7220 6f6e 2074 6865 2063  r order on the c
-0000c280: 616e 6469 6461 7465 7320 746f 2062 7265  andidates to bre
-0000c290: 616b 2061 6e79 2074 6965 7320 696e 2074  ak any ties in t
-0000c2a0: 6865 206d 6172 6769 6e73 2e20 2053 696e  he margins.  Sin
-0000c2b0: 6365 2074 6865 2074 6965 5f62 7265 616b  ce the tie_break
-0000c2c0: 6572 2069 7320 6120 6c69 6e65 6172 206f  er is a linear o
-0000c2d0: 7264 6572 2c20 7468 6973 206d 6574 686f  rder, this metho
-0000c2e0: 6420 6973 2072 6573 6f6c 7574 652e 2020  d is resolute.  
-0000c2f0: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
-0000c300: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-0000c310: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-0000c320: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-0000c330: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-0000c340: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-0000c350: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
-0000c360: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
-0000c370: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
-0000c380: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
-0000c390: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
-0000c3a0: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
-0000c3b0: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
-0000c3c0: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
-0000c3d0: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
-0000c3e0: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
-0000c3f0: 2020 7469 655f 6272 6561 6b65 7220 284c    tie_breaker (L
-0000c400: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
-0000c410: 616c 293a 2041 206c 696e 6561 7220 6f72  al): A linear or
-0000c420: 6465 7220 6f6e 2074 6865 2063 616e 6469  der on the candi
-0000c430: 6461 7465 732e 2020 4966 206e 6f74 2073  dates.  If not s
-0000c440: 6574 2c20 7468 656e 2074 6865 2063 616e  et, then the can
-0000c450: 6469 6461 7465 7320 6172 6520 736f 7274  didates are sort
-0000c460: 6564 2069 6e20 6173 6365 6e64 696e 6720  ed in ascending 
-0000c470: 6f72 6465 722e 0a20 2020 2020 2020 2073  order..        s
-0000c480: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000c490: 2028 6675 6e63 7469 6f6e 2c20 6f70 7469   (function, opti
-0000c4a0: 6f6e 616c 293a 2054 6865 2073 7472 656e  onal): The stren
-0000c4b0: 6774 6820 6675 6e63 7469 6f6e 2074 6f20  gth function to 
-0000c4c0: 6265 2075 7365 6420 746f 2063 616c 6375  be used to calcu
-0000c4d0: 6c61 7465 2074 6865 2073 7472 656e 6774  late the strengt
-0000c4e0: 6820 6f66 2061 2070 6174 682e 2020 2054  h of a path.   T
-0000c4f0: 6865 2064 6566 6175 6c74 2069 7320 7468  he default is th
-0000c500: 6520 6d61 7267 696e 206d 6574 686f 6420  e margin method 
-0000c510: 6f66 2060 6065 6461 7461 6060 2e20 2020  of ``edata``.   
-0000c520: 5468 6973 206f 6e6c 7920 6d61 7474 6572  This only matter
-0000c530: 7320 7768 656e 2074 6865 2062 616c 6c6f  s when the ballo
-0000c540: 7473 2061 7265 206e 6f74 206c 696e 6561  ts are not linea
-0000c550: 7220 6f72 6465 7273 2e20 0a0a 2020 2020  r orders. ..    
-0000c560: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
-0000c570: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
-0000c580: 6f66 2063 616e 6469 6461 7465 732e 200a  of candidates. .
-0000c590: 0a20 2020 2022 2222 0a20 2020 2063 616e  .    """.    can
-0000c5a0: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
-0000c5b0: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
-0000c5c0: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
-0000c5d0: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
-0000c5e0: 2020 2020 0a20 2020 2063 6964 785f 746f      .    cidx_to
-0000c5f0: 5f63 616e 6420 3d20 7b63 6964 783a 2063  _cand = {cidx: c
-0000c600: 2066 6f72 2063 6964 782c 2063 2069 6e20   for cidx, c in 
-0000c610: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
-0000c620: 6174 6573 297d 2020 0a20 2020 2063 616e  ates)}  .    can
-0000c630: 645f 746f 5f63 6964 7820 3d20 7b63 3a20  d_to_cidx = {c: 
-0000c640: 6369 6478 2066 6f72 2063 6964 782c 2063  cidx for cidx, c
-0000c650: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-0000c660: 6e64 6964 6174 6573 297d 2020 0a20 2020  ndidates)}  .   
-0000c670: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000c680: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
-0000c690: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
-0000c6a0: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
-0000c6b0: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
-0000c6c0: 6374 696f 6e20 2020 200a 0a20 2020 2074  ction    ..    t
-0000c6d0: 625f 7261 6e6b 696e 6720 3d20 7469 655f  b_ranking = tie_
-0000c6e0: 6272 6561 6b65 7220 6966 2074 6965 5f62  breaker if tie_b
-0000c6f0: 7265 616b 6572 2069 7320 6e6f 7420 4e6f  reaker is not No
-0000c700: 6e65 2065 6c73 6520 736f 7274 6564 286c  ne else sorted(l
-0000c710: 6973 7428 6361 6e64 6964 6174 6573 2929  ist(candidates))
-0000c720: 0a0a 2020 2020 6377 203d 2065 6461 7461  ..    cw = edata
-0000c730: 2e63 6f6e 646f 7263 6574 5f77 696e 6e65  .condorcet_winne
-0000c740: 7228 6375 7272 5f63 616e 6473 3d63 7572  r(curr_cands=cur
-0000c750: 725f 6361 6e64 7329 0a20 2020 2023 2052  r_cands).    # R
-0000c760: 6976 6572 2069 7320 436f 6e64 6f72 6365  iver is Condorce
-0000c770: 7420 636f 6e73 6973 7465 6e74 2c20 736f  t consistent, so
-0000c780: 2073 696d 706c 7920 7265 7475 726e 2074   simply return t
-0000c790: 6865 2043 6f6e 646f 7263 6574 2077 696e  he Condorcet win
-0000c7a0: 6e65 7220 6966 2065 7869 7374 730a 2020  ner if exists.  
-0000c7b0: 2020 6966 2063 7720 6973 206e 6f74 204e    if cw is not N
-0000c7c0: 6f6e 653a 200a 2020 2020 2020 2020 7769  one: .        wi
-0000c7d0: 6e6e 6572 7320 3d20 5b63 775d 0a20 2020  nners = [cw].   
-0000c7e0: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
-0000c7f0: 5f65 6467 6573 203d 205b 2863 312c 2063  _edges = [(c1, c
-0000c800: 322c 2073 7472 656e 6774 685f 6675 6e63  2, strength_func
-0000c810: 7469 6f6e 2863 312c 2063 3229 2920 666f  tion(c1, c2)) fo
-0000c820: 7220 6331 2069 6e20 6361 6e64 6964 6174  r c1 in candidat
-0000c830: 6573 2066 6f72 2063 3220 696e 2063 616e  es for c2 in can
-0000c840: 6469 6461 7465 7320 6966 2063 3120 213d  didates if c1 !=
-0000c850: 2063 3220 616e 6420 2865 6461 7461 2e6d   c2 and (edata.m
-0000c860: 616a 6f72 6974 795f 7072 6566 6572 7328  ajority_prefers(
-0000c870: 6331 2c20 6332 2920 6f72 2065 6461 7461  c1, c2) or edata
-0000c880: 2e69 735f 7469 6564 2863 312c 2063 3229  .is_tied(c1, c2)
-0000c890: 295d 0a20 2020 2020 2020 2077 696e 6e65  )].        winne
-0000c8a0: 7273 203d 206c 6973 7428 2920 200a 2020  rs = list()  .  
-0000c8b0: 2020 2020 2020 7374 7265 6e67 7468 7320        strengths 
-0000c8c0: 3d20 736f 7274 6564 286c 6973 7428 7365  = sorted(list(se
-0000c8d0: 7428 5b65 5b32 5d20 666f 7220 6520 696e  t([e[2] for e in
-0000c8e0: 2077 5f65 6467 6573 5d29 292c 2072 6576   w_edges])), rev
-0000c8f0: 6572 7365 3d54 7275 6529 0a0a 2020 2020  erse=True)..    
-0000c900: 2020 2020 7276 5f64 6566 6561 7420 3d20      rv_defeat = 
-0000c910: 5350 4f28 6c65 6e28 6361 6e64 6964 6174  SPO(len(candidat
-0000c920: 6573 2929 0a0a 2020 2020 2020 2020 666f  es))..        fo
-0000c930: 7220 7320 696e 2073 7472 656e 6774 6873  r s in strengths
-0000c940: 3a20 0a20 2020 2020 2020 2020 2020 2065  : .            e
-0000c950: 6467 6573 203d 205b 6520 666f 7220 6520  dges = [e for e 
-0000c960: 696e 2077 5f65 6467 6573 2069 6620 655b  in w_edges if e[
-0000c970: 325d 203d 3d20 735d 0a20 2020 2020 2020  2] == s].       
-0000c980: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-0000c990: 2020 2320 6272 6561 6b20 7469 6573 2075    # break ties u
-0000c9a0: 7369 6e67 2074 6865 206c 6578 6963 6f67  sing the lexicog
-0000c9b0: 7261 7068 6963 206f 7264 6572 696e 6720  raphic ordering 
-0000c9c0: 6f6e 2074 7570 6c65 7320 6769 7665 6e20  on tuples given 
-0000c9d0: 7462 5f72 616e 6b69 6e67 0a20 2020 2020  tb_ranking.     
-0000c9e0: 2020 2020 2020 2073 6f72 7465 645f 6564         sorted_ed
-0000c9f0: 6765 7320 3d20 736f 7274 6564 2865 6467  ges = sorted(edg
-0000ca00: 6573 2c20 6b65 7920 3d20 6c61 6d62 6461  es, key = lambda
-0000ca10: 2065 3a20 2874 625f 7261 6e6b 696e 672e   e: (tb_ranking.
-0000ca20: 696e 6465 7828 655b 305d 292c 2074 625f  index(e[0]), tb_
-0000ca30: 7261 6e6b 696e 672e 696e 6465 7828 655b  ranking.index(e[
-0000ca40: 315d 2929 2c20 7265 7665 7273 653d 4661  1])), reverse=Fa
-0000ca50: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-0000ca60: 2066 6f72 2065 302c 6531 2c73 2069 6e20   for e0,e1,s in 
-0000ca70: 736f 7274 6564 5f65 6467 6573 3a20 0a20  sorted_edges: . 
-0000ca80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000ca90: 6620 6e6f 7420 7276 5f64 6566 6561 742e  f not rv_defeat.
-0000caa0: 505b 6361 6e64 5f74 6f5f 6369 6478 5b65  P[cand_to_cidx[e
-0000cab0: 315d 5d5b 6361 6e64 5f74 6f5f 6369 6478  1]][cand_to_cidx
-0000cac0: 5b65 305d 5d20 616e 6420 6c65 6e28 7276  [e0]] and len(rv
-0000cad0: 5f64 6566 6561 742e 7072 6564 735b 6361  _defeat.preds[ca
-0000cae0: 6e64 5f74 6f5f 6369 6478 5b65 315d 5d29  nd_to_cidx[e1]])
-0000caf0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-0000cb00: 2020 2020 2020 2020 2020 2072 765f 6465             rv_de
-0000cb10: 6665 6174 2e61 6464 2863 616e 645f 746f  feat.add(cand_to
-0000cb20: 5f63 6964 785b 6530 5d2c 6361 6e64 5f74  _cidx[e0],cand_t
-0000cb30: 6f5f 6369 6478 5b65 315d 290a 2020 2020  o_cidx[e1]).    
-0000cb40: 2020 2020 2020 2020 7769 6e6e 6572 732e          winners.
-0000cb50: 6170 7065 6e64 2863 6964 785f 746f 5f63  append(cidx_to_c
-0000cb60: 616e 645b 7276 5f64 6566 6561 742e 696e  and[rv_defeat.in
-0000cb70: 6974 6961 6c5f 656c 656d 656e 7473 2829  itial_elements()
-0000cb80: 5b30 5d5d 290a 2020 2020 7265 7475 726e  [0]]).    return
-0000cb90: 2073 6f72 7465 6428 6c69 7374 2873 6574   sorted(list(set
-0000cba0: 2877 696e 6e65 7273 2929 290a 0a0a 4076  (winners)))...@v
-0000cbb0: 6d28 6e61 6d65 3d22 5269 7665 7220 5a54  m(name="River ZT
-0000cbc0: 2229 0a64 6566 2072 6976 6572 5f7a 7428  ").def river_zt(
-0000cbd0: 7072 6f66 696c 652c 2063 7572 725f 6361  profile, curr_ca
-0000cbe0: 6e64 7320 3d20 4e6f 6e65 2c20 7374 7265  nds = None, stre
-0000cbf0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-0000cc00: 4e6f 6e65 293a 2020 200a 2020 2020 2222  None):   .    ""
-0000cc10: 2252 6976 6572 2077 6865 7265 2061 2066  "River where a f
-0000cc20: 6978 6564 2076 6f74 6572 2062 7265 616b  ixed voter break
-0000cc30: 7320 616e 7920 7469 6573 2069 6e20 7468  s any ties in th
-0000cc40: 6520 6d61 7267 696e 732e 2020 4974 2069  e margins.  It i
-0000cc50: 7320 616c 7761 7973 2074 6865 2076 6f74  s always the vot
-0000cc60: 6572 2069 6e20 706f 7369 7469 6f6e 2030  er in position 0
-0000cc70: 2074 6861 7420 6272 6561 6b73 2074 6865   that breaks the
-0000cc80: 2074 6965 732e 2020 5369 6e63 6520 766f   ties.  Since vo
-0000cc90: 7465 7273 2068 6176 6520 7374 7269 6374  ters have strict
-0000cca0: 2070 7265 6665 7265 6e63 6573 2c20 7468   preferences, th
-0000ccb0: 6973 206d 6574 686f 6420 6973 2072 6573  is method is res
-0000ccc0: 6f6c 7574 652e 2020 0a0a 2020 2020 4172  olute.  ..    Ar
-0000ccd0: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
-0000cce0: 6120 2850 726f 6669 6c65 293a 2041 2070  a (Profile): A p
-0000ccf0: 726f 6669 6c65 206f 6620 6c69 6e65 6172  rofile of linear
-0000cd00: 206f 7264 6572 730a 2020 2020 2020 2020   orders.        
-0000cd10: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
-0000cd20: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
-0000cd30: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
-0000cd40: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
-0000cd50: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
-0000cd60: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
-0000cd70: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
-0000cd80: 6060 6375 7272 5f63 616e 6473 6060 0a0a  ``curr_cands``..
-0000cd90: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
-0000cda0: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
-0000cdb0: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
-0000cdc0: 732e 200a 0a20 2020 202e 2e20 7365 6561  s. ..    .. seea
-0000cdd0: 6c73 6f3a 3a0a 0a20 2020 2020 2020 203a  lso::..        :
-0000cde0: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-0000cdf0: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-0000ce00: 6574 686f 6473 2e72 6976 6572 602c 203a  ethods.river`, :
-0000ce10: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-0000ce20: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-0000ce30: 6574 686f 6473 2e72 6976 6572 5f77 6974  ethods.river_wit
-0000ce40: 685f 7465 7374 602c 203a 6d65 7468 3a60  h_test`, :meth:`
-0000ce50: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
-0000ce60: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
-0000ce70: 2e72 616e 6b65 645f 7061 6972 7360 0a0a  .ranked_pairs`..
-0000ce80: 2020 2020 0a20 2020 2022 2222 0a20 2020      .    """.   
-0000ce90: 2063 616e 6469 6461 7465 7320 3d20 7072   candidates = pr
-0000cea0: 6f66 696c 652e 6361 6e64 6964 6174 6573  ofile.candidates
-0000ceb0: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
-0000cec0: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
-0000ced0: 5f63 616e 6473 2020 2020 0a20 2020 200a  _cands    .    .
-0000cee0: 2020 2020 2320 7468 6520 7469 652d 6272      # the tie-br
-0000cef0: 6561 6b65 7220 6973 2061 6c77 6179 7320  eaker is always 
-0000cf00: 7468 6520 6669 7273 7420 766f 7465 722e  the first voter.
-0000cf10: 200a 2020 2020 7462 5f72 616e 6b69 6e67   .    tb_ranking
-0000cf20: 203d 2074 7570 6c65 285b 6320 666f 7220   = tuple([c for 
-0000cf30: 6320 696e 206c 6973 7428 7072 6f66 696c  c in list(profil
-0000cf40: 652e 5f72 616e 6b69 6e67 735b 305d 2920  e._rankings[0]) 
-0000cf50: 6966 2063 2069 6e20 6361 6e64 6964 6174  if c in candidat
-0000cf60: 6573 5d29 0a20 2020 200a 2020 2020 7265  es]).    .    re
-0000cf70: 7475 726e 2072 6976 6572 5f74 6228 7072  turn river_tb(pr
-0000cf80: 6f66 696c 652c 2063 7572 725f 6361 6e64  ofile, curr_cand
-0000cf90: 7320 3d20 6375 7272 5f63 616e 6473 2c20  s = curr_cands, 
-0000cfa0: 7469 655f 6272 6561 6b65 7220 3d20 7462  tie_breaker = tb
-0000cfb0: 5f72 616e 6b69 6e67 2c20 7374 7265 6e67  _ranking, streng
-0000cfc0: 7468 5f66 756e 6374 696f 6e20 3d20 7374  th_function = st
-0000cfd0: 7265 6e67 7468 5f66 756e 6374 696f 6e29  rength_function)
-0000cfe0: 0a20 2020 200a 0a23 2053 696d 706c 6520  .    ..# Simple 
-0000cff0: 5374 6162 6c65 2056 6f74 696e 6720 0a64  Stable Voting .d
-0000d000: 6566 205f 7369 6d70 6c65 5f73 7461 626c  ef _simple_stabl
-0000d010: 655f 766f 7469 6e67 2863 7572 725f 6361  e_voting(curr_ca
-0000d020: 6e64 732c 200a 2020 2020 2020 2020 2020  nds, .          
-0000d030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d040: 736f 7274 6564 5f6d 6174 6368 6573 2c0a  sorted_matches,.
-0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d060: 2020 2020 2020 2020 2020 6d65 6d5f 7376            mem_sv
-0000d070: 5f77 696e 6e65 7273 293a 0a20 2020 2027  _winners):.    '
-0000d080: 2727 0a20 2020 2044 6574 6572 6d69 6e65  ''.    Determine
-0000d090: 2074 6865 2053 696d 706c 6520 5374 6162   the Simple Stab
-0000d0a0: 6c65 2056 6f74 696e 6720 7769 6e6e 6572  le Voting winner
-0000d0b0: 7320 7768 696c 6520 6b65 6570 696e 6720  s while keeping 
-0000d0c0: 7472 6163 6b20 0a20 2020 206f 6620 7468  track .    of th
-0000d0d0: 6520 7769 6e6e 6572 7320 696e 2061 6e79  e winners in any
-0000d0e0: 2073 7562 7072 6f66 696c 6573 2063 6865   subprofiles che
-0000d0f0: 636b 6564 2064 7572 696e 6720 636f 6d70  cked during comp
-0000d100: 7574 6174 696f 6e2e 200a 2020 2020 2727  utation. .    ''
-0000d110: 270a 2020 2020 0a20 2020 2073 765f 7769  '.    .    sv_wi
-0000d120: 6e6e 6572 7320 3d20 6c69 7374 2829 0a20  nners = list(). 
-0000d130: 2020 2020 2020 200a 2020 2020 6966 206c         .    if l
-0000d140: 656e 2863 7572 725f 6361 6e64 7329 203d  en(curr_cands) =
-0000d150: 3d20 313a 200a 2020 2020 2020 2020 6d65  = 1: .        me
-0000d160: 6d5f 7376 5f77 696e 6e65 7273 5b74 7570  m_sv_winners[tup
-0000d170: 6c65 2863 7572 725f 6361 6e64 7329 5d20  le(curr_cands)] 
-0000d180: 3d20 6375 7272 5f63 616e 6473 0a20 2020  = curr_cands.   
-0000d190: 2020 2020 2072 6574 7572 6e20 6375 7272       return curr
-0000d1a0: 5f63 616e 6473 2c20 6d65 6d5f 7376 5f77  _cands, mem_sv_w
-0000d1b0: 696e 6e65 7273 0a20 2020 200a 2020 2020  inners.    .    
-0000d1c0: 6d61 7267 696e 5f77 6974 6e65 7373 696e  margin_witnessin
-0000d1d0: 675f 7769 6e20 3d20 2d6d 6174 682e 696e  g_win = -math.in
-0000d1e0: 660a 0a20 2020 2066 6f72 2061 2c20 622c  f..    for a, b,
-0000d1f0: 2073 2069 6e20 736f 7274 6564 5f6d 6174   s in sorted_mat
-0000d200: 6368 6573 3a0a 2020 2020 2020 2020 6966  ches:.        if
-0000d210: 2073 203c 206d 6172 6769 6e5f 7769 746e   s < margin_witn
-0000d220: 6573 7369 6e67 5f77 696e 3a20 0a20 2020  essing_win: .   
-0000d230: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
-0000d240: 2020 2020 2020 2069 6620 6120 6e6f 7420         if a not 
-0000d250: 696e 2073 765f 7769 6e6e 6572 733a 200a  in sv_winners: .
-0000d260: 2020 2020 2020 2020 2020 2020 6361 6e64              cand
-0000d270: 735f 6d69 6e75 735f 6220 3d20 5b63 2066  s_minus_b = [c f
-0000d280: 6f72 2063 2069 6e20 6375 7272 5f63 616e  or c in curr_can
-0000d290: 6473 2069 6620 6320 213d 2062 5d0a 2020  ds if c != b].  
-0000d2a0: 2020 2020 2020 2020 2020 6361 6e64 735f            cands_
-0000d2b0: 6d69 6e75 735f 625f 6b65 7920 3d20 7475  minus_b_key = tu
-0000d2c0: 706c 6528 736f 7274 6564 2863 616e 6473  ple(sorted(cands
-0000d2d0: 5f6d 696e 7573 5f62 2929 0a20 2020 2020  _minus_b)).     
-0000d2e0: 2020 2020 2020 2069 6620 6361 6e64 735f         if cands_
-0000d2f0: 6d69 6e75 735f 625f 6b65 7920 6e6f 7420  minus_b_key not 
-0000d300: 696e 206d 656d 5f73 765f 7769 6e6e 6572  in mem_sv_winner
-0000d310: 732e 6b65 7973 2829 3a20 0a20 2020 2020  s.keys(): .     
-0000d320: 2020 2020 2020 2020 2020 2077 732c 206d             ws, m
-0000d330: 656d 5f73 765f 7769 6e6e 6572 7320 3d20  em_sv_winners = 
-0000d340: 5f73 696d 706c 655f 7374 6162 6c65 5f76  _simple_stable_v
-0000d350: 6f74 696e 6728 6375 7272 5f63 616e 6473  oting(curr_cands
-0000d360: 203d 2063 616e 6473 5f6d 696e 7573 5f62   = cands_minus_b
-0000d370: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3a0: 2020 2020 2020 2020 2020 2020 2073 6f72               sor
-0000d3b0: 7465 645f 6d61 7463 6865 7320 3d20 5b28  ted_matches = [(
-0000d3c0: 612c 2063 2c20 7329 2066 6f72 2061 2c20  a, c, s) for a, 
-0000d3d0: 632c 2073 2069 6e20 736f 7274 6564 5f6d  c, s in sorted_m
-0000d3e0: 6174 6368 6573 2069 6620 6120 213d 2062  atches if a != b
-0000d3f0: 2061 6e64 2063 2021 3d20 625d 2c0a 2020   and c != b],.  
-0000d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d430: 2020 2020 2020 2020 206d 656d 5f73 765f           mem_sv_
-0000d440: 7769 6e6e 6572 7320 3d20 6d65 6d5f 7376  winners = mem_sv
-0000d450: 5f77 696e 6e65 7273 290a 2020 2020 2020  _winners).      
-0000d460: 2020 2020 2020 2020 2020 6d65 6d5f 7376            mem_sv
-0000d470: 5f77 696e 6e65 7273 5b63 616e 6473 5f6d  _winners[cands_m
-0000d480: 696e 7573 5f62 5f6b 6579 5d20 3d20 7773  inus_b_key] = ws
-0000d490: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000d4a0: 653a 200a 2020 2020 2020 2020 2020 2020  e: .            
-0000d4b0: 2020 2020 7773 203d 206d 656d 5f73 765f      ws = mem_sv_
-0000d4c0: 7769 6e6e 6572 735b 6361 6e64 735f 6d69  winners[cands_mi
-0000d4d0: 6e75 735f 625f 6b65 795d 0a20 2020 2020  nus_b_key].     
-0000d4e0: 2020 2020 2020 2069 6620 6120 696e 2077         if a in w
-0000d4f0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000d500: 2020 2073 765f 7769 6e6e 6572 732e 6170     sv_winners.ap
-0000d510: 7065 6e64 2861 290a 2020 2020 2020 2020  pend(a).        
-0000d520: 2020 2020 2020 2020 6d61 7267 696e 5f77          margin_w
-0000d530: 6974 6e65 7373 696e 675f 7769 6e20 3d20  itnessing_win = 
-0000d540: 730a 0a20 2020 2072 6574 7572 6e20 7376  s..    return sv
-0000d550: 5f77 696e 6e65 7273 2c20 6d65 6d5f 7376  _winners, mem_sv
-0000d560: 5f77 696e 6e65 7273 0a20 2020 200a 0a40  _winners.    ..@
-0000d570: 766d 286e 616d 6520 3d20 2253 696d 706c  vm(name = "Simpl
-0000d580: 6520 5374 6162 6c65 2056 6f74 696e 6722  e Stable Voting"
-0000d590: 290a 6465 6620 5f73 696d 706c 655f 7374  ).def _simple_st
-0000d5a0: 6162 6c65 5f76 6f74 696e 675f 7769 7468  able_voting_with
-0000d5b0: 5f63 6f6e 646f 7263 6574 5f63 6865 636b  _condorcet_check
-0000d5c0: 280a 2020 2020 6564 6174 612c 200a 2020  (.    edata, .  
-0000d5d0: 2020 6375 7272 5f63 616e 6473 203d 204e    curr_cands = N
-0000d5e0: 6f6e 652c 200a 2020 2020 7374 7265 6e67  one, .    streng
-0000d5f0: 7468 5f66 756e 6374 696f 6e20 3d20 4e6f  th_function = No
-0000d600: 6e65 293a 200a 2020 2020 2222 2253 696d  ne): .    """Sim
-0000d610: 706c 6520 5374 6162 6c65 2056 6f74 696e  ple Stable Votin
-0000d620: 6720 6973 2043 6f6e 646f 7263 6574 2063  g is Condorcet c
-0000d630: 6f6e 7369 7374 656e 742e 2020 2049 7420  onsistent.   It 
-0000d640: 6973 2066 6173 7465 7220 746f 2073 6b69  is faster to ski
-0000d650: 7020 6578 6563 7574 696e 6720 7468 6520  p executing the 
-0000d660: 7265 6375 7273 6976 6520 616c 676f 7269  recursive algori
-0000d670: 7468 6d20 7768 656e 2074 6865 7265 2069  thm when there i
-0000d680: 7320 6120 436f 6e64 6f72 6365 7420 7769  s a Condorcet wi
-0000d690: 6e6e 6572 4669 7273 7420 6368 6563 6b20  nnerFirst check 
-0000d6a0: 6966 2074 6865 7265 2069 7320 6120 436f  if there is a Co
-0000d6b0: 6e64 6f72 6365 7420 7769 6e6e 6572 2e20  ndorcet winner. 
-0000d6c0: 2049 6620 736f 2c20 7265 7475 726e 2074   If so, return t
-0000d6d0: 6865 2043 6f6e 646f 7263 6574 2077 696e  he Condorcet win
-0000d6e0: 6e65 722c 206f 7468 6572 7769 7365 2066  ner, otherwise f
-0000d6f0: 696e 6420 7468 6520 5369 6d70 6c65 2053  ind the Simple S
-0000d700: 7461 626c 6520 566f 7469 6e67 2077 696e  table Voting win
-0000d710: 6e65 7220 7573 696e 6720 5f73 696d 706c  ner using _simpl
-0000d720: 655f 7374 6162 6c65 5f76 6f74 696e 670a  e_stable_voting.
-0000d730: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-0000d740: 2020 2065 6461 7461 2028 5072 6f66 696c     edata (Profil
-0000d750: 652c 2050 726f 6669 6c65 5769 7468 5469  e, ProfileWithTi
-0000d760: 6573 2c20 4d61 7267 696e 4772 6170 6829  es, MarginGraph)
-0000d770: 3a20 416e 7920 656c 6563 7469 6f6e 2064  : Any election d
-0000d780: 6174 6120 7468 6174 2068 6173 2061 2060  ata that has a `
-0000d790: 6d61 7267 696e 6020 6d65 7468 6f64 2e20  margin` method. 
-0000d7a0: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
-0000d7b0: 6e64 7320 284c 6973 745b 696e 745d 2c20  nds (List[int], 
-0000d7c0: 6f70 7469 6f6e 616c 293a 2049 6620 7365  optional): If se
-0000d7d0: 742c 2074 6865 6e20 6669 6e64 2074 6865  t, then find the
-0000d7e0: 2077 696e 6e65 7273 2066 6f72 2074 6865   winners for the
-0000d7f0: 2070 726f 6669 6c65 2072 6573 7472 6963   profile restric
-0000d800: 7465 6420 746f 2074 6865 2063 616e 6469  ted to the candi
-0000d810: 6461 7465 7320 696e 2060 6063 7572 725f  dates in ``curr_
-0000d820: 6361 6e64 7360 600a 2020 2020 2020 2020  cands``.        
-0000d830: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000d840: 6e20 2866 756e 6374 696f 6e2c 206f 7074  n (function, opt
-0000d850: 696f 6e61 6c29 3a20 5468 6520 7374 7265  ional): The stre
-0000d860: 6e67 7468 2066 756e 6374 696f 6e20 746f  ngth function to
-0000d870: 2062 6520 7573 6564 2074 6f20 6361 6c63   be used to calc
-0000d880: 756c 6174 6520 7468 6520 7374 7265 6e67  ulate the streng
-0000d890: 7468 206f 6620 6120 7061 7468 2e20 2020  th of a path.   
-0000d8a0: 5468 6520 6465 6661 756c 7420 6973 2074  The default is t
-0000d8b0: 6865 206d 6172 6769 6e20 6d65 7468 6f64  he margin method
-0000d8c0: 206f 6620 6060 6564 6174 6160 602e 2020   of ``edata``.  
-0000d8d0: 2054 6869 7320 6f6e 6c79 206d 6174 7465   This only matte
-0000d8e0: 7273 2077 6865 6e20 7468 6520 6261 6c6c  rs when the ball
-0000d8f0: 6f74 7320 6172 6520 6e6f 7420 6c69 6e65  ots are not line
-0000d900: 6172 206f 7264 6572 732e 200a 0a20 2020  ar orders. ..   
-0000d910: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
-0000d920: 2020 2041 2073 6f72 7465 6420 6c69 7374     A sorted list
-0000d930: 206f 6620 6361 6e64 6964 6174 6573 2e20   of candidates. 
-0000d940: 0a0a 2020 2020 2222 220a 2020 2020 0a20  ..    """.    . 
-0000d950: 2020 2063 7720 3d20 6564 6174 612e 636f     cw = edata.co
-0000d960: 6e64 6f72 6365 745f 7769 6e6e 6572 2863  ndorcet_winner(c
-0000d970: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
-0000d980: 5f63 616e 6473 290a 2020 2020 6966 2063  _cands).    if c
-0000d990: 7720 6973 206e 6f74 204e 6f6e 653a 200a  w is not None: .
-0000d9a0: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-0000d9b0: 6377 5d0a 2020 2020 656c 7365 3a20 0a20  cw].    else: . 
-0000d9c0: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
-0000d9d0: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-0000d9e0: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-0000d9f0: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-0000da00: 6375 7272 5f63 616e 6473 0a20 2020 2020  curr_cands.     
-0000da10: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-0000da20: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
-0000da30: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
-0000da40: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
-0000da50: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
-0000da60: 756e 6374 696f 6e20 200a 0a20 2020 2020  unction  ..     
-0000da70: 2020 206d 6174 6368 6573 203d 205b 2861     matches = [(a
-0000da80: 2c20 622c 2073 7472 656e 6774 685f 6675  , b, strength_fu
-0000da90: 6e63 7469 6f6e 2861 2c20 6229 2920 666f  nction(a, b)) fo
-0000daa0: 7220 6120 696e 2063 7572 725f 6361 6e64  r a in curr_cand
-0000dab0: 7320 666f 7220 6220 696e 2063 7572 725f  s for b in curr_
-0000dac0: 6361 6e64 7320 6966 2061 2021 3d20 625d  cands if a != b]
-0000dad0: 0a20 2020 2020 2020 2073 6f72 7465 645f  .        sorted_
-0000dae0: 6d61 7463 6865 7320 3d20 736f 7274 6564  matches = sorted
-0000daf0: 286d 6174 6368 6573 2c20 7265 7665 7273  (matches, revers
-0000db00: 653d 5472 7565 2c20 6b65 793d 6c61 6d62  e=True, key=lamb
-0000db10: 6461 206d 5f77 5f77 6569 6768 743a 206d  da m_w_weight: m
-0000db20: 5f77 5f77 6569 6768 745b 325d 290a 2020  _w_weight[2]).  
-0000db30: 2020 0a20 2020 2020 2020 2072 6574 7572    .        retur
-0000db40: 6e20 736f 7274 6564 285f 7369 6d70 6c65  n sorted(_simple
-0000db50: 5f73 7461 626c 655f 766f 7469 6e67 2863  _stable_voting(c
-0000db60: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
-0000db70: 5f63 616e 6473 2c20 0a20 2020 2020 2020  _cands, .       
-0000db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dba0: 2020 2020 2073 6f72 7465 645f 6d61 7463       sorted_matc
-0000dbb0: 6865 7320 3d20 736f 7274 6564 5f6d 6174  hes = sorted_mat
-0000dbc0: 6368 6573 2c0a 2020 2020 2020 2020 2020  ches,.          
-0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbf0: 2020 6d65 6d5f 7376 5f77 696e 6e65 7273    mem_sv_winners
-0000dc00: 203d 207b 7d29 5b30 5d29 0a0a 0a64 6566   = {})[0])...def
-0000dc10: 205f 7369 6d70 6c65 5f73 7461 626c 655f   _simple_stable_
-0000dc20: 766f 7469 6e67 5f62 6173 6963 2865 6461  voting_basic(eda
-0000dc30: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
-0000dc40: 204e 6f6e 652c 2073 7472 656e 6774 685f   None, strength_
-0000dc50: 6675 6e63 7469 6f6e 203d 204e 6f6e 6529  function = None)
-0000dc60: 3a20 0a20 2020 2022 2222 496d 706c 656d  : .    """Implem
-0000dc70: 656e 7461 7469 6f6e 206f 6620 5369 6d70  entation of Simp
-0000dc80: 6c65 2053 7461 626c 6520 566f 7469 6e67  le Stable Voting
-0000dc90: 2066 726f 6d20 6874 7470 733a 2f2f 6172   from https://ar
-0000dca0: 7869 762e 6f72 672f 6162 732f 3231 3038  xiv.org/abs/2108
-0000dcb0: 2e30 3035 3432 2e20 0a0a 2020 2020 4172  .00542. ..    Ar
-0000dcc0: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
-0000dcd0: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
-0000dce0: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
-0000dcf0: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
-0000dd00: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
-0000dd10: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
-0000dd20: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
-0000dd30: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
-0000dd40: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
-0000dd50: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
-0000dd60: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
-0000dd70: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
-0000dd80: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
-0000dd90: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
-0000dda0: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
-0000ddb0: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
-0000ddc0: 685f 6675 6e63 7469 6f6e 2028 6675 6e63  h_function (func
-0000ddd0: 7469 6f6e 2c20 6f70 7469 6f6e 616c 293a  tion, optional):
-0000dde0: 2054 6865 2073 7472 656e 6774 6820 6675   The strength fu
-0000ddf0: 6e63 7469 6f6e 2074 6f20 6265 2075 7365  nction to be use
-0000de00: 6420 746f 2063 616c 6375 6c61 7465 2074  d to calculate t
-0000de10: 6865 2073 7472 656e 6774 6820 6f66 2061  he strength of a
-0000de20: 2070 6174 682e 2020 2054 6865 2064 6566   path.   The def
-0000de30: 6175 6c74 2069 7320 7468 6520 6d61 7267  ault is the marg
-0000de40: 696e 206d 6574 686f 6420 6f66 2060 6065  in method of ``e
-0000de50: 6461 7461 6060 2e20 2020 5468 6973 206f  data``.   This o
-0000de60: 6e6c 7920 6d61 7474 6572 7320 7768 656e  nly matters when
-0000de70: 2074 6865 2062 616c 6c6f 7473 2061 7265   the ballots are
-0000de80: 206e 6f74 206c 696e 6561 7220 6f72 6465   not linear orde
-0000de90: 7273 2e20 0a0a 2020 2020 5265 7475 726e  rs. ..    Return
-0000dea0: 733a 200a 2020 2020 2020 2020 4120 736f  s: .        A so
-0000deb0: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
-0000dec0: 6469 6461 7465 732e 200a 0a20 2020 2022  didates. ..    "
-0000ded0: 2222 0a20 2020 200a 2020 2020 6375 7272  "".    .    curr
-0000dee0: 5f63 616e 6473 203d 2065 6461 7461 2e63  _cands = edata.c
-0000def0: 616e 6469 6461 7465 7320 6966 2063 7572  andidates if cur
-0000df00: 725f 6361 6e64 7320 6973 204e 6f6e 6520  r_cands is None 
-0000df10: 656c 7365 2063 7572 725f 6361 6e64 730a  else curr_cands.
-0000df20: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
-0000df30: 6374 696f 6e20 3d20 6564 6174 612e 6d61  ction = edata.ma
-0000df40: 7267 696e 2069 6620 7374 7265 6e67 7468  rgin if strength
-0000df50: 5f66 756e 6374 696f 6e20 6973 204e 6f6e  _function is Non
-0000df60: 6520 656c 7365 2073 7472 656e 6774 685f  e else strength_
-0000df70: 6675 6e63 7469 6f6e 2020 0a0a 2020 2020  function  ..    
-0000df80: 6d61 7463 6865 7320 3d20 5b28 612c 2062  matches = [(a, b
-0000df90: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
-0000dfa0: 696f 6e28 612c 2062 2929 2066 6f72 2061  ion(a, b)) for a
-0000dfb0: 2069 6e20 6375 7272 5f63 616e 6473 2066   in curr_cands f
-0000dfc0: 6f72 2062 2069 6e20 6375 7272 5f63 616e  or b in curr_can
-0000dfd0: 6473 2069 6620 6120 213d 2062 5d0a 2020  ds if a != b].  
-0000dfe0: 2020 736f 7274 6564 5f6d 6174 6368 6573    sorted_matches
-0000dff0: 203d 2073 6f72 7465 6428 6d61 7463 6865   = sorted(matche
-0000e000: 732c 2072 6576 6572 7365 3d54 7275 652c  s, reverse=True,
-0000e010: 206b 6579 3d6c 616d 6264 6120 6d5f 775f   key=lambda m_w_
-0000e020: 7765 6967 6874 3a20 6d5f 775f 7765 6967  weight: m_w_weig
-0000e030: 6874 5b32 5d29 0a20 2020 200a 2020 2020  ht[2]).    .    
-0000e040: 7265 7475 726e 2073 6f72 7465 6428 5f73  return sorted(_s
-0000e050: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
-0000e060: 696e 6728 6375 7272 5f63 616e 6473 203d  ing(curr_cands =
-0000e070: 2063 7572 725f 6361 6e64 732c 200a 2020   curr_cands, .  
-0000e080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0a0: 2020 2020 2020 736f 7274 6564 5f6d 6174        sorted_mat
-0000e0b0: 6368 6573 203d 2073 6f72 7465 645f 6d61  ches = sorted_ma
-0000e0c0: 7463 6865 732c 0a20 2020 2020 2020 2020  tches,.         
-0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0e0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000e0f0: 656d 5f73 765f 7769 6e6e 6572 7320 3d20  em_sv_winners = 
-0000e100: 7b7d 295b 305d 290a 0a0a 4076 6d28 6e61  {})[0])...@vm(na
-0000e110: 6d65 203d 2022 5369 6d70 6c65 2053 7461  me = "Simple Sta
-0000e120: 626c 6520 566f 7469 6e67 2229 0a64 6566  ble Voting").def
-0000e130: 2073 696d 706c 655f 7374 6162 6c65 5f76   simple_stable_v
-0000e140: 6f74 696e 6728 0a20 2020 2065 6461 7461  oting(.    edata
-0000e150: 2c20 0a20 2020 2063 7572 725f 6361 6e64  , .    curr_cand
-0000e160: 733d 4e6f 6e65 2c20 0a20 2020 2073 7472  s=None, .    str
-0000e170: 656e 6774 685f 6675 6e63 7469 6f6e 3d4e  ength_function=N
-0000e180: 6f6e 652c 0a20 2020 2061 6c67 6f72 6974  one,.    algorit
-0000e190: 686d 203d 2027 6261 7369 6327 293a 200a  hm = 'basic'): .
-0000e1a0: 0a20 2020 2022 2222 496d 706c 656d 656e  .    """Implemen
-0000e1b0: 7461 7469 6f6e 206f 6620 5369 6d70 6c65  tation of Simple
-0000e1c0: 2053 7461 626c 6520 566f 7469 6e67 2066   Stable Voting f
-0000e1d0: 726f 6d20 6874 7470 733a 2f2f 6172 7869  rom https://arxi
-0000e1e0: 762e 6f72 672f 6162 732f 3231 3038 2e30  v.org/abs/2108.0
-0000e1f0: 3035 3432 2e20 0a0a 2020 2020 5369 6d70  0542. ..    Simp
-0000e200: 6c65 2053 7461 626c 6520 566f 7469 6e67  le Stable Voting
-0000e210: 2069 7320 6120 7265 6375 7273 6976 6520   is a recursive 
-0000e220: 766f 7469 6e67 206d 6574 686f 6420 6465  voting method de
-0000e230: 6669 6e65 6420 6173 2066 6f6c 6c6f 7773  fined as follows
-0000e240: 3a20 0a0a 2020 2020 312e 2049 6620 7468  : ..    1. If th
-0000e250: 6572 6520 6973 206f 6e6c 7920 6f6e 6520  ere is only one 
-0000e260: 6361 6e64 6964 6174 6520 696e 2074 6865  candidate in the
-0000e270: 2070 726f 6669 6c65 2c20 7468 656e 2074   profile, then t
-0000e280: 6861 7420 6361 6e64 6964 6174 6520 6973  hat candidate is
-0000e290: 2074 6865 2077 696e 6e65 722e 200a 2020   the winner. .  
-0000e2a0: 2020 322e 204f 7264 6572 2074 6865 2070    2. Order the p
-0000e2b0: 6169 7273 203a 6d61 7468 3a60 2861 2c62  airs :math:`(a,b
-0000e2c0: 2960 206f 6620 6361 6e64 6964 6174 6573  )` of candidates
-0000e2d0: 2066 726f 6d20 6c61 7267 6573 7420 746f   from largest to
-0000e2e0: 2073 6d61 6c6c 6573 7420 7661 6c75 6520   smallest value 
-0000e2f0: 6f66 2074 6865 206d 6172 6769 6e20 6f66  of the margin of
-0000e300: 203a 6d61 7468 3a60 6160 206f 7665 7220   :math:`a` over 
-0000e310: 3a6d 6174 683a 6062 602c 2061 6e64 2064  :math:`b`, and d
-0000e320: 6563 6c61 7265 2061 7320 5369 6d70 6c65  eclare as Simple
-0000e330: 2053 7461 626c 6520 566f 7469 6e67 2077   Stable Voting w
-0000e340: 696e 6e65 7273 2074 6865 2063 616e 6469  inners the candi
-0000e350: 6461 7465 2873 2920 3a6d 6174 683a 6061  date(s) :math:`a
-0000e360: 6020 6672 6f6d 2074 6865 2065 6172 6c69  ` from the earli
-0000e370: 6573 7420 7061 6972 2873 2920 3a6d 6174  est pair(s) :mat
-0000e380: 683a 6028 612c 6229 6020 7375 6368 2074  h:`(a,b)` such t
-0000e390: 6861 7420 3a6d 6174 683a 6061 6020 6973  hat :math:`a` is
-0000e3a0: 2061 2053 696d 706c 6520 5374 6162 6c65   a Simple Stable
-0000e3b0: 2056 6f74 696e 6720 7769 6e6e 6572 2069   Voting winner i
-0000e3c0: 6e20 7468 6520 656c 6563 7469 6f6e 2077  n the election w
-0000e3d0: 6974 686f 7574 203a 6d61 7468 3a60 6260  ithout :math:`b`
-0000e3e0: 2e20 0a0a 2020 2020 4172 6773 3a0a 2020  . ..    Args:.  
-0000e3f0: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
-0000e400: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
-0000e410: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
-0000e420: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
-0000e430: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
-0000e440: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
-0000e450: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
-0000e460: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
-0000e470: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
-0000e480: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
-0000e490: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
-0000e4a0: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
-0000e4b0: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
-0000e4c0: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
-0000e4d0: 7272 5f63 616e 6473 6060 0a20 2020 2020  rr_cands``.     
-0000e4e0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-0000e4f0: 7469 6f6e 2028 6675 6e63 7469 6f6e 2c20  tion (function, 
-0000e500: 6f70 7469 6f6e 616c 293a 2054 6865 2073  optional): The s
-0000e510: 7472 656e 6774 6820 6675 6e63 7469 6f6e  trength function
-0000e520: 2074 6f20 6265 2075 7365 6420 746f 2063   to be used to c
-0000e530: 616c 6375 6c61 7465 2074 6865 2073 7472  alculate the str
-0000e540: 656e 6774 6820 6f66 2061 2070 6174 682e  ength of a path.
-0000e550: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
-0000e560: 7320 7468 6520 6d61 7267 696e 206d 6574  s the margin met
-0000e570: 686f 6420 6f66 2060 6065 6461 7461 6060  hod of ``edata``
-0000e580: 2e20 2020 5468 6973 206f 6e6c 7920 6d61  .   This only ma
-0000e590: 7474 6572 7320 7768 656e 2074 6865 2062  tters when the b
-0000e5a0: 616c 6c6f 7473 2061 7265 206e 6f74 206c  allots are not l
-0000e5b0: 696e 6561 7220 6f72 6465 7273 2e20 0a20  inear orders. . 
-0000e5c0: 2020 2020 2020 2061 6c67 6f72 6974 686d         algorithm
-0000e5d0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-0000e5e0: 3a20 5370 6563 6966 7920 7768 6963 6820  : Specify which 
-0000e5f0: 616c 676f 7269 7468 6d20 746f 2075 7365  algorithm to use
-0000e600: 2e20 204f 7074 696f 6e73 2061 7265 2027  .  Options are '
-0000e610: 6261 7369 6327 2028 7468 6520 6465 6661  basic' (the defa
-0000e620: 756c 7429 2061 6e64 2027 7769 7468 5f63  ult) and 'with_c
-0000e630: 6f6e 646f 7263 6574 5f63 6865 636b 272e  ondorcet_check'.
-0000e640: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
-0000e650: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
-0000e660: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
-0000e670: 7465 732e 200a 0a20 2020 202e 2e20 7365  tes. ..    .. se
-0000e680: 6561 6c73 6f3a 3a0a 0a20 2020 2020 2020  ealso::..       
-0000e690: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
-0000e6a0: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
-0000e6b0: 5f6d 6574 686f 6473 2e73 696d 706c 655f  _methods.simple_
-0000e6c0: 7374 6162 6c65 5f76 6f74 696e 675f 6661  stable_voting_fa
-0000e6d0: 7374 6572 602c 203a 6d65 7468 3a60 7072  ster`, :meth:`pr
-0000e6e0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-0000e6f0: 5f62 6173 6564 5f6d 6574 686f 6473 2e73  _based_methods.s
-0000e700: 7461 626c 655f 766f 7469 6e67 600a 0a20  table_voting`.. 
-0000e710: 2020 203a 4578 616d 706c 653a 200a 0a20     :Example: .. 
-0000e720: 2020 202e 2e20 6578 6563 5f63 6f64 653a     .. exec_code:
-0000e730: 3a0a 0a20 2020 2020 2020 2066 726f 6d20  :..        from 
-0000e740: 7072 6566 5f76 6f74 696e 672e 7765 6967  pref_voting.weig
-0000e750: 6874 6564 5f6d 616a 6f72 6974 795f 6772  hted_majority_gr
-0000e760: 6170 6873 2069 6d70 6f72 7420 4d61 7267  aphs import Marg
-0000e770: 696e 4772 6170 680a 2020 2020 2020 2020  inGraph.        
-0000e780: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
-0000e790: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-0000e7a0: 7468 6f64 7320 696d 706f 7274 2073 696d  thods import sim
-0000e7b0: 706c 655f 7374 6162 6c65 5f76 6f74 696e  ple_stable_votin
-0000e7c0: 670a 0a20 2020 2020 2020 206d 6720 3d20  g..        mg = 
-0000e7d0: 4d61 7267 696e 4772 6170 6828 5b30 2c20  MarginGraph([0, 
-0000e7e0: 312c 2032 2c20 335d 2c20 5b28 302c 2033  1, 2, 3], [(0, 3
-0000e7f0: 2c20 3829 2c20 2831 2c20 302c 2031 3029  , 8), (1, 0, 10)
-0000e800: 2c20 2832 2c20 302c 2034 292c 2028 322c  , (2, 0, 4), (2,
-0000e810: 2031 2c20 3829 2c20 2833 2c20 312c 2038   1, 8), (3, 1, 8
-0000e820: 295d 290a 0a20 2020 2020 2020 2073 696d  )])..        sim
-0000e830: 706c 655f 7374 6162 6c65 5f76 6f74 696e  ple_stable_votin
-0000e840: 672e 6469 7370 6c61 7928 6d67 290a 2020  g.display(mg).  
-0000e850: 2020 2020 2020 7369 6d70 6c65 5f73 7461        simple_sta
-0000e860: 626c 655f 766f 7469 6e67 2e64 6973 706c  ble_voting.displ
-0000e870: 6179 286d 672c 2061 6c67 6f72 6974 686d  ay(mg, algorithm
-0000e880: 3d27 6261 7369 6327 290a 2020 2020 2020  ='basic').      
-0000e890: 2020 7369 6d70 6c65 5f73 7461 626c 655f    simple_stable_
-0000e8a0: 766f 7469 6e67 2e64 6973 706c 6179 286d  voting.display(m
-0000e8b0: 672c 2061 6c67 6f72 6974 686d 3d27 7769  g, algorithm='wi
-0000e8c0: 7468 5f63 6f6e 646f 7263 6574 5f63 6865  th_condorcet_che
-0000e8d0: 636b 2729 0a0a 2020 2020 2222 220a 2020  ck')..    """.  
-0000e8e0: 2020 0a20 2020 2069 6620 616c 676f 7269    .    if algori
-0000e8f0: 7468 6d20 3d3d 2027 6261 7369 6327 3a20  thm == 'basic': 
-0000e900: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000e910: 5f73 696d 706c 655f 7374 6162 6c65 5f76  _simple_stable_v
-0000e920: 6f74 696e 675f 6261 7369 6328 6564 6174  oting_basic(edat
-0000e930: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
-0000e940: 6375 7272 5f63 616e 6473 2c20 7374 7265  curr_cands, stre
-0000e950: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-0000e960: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000e970: 6e29 0a20 2020 2065 6c69 6620 616c 676f  n).    elif algo
-0000e980: 7269 7468 6d20 3d3d 2027 7769 7468 5f63  rithm == 'with_c
-0000e990: 6f6e 646f 7263 6574 5f63 6865 636b 273a  ondorcet_check':
-0000e9a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000e9b0: 5f73 696d 706c 655f 7374 6162 6c65 5f76  _simple_stable_v
-0000e9c0: 6f74 696e 675f 7769 7468 5f63 6f6e 646f  oting_with_condo
-0000e9d0: 7263 6574 5f63 6865 636b 2865 6461 7461  rcet_check(edata
-0000e9e0: 2c20 6375 7272 5f63 616e 6473 203d 2063  , curr_cands = c
-0000e9f0: 7572 725f 6361 6e64 732c 2073 7472 656e  urr_cands, stren
-0000ea00: 6774 685f 6675 6e63 7469 6f6e 203d 2073  gth_function = s
-0000ea10: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000ea20: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-0000ea30: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000ea40: 7272 6f72 2822 496e 7661 6c69 6420 616c  rror("Invalid al
-0000ea50: 676f 7269 7468 6d20 7370 6563 6966 6965  gorithm specifie
-0000ea60: 642e 2229 0a20 2020 200a 0a64 6566 205f  d.").    ..def _
-0000ea70: 7374 6162 6c65 5f76 6f74 696e 6728 6564  stable_voting(ed
-0000ea80: 6174 612c 200a 2020 2020 2020 2020 2020  ata, .          
-0000ea90: 2020 2020 2020 2020 2063 7572 725f 6361           curr_ca
-0000eaa0: 6e64 732c 0a20 2020 2020 2020 2020 2020  nds,.           
-0000eab0: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
-0000eac0: 5f66 756e 6374 696f 6e2c 0a20 2020 2020  _function,.     
-0000ead0: 2020 2020 2020 2020 2020 2020 2020 736f                so
-0000eae0: 7274 6564 5f6d 6174 6368 6573 2c0a 2020  rted_matches,.  
-0000eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb00: 206d 656d 5f73 765f 7769 6e6e 6572 7329   mem_sv_winners)
-0000eb10: 3a20 0a20 2020 2027 2727 0a20 2020 2044  : .    '''.    D
-0000eb20: 6574 6572 6d69 6e65 2074 6865 2053 7461  etermine the Sta
-0000eb30: 626c 6520 566f 7469 6e67 2077 696e 6e65  ble Voting winne
-0000eb40: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
-0000eb50: 6c65 2077 6869 6c65 206b 6565 7069 6e67  le while keeping
-0000eb60: 2074 7261 636b 206f 6620 7468 6520 7769   track of the wi
-0000eb70: 6e6e 6572 7320 696e 2061 6e79 2073 7562  nners in any sub
-0000eb80: 7072 6f66 696c 6573 2063 6865 636b 6564  profiles checked
-0000eb90: 2064 7572 696e 6720 636f 6d70 7574 6174   during computat
-0000eba0: 696f 6e2e 200a 2020 2020 2727 270a 2020  ion. .    '''.  
-0000ebb0: 2020 0a20 2020 2073 765f 7769 6e6e 6572    .    sv_winner
-0000ebc0: 7320 3d20 6c69 7374 2829 0a20 2020 200a  s = list().    .
-0000ebd0: 2020 2020 756e 6465 6665 6174 6564 5f63      undefeated_c
-0000ebe0: 616e 6469 6461 7465 7320 3d20 7370 6c69  andidates = spli
-0000ebf0: 745f 6379 636c 6528 6564 6174 612c 2063  t_cycle(edata, c
-0000ec00: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
-0000ec10: 5f63 616e 6473 2c20 7374 7265 6e67 7468  _cands, strength
-0000ec20: 5f66 756e 6374 696f 6e20 3d20 7374 7265  _function = stre
-0000ec30: 6e67 7468 5f66 756e 6374 696f 6e29 0a0a  ngth_function)..
-0000ec40: 2020 2020 6966 206c 656e 2863 7572 725f      if len(curr_
-0000ec50: 6361 6e64 7329 203d 3d20 313a 200a 2020  cands) == 1: .  
-0000ec60: 2020 2020 2020 6d65 6d5f 7376 5f77 696e        mem_sv_win
-0000ec70: 6e65 7273 5b74 7570 6c65 2863 7572 725f  ners[tuple(curr_
-0000ec80: 6361 6e64 7329 5d20 3d20 6375 7272 5f63  cands)] = curr_c
-0000ec90: 616e 6473 0a20 2020 2020 2020 2072 6574  ands.        ret
-0000eca0: 7572 6e20 6375 7272 5f63 616e 6473 2c20  urn curr_cands, 
-0000ecb0: 6d65 6d5f 7376 5f77 696e 6e65 7273 0a20  mem_sv_winners. 
-0000ecc0: 2020 200a 2020 2020 6d61 7267 696e 5f77     .    margin_w
-0000ecd0: 6974 6e65 7373 696e 675f 7769 6e20 3d20  itnessing_win = 
-0000ece0: 2d6d 6174 682e 696e 660a 0a20 2020 2066  -math.inf..    f
-0000ecf0: 6f72 2061 2c20 622c 2073 2069 6e20 736f  or a, b, s in so
-0000ed00: 7274 6564 5f6d 6174 6368 6573 3a0a 2020  rted_matches:.  
-0000ed10: 2020 2020 2020 6966 2073 203c 206d 6172        if s < mar
-0000ed20: 6769 6e5f 7769 746e 6573 7369 6e67 5f77  gin_witnessing_w
-0000ed30: 696e 3a20 0a20 2020 2020 2020 2020 2020  in: .           
-0000ed40: 2062 7265 616b 0a20 2020 2020 2020 2069   break.        i
-0000ed50: 6620 6120 696e 2075 6e64 6566 6561 7465  f a in undefeate
-0000ed60: 645f 6361 6e64 6964 6174 6573 2061 6e64  d_candidates and
-0000ed70: 2061 206e 6f74 2069 6e20 7376 5f77 696e   a not in sv_win
-0000ed80: 6e65 7273 3a20 0a20 2020 2020 2020 2020  ners: .         
-0000ed90: 2020 2063 616e 6473 5f6d 696e 7573 5f62     cands_minus_b
-0000eda0: 203d 205b 6320 666f 7220 6320 696e 2063   = [c for c in c
-0000edb0: 7572 725f 6361 6e64 7320 6966 2063 2021  urr_cands if c !
-0000edc0: 3d20 625d 0a20 2020 2020 2020 2020 2020  = b].           
-0000edd0: 2063 616e 6473 5f6d 696e 7573 5f62 5f6b   cands_minus_b_k
-0000ede0: 6579 203d 2074 7570 6c65 2873 6f72 7465  ey = tuple(sorte
-0000edf0: 6428 6361 6e64 735f 6d69 6e75 735f 6229  d(cands_minus_b)
-0000ee00: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000ee10: 2063 616e 6473 5f6d 696e 7573 5f62 5f6b   cands_minus_b_k
-0000ee20: 6579 206e 6f74 2069 6e20 6d65 6d5f 7376  ey not in mem_sv
-0000ee30: 5f77 696e 6e65 7273 2e6b 6579 7328 293a  _winners.keys():
-0000ee40: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0000ee50: 2020 7773 2c20 6d65 6d5f 7376 5f77 696e    ws, mem_sv_win
-0000ee60: 6e65 7273 203d 205f 7374 6162 6c65 5f76  ners = _stable_v
-0000ee70: 6f74 696e 6728 6564 6174 612c 0a20 2020  oting(edata,.   
-0000ee80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eeb0: 2063 7572 725f 6361 6e64 7320 3d20 6361   curr_cands = ca
-0000eec0: 6e64 735f 6d69 6e75 735f 622c 0a20 2020  nds_minus_b,.   
-0000eed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef00: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000ef10: 6f6e 203d 2073 7472 656e 6774 685f 6675  on = strength_fu
-0000ef20: 6e63 7469 6f6e 2c0a 2020 2020 2020 2020  nction,.        
-0000ef30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef50: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-0000ef60: 6564 5f6d 6174 6368 6573 203d 205b 2861  ed_matches = [(a
-0000ef70: 2c20 632c 2073 2920 666f 7220 612c 2063  , c, s) for a, c
-0000ef80: 2c20 7320 696e 2073 6f72 7465 645f 6d61  , s in sorted_ma
-0000ef90: 7463 6865 7320 6966 2061 2021 3d20 6220  tches if a != b 
-0000efa0: 616e 6420 6320 213d 2062 5d2c 0a20 2020  and c != b],.   
-0000efb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efe0: 206d 656d 5f73 765f 7769 6e6e 6572 7320   mem_sv_winners 
-0000eff0: 3d20 6d65 6d5f 7376 5f77 696e 6e65 7273  = mem_sv_winners
-0000f000: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f010: 2020 6d65 6d5f 7376 5f77 696e 6e65 7273    mem_sv_winners
-0000f020: 5b63 616e 6473 5f6d 696e 7573 5f62 5f6b  [cands_minus_b_k
-0000f030: 6579 5d20 3d20 7773 0a20 2020 2020 2020  ey] = ws.       
-0000f040: 2020 2020 2065 6c73 653a 200a 2020 2020       else: .    
-0000f050: 2020 2020 2020 2020 2020 2020 7773 203d              ws =
-0000f060: 206d 656d 5f73 765f 7769 6e6e 6572 735b   mem_sv_winners[
-0000f070: 6361 6e64 735f 6d69 6e75 735f 625f 6b65  cands_minus_b_ke
-0000f080: 795d 0a20 2020 2020 2020 2020 2020 2069  y].            i
-0000f090: 6620 6120 696e 2077 733a 0a20 2020 2020  f a in ws:.     
-0000f0a0: 2020 2020 2020 2020 2020 2073 765f 7769             sv_wi
-0000f0b0: 6e6e 6572 732e 6170 7065 6e64 2861 290a  nners.append(a).
-0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0d0: 6d61 7267 696e 5f77 6974 6e65 7373 696e  margin_witnessin
-0000f0e0: 675f 7769 6e20 3d20 730a 2020 2020 2020  g_win = s.      
-0000f0f0: 2020 2020 2020 2020 2020 0a20 2020 2072            .    r
-0000f100: 6574 7572 6e20 7376 5f77 696e 6e65 7273  eturn sv_winners
-0000f110: 2c20 6d65 6d5f 7376 5f77 696e 6e65 7273  , mem_sv_winners
-0000f120: 0a20 2020 2020 2020 200a 4076 6d28 6e61  .        .@vm(na
-0000f130: 6d65 203d 2022 5374 6162 6c65 2056 6f74  me = "Stable Vot
-0000f140: 696e 6722 290a 6465 6620 5f73 7461 626c  ing").def _stabl
-0000f150: 655f 766f 7469 6e67 5f77 6974 685f 636f  e_voting_with_co
-0000f160: 6e64 6f72 6365 745f 6368 6563 6b28 0a20  ndorcet_check(. 
-0000f170: 2020 2065 6461 7461 2c20 0a20 2020 2063     edata, .    c
-0000f180: 7572 725f 6361 6e64 733d 4e6f 6e65 2c20  urr_cands=None, 
-0000f190: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
-0000f1a0: 6e63 7469 6f6e 3d4e 6f6e 6529 3a20 0a20  nction=None): . 
-0000f1b0: 2020 2022 2222 0a20 2020 2053 7461 626c     """.    Stabl
-0000f1c0: 6520 566f 7469 6e67 2069 7320 436f 6e64  e Voting is Cond
-0000f1d0: 6f72 6365 7420 636f 6e73 6973 7465 6e74  orcet consistent
-0000f1e0: 2e20 2020 4974 2069 7320 6661 7374 6572  .   It is faster
-0000f1f0: 2074 6f20 736b 6970 2065 7865 6375 7469   to skip executi
-0000f200: 6e67 2074 6865 2072 6563 7572 7369 7665  ng the recursive
-0000f210: 2061 6c67 6f72 6974 686d 2077 6865 6e20   algorithm when 
-0000f220: 7468 6572 6520 6973 2061 2043 6f6e 646f  there is a Condo
-0000f230: 7263 6574 2077 696e 6e65 722e 2020 0a0a  rcet winner.  ..
-0000f240: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000f250: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
-0000f260: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
-0000f270: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
-0000f280: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
-0000f290: 7461 2074 6861 7420 6861 7320 6120 606d  ta that has a `m
-0000f2a0: 6172 6769 6e60 206d 6574 686f 642e 200a  argin` method. .
-0000f2b0: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
-0000f2c0: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
-0000f2d0: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
-0000f2e0: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
-0000f2f0: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
-0000f300: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
-0000f310: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
-0000f320: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
-0000f330: 616e 6473 6060 0a20 2020 2020 2020 2073  ands``.        s
-0000f340: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000f350: 2028 6675 6e63 7469 6f6e 2c20 6f70 7469   (function, opti
-0000f360: 6f6e 616c 293a 2054 6865 2073 7472 656e  onal): The stren
-0000f370: 6774 6820 6675 6e63 7469 6f6e 2074 6f20  gth function to 
-0000f380: 6265 2075 7365 6420 746f 2063 616c 6375  be used to calcu
-0000f390: 6c61 7465 2074 6865 2073 7472 656e 6774  late the strengt
-0000f3a0: 6820 6f66 2061 2070 6174 682e 2020 2054  h of a path.   T
-0000f3b0: 6865 2064 6566 6175 6c74 2069 7320 7468  he default is th
-0000f3c0: 6520 6d61 7267 696e 206d 6574 686f 6420  e margin method 
-0000f3d0: 6f66 2060 6065 6461 7461 6060 2e20 2020  of ``edata``.   
-0000f3e0: 5468 6973 206f 6e6c 7920 6d61 7474 6572  This only matter
-0000f3f0: 7320 7768 656e 2074 6865 2062 616c 6c6f  s when the ballo
-0000f400: 7473 2061 7265 206e 6f74 206c 696e 6561  ts are not linea
-0000f410: 7220 6f72 6465 7273 2e20 0a0a 2020 2020  r orders. ..    
-0000f420: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
-0000f430: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
-0000f440: 6f66 2063 616e 6469 6461 7465 732e 200a  of candidates. .
-0000f450: 0a20 2020 2022 2222 0a20 2020 2063 7720  .    """.    cw 
-0000f460: 3d20 6564 6174 612e 636f 6e64 6f72 6365  = edata.condorce
-0000f470: 745f 7769 6e6e 6572 2863 7572 725f 6361  t_winner(curr_ca
-0000f480: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
-0000f490: 290a 2020 2020 6966 2063 7720 6973 206e  ).    if cw is n
-0000f4a0: 6f74 204e 6f6e 653a 200a 2020 2020 2020  ot None: .      
-0000f4b0: 2020 7265 7475 726e 205b 6377 5d0a 2020    return [cw].  
-0000f4c0: 2020 656c 7365 3a20 0a20 2020 2020 2020    else: .       
-0000f4d0: 2063 7572 725f 6361 6e64 7320 3d20 6564   curr_cands = ed
-0000f4e0: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
-0000f4f0: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
-0000f500: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
-0000f510: 616e 6473 0a20 2020 2020 2020 2073 7472  ands.        str
-0000f520: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-0000f530: 2065 6461 7461 2e6d 6172 6769 6e20 6966   edata.margin if
-0000f540: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000f550: 6f6e 2069 7320 4e6f 6e65 2065 6c73 6520  on is None else 
-0000f560: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000f570: 6e20 200a 0a20 2020 2020 2020 206d 6174  n  ..        mat
-0000f580: 6368 6573 203d 205b 2861 2c20 622c 2073  ches = [(a, b, s
-0000f590: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000f5a0: 2861 2c20 6229 2920 666f 7220 6120 696e  (a, b)) for a in
-0000f5b0: 2063 7572 725f 6361 6e64 7320 666f 7220   curr_cands for 
-0000f5c0: 6220 696e 2063 7572 725f 6361 6e64 7320  b in curr_cands 
-0000f5d0: 6966 2061 2021 3d20 625d 0a20 2020 2020  if a != b].     
-0000f5e0: 2020 2073 6f72 7465 645f 6d61 7463 6865     sorted_matche
-0000f5f0: 7320 3d20 736f 7274 6564 286d 6174 6368  s = sorted(match
-0000f600: 6573 2c20 7265 7665 7273 653d 5472 7565  es, reverse=True
-0000f610: 2c20 6b65 793d 6c61 6d62 6461 206d 5f77  , key=lambda m_w
-0000f620: 5f77 6569 6768 743a 206d 5f77 5f77 6569  _weight: m_w_wei
-0000f630: 6768 745b 325d 290a 0a20 2020 2020 2020  ght[2])..       
-0000f640: 2072 6574 7572 6e20 736f 7274 6564 285f   return sorted(_
-0000f650: 7374 6162 6c65 5f76 6f74 696e 6728 6564  stable_voting(ed
-0000f660: 6174 612c 200a 2020 2020 2020 2020 2020  ata, .          
-0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f680: 2020 2020 2020 2020 2020 6375 7272 5f63            curr_c
-0000f690: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
-0000f6a0: 732c 200a 2020 2020 2020 2020 2020 2020  s, .            
-0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6c0: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
-0000f6d0: 5f66 756e 6374 696f 6e20 3d20 7374 7265  _function = stre
-0000f6e0: 6e67 7468 5f66 756e 6374 696f 6e2c 0a20  ngth_function,. 
-0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f710: 2020 2073 6f72 7465 645f 6d61 7463 6865     sorted_matche
-0000f720: 7320 3d20 736f 7274 6564 5f6d 6174 6368  s = sorted_match
-0000f730: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-0000f740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f750: 2020 2020 2020 2020 6d65 6d5f 7376 5f77          mem_sv_w
-0000f760: 696e 6e65 7273 203d 207b 7d29 5b30 5d29  inners = {})[0])
-0000f770: 0a0a 6465 6620 5f73 7461 626c 655f 766f  ..def _stable_vo
-0000f780: 7469 6e67 5f62 6173 6963 280a 2020 2020  ting_basic(.    
-0000f790: 2020 2020 6564 6174 612c 200a 2020 2020      edata, .    
-0000f7a0: 2020 2020 6375 7272 5f63 616e 6473 203d      curr_cands =
-0000f7b0: 204e 6f6e 652c 200a 2020 2020 2020 2020   None, .        
-0000f7c0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000f7d0: 6e20 3d20 4e6f 6e65 293a 200a 2020 2020  n = None): .    
-0000f7e0: 2222 2249 6d70 6c65 6d65 6e74 6174 696f  """Implementatio
-0000f7f0: 6e20 6f66 2020 5374 6162 6c65 2056 6f74  n of  Stable Vot
-0000f800: 696e 6720 6672 6f6d 2068 7474 7073 3a2f  ing from https:/
-0000f810: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-0000f820: 3130 382e 3030 3534 322e 200a 0a20 2020  108.00542. ..   
-0000f830: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
-0000f840: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
-0000f850: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
-0000f860: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
-0000f870: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
-0000f880: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
-0000f890: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
-0000f8a0: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-0000f8b0: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-0000f8c0: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-0000f8d0: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-0000f8e0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-0000f8f0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-0000f900: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-0000f910: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-0000f920: 7360 600a 2020 2020 2020 2020 7374 7265  s``.        stre
-0000f930: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
-0000f940: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
-0000f950: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
-0000f960: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
-0000f970: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
-0000f980: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
-0000f990: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
-0000f9a0: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
-0000f9b0: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
-0000f9c0: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
-0000f9d0: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
-0000f9e0: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
-0000f9f0: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
-0000fa00: 7264 6572 732e 200a 0a20 2020 2052 6574  rders. ..    Ret
-0000fa10: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
-0000fa20: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
-0000fa30: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
-0000fa40: 2020 2222 220a 0a20 2020 2063 7572 725f    """..    curr_
-0000fa50: 6361 6e64 7320 3d20 6564 6174 612e 6361  cands = edata.ca
-0000fa60: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
-0000fa70: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
-0000fa80: 6c73 6520 6375 7272 5f63 616e 6473 0a20  lse curr_cands. 
-0000fa90: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-0000faa0: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
-0000fab0: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
-0000fac0: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
-0000fad0: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
-0000fae0: 756e 6374 696f 6e20 200a 0a20 2020 206d  unction  ..    m
-0000faf0: 6174 6368 6573 203d 205b 2861 2c20 622c  atches = [(a, b,
-0000fb00: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000fb10: 6f6e 2861 2c20 6229 2920 666f 7220 6120  on(a, b)) for a 
-0000fb20: 696e 2063 7572 725f 6361 6e64 7320 666f  in curr_cands fo
-0000fb30: 7220 6220 696e 2063 7572 725f 6361 6e64  r b in curr_cand
-0000fb40: 7320 6966 2061 2021 3d20 625d 0a20 2020  s if a != b].   
-0000fb50: 2073 6f72 7465 645f 6d61 7463 6865 7320   sorted_matches 
-0000fb60: 3d20 736f 7274 6564 286d 6174 6368 6573  = sorted(matches
-0000fb70: 2c20 7265 7665 7273 653d 5472 7565 2c20  , reverse=True, 
-0000fb80: 6b65 793d 6c61 6d62 6461 206d 5f77 5f77  key=lambda m_w_w
-0000fb90: 6569 6768 743a 206d 5f77 5f77 6569 6768  eight: m_w_weigh
-0000fba0: 745b 325d 290a 0a20 2020 2072 6574 7572  t[2])..    retur
-0000fbb0: 6e20 736f 7274 6564 285f 7374 6162 6c65  n sorted(_stable
-0000fbc0: 5f76 6f74 696e 6728 6564 6174 612c 200a  _voting(edata, .
-0000fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbf0: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
-0000fc00: 7272 5f63 616e 6473 2c20 0a20 2020 2020  rr_cands, .     
-0000fc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc20: 2020 2020 2020 2020 2020 2020 7374 7265              stre
-0000fc30: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-0000fc40: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000fc50: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-0000fc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc70: 2020 2020 736f 7274 6564 5f6d 6174 6368      sorted_match
-0000fc80: 6573 203d 2073 6f72 7465 645f 6d61 7463  es = sorted_matc
-0000fc90: 6865 732c 0a20 2020 2020 2020 2020 2020  hes,.           
-0000fca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcb0: 2020 2020 2020 6d65 6d5f 7376 5f77 696e        mem_sv_win
-0000fcc0: 6e65 7273 203d 207b 7d29 5b30 5d29 0a0a  ners = {})[0])..
-0000fcd0: 0a0a 4076 6d28 6e61 6d65 203d 2022 5374  ..@vm(name = "St
-0000fce0: 6162 6c65 2056 6f74 696e 6722 290a 6465  able Voting").de
-0000fcf0: 6620 7374 6162 6c65 5f76 6f74 696e 6728  f stable_voting(
-0000fd00: 0a20 2020 2065 6461 7461 2c20 0a20 2020  .    edata, .   
-0000fd10: 2063 7572 725f 6361 6e64 733d 4e6f 6e65   curr_cands=None
-0000fd20: 2c20 0a20 2020 2073 7472 656e 6774 685f  , .    strength_
-0000fd30: 6675 6e63 7469 6f6e 3d4e 6f6e 652c 200a  function=None, .
-0000fd40: 2020 2020 616c 676f 7269 7468 6d3d 2762      algorithm='b
-0000fd50: 6173 6963 2729 3a20 0a20 2020 2022 2222  asic'): .    """
-0000fd60: 496d 706c 656d 656e 7461 7469 6f6e 206f  Implementation o
-0000fd70: 6620 2053 7461 626c 6520 566f 7469 6e67  f  Stable Voting
-0000fd80: 2066 726f 6d20 6874 7470 733a 2f2f 6172   from https://ar
-0000fd90: 7869 762e 6f72 672f 6162 732f 3231 3038  xiv.org/abs/2108
-0000fda0: 2e30 3035 3432 2e20 0a0a 2020 2020 5374  .00542. ..    St
-0000fdb0: 6162 6c65 2056 6f74 696e 6720 6973 2061  able Voting is a
-0000fdc0: 2072 6563 7572 7369 7665 2076 6f74 696e   recursive votin
-0000fdd0: 6720 6d65 7468 6f64 2064 6566 696e 6564  g method defined
-0000fde0: 2061 7320 666f 6c6c 6f77 733a 200a 0a20   as follows: .. 
-0000fdf0: 2020 2031 2e20 2049 6620 7468 6572 6520     1.  If there 
-0000fe00: 6973 206f 6e6c 7920 6f6e 6520 6361 6e64  is only one cand
-0000fe10: 6964 6174 6520 696e 2074 6865 2070 726f  idate in the pro
-0000fe20: 6669 6c65 2c20 7468 656e 2074 6861 7420  file, then that 
-0000fe30: 6361 6e64 6964 6174 6520 6973 2074 6865  candidate is the
-0000fe40: 2077 696e 6e65 722e 200a 2020 2020 322e   winner. .    2.
-0000fe50: 204f 7264 6572 2074 6865 2070 6169 7273   Order the pairs
-0000fe60: 203a 6d61 7468 3a60 2861 2c62 2960 206f   :math:`(a,b)` o
-0000fe70: 6620 6361 6e64 6964 6174 6573 2066 726f  f candidates fro
-0000fe80: 6d20 6c61 7267 6573 7420 746f 2073 6d61  m largest to sma
-0000fe90: 6c6c 6573 7420 7661 6c75 6520 6f66 2074  llest value of t
-0000fea0: 6865 206d 6172 6769 6e20 6f66 203a 6d61  he margin of :ma
-0000feb0: 7468 3a60 6160 206f 7665 7220 3a6d 6174  th:`a` over :mat
-0000fec0: 683a 6062 6020 7375 6368 2074 6861 7420  h:`b` such that 
-0000fed0: 3a6d 6174 683a 6061 6020 6973 2075 6e64  :math:`a` is und
-0000fee0: 6566 6561 7465 6420 6163 636f 7264 696e  efeated accordin
-0000fef0: 6720 746f 2053 706c 6974 2043 7963 6c65  g to Split Cycle
-0000ff00: 2c20 616e 6420 6465 636c 6172 6520 6173  , and declare as
-0000ff10: 2053 7461 626c 6520 566f 7469 6e67 2077   Stable Voting w
-0000ff20: 696e 6e65 7273 2074 6865 2063 616e 6469  inners the candi
-0000ff30: 6461 7465 2873 2920 3a6d 6174 683a 6061  date(s) :math:`a
-0000ff40: 6020 6672 6f6d 2074 6865 2065 6172 6c69  ` from the earli
-0000ff50: 6573 7420 7061 6972 2873 2920 3a6d 6174  est pair(s) :mat
-0000ff60: 683a 6028 612c 6229 6020 7375 6368 2074  h:`(a,b)` such t
-0000ff70: 6861 7420 3a6d 6174 683a 6061 6020 6973  hat :math:`a` is
-0000ff80: 2061 2053 696d 706c 6520 5374 6162 6c65   a Simple Stable
-0000ff90: 2056 6f74 696e 6720 7769 6e6e 6572 2069   Voting winner i
-0000ffa0: 6e20 7468 6520 656c 6563 7469 6f6e 2077  n the election w
-0000ffb0: 6974 686f 7574 203a 6d61 7468 3a60 6260  ithout :math:`b`
-0000ffc0: 2e20 0a0a 2020 2020 4172 6773 3a0a 2020  . ..    Args:.  
-0000ffd0: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
-0000ffe0: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
-0000fff0: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
-00010000: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
-00010010: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
-00010020: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
-00010030: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
-00010040: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
-00010050: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
-00010060: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
-00010070: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
-00010080: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
-00010090: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
-000100a0: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
-000100b0: 7272 5f63 616e 6473 6060 0a20 2020 2020  rr_cands``.     
-000100c0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-000100d0: 7469 6f6e 2028 6675 6e63 7469 6f6e 2c20  tion (function, 
-000100e0: 6f70 7469 6f6e 616c 293a 2054 6865 2073  optional): The s
-000100f0: 7472 656e 6774 6820 6675 6e63 7469 6f6e  trength function
-00010100: 2074 6f20 6265 2075 7365 6420 746f 2063   to be used to c
-00010110: 616c 6375 6c61 7465 2074 6865 2073 7472  alculate the str
-00010120: 656e 6774 6820 6f66 2061 2070 6174 682e  ength of a path.
-00010130: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
-00010140: 7320 7468 6520 6d61 7267 696e 206d 6574  s the margin met
-00010150: 686f 6420 6f66 2060 6065 6461 7461 6060  hod of ``edata``
-00010160: 2e20 2020 5468 6973 206f 6e6c 7920 6d61  .   This only ma
-00010170: 7474 6572 7320 7768 656e 2074 6865 2062  tters when the b
-00010180: 616c 6c6f 7473 2061 7265 206e 6f74 206c  allots are not l
-00010190: 696e 6561 7220 6f72 6465 7273 2e20 0a0a  inear orders. ..
-000101a0: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
-000101b0: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
-000101c0: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
-000101d0: 732e 200a 0a20 2020 202e 2e20 7365 6561  s. ..    .. seea
-000101e0: 6c73 6f3a 3a0a 0a20 2020 2020 2020 203a  lso::..        :
-000101f0: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-00010200: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-00010210: 6574 686f 6473 2e73 696d 706c 655f 7374  ethods.simple_st
-00010220: 6162 6c65 5f66 6173 7465 7260 2c20 3a6d  able_faster`, :m
-00010230: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
-00010240: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-00010250: 7468 6f64 732e 7369 6d70 6c65 5f73 7461  thods.simple_sta
-00010260: 626c 655f 766f 7469 6e67 600a 0a0a 2020  ble_voting`...  
-00010270: 2020 3a45 7861 6d70 6c65 3a20 0a0a 2020    :Example: ..  
-00010280: 2020 2e2e 2065 7865 635f 636f 6465 3a3a    .. exec_code::
-00010290: 0a0a 2020 2020 2020 2020 6672 6f6d 2070  ..        from p
-000102a0: 7265 665f 766f 7469 6e67 2e77 6569 6768  ref_voting.weigh
-000102b0: 7465 645f 6d61 6a6f 7269 7479 5f67 7261  ted_majority_gra
-000102c0: 7068 7320 696d 706f 7274 204d 6172 6769  phs import Margi
-000102d0: 6e47 7261 7068 0a20 2020 2020 2020 2066  nGraph.        f
-000102e0: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
-000102f0: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-00010300: 686f 6473 2069 6d70 6f72 7420 7374 6162  hods import stab
-00010310: 6c65 5f76 6f74 696e 670a 0a20 2020 2020  le_voting..     
-00010320: 2020 206d 6720 3d20 4d61 7267 696e 4772     mg = MarginGr
-00010330: 6170 6828 5b30 2c20 312c 2032 2c20 335d  aph([0, 1, 2, 3]
-00010340: 2c20 5b28 302c 2033 2c20 3829 2c20 2831  , [(0, 3, 8), (1
-00010350: 2c20 302c 2031 3029 2c20 2832 2c20 302c  , 0, 10), (2, 0,
-00010360: 2034 292c 2028 322c 2031 2c20 3829 2c20   4), (2, 1, 8), 
-00010370: 2833 2c20 312c 2038 295d 290a 0a20 2020  (3, 1, 8)])..   
-00010380: 2020 2020 2073 7461 626c 655f 766f 7469       stable_voti
-00010390: 6e67 2e64 6973 706c 6179 286d 6729 0a20  ng.display(mg). 
-000103a0: 2020 2020 2020 2073 7461 626c 655f 766f         stable_vo
-000103b0: 7469 6e67 2e64 6973 706c 6179 286d 672c  ting.display(mg,
-000103c0: 2061 6c67 6f72 6974 686d 3d27 6261 7369   algorithm='basi
-000103d0: 6327 290a 2020 2020 2020 2020 7374 6162  c').        stab
-000103e0: 6c65 5f76 6f74 696e 672e 6469 7370 6c61  le_voting.displa
-000103f0: 7928 6d67 2c20 616c 676f 7269 7468 6d3d  y(mg, algorithm=
-00010400: 2777 6974 685f 636f 6e64 6f72 6365 745f  'with_condorcet_
-00010410: 6368 6563 6b27 290a 0a20 2020 2022 2222  check')..    """
-00010420: 0a0a 2020 2020 6966 2061 6c67 6f72 6974  ..    if algorit
-00010430: 686d 203d 3d20 2762 6173 6963 273a 200a  hm == 'basic': .
-00010440: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00010450: 7374 6162 6c65 5f76 6f74 696e 675f 6261  stable_voting_ba
-00010460: 7369 6328 6564 6174 612c 2063 7572 725f  sic(edata, curr_
-00010470: 6361 6e64 7320 3d20 6375 7272 5f63 616e  cands = curr_can
-00010480: 6473 2c20 7374 7265 6e67 7468 5f66 756e  ds, strength_fun
-00010490: 6374 696f 6e20 3d20 7374 7265 6e67 7468  ction = strength
-000104a0: 5f66 756e 6374 696f 6e29 0a20 2020 2065  _function).    e
-000104b0: 6c69 6620 616c 676f 7269 7468 6d20 3d3d  lif algorithm ==
-000104c0: 2027 7769 7468 5f63 6f6e 646f 7263 6574   'with_condorcet
-000104d0: 5f63 6865 636b 273a 0a20 2020 2020 2020  _check':.       
-000104e0: 2072 6574 7572 6e20 5f73 7461 626c 655f   return _stable_
-000104f0: 766f 7469 6e67 5f77 6974 685f 636f 6e64  voting_with_cond
-00010500: 6f72 6365 745f 6368 6563 6b28 6564 6174  orcet_check(edat
-00010510: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
-00010520: 6375 7272 5f63 616e 6473 2c20 7374 7265  curr_cands, stre
-00010530: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-00010540: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00010550: 6e29 0a20 2020 2065 6c73 653a 0a20 2020  n).    else:.   
-00010560: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00010570: 4572 726f 7228 2249 6e76 616c 6964 2061  Error("Invalid a
-00010580: 6c67 6f72 6974 686d 2073 7065 6369 6669  lgorithm specifi
-00010590: 6564 2e22 290a 2020 2020 0a0a 0a0a 4076  ed.").    ....@v
-000105a0: 6d28 6e61 6d65 3d22 4573 7365 6e74 6961  m(name="Essentia
-000105b0: 6c20 5365 7422 290a 6465 6620 6573 7365  l Set").def esse
-000105c0: 6e74 6961 6c28 6564 6174 612c 2063 7572  ntial(edata, cur
-000105d0: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
-000105e0: 7468 7265 7368 6f6c 6420 3d20 302e 3030  threshold = 0.00
-000105f0: 3030 3030 3129 3a20 0a20 2020 2022 2222  00001): .    """
-00010600: 5468 6520 4573 7365 6e74 6961 6c20 5365  The Essential Se
-00010610: 7420 6973 2074 6865 2073 7570 706f 7274  t is the support
-00010620: 206f 6620 7468 6520 2863 686f 7365 6e29   of the (chosen)
-00010630: 2043 3220 6d61 7869 6d61 6c20 6c6f 7474   C2 maximal lott
-00010640: 6572 792e 0a0a 2020 2020 4172 6773 3a0a  ery...    Args:.
-00010650: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
-00010660: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
-00010670: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
-00010680: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
-00010690: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
-000106a0: 7320 6120 606d 6172 6769 6e5f 6d61 7472  s a `margin_matr
-000106b0: 6978 6020 6174 7472 6962 7574 652e 0a20  ix` attribute.. 
-000106c0: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
-000106d0: 7320 284c 6973 745b 696e 745d 2c20 6f70  s (List[int], op
-000106e0: 7469 6f6e 616c 293a 2049 6620 7365 742c  tional): If set,
-000106f0: 2074 6865 6e20 6669 6e64 2074 6865 2077   then find the w
-00010700: 696e 6e65 7273 2066 6f72 2074 6865 2070  inners for the p
-00010710: 726f 6669 6c65 2072 6573 7472 6963 7465  rofile restricte
-00010720: 6420 746f 2074 6865 2063 616e 6469 6461  d to the candida
-00010730: 7465 7320 696e 2060 6063 7572 725f 6361  tes in ``curr_ca
-00010740: 6e64 7360 600a 0a20 2020 2052 6574 7572  nds``..    Retur
-00010750: 6e73 3a0a 2020 2020 2020 2020 4120 736f  ns:.        A so
-00010760: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
-00010770: 6469 6461 7465 732e 0a0a 2020 2020 2222  didates...    ""
-00010780: 220a 2020 2020 6d6c 203d 206d 6178 696d  ".    ml = maxim
-00010790: 616c 5f6c 6f74 7465 7279 2865 6461 7461  al_lottery(edata
-000107a0: 2c20 6375 7272 5f63 616e 6473 3d63 7572  , curr_cands=cur
-000107b0: 725f 6361 6e64 7329 0a0a 2020 2020 7265  r_cands)..    re
-000107c0: 7475 726e 2073 6f72 7465 6428 5b63 2066  turn sorted([c f
-000107d0: 6f72 2063 2069 6e20 6d6c 2e6b 6579 7328  or c in ml.keys(
-000107e0: 2920 6966 206d 6c5b 635d 203e 2074 6872  ) if ml[c] > thr
-000107f0: 6573 686f 6c64 5d29 0a0a 4076 6d28 6e61  eshold])..@vm(na
-00010800: 6d65 3d22 5765 6967 6874 6564 2043 6f76  me="Weighted Cov
-00010810: 6572 696e 6722 290a 6465 6620 7765 6967  ering").def weig
-00010820: 6874 6564 5f63 6f76 6572 696e 6728 6564  hted_covering(ed
-00010830: 6174 612c 2063 7572 725f 6361 6e64 733d  ata, curr_cands=
-00010840: 4e6f 6e65 293a 200a 2020 2020 2222 2241  None): .    """A
-00010850: 6363 6f72 6469 6e67 2074 6f20 5765 6967  ccording to Weig
-00010860: 6874 6564 2043 6f76 6572 696e 672c 2078  hted Covering, x
-00010870: 2064 6566 6561 7473 2079 2069 6620 7468   defeats y if th
-00010880: 6520 6d61 7267 696e 206f 6620 7820 6f76  e margin of x ov
-00010890: 6572 2079 2069 7320 706f 7369 7469 7665  er y is positive
-000108a0: 2061 6e64 2066 6f72 2065 7665 7279 206f   and for every o
-000108b0: 7468 6572 207a 2c20 7468 6520 6d61 7267  ther z, the marg
-000108c0: 696e 206f 6620 7820 6f76 6572 207a 2069  in of x over z i
-000108d0: 7320 6772 6561 7465 7220 7468 616e 206f  s greater than o
-000108e0: 7220 6571 7561 6c20 746f 2074 6865 206d  r equal to the m
-000108f0: 6172 6769 6e20 6f66 2079 206f 7665 7220  argin of y over 
-00010900: 7a2e 200a 0a20 2020 2041 7267 733a 0a20  z. ..    Args:. 
-00010910: 2020 2020 2020 2065 6461 7461 2028 5072         edata (Pr
-00010920: 6f66 696c 652c 2050 726f 6669 6c65 5769  ofile, ProfileWi
-00010930: 7468 5469 6573 2c20 4d61 7267 696e 4772  thTies, MarginGr
-00010940: 6170 6829 3a20 416e 7920 656c 6563 7469  aph): Any electi
-00010950: 6f6e 2064 6174 6120 7468 6174 2068 6173  on data that has
-00010960: 2061 2060 6d61 7267 696e 6020 6d65 7468   a `margin` meth
-00010970: 6f64 2e0a 2020 2020 2020 2020 6375 7272  od..        curr
-00010980: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
-00010990: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
-000109a0: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
-000109b0: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
-000109c0: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
-000109d0: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
-000109e0: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
-000109f0: 7272 5f63 616e 6473 6060 0a0a 2020 2020  rr_cands``..    
-00010a00: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00010a10: 2041 2073 6f72 7465 6420 6c69 7374 206f   A sorted list o
-00010a20: 6620 6361 6e64 6964 6174 6573 2e0a 0a20  f candidates... 
-00010a30: 2020 202e 2e20 6e6f 7465 3a3a 0a20 2020     .. note::.   
-00010a40: 2020 2020 2053 6565 2c20 652e 672e 2c20       See, e.g., 
-00010a50: 4268 6173 6b61 7220 4475 7474 6120 616e  Bhaskar Dutta an
-00010a60: 6420 4a65 616e 2d46 7261 6e63 6f69 7320  d Jean-Francois 
-00010a70: 4c61 736c 6965 722c 2022 436f 6d70 6172  Laslier, "Compar
-00010a80: 6973 6f6e 2066 756e 6374 696f 6e73 2061  ison functions a
-00010a90: 6e64 2063 686f 6963 6520 636f 7272 6573  nd choice corres
-00010aa0: 706f 6e64 656e 6365 732c 2220 536f 6369  pondences," Soci
-00010ab0: 616c 2043 686f 6963 6520 616e 6420 5765  al Choice and We
-00010ac0: 6c66 6172 652c 2031 363a 3531 33e2 8093  lfare, 16:513...
-00010ad0: 3533 322c 2031 3939 392c 2064 6f69 3a31  532, 1999, doi:1
-00010ae0: 302e 3130 3037 2f73 3030 3335 3530 3035  0.1007/s00355005
-00010af0: 3031 3538 2c20 616e 6420 5261 75cc 816c  0158, and Rau..l
-00010b00: 2050 65cc 8172 657a 2d46 6572 6e61 cc81   Pe..rez-Ferna..
-00010b10: 6e64 657a 2061 6e64 2042 6572 6e61 7264  ndez and Bernard
-00010b20: 2044 6520 4261 6574 732c 2022 5468 6520   De Baets, "The 
-00010b30: 7375 7065 7263 6f76 6572 696e 6720 7265  supercovering re
-00010b40: 6c61 7469 6f6e 2c20 7468 6520 7061 6972  lation, the pair
-00010b50: 7769 7365 2077 696e 6e65 722c 2061 6e64  wise winner, and
-00010b60: 206d 6f72 6520 6d69 7373 696e 6720 6c69   more missing li
-00010b70: 6e6b 7320 6265 7477 6565 6e20 426f 7264  nks between Bord
-00010b80: 6120 616e 6420 436f 6e64 6f72 6365 742c  a and Condorcet,
-00010b90: 2220 536f 6369 616c 2043 686f 6963 6520  " Social Choice 
-00010ba0: 616e 6420 5765 6c66 6172 652c 2035 303a  and Welfare, 50:
-00010bb0: 3332 39e2 8093 3335 322c 2032 3031 382c  329...352, 2018,
-00010bc0: 2064 6f69 3a31 302e 3130 3037 2f73 3030   doi:10.1007/s00
-00010bd0: 3335 352d 3031 372d 3130 3836 2d30 2e0a  355-017-1086-0..
-00010be0: 2020 2020 2222 220a 0a20 2020 2063 616e      """..    can
-00010bf0: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
-00010c00: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
-00010c10: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
-00010c20: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
-00010c30: 0a0a 2020 2020 646f 6d20 3d20 7b63 3a20  ..    dom = {c: 
-00010c40: 7365 7428 6564 6174 612e 646f 6d69 6e61  set(edata.domina
-00010c50: 746f 7273 2863 2c20 6375 7272 5f63 616e  tors(c, curr_can
-00010c60: 6473 203d 2063 7572 725f 6361 6e64 7329  ds = curr_cands)
-00010c70: 2920 666f 7220 6320 696e 2063 616e 6469  ) for c in candi
-00010c80: 6461 7465 737d 0a20 2020 2075 635f 7365  dates}.    uc_se
-00010c90: 7420 3d20 6c69 7374 2829 0a0a 2020 2020  t = list()..    
-00010ca0: 666f 7220 7920 696e 2063 616e 6469 6461  for y in candida
-00010cb0: 7465 733a 0a20 2020 2020 2020 2069 735f  tes:.        is_
-00010cc0: 696e 5f75 6373 203d 2054 7275 650a 2020  in_ucs = True.  
-00010cd0: 2020 2020 2020 666f 7220 7820 696e 2065        for x in e
-00010ce0: 6461 7461 2e64 6f6d 696e 6174 6f72 7328  data.dominators(
-00010cf0: 792c 2063 7572 725f 6361 6e64 7320 3d20  y, curr_cands = 
-00010d00: 6375 7272 5f63 616e 6473 293a 0a20 2020  curr_cands):.   
-00010d10: 2020 2020 2020 2020 2023 2063 6865 636b           # check
-00010d20: 2069 6620 7920 636f 7665 7273 2078 2c20   if y covers x, 
-00010d30: 692e 652e 2c20 666f 7220 6576 6572 7920  i.e., for every 
-00010d40: 7a2c 206d 6172 6769 6e28 782c 207a 2920  z, margin(x, z) 
-00010d50: 3e3d 206d 6172 6769 6e28 792c 207a 290a  >= margin(y, z).
-00010d60: 2020 2020 2020 2020 2020 2020 636f 7665              cove
-00010d70: 7273 203d 2054 7275 650a 2020 2020 2020  rs = True.      
-00010d80: 2020 2020 2020 666f 7220 7a20 696e 2063        for z in c
-00010d90: 616e 6469 6461 7465 733a 0a20 2020 2020  andidates:.     
-00010da0: 2020 2020 2020 2020 2020 2069 6620 6564             if ed
-00010db0: 6174 612e 6d61 7267 696e 2878 2c20 7a29  ata.margin(x, z)
-00010dc0: 203c 2065 6461 7461 2e6d 6172 6769 6e28   < edata.margin(
-00010dd0: 792c 207a 293a 0a20 2020 2020 2020 2020  y, z):.         
-00010de0: 2020 2020 2020 2020 2020 2063 6f76 6572             cover
-00010df0: 7320 3d20 4661 6c73 650a 2020 2020 2020  s = False.      
-00010e00: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00010e10: 6561 6b0a 2020 2020 2020 2020 2020 0a20  eak.          . 
-00010e20: 2020 2020 2020 2020 2020 2069 6620 636f             if co
-00010e30: 7665 7273 3a0a 2020 2020 2020 2020 2020  vers:.          
-00010e40: 2020 2020 2020 6973 5f69 6e5f 7563 7320        is_in_ucs 
-00010e50: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00010e60: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
-00010e70: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-00010e80: 2020 2020 2020 2069 6620 6973 5f69 6e5f         if is_in_
-00010e90: 7563 733a 0a20 2020 2020 2020 2020 2020  ucs:.           
-00010ea0: 2075 635f 7365 742e 6170 7065 6e64 2879   uc_set.append(y
-00010eb0: 290a 0a20 2020 2072 6574 7572 6e20 736f  )..    return so
-00010ec0: 7274 6564 2875 635f 7365 7429 0a0a 4076  rted(uc_set)..@v
-00010ed0: 6d28 6e61 6d65 203d 2022 4c6f 7373 2d54  m(name = "Loss-T
-00010ee0: 7269 6d6d 6572 2056 6f74 696e 6722 290a  rimmer Voting").
-00010ef0: 6465 6620 6c6f 7373 5f74 7269 6d6d 6572  def loss_trimmer
-00010f00: 2865 6461 7461 2c20 6375 7272 5f63 616e  (edata, curr_can
-00010f10: 6473 203d 204e 6f6e 6529 3a0a 2020 2020  ds = None):.    
-00010f20: 2222 2249 7465 7261 7469 7665 6c79 2065  """Iteratively e
-00010f30: 6c69 6d69 6e61 7465 2074 6865 2063 616e  liminate the can
-00010f40: 6469 6461 7465 2077 6974 6820 7468 6520  didate with the 
-00010f50: 6c61 7267 6573 7420 7375 6d20 6f66 206d  largest sum of m
-00010f60: 6172 6769 6e73 206f 6620 6c6f 7373 2075  argins of loss u
-00010f70: 6e74 696c 2061 2043 6f6e 646f 7263 6574  ntil a Condorcet
-00010f80: 2077 696e 6e65 7220 6973 2066 6f75 6e64   winner is found
-00010f90: 2e20 496e 2074 6869 7320 7665 7273 696f  . In this versio
-00010fa0: 6e20 6f66 2074 6865 206d 6574 686f 642c  n of the method,
-00010fb0: 2070 6172 616c 6c65 6c2d 756e 6976 6572   parallel-univer
-00010fc0: 7365 2074 6965 6272 6561 6b69 6e67 2069  se tiebreaking i
-00010fd0: 7320 7573 6564 2069 6620 7468 6572 6520  s used if there 
-00010fe0: 6172 6520 6d75 6c74 6970 6c65 2063 616e  are multiple can
-00010ff0: 6469 6461 7465 7320 7769 7468 2074 6865  didates with the
-00011000: 206c 6172 6765 7374 2073 756d 206f 6620   largest sum of 
-00011010: 6d61 7267 696e 7320 6f66 206c 6f73 732e  margins of loss.
-00011020: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00011030: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
-00011040: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
-00011050: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
-00011060: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
-00011070: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
-00011080: 6d61 7267 696e 206d 6574 686f 642e 0a20  margin method.. 
-00011090: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
-000110a0: 7320 284c 6973 745b 696e 745d 2c20 6f70  s (List[int], op
-000110b0: 7469 6f6e 616c 293a 2049 6620 7365 742c  tional): If set,
-000110c0: 2074 6865 6e20 6669 6e64 2074 6865 2077   then find the w
-000110d0: 696e 6e65 7273 2066 6f72 2074 6865 2070  inners for the p
-000110e0: 726f 6669 6c65 2072 6573 7472 6963 7465  rofile restricte
-000110f0: 6420 746f 2074 6865 2063 616e 6469 6461  d to the candida
-00011100: 7465 7320 696e 2060 6063 7572 725f 6361  tes in ``curr_ca
-00011110: 6e64 7360 600a 0a20 2020 2052 6574 7572  nds``..    Retur
-00011120: 6e73 3a20 0a20 2020 2020 2020 2041 2073  ns: .        A s
-00011130: 6f72 7465 6420 6c69 7374 206f 6620 6361  orted list of ca
-00011140: 6e64 6964 6174 6573 0a0a 2020 2020 2e2e  ndidates..    ..
-00011150: 206e 6f74 653a 3a0a 2020 2020 2020 2020   note::.        
-00011160: 4d65 7468 6f64 2070 726f 706f 7365 6420  Method proposed 
-00011170: 6279 2052 6963 6861 7264 2042 2e20 4461  by Richard B. Da
-00011180: 726c 696e 6774 6f6e 2069 6e20 2254 6865  rlington in "The
-00011190: 2043 6173 6520 666f 7220 7468 6520 4c6f   Case for the Lo
-000111a0: 7373 2d54 7269 6d6d 6572 2056 6f74 696e  ss-Trimmer Votin
-000111b0: 6720 5379 7374 656d 2e22 0a0a 2020 2020  g System."..    
-000111c0: 2222 220a 0a20 2020 2063 7572 725f 6361  """..    curr_ca
-000111d0: 6e64 7320 3d20 6564 6174 612e 6361 6e64  nds = edata.cand
-000111e0: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
-000111f0: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
-00011200: 6520 6375 7272 5f63 616e 6473 0a0a 2020  e curr_cands..  
-00011210: 2020 7765 616b 5f63 7720 3d20 6564 6174    weak_cw = edat
-00011220: 612e 7765 616b 5f63 6f6e 646f 7263 6574  a.weak_condorcet
-00011230: 5f77 696e 6e65 7228 6375 7272 5f63 616e  _winner(curr_can
-00011240: 6473 203d 2063 7572 725f 6361 6e64 7329  ds = curr_cands)
-00011250: 0a20 2020 2023 2049 6620 7468 6572 6520  .    # If there 
-00011260: 6172 6520 7765 616b 2043 6f6e 646f 7263  are weak Condorc
-00011270: 6574 2077 696e 6e65 7273 2c20 7265 7475  et winners, retu
-00011280: 726e 2074 686f 7365 2063 616e 6469 6461  rn those candida
-00011290: 7465 730a 2020 2020 6966 2065 6461 7461  tes.    if edata
-000112a0: 2e77 6561 6b5f 636f 6e64 6f72 6365 745f  .weak_condorcet_
-000112b0: 7769 6e6e 6572 2863 7572 725f 6361 6e64  winner(curr_cand
-000112c0: 7320 3d20 6375 7272 5f63 616e 6473 2920  s = curr_cands) 
-000112d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000112e0: 2020 2020 2072 6574 7572 6e20 736f 7274       return sort
-000112f0: 6564 2877 6561 6b5f 6377 290a 2020 2020  ed(weak_cw).    
-00011300: 0a20 2020 2023 204f 7468 6572 7769 7365  .    # Otherwise
-00011310: 2c20 6361 6c63 756c 6174 6520 7468 6520  , calculate the 
-00011320: 7375 6d20 6f66 206d 6172 6769 6e73 206f  sum of margins o
-00011330: 6620 6c6f 7373 2066 6f72 2065 6163 6820  f loss for each 
-00011340: 6361 6e64 6964 6174 650a 2020 2020 7375  candidate.    su
-00011350: 6d5f 6f66 5f6d 6172 6769 6e73 5f6f 665f  m_of_margins_of_
-00011360: 6c6f 7373 203d 207b 6361 6e64 3a20 7375  loss = {cand: su
-00011370: 6d28 5b65 6461 7461 2e6d 6172 6769 6e28  m([edata.margin(
-00011380: 6f74 6865 725f 6361 6e64 2c20 6361 6e64  other_cand, cand
-00011390: 2920 666f 7220 6f74 6865 725f 6361 6e64  ) for other_cand
-000113a0: 2069 6e20 6375 7272 5f63 616e 6473 2069   in curr_cands i
-000113b0: 6620 6564 6174 612e 6d61 7267 696e 286f  f edata.margin(o
-000113c0: 7468 6572 5f63 616e 642c 2063 616e 6429  ther_cand, cand)
-000113d0: 203e 2030 5d29 2066 6f72 2063 616e 6420   > 0]) for cand 
-000113e0: 696e 2063 7572 725f 6361 6e64 737d 0a0a  in curr_cands}..
-000113f0: 2020 2020 2320 4669 6e64 2074 6865 2063      # Find the c
-00011400: 616e 6469 6461 7465 7320 7769 7468 2074  andidates with t
-00011410: 6865 206c 6172 6765 7374 2073 756d 206f  he largest sum o
-00011420: 6620 6d61 7267 696e 7320 6f66 206c 6f73  f margins of los
-00011430: 730a 2020 2020 6d61 785f 7375 6d5f 6f66  s.    max_sum_of
-00011440: 5f6d 6172 6769 6e73 5f6f 665f 6c6f 7373  _margins_of_loss
-00011450: 203d 206d 6178 2873 756d 5f6f 665f 6d61   = max(sum_of_ma
-00011460: 7267 696e 735f 6f66 5f6c 6f73 732e 7661  rgins_of_loss.va
-00011470: 6c75 6573 2829 290a 2020 2020 6269 6767  lues()).    bigg
-00011480: 6573 745f 6c6f 7365 7273 203d 205b 6361  est_losers = [ca
-00011490: 6e64 2066 6f72 2063 616e 6420 696e 2063  nd for cand in c
-000114a0: 7572 725f 6361 6e64 7320 6966 2073 756d  urr_cands if sum
-000114b0: 5f6f 665f 6d61 7267 696e 735f 6f66 5f6c  _of_margins_of_l
-000114c0: 6f73 735b 6361 6e64 5d20 3d3d 206d 6178  oss[cand] == max
-000114d0: 5f73 756d 5f6f 665f 6d61 7267 696e 735f  _sum_of_margins_
-000114e0: 6f66 5f6c 6f73 735d 0a0a 2020 2020 7769  of_loss]..    wi
-000114f0: 6e6e 6572 7320 3d20 5b5d 0a0a 2020 2020  nners = []..    
-00011500: 2320 466f 7220 6561 6368 2062 6967 6765  # For each bigge
-00011510: 7374 206c 6f73 6572 2c20 6361 6c63 756c  st loser, calcul
-00011520: 6174 6520 7468 6520 7769 6e6e 6572 7320  ate the winners 
-00011530: 6166 7465 7220 7265 6d6f 7669 6e67 2074  after removing t
-00011540: 6861 7420 6361 6e64 6964 6174 652e 2054  hat candidate. T
-00011550: 6865 2075 6e69 6f6e 206f 6620 7468 6573  he union of thes
-00011560: 6520 7365 7473 2069 7320 7468 6520 7365  e sets is the se
-00011570: 7420 6f66 2077 696e 6e65 7273 2e0a 2020  t of winners..  
-00011580: 2020 666f 7220 626c 2069 6e20 6269 6767    for bl in bigg
-00011590: 6573 745f 6c6f 7365 7273 3a0a 2020 2020  est_losers:.    
-000115a0: 2020 2020 7769 6e6e 6572 735f 7769 7468      winners_with
-000115b0: 6f75 745f 626c 203d 206c 6f73 735f 7472  out_bl = loss_tr
-000115c0: 696d 6d65 7228 6564 6174 612c 2063 7572  immer(edata, cur
-000115d0: 725f 6361 6e64 7320 3d20 5b63 616e 6420  r_cands = [cand 
-000115e0: 666f 7220 6361 6e64 2069 6e20 6375 7272  for cand in curr
-000115f0: 5f63 616e 6473 2069 6620 6361 6e64 2021  _cands if cand !
-00011600: 3d20 626c 5d29 0a20 2020 2020 2020 2077  = bl]).        w
-00011610: 696e 6e65 7273 202b 3d20 7769 6e6e 6572  inners += winner
-00011620: 735f 7769 7468 6f75 745f 626c 0a0a 2020  s_without_bl..  
-00011630: 2020 7265 7475 726e 2073 6f72 7465 6428    return sorted(
-00011640: 6c69 7374 2873 6574 2877 696e 6e65 7273  list(set(winners
-00011650: 2929 290a 0a0a 6465 6620 6469 7374 616e  )))...def distan
-00011660: 6365 5f74 6f5f 6d61 7267 696e 5f67 7261  ce_to_margin_gra
-00011670: 7068 2865 6461 7461 2c20 7265 6c2c 2065  ph(edata, rel, e
-00011680: 7870 203d 2031 2c20 6375 7272 5f63 616e  xp = 1, curr_can
-00011690: 6473 203d 204e 6f6e 6529 3a20 0a20 2020  ds = None): .   
-000116a0: 2022 2222 0a20 2020 2043 616c 6375 6c61   """.    Calcula
-000116b0: 7465 2074 6865 2064 6973 7461 6e63 6520  te the distance 
-000116c0: 6f66 2060 6072 656c 6060 2028 6120 7265  of ``rel`` (a re
-000116d0: 6c61 7469 6f6e 2920 746f 2074 6865 206d  lation) to the m
-000116e0: 616a 6f72 6974 7920 6772 6170 6820 6f66  ajority graph of
-000116f0: 2060 6065 6461 7461 6060 2e20 0a20 2020   ``edata``. .   
-00011700: 2022 2222 0a20 2020 2063 616e 6469 6461   """.    candida
-00011710: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
-00011720: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
-00011730: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
-00011740: 6520 6375 7272 5f63 616e 6473 0a20 2020  e curr_cands.   
-00011750: 200a 2020 2020 6966 2074 7970 6528 6564   .    if type(ed
-00011760: 6174 6129 203d 3d20 4d61 6a6f 7269 7479  ata) == Majority
-00011770: 4772 6170 6820 616e 6420 6578 7020 3d3d  Graph and exp ==
-00011780: 2030 3a0a 2020 2020 2020 2020 2320 6966   0:.        # if
-00011790: 2065 6461 7461 2069 7320 6120 4d61 6a6f   edata is a Majo
-000117a0: 7269 7479 4772 6170 682c 2077 6520 6e65  rityGraph, we ne
-000117b0: 6564 2074 6f20 6164 6420 6d61 7267 696e  ed to add margin
-000117c0: 7320 666f 7220 7468 6520 666f 6c6c 6f77  s for the follow
-000117d0: 696e 6720 636f 6465 2074 6f20 776f 726b  ing code to work
-000117e0: 2e20 2054 6865 206d 6172 6769 6e73 2064  .  The margins d
-000117f0: 6f20 6e6f 7420 6d61 7474 6572 2077 6865  o not matter whe
-00011800: 6e20 6578 703d 3d30 2e20 2020 0a20 2020  n exp==0.   .   
-00011810: 2020 2020 2065 6461 7461 203d 204d 6172       edata = Mar
-00011820: 6769 6e47 7261 7068 2863 616e 6469 6461  ginGraph(candida
-00011830: 7465 732c 205b 2863 312c 2063 322c 2031  tes, [(c1, c2, 1
-00011840: 2920 666f 7220 6331 2c20 6332 2069 6e20  ) for c1, c2 in 
-00011850: 6564 6174 612e 6564 6765 7320 6966 2028  edata.edges if (
-00011860: 6331 2069 6e20 6361 6e64 6964 6174 6573  c1 in candidates
-00011870: 2061 6e64 2063 3220 696e 2063 616e 6469   and c2 in candi
-00011880: 6461 7465 7329 5d29 0a20 2020 2070 656e  dates)]).    pen
-00011890: 616c 7479 203d 2030 0a20 2020 2066 6f72  alty = 0.    for
-000118a0: 2061 2c62 2069 6e20 636f 6d62 696e 6174   a,b in combinat
-000118b0: 696f 6e73 2863 616e 6469 6461 7465 732c  ions(candidates,
-000118c0: 2032 293a 200a 2020 2020 2020 2020 6966   2): .        if
-000118d0: 2065 6461 7461 2e6d 616a 6f72 6974 795f   edata.majority_
-000118e0: 7072 6566 6572 7328 612c 2062 2920 616e  prefers(a, b) an
-000118f0: 6420 2862 2c61 2920 696e 2072 656c 3a20  d (b,a) in rel: 
-00011900: 0a20 2020 2020 2020 2020 2020 2070 656e  .            pen
-00011910: 616c 7479 202b 3d20 2865 6461 7461 2e6d  alty += (edata.m
-00011920: 6172 6769 6e28 612c 2062 2920 2a2a 2065  argin(a, b) ** e
-00011930: 7870 290a 2020 2020 2020 2020 656c 6966  xp).        elif
-00011940: 2065 6461 7461 2e6d 616a 6f72 6974 795f   edata.majority_
-00011950: 7072 6566 6572 7328 622c 2061 2920 616e  prefers(b, a) an
-00011960: 6420 2861 2c62 2920 696e 2072 656c 3a20  d (a,b) in rel: 
-00011970: 0a20 2020 2020 2020 2020 2020 2070 656e  .            pen
-00011980: 616c 7479 202b 3d20 2865 6461 7461 2e6d  alty += (edata.m
-00011990: 6172 6769 6e28 622c 2061 2920 2a2a 2065  argin(b, a) ** e
-000119a0: 7870 290a 2020 2020 2020 2020 656c 6966  xp).        elif
-000119b0: 2065 6461 7461 2e6d 616a 6f72 6974 795f   edata.majority_
-000119c0: 7072 6566 6572 7328 612c 2062 2920 616e  prefers(a, b) an
-000119d0: 6420 2861 2c62 2920 6e6f 7420 696e 2072  d (a,b) not in r
-000119e0: 656c 2061 6e64 2028 622c 6129 206e 6f74  el and (b,a) not
-000119f0: 2069 6e20 7265 6c3a 200a 2020 2020 2020   in rel: .      
-00011a00: 2020 2020 2020 7065 6e61 6c74 7920 2b3d        penalty +=
-00011a10: 2028 6564 6174 612e 6d61 7267 696e 2861   (edata.margin(a
-00011a20: 2c20 6229 202a 2a20 6578 7029 202f 2032  , b) ** exp) / 2
-00011a30: 200a 2020 2020 2020 2020 656c 6966 2065   .        elif e
-00011a40: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
-00011a50: 6566 6572 7328 622c 2061 2920 616e 6420  efers(b, a) and 
-00011a60: 2861 2c62 2920 6e6f 7420 696e 2072 656c  (a,b) not in rel
-00011a70: 2061 6e64 2028 622c 6129 206e 6f74 2069   and (b,a) not i
-00011a80: 6e20 7265 6c3a 200a 2020 2020 2020 2020  n rel: .        
-00011a90: 2020 2020 7065 6e61 6c74 7920 2b3d 2028      penalty += (
-00011aa0: 6564 6174 612e 6d61 7267 696e 2862 2c20  edata.margin(b, 
-00011ab0: 6129 202a 2a20 6578 7029 2020 2f20 320a  a) ** exp)  / 2.
-00011ac0: 2020 2020 7265 7475 726e 2070 656e 616c      return penal
-00011ad0: 7479 0a0a 0a6d 675f 766d 7320 3d20 5b0a  ty...mg_vms = [.
-00011ae0: 2020 2020 6d69 6e69 6d61 782c 200a 2020      minimax, .  
-00011af0: 2020 7370 6c69 745f 6379 636c 652c 0a20    split_cycle,. 
-00011b00: 2020 2023 6265 6174 5f70 6174 682c 0a20     #beat_path,. 
-00011b10: 2020 2023 7261 6e6b 6564 5f70 6169 7273     #ranked_pairs
-00011b20: 2c0a 2020 2020 2372 616e 6b65 645f 7061  ,.    #ranked_pa
-00011b30: 6972 735f 7769 7468 5f74 6573 742c 0a20  irs_with_test,. 
-00011b40: 2020 2072 616e 6b65 645f 7061 6972 735f     ranked_pairs_
-00011b50: 7a74 2c0a 2020 2020 7261 6e6b 6564 5f70  zt,.    ranked_p
-00011b60: 6169 7273 5f74 622c 0a20 2020 2023 7269  airs_tb,.    #ri
-00011b70: 7665 722c 0a20 2020 2023 7269 7665 725f  ver,.    #river_
-00011b80: 7769 7468 5f74 6573 742c 200a 2020 2020  with_test, .    
-00011b90: 7369 6d70 6c65 5f73 7461 626c 655f 766f  simple_stable_vo
-00011ba0: 7469 6e67 2c0a 2020 2020 2373 696d 706c  ting,.    #simpl
-00011bb0: 655f 7374 6162 6c65 5f76 6f74 696e 675f  e_stable_voting_
-00011bc0: 6661 7374 6572 2c0a 2020 2020 7374 6162  faster,.    stab
-00011bd0: 6c65 5f76 6f74 696e 672c 0a20 2020 2023  le_voting,.    #
-00011be0: 7374 6162 6c65 5f76 6f74 696e 675f 6661  stable_voting_fa
-00011bf0: 7374 6572 2c0a 2020 2020 6573 7365 6e74  ster,.    essent
-00011c00: 6961 6c2c 0a20 2020 2077 6569 6768 7465  ial,.    weighte
-00011c10: 645f 636f 7665 7269 6e67 2c0a 2020 2020  d_covering,.    
-00011c20: 6c6f 7373 5f74 7269 6d6d 6572 0a5d 0a0a  loss_trimmer.]..
-00011c30: 0a6d 675f 766d 735f 616c 6c20 3d20 5b0a  .mg_vms_all = [.
-00011c40: 2020 2020 6d69 6e69 6d61 782c 200a 2020      minimax, .  
-00011c50: 2020 7370 6c69 745f 6379 636c 652c 0a20    split_cycle,. 
-00011c60: 2020 2062 6561 745f 7061 7468 2c0a 2020     beat_path,.  
-00011c70: 2020 7261 6e6b 6564 5f70 6169 7273 2c0a    ranked_pairs,.
-00011c80: 2020 2020 7261 6e6b 6564 5f70 6169 7273      ranked_pairs
-00011c90: 5f77 6974 685f 7465 7374 2c0a 2020 2020  _with_test,.    
-00011ca0: 7261 6e6b 6564 5f70 6169 7273 5f7a 742c  ranked_pairs_zt,
-00011cb0: 0a20 2020 2072 616e 6b65 645f 7061 6972  .    ranked_pair
-00011cc0: 735f 7462 2c0a 2020 2020 7269 7665 722c  s_tb,.    river,
-00011cd0: 0a20 2020 2072 6976 6572 5f77 6974 685f  .    river_with_
-00011ce0: 7465 7374 2c20 0a20 2020 2073 696d 706c  test, .    simpl
-00011cf0: 655f 7374 6162 6c65 5f76 6f74 696e 672c  e_stable_voting,
-00011d00: 0a20 2020 2073 7461 626c 655f 766f 7469  .    stable_voti
-00011d10: 6e67 2c0a 2020 2020 6573 7365 6e74 6961  ng,.    essentia
-00011d20: 6c2c 0a20 2020 2077 6569 6768 7465 645f  l,.    weighted_
-00011d30: 636f 7665 7269 6e67 2c0a 2020 2020 6c6f  covering,.    lo
-00011d40: 7373 5f74 7269 6d6d 6572 0a5d            ss_trimmer.]
+000066c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000066d0: 2020 3a6d 6574 683a 6070 7265 665f 766f    :meth:`pref_vo
+000066e0: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+000066f0: 645f 6d65 7468 6f64 732e 6973 5f73 7461  d_methods.is_sta
+00006700: 636b 600a 0a0a 2020 2020 2222 2220 2020  ck`...    """   
+00006710: 200a 0a20 2020 2063 616e 6469 6461 7465   ..    candidate
+00006720: 7320 3d20 6375 7272 5f63 616e 6473 2069  s = curr_cands i
+00006730: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
+00006740: 6e6f 7420 4e6f 6e65 2065 6c73 6520 6564  not None else ed
+00006750: 6174 612e 6361 6e64 6964 6174 6573 0a20  ata.candidates. 
+00006760: 2020 2077 696e 6e65 7273 203d 206c 6973     winners = lis
+00006770: 7428 290a 2020 2020 666f 7220 636c 6973  t().    for clis
+00006780: 7420 696e 2070 6572 6d75 7461 7469 6f6e  t in permutation
+00006790: 7328 6361 6e64 6964 6174 6573 293a 200a  s(candidates): .
+000067a0: 2020 2020 2020 2020 6973 7374 6163 6b20          isstack 
+000067b0: 3d20 6973 5f73 7461 636b 2865 6461 7461  = is_stack(edata
+000067c0: 2c20 636c 6973 742c 2063 7572 725f 6361  , clist, curr_ca
+000067d0: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
+000067e0: 290a 2020 2020 2020 2020 6966 2069 7373  ).        if iss
+000067f0: 7461 636b 3a20 0a20 2020 2020 2020 2020  tack: .         
+00006800: 2020 2077 696e 6e65 7273 2e61 7070 656e     winners.appen
+00006810: 6428 636c 6973 745b 305d 290a 2020 2020  d(clist[0]).    
+00006820: 2020 2020 2020 2020 0a20 2020 2072 6574          .    ret
+00006830: 7572 6e20 736f 7274 6564 286c 6973 7428  urn sorted(list(
+00006840: 7365 7428 7769 6e6e 6572 7329 2929 0a0a  set(winners)))..
+00006850: 6465 6620 5f72 616e 6b65 645f 7061 6972  def _ranked_pair
+00006860: 735f 6261 7369 6328 0a20 2020 2065 6461  s_basic(.    eda
+00006870: 7461 2c20 0a20 2020 2063 7572 725f 6361  ta, .    curr_ca
+00006880: 6e64 7320 3d20 4e6f 6e65 2c20 0a20 2020  nds = None, .   
+00006890: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+000068a0: 6f6e 203d 204e 6f6e 6529 3a20 2020 0a20  on = None):   . 
+000068b0: 2020 2022 2222 416e 2069 6d70 6c65 6d65     """An impleme
+000068c0: 6e74 6174 696f 6e20 6f66 2052 616e 6b65  ntation of Ranke
+000068d0: 6420 5061 6972 7320 7468 6174 2075 7365  d Pairs that use
+000068e0: 7320 6120 6261 7369 6320 616c 676f 7269  s a basic algori
+000068f0: 7468 6d2e 200a 0a20 2020 2041 7267 733a  thm. ..    Args:
+00006900: 0a20 2020 2020 2020 2065 6461 7461 2028  .        edata (
+00006910: 5072 6f66 696c 652c 2050 726f 6669 6c65  Profile, Profile
+00006920: 5769 7468 5469 6573 2c20 4d61 7267 696e  WithTies, Margin
+00006930: 4772 6170 6829 3a20 416e 7920 656c 6563  Graph): Any elec
+00006940: 7469 6f6e 2064 6174 6120 7468 6174 2068  tion data that h
+00006950: 6173 2061 2060 6d61 7267 696e 6020 6d65  as a `margin` me
+00006960: 7468 6f64 2e20 0a20 2020 2020 2020 2063  thod. .        c
+00006970: 7572 725f 6361 6e64 7320 284c 6973 745b  urr_cands (List[
+00006980: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
+00006990: 2049 6620 7365 742c 2074 6865 6e20 6669   If set, then fi
+000069a0: 6e64 2074 6865 2077 696e 6e65 7273 2066  nd the winners f
+000069b0: 6f72 2074 6865 2070 726f 6669 6c65 2072  or the profile r
+000069c0: 6573 7472 6963 7465 6420 746f 2074 6865  estricted to the
+000069d0: 2063 616e 6469 6461 7465 7320 696e 2060   candidates in `
+000069e0: 6063 7572 725f 6361 6e64 7360 600a 0a20  `curr_cands``.. 
+000069f0: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+00006a00: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
+00006a10: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
+00006a20: 2e20 0a0a 2020 2020 2222 220a 2020 2020  . ..    """.    
+00006a30: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
+00006a40: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
+00006a50: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
+00006a60: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
+00006a70: 6e64 7320 0a20 2020 2063 6964 785f 746f  nds .    cidx_to
+00006a80: 5f63 616e 6420 3d20 7b63 6964 783a 2063  _cand = {cidx: c
+00006a90: 2066 6f72 2063 6964 782c 2063 2069 6e20   for cidx, c in 
+00006aa0: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
+00006ab0: 6174 6573 297d 2020 0a20 2020 2063 616e  ates)}  .    can
+00006ac0: 645f 746f 5f63 6964 7820 3d20 7b63 3a20  d_to_cidx = {c: 
+00006ad0: 6369 6478 2066 6f72 2063 6964 782c 2063  cidx for cidx, c
+00006ae0: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
+00006af0: 6e64 6964 6174 6573 297d 2020 0a20 2020  ndidates)}  .   
+00006b00: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00006b10: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
+00006b20: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
+00006b30: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
+00006b40: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
+00006b50: 6374 696f 6e20 2020 200a 0a20 2020 2063  ction    ..    c
+00006b60: 7720 3d20 6564 6174 612e 636f 6e64 6f72  w = edata.condor
+00006b70: 6365 745f 7769 6e6e 6572 2863 7572 725f  cet_winner(curr_
+00006b80: 6361 6e64 733d 6375 7272 5f63 616e 6473  cands=curr_cands
+00006b90: 290a 2020 2020 2320 5261 6e6b 6564 2050  ).    # Ranked P
+00006ba0: 6169 7273 2069 7320 436f 6e64 6f72 6365  airs is Condorce
+00006bb0: 7420 636f 6e73 6973 7465 6e74 2c20 736f  t consistent, so
+00006bc0: 2073 696d 706c 7920 7265 7475 726e 2074   simply return t
+00006bd0: 6865 2043 6f6e 646f 7263 6574 2077 696e  he Condorcet win
+00006be0: 6e65 7220 6966 2065 7869 7374 730a 2020  ner if exists.  
+00006bf0: 2020 6966 2063 7720 6973 206e 6f74 204e    if cw is not N
+00006c00: 6f6e 653a 200a 2020 2020 2020 2020 7769  one: .        wi
+00006c10: 6e6e 6572 7320 3d20 5b63 775d 0a20 2020  nners = [cw].   
+00006c20: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
+00006c30: 5f65 6467 6573 203d 205b 2863 312c 2063  _edges = [(c1, c
+00006c40: 322c 2073 7472 656e 6774 685f 6675 6e63  2, strength_func
+00006c50: 7469 6f6e 2863 312c 2063 3229 2920 666f  tion(c1, c2)) fo
+00006c60: 7220 6331 2069 6e20 6361 6e64 6964 6174  r c1 in candidat
+00006c70: 6573 2066 6f72 2063 3220 696e 2063 616e  es for c2 in can
+00006c80: 6469 6461 7465 7320 0a20 2020 2020 2020  didates .       
+00006c90: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00006ca0: 3120 213d 2063 3220 616e 6420 2865 6461  1 != c2 and (eda
+00006cb0: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+00006cc0: 6572 7328 6331 2c20 6332 2920 6f72 2065  ers(c1, c2) or e
+00006cd0: 6461 7461 2e69 735f 7469 6564 2863 312c  data.is_tied(c1,
+00006ce0: 2063 3229 295d 0a20 2020 2020 2020 2077   c2))].        w
+00006cf0: 696e 6e65 7273 203d 206c 6973 7428 2920  inners = list() 
+00006d00: 2020 0a20 2020 2020 2020 2069 6620 6c65    .        if le
+00006d10: 6e28 775f 6564 6765 7329 203e 2030 3a20  n(w_edges) > 0: 
+00006d20: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00006d30: 2020 2020 2020 7374 7265 6e67 7468 7320        strengths 
+00006d40: 3d20 736f 7274 6564 286c 6973 7428 7365  = sorted(list(se
+00006d50: 7428 5b65 5b32 5d20 666f 7220 6520 696e  t([e[2] for e in
+00006d60: 2077 5f65 6467 6573 5d29 292c 2072 6576   w_edges])), rev
+00006d70: 6572 7365 3d54 7275 6529 0a20 2020 2020  erse=True).     
+00006d80: 2020 2020 2020 2073 6f72 7465 645f 6564         sorted_ed
+00006d90: 6765 7320 3d20 5b5b 6520 666f 7220 6520  ges = [[e for e 
+00006da0: 696e 2077 5f65 6467 6573 2069 6620 655b  in w_edges if e[
+00006db0: 325d 203d 3d20 735d 2066 6f72 2073 2069  2] == s] for s i
+00006dc0: 6e20 7374 7265 6e67 7468 735d 0a20 2020  n strengths].   
+00006dd0: 2020 2020 2020 2020 2074 6273 203d 2070           tbs = p
+00006de0: 726f 6475 6374 282a 5b70 6572 6d75 7461  roduct(*[permuta
+00006df0: 7469 6f6e 7328 6564 6765 7329 2066 6f72  tions(edges) for
+00006e00: 2065 6467 6573 2069 6e20 736f 7274 6564   edges in sorted
+00006e10: 5f65 6467 6573 5d29 0a20 2020 2020 2020  _edges]).       
+00006e20: 2020 2020 2066 6f72 2074 6220 696e 2074       for tb in t
+00006e30: 6273 3a0a 2020 2020 2020 2020 2020 2020  bs:.            
+00006e40: 2020 2020 6564 6765 7320 3d20 666c 6174      edges = flat
+00006e50: 7465 6e28 7462 290a 2020 2020 2020 2020  ten(tb).        
+00006e60: 2020 2020 2020 2020 7270 5f64 6566 6561          rp_defea
+00006e70: 7420 3d20 5350 4f28 6c65 6e28 6361 6e64  t = SPO(len(cand
+00006e80: 6964 6174 6573 2929 0a20 2020 2020 2020  idates)).       
+00006e90: 2020 2020 2020 2020 2066 6f72 2065 302c           for e0,
+00006ea0: 6531 2c73 2069 6e20 6564 6765 733a 200a  e1,s in edges: .
+00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ec0: 2020 2020 6966 206e 6f74 2072 705f 6465      if not rp_de
+00006ed0: 6665 6174 2e50 5b63 616e 645f 746f 5f63  feat.P[cand_to_c
+00006ee0: 6964 785b 6531 5d5d 5b63 616e 645f 746f  idx[e1]][cand_to
+00006ef0: 5f63 6964 785b 6530 5d5d 3a0a 2020 2020  _cidx[e0]]:.    
+00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f10: 2020 2020 7270 5f64 6566 6561 742e 6164      rp_defeat.ad
+00006f20: 6428 6361 6e64 5f74 6f5f 6369 6478 5b65  d(cand_to_cidx[e
+00006f30: 305d 2c63 616e 645f 746f 5f63 6964 785b  0],cand_to_cidx[
+00006f40: 6531 5d29 0a20 2020 2020 2020 2020 2020  e1]).           
+00006f50: 2020 2020 2077 696e 6e65 7273 2e61 7070       winners.app
+00006f60: 656e 6428 6369 6478 5f74 6f5f 6361 6e64  end(cidx_to_cand
+00006f70: 5b72 705f 6465 6665 6174 2e69 6e69 7469  [rp_defeat.initi
+00006f80: 616c 5f65 6c65 6d65 6e74 7328 295b 305d  al_elements()[0]
+00006f90: 5d29 0a20 2020 2020 2020 2065 6c73 653a  ]).        else:
+00006fa0: 200a 2020 2020 2020 2020 2020 2020 7769   .            wi
+00006fb0: 6e6e 6572 7320 3d20 6361 6e64 6964 6174  nners = candidat
+00006fc0: 6573 0a20 2020 2072 6574 7572 6e20 736f  es.    return so
+00006fd0: 7274 6564 286c 6973 7428 7365 7428 7769  rted(list(set(wi
+00006fe0: 6e6e 6572 7329 2929 0a0a 0a40 766d 286e  nners)))...@vm(n
+00006ff0: 616d 653d 2252 616e 6b65 6420 5061 6972  ame="Ranked Pair
+00007000: 7322 290a 6465 6620 7261 6e6b 6564 5f70  s").def ranked_p
+00007010: 6169 7273 280a 2020 2020 6564 6174 612c  airs(.    edata,
+00007020: 200a 2020 2020 6375 7272 5f63 616e 6473   .    curr_cands
+00007030: 3d4e 6f6e 652c 200a 2020 2020 7374 7265  =None, .    stre
+00007040: 6e67 7468 5f66 756e 6374 696f 6e3d 4e6f  ngth_function=No
+00007050: 6e65 2c20 0a20 2020 2061 6c67 6f72 6974  ne, .    algorit
+00007060: 686d 3d27 6261 7369 6327 293a 2020 200a  hm='basic'):   .
+00007070: 2020 2020 2222 220a 2020 2020 4f72 6465      """.    Orde
+00007080: 7220 7468 6520 6564 6765 7320 696e 2074  r the edges in t
+00007090: 6865 206d 6172 6769 6e20 6772 6170 6820  he margin graph 
+000070a0: 6672 6f6d 206c 6172 6765 7374 2074 6f20  from largest to 
+000070b0: 736d 616c 6c65 7374 2061 6e64 206c 6f63  smallest and loc
+000070c0: 6b20 7468 656d 2069 6e20 696e 2074 6861  k them in in tha
+000070d0: 7420 6f72 6465 722c 2073 6b69 7070 696e  t order, skippin
+000070e0: 6720 6564 6765 7320 7468 6174 2063 7265  g edges that cre
+000070f0: 6174 6520 6120 6379 636c 652e 2020 4966  ate a cycle.  If
+00007100: 2074 6865 7265 2061 7265 2074 6965 7320   there are ties 
+00007110: 696e 2074 6865 206d 6172 6769 6e73 2c20  in the margins, 
+00007120: 6272 6561 6b20 7468 6520 7469 6573 2075  break the ties u
+00007130: 7369 6e67 2061 2074 6965 2d62 7265 616b  sing a tie-break
+00007140: 696e 6720 7275 6c65 3a20 6120 6c69 6e65  ing rule: a line
+00007150: 6172 206f 7264 6572 696e 6720 6f76 6572  ar ordering over
+00007160: 2074 6865 2065 6467 6573 2e20 2020 4120   the edges.   A 
+00007170: 6361 6e64 6964 6174 6520 6973 2061 2052  candidate is a R
+00007180: 616e 6b65 6420 5061 6972 7320 7769 6e6e  anked Pairs winn
+00007190: 6572 2069 6620 6974 2077 696e 7320 6163  er if it wins ac
+000071a0: 636f 7264 696e 6720 746f 2073 6f6d 6520  cording to some 
+000071b0: 7469 652d 6272 6561 6b69 6e67 2072 756c  tie-breaking rul
+000071c0: 652e 2041 6c73 6f20 6b6e 6f77 6e20 6173  e. Also known as
+000071d0: 2054 6964 656d 616e 2773 2052 756c 652e   Tideman's Rule.
+000071e0: 0a0a 2020 2020 2e2e 2077 6172 6e69 6e67  ..    .. warning
+000071f0: 3a3a 200a 2020 2020 2020 2020 5468 6973  :: .        This
+00007200: 206d 6574 686f 6420 6361 6e20 7461 6b65   method can take
+00007210: 2061 2076 6572 7920 6c6f 6e67 2074 696d   a very long tim
+00007220: 6520 746f 2066 696e 6420 7769 6e6e 6572  e to find winner
+00007230: 732e 200a 2020 2020 2020 2020 0a20 2020  s. .        .   
+00007240: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
+00007250: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
+00007260: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
+00007270: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
+00007280: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
+00007290: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
+000072a0: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
+000072b0: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
+000072c0: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
+000072d0: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
+000072e0: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
+000072f0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
+00007300: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
+00007310: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
+00007320: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
+00007330: 7360 600a 2020 2020 2020 2020 7374 7265  s``.        stre
+00007340: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
+00007350: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
+00007360: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
+00007370: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
+00007380: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
+00007390: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
+000073a0: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
+000073b0: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
+000073c0: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
+000073d0: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
+000073e0: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
+000073f0: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
+00007400: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
+00007410: 7264 6572 732e 200a 2020 2020 2020 2020  rders. .        
+00007420: 616c 676f 7269 7468 6d20 2873 7472 2c20  algorithm (str, 
+00007430: 6f70 7469 6f6e 616c 293a 2053 7065 6369  optional): Speci
+00007440: 6679 2077 6869 6368 2061 6c67 6f72 6974  fy which algorit
+00007450: 686d 2074 6f20 7573 652e 2020 4f70 7469  hm to use.  Opti
+00007460: 6f6e 7320 6172 6520 2762 6173 6963 2720  ons are 'basic' 
+00007470: 2874 6865 2064 6566 6175 6c74 2920 616e  (the default) an
+00007480: 6420 2766 726f 6d5f 7374 6163 6b73 272e  d 'from_stacks'.
+00007490: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
+000074a0: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
+000074b0: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
+000074c0: 7465 732e 200a 0a20 2020 202e 2e20 7365  tes. ..    .. se
+000074d0: 6561 6c73 6f3a 3a0a 0a20 2020 2020 2020  ealso::..       
+000074e0: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
+000074f0: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
+00007500: 5f6d 6574 686f 6473 2e72 616e 6b65 645f  _methods.ranked_
+00007510: 7061 6972 735f 7769 7468 5f74 6573 7460  pairs_with_test`
+00007520: 2c20 3a6d 6574 683a 6070 7265 665f 766f  , :meth:`pref_vo
+00007530: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+00007540: 645f 6d65 7468 6f64 732e 7261 6e6b 6564  d_methods.ranked
+00007550: 5f70 6169 7273 5f7a 7460 2c20 3a6d 6574  _pairs_zt`, :met
+00007560: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
+00007570: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+00007580: 6f64 732e 7261 6e6b 6564 5f70 6169 7273  ods.ranked_pairs
+00007590: 5f64 6566 6561 7473 600a 0a20 2020 203a  _defeats`..    :
+000075a0: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
+000075b0: 2e20 706c 6f74 3a3a 2020 6d61 7267 696e  . plot::  margin
+000075c0: 5f67 7261 7068 735f 6578 616d 706c 6573  _graphs_examples
+000075d0: 2f6d 675f 6578 5f62 705f 7270 2e70 790a  /mg_ex_bp_rp.py.
+000075e0: 2020 2020 2020 2020 3a63 6f6e 7465 7874          :context
+000075f0: 3a20 7265 7365 7420 200a 2020 2020 2020  : reset  .      
+00007600: 2020 3a69 6e63 6c75 6465 2d73 6f75 7263    :include-sourc
+00007610: 653a 2054 7275 650a 0a0a 2020 2020 2e2e  e: True...    ..
+00007620: 2063 6f64 652d 626c 6f63 6b3a 3a20 0a0a   code-block:: ..
+00007630: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+00007640: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+00007650: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
+00007660: 706f 7274 2072 616e 6b65 645f 7061 6972  port ranked_pair
+00007670: 730a 0a20 2020 2020 2020 2072 616e 6b65  s..        ranke
+00007680: 645f 7061 6972 732e 6469 7370 6c61 7928  d_pairs.display(
+00007690: 6d67 290a 2020 2020 2020 2020 7261 6e6b  mg).        rank
+000076a0: 6564 5f70 6169 7273 2e64 6973 706c 6179  ed_pairs.display
+000076b0: 286d 672c 2061 6c67 6f72 6974 686d 3d27  (mg, algorithm='
+000076c0: 6261 7369 6327 2920 0a20 2020 2020 2020  basic') .       
+000076d0: 2072 616e 6b65 645f 7061 6972 732e 6469   ranked_pairs.di
+000076e0: 7370 6c61 7928 6d67 2c20 616c 676f 7269  splay(mg, algori
+000076f0: 7468 6d3d 2766 726f 6d5f 7374 6163 6b73  thm='from_stacks
+00007700: 2729 2020 2020 0a0a 0a20 2020 202e 2e20  ')    ...    .. 
+00007710: 6578 6563 5f63 6f64 653a 3a20 0a20 2020  exec_code:: .   
+00007720: 2020 2020 203a 6869 6465 5f63 6f64 653a       :hide_code:
+00007730: 0a0a 2020 2020 2020 2020 6672 6f6d 2070  ..        from p
+00007740: 7265 665f 766f 7469 6e67 2e77 6569 6768  ref_voting.weigh
+00007750: 7465 645f 6d61 6a6f 7269 7479 5f67 7261  ted_majority_gra
+00007760: 7068 7320 696d 706f 7274 204d 6172 6769  phs import Margi
+00007770: 6e47 7261 7068 0a20 2020 2020 2020 2066  nGraph.        f
+00007780: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
+00007790: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+000077a0: 686f 6473 2069 6d70 6f72 7420 7261 6e6b  hods import rank
+000077b0: 6564 5f70 6169 7273 0a20 2020 2020 2020  ed_pairs.       
+000077c0: 200a 2020 2020 2020 2020 6d67 203d 204d   .        mg = M
+000077d0: 6172 6769 6e47 7261 7068 285b 302c 2031  arginGraph([0, 1
+000077e0: 2c20 322c 2033 5d2c 205b 2830 2c20 322c  , 2, 3], [(0, 2,
+000077f0: 2033 292c 2028 312c 2030 2c20 3529 2c20   3), (1, 0, 5), 
+00007800: 2832 2c20 312c 2035 292c 2028 322c 2033  (2, 1, 5), (2, 3
+00007810: 2c20 3129 2c20 2833 2c20 302c 2033 292c  , 1), (3, 0, 3),
+00007820: 2028 332c 2031 2c20 3129 5d29 0a20 2020   (3, 1, 1)]).   
+00007830: 2020 2020 200a 2020 2020 2020 2020 7261       .        ra
+00007840: 6e6b 6564 5f70 6169 7273 2e64 6973 706c  nked_pairs.displ
+00007850: 6179 286d 6729 0a20 2020 2020 2020 2072  ay(mg).        r
+00007860: 616e 6b65 645f 7061 6972 732e 6469 7370  anked_pairs.disp
+00007870: 6c61 7928 6d67 2c20 616c 676f 7269 7468  lay(mg, algorith
+00007880: 6d3d 2762 6173 6963 2729 0a20 2020 2020  m='basic').     
+00007890: 2020 2072 616e 6b65 645f 7061 6972 732e     ranked_pairs.
+000078a0: 6469 7370 6c61 7928 6d67 2c20 616c 676f  display(mg, algo
+000078b0: 7269 7468 6d3d 2766 726f 6d5f 7374 6163  rithm='from_stac
+000078c0: 6b73 2729 0a0a 2020 2020 2222 220a 0a20  ks')..    """.. 
+000078d0: 2020 2069 6620 616c 676f 7269 7468 6d20     if algorithm 
+000078e0: 3d3d 2027 6261 7369 6327 3a0a 2020 2020  == 'basic':.    
+000078f0: 2020 2020 7265 7475 726e 205f 7261 6e6b      return _rank
+00007900: 6564 5f70 6169 7273 5f62 6173 6963 2865  ed_pairs_basic(e
+00007910: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
+00007920: 203d 2063 7572 725f 6361 6e64 732c 2073   = curr_cands, s
+00007930: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00007940: 203d 2073 7472 656e 6774 685f 6675 6e63   = strength_func
+00007950: 7469 6f6e 290a 2020 2020 656c 6966 2061  tion).    elif a
+00007960: 6c67 6f72 6974 686d 203d 3d20 2766 726f  lgorithm == 'fro
+00007970: 6d5f 7374 6163 6b73 273a 0a20 2020 2020  m_stacks':.     
+00007980: 2020 2072 6574 7572 6e20 5f72 616e 6b65     return _ranke
+00007990: 645f 7061 6972 735f 6672 6f6d 5f73 7461  d_pairs_from_sta
+000079a0: 636b 7328 6564 6174 612c 2063 7572 725f  cks(edata, curr_
+000079b0: 6361 6e64 7320 3d20 6375 7272 5f63 616e  cands = curr_can
+000079c0: 6473 290a 2020 2020 656c 7365 3a0a 2020  ds).    else:.  
+000079d0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+000079e0: 6545 7272 6f72 2822 496e 7661 6c69 6420  eError("Invalid 
+000079f0: 616c 676f 7269 7468 6d20 7370 6563 6966  algorithm specif
+00007a00: 6965 642e 2229 0a0a 0a40 766d 286e 616d  ied.")...@vm(nam
+00007a10: 653d 2252 616e 6b65 6420 5061 6972 7322  e="Ranked Pairs"
+00007a20: 290a 6465 6620 7261 6e6b 6564 5f70 6169  ).def ranked_pai
+00007a30: 7273 5f77 6974 685f 7465 7374 280a 2020  rs_with_test(.  
+00007a40: 2020 6564 6174 612c 200a 2020 2020 6375    edata, .    cu
+00007a50: 7272 5f63 616e 6473 3d4e 6f6e 652c 200a  rr_cands=None, .
+00007a60: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+00007a70: 6374 696f 6e3d 4e6f 6e65 293a 2020 200a  ction=None):   .
+00007a80: 2020 2020 2222 2246 696e 6420 7468 6520      """Find the 
+00007a90: 5261 6e6b 6564 2050 6169 7273 2077 696e  Ranked Pairs win
+00007aa0: 6e65 7273 2c20 6275 7420 696e 636c 7564  ners, but includ
+00007ab0: 6520 6120 7465 7374 2074 6f20 6465 7465  e a test to dete
+00007ac0: 726d 696e 6564 2069 6620 6974 2077 696c  rmined if it wil
+00007ad0: 6c20 7461 6b65 2074 6f6f 206c 6f6e 6720  l take too long 
+00007ae0: 746f 2063 6f6d 7075 7465 2074 6865 2052  to compute the R
+00007af0: 616e 6b65 6420 5061 6972 7320 7769 6e6e  anked Pairs winn
+00007b00: 6572 732e 2049 6620 7468 6520 6361 6c63  ers. If the calc
+00007b10: 756c 6174 696f 6e20 6f66 2074 6865 2077  ulation of the w
+00007b20: 696e 6e65 7273 2077 696c 6c20 7461 6b65  inners will take
+00007b30: 2074 6f6f 206c 6f6e 672c 2072 6574 7572   too long, retur
+00007b40: 6e20 4e6f 6e65 2e0a 0a20 2020 202e 2e20  n None...    .. 
+00007b50: 696d 706f 7274 616e 743a 3a0a 2020 2020  important::.    
+00007b60: 2020 2020 5468 6973 2076 6f74 696e 6720      This voting 
+00007b70: 6d65 7468 6f64 2074 6861 7420 6d69 6768  method that migh
+00007b80: 7420 7265 7475 726e 204e 6f6e 6520 7261  t return None ra
+00007b90: 7468 6572 2074 6861 6e20 6120 6c69 7374  ther than a list
+00007ba0: 206f 6620 6361 6e64 6964 6174 6573 2e20   of candidates. 
+00007bb0: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
+00007bc0: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
+00007bd0: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
+00007be0: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
+00007bf0: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
+00007c00: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
+00007c10: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
+00007c20: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
+00007c30: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
+00007c40: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+00007c50: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
+00007c60: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
+00007c70: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
+00007c80: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
+00007c90: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
+00007ca0: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
+00007cb0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+00007cc0: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
+00007cd0: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
+00007ce0: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
+00007cf0: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
+00007d00: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
+00007d10: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
+00007d20: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
+00007d30: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
+00007d40: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
+00007d50: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
+00007d60: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
+00007d70: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
+00007d80: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
+00007d90: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+00007da0: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
+00007db0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
+00007dc0: 2e20 0a0a 2020 2020 2e2e 2073 6565 616c  . ..    .. seeal
+00007dd0: 736f 3a3a 0a0a 2020 2020 2020 2020 3a6d  so::..        :m
+00007de0: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
+00007df0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+00007e00: 7468 6f64 732e 7261 6e6b 6564 5f70 6169  thods.ranked_pai
+00007e10: 7273 5f77 6974 685f 7465 7374 602c 203a  rs_with_test`, :
+00007e20: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
+00007e30: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
+00007e40: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
+00007e50: 6972 735f 7a74 602c 203a 6d65 7468 3a60  irs_zt`, :meth:`
+00007e60: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+00007e70: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+00007e80: 2e72 616e 6b65 645f 7061 6972 735f 6465  .ranked_pairs_de
+00007e90: 6665 6174 7360 0a0a 2020 2020 3a45 7861  feats`..    :Exa
+00007ea0: 6d70 6c65 3a20 0a0a 2020 2020 2e2e 2070  mple: ..    .. p
+00007eb0: 6c6f 743a 3a20 206d 6172 6769 6e5f 6772  lot::  margin_gr
+00007ec0: 6170 6873 5f65 7861 6d70 6c65 732f 6d67  aphs_examples/mg
+00007ed0: 5f65 785f 7270 5f77 6974 685f 7465 7374  _ex_rp_with_test
+00007ee0: 2e70 790a 2020 2020 2020 2020 3a63 6f6e  .py.        :con
+00007ef0: 7465 7874 3a20 7265 7365 7420 200a 2020  text: reset  .  
+00007f00: 2020 2020 2020 3a69 6e63 6c75 6465 2d73        :include-s
+00007f10: 6f75 7263 653a 2054 7275 650a 0a0a 2020  ource: True...  
+00007f20: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+00007f30: 3a20 0a0a 2020 2020 2020 2020 6672 6f6d  : ..        from
+00007f40: 2070 7265 665f 766f 7469 6e67 2e6d 6172   pref_voting.mar
+00007f50: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+00007f60: 7320 696d 706f 7274 2072 616e 6b65 645f  s import ranked_
+00007f70: 7061 6972 735f 7769 7468 5f74 6573 740a  pairs_with_test.
+00007f80: 0a20 2020 2020 2020 2072 616e 6b65 645f  .        ranked_
+00007f90: 7061 6972 735f 7769 7468 5f74 6573 742e  pairs_with_test.
+00007fa0: 6469 7370 6c61 7928 6d67 290a 0a0a 2020  display(mg)...  
+00007fb0: 2020 2e2e 2065 7865 635f 636f 6465 3a3a    .. exec_code::
+00007fc0: 200a 2020 2020 2020 2020 3a68 6964 655f   .        :hide_
+00007fd0: 636f 6465 3a0a 0a20 2020 2020 2020 2066  code:..        f
+00007fe0: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
+00007ff0: 7765 6967 6874 6564 5f6d 616a 6f72 6974  weighted_majorit
+00008000: 795f 6772 6170 6873 2069 6d70 6f72 7420  y_graphs import 
+00008010: 4d61 7267 696e 4772 6170 680a 2020 2020  MarginGraph.    
+00008020: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
+00008030: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+00008040: 645f 6d65 7468 6f64 7320 696d 706f 7274  d_methods import
+00008050: 2072 616e 6b65 645f 7061 6972 735f 7769   ranked_pairs_wi
+00008060: 7468 5f74 6573 740a 2020 2020 2020 2020  th_test.        
+00008070: 0a20 2020 2020 2020 206d 6720 3d20 4d61  .        mg = Ma
+00008080: 7267 696e 4772 6170 6828 5b30 2c20 312c  rginGraph([0, 1,
+00008090: 2032 2c20 335d 2c20 5b28 312c 2032 2c20   2, 3], [(1, 2, 
+000080a0: 3229 2c20 2831 2c20 332c 2032 292c 2028  2), (1, 3, 2), (
+000080b0: 322c 2030 2c20 3229 5d29 0a20 2020 2020  2, 0, 2)]).     
+000080c0: 2020 200a 2020 2020 2020 2020 7261 6e6b     .        rank
+000080d0: 6564 5f70 6169 7273 5f77 6974 685f 7465  ed_pairs_with_te
+000080e0: 7374 2e64 6973 706c 6179 286d 6729 0a0a  st.display(mg)..
+000080f0: 0a20 2020 2022 2222 2020 2020 0a20 2020  .    """    .   
+00008100: 2063 616e 6469 6461 7465 7320 3d20 6564   candidates = ed
+00008110: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
+00008120: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
+00008130: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
+00008140: 616e 6473 2020 2020 0a20 2020 2063 6964  ands    .    cid
+00008150: 785f 746f 5f63 616e 6420 3d20 7b63 6964  x_to_cand = {cid
+00008160: 783a 2063 2066 6f72 2063 6964 782c 2063  x: c for cidx, c
+00008170: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
+00008180: 6e64 6964 6174 6573 297d 2020 0a20 2020  ndidates)}  .   
+00008190: 2063 616e 645f 746f 5f63 6964 7820 3d20   cand_to_cidx = 
+000081a0: 7b63 3a20 6369 6478 2066 6f72 2063 6964  {c: cidx for cid
+000081b0: 782c 2063 2069 6e20 656e 756d 6572 6174  x, c in enumerat
+000081c0: 6528 6361 6e64 6964 6174 6573 297d 2020  e(candidates)}  
+000081d0: 0a20 2020 200a 2020 2020 7374 7265 6e67  .    .    streng
+000081e0: 7468 5f66 756e 6374 696f 6e20 3d20 6564  th_function = ed
+000081f0: 6174 612e 6d61 7267 696e 2069 6620 7374  ata.margin if st
+00008200: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+00008210: 6973 204e 6f6e 6520 656c 7365 2073 7472  is None else str
+00008220: 656e 6774 685f 6675 6e63 7469 6f6e 2020  ength_function  
+00008230: 200a 0a20 2020 2063 7720 3d20 6564 6174   ..    cw = edat
+00008240: 612e 636f 6e64 6f72 6365 745f 7769 6e6e  a.condorcet_winn
+00008250: 6572 2863 7572 725f 6361 6e64 7320 3d20  er(curr_cands = 
+00008260: 6375 7272 5f63 616e 6473 290a 2020 2020  curr_cands).    
+00008270: 2320 5261 6e6b 6564 2050 6169 7273 2069  # Ranked Pairs i
+00008280: 7320 436f 6e64 6f72 6365 7420 636f 6e73  s Condorcet cons
+00008290: 6973 7465 6e74 2c20 736f 2073 696d 706c  istent, so simpl
+000082a0: 7920 7265 7475 726e 2074 6865 2043 6f6e  y return the Con
+000082b0: 646f 7263 6574 2077 696e 6e65 7220 6966  dorcet winner if
+000082c0: 2065 7869 7374 730a 2020 2020 6966 2063   exists.    if c
+000082d0: 7720 6973 206e 6f74 204e 6f6e 653a 200a  w is not None: .
+000082e0: 2020 2020 2020 2020 7769 6e6e 6572 7320          winners 
+000082f0: 3d20 5b63 775d 0a20 2020 2065 6c73 653a  = [cw].    else:
+00008300: 0a20 2020 2020 2020 2077 5f65 6467 6573  .        w_edges
+00008310: 203d 205b 2863 312c 2063 322c 2073 7472   = [(c1, c2, str
+00008320: 656e 6774 685f 6675 6e63 7469 6f6e 2863  ength_function(c
+00008330: 312c 2063 3229 2920 666f 7220 6331 2069  1, c2)) for c1 i
+00008340: 6e20 6361 6e64 6964 6174 6573 2066 6f72  n candidates for
+00008350: 2063 3220 696e 2063 616e 6469 6461 7465   c2 in candidate
+00008360: 7320 0a20 2020 2020 2020 2020 2020 2020  s .             
+00008370: 2020 2020 2020 6966 2063 3120 213d 2063        if c1 != c
+00008380: 3220 616e 6420 2865 6461 7461 2e6d 616a  2 and (edata.maj
+00008390: 6f72 6974 795f 7072 6566 6572 7328 6331  ority_prefers(c1
+000083a0: 2c20 6332 2920 6f72 2065 6461 7461 2e69  , c2) or edata.i
+000083b0: 735f 7469 6564 2863 312c 2063 3229 295d  s_tied(c1, c2))]
+000083c0: 0a20 2020 2020 2020 2077 696e 6e65 7273  .        winners
+000083d0: 203d 206c 6973 7428 2920 2020 2020 2020   = list()       
+000083e0: 2020 2020 200a 2020 2020 2020 2020 7374       .        st
+000083f0: 7265 6e67 7468 7320 3d20 736f 7274 6564  rengths = sorted
+00008400: 286c 6973 7428 7365 7428 5b65 5b32 5d20  (list(set([e[2] 
+00008410: 666f 7220 6520 696e 2077 5f65 6467 6573  for e in w_edges
+00008420: 5d29 292c 2072 6576 6572 7365 3d54 7275  ])), reverse=Tru
+00008430: 6529 0a20 2020 2020 2020 2073 6f72 7465  e).        sorte
+00008440: 645f 6564 6765 7320 3d20 5b5b 6520 666f  d_edges = [[e fo
+00008450: 7220 6520 696e 2077 5f65 6467 6573 2069  r e in w_edges i
+00008460: 6620 655b 325d 203d 3d20 735d 2066 6f72  f e[2] == s] for
+00008470: 2073 2069 6e20 7374 7265 6e67 7468 735d   s in strengths]
+00008480: 0a20 2020 2020 2020 2069 6620 6e70 2e70  .        if np.p
+00008490: 726f 6428 5b6d 6174 682e 6661 6374 6f72  rod([math.factor
+000084a0: 6961 6c28 6c65 6e28 6573 2929 2066 6f72  ial(len(es)) for
+000084b0: 2065 7320 696e 2073 6f72 7465 645f 6564   es in sorted_ed
+000084c0: 6765 735d 2920 3e20 3330 3030 3a20 0a20  ges]) > 3000: . 
+000084d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000084e0: 6e20 4e6f 6e65 0a20 2020 2020 2020 2065  n None.        e
+000084f0: 6c73 653a 200a 2020 2020 2020 2020 2020  lse: .          
+00008500: 2020 7462 7320 3d20 7072 6f64 7563 7428    tbs = product(
+00008510: 2a5b 7065 726d 7574 6174 696f 6e73 2865  *[permutations(e
+00008520: 6467 6573 2920 666f 7220 6564 6765 7320  dges) for edges 
+00008530: 696e 2073 6f72 7465 645f 6564 6765 735d  in sorted_edges]
+00008540: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+00008550: 7220 7462 2069 6e20 7462 733a 0a20 2020  r tb in tbs:.   
+00008560: 2020 2020 2020 2020 2020 2020 2065 6467               edg
+00008570: 6573 203d 2066 6c61 7474 656e 2874 6229  es = flatten(tb)
+00008580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008590: 2072 705f 6465 6665 6174 203d 2053 504f   rp_defeat = SPO
+000085a0: 286c 656e 2863 616e 6469 6461 7465 7329  (len(candidates)
+000085b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000085c0: 2020 666f 7220 6530 2c65 312c 7320 696e    for e0,e1,s in
+000085d0: 2065 6467 6573 3a20 0a20 2020 2020 2020   edges: .       
+000085e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000085f0: 6e6f 7420 7270 5f64 6566 6561 742e 505b  not rp_defeat.P[
+00008600: 6361 6e64 5f74 6f5f 6369 6478 5b65 315d  cand_to_cidx[e1]
+00008610: 5d5b 6361 6e64 5f74 6f5f 6369 6478 5b65  ][cand_to_cidx[e
+00008620: 305d 5d3a 0a20 2020 2020 2020 2020 2020  0]]:.           
+00008630: 2020 2020 2020 2020 2020 2020 2072 705f               rp_
+00008640: 6465 6665 6174 2e61 6464 2863 616e 645f  defeat.add(cand_
+00008650: 746f 5f63 6964 785b 6530 5d2c 6361 6e64  to_cidx[e0],cand
+00008660: 5f74 6f5f 6369 6478 5b65 315d 290a 2020  _to_cidx[e1]).  
+00008670: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00008680: 6e6e 6572 732e 6170 7065 6e64 2863 6964  nners.append(cid
+00008690: 785f 746f 5f63 616e 645b 7270 5f64 6566  x_to_cand[rp_def
+000086a0: 6561 742e 696e 6974 6961 6c5f 656c 656d  eat.initial_elem
+000086b0: 656e 7473 2829 5b30 5d5d 290a 2020 2020  ents()[0]]).    
+000086c0: 7265 7475 726e 2073 6f72 7465 6428 6c69  return sorted(li
+000086d0: 7374 2873 6574 2877 696e 6e65 7273 2929  st(set(winners))
+000086e0: 290a 0a64 6566 2072 616e 6b65 645f 7061  )..def ranked_pa
+000086f0: 6972 735f 6465 6665 6174 7328 6564 6174  irs_defeats(edat
+00008700: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
+00008710: 4e6f 6e65 2c20 7374 7265 6e67 7468 5f66  None, strength_f
+00008720: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
+00008730: 2020 200a 2020 2020 2222 220a 2020 2020     .    """.    
+00008740: 5265 7475 726e 7320 7468 6520 5261 6e6b  Returns the Rank
+00008750: 6564 2050 6169 7273 2064 6566 6561 7420  ed Pairs defeat 
+00008760: 7265 6c61 7469 6f6e 7320 7072 6f64 7563  relations produc
+00008770: 6564 2062 7920 7468 6520 5261 6e6b 6564  ed by the Ranked
+00008780: 2050 6169 7273 2061 6c67 6f72 6974 686d   Pairs algorithm
+00008790: 2e20 0a0a 2020 2020 2e2e 2069 6d70 6f72  . ..    .. impor
+000087a0: 7461 6e74 3a3a 0a20 2020 2020 2020 2055  tant::.        U
+000087b0: 6e6c 696b 6520 7468 6520 6f74 6865 7220  nlike the other 
+000087c0: 6675 6e63 7469 6f6e 7320 7468 6174 2072  functions that r
+000087d0: 6574 7572 6e20 6120 7369 6e67 6c65 2064  eturn a single d
+000087e0: 6566 6561 7420 7265 6c61 7469 6f6e 2c20  efeat relation, 
+000087f0: 7468 6973 2072 6574 7572 6e73 2061 206c  this returns a l
+00008800: 6973 7420 6f66 2064 6566 6561 7420 7265  ist of defeat re
+00008810: 6c61 7469 6f6e 732e 200a 2020 2020 2020  lations. .      
+00008820: 2020 0a20 2020 2041 7267 733a 0a20 2020    .    Args:.   
+00008830: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
+00008840: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
+00008850: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
+00008860: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
+00008870: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
+00008880: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
+00008890: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
+000088a0: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
+000088b0: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+000088c0: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
+000088d0: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
+000088e0: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
+000088f0: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
+00008900: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
+00008910: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
+00008920: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+00008930: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
+00008940: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
+00008950: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
+00008960: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
+00008970: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
+00008980: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
+00008990: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
+000089a0: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
+000089b0: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
+000089c0: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
+000089d0: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
+000089e0: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
+000089f0: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
+00008a00: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+00008a10: 2020 2020 2041 206e 6574 776f 726b 7820       A networkx 
+00008a20: 4469 4772 6170 6820 7265 7072 6573 656e  DiGraph represen
+00008a30: 7469 6e67 2074 6865 2052 616e 6b65 6420  ting the Ranked 
+00008a40: 5061 6972 7320 6465 6665 6174 2072 656c  Pairs defeat rel
+00008a50: 6174 696f 6e2e 200a 0a20 2020 202e 2e20  ation. ..    .. 
+00008a60: 7365 6561 6c73 6f3a 3a0a 0a20 2020 2020  seealso::..     
+00008a70: 2020 203a 6d65 7468 3a60 7072 6566 5f76     :meth:`pref_v
+00008a80: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
+00008a90: 6564 5f6d 6574 686f 6473 2e72 616e 6b65  ed_methods.ranke
+00008aa0: 645f 7061 6972 7360 2c20 3a6d 6574 683a  d_pairs`, :meth:
+00008ab0: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
+00008ac0: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+00008ad0: 732e 7261 6e6b 6564 5f70 6169 7273 5f77  s.ranked_pairs_w
+00008ae0: 6974 685f 7465 7374 600a 0a20 2020 203a  ith_test`..    :
+00008af0: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
+00008b00: 2e20 706c 6f74 3a3a 2020 6d61 7267 696e  . plot::  margin
+00008b10: 5f67 7261 7068 735f 6578 616d 706c 6573  _graphs_examples
+00008b20: 2f6d 675f 6578 5f72 705f 6465 6665 6174  /mg_ex_rp_defeat
+00008b30: 732e 7079 0a20 2020 2020 2020 203a 636f  s.py.        :co
+00008b40: 6e74 6578 743a 2072 6573 6574 2020 0a20  ntext: reset  . 
+00008b50: 2020 2020 2020 203a 696e 636c 7564 652d         :include-
+00008b60: 736f 7572 6365 3a20 5472 7565 0a0a 2020  source: True..  
+00008b70: 2020 2e2e 2065 7865 635f 636f 6465 3a3a    .. exec_code::
+00008b80: 0a0a 0a20 2020 2020 2020 2066 726f 6d20  ...        from 
+00008b90: 7072 6566 5f76 6f74 696e 672e 7765 6967  pref_voting.weig
+00008ba0: 6874 6564 5f6d 616a 6f72 6974 795f 6772  hted_majority_gr
+00008bb0: 6170 6873 2069 6d70 6f72 7420 4d61 7267  aphs import Marg
+00008bc0: 696e 4772 6170 680a 2020 2020 2020 2020  inGraph.        
+00008bd0: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
+00008be0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+00008bf0: 7468 6f64 7320 696d 706f 7274 2072 616e  thods import ran
+00008c00: 6b65 645f 7061 6972 735f 6465 6665 6174  ked_pairs_defeat
+00008c10: 730a 0a20 2020 2020 2020 206d 6720 3d20  s..        mg = 
+00008c20: 4d61 7267 696e 4772 6170 6828 5b30 2c20  MarginGraph([0, 
+00008c30: 312c 2032 2c20 335d 2c20 5b28 302c 2031  1, 2, 3], [(0, 1
+00008c40: 2c20 3130 292c 2028 302c 2032 2c20 3229  , 10), (0, 2, 2)
+00008c50: 2c20 2831 2c20 332c 2034 292c 2028 322c  , (1, 3, 4), (2,
+00008c60: 2031 2c20 3629 2c20 2832 2c20 332c 2038   1, 6), (2, 3, 8
+00008c70: 292c 2028 332c 2030 2c20 3429 5d29 0a20  ), (3, 0, 4)]). 
+00008c80: 2020 2020 2020 2072 705f 6465 6665 6174         rp_defeat
+00008c90: 7320 3d20 7261 6e6b 6564 5f70 6169 7273  s = ranked_pairs
+00008ca0: 5f64 6566 6561 7473 286d 6729 0a0a 2020  _defeats(mg)..  
+00008cb0: 2020 2020 2020 666f 7220 7270 6420 696e        for rpd in
+00008cc0: 2072 705f 6465 6665 6174 733a 200a 2020   rp_defeats: .  
+00008cd0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00008ce0: 7270 642e 6564 6765 7329 0a0a 2020 2020  rpd.edges)..    
+00008cf0: 2222 220a 2020 2020 0a20 2020 2063 616e  """.    .    can
+00008d00: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
+00008d10: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
+00008d20: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
+00008d30: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
+00008d40: 2020 2020 0a20 2020 2073 7472 656e 6774      .    strengt
+00008d50: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
+00008d60: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
+00008d70: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
+00008d80: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
+00008d90: 6e67 7468 5f66 756e 6374 696f 6e20 2020  ngth_function   
+00008da0: 200a 0a20 2020 2077 5f65 6467 6573 203d   ..    w_edges =
+00008db0: 205b 2863 312c 2063 322c 2073 7472 656e   [(c1, c2, stren
+00008dc0: 6774 685f 6675 6e63 7469 6f6e 2863 312c  gth_function(c1,
+00008dd0: 2063 3229 2920 666f 7220 6331 2069 6e20   c2)) for c1 in 
+00008de0: 6361 6e64 6964 6174 6573 2066 6f72 2063  candidates for c
+00008df0: 3220 696e 2063 616e 6469 6461 7465 7320  2 in candidates 
+00008e00: 6966 2063 3120 213d 2063 3220 616e 6420  if c1 != c2 and 
+00008e10: 2865 6461 7461 2e6d 616a 6f72 6974 795f  (edata.majority_
+00008e20: 7072 6566 6572 7328 6331 2c20 6332 2920  prefers(c1, c2) 
+00008e30: 6f72 2065 6461 7461 2e69 735f 7469 6564  or edata.is_tied
+00008e40: 2863 312c 2063 3229 295d 0a20 2020 2077  (c1, c2))].    w
+00008e50: 696e 6e65 7273 203d 206c 6973 7428 2920  inners = list() 
+00008e60: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00008e70: 7374 7265 6e67 7468 7320 3d20 736f 7274  strengths = sort
+00008e80: 6564 286c 6973 7428 7365 7428 5b65 5b32  ed(list(set([e[2
+00008e90: 5d20 666f 7220 6520 696e 2077 5f65 6467  ] for e in w_edg
+00008ea0: 6573 5d29 292c 2072 6576 6572 7365 3d54  es])), reverse=T
+00008eb0: 7275 6529 0a20 2020 2073 6f72 7465 645f  rue).    sorted_
+00008ec0: 6564 6765 7320 3d20 5b5b 6520 666f 7220  edges = [[e for 
+00008ed0: 6520 696e 2077 5f65 6467 6573 2069 6620  e in w_edges if 
+00008ee0: 655b 325d 203d 3d20 735d 2066 6f72 2073  e[2] == s] for s
+00008ef0: 2069 6e20 7374 7265 6e67 7468 735d 0a20   in strengths]. 
+00008f00: 2020 2074 6273 203d 2070 726f 6475 6374     tbs = product
+00008f10: 282a 5b70 6572 6d75 7461 7469 6f6e 7328  (*[permutations(
+00008f20: 6564 6765 7329 2066 6f72 2065 6467 6573  edges) for edges
+00008f30: 2069 6e20 736f 7274 6564 5f65 6467 6573   in sorted_edges
+00008f40: 5d29 0a20 2020 2072 705f 6465 6665 6174  ]).    rp_defeat
+00008f50: 7320 3d20 6c69 7374 2829 0a20 2020 2066  s = list().    f
+00008f60: 6f72 2074 6220 696e 2074 6273 3a0a 2020  or tb in tbs:.  
+00008f70: 2020 2020 2020 6564 6765 7320 3d20 666c        edges = fl
+00008f80: 6174 7465 6e28 7462 290a 2020 2020 2020  atten(tb).      
+00008f90: 2020 7270 5f64 6566 6561 7420 3d20 6e78    rp_defeat = nx
+00008fa0: 2e44 6947 7261 7068 2829 200a 2020 2020  .DiGraph() .    
+00008fb0: 2020 2020 666f 7220 6520 696e 2065 6467      for e in edg
+00008fc0: 6573 3a20 0a20 2020 2020 2020 2020 2020  es: .           
+00008fd0: 2072 705f 6465 6665 6174 2e61 6464 5f65   rp_defeat.add_e
+00008fe0: 6467 6528 655b 305d 2c20 655b 315d 2c20  dge(e[0], e[1], 
+00008ff0: 7765 6967 6874 3d65 5b32 5d29 0a20 2020  weight=e[2]).   
+00009000: 2020 2020 2020 2020 2069 6620 646f 6573           if does
+00009010: 5f63 7265 6174 655f 6379 636c 6528 7270  _create_cycle(rp
+00009020: 5f64 6566 6561 742c 2065 293a 0a20 2020  _defeat, e):.   
+00009030: 2020 2020 2020 2020 2020 2020 2072 705f               rp_
+00009040: 6465 6665 6174 2e72 656d 6f76 655f 6564  defeat.remove_ed
+00009050: 6765 2865 5b30 5d2c 2065 5b31 5d29 0a20  ge(e[0], e[1]). 
+00009060: 2020 2020 2020 2072 705f 6465 6665 6174         rp_defeat
+00009070: 732e 6170 7065 6e64 2872 705f 6465 6665  s.append(rp_defe
+00009080: 6174 290a 2020 2020 2020 2020 7769 6e6e  at).        winn
+00009090: 6572 732e 6170 7065 6e64 286d 6178 696d  ers.append(maxim
+000090a0: 616c 5f65 6c65 6d65 6e74 7328 7270 5f64  al_elements(rp_d
+000090b0: 6566 6561 7429 5b30 5d29 0a20 2020 2072  efeat)[0]).    r
+000090c0: 6574 7572 6e20 7270 5f64 6566 6561 7473  eturn rp_defeats
+000090d0: 0a0a 0a40 766d 286e 616d 653d 2252 616e  ...@vm(name="Ran
+000090e0: 6b65 6420 5061 6972 7320 5442 2229 0a64  ked Pairs TB").d
+000090f0: 6566 2072 616e 6b65 645f 7061 6972 735f  ef ranked_pairs_
+00009100: 7462 280a 2020 2020 6564 6174 612c 200a  tb(.    edata, .
+00009110: 2020 2020 6375 7272 5f63 616e 6473 203d      curr_cands =
+00009120: 204e 6f6e 652c 200a 2020 2020 7469 655f   None, .    tie_
+00009130: 6272 6561 6b65 7220 3d20 4e6f 6e65 2c20  breaker = None, 
+00009140: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
+00009150: 6e63 7469 6f6e 203d 204e 6f6e 6529 3a20  nction = None): 
+00009160: 2020 0a20 2020 2022 2222 0a20 2020 2052    .    """.    R
+00009170: 616e 6b65 6420 5061 6972 7320 7769 7468  anked Pairs with
+00009180: 2061 2066 6978 6564 206c 696e 6561 7220   a fixed linear 
+00009190: 6f72 6465 7220 6f6e 2074 6865 2063 616e  order on the can
+000091a0: 6469 6461 7465 7320 746f 2062 7265 616b  didates to break
+000091b0: 2061 6e79 2074 6965 7320 696e 2074 6865   any ties in the
+000091c0: 206d 6172 6769 6e73 2e20 2020 0a20 2020   margins.   .   
+000091d0: 2053 696e 6365 2074 6865 2074 6965 5f62   Since the tie_b
+000091e0: 7265 616b 6572 2069 7320 6120 6c69 6e65  reaker is a line
+000091f0: 6172 206f 7264 6572 2c20 7468 6973 206d  ar order, this m
+00009200: 6574 686f 6420 6973 2072 6573 6f6c 7574  ethod is resolut
+00009210: 652e 2020 200a 0a20 2020 2041 7267 733a  e.   ..    Args:
+00009220: 0a20 2020 2020 2020 2065 6461 7461 2028  .        edata (
+00009230: 5072 6f66 696c 652c 2050 726f 6669 6c65  Profile, Profile
+00009240: 5769 7468 5469 6573 2c20 4d61 7267 696e  WithTies, Margin
+00009250: 4772 6170 6829 3a20 416e 7920 656c 6563  Graph): Any elec
+00009260: 7469 6f6e 2064 6174 6120 7468 6174 2068  tion data that h
+00009270: 6173 2061 2060 6d61 7267 696e 6020 6d65  as a `margin` me
+00009280: 7468 6f64 2e20 0a20 2020 2020 2020 2063  thod. .        c
+00009290: 7572 725f 6361 6e64 7320 284c 6973 745b  urr_cands (List[
+000092a0: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
+000092b0: 2049 6620 7365 742c 2074 6865 6e20 6669   If set, then fi
+000092c0: 6e64 2074 6865 2077 696e 6e65 7273 2066  nd the winners f
+000092d0: 6f72 2074 6865 2070 726f 6669 6c65 2072  or the profile r
+000092e0: 6573 7472 6963 7465 6420 746f 2074 6865  estricted to the
+000092f0: 2063 616e 6469 6461 7465 7320 696e 2060   candidates in `
+00009300: 6063 7572 725f 6361 6e64 7360 600a 2020  `curr_cands``.  
+00009310: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
+00009320: 756e 6374 696f 6e20 2866 756e 6374 696f  unction (functio
+00009330: 6e2c 206f 7074 696f 6e61 6c29 3a20 5468  n, optional): Th
+00009340: 6520 7374 7265 6e67 7468 2066 756e 6374  e strength funct
+00009350: 696f 6e20 746f 2062 6520 7573 6564 2074  ion to be used t
+00009360: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
+00009370: 7374 7265 6e67 7468 206f 6620 6120 7061  strength of a pa
+00009380: 7468 2e20 2020 5468 6520 6465 6661 756c  th.   The defaul
+00009390: 7420 6973 2074 6865 206d 6172 6769 6e20  t is the margin 
+000093a0: 6d65 7468 6f64 206f 6620 6060 6564 6174  method of ``edat
+000093b0: 6160 602e 2020 2054 6869 7320 6f6e 6c79  a``.   This only
+000093c0: 206d 6174 7465 7273 2077 6865 6e20 7468   matters when th
+000093d0: 6520 6261 6c6c 6f74 7320 6172 6520 6e6f  e ballots are no
+000093e0: 7420 6c69 6e65 6172 206f 7264 6572 732e  t linear orders.
+000093f0: 200a 0a20 2020 2052 6574 7572 6e73 3a20   ..    Returns: 
+00009400: 0a20 2020 2020 2020 2041 2073 6f72 7465  .        A sorte
+00009410: 6420 6c69 7374 206f 6620 6361 6e64 6964  d list of candid
+00009420: 6174 6573 2e20 0a0a 2020 2020 2e2e 2073  ates. ..    .. s
+00009430: 6565 616c 736f 3a3a 0a0a 2020 2020 2020  eealso::..      
+00009440: 2020 3a6d 6574 683a 6070 7265 665f 766f    :meth:`pref_vo
+00009450: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+00009460: 645f 6d65 7468 6f64 732e 7261 6e6b 6564  d_methods.ranked
+00009470: 5f70 6169 7273 602c 203a 6d65 7468 3a60  _pairs`, :meth:`
+00009480: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+00009490: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+000094a0: 2e72 616e 6b65 645f 7061 6972 735f 7769  .ranked_pairs_wi
+000094b0: 7468 5f74 6573 7460 0a0a 2020 2020 2e2e  th_test`..    ..
+000094c0: 2065 7865 635f 636f 6465 3a3a 0a0a 2020   exec_code::..  
+000094d0: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+000094e0: 766f 7469 6e67 2e70 726f 6669 6c65 7320  voting.profiles 
+000094f0: 696d 706f 7274 2050 726f 6669 6c65 0a20  import Profile. 
+00009500: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
+00009510: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+00009520: 6173 6564 5f6d 6574 686f 6473 2069 6d70  ased_methods imp
+00009530: 6f72 7420 7261 6e6b 6564 5f70 6169 7273  ort ranked_pairs
+00009540: 5f74 622c 2072 616e 6b65 645f 7061 6972  _tb, ranked_pair
+00009550: 735f 7a74 0a0a 2020 2020 2020 2020 7072  s_zt..        pr
+00009560: 6f66 203d 2050 726f 6669 6c65 285b 5b32  of = Profile([[2
+00009570: 2c20 332c 2031 2c20 305d 2c20 5b30 2c20  , 3, 1, 0], [0, 
+00009580: 332c 2031 2c20 325d 2c20 5b31 2c20 332c  3, 1, 2], [1, 3,
+00009590: 2032 2c20 305d 2c20 5b32 2c20 312c 2033   2, 0], [2, 1, 3
+000095a0: 2c20 305d 5d2c 205b 312c 2031 2c20 312c  , 0]], [1, 1, 1,
+000095b0: 2031 5d29 0a0a 2020 2020 2020 2020 7072   1])..        pr
+000095c0: 6f66 2e64 6973 706c 6179 2829 0a0a 2020  of.display()..  
+000095d0: 2020 2020 2020 7261 6e6b 6564 5f70 6169        ranked_pai
+000095e0: 7273 5f74 622e 6469 7370 6c61 7928 7072  rs_tb.display(pr
+000095f0: 6f66 290a 2020 2020 2020 2020 7261 6e6b  of).        rank
+00009600: 6564 5f70 6169 7273 5f74 622e 6469 7370  ed_pairs_tb.disp
+00009610: 6c61 7928 7072 6f66 2c20 7469 655f 6272  lay(prof, tie_br
+00009620: 6561 6b65 7220 3d20 5b33 2c20 322c 2031  eaker = [3, 2, 1
+00009630: 2c20 305d 290a 2020 2020 2020 2020 7261  , 0]).        ra
+00009640: 6e6b 6564 5f70 6169 7273 5f7a 742e 6469  nked_pairs_zt.di
+00009650: 7370 6c61 7928 7072 6f66 290a 0a20 2020  splay(prof)..   
+00009660: 2022 2222 0a0a 2020 2020 6361 6e64 6964   """..    candid
+00009670: 6174 6573 203d 2065 6461 7461 2e63 616e  ates = edata.can
+00009680: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
+00009690: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
+000096a0: 7365 2063 7572 725f 6361 6e64 7320 2020  se curr_cands   
+000096b0: 200a 2020 2020 6369 6478 5f74 6f5f 6361   .    cidx_to_ca
+000096c0: 6e64 203d 207b 6369 6478 3a20 6320 666f  nd = {cidx: c fo
+000096d0: 7220 6369 6478 2c20 6320 696e 2065 6e75  r cidx, c in enu
+000096e0: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
+000096f0: 7329 7d20 200a 2020 2020 6361 6e64 5f74  s)}  .    cand_t
+00009700: 6f5f 6369 6478 203d 207b 633a 2063 6964  o_cidx = {c: cid
+00009710: 7820 666f 7220 6369 6478 2c20 6320 696e  x for cidx, c in
+00009720: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
+00009730: 6461 7465 7329 7d20 200a 0a20 2020 2073  dates)}  ..    s
+00009740: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00009750: 203d 2065 6461 7461 2e6d 6172 6769 6e20   = edata.margin 
+00009760: 6966 2073 7472 656e 6774 685f 6675 6e63  if strength_func
+00009770: 7469 6f6e 2069 7320 4e6f 6e65 2065 6c73  tion is None els
+00009780: 6520 7374 7265 6e67 7468 5f66 756e 6374  e strength_funct
+00009790: 696f 6e0a 2020 2020 0a20 2020 2074 625f  ion.    .    tb_
+000097a0: 7261 6e6b 696e 6720 3d20 7469 655f 6272  ranking = tie_br
+000097b0: 6561 6b65 7220 6966 2074 6965 5f62 7265  eaker if tie_bre
+000097c0: 616b 6572 2069 7320 6e6f 7420 4e6f 6e65  aker is not None
+000097d0: 2065 6c73 6520 736f 7274 6564 286c 6973   else sorted(lis
+000097e0: 7428 6361 6e64 6964 6174 6573 2929 0a0a  t(candidates))..
+000097f0: 2020 2020 6377 203d 2065 6461 7461 2e63      cw = edata.c
+00009800: 6f6e 646f 7263 6574 5f77 696e 6e65 7228  ondorcet_winner(
+00009810: 6375 7272 5f63 616e 6473 3d63 7572 725f  curr_cands=curr_
+00009820: 6361 6e64 7329 0a20 2020 2023 2052 616e  cands).    # Ran
+00009830: 6b65 6420 5061 6972 7320 6973 2043 6f6e  ked Pairs is Con
+00009840: 646f 7263 6574 2063 6f6e 7369 7374 656e  dorcet consisten
+00009850: 742c 2073 6f20 7369 6d70 6c79 2072 6574  t, so simply ret
+00009860: 7572 6e20 7468 6520 436f 6e64 6f72 6365  urn the Condorce
+00009870: 7420 7769 6e6e 6572 2069 6620 6578 6973  t winner if exis
+00009880: 7473 0a20 2020 2069 6620 6377 2069 7320  ts.    if cw is 
+00009890: 6e6f 7420 4e6f 6e65 3a20 0a20 2020 2020  not None: .     
+000098a0: 2020 2077 696e 6e65 7273 203d 205b 6377     winners = [cw
+000098b0: 5d0a 2020 2020 656c 7365 3a0a 2020 2020  ].    else:.    
+000098c0: 2020 2020 775f 6564 6765 7320 3d20 5b28      w_edges = [(
+000098d0: 6331 2c20 6332 2c20 7374 7265 6e67 7468  c1, c2, strength
+000098e0: 5f66 756e 6374 696f 6e28 6331 2c20 6332  _function(c1, c2
+000098f0: 2929 2066 6f72 2063 3120 696e 2063 616e  )) for c1 in can
+00009900: 6469 6461 7465 7320 666f 7220 6332 2069  didates for c2 i
+00009910: 6e20 6361 6e64 6964 6174 6573 200a 2020  n candidates .  
+00009920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009930: 2069 6620 6331 2021 3d20 6332 2061 6e64   if c1 != c2 and
+00009940: 2028 6564 6174 612e 6d61 6a6f 7269 7479   (edata.majority
+00009950: 5f70 7265 6665 7273 2863 312c 2063 3229  _prefers(c1, c2)
+00009960: 206f 7220 6564 6174 612e 6973 5f74 6965   or edata.is_tie
+00009970: 6428 6331 2c20 6332 2929 5d0a 2020 2020  d(c1, c2))].    
+00009980: 2020 2020 7769 6e6e 6572 7320 3d20 6c69      winners = li
+00009990: 7374 2829 2020 2020 2020 2020 2020 2020  st()            
+000099a0: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
+000099b0: 6873 203d 2073 6f72 7465 6428 6c69 7374  hs = sorted(list
+000099c0: 2873 6574 285b 655b 325d 2066 6f72 2065  (set([e[2] for e
+000099d0: 2069 6e20 775f 6564 6765 735d 2929 2c20   in w_edges])), 
+000099e0: 7265 7665 7273 653d 5472 7565 290a 2020  reverse=True).  
+000099f0: 2020 2020 2020 0a20 2020 2020 2020 2072        .        r
+00009a00: 705f 6465 6665 6174 203d 2053 504f 286c  p_defeat = SPO(l
+00009a10: 656e 2863 616e 6469 6461 7465 7329 290a  en(candidates)).
+00009a20: 0a20 2020 2020 2020 2066 6f72 2073 2069  .        for s i
+00009a30: 6e20 7374 7265 6e67 7468 733a 200a 2020  n strengths: .  
+00009a40: 2020 2020 2020 2020 2020 6564 6765 7320            edges 
+00009a50: 3d20 5b65 2066 6f72 2065 2069 6e20 775f  = [e for e in w_
+00009a60: 6564 6765 7320 6966 2065 5b32 5d20 3d3d  edges if e[2] ==
+00009a70: 2073 5d0a 2020 2020 2020 2020 2020 2020   s].            
+00009a80: 0a20 2020 2020 2020 2020 2020 2023 2062  .            # b
+00009a90: 7265 616b 2074 6965 7320 7573 696e 6720  reak ties using 
+00009aa0: 7468 6520 6c65 7869 636f 6772 6170 6869  the lexicographi
+00009ab0: 6320 6f72 6465 7269 6e67 206f 6e20 7475  c ordering on tu
+00009ac0: 706c 6573 2067 6976 656e 2074 625f 7261  ples given tb_ra
+00009ad0: 6e6b 696e 670a 2020 2020 2020 2020 2020  nking.          
+00009ae0: 2020 736f 7274 6564 5f65 6467 6573 203d    sorted_edges =
+00009af0: 2073 6f72 7465 6428 6564 6765 732c 206b   sorted(edges, k
+00009b00: 6579 203d 206c 616d 6264 6120 653a 2028  ey = lambda e: (
+00009b10: 7462 5f72 616e 6b69 6e67 2e69 6e64 6578  tb_ranking.index
+00009b20: 2865 5b30 5d29 2c20 7462 5f72 616e 6b69  (e[0]), tb_ranki
+00009b30: 6e67 2e69 6e64 6578 2865 5b31 5d29 292c  ng.index(e[1])),
+00009b40: 2072 6576 6572 7365 3d46 616c 7365 290a   reverse=False).
+00009b50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00009b60: 6530 2c65 312c 7320 696e 2065 6467 6573  e0,e1,s in edges
+00009b70: 3a20 0a20 2020 2020 2020 2020 2020 2020  : .             
+00009b80: 2020 2069 6620 6e6f 7420 7270 5f64 6566     if not rp_def
+00009b90: 6561 742e 505b 6361 6e64 5f74 6f5f 6369  eat.P[cand_to_ci
+00009ba0: 6478 5b65 315d 5d5b 6361 6e64 5f74 6f5f  dx[e1]][cand_to_
+00009bb0: 6369 6478 5b65 305d 5d3a 0a20 2020 2020  cidx[e0]]:.     
+00009bc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00009bd0: 705f 6465 6665 6174 2e61 6464 2863 616e  p_defeat.add(can
+00009be0: 645f 746f 5f63 6964 785b 6530 5d2c 6361  d_to_cidx[e0],ca
+00009bf0: 6e64 5f74 6f5f 6369 6478 5b65 315d 290a  nd_to_cidx[e1]).
+00009c00: 2020 2020 2020 2020 2020 2020 7769 6e6e              winn
+00009c10: 6572 732e 6170 7065 6e64 2863 6964 785f  ers.append(cidx_
+00009c20: 746f 5f63 616e 645b 7270 5f64 6566 6561  to_cand[rp_defea
+00009c30: 742e 696e 6974 6961 6c5f 656c 656d 656e  t.initial_elemen
+00009c40: 7473 2829 5b30 5d5d 290a 0a20 2020 2072  ts()[0]])..    r
+00009c50: 6574 7572 6e20 736f 7274 6564 286c 6973  eturn sorted(lis
+00009c60: 7428 7365 7428 7769 6e6e 6572 7329 2929  t(set(winners)))
+00009c70: 0a0a 0a40 766d 286e 616d 653d 2252 616e  ...@vm(name="Ran
+00009c80: 6b65 6420 5061 6972 7320 5a54 2229 0a64  ked Pairs ZT").d
+00009c90: 6566 2072 616e 6b65 645f 7061 6972 735f  ef ranked_pairs_
+00009ca0: 7a74 280a 2020 2020 7072 6f66 696c 652c  zt(.    profile,
+00009cb0: 200a 2020 2020 6375 7272 5f63 616e 6473   .    curr_cands
+00009cc0: 203d 204e 6f6e 652c 200a 2020 2020 7374   = None, .    st
+00009cd0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+00009ce0: 3d20 4e6f 6e65 293a 2020 200a 2020 2020  = None):   .    
+00009cf0: 2222 2252 616e 6b65 6420 7061 6972 7320  """Ranked pairs 
+00009d00: 7768 6572 6520 6120 6669 7865 6420 766f  where a fixed vo
+00009d10: 7465 7220 6272 6561 6b73 2061 6e79 2074  ter breaks any t
+00009d20: 6965 7320 696e 2074 6865 206d 6172 6769  ies in the margi
+00009d30: 6e73 2e20 2049 7420 6973 2061 6c77 6179  ns.  It is alway
+00009d40: 7320 7468 6520 766f 7465 7220 696e 2070  s the voter in p
+00009d50: 6f73 6974 696f 6e20 3020 7468 6174 2062  osition 0 that b
+00009d60: 7265 616b 7320 7468 6520 7469 6573 2e20  reaks the ties. 
+00009d70: 2053 696e 6365 2076 6f74 6572 7320 6861   Since voters ha
+00009d80: 7665 2073 7472 6963 7420 7072 6566 6572  ve strict prefer
+00009d90: 656e 6365 732c 2074 6869 7320 6d65 7468  ences, this meth
+00009da0: 6f64 2069 7320 7265 736f 6c75 7465 2e20  od is resolute. 
+00009db0: 2054 6869 7320 6973 206b 6e6f 776e 2061   This is known a
+00009dc0: 7320 5261 6e6b 6564 2050 6169 7273 205a  s Ranked Pairs Z
+00009dd0: 542c 2066 6f72 205a 6176 6973 7420 5469  T, for Zavist Ti
+00009de0: 6465 6d61 6e2e 0a0a 2020 2020 4172 6773  deman...    Args
+00009df0: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
+00009e00: 2850 726f 6669 6c65 293a 2041 2070 726f  (Profile): A pro
+00009e10: 6669 6c65 206f 6620 6c69 6e65 6172 206f  file of linear o
+00009e20: 7264 6572 730a 2020 2020 2020 2020 6375  rders.        cu
+00009e30: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
+00009e40: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
+00009e50: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
+00009e60: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
+00009e70: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
+00009e80: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
+00009e90: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
+00009ea0: 6375 7272 5f63 616e 6473 6060 0a0a 2020  curr_cands``..  
+00009eb0: 2020 5265 7475 726e 733a 200a 2020 2020    Returns: .    
+00009ec0: 2020 2020 4120 736f 7274 6564 206c 6973      A sorted lis
+00009ed0: 7420 6f66 2063 616e 6469 6461 7465 732e  t of candidates.
+00009ee0: 200a 0a20 2020 202e 2e20 7365 6561 6c73   ..    .. seeals
+00009ef0: 6f3a 3a0a 0a20 2020 2020 2020 203a 6d65  o::..        :me
+00009f00: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
+00009f10: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+00009f20: 686f 6473 2e72 616e 6b65 645f 7061 6972  hods.ranked_pair
+00009f30: 7360 2c20 3a6d 6574 683a 6070 7265 665f  s`, :meth:`pref_
+00009f40: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+00009f50: 7365 645f 6d65 7468 6f64 732e 7261 6e6b  sed_methods.rank
+00009f60: 6564 5f70 6169 7273 5f77 6974 685f 7465  ed_pairs_with_te
+00009f70: 7374 600a 0a20 2020 202e 2e20 6578 6563  st`..    .. exec
+00009f80: 5f63 6f64 653a 3a0a 0a20 2020 2020 2020  _code::..       
+00009f90: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
+00009fa0: 672e 7072 6f66 696c 6573 2069 6d70 6f72  g.profiles impor
+00009fb0: 7420 5072 6f66 696c 650a 2020 2020 2020  t Profile.      
+00009fc0: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
+00009fd0: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
+00009fe0: 6d65 7468 6f64 7320 696d 706f 7274 2072  methods import r
+00009ff0: 616e 6b65 645f 7061 6972 735f 7462 2c20  anked_pairs_tb, 
+0000a000: 7261 6e6b 6564 5f70 6169 7273 5f7a 740a  ranked_pairs_zt.
+0000a010: 0a20 2020 2020 2020 2070 726f 6620 3d20  .        prof = 
+0000a020: 5072 6f66 696c 6528 5b5b 322c 2033 2c20  Profile([[2, 3, 
+0000a030: 312c 2030 5d2c 205b 302c 2033 2c20 312c  1, 0], [0, 3, 1,
+0000a040: 2032 5d2c 205b 312c 2033 2c20 322c 2030   2], [1, 3, 2, 0
+0000a050: 5d2c 205b 322c 2031 2c20 332c 2030 5d5d  ], [2, 1, 3, 0]]
+0000a060: 2c20 5b31 2c20 312c 2031 2c20 315d 290a  , [1, 1, 1, 1]).
+0000a070: 0a20 2020 2020 2020 2070 726f 662e 6469  .        prof.di
+0000a080: 7370 6c61 7928 290a 0a20 2020 2020 2020  splay()..       
+0000a090: 2072 616e 6b65 645f 7061 6972 735f 7462   ranked_pairs_tb
+0000a0a0: 2e64 6973 706c 6179 2870 726f 6629 0a20  .display(prof). 
+0000a0b0: 2020 2020 2020 2072 616e 6b65 645f 7061         ranked_pa
+0000a0c0: 6972 735f 7462 2e64 6973 706c 6179 2870  irs_tb.display(p
+0000a0d0: 726f 662c 2074 6965 5f62 7265 616b 6572  rof, tie_breaker
+0000a0e0: 203d 205b 332c 2032 2c20 312c 2030 5d29   = [3, 2, 1, 0])
+0000a0f0: 0a20 2020 2020 2020 2072 616e 6b65 645f  .        ranked_
+0000a100: 7061 6972 735f 7a74 2e64 6973 706c 6179  pairs_zt.display
+0000a110: 2870 726f 6629 0a0a 2020 2020 0a20 2020  (prof)..    .   
+0000a120: 2022 2222 0a20 2020 2063 616e 6469 6461   """.    candida
+0000a130: 7465 7320 3d20 7072 6f66 696c 652e 6361  tes = profile.ca
+0000a140: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
+0000a150: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
+0000a160: 6c73 6520 6375 7272 5f63 616e 6473 2020  lse curr_cands  
+0000a170: 2020 0a20 2020 200a 2020 2020 2320 7468    .    .    # th
+0000a180: 6520 7469 652d 6272 6561 6b65 7220 6973  e tie-breaker is
+0000a190: 2061 6c77 6179 7320 7468 6520 6669 7273   always the firs
+0000a1a0: 7420 766f 7465 722e 200a 2020 2020 7462  t voter. .    tb
+0000a1b0: 5f72 616e 6b69 6e67 203d 2074 7570 6c65  _ranking = tuple
+0000a1c0: 285b 6320 666f 7220 6320 696e 206c 6973  ([c for c in lis
+0000a1d0: 7428 7072 6f66 696c 652e 5f72 616e 6b69  t(profile._ranki
+0000a1e0: 6e67 735b 305d 2920 6966 2063 2069 6e20  ngs[0]) if c in 
+0000a1f0: 6361 6e64 6964 6174 6573 5d29 0a20 2020  candidates]).   
+0000a200: 200a 2020 2020 7265 7475 726e 2072 616e   .    return ran
+0000a210: 6b65 645f 7061 6972 735f 7462 2870 726f  ked_pairs_tb(pro
+0000a220: 6669 6c65 2c20 6375 7272 5f63 616e 6473  file, curr_cands
+0000a230: 203d 2063 7572 725f 6361 6e64 732c 2074   = curr_cands, t
+0000a240: 6965 5f62 7265 616b 6572 203d 2074 625f  ie_breaker = tb_
+0000a250: 7261 6e6b 696e 672c 2073 7472 656e 6774  ranking, strengt
+0000a260: 685f 6675 6e63 7469 6f6e 203d 2073 7472  h_function = str
+0000a270: 656e 6774 685f 6675 6e63 7469 6f6e 290a  ength_function).
+0000a280: 0a0a 4076 6d28 6e61 6d65 3d22 5269 7665  ..@vm(name="Rive
+0000a290: 7222 290a 6465 6620 7269 7665 7228 6564  r").def river(ed
+0000a2a0: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
+0000a2b0: 3d20 4e6f 6e65 2c20 7374 7265 6e67 7468  = None, strength
+0000a2c0: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
+0000a2d0: 293a 2020 200a 2020 2020 2222 220a 2020  ):   .    """.  
+0000a2e0: 2020 4f72 6465 7220 7468 6520 6564 6765    Order the edge
+0000a2f0: 7320 696e 2074 6865 2077 6561 6b20 6d61  s in the weak ma
+0000a300: 7267 696e 2067 7261 7068 2066 726f 6d20  rgin graph from 
+0000a310: 6c61 7267 6573 7420 746f 2073 6d61 6c6c  largest to small
+0000a320: 6573 7420 616e 6420 6c6f 636b 2074 6865  est and lock the
+0000a330: 6d20 696e 2069 6e20 7468 6174 206f 7264  m in in that ord
+0000a340: 6572 2c20 736b 6970 7069 6e67 2065 6467  er, skipping edg
+0000a350: 6573 2074 6861 7420 6372 6561 7465 2061  es that create a
+0000a360: 2063 7963 6c65 202a 616e 6420 6564 6765   cycle *and edge
+0000a370: 7320 696e 2077 6869 6368 2074 6865 7265  s in which there
+0000a380: 2069 7320 616c 7265 6164 7920 616e 2065   is already an e
+0000a390: 6467 6520 706f 696e 7469 6e67 2074 6f20  dge pointing to 
+0000a3a0: 7468 6520 7461 7267 6574 2a2e 2020 4272  the target*.  Br
+0000a3b0: 6561 6b20 7469 6573 2075 7369 6e67 2061  eak ties using a
+0000a3c0: 2074 6965 2d62 7265 616b 696e 6720 206c   tie-breaking  l
+0000a3d0: 696e 6561 7220 6f72 6465 7269 6e67 206f  inear ordering o
+0000a3e0: 7665 7220 7468 6520 6564 6765 732e 2020  ver the edges.  
+0000a3f0: 4120 6361 6e64 6964 6174 6520 6973 2061  A candidate is a
+0000a400: 2052 6976 6572 2077 696e 6e65 7220 6966   River winner if
+0000a410: 2069 7420 7769 6e73 2061 6363 6f72 6469   it wins accordi
+0000a420: 6e67 2074 6f20 736f 6d65 2074 6965 2d62  ng to some tie-b
+0000a430: 7265 616b 696e 6720 7275 6c65 2e20 5365  reaking rule. Se
+0000a440: 6520 6874 7470 733a 2f2f 656c 6563 746f  e https://electo
+0000a450: 7769 6b69 2e6f 7267 2f77 696b 692f 5269  wiki.org/wiki/Ri
+0000a460: 7665 722e 0a0a 2020 2020 4172 6773 3a0a  ver...    Args:.
+0000a470: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
+0000a480: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
+0000a490: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
+0000a4a0: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
+0000a4b0: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
+0000a4c0: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
+0000a4d0: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
+0000a4e0: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
+0000a4f0: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
+0000a500: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
+0000a510: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
+0000a520: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
+0000a530: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
+0000a540: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
+0000a550: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
+0000a560: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
+0000a570: 6e63 7469 6f6e 2028 6675 6e63 7469 6f6e  nction (function
+0000a580: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+0000a590: 2073 7472 656e 6774 6820 6675 6e63 7469   strength functi
+0000a5a0: 6f6e 2074 6f20 6265 2075 7365 6420 746f  on to be used to
+0000a5b0: 2063 616c 6375 6c61 7465 2074 6865 2073   calculate the s
+0000a5c0: 7472 656e 6774 6820 6f66 2061 2070 6174  trength of a pat
+0000a5d0: 682e 2020 2054 6865 2064 6566 6175 6c74  h.   The default
+0000a5e0: 2069 7320 7468 6520 6d61 7267 696e 206d   is the margin m
+0000a5f0: 6574 686f 6420 6f66 2060 6065 6461 7461  ethod of ``edata
+0000a600: 6060 2e20 2020 5468 6973 206f 6e6c 7920  ``.   This only 
+0000a610: 6d61 7474 6572 7320 7768 656e 2074 6865  matters when the
+0000a620: 2062 616c 6c6f 7473 2061 7265 206e 6f74   ballots are not
+0000a630: 206c 696e 6561 7220 6f72 6465 7273 2e20   linear orders. 
+0000a640: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
+0000a650: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
+0000a660: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
+0000a670: 7465 732e 200a 0a20 2020 203a 4578 616d  tes. ..    :Exam
+0000a680: 706c 653a 200a 0a20 2020 202e 2e20 6578  ple: ..    .. ex
+0000a690: 6563 5f63 6f64 653a 3a20 0a0a 2020 2020  ec_code:: ..    
+0000a6a0: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
+0000a6b0: 7469 6e67 2e77 6569 6768 7465 645f 6d61  ting.weighted_ma
+0000a6c0: 6a6f 7269 7479 5f67 7261 7068 7320 696d  jority_graphs im
+0000a6d0: 706f 7274 204d 6172 6769 6e47 7261 7068  port MarginGraph
+0000a6e0: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
+0000a6f0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+0000a700: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
+0000a710: 6d70 6f72 7420 7269 7665 722c 2072 616e  mport river, ran
+0000a720: 6b65 645f 7061 6972 730a 2020 2020 2020  ked_pairs.      
+0000a730: 2020 0a20 2020 2020 2020 206d 6720 3d20    .        mg = 
+0000a740: 4d61 7267 696e 4772 6170 6828 5b30 2c20  MarginGraph([0, 
+0000a750: 312c 2032 2c20 335d 2c20 5b28 302c 2032  1, 2, 3], [(0, 2
+0000a760: 2c20 3229 2c20 2830 2c20 332c 2038 292c  , 2), (0, 3, 8),
+0000a770: 2028 312c 2030 2c20 3132 292c 2028 322c   (1, 0, 12), (2,
+0000a780: 2033 2c20 3132 292c 2028 332c 2031 2c20   3, 12), (3, 1, 
+0000a790: 3629 5d29 0a0a 2020 2020 2020 2020 7261  6)])..        ra
+0000a7a0: 6e6b 6564 5f70 6169 7273 2e64 6973 706c  nked_pairs.displ
+0000a7b0: 6179 286d 6729 0a20 2020 2020 2020 2072  ay(mg).        r
+0000a7c0: 6976 6572 2e64 6973 706c 6179 286d 6729  iver.display(mg)
+0000a7d0: 0a0a 2020 2020 2222 220a 2020 2020 6361  ..    """.    ca
+0000a7e0: 6e64 6964 6174 6573 203d 2065 6461 7461  ndidates = edata
+0000a7f0: 2e63 616e 6469 6461 7465 7320 6966 2063  .candidates if c
+0000a800: 7572 725f 6361 6e64 7320 6973 204e 6f6e  urr_cands is Non
+0000a810: 6520 656c 7365 2063 7572 725f 6361 6e64  e else curr_cand
+0000a820: 7320 2020 200a 2020 2020 6369 6478 5f74  s    .    cidx_t
+0000a830: 6f5f 6361 6e64 203d 207b 6369 6478 3a20  o_cand = {cidx: 
+0000a840: 6320 666f 7220 6369 6478 2c20 6320 696e  c for cidx, c in
+0000a850: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
+0000a860: 6461 7465 7329 7d20 200a 2020 2020 6361  dates)}  .    ca
+0000a870: 6e64 5f74 6f5f 6369 6478 203d 207b 633a  nd_to_cidx = {c:
+0000a880: 2063 6964 7820 666f 7220 6369 6478 2c20   cidx for cidx, 
+0000a890: 6320 696e 2065 6e75 6d65 7261 7465 2863  c in enumerate(c
+0000a8a0: 616e 6469 6461 7465 7329 7d20 200a 0a20  andidates)}  .. 
+0000a8b0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+0000a8c0: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
+0000a8d0: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
+0000a8e0: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
+0000a8f0: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
+0000a900: 756e 6374 696f 6e20 2020 200a 0a20 2020  unction    ..   
+0000a910: 2063 7720 3d20 6564 6174 612e 636f 6e64   cw = edata.cond
+0000a920: 6f72 6365 745f 7769 6e6e 6572 2863 7572  orcet_winner(cur
+0000a930: 725f 6361 6e64 733d 6375 7272 5f63 616e  r_cands=curr_can
+0000a940: 6473 290a 2020 2020 2320 5261 6e6b 6564  ds).    # Ranked
+0000a950: 2050 6169 7273 2069 7320 436f 6e64 6f72   Pairs is Condor
+0000a960: 6365 7420 636f 6e73 6973 7465 6e74 2c20  cet consistent, 
+0000a970: 736f 2073 696d 706c 7920 7265 7475 726e  so simply return
+0000a980: 2074 6865 2043 6f6e 646f 7263 6574 2077   the Condorcet w
+0000a990: 696e 6e65 7220 6966 2065 7869 7374 730a  inner if exists.
+0000a9a0: 2020 2020 6966 2063 7720 6973 206e 6f74      if cw is not
+0000a9b0: 204e 6f6e 653a 200a 2020 2020 2020 2020   None: .        
+0000a9c0: 7769 6e6e 6572 7320 3d20 5b63 775d 0a20  winners = [cw]. 
+0000a9d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000a9e0: 2077 5f65 6467 6573 203d 205b 2863 312c   w_edges = [(c1,
+0000a9f0: 2063 322c 2073 7472 656e 6774 685f 6675   c2, strength_fu
+0000aa00: 6e63 7469 6f6e 2863 312c 2063 3229 2920  nction(c1, c2)) 
+0000aa10: 666f 7220 6331 2069 6e20 6361 6e64 6964  for c1 in candid
+0000aa20: 6174 6573 2066 6f72 2063 3220 696e 2063  ates for c2 in c
+0000aa30: 616e 6469 6461 7465 7320 0a20 2020 2020  andidates .     
+0000aa40: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000aa50: 2063 3120 213d 2063 3220 616e 6420 2865   c1 != c2 and (e
+0000aa60: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
+0000aa70: 6566 6572 7328 6331 2c20 6332 2920 6f72  efers(c1, c2) or
+0000aa80: 2065 6461 7461 2e69 735f 7469 6564 2863   edata.is_tied(c
+0000aa90: 312c 2063 3229 295d 0a20 2020 2020 2020  1, c2))].       
+0000aaa0: 2077 696e 6e65 7273 203d 206c 6973 7428   winners = list(
+0000aab0: 2920 2020 2020 2020 2020 2020 200a 2020  )            .  
+0000aac0: 2020 2020 2020 7374 7265 6e67 7468 7320        strengths 
+0000aad0: 3d20 736f 7274 6564 286c 6973 7428 7365  = sorted(list(se
+0000aae0: 7428 5b65 5b32 5d20 666f 7220 6520 696e  t([e[2] for e in
+0000aaf0: 2077 5f65 6467 6573 5d29 292c 2072 6576   w_edges])), rev
+0000ab00: 6572 7365 3d54 7275 6529 0a20 2020 2020  erse=True).     
+0000ab10: 2020 2073 6f72 7465 645f 6564 6765 7320     sorted_edges 
+0000ab20: 3d20 5b5b 6520 666f 7220 6520 696e 2077  = [[e for e in w
+0000ab30: 5f65 6467 6573 2069 6620 655b 325d 203d  _edges if e[2] =
+0000ab40: 3d20 735d 2066 6f72 2073 2069 6e20 7374  = s] for s in st
+0000ab50: 7265 6e67 7468 735d 0a20 2020 2020 2020  rengths].       
+0000ab60: 2074 6273 203d 2070 726f 6475 6374 282a   tbs = product(*
+0000ab70: 5b70 6572 6d75 7461 7469 6f6e 7328 6564  [permutations(ed
+0000ab80: 6765 7329 2066 6f72 2065 6467 6573 2069  ges) for edges i
+0000ab90: 6e20 736f 7274 6564 5f65 6467 6573 5d29  n sorted_edges])
+0000aba0: 0a20 2020 2020 2020 2066 6f72 2074 6220  .        for tb 
+0000abb0: 696e 2074 6273 3a0a 2020 2020 2020 2020  in tbs:.        
+0000abc0: 2020 2020 6564 6765 7320 3d20 666c 6174      edges = flat
+0000abd0: 7465 6e28 7462 290a 2020 2020 2020 2020  ten(tb).        
+0000abe0: 2020 2020 7276 5f64 6566 6561 7420 3d20      rv_defeat = 
+0000abf0: 5350 4f28 6c65 6e28 6361 6e64 6964 6174  SPO(len(candidat
+0000ac00: 6573 2929 0a20 2020 2020 2020 2020 2020  es)).           
+0000ac10: 2066 6f72 2065 302c 6531 2c73 2069 6e20   for e0,e1,s in 
+0000ac20: 6564 6765 733a 200a 2020 2020 2020 2020  edges: .        
+0000ac30: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+0000ac40: 765f 6465 6665 6174 2e50 5b63 616e 645f  v_defeat.P[cand_
+0000ac50: 746f 5f63 6964 785b 6531 5d5d 5b63 616e  to_cidx[e1]][can
+0000ac60: 645f 746f 5f63 6964 785b 6530 5d5d 2061  d_to_cidx[e0]] a
+0000ac70: 6e64 206c 656e 2872 765f 6465 6665 6174  nd len(rv_defeat
+0000ac80: 2e70 7265 6473 5b63 616e 645f 746f 5f63  .preds[cand_to_c
+0000ac90: 6964 785b 6531 5d5d 2920 3d3d 2030 3a0a  idx[e1]]) == 0:.
+0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acb0: 2020 2020 7276 5f64 6566 6561 742e 6164      rv_defeat.ad
+0000acc0: 6428 6361 6e64 5f74 6f5f 6369 6478 5b65  d(cand_to_cidx[e
+0000acd0: 305d 2c63 616e 645f 746f 5f63 6964 785b  0],cand_to_cidx[
+0000ace0: 6531 5d29 0a20 2020 2020 2020 2020 2020  e1]).           
+0000acf0: 2077 696e 6e65 7273 2e61 7070 656e 6428   winners.append(
+0000ad00: 6369 6478 5f74 6f5f 6361 6e64 5b72 765f  cidx_to_cand[rv_
+0000ad10: 6465 6665 6174 2e69 6e69 7469 616c 5f65  defeat.initial_e
+0000ad20: 6c65 6d65 6e74 7328 295b 305d 5d29 0a0a  lements()[0]])..
+0000ad30: 2020 2020 7265 7475 726e 2073 6f72 7465      return sorte
+0000ad40: 6428 6c69 7374 2873 6574 2877 696e 6e65  d(list(set(winne
+0000ad50: 7273 2929 290a 0a64 6566 2072 6976 6572  rs)))..def river
+0000ad60: 5f64 6566 6561 7473 2865 6461 7461 2c20  _defeats(edata, 
+0000ad70: 6375 7272 5f63 616e 6473 203d 204e 6f6e  curr_cands = Non
+0000ad80: 652c 2073 7472 656e 6774 685f 6675 6e63  e, strength_func
+0000ad90: 7469 6f6e 203d 204e 6f6e 6529 3a0a 2020  tion = None):.  
+0000ada0: 2020 2222 220a 2020 2020 5265 7475 726e    """.    Return
+0000adb0: 7320 7468 6520 5269 7665 7220 6465 6665  s the River defe
+0000adc0: 6174 2072 656c 6174 696f 6e73 2070 726f  at relations pro
+0000add0: 6475 6365 6420 6279 2074 6865 2052 6976  duced by the Riv
+0000ade0: 6572 2061 6c67 6f72 6974 686d 2e0a 0a20  er algorithm... 
+0000adf0: 2020 202e 2e20 696d 706f 7274 616e 743a     .. important:
+0000ae00: 3a0a 2020 2020 2020 2020 556e 6c69 6b65  :.        Unlike
+0000ae10: 2074 6865 206f 7468 6572 2066 756e 6374   the other funct
+0000ae20: 696f 6e73 2074 6861 7420 7265 7475 726e  ions that return
+0000ae30: 2061 2073 696e 676c 6520 6465 6665 6174   a single defeat
+0000ae40: 2072 656c 6174 696f 6e2c 2074 6869 7320   relation, this 
+0000ae50: 7265 7475 726e 7320 6120 6c69 7374 206f  returns a list o
+0000ae60: 6620 6465 6665 6174 2072 656c 6174 696f  f defeat relatio
+0000ae70: 6e73 2e20 0a20 2020 2020 2020 200a 2020  ns. .        .  
+0000ae80: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000ae90: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
+0000aea0: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
+0000aeb0: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
+0000aec0: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
+0000aed0: 2074 6861 7420 6861 7320 6120 606d 6172   that has a `mar
+0000aee0: 6769 6e60 206d 6574 686f 642e 200a 2020  gin` method. .  
+0000aef0: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
+0000af00: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
+0000af10: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
+0000af20: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
+0000af30: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
+0000af40: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
+0000af50: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
+0000af60: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
+0000af70: 6473 6060 0a20 2020 2020 2020 2073 7472  ds``.        str
+0000af80: 656e 6774 685f 6675 6e63 7469 6f6e 2028  ength_function (
+0000af90: 6675 6e63 7469 6f6e 2c20 6f70 7469 6f6e  function, option
+0000afa0: 616c 293a 2054 6865 2073 7472 656e 6774  al): The strengt
+0000afb0: 6820 6675 6e63 7469 6f6e 2074 6f20 6265  h function to be
+0000afc0: 2075 7365 6420 746f 2063 616c 6375 6c61   used to calcula
+0000afd0: 7465 2074 6865 2073 7472 656e 6774 6820  te the strength 
+0000afe0: 6f66 2061 2070 6174 682e 2020 2054 6865  of a path.   The
+0000aff0: 2064 6566 6175 6c74 2069 7320 7468 6520   default is the 
+0000b000: 6d61 7267 696e 206d 6574 686f 6420 6f66  margin method of
+0000b010: 2060 6065 6461 7461 6060 2e20 2020 5468   ``edata``.   Th
+0000b020: 6973 206f 6e6c 7920 6d61 7474 6572 7320  is only matters 
+0000b030: 7768 656e 2074 6865 2062 616c 6c6f 7473  when the ballots
+0000b040: 2061 7265 206e 6f74 206c 696e 6561 7220   are not linear 
+0000b050: 6f72 6465 7273 2e20 0a0a 2020 2020 5265  orders. ..    Re
+0000b060: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
+0000b070: 4120 6e65 7477 6f72 6b78 2044 6947 7261  A networkx DiGra
+0000b080: 7068 2072 6570 7265 7365 6e74 696e 6720  ph representing 
+0000b090: 7468 6520 5269 7665 7220 6465 6665 6174  the River defeat
+0000b0a0: 2072 656c 6174 696f 6e2e 200a 2020 2020   relation. .    
+0000b0b0: 2222 220a 0a20 2020 2063 616e 6469 6461  """..    candida
+0000b0c0: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
+0000b0d0: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
+0000b0e0: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
+0000b0f0: 6520 6375 7272 5f63 616e 6473 2020 2020  e curr_cands    
+0000b100: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
+0000b110: 6e63 7469 6f6e 203d 2065 6461 7461 2e6d  nction = edata.m
+0000b120: 6172 6769 6e20 6966 2073 7472 656e 6774  argin if strengt
+0000b130: 685f 6675 6e63 7469 6f6e 2069 7320 4e6f  h_function is No
+0000b140: 6e65 2065 6c73 6520 7374 7265 6e67 7468  ne else strength
+0000b150: 5f66 756e 6374 696f 6e20 2020 200a 0a20  _function    .. 
+0000b160: 2020 2077 5f65 6467 6573 203d 205b 2863     w_edges = [(c
+0000b170: 312c 2063 322c 2073 7472 656e 6774 685f  1, c2, strength_
+0000b180: 6675 6e63 7469 6f6e 2863 312c 2063 3229  function(c1, c2)
+0000b190: 2920 666f 7220 6331 2069 6e20 6361 6e64  ) for c1 in cand
+0000b1a0: 6964 6174 6573 2066 6f72 2063 3220 696e  idates for c2 in
+0000b1b0: 2063 616e 6469 6461 7465 7320 6966 2063   candidates if c
+0000b1c0: 3120 213d 2063 3220 616e 6420 2865 6461  1 != c2 and (eda
+0000b1d0: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+0000b1e0: 6572 7328 6331 2c20 6332 2920 6f72 2065  ers(c1, c2) or e
+0000b1f0: 6461 7461 2e69 735f 7469 6564 2863 312c  data.is_tied(c1,
+0000b200: 2063 3229 295d 0a0a 2020 2020 7374 7265   c2))]..    stre
+0000b210: 6e67 7468 7320 3d20 736f 7274 6564 286c  ngths = sorted(l
+0000b220: 6973 7428 7365 7428 5b65 5b32 5d20 666f  ist(set([e[2] fo
+0000b230: 7220 6520 696e 2077 5f65 6467 6573 5d29  r e in w_edges])
+0000b240: 292c 2072 6576 6572 7365 3d54 7275 6529  ), reverse=True)
+0000b250: 0a20 2020 2073 6f72 7465 645f 6564 6765  .    sorted_edge
+0000b260: 7320 3d20 5b5b 6520 666f 7220 6520 696e  s = [[e for e in
+0000b270: 2077 5f65 6467 6573 2069 6620 655b 325d   w_edges if e[2]
+0000b280: 203d 3d20 735d 2066 6f72 2073 2069 6e20   == s] for s in 
+0000b290: 7374 7265 6e67 7468 735d 0a20 2020 2074  strengths].    t
+0000b2a0: 6273 203d 2070 726f 6475 6374 282a 5b70  bs = product(*[p
+0000b2b0: 6572 6d75 7461 7469 6f6e 7328 6564 6765  ermutations(edge
+0000b2c0: 7329 2066 6f72 2065 6467 6573 2069 6e20  s) for edges in 
+0000b2d0: 736f 7274 6564 5f65 6467 6573 5d29 0a0a  sorted_edges])..
+0000b2e0: 2020 2020 7269 7665 725f 6465 6665 6174      river_defeat
+0000b2f0: 7320 3d20 6c69 7374 2829 0a20 2020 2066  s = list().    f
+0000b300: 6f72 2074 6220 696e 2074 6273 3a0a 2020  or tb in tbs:.  
+0000b310: 2020 2020 2020 6564 6765 7320 3d20 666c        edges = fl
+0000b320: 6174 7465 6e28 7462 290a 2020 2020 2020  atten(tb).      
+0000b330: 2020 7269 7665 725f 6465 6665 6174 203d    river_defeat =
+0000b340: 206e 782e 4469 4772 6170 6828 2920 0a20   nx.DiGraph() . 
+0000b350: 2020 2020 2020 2066 6f72 2065 2069 6e20         for e in 
+0000b360: 6564 6765 733a 200a 2020 2020 2020 2020  edges: .        
+0000b370: 2020 2020 6966 2065 5b31 5d20 6e6f 7420      if e[1] not 
+0000b380: 696e 2072 6976 6572 5f64 6566 6561 742e  in river_defeat.
+0000b390: 6e6f 6465 7320 6f72 206c 656e 286c 6973  nodes or len(lis
+0000b3a0: 7428 7269 7665 725f 6465 6665 6174 2e69  t(river_defeat.i
+0000b3b0: 6e5f 6564 6765 7328 655b 315d 2929 2920  n_edges(e[1]))) 
+0000b3c0: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+0000b3d0: 2020 2020 2020 7269 7665 725f 6465 6665        river_defe
+0000b3e0: 6174 2e61 6464 5f65 6467 6528 655b 305d  at.add_edge(e[0]
+0000b3f0: 2c20 655b 315d 2c20 7765 6967 6874 3d65  , e[1], weight=e
+0000b400: 5b32 5d29 0a20 2020 2020 2020 2020 2020  [2]).           
+0000b410: 2020 2020 2069 6620 646f 6573 5f63 7265       if does_cre
+0000b420: 6174 655f 6379 636c 6528 7269 7665 725f  ate_cycle(river_
+0000b430: 6465 6665 6174 2c20 6529 3a0a 2020 2020  defeat, e):.    
+0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b450: 7269 7665 725f 6465 6665 6174 2e72 656d  river_defeat.rem
+0000b460: 6f76 655f 6564 6765 2865 5b30 5d2c 2065  ove_edge(e[0], e
+0000b470: 5b31 5d29 0a20 2020 2020 2020 2020 2020  [1]).           
+0000b480: 200a 2020 2020 2020 2020 7269 7665 725f   .        river_
+0000b490: 6465 6665 6174 732e 6170 7065 6e64 2872  defeats.append(r
+0000b4a0: 6976 6572 5f64 6566 6561 7429 0a0a 2020  iver_defeat)..  
+0000b4b0: 2020 7265 7475 726e 2072 6976 6572 5f64    return river_d
+0000b4c0: 6566 6561 7473 0a0a 4076 6d28 6e61 6d65  efeats..@vm(name
+0000b4d0: 3d22 5269 7665 7222 290a 6465 6620 7269  ="River").def ri
+0000b4e0: 7665 725f 7769 7468 5f74 6573 7428 6564  ver_with_test(ed
+0000b4f0: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
+0000b500: 3d20 4e6f 6e65 2c20 7374 7265 6e67 7468  = None, strength
+0000b510: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
+0000b520: 293a 2020 200a 2020 2020 2222 2246 696e  ):   .    """Fin
+0000b530: 6420 7468 6520 5269 7665 7220 7769 6e6e  d the River winn
+0000b540: 6572 7320 7769 7468 2061 2074 6573 7420  ers with a test 
+0000b550: 746f 2064 6574 6572 6d69 6e65 6420 6966  to determined if
+0000b560: 2069 7420 7769 6c6c 2074 616b 6520 746f   it will take to
+0000b570: 6f20 6c6f 6e67 2074 6f20 636f 6d70 7574  o long to comput
+0000b580: 6520 7468 6520 5269 7665 7220 7769 6e6e  e the River winn
+0000b590: 6572 732e 2049 6620 7468 6520 6361 6c63  ers. If the calc
+0000b5a0: 756c 6174 696f 6e20 6f66 2074 6865 2077  ulation of the w
+0000b5b0: 696e 6e65 7273 2077 696c 6c20 7461 6b65  inners will take
+0000b5c0: 2074 6f6f 206c 6f6e 672c 2072 6574 7572   too long, retur
+0000b5d0: 6e20 4e6f 6e65 2e20 0a20 2020 2020 2020  n None. .       
+0000b5e0: 200a 2020 2020 2e2e 2069 6d70 6f72 7461   .    .. importa
+0000b5f0: 6e74 3a3a 0a20 2020 2020 2020 2054 6869  nt::.        Thi
+0000b600: 7320 766f 7469 6e67 206d 6574 686f 6420  s voting method 
+0000b610: 7468 6174 206d 6967 6874 2072 6574 7572  that might retur
+0000b620: 6e20 4e6f 6e65 2072 6174 6865 7220 7468  n None rather th
+0000b630: 616e 2061 206c 6973 7420 6f66 2063 616e  an a list of can
+0000b640: 6469 6461 7465 732e 2020 0a0a 2020 2020  didates.  ..    
+0000b650: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
+0000b660: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
+0000b670: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
+0000b680: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
+0000b690: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
+0000b6a0: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
+0000b6b0: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
+0000b6c0: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
+0000b6d0: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
+0000b6e0: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
+0000b6f0: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
+0000b700: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
+0000b710: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
+0000b720: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
+0000b730: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
+0000b740: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
+0000b750: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
+0000b760: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
+0000b770: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
+0000b780: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
+0000b790: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
+0000b7a0: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
+0000b7b0: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
+0000b7c0: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
+0000b7d0: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
+0000b7e0: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
+0000b7f0: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
+0000b800: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
+0000b810: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
+0000b820: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
+0000b830: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
+0000b840: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
+0000b850: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
+0000b860: 202e 2e20 7365 6561 6c73 6f3a 3a0a 0a20   .. seealso::.. 
+0000b870: 2020 2020 2020 203a 6d65 7468 3a60 7072         :meth:`pr
+0000b880: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+0000b890: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
+0000b8a0: 616e 6b65 645f 7061 6972 735f 7769 7468  anked_pairs_with
+0000b8b0: 5f74 6573 7460 2c20 3a6d 6574 683a 6070  _test`, :meth:`p
+0000b8c0: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
+0000b8d0: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
+0000b8e0: 7269 7665 7260 0a0a 2020 2020 2222 220a  river`..    """.
+0000b8f0: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
+0000b900: 2065 6461 7461 2e63 616e 6469 6461 7465   edata.candidate
+0000b910: 7320 6966 2063 7572 725f 6361 6e64 7320  s if curr_cands 
+0000b920: 6973 204e 6f6e 6520 656c 7365 2063 7572  is None else cur
+0000b930: 725f 6361 6e64 7320 2020 200a 2020 2020  r_cands    .    
+0000b940: 6369 6478 5f74 6f5f 6361 6e64 203d 207b  cidx_to_cand = {
+0000b950: 6369 6478 3a20 6320 666f 7220 6369 6478  cidx: c for cidx
+0000b960: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
+0000b970: 2863 616e 6469 6461 7465 7329 7d20 200a  (candidates)}  .
+0000b980: 2020 2020 6361 6e64 5f74 6f5f 6369 6478      cand_to_cidx
+0000b990: 203d 207b 633a 2063 6964 7820 666f 7220   = {c: cidx for 
+0000b9a0: 6369 6478 2c20 6320 696e 2065 6e75 6d65  cidx, c in enume
+0000b9b0: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+0000b9c0: 7d20 200a 0a20 2020 2073 7472 656e 6774  }  ..    strengt
+0000b9d0: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
+0000b9e0: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
+0000b9f0: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
+0000ba00: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
+0000ba10: 6e67 7468 5f66 756e 6374 696f 6e20 2020  ngth_function   
+0000ba20: 200a 0a20 2020 2063 7720 3d20 6564 6174   ..    cw = edat
+0000ba30: 612e 636f 6e64 6f72 6365 745f 7769 6e6e  a.condorcet_winn
+0000ba40: 6572 2863 7572 725f 6361 6e64 733d 6375  er(curr_cands=cu
+0000ba50: 7272 5f63 616e 6473 290a 2020 2020 2320  rr_cands).    # 
+0000ba60: 5261 6e6b 6564 2050 6169 7273 2069 7320  Ranked Pairs is 
+0000ba70: 436f 6e64 6f72 6365 7420 636f 6e73 6973  Condorcet consis
+0000ba80: 7465 6e74 2c20 736f 2073 696d 706c 7920  tent, so simply 
+0000ba90: 7265 7475 726e 2074 6865 2043 6f6e 646f  return the Condo
+0000baa0: 7263 6574 2077 696e 6e65 7220 6966 2065  rcet winner if e
+0000bab0: 7869 7374 730a 2020 2020 6966 2063 7720  xists.    if cw 
+0000bac0: 6973 206e 6f74 204e 6f6e 653a 200a 2020  is not None: .  
+0000bad0: 2020 2020 2020 7769 6e6e 6572 7320 3d20        winners = 
+0000bae0: 5b63 775d 0a20 2020 2065 6c73 653a 0a20  [cw].    else:. 
+0000baf0: 2020 2020 2020 2077 5f65 6467 6573 203d         w_edges =
+0000bb00: 205b 2863 312c 2063 322c 2073 7472 656e   [(c1, c2, stren
+0000bb10: 6774 685f 6675 6e63 7469 6f6e 2863 312c  gth_function(c1,
+0000bb20: 2063 3229 2920 666f 7220 6331 2069 6e20   c2)) for c1 in 
+0000bb30: 6361 6e64 6964 6174 6573 2066 6f72 2063  candidates for c
+0000bb40: 3220 696e 2063 616e 6469 6461 7465 7320  2 in candidates 
+0000bb50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bb60: 2020 2020 6966 2063 3120 213d 2063 3220      if c1 != c2 
+0000bb70: 616e 6420 2865 6461 7461 2e6d 616a 6f72  and (edata.major
+0000bb80: 6974 795f 7072 6566 6572 7328 6331 2c20  ity_prefers(c1, 
+0000bb90: 6332 2920 6f72 2065 6461 7461 2e69 735f  c2) or edata.is_
+0000bba0: 7469 6564 2863 312c 2063 3229 295d 0a20  tied(c1, c2))]. 
+0000bbb0: 2020 2020 2020 2077 696e 6e65 7273 203d         winners =
+0000bbc0: 206c 6973 7428 2920 2020 2020 2020 2020   list()         
+0000bbd0: 2020 200a 2020 2020 2020 2020 7374 7265     .        stre
+0000bbe0: 6e67 7468 7320 3d20 736f 7274 6564 286c  ngths = sorted(l
+0000bbf0: 6973 7428 7365 7428 5b65 5b32 5d20 666f  ist(set([e[2] fo
+0000bc00: 7220 6520 696e 2077 5f65 6467 6573 5d29  r e in w_edges])
+0000bc10: 292c 2072 6576 6572 7365 3d54 7275 6529  ), reverse=True)
+0000bc20: 0a20 2020 2020 2020 2073 6f72 7465 645f  .        sorted_
+0000bc30: 6564 6765 7320 3d20 5b5b 6520 666f 7220  edges = [[e for 
+0000bc40: 6520 696e 2077 5f65 6467 6573 2069 6620  e in w_edges if 
+0000bc50: 655b 325d 203d 3d20 735d 2066 6f72 2073  e[2] == s] for s
+0000bc60: 2069 6e20 7374 7265 6e67 7468 735d 0a20   in strengths]. 
+0000bc70: 2020 2020 2020 2069 6620 6e70 2e70 726f         if np.pro
+0000bc80: 6428 5b6d 6174 682e 6661 6374 6f72 6961  d([math.factoria
+0000bc90: 6c28 6c65 6e28 6573 2929 2066 6f72 2065  l(len(es)) for e
+0000bca0: 7320 696e 2073 6f72 7465 645f 6564 6765  s in sorted_edge
+0000bcb0: 735d 2920 3e20 3330 3030 3a20 0a20 2020  s]) > 3000: .   
+0000bcc0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000bcd0: 4e6f 6e65 0a20 2020 2020 2020 2065 6c73  None.        els
+0000bce0: 653a 200a 2020 2020 2020 2020 2020 2020  e: .            
+0000bcf0: 7462 7320 3d20 7072 6f64 7563 7428 2a5b  tbs = product(*[
+0000bd00: 7065 726d 7574 6174 696f 6e73 2865 6467  permutations(edg
+0000bd10: 6573 2920 666f 7220 6564 6765 7320 696e  es) for edges in
+0000bd20: 2073 6f72 7465 645f 6564 6765 735d 290a   sorted_edges]).
+0000bd30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000bd40: 7462 2069 6e20 7462 733a 0a20 2020 2020  tb in tbs:.     
+0000bd50: 2020 2020 2020 2020 2020 2065 6467 6573             edges
+0000bd60: 203d 2066 6c61 7474 656e 2874 6229 0a20   = flatten(tb). 
+0000bd70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000bd80: 765f 6465 6665 6174 203d 2053 504f 286c  v_defeat = SPO(l
+0000bd90: 656e 2863 616e 6469 6461 7465 7329 290a  en(candidates)).
+0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdb0: 666f 7220 6530 2c65 312c 7320 696e 2065  for e0,e1,s in e
+0000bdc0: 6467 6573 3a20 0a20 2020 2020 2020 2020  dges: .         
+0000bdd0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0000bde0: 7420 7276 5f64 6566 6561 742e 505b 6361  t rv_defeat.P[ca
+0000bdf0: 6e64 5f74 6f5f 6369 6478 5b65 315d 5d5b  nd_to_cidx[e1]][
+0000be00: 6361 6e64 5f74 6f5f 6369 6478 5b65 305d  cand_to_cidx[e0]
+0000be10: 5d20 616e 6420 6c65 6e28 7276 5f64 6566  ] and len(rv_def
+0000be20: 6561 742e 7072 6564 735b 6361 6e64 5f74  eat.preds[cand_t
+0000be30: 6f5f 6369 6478 5b65 315d 5d29 203d 3d20  o_cidx[e1]]) == 
+0000be40: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+0000be50: 2020 2020 2020 2020 2020 2072 765f 6465             rv_de
+0000be60: 6665 6174 2e61 6464 2863 616e 645f 746f  feat.add(cand_to
+0000be70: 5f63 6964 785b 6530 5d2c 6361 6e64 5f74  _cidx[e0],cand_t
+0000be80: 6f5f 6369 6478 5b65 315d 290a 2020 2020  o_cidx[e1]).    
+0000be90: 2020 2020 2020 2020 2020 2020 7769 6e6e              winn
+0000bea0: 6572 732e 6170 7065 6e64 2863 6964 785f  ers.append(cidx_
+0000beb0: 746f 5f63 616e 645b 7276 5f64 6566 6561  to_cand[rv_defea
+0000bec0: 742e 696e 6974 6961 6c5f 656c 656d 656e  t.initial_elemen
+0000bed0: 7473 2829 5b30 5d5d 290a 2020 2020 7265  ts()[0]]).    re
+0000bee0: 7475 726e 2073 6f72 7465 6428 6c69 7374  turn sorted(list
+0000bef0: 2873 6574 2877 696e 6e65 7273 2929 290a  (set(winners))).
+0000bf00: 0a40 766d 286e 616d 653d 2252 6976 6572  .@vm(name="River
+0000bf10: 2054 4222 290a 6465 6620 7269 7665 725f   TB").def river_
+0000bf20: 7462 2865 6461 7461 2c20 6375 7272 5f63  tb(edata, curr_c
+0000bf30: 616e 6473 203d 204e 6f6e 652c 2074 6965  ands = None, tie
+0000bf40: 5f62 7265 616b 6572 203d 204e 6f6e 652c  _breaker = None,
+0000bf50: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000bf60: 6f6e 203d 204e 6f6e 6529 3a20 2020 0a20  on = None):   . 
+0000bf70: 2020 2022 2222 0a20 2020 2052 6976 6572     """.    River
+0000bf80: 2077 6974 6820 6120 6669 7865 6420 6c69   with a fixed li
+0000bf90: 6e65 6172 206f 7264 6572 206f 6e20 7468  near order on th
+0000bfa0: 6520 6361 6e64 6964 6174 6573 2074 6f20  e candidates to 
+0000bfb0: 6272 6561 6b20 616e 7920 7469 6573 2069  break any ties i
+0000bfc0: 6e20 7468 6520 6d61 7267 696e 732e 2020  n the margins.  
+0000bfd0: 5369 6e63 6520 7468 6520 7469 655f 6272  Since the tie_br
+0000bfe0: 6561 6b65 7220 6973 2061 206c 696e 6561  eaker is a linea
+0000bff0: 7220 6f72 6465 722c 2074 6869 7320 6d65  r order, this me
+0000c000: 7468 6f64 2069 7320 7265 736f 6c75 7465  thod is resolute
+0000c010: 2e20 2020 0a0a 2020 2020 4172 6773 3a0a  .   ..    Args:.
+0000c020: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
+0000c030: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
+0000c040: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
+0000c050: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
+0000c060: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
+0000c070: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
+0000c080: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
+0000c090: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
+0000c0a0: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
+0000c0b0: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
+0000c0c0: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
+0000c0d0: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
+0000c0e0: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
+0000c0f0: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
+0000c100: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
+0000c110: 2020 2020 2074 6965 5f62 7265 616b 6572       tie_breaker
+0000c120: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
+0000c130: 696f 6e61 6c29 3a20 4120 6c69 6e65 6172  ional): A linear
+0000c140: 206f 7264 6572 206f 6e20 7468 6520 6361   order on the ca
+0000c150: 6e64 6964 6174 6573 2e20 2049 6620 6e6f  ndidates.  If no
+0000c160: 7420 7365 742c 2074 6865 6e20 7468 6520  t set, then the 
+0000c170: 6361 6e64 6964 6174 6573 2061 7265 2073  candidates are s
+0000c180: 6f72 7465 6420 696e 2061 7363 656e 6469  orted in ascendi
+0000c190: 6e67 206f 7264 6572 2e0a 2020 2020 2020  ng order..      
+0000c1a0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+0000c1b0: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
+0000c1c0: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
+0000c1d0: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
+0000c1e0: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
+0000c1f0: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
+0000c200: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
+0000c210: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
+0000c220: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
+0000c230: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
+0000c240: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
+0000c250: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
+0000c260: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
+0000c270: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
+0000c280: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+0000c290: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
+0000c2a0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
+0000c2b0: 2e20 0a0a 2020 2020 2222 220a 2020 2020  . ..    """.    
+0000c2c0: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
+0000c2d0: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
+0000c2e0: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
+0000c2f0: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
+0000c300: 6e64 7320 2020 200a 2020 2020 6369 6478  nds    .    cidx
+0000c310: 5f74 6f5f 6361 6e64 203d 207b 6369 6478  _to_cand = {cidx
+0000c320: 3a20 6320 666f 7220 6369 6478 2c20 6320  : c for cidx, c 
+0000c330: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+0000c340: 6469 6461 7465 7329 7d20 200a 2020 2020  didates)}  .    
+0000c350: 6361 6e64 5f74 6f5f 6369 6478 203d 207b  cand_to_cidx = {
+0000c360: 633a 2063 6964 7820 666f 7220 6369 6478  c: cidx for cidx
+0000c370: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
+0000c380: 2863 616e 6469 6461 7465 7329 7d20 200a  (candidates)}  .
+0000c390: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+0000c3a0: 6374 696f 6e20 3d20 6564 6174 612e 6d61  ction = edata.ma
+0000c3b0: 7267 696e 2069 6620 7374 7265 6e67 7468  rgin if strength
+0000c3c0: 5f66 756e 6374 696f 6e20 6973 204e 6f6e  _function is Non
+0000c3d0: 6520 656c 7365 2073 7472 656e 6774 685f  e else strength_
+0000c3e0: 6675 6e63 7469 6f6e 2020 2020 0a0a 2020  function    ..  
+0000c3f0: 2020 7462 5f72 616e 6b69 6e67 203d 2074    tb_ranking = t
+0000c400: 6965 5f62 7265 616b 6572 2069 6620 7469  ie_breaker if ti
+0000c410: 655f 6272 6561 6b65 7220 6973 206e 6f74  e_breaker is not
+0000c420: 204e 6f6e 6520 656c 7365 2073 6f72 7465   None else sorte
+0000c430: 6428 6c69 7374 2863 616e 6469 6461 7465  d(list(candidate
+0000c440: 7329 290a 0a20 2020 2063 7720 3d20 6564  s))..    cw = ed
+0000c450: 6174 612e 636f 6e64 6f72 6365 745f 7769  ata.condorcet_wi
+0000c460: 6e6e 6572 2863 7572 725f 6361 6e64 733d  nner(curr_cands=
+0000c470: 6375 7272 5f63 616e 6473 290a 2020 2020  curr_cands).    
+0000c480: 2320 5269 7665 7220 6973 2043 6f6e 646f  # River is Condo
+0000c490: 7263 6574 2063 6f6e 7369 7374 656e 742c  rcet consistent,
+0000c4a0: 2073 6f20 7369 6d70 6c79 2072 6574 7572   so simply retur
+0000c4b0: 6e20 7468 6520 436f 6e64 6f72 6365 7420  n the Condorcet 
+0000c4c0: 7769 6e6e 6572 2069 6620 6578 6973 7473  winner if exists
+0000c4d0: 0a20 2020 2069 6620 6377 2069 7320 6e6f  .    if cw is no
+0000c4e0: 7420 4e6f 6e65 3a20 0a20 2020 2020 2020  t None: .       
+0000c4f0: 2077 696e 6e65 7273 203d 205b 6377 5d0a   winners = [cw].
+0000c500: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000c510: 2020 775f 6564 6765 7320 3d20 5b28 6331    w_edges = [(c1
+0000c520: 2c20 6332 2c20 7374 7265 6e67 7468 5f66  , c2, strength_f
+0000c530: 756e 6374 696f 6e28 6331 2c20 6332 2929  unction(c1, c2))
+0000c540: 2066 6f72 2063 3120 696e 2063 616e 6469   for c1 in candi
+0000c550: 6461 7465 7320 666f 7220 6332 2069 6e20  dates for c2 in 
+0000c560: 6361 6e64 6964 6174 6573 2069 6620 6331  candidates if c1
+0000c570: 2021 3d20 6332 2061 6e64 2028 6564 6174   != c2 and (edat
+0000c580: 612e 6d61 6a6f 7269 7479 5f70 7265 6665  a.majority_prefe
+0000c590: 7273 2863 312c 2063 3229 206f 7220 6564  rs(c1, c2) or ed
+0000c5a0: 6174 612e 6973 5f74 6965 6428 6331 2c20  ata.is_tied(c1, 
+0000c5b0: 6332 2929 5d0a 2020 2020 2020 2020 7769  c2))].        wi
+0000c5c0: 6e6e 6572 7320 3d20 6c69 7374 2829 2020  nners = list()  
+0000c5d0: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
+0000c5e0: 6873 203d 2073 6f72 7465 6428 6c69 7374  hs = sorted(list
+0000c5f0: 2873 6574 285b 655b 325d 2066 6f72 2065  (set([e[2] for e
+0000c600: 2069 6e20 775f 6564 6765 735d 2929 2c20   in w_edges])), 
+0000c610: 7265 7665 7273 653d 5472 7565 290a 0a20  reverse=True).. 
+0000c620: 2020 2020 2020 2072 765f 6465 6665 6174         rv_defeat
+0000c630: 203d 2053 504f 286c 656e 2863 616e 6469   = SPO(len(candi
+0000c640: 6461 7465 7329 290a 0a20 2020 2020 2020  dates))..       
+0000c650: 2066 6f72 2073 2069 6e20 7374 7265 6e67   for s in streng
+0000c660: 7468 733a 200a 2020 2020 2020 2020 2020  ths: .          
+0000c670: 2020 6564 6765 7320 3d20 5b65 2066 6f72    edges = [e for
+0000c680: 2065 2069 6e20 775f 6564 6765 7320 6966   e in w_edges if
+0000c690: 2065 5b32 5d20 3d3d 2073 5d0a 2020 2020   e[2] == s].    
+0000c6a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0000c6b0: 2020 2020 2023 2062 7265 616b 2074 6965       # break tie
+0000c6c0: 7320 7573 696e 6720 7468 6520 6c65 7869  s using the lexi
+0000c6d0: 636f 6772 6170 6869 6320 6f72 6465 7269  cographic orderi
+0000c6e0: 6e67 206f 6e20 7475 706c 6573 2067 6976  ng on tuples giv
+0000c6f0: 656e 2074 625f 7261 6e6b 696e 670a 2020  en tb_ranking.  
+0000c700: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
+0000c710: 5f65 6467 6573 203d 2073 6f72 7465 6428  _edges = sorted(
+0000c720: 6564 6765 732c 206b 6579 203d 206c 616d  edges, key = lam
+0000c730: 6264 6120 653a 2028 7462 5f72 616e 6b69  bda e: (tb_ranki
+0000c740: 6e67 2e69 6e64 6578 2865 5b30 5d29 2c20  ng.index(e[0]), 
+0000c750: 7462 5f72 616e 6b69 6e67 2e69 6e64 6578  tb_ranking.index
+0000c760: 2865 5b31 5d29 292c 2072 6576 6572 7365  (e[1])), reverse
+0000c770: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+0000c780: 2020 2020 666f 7220 6530 2c65 312c 7320      for e0,e1,s 
+0000c790: 696e 2073 6f72 7465 645f 6564 6765 733a  in sorted_edges:
+0000c7a0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0000c7b0: 2020 6966 206e 6f74 2072 765f 6465 6665    if not rv_defe
+0000c7c0: 6174 2e50 5b63 616e 645f 746f 5f63 6964  at.P[cand_to_cid
+0000c7d0: 785b 6531 5d5d 5b63 616e 645f 746f 5f63  x[e1]][cand_to_c
+0000c7e0: 6964 785b 6530 5d5d 2061 6e64 206c 656e  idx[e0]] and len
+0000c7f0: 2872 765f 6465 6665 6174 2e70 7265 6473  (rv_defeat.preds
+0000c800: 5b63 616e 645f 746f 5f63 6964 785b 6531  [cand_to_cidx[e1
+0000c810: 5d5d 2920 3d3d 2030 3a0a 2020 2020 2020  ]]) == 0:.      
+0000c820: 2020 2020 2020 2020 2020 2020 2020 7276                rv
+0000c830: 5f64 6566 6561 742e 6164 6428 6361 6e64  _defeat.add(cand
+0000c840: 5f74 6f5f 6369 6478 5b65 305d 2c63 616e  _to_cidx[e0],can
+0000c850: 645f 746f 5f63 6964 785b 6531 5d29 0a20  d_to_cidx[e1]). 
+0000c860: 2020 2020 2020 2020 2020 2077 696e 6e65             winne
+0000c870: 7273 2e61 7070 656e 6428 6369 6478 5f74  rs.append(cidx_t
+0000c880: 6f5f 6361 6e64 5b72 765f 6465 6665 6174  o_cand[rv_defeat
+0000c890: 2e69 6e69 7469 616c 5f65 6c65 6d65 6e74  .initial_element
+0000c8a0: 7328 295b 305d 5d29 0a20 2020 2072 6574  s()[0]]).    ret
+0000c8b0: 7572 6e20 736f 7274 6564 286c 6973 7428  urn sorted(list(
+0000c8c0: 7365 7428 7769 6e6e 6572 7329 2929 0a0a  set(winners)))..
+0000c8d0: 0a40 766d 286e 616d 653d 2252 6976 6572  .@vm(name="River
+0000c8e0: 205a 5422 290a 6465 6620 7269 7665 725f   ZT").def river_
+0000c8f0: 7a74 2870 726f 6669 6c65 2c20 6375 7272  zt(profile, curr
+0000c900: 5f63 616e 6473 203d 204e 6f6e 652c 2073  _cands = None, s
+0000c910: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000c920: 203d 204e 6f6e 6529 3a20 2020 0a20 2020   = None):   .   
+0000c930: 2022 2222 5269 7665 7220 7768 6572 6520   """River where 
+0000c940: 6120 6669 7865 6420 766f 7465 7220 6272  a fixed voter br
+0000c950: 6561 6b73 2061 6e79 2074 6965 7320 696e  eaks any ties in
+0000c960: 2074 6865 206d 6172 6769 6e73 2e20 2049   the margins.  I
+0000c970: 7420 6973 2061 6c77 6179 7320 7468 6520  t is always the 
+0000c980: 766f 7465 7220 696e 2070 6f73 6974 696f  voter in positio
+0000c990: 6e20 3020 7468 6174 2062 7265 616b 7320  n 0 that breaks 
+0000c9a0: 7468 6520 7469 6573 2e20 2053 696e 6365  the ties.  Since
+0000c9b0: 2076 6f74 6572 7320 6861 7665 2073 7472   voters have str
+0000c9c0: 6963 7420 7072 6566 6572 656e 6365 732c  ict preferences,
+0000c9d0: 2074 6869 7320 6d65 7468 6f64 2069 7320   this method is 
+0000c9e0: 7265 736f 6c75 7465 2e20 200a 0a20 2020  resolute.  ..   
+0000c9f0: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
+0000ca00: 6461 7461 2028 5072 6f66 696c 6529 3a20  data (Profile): 
+0000ca10: 4120 7072 6f66 696c 6520 6f66 206c 696e  A profile of lin
+0000ca20: 6561 7220 6f72 6465 7273 0a20 2020 2020  ear orders.     
+0000ca30: 2020 2063 7572 725f 6361 6e64 7320 284c     curr_cands (L
+0000ca40: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
+0000ca50: 616c 293a 2049 6620 7365 742c 2074 6865  al): If set, the
+0000ca60: 6e20 6669 6e64 2074 6865 2077 696e 6e65  n find the winne
+0000ca70: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
+0000ca80: 6c65 2072 6573 7472 6963 7465 6420 746f  le restricted to
+0000ca90: 2074 6865 2063 616e 6469 6461 7465 7320   the candidates 
+0000caa0: 696e 2060 6063 7572 725f 6361 6e64 7360  in ``curr_cands`
+0000cab0: 600a 0a20 2020 2052 6574 7572 6e73 3a20  `..    Returns: 
+0000cac0: 0a20 2020 2020 2020 2041 2073 6f72 7465  .        A sorte
+0000cad0: 6420 6c69 7374 206f 6620 6361 6e64 6964  d list of candid
+0000cae0: 6174 6573 2e20 0a0a 2020 2020 2e2e 2073  ates. ..    .. s
+0000caf0: 6565 616c 736f 3a3a 0a0a 2020 2020 2020  eealso::..      
+0000cb00: 2020 3a6d 6574 683a 6070 7265 665f 766f    :meth:`pref_vo
+0000cb10: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+0000cb20: 645f 6d65 7468 6f64 732e 7269 7665 7260  d_methods.river`
+0000cb30: 2c20 3a6d 6574 683a 6070 7265 665f 766f  , :meth:`pref_vo
+0000cb40: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+0000cb50: 645f 6d65 7468 6f64 732e 7269 7665 725f  d_methods.river_
+0000cb60: 7769 7468 5f74 6573 7460 2c20 3a6d 6574  with_test`, :met
+0000cb70: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
+0000cb80: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+0000cb90: 6f64 732e 7261 6e6b 6564 5f70 6169 7273  ods.ranked_pairs
+0000cba0: 600a 0a20 2020 200a 2020 2020 2222 220a  `..    .    """.
+0000cbb0: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
+0000cbc0: 2070 726f 6669 6c65 2e63 616e 6469 6461   profile.candida
+0000cbd0: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
+0000cbe0: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
+0000cbf0: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
+0000cc00: 2020 0a20 2020 2023 2074 6865 2074 6965    .    # the tie
+0000cc10: 2d62 7265 616b 6572 2069 7320 616c 7761  -breaker is alwa
+0000cc20: 7973 2074 6865 2066 6972 7374 2076 6f74  ys the first vot
+0000cc30: 6572 2e20 0a20 2020 2074 625f 7261 6e6b  er. .    tb_rank
+0000cc40: 696e 6720 3d20 7475 706c 6528 5b63 2066  ing = tuple([c f
+0000cc50: 6f72 2063 2069 6e20 6c69 7374 2870 726f  or c in list(pro
+0000cc60: 6669 6c65 2e5f 7261 6e6b 696e 6773 5b30  file._rankings[0
+0000cc70: 5d29 2069 6620 6320 696e 2063 616e 6469  ]) if c in candi
+0000cc80: 6461 7465 735d 290a 2020 2020 0a20 2020  dates]).    .   
+0000cc90: 2072 6574 7572 6e20 7269 7665 725f 7462   return river_tb
+0000cca0: 2870 726f 6669 6c65 2c20 6375 7272 5f63  (profile, curr_c
+0000ccb0: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
+0000ccc0: 732c 2074 6965 5f62 7265 616b 6572 203d  s, tie_breaker =
+0000ccd0: 2074 625f 7261 6e6b 696e 672c 2073 7472   tb_ranking, str
+0000cce0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+0000ccf0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000cd00: 6f6e 290a 2020 2020 0a0a 2320 5369 6d70  on).    ..# Simp
+0000cd10: 6c65 2053 7461 626c 6520 566f 7469 6e67  le Stable Voting
+0000cd20: 200a 6465 6620 5f73 696d 706c 655f 7374   .def _simple_st
+0000cd30: 6162 6c65 5f76 6f74 696e 6728 6375 7272  able_voting(curr
+0000cd40: 5f63 616e 6473 2c20 0a20 2020 2020 2020  _cands, .       
+0000cd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd60: 2020 2073 6f72 7465 645f 6d61 7463 6865     sorted_matche
+0000cd70: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0000cd80: 2020 2020 2020 2020 2020 2020 206d 656d               mem
+0000cd90: 5f73 765f 7769 6e6e 6572 7329 3a0a 2020  _sv_winners):.  
+0000cda0: 2020 2727 270a 2020 2020 4465 7465 726d    '''.    Determ
+0000cdb0: 696e 6520 7468 6520 5369 6d70 6c65 2053  ine the Simple S
+0000cdc0: 7461 626c 6520 566f 7469 6e67 2077 696e  table Voting win
+0000cdd0: 6e65 7273 2077 6869 6c65 206b 6565 7069  ners while keepi
+0000cde0: 6e67 2074 7261 636b 200a 2020 2020 6f66  ng track .    of
+0000cdf0: 2074 6865 2077 696e 6e65 7273 2069 6e20   the winners in 
+0000ce00: 616e 7920 7375 6270 726f 6669 6c65 7320  any subprofiles 
+0000ce10: 6368 6563 6b65 6420 6475 7269 6e67 2063  checked during c
+0000ce20: 6f6d 7075 7461 7469 6f6e 2e20 0a20 2020  omputation. .   
+0000ce30: 2027 2727 0a20 2020 200a 2020 2020 7376   '''.    .    sv
+0000ce40: 5f77 696e 6e65 7273 203d 206c 6973 7428  _winners = list(
+0000ce50: 290a 2020 2020 2020 2020 0a20 2020 2069  ).        .    i
+0000ce60: 6620 6c65 6e28 6375 7272 5f63 616e 6473  f len(curr_cands
+0000ce70: 2920 3d3d 2031 3a20 0a20 2020 2020 2020  ) == 1: .       
+0000ce80: 206d 656d 5f73 765f 7769 6e6e 6572 735b   mem_sv_winners[
+0000ce90: 7475 706c 6528 6375 7272 5f63 616e 6473  tuple(curr_cands
+0000cea0: 295d 203d 2063 7572 725f 6361 6e64 730a  )] = curr_cands.
+0000ceb0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+0000cec0: 7572 725f 6361 6e64 732c 206d 656d 5f73  urr_cands, mem_s
+0000ced0: 765f 7769 6e6e 6572 730a 2020 2020 0a20  v_winners.    . 
+0000cee0: 2020 206d 6172 6769 6e5f 7769 746e 6573     margin_witnes
+0000cef0: 7369 6e67 5f77 696e 203d 202d 6d61 7468  sing_win = -math
+0000cf00: 2e69 6e66 0a0a 2020 2020 666f 7220 612c  .inf..    for a,
+0000cf10: 2062 2c20 7320 696e 2073 6f72 7465 645f   b, s in sorted_
+0000cf20: 6d61 7463 6865 733a 0a20 2020 2020 2020  matches:.       
+0000cf30: 2069 6620 7320 3c20 6d61 7267 696e 5f77   if s < margin_w
+0000cf40: 6974 6e65 7373 696e 675f 7769 6e3a 200a  itnessing_win: .
+0000cf50: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+0000cf60: 6b0a 2020 2020 2020 2020 6966 2061 206e  k.        if a n
+0000cf70: 6f74 2069 6e20 7376 5f77 696e 6e65 7273  ot in sv_winners
+0000cf80: 3a20 0a20 2020 2020 2020 2020 2020 2063  : .            c
+0000cf90: 616e 6473 5f6d 696e 7573 5f62 203d 205b  ands_minus_b = [
+0000cfa0: 6320 666f 7220 6320 696e 2063 7572 725f  c for c in curr_
+0000cfb0: 6361 6e64 7320 6966 2063 2021 3d20 625d  cands if c != b]
+0000cfc0: 0a20 2020 2020 2020 2020 2020 2063 616e  .            can
+0000cfd0: 6473 5f6d 696e 7573 5f62 5f6b 6579 203d  ds_minus_b_key =
+0000cfe0: 2074 7570 6c65 2873 6f72 7465 6428 6361   tuple(sorted(ca
+0000cff0: 6e64 735f 6d69 6e75 735f 6229 290a 2020  nds_minus_b)).  
+0000d000: 2020 2020 2020 2020 2020 6966 2063 616e            if can
+0000d010: 6473 5f6d 696e 7573 5f62 5f6b 6579 206e  ds_minus_b_key n
+0000d020: 6f74 2069 6e20 6d65 6d5f 7376 5f77 696e  ot in mem_sv_win
+0000d030: 6e65 7273 2e6b 6579 7328 293a 200a 2020  ners.keys(): .  
+0000d040: 2020 2020 2020 2020 2020 2020 2020 7773                ws
+0000d050: 2c20 6d65 6d5f 7376 5f77 696e 6e65 7273  , mem_sv_winners
+0000d060: 203d 205f 7369 6d70 6c65 5f73 7461 626c   = _simple_stabl
+0000d070: 655f 766f 7469 6e67 2863 7572 725f 6361  e_voting(curr_ca
+0000d080: 6e64 7320 3d20 6361 6e64 735f 6d69 6e75  nds = cands_minu
+0000d090: 735f 622c 0a20 2020 2020 2020 2020 2020  s_b,.           
+0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0d0: 736f 7274 6564 5f6d 6174 6368 6573 203d  sorted_matches =
+0000d0e0: 205b 2861 2c20 632c 2073 2920 666f 7220   [(a, c, s) for 
+0000d0f0: 612c 2063 2c20 7320 696e 2073 6f72 7465  a, c, s in sorte
+0000d100: 645f 6d61 7463 6865 7320 6966 2061 2021  d_matches if a !
+0000d110: 3d20 6220 616e 6420 6320 213d 2062 5d2c  = b and c != b],
+0000d120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d150: 2020 2020 2020 2020 2020 2020 6d65 6d5f              mem_
+0000d160: 7376 5f77 696e 6e65 7273 203d 206d 656d  sv_winners = mem
+0000d170: 5f73 765f 7769 6e6e 6572 7329 0a20 2020  _sv_winners).   
+0000d180: 2020 2020 2020 2020 2020 2020 206d 656d               mem
+0000d190: 5f73 765f 7769 6e6e 6572 735b 6361 6e64  _sv_winners[cand
+0000d1a0: 735f 6d69 6e75 735f 625f 6b65 795d 203d  s_minus_b_key] =
+0000d1b0: 2077 730a 2020 2020 2020 2020 2020 2020   ws.            
+0000d1c0: 656c 7365 3a20 0a20 2020 2020 2020 2020  else: .         
+0000d1d0: 2020 2020 2020 2077 7320 3d20 6d65 6d5f         ws = mem_
+0000d1e0: 7376 5f77 696e 6e65 7273 5b63 616e 6473  sv_winners[cands
+0000d1f0: 5f6d 696e 7573 5f62 5f6b 6579 5d0a 2020  _minus_b_key].  
+0000d200: 2020 2020 2020 2020 2020 6966 2061 2069            if a i
+0000d210: 6e20 7773 3a0a 2020 2020 2020 2020 2020  n ws:.          
+0000d220: 2020 2020 2020 7376 5f77 696e 6e65 7273        sv_winners
+0000d230: 2e61 7070 656e 6428 6129 0a20 2020 2020  .append(a).     
+0000d240: 2020 2020 2020 2020 2020 206d 6172 6769             margi
+0000d250: 6e5f 7769 746e 6573 7369 6e67 5f77 696e  n_witnessing_win
+0000d260: 203d 2073 0a0a 2020 2020 7265 7475 726e   = s..    return
+0000d270: 2073 765f 7769 6e6e 6572 732c 206d 656d   sv_winners, mem
+0000d280: 5f73 765f 7769 6e6e 6572 730a 2020 2020  _sv_winners.    
+0000d290: 0a0a 4076 6d28 6e61 6d65 203d 2022 5369  ..@vm(name = "Si
+0000d2a0: 6d70 6c65 2053 7461 626c 6520 566f 7469  mple Stable Voti
+0000d2b0: 6e67 2229 0a64 6566 205f 7369 6d70 6c65  ng").def _simple
+0000d2c0: 5f73 7461 626c 655f 766f 7469 6e67 5f77  _stable_voting_w
+0000d2d0: 6974 685f 636f 6e64 6f72 6365 745f 6368  ith_condorcet_ch
+0000d2e0: 6563 6b28 0a20 2020 2065 6461 7461 2c20  eck(.    edata, 
+0000d2f0: 0a20 2020 2063 7572 725f 6361 6e64 7320  .    curr_cands 
+0000d300: 3d20 4e6f 6e65 2c20 0a20 2020 2073 7472  = None, .    str
+0000d310: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+0000d320: 204e 6f6e 6529 3a20 0a20 2020 2022 2222   None): .    """
+0000d330: 5369 6d70 6c65 2053 7461 626c 6520 566f  Simple Stable Vo
+0000d340: 7469 6e67 2069 7320 436f 6e64 6f72 6365  ting is Condorce
+0000d350: 7420 636f 6e73 6973 7465 6e74 2e20 2020  t consistent.   
+0000d360: 4974 2069 7320 6661 7374 6572 2074 6f20  It is faster to 
+0000d370: 736b 6970 2065 7865 6375 7469 6e67 2074  skip executing t
+0000d380: 6865 2072 6563 7572 7369 7665 2061 6c67  he recursive alg
+0000d390: 6f72 6974 686d 2077 6865 6e20 7468 6572  orithm when ther
+0000d3a0: 6520 6973 2061 2043 6f6e 646f 7263 6574  e is a Condorcet
+0000d3b0: 2077 696e 6e65 7246 6972 7374 2063 6865   winnerFirst che
+0000d3c0: 636b 2069 6620 7468 6572 6520 6973 2061  ck if there is a
+0000d3d0: 2043 6f6e 646f 7263 6574 2077 696e 6e65   Condorcet winne
+0000d3e0: 722e 2020 4966 2073 6f2c 2072 6574 7572  r.  If so, retur
+0000d3f0: 6e20 7468 6520 436f 6e64 6f72 6365 7420  n the Condorcet 
+0000d400: 7769 6e6e 6572 2c20 6f74 6865 7277 6973  winner, otherwis
+0000d410: 6520 6669 6e64 2074 6865 2053 696d 706c  e find the Simpl
+0000d420: 6520 5374 6162 6c65 2056 6f74 696e 6720  e Stable Voting 
+0000d430: 7769 6e6e 6572 2075 7369 6e67 205f 7369  winner using _si
+0000d440: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
+0000d450: 6e67 0a0a 2020 2020 4172 6773 3a0a 2020  ng..    Args:.  
+0000d460: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
+0000d470: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
+0000d480: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
+0000d490: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
+0000d4a0: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
+0000d4b0: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
+0000d4c0: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
+0000d4d0: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
+0000d4e0: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
+0000d4f0: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
+0000d500: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
+0000d510: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
+0000d520: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
+0000d530: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
+0000d540: 7272 5f63 616e 6473 6060 0a20 2020 2020  rr_cands``.     
+0000d550: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+0000d560: 7469 6f6e 2028 6675 6e63 7469 6f6e 2c20  tion (function, 
+0000d570: 6f70 7469 6f6e 616c 293a 2054 6865 2073  optional): The s
+0000d580: 7472 656e 6774 6820 6675 6e63 7469 6f6e  trength function
+0000d590: 2074 6f20 6265 2075 7365 6420 746f 2063   to be used to c
+0000d5a0: 616c 6375 6c61 7465 2074 6865 2073 7472  alculate the str
+0000d5b0: 656e 6774 6820 6f66 2061 2070 6174 682e  ength of a path.
+0000d5c0: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
+0000d5d0: 7320 7468 6520 6d61 7267 696e 206d 6574  s the margin met
+0000d5e0: 686f 6420 6f66 2060 6065 6461 7461 6060  hod of ``edata``
+0000d5f0: 2e20 2020 5468 6973 206f 6e6c 7920 6d61  .   This only ma
+0000d600: 7474 6572 7320 7768 656e 2074 6865 2062  tters when the b
+0000d610: 616c 6c6f 7473 2061 7265 206e 6f74 206c  allots are not l
+0000d620: 696e 6561 7220 6f72 6465 7273 2e20 0a0a  inear orders. ..
+0000d630: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
+0000d640: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
+0000d650: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
+0000d660: 732e 200a 0a20 2020 2022 2222 0a20 2020  s. ..    """.   
+0000d670: 200a 2020 2020 6377 203d 2065 6461 7461   .    cw = edata
+0000d680: 2e63 6f6e 646f 7263 6574 5f77 696e 6e65  .condorcet_winne
+0000d690: 7228 6375 7272 5f63 616e 6473 203d 2063  r(curr_cands = c
+0000d6a0: 7572 725f 6361 6e64 7329 0a20 2020 2069  urr_cands).    i
+0000d6b0: 6620 6377 2069 7320 6e6f 7420 4e6f 6e65  f cw is not None
+0000d6c0: 3a20 0a20 2020 2020 2020 2072 6574 7572  : .        retur
+0000d6d0: 6e20 5b63 775d 0a20 2020 2065 6c73 653a  n [cw].    else:
+0000d6e0: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
+0000d6f0: 616e 6473 203d 2065 6461 7461 2e63 616e  ands = edata.can
+0000d700: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
+0000d710: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
+0000d720: 7365 2063 7572 725f 6361 6e64 730a 2020  se curr_cands.  
+0000d730: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
+0000d740: 756e 6374 696f 6e20 3d20 6564 6174 612e  unction = edata.
+0000d750: 6d61 7267 696e 2069 6620 7374 7265 6e67  margin if streng
+0000d760: 7468 5f66 756e 6374 696f 6e20 6973 204e  th_function is N
+0000d770: 6f6e 6520 656c 7365 2073 7472 656e 6774  one else strengt
+0000d780: 685f 6675 6e63 7469 6f6e 2020 0a0a 2020  h_function  ..  
+0000d790: 2020 2020 2020 6d61 7463 6865 7320 3d20        matches = 
+0000d7a0: 5b28 612c 2062 2c20 7374 7265 6e67 7468  [(a, b, strength
+0000d7b0: 5f66 756e 6374 696f 6e28 612c 2062 2929  _function(a, b))
+0000d7c0: 2066 6f72 2061 2069 6e20 6375 7272 5f63   for a in curr_c
+0000d7d0: 616e 6473 2066 6f72 2062 2069 6e20 6375  ands for b in cu
+0000d7e0: 7272 5f63 616e 6473 2069 6620 6120 213d  rr_cands if a !=
+0000d7f0: 2062 5d0a 2020 2020 2020 2020 736f 7274   b].        sort
+0000d800: 6564 5f6d 6174 6368 6573 203d 2073 6f72  ed_matches = sor
+0000d810: 7465 6428 6d61 7463 6865 732c 2072 6576  ted(matches, rev
+0000d820: 6572 7365 3d54 7275 652c 206b 6579 3d6c  erse=True, key=l
+0000d830: 616d 6264 6120 6d5f 775f 7765 6967 6874  ambda m_w_weight
+0000d840: 3a20 6d5f 775f 7765 6967 6874 5b32 5d29  : m_w_weight[2])
+0000d850: 0a20 2020 200a 2020 2020 2020 2020 7265  .    .        re
+0000d860: 7475 726e 2073 6f72 7465 6428 5f73 696d  turn sorted(_sim
+0000d870: 706c 655f 7374 6162 6c65 5f76 6f74 696e  ple_stable_votin
+0000d880: 6728 6375 7272 5f63 616e 6473 203d 2063  g(curr_cands = c
+0000d890: 7572 725f 6361 6e64 732c 200a 2020 2020  urr_cands, .    
+0000d8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8c0: 2020 2020 2020 2020 736f 7274 6564 5f6d          sorted_m
+0000d8d0: 6174 6368 6573 203d 2073 6f72 7465 645f  atches = sorted_
+0000d8e0: 6d61 7463 6865 732c 0a20 2020 2020 2020  matches,.       
+0000d8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d910: 2020 2020 206d 656d 5f73 765f 7769 6e6e       mem_sv_winn
+0000d920: 6572 7320 3d20 7b7d 295b 305d 290a 0a0a  ers = {})[0])...
+0000d930: 6465 6620 5f73 696d 706c 655f 7374 6162  def _simple_stab
+0000d940: 6c65 5f76 6f74 696e 675f 6261 7369 6328  le_voting_basic(
+0000d950: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
+0000d960: 7320 3d20 4e6f 6e65 2c20 7374 7265 6e67  s = None, streng
+0000d970: 7468 5f66 756e 6374 696f 6e20 3d20 4e6f  th_function = No
+0000d980: 6e65 293a 200a 2020 2020 2222 2249 6d70  ne): .    """Imp
+0000d990: 6c65 6d65 6e74 6174 696f 6e20 6f66 2053  lementation of S
+0000d9a0: 696d 706c 6520 5374 6162 6c65 2056 6f74  imple Stable Vot
+0000d9b0: 696e 6720 6672 6f6d 2068 7474 7073 3a2f  ing from https:/
+0000d9c0: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+0000d9d0: 3130 382e 3030 3534 322e 200a 0a20 2020  108.00542. ..   
+0000d9e0: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
+0000d9f0: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
+0000da00: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
+0000da10: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
+0000da20: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
+0000da30: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
+0000da40: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
+0000da50: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
+0000da60: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
+0000da70: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
+0000da80: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
+0000da90: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
+0000daa0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
+0000dab0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
+0000dac0: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
+0000dad0: 7360 600a 2020 2020 2020 2020 7374 7265  s``.        stre
+0000dae0: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
+0000daf0: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
+0000db00: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
+0000db10: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
+0000db20: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
+0000db30: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
+0000db40: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
+0000db50: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
+0000db60: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
+0000db70: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
+0000db80: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
+0000db90: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
+0000dba0: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
+0000dbb0: 7264 6572 732e 200a 0a20 2020 2052 6574  rders. ..    Ret
+0000dbc0: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
+0000dbd0: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
+0000dbe0: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
+0000dbf0: 2020 2222 220a 2020 2020 0a20 2020 2063    """.    .    c
+0000dc00: 7572 725f 6361 6e64 7320 3d20 6564 6174  urr_cands = edat
+0000dc10: 612e 6361 6e64 6964 6174 6573 2069 6620  a.candidates if 
+0000dc20: 6375 7272 5f63 616e 6473 2069 7320 4e6f  curr_cands is No
+0000dc30: 6e65 2065 6c73 6520 6375 7272 5f63 616e  ne else curr_can
+0000dc40: 6473 0a20 2020 2073 7472 656e 6774 685f  ds.    strength_
+0000dc50: 6675 6e63 7469 6f6e 203d 2065 6461 7461  function = edata
+0000dc60: 2e6d 6172 6769 6e20 6966 2073 7472 656e  .margin if stren
+0000dc70: 6774 685f 6675 6e63 7469 6f6e 2069 7320  gth_function is 
+0000dc80: 4e6f 6e65 2065 6c73 6520 7374 7265 6e67  None else streng
+0000dc90: 7468 5f66 756e 6374 696f 6e20 200a 0a20  th_function  .. 
+0000dca0: 2020 206d 6174 6368 6573 203d 205b 2861     matches = [(a
+0000dcb0: 2c20 622c 2073 7472 656e 6774 685f 6675  , b, strength_fu
+0000dcc0: 6e63 7469 6f6e 2861 2c20 6229 2920 666f  nction(a, b)) fo
+0000dcd0: 7220 6120 696e 2063 7572 725f 6361 6e64  r a in curr_cand
+0000dce0: 7320 666f 7220 6220 696e 2063 7572 725f  s for b in curr_
+0000dcf0: 6361 6e64 7320 6966 2061 2021 3d20 625d  cands if a != b]
+0000dd00: 0a20 2020 2073 6f72 7465 645f 6d61 7463  .    sorted_matc
+0000dd10: 6865 7320 3d20 736f 7274 6564 286d 6174  hes = sorted(mat
+0000dd20: 6368 6573 2c20 7265 7665 7273 653d 5472  ches, reverse=Tr
+0000dd30: 7565 2c20 6b65 793d 6c61 6d62 6461 206d  ue, key=lambda m
+0000dd40: 5f77 5f77 6569 6768 743a 206d 5f77 5f77  _w_weight: m_w_w
+0000dd50: 6569 6768 745b 325d 290a 2020 2020 0a20  eight[2]).    . 
+0000dd60: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
+0000dd70: 285f 7369 6d70 6c65 5f73 7461 626c 655f  (_simple_stable_
+0000dd80: 766f 7469 6e67 2863 7572 725f 6361 6e64  voting(curr_cand
+0000dd90: 7320 3d20 6375 7272 5f63 616e 6473 2c20  s = curr_cands, 
+0000dda0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddc0: 2020 2020 2020 2020 2073 6f72 7465 645f           sorted_
+0000ddd0: 6d61 7463 6865 7320 3d20 736f 7274 6564  matches = sorted
+0000dde0: 5f6d 6174 6368 6573 2c0a 2020 2020 2020  _matches,.      
+0000ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de10: 2020 6d65 6d5f 7376 5f77 696e 6e65 7273    mem_sv_winners
+0000de20: 203d 207b 7d29 5b30 5d29 0a0a 0a40 766d   = {})[0])...@vm
+0000de30: 286e 616d 6520 3d20 2253 696d 706c 6520  (name = "Simple 
+0000de40: 5374 6162 6c65 2056 6f74 696e 6722 290a  Stable Voting").
+0000de50: 6465 6620 7369 6d70 6c65 5f73 7461 626c  def simple_stabl
+0000de60: 655f 766f 7469 6e67 280a 2020 2020 6564  e_voting(.    ed
+0000de70: 6174 612c 200a 2020 2020 6375 7272 5f63  ata, .    curr_c
+0000de80: 616e 6473 3d4e 6f6e 652c 200a 2020 2020  ands=None, .    
+0000de90: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+0000dea0: 6e3d 4e6f 6e65 2c0a 2020 2020 616c 676f  n=None,.    algo
+0000deb0: 7269 7468 6d20 3d20 2762 6173 6963 2729  rithm = 'basic')
+0000dec0: 3a20 0a0a 2020 2020 2222 2249 6d70 6c65  : ..    """Imple
+0000ded0: 6d65 6e74 6174 696f 6e20 6f66 2053 696d  mentation of Sim
+0000dee0: 706c 6520 5374 6162 6c65 2056 6f74 696e  ple Stable Votin
+0000def0: 6720 6672 6f6d 2068 7474 7073 3a2f 2f61  g from https://a
+0000df00: 7278 6976 2e6f 7267 2f61 6273 2f32 3130  rxiv.org/abs/210
+0000df10: 382e 3030 3534 322e 200a 0a20 2020 2053  8.00542. ..    S
+0000df20: 696d 706c 6520 5374 6162 6c65 2056 6f74  imple Stable Vot
+0000df30: 696e 6720 6973 2061 2072 6563 7572 7369  ing is a recursi
+0000df40: 7665 2076 6f74 696e 6720 6d65 7468 6f64  ve voting method
+0000df50: 2064 6566 696e 6564 2061 7320 666f 6c6c   defined as foll
+0000df60: 6f77 733a 200a 0a20 2020 2031 2e20 4966  ows: ..    1. If
+0000df70: 2074 6865 7265 2069 7320 6f6e 6c79 206f   there is only o
+0000df80: 6e65 2063 616e 6469 6461 7465 2069 6e20  ne candidate in 
+0000df90: 7468 6520 7072 6f66 696c 652c 2074 6865  the profile, the
+0000dfa0: 6e20 7468 6174 2063 616e 6469 6461 7465  n that candidate
+0000dfb0: 2069 7320 7468 6520 7769 6e6e 6572 2e20   is the winner. 
+0000dfc0: 0a20 2020 2032 2e20 4f72 6465 7220 7468  .    2. Order th
+0000dfd0: 6520 7061 6972 7320 3a6d 6174 683a 6028  e pairs :math:`(
+0000dfe0: 612c 6229 6020 6f66 2063 616e 6469 6461  a,b)` of candida
+0000dff0: 7465 7320 6672 6f6d 206c 6172 6765 7374  tes from largest
+0000e000: 2074 6f20 736d 616c 6c65 7374 2076 616c   to smallest val
+0000e010: 7565 206f 6620 7468 6520 6d61 7267 696e  ue of the margin
+0000e020: 206f 6620 3a6d 6174 683a 6061 6020 6f76   of :math:`a` ov
+0000e030: 6572 203a 6d61 7468 3a60 6260 2c20 616e  er :math:`b`, an
+0000e040: 6420 6465 636c 6172 6520 6173 2053 696d  d declare as Sim
+0000e050: 706c 6520 5374 6162 6c65 2056 6f74 696e  ple Stable Votin
+0000e060: 6720 7769 6e6e 6572 7320 7468 6520 6361  g winners the ca
+0000e070: 6e64 6964 6174 6528 7329 203a 6d61 7468  ndidate(s) :math
+0000e080: 3a60 6160 2066 726f 6d20 7468 6520 6561  :`a` from the ea
+0000e090: 726c 6965 7374 2070 6169 7228 7329 203a  rliest pair(s) :
+0000e0a0: 6d61 7468 3a60 2861 2c62 2960 2073 7563  math:`(a,b)` suc
+0000e0b0: 6820 7468 6174 203a 6d61 7468 3a60 6160  h that :math:`a`
+0000e0c0: 2069 7320 6120 5369 6d70 6c65 2053 7461   is a Simple Sta
+0000e0d0: 626c 6520 566f 7469 6e67 2077 696e 6e65  ble Voting winne
+0000e0e0: 7220 696e 2074 6865 2065 6c65 6374 696f  r in the electio
+0000e0f0: 6e20 7769 7468 6f75 7420 3a6d 6174 683a  n without :math:
+0000e100: 6062 602e 200a 0a20 2020 2041 7267 733a  `b`. ..    Args:
+0000e110: 0a20 2020 2020 2020 2065 6461 7461 2028  .        edata (
+0000e120: 5072 6f66 696c 652c 2050 726f 6669 6c65  Profile, Profile
+0000e130: 5769 7468 5469 6573 2c20 4d61 7267 696e  WithTies, Margin
+0000e140: 4772 6170 6829 3a20 416e 7920 656c 6563  Graph): Any elec
+0000e150: 7469 6f6e 2064 6174 6120 7468 6174 2068  tion data that h
+0000e160: 6173 2061 2060 6d61 7267 696e 6020 6d65  as a `margin` me
+0000e170: 7468 6f64 2e20 0a20 2020 2020 2020 2063  thod. .        c
+0000e180: 7572 725f 6361 6e64 7320 284c 6973 745b  urr_cands (List[
+0000e190: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
+0000e1a0: 2049 6620 7365 742c 2074 6865 6e20 6669   If set, then fi
+0000e1b0: 6e64 2074 6865 2077 696e 6e65 7273 2066  nd the winners f
+0000e1c0: 6f72 2074 6865 2070 726f 6669 6c65 2072  or the profile r
+0000e1d0: 6573 7472 6963 7465 6420 746f 2074 6865  estricted to the
+0000e1e0: 2063 616e 6469 6461 7465 7320 696e 2060   candidates in `
+0000e1f0: 6063 7572 725f 6361 6e64 7360 600a 2020  `curr_cands``.  
+0000e200: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
+0000e210: 756e 6374 696f 6e20 2866 756e 6374 696f  unction (functio
+0000e220: 6e2c 206f 7074 696f 6e61 6c29 3a20 5468  n, optional): Th
+0000e230: 6520 7374 7265 6e67 7468 2066 756e 6374  e strength funct
+0000e240: 696f 6e20 746f 2062 6520 7573 6564 2074  ion to be used t
+0000e250: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
+0000e260: 7374 7265 6e67 7468 206f 6620 6120 7061  strength of a pa
+0000e270: 7468 2e20 2020 5468 6520 6465 6661 756c  th.   The defaul
+0000e280: 7420 6973 2074 6865 206d 6172 6769 6e20  t is the margin 
+0000e290: 6d65 7468 6f64 206f 6620 6060 6564 6174  method of ``edat
+0000e2a0: 6160 602e 2020 2054 6869 7320 6f6e 6c79  a``.   This only
+0000e2b0: 206d 6174 7465 7273 2077 6865 6e20 7468   matters when th
+0000e2c0: 6520 6261 6c6c 6f74 7320 6172 6520 6e6f  e ballots are no
+0000e2d0: 7420 6c69 6e65 6172 206f 7264 6572 732e  t linear orders.
+0000e2e0: 200a 2020 2020 2020 2020 616c 676f 7269   .        algori
+0000e2f0: 7468 6d20 2873 7472 2c20 6f70 7469 6f6e  thm (str, option
+0000e300: 616c 293a 2053 7065 6369 6679 2077 6869  al): Specify whi
+0000e310: 6368 2061 6c67 6f72 6974 686d 2074 6f20  ch algorithm to 
+0000e320: 7573 652e 2020 4f70 7469 6f6e 7320 6172  use.  Options ar
+0000e330: 6520 2762 6173 6963 2720 2874 6865 2064  e 'basic' (the d
+0000e340: 6566 6175 6c74 2920 616e 6420 2777 6974  efault) and 'wit
+0000e350: 685f 636f 6e64 6f72 6365 745f 6368 6563  h_condorcet_chec
+0000e360: 6b27 2e0a 0a20 2020 2052 6574 7572 6e73  k'...    Returns
+0000e370: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
+0000e380: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
+0000e390: 6964 6174 6573 2e20 0a0a 2020 2020 2e2e  idates. ..    ..
+0000e3a0: 2073 6565 616c 736f 3a3a 0a0a 2020 2020   seealso::..    
+0000e3b0: 2020 2020 3a6d 6574 683a 6070 7265 665f      :meth:`pref_
+0000e3c0: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+0000e3d0: 7365 645f 6d65 7468 6f64 732e 7374 6162  sed_methods.stab
+0000e3e0: 6c65 5f76 6f74 696e 6760 0a0a 2020 2020  le_voting`..    
+0000e3f0: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
+0000e400: 2e2e 2065 7865 635f 636f 6465 3a3a 0a0a  .. exec_code::..
+0000e410: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+0000e420: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
+0000e430: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
+0000e440: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
+0000e450: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
+0000e460: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
+0000e470: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+0000e480: 6473 2069 6d70 6f72 7420 7369 6d70 6c65  ds import simple
+0000e490: 5f73 7461 626c 655f 766f 7469 6e67 0a0a  _stable_voting..
+0000e4a0: 2020 2020 2020 2020 6d67 203d 204d 6172          mg = Mar
+0000e4b0: 6769 6e47 7261 7068 285b 302c 2031 2c20  ginGraph([0, 1, 
+0000e4c0: 322c 2033 5d2c 205b 2830 2c20 332c 2038  2, 3], [(0, 3, 8
+0000e4d0: 292c 2028 312c 2030 2c20 3130 292c 2028  ), (1, 0, 10), (
+0000e4e0: 322c 2030 2c20 3429 2c20 2832 2c20 312c  2, 0, 4), (2, 1,
+0000e4f0: 2038 292c 2028 332c 2031 2c20 3829 5d29   8), (3, 1, 8)])
+0000e500: 0a0a 2020 2020 2020 2020 7369 6d70 6c65  ..        simple
+0000e510: 5f73 7461 626c 655f 766f 7469 6e67 2e64  _stable_voting.d
+0000e520: 6973 706c 6179 286d 6729 0a20 2020 2020  isplay(mg).     
+0000e530: 2020 2073 696d 706c 655f 7374 6162 6c65     simple_stable
+0000e540: 5f76 6f74 696e 672e 6469 7370 6c61 7928  _voting.display(
+0000e550: 6d67 2c20 616c 676f 7269 7468 6d3d 2762  mg, algorithm='b
+0000e560: 6173 6963 2729 0a20 2020 2020 2020 2073  asic').        s
+0000e570: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
+0000e580: 696e 672e 6469 7370 6c61 7928 6d67 2c20  ing.display(mg, 
+0000e590: 616c 676f 7269 7468 6d3d 2777 6974 685f  algorithm='with_
+0000e5a0: 636f 6e64 6f72 6365 745f 6368 6563 6b27  condorcet_check'
+0000e5b0: 290a 0a20 2020 2022 2222 0a20 2020 200a  )..    """.    .
+0000e5c0: 2020 2020 6966 2061 6c67 6f72 6974 686d      if algorithm
+0000e5d0: 203d 3d20 2762 6173 6963 273a 200a 2020   == 'basic': .  
+0000e5e0: 2020 2020 2020 7265 7475 726e 205f 7369        return _si
+0000e5f0: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
+0000e600: 6e67 5f62 6173 6963 2865 6461 7461 2c20  ng_basic(edata, 
+0000e610: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
+0000e620: 725f 6361 6e64 732c 2073 7472 656e 6774  r_cands, strengt
+0000e630: 685f 6675 6e63 7469 6f6e 203d 2073 7472  h_function = str
+0000e640: 656e 6774 685f 6675 6e63 7469 6f6e 290a  ength_function).
+0000e650: 2020 2020 656c 6966 2061 6c67 6f72 6974      elif algorit
+0000e660: 686d 203d 3d20 2777 6974 685f 636f 6e64  hm == 'with_cond
+0000e670: 6f72 6365 745f 6368 6563 6b27 3a0a 2020  orcet_check':.  
+0000e680: 2020 2020 2020 7265 7475 726e 205f 7369        return _si
+0000e690: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
+0000e6a0: 6e67 5f77 6974 685f 636f 6e64 6f72 6365  ng_with_condorce
+0000e6b0: 745f 6368 6563 6b28 6564 6174 612c 2063  t_check(edata, c
+0000e6c0: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
+0000e6d0: 5f63 616e 6473 2c20 7374 7265 6e67 7468  _cands, strength
+0000e6e0: 5f66 756e 6374 696f 6e20 3d20 7374 7265  _function = stre
+0000e6f0: 6e67 7468 5f66 756e 6374 696f 6e29 0a20  ngth_function). 
+0000e700: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000e710: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+0000e720: 7228 2249 6e76 616c 6964 2061 6c67 6f72  r("Invalid algor
+0000e730: 6974 686d 2073 7065 6369 6669 6564 2e22  ithm specified."
+0000e740: 290a 2020 2020 0a0a 6465 6620 5f73 7461  ).    ..def _sta
+0000e750: 626c 655f 766f 7469 6e67 2865 6461 7461  ble_voting(edata
+0000e760: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
+0000e770: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
+0000e780: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e790: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
+0000e7a0: 6e63 7469 6f6e 2c0a 2020 2020 2020 2020  nction,.        
+0000e7b0: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
+0000e7c0: 645f 6d61 7463 6865 732c 0a20 2020 2020  d_matches,.     
+0000e7d0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0000e7e0: 6d5f 7376 5f77 696e 6e65 7273 293a 200a  m_sv_winners): .
+0000e7f0: 2020 2020 2727 270a 2020 2020 4465 7465      '''.    Dete
+0000e800: 726d 696e 6520 7468 6520 5374 6162 6c65  rmine the Stable
+0000e810: 2056 6f74 696e 6720 7769 6e6e 6572 7320   Voting winners 
+0000e820: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
+0000e830: 7768 696c 6520 6b65 6570 696e 6720 7472  while keeping tr
+0000e840: 6163 6b20 6f66 2074 6865 2077 696e 6e65  ack of the winne
+0000e850: 7273 2069 6e20 616e 7920 7375 6270 726f  rs in any subpro
+0000e860: 6669 6c65 7320 6368 6563 6b65 6420 6475  files checked du
+0000e870: 7269 6e67 2063 6f6d 7075 7461 7469 6f6e  ring computation
+0000e880: 2e20 0a20 2020 2027 2727 0a20 2020 200a  . .    '''.    .
+0000e890: 2020 2020 7376 5f77 696e 6e65 7273 203d      sv_winners =
+0000e8a0: 206c 6973 7428 290a 2020 2020 0a20 2020   list().    .   
+0000e8b0: 2075 6e64 6566 6561 7465 645f 6361 6e64   undefeated_cand
+0000e8c0: 6964 6174 6573 203d 2073 706c 6974 5f63  idates = split_c
+0000e8d0: 7963 6c65 2865 6461 7461 2c20 6375 7272  ycle(edata, curr
+0000e8e0: 5f63 616e 6473 203d 2063 7572 725f 6361  _cands = curr_ca
+0000e8f0: 6e64 732c 2073 7472 656e 6774 685f 6675  nds, strength_fu
+0000e900: 6e63 7469 6f6e 203d 2073 7472 656e 6774  nction = strengt
+0000e910: 685f 6675 6e63 7469 6f6e 290a 0a20 2020  h_function)..   
+0000e920: 2069 6620 6c65 6e28 6375 7272 5f63 616e   if len(curr_can
+0000e930: 6473 2920 3d3d 2031 3a20 0a20 2020 2020  ds) == 1: .     
+0000e940: 2020 206d 656d 5f73 765f 7769 6e6e 6572     mem_sv_winner
+0000e950: 735b 7475 706c 6528 6375 7272 5f63 616e  s[tuple(curr_can
+0000e960: 6473 295d 203d 2063 7572 725f 6361 6e64  ds)] = curr_cand
+0000e970: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
+0000e980: 2063 7572 725f 6361 6e64 732c 206d 656d   curr_cands, mem
+0000e990: 5f73 765f 7769 6e6e 6572 730a 2020 2020  _sv_winners.    
+0000e9a0: 0a20 2020 206d 6172 6769 6e5f 7769 746e  .    margin_witn
+0000e9b0: 6573 7369 6e67 5f77 696e 203d 202d 6d61  essing_win = -ma
+0000e9c0: 7468 2e69 6e66 0a0a 2020 2020 666f 7220  th.inf..    for 
+0000e9d0: 612c 2062 2c20 7320 696e 2073 6f72 7465  a, b, s in sorte
+0000e9e0: 645f 6d61 7463 6865 733a 0a20 2020 2020  d_matches:.     
+0000e9f0: 2020 2069 6620 7320 3c20 6d61 7267 696e     if s < margin
+0000ea00: 5f77 6974 6e65 7373 696e 675f 7769 6e3a  _witnessing_win:
+0000ea10: 200a 2020 2020 2020 2020 2020 2020 6272   .            br
+0000ea20: 6561 6b0a 2020 2020 2020 2020 6966 2061  eak.        if a
+0000ea30: 2069 6e20 756e 6465 6665 6174 6564 5f63   in undefeated_c
+0000ea40: 616e 6469 6461 7465 7320 616e 6420 6120  andidates and a 
+0000ea50: 6e6f 7420 696e 2073 765f 7769 6e6e 6572  not in sv_winner
+0000ea60: 733a 200a 2020 2020 2020 2020 2020 2020  s: .            
+0000ea70: 6361 6e64 735f 6d69 6e75 735f 6220 3d20  cands_minus_b = 
+0000ea80: 5b63 2066 6f72 2063 2069 6e20 6375 7272  [c for c in curr
+0000ea90: 5f63 616e 6473 2069 6620 6320 213d 2062  _cands if c != b
+0000eaa0: 5d0a 2020 2020 2020 2020 2020 2020 6361  ].            ca
+0000eab0: 6e64 735f 6d69 6e75 735f 625f 6b65 7920  nds_minus_b_key 
+0000eac0: 3d20 7475 706c 6528 736f 7274 6564 2863  = tuple(sorted(c
+0000ead0: 616e 6473 5f6d 696e 7573 5f62 2929 0a20  ands_minus_b)). 
+0000eae0: 2020 2020 2020 2020 2020 2069 6620 6361             if ca
+0000eaf0: 6e64 735f 6d69 6e75 735f 625f 6b65 7920  nds_minus_b_key 
+0000eb00: 6e6f 7420 696e 206d 656d 5f73 765f 7769  not in mem_sv_wi
+0000eb10: 6e6e 6572 732e 6b65 7973 2829 3a20 0a20  nners.keys(): . 
+0000eb20: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000eb30: 732c 206d 656d 5f73 765f 7769 6e6e 6572  s, mem_sv_winner
+0000eb40: 7320 3d20 5f73 7461 626c 655f 766f 7469  s = _stable_voti
+0000eb50: 6e67 2865 6461 7461 2c0a 2020 2020 2020  ng(edata,.      
+0000eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb80: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+0000eb90: 7272 5f63 616e 6473 203d 2063 616e 6473  rr_cands = cands
+0000eba0: 5f6d 696e 7573 5f62 2c0a 2020 2020 2020  _minus_b,.      
+0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebd0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000ebe0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+0000ebf0: 3d20 7374 7265 6e67 7468 5f66 756e 6374  = strength_funct
+0000ec00: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+0000ec10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec30: 2020 2020 2020 2020 2073 6f72 7465 645f           sorted_
+0000ec40: 6d61 7463 6865 7320 3d20 5b28 612c 2063  matches = [(a, c
+0000ec50: 2c20 7329 2066 6f72 2061 2c20 632c 2073  , s) for a, c, s
+0000ec60: 2069 6e20 736f 7274 6564 5f6d 6174 6368   in sorted_match
+0000ec70: 6573 2069 6620 6120 213d 2062 2061 6e64  es if a != b and
+0000ec80: 2063 2021 3d20 625d 2c0a 2020 2020 2020   c != b],.      
+0000ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ecb0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0000ecc0: 6d5f 7376 5f77 696e 6e65 7273 203d 206d  m_sv_winners = m
+0000ecd0: 656d 5f73 765f 7769 6e6e 6572 7329 0a20  em_sv_winners). 
+0000ece0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000ecf0: 656d 5f73 765f 7769 6e6e 6572 735b 6361  em_sv_winners[ca
+0000ed00: 6e64 735f 6d69 6e75 735f 625f 6b65 795d  nds_minus_b_key]
+0000ed10: 203d 2077 730a 2020 2020 2020 2020 2020   = ws.          
+0000ed20: 2020 656c 7365 3a20 0a20 2020 2020 2020    else: .       
+0000ed30: 2020 2020 2020 2020 2077 7320 3d20 6d65           ws = me
+0000ed40: 6d5f 7376 5f77 696e 6e65 7273 5b63 616e  m_sv_winners[can
+0000ed50: 6473 5f6d 696e 7573 5f62 5f6b 6579 5d0a  ds_minus_b_key].
+0000ed60: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+0000ed70: 2069 6e20 7773 3a0a 2020 2020 2020 2020   in ws:.        
+0000ed80: 2020 2020 2020 2020 7376 5f77 696e 6e65          sv_winne
+0000ed90: 7273 2e61 7070 656e 6428 6129 0a20 2020  rs.append(a).   
+0000eda0: 2020 2020 2020 2020 2020 2020 206d 6172               mar
+0000edb0: 6769 6e5f 7769 746e 6573 7369 6e67 5f77  gin_witnessing_w
+0000edc0: 696e 203d 2073 0a20 2020 2020 2020 2020  in = s.         
+0000edd0: 2020 2020 2020 200a 2020 2020 7265 7475         .    retu
+0000ede0: 726e 2073 765f 7769 6e6e 6572 732c 206d  rn sv_winners, m
+0000edf0: 656d 5f73 765f 7769 6e6e 6572 730a 2020  em_sv_winners.  
+0000ee00: 2020 2020 2020 0a40 766d 286e 616d 6520        .@vm(name 
+0000ee10: 3d20 2253 7461 626c 6520 566f 7469 6e67  = "Stable Voting
+0000ee20: 2229 0a64 6566 205f 7374 6162 6c65 5f76  ").def _stable_v
+0000ee30: 6f74 696e 675f 7769 7468 5f63 6f6e 646f  oting_with_condo
+0000ee40: 7263 6574 5f63 6865 636b 280a 2020 2020  rcet_check(.    
+0000ee50: 6564 6174 612c 200a 2020 2020 6375 7272  edata, .    curr
+0000ee60: 5f63 616e 6473 3d4e 6f6e 652c 200a 2020  _cands=None, .  
+0000ee70: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+0000ee80: 696f 6e3d 4e6f 6e65 293a 200a 2020 2020  ion=None): .    
+0000ee90: 2222 220a 2020 2020 5374 6162 6c65 2056  """.    Stable V
+0000eea0: 6f74 696e 6720 6973 2043 6f6e 646f 7263  oting is Condorc
+0000eeb0: 6574 2063 6f6e 7369 7374 656e 742e 2020  et consistent.  
+0000eec0: 2049 7420 6973 2066 6173 7465 7220 746f   It is faster to
+0000eed0: 2073 6b69 7020 6578 6563 7574 696e 6720   skip executing 
+0000eee0: 7468 6520 7265 6375 7273 6976 6520 616c  the recursive al
+0000eef0: 676f 7269 7468 6d20 7768 656e 2074 6865  gorithm when the
+0000ef00: 7265 2069 7320 6120 436f 6e64 6f72 6365  re is a Condorce
+0000ef10: 7420 7769 6e6e 6572 2e20 200a 0a20 2020  t winner.  ..   
+0000ef20: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
+0000ef30: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
+0000ef40: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
+0000ef50: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
+0000ef60: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
+0000ef70: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
+0000ef80: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
+0000ef90: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
+0000efa0: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
+0000efb0: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
+0000efc0: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
+0000efd0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
+0000efe0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
+0000eff0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
+0000f000: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
+0000f010: 7360 600a 2020 2020 2020 2020 7374 7265  s``.        stre
+0000f020: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
+0000f030: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
+0000f040: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
+0000f050: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
+0000f060: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
+0000f070: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
+0000f080: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
+0000f090: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
+0000f0a0: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
+0000f0b0: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
+0000f0c0: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
+0000f0d0: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
+0000f0e0: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
+0000f0f0: 7264 6572 732e 200a 0a20 2020 2052 6574  rders. ..    Ret
+0000f100: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
+0000f110: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
+0000f120: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
+0000f130: 2020 2222 220a 2020 2020 6377 203d 2065    """.    cw = e
+0000f140: 6461 7461 2e63 6f6e 646f 7263 6574 5f77  data.condorcet_w
+0000f150: 696e 6e65 7228 6375 7272 5f63 616e 6473  inner(curr_cands
+0000f160: 203d 2063 7572 725f 6361 6e64 7329 0a20   = curr_cands). 
+0000f170: 2020 2069 6620 6377 2069 7320 6e6f 7420     if cw is not 
+0000f180: 4e6f 6e65 3a20 0a20 2020 2020 2020 2072  None: .        r
+0000f190: 6574 7572 6e20 5b63 775d 0a20 2020 2065  eturn [cw].    e
+0000f1a0: 6c73 653a 200a 2020 2020 2020 2020 6375  lse: .        cu
+0000f1b0: 7272 5f63 616e 6473 203d 2065 6461 7461  rr_cands = edata
+0000f1c0: 2e63 616e 6469 6461 7465 7320 6966 2063  .candidates if c
+0000f1d0: 7572 725f 6361 6e64 7320 6973 204e 6f6e  urr_cands is Non
+0000f1e0: 6520 656c 7365 2063 7572 725f 6361 6e64  e else curr_cand
+0000f1f0: 730a 2020 2020 2020 2020 7374 7265 6e67  s.        streng
+0000f200: 7468 5f66 756e 6374 696f 6e20 3d20 6564  th_function = ed
+0000f210: 6174 612e 6d61 7267 696e 2069 6620 7374  ata.margin if st
+0000f220: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+0000f230: 6973 204e 6f6e 6520 656c 7365 2073 7472  is None else str
+0000f240: 656e 6774 685f 6675 6e63 7469 6f6e 2020  ength_function  
+0000f250: 0a0a 2020 2020 2020 2020 6d61 7463 6865  ..        matche
+0000f260: 7320 3d20 5b28 612c 2062 2c20 7374 7265  s = [(a, b, stre
+0000f270: 6e67 7468 5f66 756e 6374 696f 6e28 612c  ngth_function(a,
+0000f280: 2062 2929 2066 6f72 2061 2069 6e20 6375   b)) for a in cu
+0000f290: 7272 5f63 616e 6473 2066 6f72 2062 2069  rr_cands for b i
+0000f2a0: 6e20 6375 7272 5f63 616e 6473 2069 6620  n curr_cands if 
+0000f2b0: 6120 213d 2062 5d0a 2020 2020 2020 2020  a != b].        
+0000f2c0: 736f 7274 6564 5f6d 6174 6368 6573 203d  sorted_matches =
+0000f2d0: 2073 6f72 7465 6428 6d61 7463 6865 732c   sorted(matches,
+0000f2e0: 2072 6576 6572 7365 3d54 7275 652c 206b   reverse=True, k
+0000f2f0: 6579 3d6c 616d 6264 6120 6d5f 775f 7765  ey=lambda m_w_we
+0000f300: 6967 6874 3a20 6d5f 775f 7765 6967 6874  ight: m_w_weight
+0000f310: 5b32 5d29 0a0a 2020 2020 2020 2020 7265  [2])..        re
+0000f320: 7475 726e 2073 6f72 7465 6428 5f73 7461  turn sorted(_sta
+0000f330: 626c 655f 766f 7469 6e67 2865 6461 7461  ble_voting(edata
+0000f340: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
+0000f350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f360: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
+0000f370: 7320 3d20 6375 7272 5f63 616e 6473 2c20  s = curr_cands, 
+0000f380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3a0: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
+0000f3b0: 6e63 7469 6f6e 203d 2073 7472 656e 6774  nction = strengt
+0000f3c0: 685f 6675 6e63 7469 6f6e 2c0a 2020 2020  h_function,.    
+0000f3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3f0: 736f 7274 6564 5f6d 6174 6368 6573 203d  sorted_matches =
+0000f400: 2073 6f72 7465 645f 6d61 7463 6865 732c   sorted_matches,
+0000f410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f430: 2020 2020 206d 656d 5f73 765f 7769 6e6e       mem_sv_winn
+0000f440: 6572 7320 3d20 7b7d 295b 305d 290a 0a64  ers = {})[0])..d
+0000f450: 6566 205f 7374 6162 6c65 5f76 6f74 696e  ef _stable_votin
+0000f460: 675f 6261 7369 6328 0a20 2020 2020 2020  g_basic(.       
+0000f470: 2065 6461 7461 2c20 0a20 2020 2020 2020   edata, .       
+0000f480: 2063 7572 725f 6361 6e64 7320 3d20 4e6f   curr_cands = No
+0000f490: 6e65 2c20 0a20 2020 2020 2020 2073 7472  ne, .        str
+0000f4a0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+0000f4b0: 204e 6f6e 6529 3a20 0a20 2020 2022 2222   None): .    """
+0000f4c0: 496d 706c 656d 656e 7461 7469 6f6e 206f  Implementation o
+0000f4d0: 6620 2053 7461 626c 6520 566f 7469 6e67  f  Stable Voting
+0000f4e0: 2066 726f 6d20 6874 7470 733a 2f2f 6172   from https://ar
+0000f4f0: 7869 762e 6f72 672f 6162 732f 3231 3038  xiv.org/abs/2108
+0000f500: 2e30 3035 3432 2e20 0a0a 2020 2020 4172  .00542. ..    Ar
+0000f510: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
+0000f520: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
+0000f530: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
+0000f540: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
+0000f550: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
+0000f560: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
+0000f570: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
+0000f580: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
+0000f590: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
+0000f5a0: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
+0000f5b0: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
+0000f5c0: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
+0000f5d0: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
+0000f5e0: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
+0000f5f0: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
+0000f600: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
+0000f610: 685f 6675 6e63 7469 6f6e 2028 6675 6e63  h_function (func
+0000f620: 7469 6f6e 2c20 6f70 7469 6f6e 616c 293a  tion, optional):
+0000f630: 2054 6865 2073 7472 656e 6774 6820 6675   The strength fu
+0000f640: 6e63 7469 6f6e 2074 6f20 6265 2075 7365  nction to be use
+0000f650: 6420 746f 2063 616c 6375 6c61 7465 2074  d to calculate t
+0000f660: 6865 2073 7472 656e 6774 6820 6f66 2061  he strength of a
+0000f670: 2070 6174 682e 2020 2054 6865 2064 6566   path.   The def
+0000f680: 6175 6c74 2069 7320 7468 6520 6d61 7267  ault is the marg
+0000f690: 696e 206d 6574 686f 6420 6f66 2060 6065  in method of ``e
+0000f6a0: 6461 7461 6060 2e20 2020 5468 6973 206f  data``.   This o
+0000f6b0: 6e6c 7920 6d61 7474 6572 7320 7768 656e  nly matters when
+0000f6c0: 2074 6865 2062 616c 6c6f 7473 2061 7265   the ballots are
+0000f6d0: 206e 6f74 206c 696e 6561 7220 6f72 6465   not linear orde
+0000f6e0: 7273 2e20 0a0a 2020 2020 5265 7475 726e  rs. ..    Return
+0000f6f0: 733a 200a 2020 2020 2020 2020 4120 736f  s: .        A so
+0000f700: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
+0000f710: 6469 6461 7465 732e 200a 0a20 2020 2022  didates. ..    "
+0000f720: 2222 0a0a 2020 2020 6375 7272 5f63 616e  ""..    curr_can
+0000f730: 6473 203d 2065 6461 7461 2e63 616e 6469  ds = edata.candi
+0000f740: 6461 7465 7320 6966 2063 7572 725f 6361  dates if curr_ca
+0000f750: 6e64 7320 6973 204e 6f6e 6520 656c 7365  nds is None else
+0000f760: 2063 7572 725f 6361 6e64 730a 2020 2020   curr_cands.    
+0000f770: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+0000f780: 6e20 3d20 6564 6174 612e 6d61 7267 696e  n = edata.margin
+0000f790: 2069 6620 7374 7265 6e67 7468 5f66 756e   if strength_fun
+0000f7a0: 6374 696f 6e20 6973 204e 6f6e 6520 656c  ction is None el
+0000f7b0: 7365 2073 7472 656e 6774 685f 6675 6e63  se strength_func
+0000f7c0: 7469 6f6e 2020 0a0a 2020 2020 6d61 7463  tion  ..    matc
+0000f7d0: 6865 7320 3d20 5b28 612c 2062 2c20 7374  hes = [(a, b, st
+0000f7e0: 7265 6e67 7468 5f66 756e 6374 696f 6e28  rength_function(
+0000f7f0: 612c 2062 2929 2066 6f72 2061 2069 6e20  a, b)) for a in 
+0000f800: 6375 7272 5f63 616e 6473 2066 6f72 2062  curr_cands for b
+0000f810: 2069 6e20 6375 7272 5f63 616e 6473 2069   in curr_cands i
+0000f820: 6620 6120 213d 2062 5d0a 2020 2020 736f  f a != b].    so
+0000f830: 7274 6564 5f6d 6174 6368 6573 203d 2073  rted_matches = s
+0000f840: 6f72 7465 6428 6d61 7463 6865 732c 2072  orted(matches, r
+0000f850: 6576 6572 7365 3d54 7275 652c 206b 6579  everse=True, key
+0000f860: 3d6c 616d 6264 6120 6d5f 775f 7765 6967  =lambda m_w_weig
+0000f870: 6874 3a20 6d5f 775f 7765 6967 6874 5b32  ht: m_w_weight[2
+0000f880: 5d29 0a0a 2020 2020 7265 7475 726e 2073  ])..    return s
+0000f890: 6f72 7465 6428 5f73 7461 626c 655f 766f  orted(_stable_vo
+0000f8a0: 7469 6e67 2865 6461 7461 2c20 0a20 2020  ting(edata, .   
+0000f8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8c0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+0000f8d0: 7272 5f63 616e 6473 203d 2063 7572 725f  rr_cands = curr_
+0000f8e0: 6361 6e64 732c 200a 2020 2020 2020 2020  cands, .        
+0000f8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f900: 2020 2020 2020 2020 2073 7472 656e 6774           strengt
+0000f910: 685f 6675 6e63 7469 6f6e 203d 2073 7472  h_function = str
+0000f920: 656e 6774 685f 6675 6e63 7469 6f6e 2c0a  ength_function,.
+0000f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f950: 2073 6f72 7465 645f 6d61 7463 6865 7320   sorted_matches 
+0000f960: 3d20 736f 7274 6564 5f6d 6174 6368 6573  = sorted_matches
+0000f970: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f990: 2020 206d 656d 5f73 765f 7769 6e6e 6572     mem_sv_winner
+0000f9a0: 7320 3d20 7b7d 295b 305d 290a 0a0a 0a40  s = {})[0])....@
+0000f9b0: 766d 286e 616d 6520 3d20 2253 7461 626c  vm(name = "Stabl
+0000f9c0: 6520 566f 7469 6e67 2229 0a64 6566 2073  e Voting").def s
+0000f9d0: 7461 626c 655f 766f 7469 6e67 280a 2020  table_voting(.  
+0000f9e0: 2020 6564 6174 612c 200a 2020 2020 6375    edata, .    cu
+0000f9f0: 7272 5f63 616e 6473 3d4e 6f6e 652c 200a  rr_cands=None, .
+0000fa00: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+0000fa10: 6374 696f 6e3d 4e6f 6e65 2c20 0a20 2020  ction=None, .   
+0000fa20: 2061 6c67 6f72 6974 686d 3d27 6261 7369   algorithm='basi
+0000fa30: 6327 293a 200a 2020 2020 2222 2249 6d70  c'): .    """Imp
+0000fa40: 6c65 6d65 6e74 6174 696f 6e20 6f66 2020  lementation of  
+0000fa50: 5374 6162 6c65 2056 6f74 696e 6720 6672  Stable Voting fr
+0000fa60: 6f6d 2068 7474 7073 3a2f 2f61 7278 6976  om https://arxiv
+0000fa70: 2e6f 7267 2f61 6273 2f32 3130 382e 3030  .org/abs/2108.00
+0000fa80: 3534 322e 200a 0a20 2020 2053 7461 626c  542. ..    Stabl
+0000fa90: 6520 566f 7469 6e67 2069 7320 6120 7265  e Voting is a re
+0000faa0: 6375 7273 6976 6520 766f 7469 6e67 206d  cursive voting m
+0000fab0: 6574 686f 6420 6465 6669 6e65 6420 6173  ethod defined as
+0000fac0: 2066 6f6c 6c6f 7773 3a20 0a0a 2020 2020   follows: ..    
+0000fad0: 312e 2020 4966 2074 6865 7265 2069 7320  1.  If there is 
+0000fae0: 6f6e 6c79 206f 6e65 2063 616e 6469 6461  only one candida
+0000faf0: 7465 2069 6e20 7468 6520 7072 6f66 696c  te in the profil
+0000fb00: 652c 2074 6865 6e20 7468 6174 2063 616e  e, then that can
+0000fb10: 6469 6461 7465 2069 7320 7468 6520 7769  didate is the wi
+0000fb20: 6e6e 6572 2e20 0a20 2020 2032 2e20 4f72  nner. .    2. Or
+0000fb30: 6465 7220 7468 6520 7061 6972 7320 3a6d  der the pairs :m
+0000fb40: 6174 683a 6028 612c 6229 6020 6f66 2063  ath:`(a,b)` of c
+0000fb50: 616e 6469 6461 7465 7320 6672 6f6d 206c  andidates from l
+0000fb60: 6172 6765 7374 2074 6f20 736d 616c 6c65  argest to smalle
+0000fb70: 7374 2076 616c 7565 206f 6620 7468 6520  st value of the 
+0000fb80: 6d61 7267 696e 206f 6620 3a6d 6174 683a  margin of :math:
+0000fb90: 6061 6020 6f76 6572 203a 6d61 7468 3a60  `a` over :math:`
+0000fba0: 6260 2073 7563 6820 7468 6174 203a 6d61  b` such that :ma
+0000fbb0: 7468 3a60 6160 2069 7320 756e 6465 6665  th:`a` is undefe
+0000fbc0: 6174 6564 2061 6363 6f72 6469 6e67 2074  ated according t
+0000fbd0: 6f20 5370 6c69 7420 4379 636c 652c 2061  o Split Cycle, a
+0000fbe0: 6e64 2064 6563 6c61 7265 2061 7320 5374  nd declare as St
+0000fbf0: 6162 6c65 2056 6f74 696e 6720 7769 6e6e  able Voting winn
+0000fc00: 6572 7320 7468 6520 6361 6e64 6964 6174  ers the candidat
+0000fc10: 6528 7329 203a 6d61 7468 3a60 6160 2066  e(s) :math:`a` f
+0000fc20: 726f 6d20 7468 6520 6561 726c 6965 7374  rom the earliest
+0000fc30: 2070 6169 7228 7329 203a 6d61 7468 3a60   pair(s) :math:`
+0000fc40: 2861 2c62 2960 2073 7563 6820 7468 6174  (a,b)` such that
+0000fc50: 203a 6d61 7468 3a60 6160 2069 7320 6120   :math:`a` is a 
+0000fc60: 5369 6d70 6c65 2053 7461 626c 6520 566f  Simple Stable Vo
+0000fc70: 7469 6e67 2077 696e 6e65 7220 696e 2074  ting winner in t
+0000fc80: 6865 2065 6c65 6374 696f 6e20 7769 7468  he election with
+0000fc90: 6f75 7420 3a6d 6174 683a 6062 602e 200a  out :math:`b`. .
+0000fca0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+0000fcb0: 2020 2065 6461 7461 2028 5072 6f66 696c     edata (Profil
+0000fcc0: 652c 2050 726f 6669 6c65 5769 7468 5469  e, ProfileWithTi
+0000fcd0: 6573 2c20 4d61 7267 696e 4772 6170 6829  es, MarginGraph)
+0000fce0: 3a20 416e 7920 656c 6563 7469 6f6e 2064  : Any election d
+0000fcf0: 6174 6120 7468 6174 2068 6173 2061 2060  ata that has a `
+0000fd00: 6d61 7267 696e 6020 6d65 7468 6f64 2e20  margin` method. 
+0000fd10: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
+0000fd20: 6e64 7320 284c 6973 745b 696e 745d 2c20  nds (List[int], 
+0000fd30: 6f70 7469 6f6e 616c 293a 2049 6620 7365  optional): If se
+0000fd40: 742c 2074 6865 6e20 6669 6e64 2074 6865  t, then find the
+0000fd50: 2077 696e 6e65 7273 2066 6f72 2074 6865   winners for the
+0000fd60: 2070 726f 6669 6c65 2072 6573 7472 6963   profile restric
+0000fd70: 7465 6420 746f 2074 6865 2063 616e 6469  ted to the candi
+0000fd80: 6461 7465 7320 696e 2060 6063 7572 725f  dates in ``curr_
+0000fd90: 6361 6e64 7360 600a 2020 2020 2020 2020  cands``.        
+0000fda0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+0000fdb0: 6e20 2866 756e 6374 696f 6e2c 206f 7074  n (function, opt
+0000fdc0: 696f 6e61 6c29 3a20 5468 6520 7374 7265  ional): The stre
+0000fdd0: 6e67 7468 2066 756e 6374 696f 6e20 746f  ngth function to
+0000fde0: 2062 6520 7573 6564 2074 6f20 6361 6c63   be used to calc
+0000fdf0: 756c 6174 6520 7468 6520 7374 7265 6e67  ulate the streng
+0000fe00: 7468 206f 6620 6120 7061 7468 2e20 2020  th of a path.   
+0000fe10: 5468 6520 6465 6661 756c 7420 6973 2074  The default is t
+0000fe20: 6865 206d 6172 6769 6e20 6d65 7468 6f64  he margin method
+0000fe30: 206f 6620 6060 6564 6174 6160 602e 2020   of ``edata``.  
+0000fe40: 2054 6869 7320 6f6e 6c79 206d 6174 7465   This only matte
+0000fe50: 7273 2077 6865 6e20 7468 6520 6261 6c6c  rs when the ball
+0000fe60: 6f74 7320 6172 6520 6e6f 7420 6c69 6e65  ots are not line
+0000fe70: 6172 206f 7264 6572 732e 200a 0a20 2020  ar orders. ..   
+0000fe80: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
+0000fe90: 2020 2041 2073 6f72 7465 6420 6c69 7374     A sorted list
+0000fea0: 206f 6620 6361 6e64 6964 6174 6573 2e20   of candidates. 
+0000feb0: 0a0a 2020 2020 2e2e 2073 6565 616c 736f  ..    .. seealso
+0000fec0: 3a3a 0a0a 2020 2020 2020 2020 3a6d 6574  ::..        :met
+0000fed0: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
+0000fee0: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+0000fef0: 6f64 732e 7369 6d70 6c65 5f73 7461 626c  ods.simple_stabl
+0000ff00: 655f 766f 7469 6e67 600a 0a0a 2020 2020  e_voting`...    
+0000ff10: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
+0000ff20: 2e2e 2065 7865 635f 636f 6465 3a3a 0a0a  .. exec_code::..
+0000ff30: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+0000ff40: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
+0000ff50: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
+0000ff60: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
+0000ff70: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
+0000ff80: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
+0000ff90: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+0000ffa0: 6473 2069 6d70 6f72 7420 7374 6162 6c65  ds import stable
+0000ffb0: 5f76 6f74 696e 670a 0a20 2020 2020 2020  _voting..       
+0000ffc0: 206d 6720 3d20 4d61 7267 696e 4772 6170   mg = MarginGrap
+0000ffd0: 6828 5b30 2c20 312c 2032 2c20 335d 2c20  h([0, 1, 2, 3], 
+0000ffe0: 5b28 302c 2033 2c20 3829 2c20 2831 2c20  [(0, 3, 8), (1, 
+0000fff0: 302c 2031 3029 2c20 2832 2c20 302c 2034  0, 10), (2, 0, 4
+00010000: 292c 2028 322c 2031 2c20 3829 2c20 2833  ), (2, 1, 8), (3
+00010010: 2c20 312c 2038 295d 290a 0a20 2020 2020  , 1, 8)])..     
+00010020: 2020 2073 7461 626c 655f 766f 7469 6e67     stable_voting
+00010030: 2e64 6973 706c 6179 286d 6729 0a20 2020  .display(mg).   
+00010040: 2020 2020 2073 7461 626c 655f 766f 7469       stable_voti
+00010050: 6e67 2e64 6973 706c 6179 286d 672c 2061  ng.display(mg, a
+00010060: 6c67 6f72 6974 686d 3d27 6261 7369 6327  lgorithm='basic'
+00010070: 290a 2020 2020 2020 2020 7374 6162 6c65  ).        stable
+00010080: 5f76 6f74 696e 672e 6469 7370 6c61 7928  _voting.display(
+00010090: 6d67 2c20 616c 676f 7269 7468 6d3d 2777  mg, algorithm='w
+000100a0: 6974 685f 636f 6e64 6f72 6365 745f 6368  ith_condorcet_ch
+000100b0: 6563 6b27 290a 0a20 2020 2022 2222 0a0a  eck')..    """..
+000100c0: 2020 2020 6966 2061 6c67 6f72 6974 686d      if algorithm
+000100d0: 203d 3d20 2762 6173 6963 273a 200a 2020   == 'basic': .  
+000100e0: 2020 2020 2020 7265 7475 726e 205f 7374        return _st
+000100f0: 6162 6c65 5f76 6f74 696e 675f 6261 7369  able_voting_basi
+00010100: 6328 6564 6174 612c 2063 7572 725f 6361  c(edata, curr_ca
+00010110: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
+00010120: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+00010130: 696f 6e20 3d20 7374 7265 6e67 7468 5f66  ion = strength_f
+00010140: 756e 6374 696f 6e29 0a20 2020 2065 6c69  unction).    eli
+00010150: 6620 616c 676f 7269 7468 6d20 3d3d 2027  f algorithm == '
+00010160: 7769 7468 5f63 6f6e 646f 7263 6574 5f63  with_condorcet_c
+00010170: 6865 636b 273a 0a20 2020 2020 2020 2072  heck':.        r
+00010180: 6574 7572 6e20 5f73 7461 626c 655f 766f  eturn _stable_vo
+00010190: 7469 6e67 5f77 6974 685f 636f 6e64 6f72  ting_with_condor
+000101a0: 6365 745f 6368 6563 6b28 6564 6174 612c  cet_check(edata,
+000101b0: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
+000101c0: 7272 5f63 616e 6473 2c20 7374 7265 6e67  rr_cands, streng
+000101d0: 7468 5f66 756e 6374 696f 6e20 3d20 7374  th_function = st
+000101e0: 7265 6e67 7468 5f66 756e 6374 696f 6e29  rength_function)
+000101f0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00010200: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00010210: 726f 7228 2249 6e76 616c 6964 2061 6c67  ror("Invalid alg
+00010220: 6f72 6974 686d 2073 7065 6369 6669 6564  orithm specified
+00010230: 2e22 290a 2020 2020 0a0a 0a0a 4076 6d28  .").    ....@vm(
+00010240: 6e61 6d65 3d22 4573 7365 6e74 6961 6c20  name="Essential 
+00010250: 5365 7422 290a 6465 6620 6573 7365 6e74  Set").def essent
+00010260: 6961 6c28 6564 6174 612c 2063 7572 725f  ial(edata, curr_
+00010270: 6361 6e64 7320 3d20 4e6f 6e65 2c20 7468  cands = None, th
+00010280: 7265 7368 6f6c 6420 3d20 302e 3030 3030  reshold = 0.0000
+00010290: 3030 3129 3a20 0a20 2020 2022 2222 5468  001): .    """Th
+000102a0: 6520 4573 7365 6e74 6961 6c20 5365 7420  e Essential Set 
+000102b0: 6973 2074 6865 2073 7570 706f 7274 206f  is the support o
+000102c0: 6620 7468 6520 2863 686f 7365 6e29 2043  f the (chosen) C
+000102d0: 3220 6d61 7869 6d61 6c20 6c6f 7474 6572  2 maximal lotter
+000102e0: 792e 0a0a 2020 2020 4172 6773 3a0a 2020  y...    Args:.  
+000102f0: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
+00010300: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
+00010310: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
+00010320: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
+00010330: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
+00010340: 6120 606d 6172 6769 6e5f 6d61 7472 6978  a `margin_matrix
+00010350: 6020 6174 7472 6962 7574 652e 0a20 2020  ` attribute..   
+00010360: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
+00010370: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
+00010380: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
+00010390: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
+000103a0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
+000103b0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
+000103c0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
+000103d0: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
+000103e0: 7360 600a 0a20 2020 2052 6574 7572 6e73  s``..    Returns
+000103f0: 3a0a 2020 2020 2020 2020 4120 736f 7274  :.        A sort
+00010400: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
+00010410: 6461 7465 732e 0a0a 2020 2020 2222 220a  dates...    """.
+00010420: 2020 2020 6d6c 203d 206d 6178 696d 616c      ml = maximal
+00010430: 5f6c 6f74 7465 7279 2865 6461 7461 2c20  _lottery(edata, 
+00010440: 6375 7272 5f63 616e 6473 3d63 7572 725f  curr_cands=curr_
+00010450: 6361 6e64 7329 0a0a 2020 2020 7265 7475  cands)..    retu
+00010460: 726e 2073 6f72 7465 6428 5b63 2066 6f72  rn sorted([c for
+00010470: 2063 2069 6e20 6d6c 2e6b 6579 7328 2920   c in ml.keys() 
+00010480: 6966 206d 6c5b 635d 203e 2074 6872 6573  if ml[c] > thres
+00010490: 686f 6c64 5d29 0a0a 4076 6d28 6e61 6d65  hold])..@vm(name
+000104a0: 3d22 5765 6967 6874 6564 2043 6f76 6572  ="Weighted Cover
+000104b0: 696e 6722 290a 6465 6620 7765 6967 6874  ing").def weight
+000104c0: 6564 5f63 6f76 6572 696e 6728 6564 6174  ed_covering(edat
+000104d0: 612c 2063 7572 725f 6361 6e64 733d 4e6f  a, curr_cands=No
+000104e0: 6e65 293a 200a 2020 2020 2222 2241 6363  ne): .    """Acc
+000104f0: 6f72 6469 6e67 2074 6f20 5765 6967 6874  ording to Weight
+00010500: 6564 2043 6f76 6572 696e 672c 2078 2064  ed Covering, x d
+00010510: 6566 6561 7473 2079 2069 6620 7468 6520  efeats y if the 
+00010520: 6d61 7267 696e 206f 6620 7820 6f76 6572  margin of x over
+00010530: 2079 2069 7320 706f 7369 7469 7665 2061   y is positive a
+00010540: 6e64 2066 6f72 2065 7665 7279 206f 7468  nd for every oth
+00010550: 6572 207a 2c20 7468 6520 6d61 7267 696e  er z, the margin
+00010560: 206f 6620 7820 6f76 6572 207a 2069 7320   of x over z is 
+00010570: 6772 6561 7465 7220 7468 616e 206f 7220  greater than or 
+00010580: 6571 7561 6c20 746f 2074 6865 206d 6172  equal to the mar
+00010590: 6769 6e20 6f66 2079 206f 7665 7220 7a2e  gin of y over z.
+000105a0: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
+000105b0: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
+000105c0: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
+000105d0: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
+000105e0: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
+000105f0: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
+00010600: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
+00010610: 2e0a 2020 2020 2020 2020 6375 7272 5f63  ..        curr_c
+00010620: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
+00010630: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
+00010640: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
+00010650: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
+00010660: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
+00010670: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
+00010680: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
+00010690: 5f63 616e 6473 6060 0a0a 2020 2020 5265  _cands``..    Re
+000106a0: 7475 726e 733a 0a20 2020 2020 2020 2041  turns:.        A
+000106b0: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
+000106c0: 6361 6e64 6964 6174 6573 2e0a 0a20 2020  candidates...   
+000106d0: 202e 2e20 6e6f 7465 3a3a 0a20 2020 2020   .. note::.     
+000106e0: 2020 2053 6565 2c20 652e 672e 2c20 4268     See, e.g., Bh
+000106f0: 6173 6b61 7220 4475 7474 6120 616e 6420  askar Dutta and 
+00010700: 4a65 616e 2d46 7261 6e63 6f69 7320 4c61  Jean-Francois La
+00010710: 736c 6965 722c 2022 436f 6d70 6172 6973  slier, "Comparis
+00010720: 6f6e 2066 756e 6374 696f 6e73 2061 6e64  on functions and
+00010730: 2063 686f 6963 6520 636f 7272 6573 706f   choice correspo
+00010740: 6e64 656e 6365 732c 2220 536f 6369 616c  ndences," Social
+00010750: 2043 686f 6963 6520 616e 6420 5765 6c66   Choice and Welf
+00010760: 6172 652c 2031 363a 3531 33e2 8093 3533  are, 16:513...53
+00010770: 322c 2031 3939 392c 2064 6f69 3a31 302e  2, 1999, doi:10.
+00010780: 3130 3037 2f73 3030 3335 3530 3035 3031  1007/s0035500501
+00010790: 3538 2c20 616e 6420 5261 75cc 816c 2050  58, and Rau..l P
+000107a0: 65cc 8172 657a 2d46 6572 6e61 cc81 6e64  e..rez-Ferna..nd
+000107b0: 657a 2061 6e64 2042 6572 6e61 7264 2044  ez and Bernard D
+000107c0: 6520 4261 6574 732c 2022 5468 6520 7375  e Baets, "The su
+000107d0: 7065 7263 6f76 6572 696e 6720 7265 6c61  percovering rela
+000107e0: 7469 6f6e 2c20 7468 6520 7061 6972 7769  tion, the pairwi
+000107f0: 7365 2077 696e 6e65 722c 2061 6e64 206d  se winner, and m
+00010800: 6f72 6520 6d69 7373 696e 6720 6c69 6e6b  ore missing link
+00010810: 7320 6265 7477 6565 6e20 426f 7264 6120  s between Borda 
+00010820: 616e 6420 436f 6e64 6f72 6365 742c 2220  and Condorcet," 
+00010830: 536f 6369 616c 2043 686f 6963 6520 616e  Social Choice an
+00010840: 6420 5765 6c66 6172 652c 2035 303a 3332  d Welfare, 50:32
+00010850: 39e2 8093 3335 322c 2032 3031 382c 2064  9...352, 2018, d
+00010860: 6f69 3a31 302e 3130 3037 2f73 3030 3335  oi:10.1007/s0035
+00010870: 352d 3031 372d 3130 3836 2d30 2e0a 2020  5-017-1086-0..  
+00010880: 2020 2222 220a 0a20 2020 2063 616e 6469    """..    candi
+00010890: 6461 7465 7320 3d20 6564 6174 612e 6361  dates = edata.ca
+000108a0: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
+000108b0: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
+000108c0: 6c73 6520 6375 7272 5f63 616e 6473 0a0a  lse curr_cands..
+000108d0: 2020 2020 646f 6d20 3d20 7b63 3a20 7365      dom = {c: se
+000108e0: 7428 6564 6174 612e 646f 6d69 6e61 746f  t(edata.dominato
+000108f0: 7273 2863 2c20 6375 7272 5f63 616e 6473  rs(c, curr_cands
+00010900: 203d 2063 7572 725f 6361 6e64 7329 2920   = curr_cands)) 
+00010910: 666f 7220 6320 696e 2063 616e 6469 6461  for c in candida
+00010920: 7465 737d 0a20 2020 2075 635f 7365 7420  tes}.    uc_set 
+00010930: 3d20 6c69 7374 2829 0a0a 2020 2020 666f  = list()..    fo
+00010940: 7220 7920 696e 2063 616e 6469 6461 7465  r y in candidate
+00010950: 733a 0a20 2020 2020 2020 2069 735f 696e  s:.        is_in
+00010960: 5f75 6373 203d 2054 7275 650a 2020 2020  _ucs = True.    
+00010970: 2020 2020 666f 7220 7820 696e 2065 6461      for x in eda
+00010980: 7461 2e64 6f6d 696e 6174 6f72 7328 792c  ta.dominators(y,
+00010990: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
+000109a0: 7272 5f63 616e 6473 293a 0a20 2020 2020  rr_cands):.     
+000109b0: 2020 2020 2020 2023 2063 6865 636b 2069         # check i
+000109c0: 6620 7920 636f 7665 7273 2078 2c20 692e  f y covers x, i.
+000109d0: 652e 2c20 666f 7220 6576 6572 7920 7a2c  e., for every z,
+000109e0: 206d 6172 6769 6e28 782c 207a 2920 3e3d   margin(x, z) >=
+000109f0: 206d 6172 6769 6e28 792c 207a 290a 2020   margin(y, z).  
+00010a00: 2020 2020 2020 2020 2020 636f 7665 7273            covers
+00010a10: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
+00010a20: 2020 2020 666f 7220 7a20 696e 2063 616e      for z in can
+00010a30: 6469 6461 7465 733a 0a20 2020 2020 2020  didates:.       
+00010a40: 2020 2020 2020 2020 2069 6620 6564 6174           if edat
+00010a50: 612e 6d61 7267 696e 2878 2c20 7a29 203c  a.margin(x, z) <
+00010a60: 2065 6461 7461 2e6d 6172 6769 6e28 792c   edata.margin(y,
+00010a70: 207a 293a 0a20 2020 2020 2020 2020 2020   z):.           
+00010a80: 2020 2020 2020 2020 2063 6f76 6572 7320           covers 
+00010a90: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+00010aa0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00010ab0: 6b0a 2020 2020 2020 2020 2020 0a20 2020  k.          .   
+00010ac0: 2020 2020 2020 2020 2069 6620 636f 7665           if cove
+00010ad0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+00010ae0: 2020 2020 6973 5f69 6e5f 7563 7320 3d20      is_in_ucs = 
+00010af0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00010b00: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
+00010b10: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00010b20: 2020 2020 2069 6620 6973 5f69 6e5f 7563       if is_in_uc
+00010b30: 733a 0a20 2020 2020 2020 2020 2020 2075  s:.            u
+00010b40: 635f 7365 742e 6170 7065 6e64 2879 290a  c_set.append(y).
+00010b50: 0a20 2020 2072 6574 7572 6e20 736f 7274  .    return sort
+00010b60: 6564 2875 635f 7365 7429 0a0a 4076 6d28  ed(uc_set)..@vm(
+00010b70: 6e61 6d65 203d 2022 4c6f 7373 2d54 7269  name = "Loss-Tri
+00010b80: 6d6d 6572 2056 6f74 696e 6722 290a 6465  mmer Voting").de
+00010b90: 6620 6c6f 7373 5f74 7269 6d6d 6572 2865  f loss_trimmer(e
+00010ba0: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
+00010bb0: 203d 204e 6f6e 6529 3a0a 2020 2020 2222   = None):.    ""
+00010bc0: 2249 7465 7261 7469 7665 6c79 2065 6c69  "Iteratively eli
+00010bd0: 6d69 6e61 7465 2074 6865 2063 616e 6469  minate the candi
+00010be0: 6461 7465 2077 6974 6820 7468 6520 6c61  date with the la
+00010bf0: 7267 6573 7420 7375 6d20 6f66 206d 6172  rgest sum of mar
+00010c00: 6769 6e73 206f 6620 6c6f 7373 2075 6e74  gins of loss unt
+00010c10: 696c 2061 2043 6f6e 646f 7263 6574 2077  il a Condorcet w
+00010c20: 696e 6e65 7220 6973 2066 6f75 6e64 2e20  inner is found. 
+00010c30: 496e 2074 6869 7320 7665 7273 696f 6e20  In this version 
+00010c40: 6f66 2074 6865 206d 6574 686f 642c 2070  of the method, p
+00010c50: 6172 616c 6c65 6c2d 756e 6976 6572 7365  arallel-universe
+00010c60: 2074 6965 6272 6561 6b69 6e67 2069 7320   tiebreaking is 
+00010c70: 7573 6564 2069 6620 7468 6572 6520 6172  used if there ar
+00010c80: 6520 6d75 6c74 6970 6c65 2063 616e 6469  e multiple candi
+00010c90: 6461 7465 7320 7769 7468 2074 6865 206c  dates with the l
+00010ca0: 6172 6765 7374 2073 756d 206f 6620 6d61  argest sum of ma
+00010cb0: 7267 696e 7320 6f66 206c 6f73 732e 0a0a  rgins of loss...
+00010cc0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00010cd0: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
+00010ce0: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
+00010cf0: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
+00010d00: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
+00010d10: 7461 2074 6861 7420 6861 7320 6120 6d61  ta that has a ma
+00010d20: 7267 696e 206d 6574 686f 642e 0a20 2020  rgin method..   
+00010d30: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
+00010d40: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
+00010d50: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
+00010d60: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
+00010d70: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
+00010d80: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
+00010d90: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
+00010da0: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
+00010db0: 7360 600a 0a20 2020 2052 6574 7572 6e73  s``..    Returns
+00010dc0: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
+00010dd0: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
+00010de0: 6964 6174 6573 0a0a 2020 2020 2e2e 206e  idates..    .. n
+00010df0: 6f74 653a 3a0a 2020 2020 2020 2020 4d65  ote::.        Me
+00010e00: 7468 6f64 2070 726f 706f 7365 6420 6279  thod proposed by
+00010e10: 2052 6963 6861 7264 2042 2e20 4461 726c   Richard B. Darl
+00010e20: 696e 6774 6f6e 2069 6e20 2254 6865 2043  ington in "The C
+00010e30: 6173 6520 666f 7220 7468 6520 4c6f 7373  ase for the Loss
+00010e40: 2d54 7269 6d6d 6572 2056 6f74 696e 6720  -Trimmer Voting 
+00010e50: 5379 7374 656d 2e22 0a0a 2020 2020 2222  System."..    ""
+00010e60: 220a 0a20 2020 2063 7572 725f 6361 6e64  "..    curr_cand
+00010e70: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
+00010e80: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
+00010e90: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
+00010ea0: 6375 7272 5f63 616e 6473 0a0a 2020 2020  curr_cands..    
+00010eb0: 7765 616b 5f63 7720 3d20 6564 6174 612e  weak_cw = edata.
+00010ec0: 7765 616b 5f63 6f6e 646f 7263 6574 5f77  weak_condorcet_w
+00010ed0: 696e 6e65 7228 6375 7272 5f63 616e 6473  inner(curr_cands
+00010ee0: 203d 2063 7572 725f 6361 6e64 7329 0a20   = curr_cands). 
+00010ef0: 2020 2023 2049 6620 7468 6572 6520 6172     # If there ar
+00010f00: 6520 7765 616b 2043 6f6e 646f 7263 6574  e weak Condorcet
+00010f10: 2077 696e 6e65 7273 2c20 7265 7475 726e   winners, return
+00010f20: 2074 686f 7365 2063 616e 6469 6461 7465   those candidate
+00010f30: 730a 2020 2020 6966 2065 6461 7461 2e77  s.    if edata.w
+00010f40: 6561 6b5f 636f 6e64 6f72 6365 745f 7769  eak_condorcet_wi
+00010f50: 6e6e 6572 2863 7572 725f 6361 6e64 7320  nner(curr_cands 
+00010f60: 3d20 6375 7272 5f63 616e 6473 2920 6973  = curr_cands) is
+00010f70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00010f80: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
+00010f90: 2877 6561 6b5f 6377 290a 2020 2020 0a20  (weak_cw).    . 
+00010fa0: 2020 2023 204f 7468 6572 7769 7365 2c20     # Otherwise, 
+00010fb0: 6361 6c63 756c 6174 6520 7468 6520 7375  calculate the su
+00010fc0: 6d20 6f66 206d 6172 6769 6e73 206f 6620  m of margins of 
+00010fd0: 6c6f 7373 2066 6f72 2065 6163 6820 6361  loss for each ca
+00010fe0: 6e64 6964 6174 650a 2020 2020 7375 6d5f  ndidate.    sum_
+00010ff0: 6f66 5f6d 6172 6769 6e73 5f6f 665f 6c6f  of_margins_of_lo
+00011000: 7373 203d 207b 6361 6e64 3a20 7375 6d28  ss = {cand: sum(
+00011010: 5b65 6461 7461 2e6d 6172 6769 6e28 6f74  [edata.margin(ot
+00011020: 6865 725f 6361 6e64 2c20 6361 6e64 2920  her_cand, cand) 
+00011030: 666f 7220 6f74 6865 725f 6361 6e64 2069  for other_cand i
+00011040: 6e20 6375 7272 5f63 616e 6473 2069 6620  n curr_cands if 
+00011050: 6564 6174 612e 6d61 7267 696e 286f 7468  edata.margin(oth
+00011060: 6572 5f63 616e 642c 2063 616e 6429 203e  er_cand, cand) >
+00011070: 2030 5d29 2066 6f72 2063 616e 6420 696e   0]) for cand in
+00011080: 2063 7572 725f 6361 6e64 737d 0a0a 2020   curr_cands}..  
+00011090: 2020 2320 4669 6e64 2074 6865 2063 616e    # Find the can
+000110a0: 6469 6461 7465 7320 7769 7468 2074 6865  didates with the
+000110b0: 206c 6172 6765 7374 2073 756d 206f 6620   largest sum of 
+000110c0: 6d61 7267 696e 7320 6f66 206c 6f73 730a  margins of loss.
+000110d0: 2020 2020 6d61 785f 7375 6d5f 6f66 5f6d      max_sum_of_m
+000110e0: 6172 6769 6e73 5f6f 665f 6c6f 7373 203d  argins_of_loss =
+000110f0: 206d 6178 2873 756d 5f6f 665f 6d61 7267   max(sum_of_marg
+00011100: 696e 735f 6f66 5f6c 6f73 732e 7661 6c75  ins_of_loss.valu
+00011110: 6573 2829 290a 2020 2020 6269 6767 6573  es()).    bigges
+00011120: 745f 6c6f 7365 7273 203d 205b 6361 6e64  t_losers = [cand
+00011130: 2066 6f72 2063 616e 6420 696e 2063 7572   for cand in cur
+00011140: 725f 6361 6e64 7320 6966 2073 756d 5f6f  r_cands if sum_o
+00011150: 665f 6d61 7267 696e 735f 6f66 5f6c 6f73  f_margins_of_los
+00011160: 735b 6361 6e64 5d20 3d3d 206d 6178 5f73  s[cand] == max_s
+00011170: 756d 5f6f 665f 6d61 7267 696e 735f 6f66  um_of_margins_of
+00011180: 5f6c 6f73 735d 0a0a 2020 2020 7769 6e6e  _loss]..    winn
+00011190: 6572 7320 3d20 5b5d 0a0a 2020 2020 2320  ers = []..    # 
+000111a0: 466f 7220 6561 6368 2062 6967 6765 7374  For each biggest
+000111b0: 206c 6f73 6572 2c20 6361 6c63 756c 6174   loser, calculat
+000111c0: 6520 7468 6520 7769 6e6e 6572 7320 6166  e the winners af
+000111d0: 7465 7220 7265 6d6f 7669 6e67 2074 6861  ter removing tha
+000111e0: 7420 6361 6e64 6964 6174 652e 2054 6865  t candidate. The
+000111f0: 2075 6e69 6f6e 206f 6620 7468 6573 6520   union of these 
+00011200: 7365 7473 2069 7320 7468 6520 7365 7420  sets is the set 
+00011210: 6f66 2077 696e 6e65 7273 2e0a 2020 2020  of winners..    
+00011220: 666f 7220 626c 2069 6e20 6269 6767 6573  for bl in bigges
+00011230: 745f 6c6f 7365 7273 3a0a 2020 2020 2020  t_losers:.      
+00011240: 2020 7769 6e6e 6572 735f 7769 7468 6f75    winners_withou
+00011250: 745f 626c 203d 206c 6f73 735f 7472 696d  t_bl = loss_trim
+00011260: 6d65 7228 6564 6174 612c 2063 7572 725f  mer(edata, curr_
+00011270: 6361 6e64 7320 3d20 5b63 616e 6420 666f  cands = [cand fo
+00011280: 7220 6361 6e64 2069 6e20 6375 7272 5f63  r cand in curr_c
+00011290: 616e 6473 2069 6620 6361 6e64 2021 3d20  ands if cand != 
+000112a0: 626c 5d29 0a20 2020 2020 2020 2077 696e  bl]).        win
+000112b0: 6e65 7273 202b 3d20 7769 6e6e 6572 735f  ners += winners_
+000112c0: 7769 7468 6f75 745f 626c 0a0a 2020 2020  without_bl..    
+000112d0: 7265 7475 726e 2073 6f72 7465 6428 6c69  return sorted(li
+000112e0: 7374 2873 6574 2877 696e 6e65 7273 2929  st(set(winners))
+000112f0: 290a 0a0a 6465 6620 6469 7374 616e 6365  )...def distance
+00011300: 5f74 6f5f 6d61 7267 696e 5f67 7261 7068  _to_margin_graph
+00011310: 2865 6461 7461 2c20 7265 6c2c 2065 7870  (edata, rel, exp
+00011320: 203d 2031 2c20 6375 7272 5f63 616e 6473   = 1, curr_cands
+00011330: 203d 204e 6f6e 6529 3a20 0a20 2020 2022   = None): .    "
+00011340: 2222 0a20 2020 2043 616c 6375 6c61 7465  "".    Calculate
+00011350: 2074 6865 2064 6973 7461 6e63 6520 6f66   the distance of
+00011360: 2060 6072 656c 6060 2028 6120 7265 6c61   ``rel`` (a rela
+00011370: 7469 6f6e 2920 746f 2074 6865 206d 616a  tion) to the maj
+00011380: 6f72 6974 7920 6772 6170 6820 6f66 2060  ority graph of `
+00011390: 6065 6461 7461 6060 2e20 0a20 2020 2022  `edata``. .    "
+000113a0: 2222 0a20 2020 2063 616e 6469 6461 7465  "".    candidate
+000113b0: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
+000113c0: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
+000113d0: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
+000113e0: 6375 7272 5f63 616e 6473 0a20 2020 200a  curr_cands.    .
+000113f0: 2020 2020 6966 2074 7970 6528 6564 6174      if type(edat
+00011400: 6129 203d 3d20 4d61 6a6f 7269 7479 4772  a) == MajorityGr
+00011410: 6170 6820 616e 6420 6578 7020 3d3d 2030  aph and exp == 0
+00011420: 3a0a 2020 2020 2020 2020 2320 6966 2065  :.        # if e
+00011430: 6461 7461 2069 7320 6120 4d61 6a6f 7269  data is a Majori
+00011440: 7479 4772 6170 682c 2077 6520 6e65 6564  tyGraph, we need
+00011450: 2074 6f20 6164 6420 6d61 7267 696e 7320   to add margins 
+00011460: 666f 7220 7468 6520 666f 6c6c 6f77 696e  for the followin
+00011470: 6720 636f 6465 2074 6f20 776f 726b 2e20  g code to work. 
+00011480: 2054 6865 206d 6172 6769 6e73 2064 6f20   The margins do 
+00011490: 6e6f 7420 6d61 7474 6572 2077 6865 6e20  not matter when 
+000114a0: 6578 703d 3d30 2e20 2020 0a20 2020 2020  exp==0.   .     
+000114b0: 2020 2065 6461 7461 203d 204d 6172 6769     edata = Margi
+000114c0: 6e47 7261 7068 2863 616e 6469 6461 7465  nGraph(candidate
+000114d0: 732c 205b 2863 312c 2063 322c 2031 2920  s, [(c1, c2, 1) 
+000114e0: 666f 7220 6331 2c20 6332 2069 6e20 6564  for c1, c2 in ed
+000114f0: 6174 612e 6564 6765 7320 6966 2028 6331  ata.edges if (c1
+00011500: 2069 6e20 6361 6e64 6964 6174 6573 2061   in candidates a
+00011510: 6e64 2063 3220 696e 2063 616e 6469 6461  nd c2 in candida
+00011520: 7465 7329 5d29 0a20 2020 2070 656e 616c  tes)]).    penal
+00011530: 7479 203d 2030 0a20 2020 2066 6f72 2061  ty = 0.    for a
+00011540: 2c62 2069 6e20 636f 6d62 696e 6174 696f  ,b in combinatio
+00011550: 6e73 2863 616e 6469 6461 7465 732c 2032  ns(candidates, 2
+00011560: 293a 200a 2020 2020 2020 2020 6966 2065  ): .        if e
+00011570: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
+00011580: 6566 6572 7328 612c 2062 2920 616e 6420  efers(a, b) and 
+00011590: 2862 2c61 2920 696e 2072 656c 3a20 0a20  (b,a) in rel: . 
+000115a0: 2020 2020 2020 2020 2020 2070 656e 616c             penal
+000115b0: 7479 202b 3d20 2865 6461 7461 2e6d 6172  ty += (edata.mar
+000115c0: 6769 6e28 612c 2062 2920 2a2a 2065 7870  gin(a, b) ** exp
+000115d0: 290a 2020 2020 2020 2020 656c 6966 2065  ).        elif e
+000115e0: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
+000115f0: 6566 6572 7328 622c 2061 2920 616e 6420  efers(b, a) and 
+00011600: 2861 2c62 2920 696e 2072 656c 3a20 0a20  (a,b) in rel: . 
+00011610: 2020 2020 2020 2020 2020 2070 656e 616c             penal
+00011620: 7479 202b 3d20 2865 6461 7461 2e6d 6172  ty += (edata.mar
+00011630: 6769 6e28 622c 2061 2920 2a2a 2065 7870  gin(b, a) ** exp
+00011640: 290a 2020 2020 2020 2020 656c 6966 2065  ).        elif e
+00011650: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
+00011660: 6566 6572 7328 612c 2062 2920 616e 6420  efers(a, b) and 
+00011670: 2861 2c62 2920 6e6f 7420 696e 2072 656c  (a,b) not in rel
+00011680: 2061 6e64 2028 622c 6129 206e 6f74 2069   and (b,a) not i
+00011690: 6e20 7265 6c3a 200a 2020 2020 2020 2020  n rel: .        
+000116a0: 2020 2020 7065 6e61 6c74 7920 2b3d 2028      penalty += (
+000116b0: 6564 6174 612e 6d61 7267 696e 2861 2c20  edata.margin(a, 
+000116c0: 6229 202a 2a20 6578 7029 202f 2032 200a  b) ** exp) / 2 .
+000116d0: 2020 2020 2020 2020 656c 6966 2065 6461          elif eda
+000116e0: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+000116f0: 6572 7328 622c 2061 2920 616e 6420 2861  ers(b, a) and (a
+00011700: 2c62 2920 6e6f 7420 696e 2072 656c 2061  ,b) not in rel a
+00011710: 6e64 2028 622c 6129 206e 6f74 2069 6e20  nd (b,a) not in 
+00011720: 7265 6c3a 200a 2020 2020 2020 2020 2020  rel: .          
+00011730: 2020 7065 6e61 6c74 7920 2b3d 2028 6564    penalty += (ed
+00011740: 6174 612e 6d61 7267 696e 2862 2c20 6129  ata.margin(b, a)
+00011750: 202a 2a20 6578 7029 2020 2f20 320a 2020   ** exp)  / 2.  
+00011760: 2020 7265 7475 726e 2070 656e 616c 7479    return penalty
+00011770: 0a0a 0a6d 675f 766d 7320 3d20 5b0a 2020  ...mg_vms = [.  
+00011780: 2020 6d69 6e69 6d61 782c 200a 2020 2020    minimax, .    
+00011790: 7370 6c69 745f 6379 636c 652c 0a20 2020  split_cycle,.   
+000117a0: 2023 6265 6174 5f70 6174 682c 0a20 2020   #beat_path,.   
+000117b0: 2023 7261 6e6b 6564 5f70 6169 7273 2c0a   #ranked_pairs,.
+000117c0: 2020 2020 2372 616e 6b65 645f 7061 6972      #ranked_pair
+000117d0: 735f 7769 7468 5f74 6573 742c 0a20 2020  s_with_test,.   
+000117e0: 2072 616e 6b65 645f 7061 6972 735f 7a74   ranked_pairs_zt
+000117f0: 2c0a 2020 2020 7261 6e6b 6564 5f70 6169  ,.    ranked_pai
+00011800: 7273 5f74 622c 0a20 2020 2023 7269 7665  rs_tb,.    #rive
+00011810: 722c 0a20 2020 2023 7269 7665 725f 7769  r,.    #river_wi
+00011820: 7468 5f74 6573 742c 200a 2020 2020 7369  th_test, .    si
+00011830: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
+00011840: 6e67 2c0a 2020 2020 7374 6162 6c65 5f76  ng,.    stable_v
+00011850: 6f74 696e 672c 0a20 2020 2065 7373 656e  oting,.    essen
+00011860: 7469 616c 2c0a 2020 2020 7765 6967 6874  tial,.    weight
+00011870: 6564 5f63 6f76 6572 696e 672c 0a20 2020  ed_covering,.   
+00011880: 206c 6f73 735f 7472 696d 6d65 720a 5d0a   loss_trimmer.].
+00011890: 0a0a 6d67 5f76 6d73 5f61 6c6c 203d 205b  ..mg_vms_all = [
+000118a0: 0a20 2020 206d 696e 696d 6178 2c20 0a20  .    minimax, . 
+000118b0: 2020 2073 706c 6974 5f63 7963 6c65 2c0a     split_cycle,.
+000118c0: 2020 2020 6265 6174 5f70 6174 682c 0a20      beat_path,. 
+000118d0: 2020 2072 616e 6b65 645f 7061 6972 732c     ranked_pairs,
+000118e0: 0a20 2020 2072 616e 6b65 645f 7061 6972  .    ranked_pair
+000118f0: 735f 7769 7468 5f74 6573 742c 0a20 2020  s_with_test,.   
+00011900: 2072 616e 6b65 645f 7061 6972 735f 7a74   ranked_pairs_zt
+00011910: 2c0a 2020 2020 7261 6e6b 6564 5f70 6169  ,.    ranked_pai
+00011920: 7273 5f74 622c 0a20 2020 2072 6976 6572  rs_tb,.    river
+00011930: 2c0a 2020 2020 7269 7665 725f 7769 7468  ,.    river_with
+00011940: 5f74 6573 742c 200a 2020 2020 7369 6d70  _test, .    simp
+00011950: 6c65 5f73 7461 626c 655f 766f 7469 6e67  le_stable_voting
+00011960: 2c0a 2020 2020 7374 6162 6c65 5f76 6f74  ,.    stable_vot
+00011970: 696e 672c 0a20 2020 2065 7373 656e 7469  ing,.    essenti
+00011980: 616c 2c0a 2020 2020 7765 6967 6874 6564  al,.    weighted
+00011990: 5f63 6f76 6572 696e 672c 0a20 2020 206c  _covering,.    l
+000119a0: 6f73 735f 7472 696d 6d65 720a 5d         oss_trimmer.]
```

### Comparing `pref_voting-1.1.0/pref_voting/margin_based_methods_old.py` & `pref_voting-1.1.1/pref_voting/margin_based_methods_old.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/monotonicity_axioms.py` & `pref_voting-1.1.1/pref_voting/monotonicity_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/other_methods.py` & `pref_voting-1.1.1/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/prob_voting_method.py` & `pref_voting-1.1.1/pref_voting/prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/probabilistic_methods.py` & `pref_voting-1.1.1/pref_voting/probabilistic_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/profiles.py` & `pref_voting-1.1.1/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/profiles_with_ties.py` & `pref_voting-1.1.1/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/rankings.py` & `pref_voting-1.1.1/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/scoring_methods.py` & `pref_voting-1.1.1/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/social_welfare_function.py` & `pref_voting-1.1.1/pref_voting/social_welfare_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/spatial_profiles.py` & `pref_voting-1.1.1/pref_voting/spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/strategic_axioms.py` & `pref_voting-1.1.1/pref_voting/strategic_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/conftest.py` & `pref_voting-1.1.1/pref_voting/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_c1_methods.py` & `pref_voting-1.1.1/pref_voting/tests/test_c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_combined_methods.py` & `pref_voting-1.1.1/pref_voting/tests/test_combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_generate_profiles.py` & `pref_voting-1.1.1/pref_voting/tests/test_generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_generate_spatial_profile.py` & `pref_voting-1.1.1/pref_voting/tests/test_generate_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_io.py` & `pref_voting-1.1.1/pref_voting/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_iterative_methods.py` & `pref_voting-1.1.1/pref_voting/tests/test_iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_majority_graph.py` & `pref_voting-1.1.1/pref_voting/tests/test_majority_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_mapping.py` & `pref_voting-1.1.1/pref_voting/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_margin_based_methods.py` & `pref_voting-1.1.1/pref_voting/tests/test_margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_margin_graph.py` & `pref_voting-1.1.1/pref_voting/tests/test_margin_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_other_methods.py` & `pref_voting-1.1.1/pref_voting/tests/test_other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_prob_voting_method.py` & `pref_voting-1.1.1/pref_voting/tests/test_prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_profile.py` & `pref_voting-1.1.1/pref_voting/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_profile_with_ties.py` & `pref_voting-1.1.1/pref_voting/tests/test_profile_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_ranking.py` & `pref_voting-1.1.1/pref_voting/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_scoring_rules.py` & `pref_voting-1.1.1/pref_voting/tests/test_scoring_rules.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_social_welfare_functions.py` & `pref_voting-1.1.1/pref_voting/tests/test_social_welfare_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_spatial_profile.py` & `pref_voting-1.1.1/pref_voting/tests/test_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_support_graph.py` & `pref_voting-1.1.1/pref_voting/tests/test_support_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_utility_function.py` & `pref_voting-1.1.1/pref_voting/tests/test_utility_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_utility_functions.py` & `pref_voting-1.1.1/pref_voting/tests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/tests/test_voting_method.py` & `pref_voting-1.1.1/pref_voting/tests/test_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/utility_functions.py` & `pref_voting-1.1.1/pref_voting/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/utility_methods.py` & `pref_voting-1.1.1/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/utility_profiles.py` & `pref_voting-1.1.1/pref_voting/utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/variable_candidate_axioms.py` & `pref_voting-1.1.1/pref_voting/variable_candidate_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/variable_voter_axioms.py` & `pref_voting-1.1.1/pref_voting/variable_voter_axioms.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 from pref_voting.axiom import Axiom
 from pref_voting.axiom_helpers import *
 import numpy as np
 from itertools import product, combinations, permutations
 from pref_voting.helper import weak_orders
+from pref_voting.rankings import Ranking
 
 def divide_electorate(prof):
     """Given a Profile or ProfileWithTies object, yield all possible ways to divide the electorate into two nonempty electorates."""
 
     R, C = prof.rankings_counts
 
     ranges = [range(count+1) for count in C]
```

### Comparing `pref_voting-1.1.0/pref_voting/voting_method.py` & `pref_voting-1.1.1/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pref_voting/weighted_majority_graphs.py` & `pref_voting-1.1.1/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.1.0/pyproject.toml` & `pref_voting-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "1.1.0"
+version = "1.1.1"
 description = "pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-1.1.0/setup.py` & `pref_voting-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'prefsampling>=0.1.16,<0.2.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.',
     'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n\n## Documentation\n\nOnline documentation is available at [https://pref-voting.readthedocs.io](https://pref-voting.readthedocs.io).\n\n## Example Usage\n\nA profile (of linear orders over the candidates) is created by initializing a `Profile` class object.  Simply provide a list of rankings (each ranking is a tuple of numbers) and a list giving the number of voters with each ranking:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [\n    (0, 1, 2, 3), \n    (2, 3, 1, 0), \n    (3, 1, 2, 0), \n    (1, 2, 0, 3), \n    (1, 3, 2, 0)]\n\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function `generate_profile` is used to generate a profile for a given number of candidates and voters:  \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\nTo use one of the many voting methods, import the function from `pref_voting.voting_methods` and apply it to the profile: \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\nfrom pref_voting.voting_methods import *\n\nprof = generate_profile(3, 4)\nsplit_cycle(prof) # returns the sorted list of winning candidates\nsplit_cycle.display(prof) # display the winning candidates\n\n```\n\n## Questions?\n\nFeel free to [send an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
```

### Comparing `pref_voting-1.1.0/PKG-INFO` & `pref_voting-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 1.1.0
+Version: 1.1.1
 Summary: pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

