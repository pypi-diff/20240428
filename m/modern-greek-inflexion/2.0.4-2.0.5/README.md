# Comparing `tmp/modern_greek_inflexion-2.0.4.tar.gz` & `tmp/modern_greek_inflexion-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modern_greek_inflexion-2.0.4.tar", last modified: Wed Apr 24 19:13:35 2024, max compression
+gzip compressed data, was "modern_greek_inflexion-2.0.5.tar", last modified: Sun Apr 28 15:49:48 2024, max compression
```

## Comparing `modern_greek_inflexion-2.0.4.tar` & `modern_greek_inflexion-2.0.5.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.597038 modern_greek_inflexion-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-04-24 19:13:35.597038 modern_greek_inflexion-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-24 19:13:35.597038 modern_greek_inflexion-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.541038 modern_greek_inflexion-2.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.545038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.545038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.545038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/all/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31016 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/all/create_all_adj.py
--rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/all/create_all_alt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.545038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/basic/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18381 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/basic/create_basic_adj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.545038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adverb/
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adverb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.545038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/article/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/article/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.549038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38636 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/create_noun_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    28303 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/create_noun_decl.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.549038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/create_num_decl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/create_num_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.549038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/create_pron_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/create_pron_decl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.549038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/adj.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/adv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/article.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.589038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/adj_grammar_lists.pickle
--rw-r--r--   0 runner    (1001) docker     (127) 29309847 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/el_GR.pickle
--rw-r--r--   0 runner    (1001) docker     (127)   347390 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/noun_grammar_lists.pickle
--rw-r--r--   0 runner    (1001) docker     (127)    31261 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/nouns_masc_fem.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/noun.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/numerals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/prefixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/pronouns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    33779 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/verb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.589038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/
--rw-r--r--   0 runner    (1001) docker     (127)    11070 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.589038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.589038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.589038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.589038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_past_personal_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_pers_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_present_personal_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_subjunctive_personal_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_imp_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.593038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17670 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_all_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_passive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_conjunctive_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_passive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_present_forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.593038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_aorist_participles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_passive_perfect_participle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle_arch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_passive_participle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.593038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_active_root.py
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_passive_root.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_roots_from_past.py
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.593038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_active_non_past_conjugation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_passive_past_continuous_conjugation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_passive_present_continuous_conjugation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_past_conjugation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.593038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-04-24 19:13:35.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-24 19:13:35.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:13:35.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:13:35.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 19:13:35.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 19:13:35.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.593038 modern_greek_inflexion-2.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/test/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.530624 modern_greek_inflexion-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14084 2024-04-28 15:49:48.530624 modern_greek_inflexion-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13077 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-28 15:49:48.534624 modern_greek_inflexion-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.478623 modern_greek_inflexion-2.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.482623 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.482623 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.482623 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/all/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31016 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/all/create_all_adj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/all/create_all_alt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.482623 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18381 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/basic/create_basic_adj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.486623 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adverb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adverb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.486623 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/article/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/article/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.486623 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/noun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/noun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38828 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/noun/create_noun_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28612 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/noun/create_noun_decl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/noun/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.486623 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/numeral/
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/numeral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/numeral/create_num_decl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/numeral/create_num_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.486623 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/pronoun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/pronoun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/pronoun/create_pron_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/pronoun/create_pron_decl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.490623 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/adj.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/adv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/article.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.526624 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/lists/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/lists/adj_grammar_lists.pickle
+-rw-r--r--   0 runner    (1001) docker     (127) 29309847 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/lists/el_GR.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)   347390 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/lists/noun_grammar_lists.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)    31261 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/lists/nouns_masc_fem.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/noun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/numerals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/prefixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/pronouns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33779 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/verb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.526624 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/
+-rw-r--r--   0 runner    (1001) docker     (127)    11070 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.526624 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.526624 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.526624 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.526624 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/persons/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/persons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_past_personal_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_pers_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_present_personal_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_subjunctive_personal_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/persons/create_imp_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.530624 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17670 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_all_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_passive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_conjunctive_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_passive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_present_forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.530624 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/participles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/participles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_aorist_participles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_passive_perfect_participle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle_arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_passive_participle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.530624 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/roots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/roots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_active_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_passive_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/roots/create_roots_from_past.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.530624 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/recognize/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/recognize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/recognize/recognize_active_non_past_conjugation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/recognize/recognize_passive_past_continuous_conjugation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/recognize/recognize_passive_present_continuous_conjugation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/recognize/recognize_past_conjugation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.530624 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14084 2024-04-28 15:49:48.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-28 15:49:48.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:49:48.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:49:48.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-28 15:49:48.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-28 15:49:48.000000 modern_greek_inflexion-2.0.5/src/modern_greek_inflexion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:48.530624 modern_greek_inflexion-2.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 15:49:42.000000 modern_greek_inflexion-2.0.5/test/test_case.py
```

### Comparing `modern_greek_inflexion-2.0.4/LICENSE` & `modern_greek_inflexion-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/PKG-INFO` & `modern_greek_inflexion-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modern-greek-inflexion
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python 3 library for creating inflected forms given basic forms of Modern Greek words
 Home-page: https://github.com/PicusZeus/modern-greek-inflexion
 Author: Krzysztof H
 Author-email: krzysztof.hilman@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -56,14 +56,15 @@
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 
 ## Change Log
+ * 2.0.5 Improvements in handling of archaic attic declension on -ως
  * 2.0.4 Fixed bug that caused incorrect creation of gen pl for some indeclinable nouns.
  * 2.0.3 Fixed issue with augmentation of dimotic verbs prefixed with 'para'. Also forcibly removed katharevousan types from such verbs. Fixed issue with indeclinable nouns ending on 'a', for which previously erroneously gen pl with ων ending was being created.
  * 2.0.2 Fixed issue, when sigmatic aorist stem is created when it exists only for passive imperative (ζέστανα but ζεστάσου).
  * 2.0.1 Fixed inconsistencies in the format of the output (in pronouns, where in some cases forms were given as string and not as set of strings)
  * 2.0.0 Major code refactoring with changes that break previous API. Code is quicker by about 25%, better readability, new docs, before migrating, read usage docs.
  * 1.0.6 Minor fixes and dependency update
  * 1.0.5 A bug, that caused problems in aorist formation for compound verbs from βαίνω fixed.
```

### Comparing `modern_greek_inflexion-2.0.4/README.md` & `modern_greek_inflexion-2.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 
 ## Change Log
+ * 2.0.5 Improvements in handling of archaic attic declension on -ως
  * 2.0.4 Fixed bug that caused incorrect creation of gen pl for some indeclinable nouns.
  * 2.0.3 Fixed issue with augmentation of dimotic verbs prefixed with 'para'. Also forcibly removed katharevousan types from such verbs. Fixed issue with indeclinable nouns ending on 'a', for which previously erroneously gen pl with ων ending was being created.
  * 2.0.2 Fixed issue, when sigmatic aorist stem is created when it exists only for passive imperative (ζέστανα but ζεστάσου).
  * 2.0.1 Fixed inconsistencies in the format of the output (in pronouns, where in some cases forms were given as string and not as set of strings)
  * 2.0.0 Major code refactoring with changes that break previous API. Code is quicker by about 25%, better readability, new docs, before migrating, read usage docs.
  * 1.0.6 Minor fixes and dependency update
  * 1.0.5 A bug, that caused problems in aorist formation for compound verbs from βαίνω fixed.
```

### Comparing `modern_greek_inflexion-2.0.4/setup.cfg` & `modern_greek_inflexion-2.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = modern-greek-inflexion
-version = 2.0.4
+version = 2.0.5
 description = Python 3 library for creating inflected forms given basic forms of Modern Greek words
 long_description_content_type = text/markdown
 long_description = file: README.md
 license = MIT
 url = https://github.com/PicusZeus/modern-greek-inflexion
 author = Krzysztof H
 author_email = krzysztof.hilman@gmail.com
```

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/__init__.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/_helpers.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/_helpers.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/all/create_all_adj.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/all/create_all_adj.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/all/create_all_alt.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/all/create_all_alt.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/basic/create_basic_adj.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adjective/basic/create_basic_adj.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adverb/__init__.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/adverb/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/article/__init__.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/article/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/__init__.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/noun/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/create_noun_basic.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/noun/create_noun_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from modern_greek_accentuation.accentuation import convert_to_monotonic
 
 GENDERS = 'genders'
 
 
 def create_all_basic_forms(noun: str, aklito: bool | str = False, gender: genderType = None,
                            proper_name: bool = False) -> noun_basic_forms:
+
     """
     :param noun: The noun you want to inflect has to be in its basic form, that is in nominative singular, or if it's
     plural only, in plural
     :param aklito: If you know that the noun you want to inflect is not declinable, set this flag to True, the default
     value is False.
     :param gender: If you know the nouns gender, set one. There are 10 possibilities, outside of standard 'fem', 'masc',
     'neut', if you know it's only plural or singular, it can be 'fem_sg', 'fem_pl' itd. It is also possible to set
@@ -651,14 +652,17 @@
         noun_temp[GENDERS] = [FEM]
         noun_temp[NOM_PL] = noun
         noun_temp[NOM_SG] = ''
         noun_temp[GEN_SG] = ''
 
     elif noun.endswith('ώς') and gender == FEM:
         noun_temp[GEN_SG] = noun[:-2] + 'ούς'
+    elif noun[-2:] in ['ώς', 'ως'] and gender in [MASC, MASC_SG] and noun[:-2] + 'ότας' not in greek_corpus:
+        noun_temp[GEN_SG] = noun[:-1]
+        noun_temp[NOM_PL] = noun[:-1]
 
     elif noun[-1] in ['ξ', 'ψ', 'τ', 'ρ', 'β', 'ν', 'δ', 'ε', 'έ', 'ζ', 'κ', 'λ', 'μ', 'ς'] and not aklito:
 
         # not very common but existing 3rd declension nouns
         # gender would be a wild guess
 
         stems = []
@@ -700,15 +704,15 @@
             elif noun[-2:] == 'ώρ':
                 stems.append(noun[:-2] + 'όρ')
             else:
                 noun_temp[GENDERS] = [NEUT]
 
         elif noun.endswith('ώς'):
             if not gender:
-                gender = [NEUT]
+                gender = NEUT
             # ουσιαστικοποιημένες αρχαίες μετοχές
             stems.append(noun[:-1] + 'τ')
             stems.append(noun[:-2] + 'ότ')
         elif noun.endswith('ις'):
             if not gender:
                 gender = FEM
             stems.append(noun[:-1] + 'τ')
```

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/create_noun_decl.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/noun/create_noun_decl.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,19 +427,24 @@
                         noun_all[gender][SG][GEN] = gen_sg + ',' + nom_sg[:-1]
 
                         noun_all[gender][SG][ACC] = acc_sg_arch + ',' + nom_sg[:-1]
 
                 noun_all[gender][SG][VOC] = nom_sg[:-1]
                 noun_all[gender][PL][GEN] = gen_sg[:-1] + 'ν'
 
-            elif nom_sg[-2:] == 'ως' and gen_sg[-1] == 'ω':
-
-                noun_all[gender][SG][ACC] = gen_sg
+            elif nom_sg[-2:] in ['ως', 'ώς'] and gen_sg[-1] in ['ω', 'ώ']:
+                if nom_sg in ["Άθως", "άλως", "Κέως", "Κώς", "λαγώς", "Μίνως", "Τέως"]:
+                    noun_all[gender][SG][ACC] = gen_sg
+                else:
+                    noun_all[gender][SG][ACC] = gen_sg + 'ν'
                 noun_all[gender][SG][VOC] = nom_sg
-                noun_all[gender][PL][GEN] = gen_sg + 'ν'
+                if nom_pl:
+                    noun_all[gender][PL][GEN] = gen_sg + 'ν'
+                    noun_all[gender][PL][ACC] = nom_sg
+
 
             elif nom_sg == nom_pl:
                 # aklita
                 noun_all[gender][SG][ACC] = nom_sg
                 noun_all[gender][PL][GEN] = nom_pl
 
             elif gen_sg[-2:] in ['ος', 'ός'] and gen_sg[-3] not in vowels:
```

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/__init__.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/numeral/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/create_num_decl.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/numeral/create_num_decl.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/create_num_list.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/numeral/create_num_list.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/__init__.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/pronoun/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/create_pron_basic.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/pronoun/create_pron_basic.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/create_pron_decl.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/pronoun/create_pron_decl.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/adj.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/adj.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/article.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/article.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/adj_grammar_lists.pickle` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/lists/adj_grammar_lists.pickle`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/el_GR.pickle` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/lists/el_GR.pickle`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/noun_grammar_lists.pickle` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/lists/noun_grammar_lists.pickle`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/nouns_masc_fem.pickle` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/lists/nouns_masc_fem.pickle`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/noun.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/noun.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
                    'Πάσχα': {NOM_SG: 'Πάσχα', NOM_PL: '', GEN_SG: '', GENDERS: [NEUT]},
                    'δόρυ': {NOM_SG: 'δόρυ', NOM_PL: 'δόρατα', GEN_SG: 'δόρατος', GENDERS: [NEUT]},
                    'ήμισυ': {NOM_SG: 'ήμισυ', NOM_PL: 'ημίσεα', GEN_SG: 'ημίσεος', GENDERS: [NEUT]},
                    'γης': {NOM_SG: 'γης', NOM_PL: 'γαίες', GEN_SG: 'γης', GENDERS: [FEM]},
                    'γη': {NOM_SG: 'γη', NOM_PL: 'γαίες', GEN_SG: 'γης', GENDERS: [FEM]},
                    'αλλάς': {NOM_SG: 'αλλάς', NOM_PL: 'αλλάντες', GEN_SG: 'αλλάντος', GENDERS: [MASC]},
                    'χρως': {NOM_SG: 'χρως', NOM_PL: '', GEN_SG: 'χρωτός,χρωός', GENDERS: [MASC]},
-                   'κάλως': {NOM_SG: 'κάλως', NOM_PL: 'κάλως', GEN_SG: 'κάλω', GENDERS: [MASC]},
                    'μάνα': {NOM_SG: 'μάνα', NOM_PL: 'μάνες,μανάδες', GEN_SG: 'μάνας', GENDERS: [FEM]},
                    'πλάνης': {NOM_SG: 'πλάνης', NOM_PL: 'πλάνητες', GEN_SG: 'πλάνητος', GENDERS: [MASC, FEM]},
                    'άστυ': {NOM_SG: 'άστυ', NOM_PL: 'άστη', GEN_SG: 'άστεως', GENDERS: [NEUT]},
                    'βράδυ': {NOM_SG: 'βράδυ', NOM_PL: 'βράδια', GEN_SG: 'βραδιού', GENDERS: [NEUT]},
                    'στάχυ': {NOM_SG: 'στάχυ', NOM_PL: 'στάχυα', GEN_SG: 'σταχυού', GENDERS: [NEUT]},
                    'δίχτυ': {NOM_SG: 'δίχτυ', NOM_PL: 'δίχτυα', GEN_SG: 'διχτυού', GENDERS: [NEUT]},
                    'δάκρυ': {NOM_SG: 'δάκρυ', NOM_PL: 'δάκρυα', GEN_SG: 'δακρύου', GENDERS: [NEUT]},
```

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/numerals.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/numerals.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/prefixes.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/prefixes.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/pronouns.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/pronouns.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/typing.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/typing.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/variables.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/variables.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/verb.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/resources/verb.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/__init__.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_past_personal_forms.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_past_personal_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_pers_forms.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_pers_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_present_personal_forms.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_present_personal_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_subjunctive_personal_forms.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_subjunctive_personal_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_imp_pass.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/all/persons/create_imp_pass.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_all_forms.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_all_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_active.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_active.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_forms.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_passive.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_passive.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_conjunctive_forms.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_conjunctive_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_active.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_active.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_forms.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_passive.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_passive.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_present_forms.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_present_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_aorist_participles.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_aorist_participles.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_passive_perfect_participle.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_passive_perfect_participle.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle_arch.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle_arch.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_passive_participle.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_passive_participle.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_active_root.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_active_root.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_passive_root.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_passive_root.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_root.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_root.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_roots_from_past.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/create/roots/create_roots_from_past.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/helpers.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/helpers.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_active_non_past_conjugation.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/recognize/recognize_active_non_past_conjugation.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_passive_past_continuous_conjugation.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/recognize/recognize_passive_past_continuous_conjugation.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_passive_present_continuous_conjugation.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/recognize/recognize_passive_present_continuous_conjugation.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_past_conjugation.py` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion/verb/recognize/recognize_past_conjugation.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/PKG-INFO` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modern-greek-inflexion
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python 3 library for creating inflected forms given basic forms of Modern Greek words
 Home-page: https://github.com/PicusZeus/modern-greek-inflexion
 Author: Krzysztof H
 Author-email: krzysztof.hilman@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -56,14 +56,15 @@
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 
 ## Change Log
+ * 2.0.5 Improvements in handling of archaic attic declension on -ως
  * 2.0.4 Fixed bug that caused incorrect creation of gen pl for some indeclinable nouns.
  * 2.0.3 Fixed issue with augmentation of dimotic verbs prefixed with 'para'. Also forcibly removed katharevousan types from such verbs. Fixed issue with indeclinable nouns ending on 'a', for which previously erroneously gen pl with ων ending was being created.
  * 2.0.2 Fixed issue, when sigmatic aorist stem is created when it exists only for passive imperative (ζέστανα but ζεστάσου).
  * 2.0.1 Fixed inconsistencies in the format of the output (in pronouns, where in some cases forms were given as string and not as set of strings)
  * 2.0.0 Major code refactoring with changes that break previous API. Code is quicker by about 25%, better readability, new docs, before migrating, read usage docs.
  * 1.0.6 Minor fixes and dependency update
  * 1.0.5 A bug, that caused problems in aorist formation for compound verbs from βαίνω fixed.
```

### Comparing `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/SOURCES.txt` & `modern_greek_inflexion-2.0.5/src/modern_greek_inflexion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

