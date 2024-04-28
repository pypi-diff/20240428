# Comparing `tmp/ares_ai-0.5.5.tar.gz` & `tmp/ares_ai-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ares_ai-0.5.5.tar", last modified: Fri Apr 26 10:17:43 2024, max compression
+gzip compressed data, was "ares_ai-0.5.6.tar", last modified: Sun Apr 28 07:15:28 2024, max compression
```

## Comparing `ares_ai-0.5.5.tar` & `ares_ai-0.5.6.tar`

### file list

```diff
@@ -1,102 +1,100 @@
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:17:43.561436 ares_ai-0.5.5/
--rw-rw-rw-   0 manihani (23549) future   (20099)     4591 2024-04-24 11:52:46.000000 ares_ai-0.5.5/.gitignore
--rw-rw-rw-   0 manihani (23549) future   (20099)      268 2024-04-22 03:39:34.000000 ares_ai-0.5.5/CHANGELOG.md
--rw-rw-rw-   0 manihani (23549) future   (20099)    11357 2024-01-08 23:19:52.000000 ares_ai-0.5.5/LICENSE
--rw-rw-rw-   0 manihani (23549) future   (20099)       51 2024-04-25 23:18:28.000000 ares_ai-0.5.5/MANIFEST.in
--rw-r--r--   0 manihani (23549) future   (20099)    26407 2024-04-26 10:17:43.560436 ares_ai-0.5.5/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)    10868 2024-04-26 10:17:24.000000 ares_ai-0.5.5/README.md
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:17:43.386444 ares_ai-0.5.5/ares/
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:17:43.400443 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/
--rw-rw-rw-   0 manihani (23549) future   (20099)     6952 2024-04-26 08:46:18.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    29589 2024-04-26 09:47:00.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    25648 2024-04-26 09:23:11.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    17172 2024-04-26 08:52:43.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__init__.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:17:43.427442 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)     4441 2024-04-26 08:48:35.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     9876 2024-03-23 04:28:17.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    16631 2024-04-26 09:51:49.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    39678 2024-03-23 04:28:17.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    11077 2024-04-26 09:25:16.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    24854 2024-03-25 00:41:32.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9237 2024-04-26 08:55:30.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    18100 2024-03-23 04:28:17.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      159 2024-04-24 01:00:10.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      175 2024-03-23 04:28:12.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2243 2024-04-24 05:41:16.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2109 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:17:43.446442 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/
--rw-rw-rw-   0 manihani (23549) future   (20099)    33610 2024-04-25 19:02:45.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    42944 2024-04-25 18:44:17.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)       36 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    18046 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     7064 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     8000 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__init__.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:17:43.480440 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)    11001 2024-04-25 19:45:00.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    11341 2024-03-25 23:25:08.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    22313 2024-04-25 18:46:20.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    39551 2024-03-23 04:28:19.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     7856 2024-04-24 01:01:09.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    19694 2024-03-23 04:31:25.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     4238 2024-04-24 01:01:09.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     9481 2024-03-23 04:31:25.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      158 2024-04-24 01:01:00.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      169 2024-02-08 01:18:18.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     5437 2024-01-20 22:01:06.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     8966 2024-04-24 01:01:00.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    19175 2024-03-23 04:28:19.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      494 2024-01-20 21:58:30.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/test.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/ppi.py
--rw-rw-rw-   0 manihani (23549) future   (20099)       22 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/__init__.py
--rw-r--r--   0 manihani (23549) future   (20099)      152 2024-03-25 00:40:39.000000 ares_ai-0.5.5/ares/__init__.pyc
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:17:43.515438 ares_ai-0.5.5/ares/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)      166 2024-04-24 01:00:10.000000 ares_ai-0.5.5/ares/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      196 2024-03-23 04:28:12.000000 ares_ai-0.5.5/ares/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     7504 2024-04-24 11:55:06.000000 ares_ai-0.5.5/ares/__pycache__/ares.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     9734 2024-03-25 23:24:58.000000 ares_ai-0.5.5/ares/__pycache__/ares.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     4163 2024-04-24 11:55:12.000000 ares_ai-0.5.5/ares/__pycache__/binary_classifier.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     3676 2024-03-23 04:28:17.000000 ares_ai-0.5.5/ares/__pycache__/binary_classifier.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      371 2024-04-24 01:01:09.000000 ares_ai-0.5.5/ares/__pycache__/kilt_filter.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      469 2024-03-23 04:31:25.000000 ares_ai-0.5.5/ares/__pycache__/kilt_filter.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2294 2024-04-24 11:55:14.000000 ares_ai-0.5.5/ares/__pycache__/rag_scoring.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     2495 2024-03-23 04:28:19.000000 ares_ai-0.5.5/ares/__pycache__/rag_scoring.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      356 2024-04-24 01:01:09.000000 ares_ai-0.5.5/ares/__pycache__/superglue_filter.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      442 2024-03-23 04:31:25.000000 ares_ai-0.5.5/ares/__pycache__/superglue_filter.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2419 2024-04-26 07:58:28.000000 ares_ai-0.5.5/ares/__pycache__/synthetic_generator.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     3600 2024-03-23 04:28:12.000000 ares_ai-0.5.5/ares/__pycache__/synthetic_generator.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     4840 2024-04-24 11:55:15.000000 ares_ai-0.5.5/ares/__pycache__/ues_idp.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     5858 2024-03-25 23:25:08.000000 ares_ai-0.5.5/ares/__pycache__/ues_idp.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    11651 2024-04-24 11:48:03.000000 ares_ai-0.5.5/ares/ares.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:17:43.528438 ares_ai-0.5.5/ares/ares_ai.egg-info/
--rw-r--r--   0 manihani (23549) future   (20099)    26304 2024-04-05 05:20:31.000000 ares_ai-0.5.5/ares/ares_ai.egg-info/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-05 05:20:31.000000 ares_ai-0.5.5/ares/ares_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 05:20:31.000000 ares_ai-0.5.5/ares/ares_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 05:20:31.000000 ares_ai-0.5.5/ares/ares_ai.egg-info/entry_points.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)      627 2024-04-05 05:20:31.000000 ares_ai-0.5.5/ares/ares_ai.egg-info/requires.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 05:20:31.000000 ares_ai-0.5.5/ares/ares_ai.egg-info/top_level.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)     8082 2024-04-24 11:17:32.000000 ares_ai-0.5.5/ares/binary_classifier.py
--rw-rw-rw-   0 manihani (23549) future   (20099)      154 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/kilt_filter.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:17:43.535437 ares_ai-0.5.5/ares/ppi/
--rw-rw-rw-   0 manihani (23549) future   (20099)     6148 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/ppi/.DS_Store
--rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/ppi/ppi.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     9196 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/ppi/ppi_testing.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     6085 2024-04-24 11:39:44.000000 ares_ai-0.5.5/ares/rag_scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)      134 2024-04-22 03:39:34.000000 ares_ai-0.5.5/ares/superglue_filter.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     4332 2024-04-26 07:54:48.000000 ares_ai-0.5.5/ares/synthetic_generator.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    10206 2024-04-24 11:36:32.000000 ares_ai-0.5.5/ares/ues_idp.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:17:43.557436 ares_ai-0.5.5/ares_ai.egg-info/
--rw-r--r--   0 manihani (23549) future   (20099)    26407 2024-04-26 10:17:37.000000 ares_ai-0.5.5/ares_ai.egg-info/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)     4221 2024-04-26 10:17:43.000000 ares_ai-0.5.5/ares_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-26 10:17:37.000000 ares_ai-0.5.5/ares_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-26 10:17:37.000000 ares_ai-0.5.5/ares_ai.egg-info/entry_points.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)      682 2024-04-26 10:17:37.000000 ares_ai-0.5.5/ares_ai.egg-info/requires.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-26 10:17:37.000000 ares_ai-0.5.5/ares_ai.egg-info/top_level.txt
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:17:43.553437 ares_ai-0.5.5/checkpoints/
--rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:34.000000 ares_ai-0.5.5/checkpoints/.gitignore
--rw-rw-rw-   0 manihani (23549) future   (20099)     2905 2024-04-26 10:17:06.000000 ares_ai-0.5.5/pyproject.toml
--rw-rw-rw-   0 manihani (23549) future   (20099)     5066 2024-04-26 03:07:42.000000 ares_ai-0.5.5/requirements.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       93 2024-04-26 10:17:43.564436 ares_ai-0.5.5/setup.cfg
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:17:43.555436 ares_ai-0.5.5/tests/
--rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:53.000000 ares_ai-0.5.5/tests/.gitignore
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-28 07:15:28.398535 ares_ai-0.5.6/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4591 2024-04-24 11:52:46.000000 ares_ai-0.5.6/.gitignore
+-rw-rw-rw-   0 manihani (23549) future   (20099)      268 2024-04-22 03:39:34.000000 ares_ai-0.5.6/CHANGELOG.md
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11357 2024-01-08 23:19:52.000000 ares_ai-0.5.6/LICENSE
+-rw-rw-rw-   0 manihani (23549) future   (20099)       51 2024-04-25 23:18:28.000000 ares_ai-0.5.6/MANIFEST.in
+-rw-r--r--   0 manihani (23549) future   (20099)    26407 2024-04-28 07:15:28.397535 ares_ai-0.5.6/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10868 2024-04-26 10:17:24.000000 ares_ai-0.5.6/README.md
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-28 07:15:27.824561 ares_ai-0.5.6/ares/
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-28 07:15:27.839560 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     6952 2024-04-26 08:46:18.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    29888 2024-04-28 07:14:55.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    25648 2024-04-26 09:23:11.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    17172 2024-04-26 08:52:43.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__init__.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-28 07:15:27.938556 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4441 2024-04-26 08:48:35.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     9876 2024-03-23 04:28:17.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    16773 2024-04-28 07:07:41.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    39678 2024-03-23 04:28:17.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11077 2024-04-26 09:25:16.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    24854 2024-03-25 00:41:32.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9237 2024-04-26 08:55:30.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    18100 2024-03-23 04:28:17.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      159 2024-04-24 01:00:10.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      175 2024-03-23 04:28:12.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2243 2024-04-24 05:41:16.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2109 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-28 07:15:27.957555 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    33610 2024-04-25 19:02:45.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    42944 2024-04-25 18:44:17.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)       36 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    18046 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7064 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8000 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__init__.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-28 07:15:28.102548 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11001 2024-04-25 19:45:00.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    11341 2024-03-25 23:25:08.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    22313 2024-04-25 18:46:20.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    39551 2024-03-23 04:28:19.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7856 2024-04-24 01:01:09.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    19694 2024-03-23 04:31:25.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4238 2024-04-24 01:01:09.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     9481 2024-03-23 04:31:25.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      158 2024-04-24 01:01:00.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      169 2024-02-08 01:18:18.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5437 2024-01-20 22:01:06.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8966 2024-04-24 01:01:00.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    19175 2024-03-23 04:28:19.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      494 2024-01-20 21:58:30.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/test.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/ppi.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)       22 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/__init__.py
+-rw-r--r--   0 manihani (23549) future   (20099)      152 2024-03-25 00:40:39.000000 ares_ai-0.5.6/ares/__init__.pyc
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-28 07:15:28.267541 ares_ai-0.5.6/ares/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)      166 2024-04-24 01:00:10.000000 ares_ai-0.5.6/ares/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      196 2024-03-23 04:28:12.000000 ares_ai-0.5.6/ares/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7504 2024-04-24 11:55:06.000000 ares_ai-0.5.6/ares/__pycache__/ares.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     9734 2024-03-25 23:24:58.000000 ares_ai-0.5.6/ares/__pycache__/ares.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4163 2024-04-24 11:55:12.000000 ares_ai-0.5.6/ares/__pycache__/binary_classifier.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     3676 2024-03-23 04:28:17.000000 ares_ai-0.5.6/ares/__pycache__/binary_classifier.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      371 2024-04-24 01:01:09.000000 ares_ai-0.5.6/ares/__pycache__/kilt_filter.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      469 2024-03-23 04:31:25.000000 ares_ai-0.5.6/ares/__pycache__/kilt_filter.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2294 2024-04-24 11:55:14.000000 ares_ai-0.5.6/ares/__pycache__/rag_scoring.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     2495 2024-03-23 04:28:19.000000 ares_ai-0.5.6/ares/__pycache__/rag_scoring.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      356 2024-04-24 01:01:09.000000 ares_ai-0.5.6/ares/__pycache__/superglue_filter.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      442 2024-03-23 04:31:25.000000 ares_ai-0.5.6/ares/__pycache__/superglue_filter.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2419 2024-04-26 07:58:28.000000 ares_ai-0.5.6/ares/__pycache__/synthetic_generator.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     3600 2024-03-23 04:28:12.000000 ares_ai-0.5.6/ares/__pycache__/synthetic_generator.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4840 2024-04-24 11:55:15.000000 ares_ai-0.5.6/ares/__pycache__/ues_idp.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     5858 2024-03-25 23:25:08.000000 ares_ai-0.5.6/ares/__pycache__/ues_idp.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11651 2024-04-24 11:48:03.000000 ares_ai-0.5.6/ares/ares.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-28 07:15:28.334538 ares_ai-0.5.6/ares/ares_ai.egg-info/
+-rw-r--r--   0 manihani (23549) future   (20099)    26304 2024-04-05 05:20:31.000000 ares_ai-0.5.6/ares/ares_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-05 05:20:31.000000 ares_ai-0.5.6/ares/ares_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 05:20:31.000000 ares_ai-0.5.6/ares/ares_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 05:20:31.000000 ares_ai-0.5.6/ares/ares_ai.egg-info/entry_points.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)      627 2024-04-05 05:20:31.000000 ares_ai-0.5.6/ares/ares_ai.egg-info/requires.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 05:20:31.000000 ares_ai-0.5.6/ares/ares_ai.egg-info/top_level.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8082 2024-04-24 11:17:32.000000 ares_ai-0.5.6/ares/binary_classifier.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)      154 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/kilt_filter.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-28 07:15:28.373536 ares_ai-0.5.6/ares/ppi/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     6148 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/ppi/.DS_Store
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/ppi/ppi.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9196 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/ppi/ppi_testing.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     6085 2024-04-24 11:39:44.000000 ares_ai-0.5.6/ares/rag_scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)      134 2024-04-22 03:39:34.000000 ares_ai-0.5.6/ares/superglue_filter.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4332 2024-04-26 07:54:48.000000 ares_ai-0.5.6/ares/synthetic_generator.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10206 2024-04-24 11:36:32.000000 ares_ai-0.5.6/ares/ues_idp.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-28 07:15:28.394535 ares_ai-0.5.6/ares_ai.egg-info/
+-rw-r--r--   0 manihani (23549) future   (20099)    26407 2024-04-28 07:15:22.000000 ares_ai-0.5.6/ares_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4198 2024-04-28 07:15:27.000000 ares_ai-0.5.6/ares_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-28 07:15:22.000000 ares_ai-0.5.6/ares_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-28 07:15:22.000000 ares_ai-0.5.6/ares_ai.egg-info/entry_points.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)      682 2024-04-28 07:15:22.000000 ares_ai-0.5.6/ares_ai.egg-info/requires.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-28 07:15:22.000000 ares_ai-0.5.6/ares_ai.egg-info/top_level.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2905 2024-04-28 07:13:28.000000 ares_ai-0.5.6/pyproject.toml
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5066 2024-04-26 03:07:42.000000 ares_ai-0.5.6/requirements.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       93 2024-04-28 07:15:28.400535 ares_ai-0.5.6/setup.cfg
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-28 07:15:28.392535 ares_ai-0.5.6/tests/
+-rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:53.000000 ares_ai-0.5.6/tests/.gitignore
```

### Comparing `ares_ai-0.5.5/.gitignore` & `ares_ai-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/LICENSE` & `ares_ai-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/PKG-INFO` & `ares_ai-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ares-ai
-Version: 0.5.5
+Version: 0.5.6
 Summary: ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 Author-email: Jon Saad-Falcon <jonsaadfalcon@stanford.edu>, Robby Manihani <manihani@stanford.edu>, Omar Khattab <okhattab@stanford.edu>, Christopher Potts <cgpotts@stanford.edu>, Matei Zaharia <matei@berkeley.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ares_ai-0.5.5/README.md` & `ares_ai-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,21 @@
     print("Starting new learning rate: " + str(chosen_learning_rate))
     print("--------------------------------------------------------------------------")
 
     import datetime
 
     current_datetime = datetime.datetime.now().strftime("%Y-%m-%d_%H:%M:%S")
 
+    parent_dir = "checkpoints/" + model_choice.replace("/", "-")
+
+    if not os.path.exists(parent_dir):
+        print(f"Creating parent checkpoint directory: {parent_dir}")
+        print("--------------------------------------------------------------------------")
+        os.makedirs(parent_dir)
+
     checkpoint_path = "checkpoints/" + model_choice.replace("/", "-") + "/" + label_column + "_" + str(validation_set.split("/")[-1].replace(".tsv", "")) + "_" + current_datetime + ".pt"
 
     # checkpoint_path = "checkpoints/" + model_choice.replace("/", "-") + "/" + dataset.replace("../", "").replace("/", "-") + "/" + str(chosen_learning_rate) + "_"
     # checkpoint_path += str(number_of_runs) + "_" + str(validation_set_scoring) + "_" + label_column + "_" + str(validation_set.split("/")[-1].replace(".tsv", "")) + "_" + str(random_int) + ".pt"
 
     # checkpoint_path = "checkpoints/" + model_choice.replace("/", "-") + "/" + dataset.replace("../", "").replace("/", "-") + "/" + str(chosen_learning_rate) + "_"
     # checkpoint_path += str(number_of_runs) + "_" + str(validation_set_scoring) + "_" + label_column + "_" + str(validation_set.split("/")[-1].replace(".tsv", "")) + "_" + str(random_int) + ".pt"
```

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 26 09:47:00 2024 UTC, .py size: 29589 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1478 2b66 9573 0000  o........x+f.s..
+00000000: 6f0d 0d0a 0000 0000 82f5 2d66 6474 0000  o.........-fdt..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 dc02 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c02 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6400 6401 6c0a 5a0b 6400  m.Z...d.d.l.Z.d.
 00000070: 6401 6c0c 5a0d 6400 6401 6c0e 5a0e 6400  d.l.Z.d.d.l.Z.d.
@@ -248,28 +248,28 @@
 00000f70: 7878 6c61 7267 6569 0006 0000 6900 0300  xxlargei....i...
 00000f80: 00e9 0001 0000 2916 da0c 6d6f 6465 6c5f  ......)...model_
 00000f90: 6368 6f69 6365 da05 7375 7065 7272 4500  choice..superrE.
 00000fa0: 0000 da08 5f5f 696e 6974 5f5f 7210 0000  ....__init__r...
 00000fb0: 00da 0f66 726f 6d5f 7072 6574 7261 696e  ...from_pretrain
 00000fc0: 6564 5a0b 6174 746e 5f63 6f6e 6669 67da  edZ.attn_config.
 00000fd0: 106d 6178 5f74 6f6b 656e 5f6c 656e 6774  .max_token_lengt
-00000fe0: 68da 0b6d 6178 5f73 6571 5f6c 656e 720f  h..max_seq_lenr.
+00000fe0: 685a 0b6d 6178 5f73 6571 5f6c 656e 720f  hZ.max_seq_lenr.
 00000ff0: 0000 00da 0574 6f72 6368 da08 6266 6c6f  .....torch..bflo
 00001000: 6174 3136 da0b 7472 616e 7366 6f72 6d65  at16..transforme
 00001010: 72da 0c65 6e63 6f64 6572 4d6f 6465 6cda  r..encoderModel.
 00001020: 1c4d 7074 466f 7253 6571 7565 6e63 6543  .MptForSequenceC
 00001030: 6c61 7373 6966 6963 6174 696f 6e72 1100  lassificationr..
 00001040: 0000 7207 0000 00da 026e 6eda 0a53 6571  ..r......nn..Seq
 00001050: 7565 6e74 6961 6cda 064c 696e 6561 72da  uential..Linear.
 00001060: 0a63 6c61 7373 6966 6965 72da 0e65 6d62  .classifier..emb
 00001070: 6564 6469 6e67 5f73 697a 6529 06da 0473  edding_size)...s
 00001080: 656c 66da 106e 756d 6265 725f 6f66 5f6c  elf..number_of_l
 00001090: 6162 656c 7372 5200 0000 7249 0000 005a  abelsrR...rI...Z
 000010a0: 0e6d 6f64 656c 5f65 6e63 6f64 696e 6772  .model_encodingr
-000010b0: 6100 0000 a901 da09 5f5f 636c 6173 735f  a.......__class_
+000010b0: 6000 0000 a901 da09 5f5f 636c 6173 735f  `.......__class_
 000010c0: 5f72 3000 0000 7231 0000 0072 5400 0000  _r0...r1...rT...
 000010d0: 6500 0000 7348 0000 0006 010e 0108 010e  e...sH..........
 000010e0: 020a 0106 0104 0202 0102 0104 0202 0102  ................
 000010f0: 0106 fa04 080a 0108 020e 0404 0108 0108  ................
 00001100: 020a 0204 0108 0108 020a 0204 0108 0108  ................
 00001110: 020a 0204 0108 010a 0404 0106 011e 040a  ................
 00001120: 017a 1843 7573 746f 6d42 4552 544d 6f64  .z.CustomBERTMod
@@ -282,49 +282,49 @@
 00001190: 1900 7d07 7c07 6400 6400 8502 6406 6400  ..}.|.d.d...d.d.
 000011a0: 6400 8502 6603 1900 a002 6407 7c00 6a03  d...f.....d.|.j.
 000011b0: a102 7d08 7c00 a004 7c08 a101 7d09 7c09  ..}.|...|...}.|.
 000011c0: 5300 2908 4e29 04fa 0874 352d 736d 616c  S.).N)...t5-smal
 000011d0: 6c72 5000 0000 724f 0000 0072 4d00 0000  lrP...rO...rM...
 000011e0: 2902 da09 696e 7075 745f 6964 73da 0e61  )...input_ids..a
 000011f0: 7474 656e 7469 6f6e 5f6d 6173 6bda 066c  ttention_mask..l
-00001200: 6f67 6974 7329 0172 6800 0000 5a11 6c61  ogits).rh...Z.la
+00001200: 6f67 6974 7329 0172 6700 0000 5a11 6c61  ogits).rg...Z.la
 00001210: 7374 5f68 6964 6465 6e5f 7374 6174 6572  st_hidden_stater
 00001220: 0100 0000 7238 0000 0029 0572 5200 0000  ....r8...).rR...
-00001230: 725b 0000 00da 0476 6965 7772 6100 0000  r[.....viewra...
-00001240: 7260 0000 0029 0a72 6200 0000 da03 6964  r`...).rb.....id
+00001230: 725a 0000 00da 0476 6965 7772 6000 0000  rZ.....viewr`...
+00001240: 725f 0000 0029 0a72 6100 0000 da03 6964  r_...).ra.....id
 00001250: 73da 046d 6173 6bda 066c 6162 656c 73da  s..mask..labels.
 00001260: 1164 6563 6f64 6572 5f69 6e70 7574 5f69  .decoder_input_i
 00001270: 6473 7252 0000 005a 0c74 6f74 616c 5f6f  dsrR...Z.total_o
 00001280: 7574 7075 745a 0f73 6571 7565 6e63 655f  utputZ.sequence_
 00001290: 6f75 7470 7574 5a1b 6c61 7374 5f68 6964  outputZ.last_hid
 000012a0: 6465 6e5f 7374 6174 655f 666f 726d 6174  den_state_format
 000012b0: 7465 645a 0e6c 696e 6561 7232 5f6f 7574  tedZ.linear2_out
 000012c0: 7075 7472 3000 0000 7230 0000 0072 3100  putr0...r0...r1.
 000012d0: 0000 da07 666f 7277 6172 64a0 0000 0073  ....forward....s
 000012e0: 1200 0000 0601 0801 0e01 0801 0e02 0801  ................
 000012f0: 2002 0a01 0402 7a17 4375 7374 6f6d 4245   .....z.CustomBE
 00001300: 5254 4d6f 6465 6c2e 666f 7277 6172 6429  RTModel.forward)
 00001310: 024e 4e29 06da 085f 5f6e 616d 655f 5fda  .NN)...__name__.
 00001320: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00001330: 7561 6c6e 616d 655f 5f72 5400 0000 726f  ualname__rT...ro
+00001330: 7561 6c6e 616d 655f 5f72 5400 0000 726e  ualname__rT...rn
 00001340: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00001350: 5f5f 7230 0000 0072 3000 0000 7264 0000  __r0...r0...rd..
+00001350: 5f5f 7230 0000 0072 3000 0000 7263 0000  __r0...r0...rc..
 00001360: 0072 3100 0000 7245 0000 0064 0000 0073  .r1...rE...d...s
 00001370: 0600 0000 0800 0c01 123b 7245 0000 0063  .........;rE...c
 00001380: 0200 0000 0000 0000 0000 0000 0200 0000  ................
 00001390: 0500 0000 4300 0000 7312 0000 007c 007c  ....C...s....|.|
 000013a0: 0164 0119 0064 0264 0364 048d 0353 0029  .d...d.d.d...S.)
 000013b0: 054e da04 7465 7874 da0a 6d61 785f 6c65  .N..text..max_le
 000013c0: 6e67 7468 5429 02da 0770 6164 6469 6e67  ngthT)...padding
 000013d0: da0a 7472 756e 6361 7469 6f6e 7230 0000  ..truncationr0..
 000013e0: 0029 02da 0974 6f6b 656e 697a 6572 da08  .)...tokenizer..
 000013f0: 6578 616d 706c 6573 7230 0000 0072 3000  examplesr0...r0.
 00001400: 0000 7231 0000 00da 1174 6f6b 656e 697a  ..r1.....tokeniz
 00001410: 655f 6675 6e63 7469 6f6e b000 0000 7302  e_function....s.
-00001420: 0000 0012 0172 7a00 0000 6302 0000 0000  .....rz...c.....
+00001420: 0000 0012 0172 7900 0000 6302 0000 0000  .....ry...c.....
 00001430: 0000 0000 0000 0005 0000 000a 0000 0043  ...............C
 00001440: 0000 0073 b200 0000 6401 7d02 7400 6a01  ...s....d.}.t.j.
 00001450: a002 7c02 a101 730d 7400 a003 7c02 a101  ..|...s.t...|...
 00001460: 0100 6401 7c01 a004 6402 6403 a102 1700  ..d.|...d.d.....
 00001470: 7d03 7400 6a01 a002 7c03 a101 7326 7405  }.t.j...|...s&t.
 00001480: 6404 7c03 1700 8301 0100 7400 a003 7c03  d.|.......t...|.
 00001490: a101 0100 7406 4400 5d2e 7d04 7a13 7400  ....t.D.].}.z.t.
@@ -347,694 +347,703 @@
 000015a0: 706f 696e 7473 5f66 6f6c 6465 725f 7061  points_folder_pa
 000015b0: 7468 5a13 6461 7461 7365 745f 666f 6c64  thZ.dataset_fold
 000015c0: 6572 5f70 6174 68da 0764 6174 6173 6574  er_path..dataset
 000015d0: 7230 0000 0072 3000 0000 7231 0000 00da  r0...r0...r1....
 000015e0: 0b63 6865 636b 706f 696e 7473 b500 0000  .checkpoints....
 000015f0: 731c 0000 0004 010c 010a 0110 020c 010c  s...............
 00001600: 010a 0108 0202 0126 0106 0108 0124 0104  .......&.....$..
-00001610: fb72 8500 0000 6301 0000 0000 0000 0000  .r....c.........
+00001610: fb72 8400 0000 6301 0000 0000 0000 0000  .r....c.........
 00001620: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
 00001630: 1a00 0000 6401 7d01 7400 6a01 7c00 7c01  ....d.}.t.j.|.|.
 00001640: 6402 8d02 7d02 7c02 7c01 6602 5300 2903  d...}.|.|.f.S.).
 00001650: 4e72 4e00 0000 2901 da10 6d6f 6465 6c5f  NrN...)...model_
 00001660: 6d61 785f 6c65 6e67 7468 2902 7206 0000  max_length).r...
 00001670: 0072 5500 0000 2903 7252 0000 0072 5600  .rU...).rR...rV.
-00001680: 0000 7278 0000 0072 3000 0000 7230 0000  ..rx...r0...r0..
+00001680: 0000 7277 0000 0072 3000 0000 7230 0000  ..rw...r0...r0..
 00001690: 0072 3100 0000 da0a 6c6f 6164 5f6d 6f64  .r1.....load_mod
 000016a0: 656c c800 0000 7306 0000 0004 010e 0108  el....s.........
-000016b0: 0272 8700 0000 630e 0000 0000 0000 0000  .r....c.........
-000016c0: 0000 0012 0000 0006 0000 0043 0000 0073  ...........C...s
-000016d0: 2201 0000 7400 6401 8301 0100 7400 6402  "...t.d.....t.d.
+000016b0: 0272 8600 0000 630e 0000 0000 0000 0000  .r....c.........
+000016c0: 0000 0013 0000 0006 0000 0043 0000 0073  ...........C...s
+000016d0: 5601 0000 7400 6401 8301 0100 7400 6402  V...t.d.....t.d.
 000016e0: 7401 7c02 8301 1700 8301 0100 7400 6401  t.|.........t.d.
 000016f0: 8301 0100 6403 6400 6c02 7d0e 7c0e 6a02  ....d.d.l.}.|.j.
 00001700: a003 a100 a004 6404 a101 7d0f 6405 7c03  ......d...}.d.|.
-00001710: a005 6406 6407 a102 1700 6406 1700 7c06  ..d.d.....d...|.
-00001720: 1700 6408 1700 7401 7c07 a006 6406 a101  ..d...t.|...d...
-00001730: 6409 1900 a005 640a 640b a102 8301 1700  d.....d.d.......
-00001740: 6408 1700 7c0f 1700 640c 1700 7d10 7407  d...|...d...}.t.
-00001750: a007 a100 7d11 7400 640d 7c00 1700 8301  ....}.t.d.|.....
-00001760: 0100 7400 640e 7c03 1700 8301 0100 7400  ..t.d.|.......t.
-00001770: 640f 7c07 1700 8301 0100 7400 6410 7401  d.|.......t.d.t.
-00001780: 7c04 8301 1700 8301 0100 7400 6411 7401  |.........t.d.t.
-00001790: 7c02 8301 1700 8301 0100 7400 6412 7c10  |.........t.d.|.
-000017a0: 1700 8301 0100 7400 6413 7401 7c08 8301  ......t.d.t.|...
-000017b0: 1700 8301 0100 7400 6414 7401 7c05 8301  ......t.d.t.|...
-000017c0: 1700 8301 0100 7400 6415 7401 7c09 8301  ......t.d.t.|...
-000017d0: 1700 8301 0100 7400 6416 7401 7c0a 8301  ......t.d.t.|...
-000017e0: 1700 8301 0100 7400 6401 8301 0100 7c10  ......t.d.....|.
-000017f0: 7c08 6602 5300 2917 4e7a 4a2d 2d2d 2d2d  |.f.S.).NzJ-----
-00001800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001710: a005 6406 6407 a102 1700 7d10 7406 6a07  ..d.d.....}.t.j.
+00001720: a008 7c10 a101 7336 7400 6408 7c10 9b00  ..|...s6t.d.|...
+00001730: 9d02 8301 0100 7406 a009 7c10 a101 0100  ......t...|.....
+00001740: 6405 7c03 a005 6406 6407 a102 1700 6406  d.|...d.d.....d.
+00001750: 1700 7c06 1700 6409 1700 7401 7c07 a00a  ..|...d...t.|...
+00001760: 6406 a101 640a 1900 a005 640b 640c a102  d...d.....d.d...
+00001770: 8301 1700 6409 1700 7c0f 1700 640d 1700  ....d...|...d...
+00001780: 7d11 740b a00b a100 7d12 7400 640e 7c00  }.t.....}.t.d.|.
+00001790: 1700 8301 0100 7400 640f 7c03 1700 8301  ......t.d.|.....
+000017a0: 0100 7400 6410 7c07 1700 8301 0100 7400  ..t.d.|.......t.
+000017b0: 6411 7401 7c04 8301 1700 8301 0100 7400  d.t.|.........t.
+000017c0: 6412 7401 7c02 8301 1700 8301 0100 7400  d.t.|.........t.
+000017d0: 6413 7c11 1700 8301 0100 7400 6414 7401  d.|.......t.d.t.
+000017e0: 7c08 8301 1700 8301 0100 7400 6415 7401  |.........t.d.t.
+000017f0: 7c05 8301 1700 8301 0100 7400 6416 7401  |.........t.d.t.
+00001800: 7c09 8301 1700 8301 0100 7400 6417 7401  |.........t.d.t.
+00001810: 7c0a 8301 1700 8301 0100 7400 6401 8301  |.........t.d...
+00001820: 0100 7c11 7c08 6602 5300 2918 4e7a 4a2d  ..|.|.f.S.).NzJ-
 00001830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001840: 2d2d 2d2d 2d7a 1c53 7461 7274 696e 6720  -----z.Starting 
-00001850: 6e65 7720 6c65 6172 6e69 6e67 2072 6174  new learning rat
-00001860: 653a 2072 0100 0000 7a11 2559 2d25 6d2d  e: r....z.%Y-%m-
-00001870: 2564 5f25 483a 254d 3a25 5372 7b00 0000  %d_%H:%M:%Sr{...
-00001880: 727c 0000 0072 1f00 0000 da01 5f72 3800  r|...r......_r8.
-00001890: 0000 7a04 2e74 7376 727d 0000 007a 032e  ..z..tsvr}...z..
-000018a0: 7074 7a09 4461 7461 7365 743a 207a 074d  ptz.Dataset: z.M
-000018b0: 6f64 656c 3a20 7a14 5465 7374 2053 6574  odel: z.Test Set
-000018c0: 2053 656c 6563 7469 6f6e 3a20 7a10 4e75   Selection: z.Nu
-000018d0: 6d62 6572 206f 6620 5275 6e73 3a20 7a0f  mber of Runs: z.
-000018e0: 4c65 6172 6e69 6e67 2052 6174 653a 20fa  Learning Rate: .
-000018f0: 1143 6865 636b 706f 696e 7420 5061 7468  .Checkpoint Path
-00001900: 3a20 7a0a 5061 7469 656e 6365 3a20 7a17  : z.Patience: z.
-00001910: 5661 6c69 6461 7469 6f6e 2053 6574 2043  Validation Set C
-00001920: 686f 6963 653a 207a 124e 756d 6265 7220  hoice: z.Number 
-00001930: 6f66 2045 706f 6368 733a 207a 184e 756d  of Epochs: z.Num
-00001940: 6265 7220 6f66 2077 6172 6d75 7020 7374  ber of warmup st
-00001950: 6570 733a 2029 0872 2c00 0000 722d 0000  eps: ).r,...r-..
-00001960: 00da 0864 6174 6574 696d 65da 036e 6f77  ...datetime..now
-00001970: da08 7374 7266 7469 6d65 7226 0000 0072  ..strftimer&...r
-00001980: 2900 0000 da04 7469 6d65 2912 7284 0000  ).....time).r...
-00001990: 00da 156c 6561 726e 696e 675f 7261 7465  ...learning_rate
-000019a0: 5f63 686f 6963 6573 da14 6368 6f73 656e  _choices..chosen
-000019b0: 5f6c 6561 726e 696e 675f 7261 7465 7252  _learning_raterR
-000019c0: 0000 00da 0e6e 756d 6265 725f 6f66 5f72  .....number_of_r
-000019d0: 756e 73da 1676 616c 6964 6174 696f 6e5f  uns..validation_
-000019e0: 7365 745f 7363 6f72 696e 67da 0c6c 6162  set_scoring..lab
-000019f0: 656c 5f63 6f6c 756d 6eda 0e76 616c 6964  el_column..valid
-00001a00: 6174 696f 6e5f 7365 74da 0e70 6174 6965  ation_set..patie
-00001a10: 6e63 655f 7661 6c75 65da 0a6e 756d 5f65  nce_value..num_e
-00001a20: 706f 6368 73da 106e 756d 5f77 6172 6d75  pochs..num_warmu
-00001a30: 705f 7374 6570 73da 2067 7261 6469 656e  p_steps. gradien
-00001a40: 745f 6163 6375 6d75 6c61 7469 6f6e 5f6d  t_accumulation_m
-00001a50: 756c 7469 706c 6965 72da 1361 7373 6967  ultiplier..assig
-00001a60: 6e65 645f 6261 7463 685f 7369 7a65 7278  ned_batch_sizerx
-00001a70: 0000 0072 8a00 0000 5a10 6375 7272 656e  ...r....Z.curren
-00001a80: 745f 6461 7465 7469 6d65 da0f 6368 6563  t_datetime..chec
-00001a90: 6b70 6f69 6e74 5f70 6174 685a 0f65 7865  kpoint_pathZ.exe
-00001aa0: 6375 7469 6f6e 5f73 7461 7274 7230 0000  cution_startr0..
-00001ab0: 0072 3000 0000 7231 0000 00da 1670 7265  .r0...r1.....pre
-00001ac0: 7061 7265 5f61 6e64 5f63 6c65 616e 5f64  pare_and_clean_d
-00001ad0: 6174 61d0 0000 0073 2600 0000 0806 1001  ata....s&.......
-00001ae0: 0801 0802 1002 4202 0808 0c02 0c01 0c01  ......B.........
-00001af0: 1001 1001 0c01 1001 1001 1001 1001 0801  ................
-00001b00: 0802 729a 0000 0063 0400 0000 0000 0000  ..r....c........
-00001b10: 0000 0000 0400 0000 0500 0000 0300 0000  ................
-00001b20: 7324 0100 0074 006a 017c 0064 0164 028d  s$...t.j.|.d.d..
-00001b30: 0289 0064 037c 0076 0072 1d88 0064 0419  ...d.|.v.r...d..
-00001b40: 0088 0064 053c 0088 0064 0619 0088 0064  ...d.<...d.....d
-00001b50: 073c 0088 0064 0819 0088 0064 093c 0088  .<...d.....d.<..
-00001b60: 0088 007c 0119 0064 0a6b 0319 0089 0088  ...|...d.k......
-00001b70: 0088 0064 0519 00a0 02a1 0019 0089 0088  ...d............
-00001b80: 0088 0064 0919 00a0 02a1 0019 0089 0088  ...d............
-00001b90: 0088 0064 0719 00a0 02a1 0019 0089 0088  ...d............
-00001ba0: 0088 007c 0119 00a0 02a1 0019 0089 0088  ...|............
-00001bb0: 006a 0374 0488 0083 0164 0b64 0c8d 0289  .j.t.....d.d....
-00001bc0: 0064 0d7c 0176 0072 6287 0066 0164 0e64  .d.|.v.rb..f.d.d
-00001bd0: 0f84 0874 0574 0488 0083 0183 0144 0083  ...t.t.......D..
-00001be0: 0188 0064 103c 006e 0f87 0066 0164 1164  ...d.<.n...f.d.d
-00001bf0: 0f84 0874 0574 0488 0083 0183 0144 0083  ...t.t.......D..
-00001c00: 0188 0064 103c 0087 0166 0164 1264 0f84  ...d.<...f.d.d..
-00001c10: 0874 0688 0064 1019 0064 1364 148d 0244  .t...d...d.d...D
-00001c20: 0083 0188 0064 153c 0088 00a0 0764 1067  .....d.<.....d.g
-00001c30: 01a1 0189 0088 0088 0064 1519 0064 166b  .........d...d.k
-00001c40: 0119 0089 0088 0053 0029 174e 721d 0000  .......S.).Nr...
-00001c50: 00a9 01da 0373 6570 da0e 6e71 5f72 6566  .....sep..nq_ref
-00001c60: 6f72 6d61 7474 6564 da05 5175 6572 79da  ormatted..Query.
-00001c70: 0f73 796e 7468 6574 6963 5f71 7565 7279  .synthetic_query
-00001c80: da06 416e 7377 6572 da10 6765 6e65 7261  ..Answer..genera
-00001c90: 7465 645f 616e 7377 6572 da08 446f 6375  ted_answer..Docu
-00001ca0: 6d65 6e74 7218 0000 00da 034e 614e 7236  mentr......NaNr6
-00001cb0: 0000 0029 02da 016e da0c 7261 6e64 6f6d  ...)...n..random
-00001cc0: 5f73 7461 7465 da07 436f 6e74 6578 7463  _state..Contextc
-00001cd0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001ce0: 0600 0000 1300 0000 f32a 0000 0067 007c  .........*...g.|
-00001cf0: 005d 117d 0174 0088 006a 017c 0119 0064  .].}.t...j.|...d
-00001d00: 0019 0088 006a 017c 0119 0064 0119 0083  .....j.|...d....
-00001d10: 0291 0271 0253 0029 0272 9f00 0000 7218  ...q.S.).r....r.
-00001d20: 0000 00a9 0272 3200 0000 da04 696c 6f63  .....r2.....iloc
-00001d30: a902 723b 0000 0072 3c00 0000 a901 da0d  ..r;...r<.......
-00001d40: 7379 6e74 685f 7175 6572 6965 7372 3000  synth_queriesr0.
-00001d50: 0000 7231 0000 0072 3e00 0000 1601 0000  ..r1...r>.......
-00001d60: f302 0000 002a 007a 2b61 6e61 6c79 7a65  .....*.z+analyze
-00001d70: 5f61 6e64 5f72 6570 6f72 745f 6461 7461  _and_report_data
-00001d80: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00001d90: 6f6d 703e da0b 636f 6e63 6174 5f74 6578  omp>..concat_tex
-00001da0: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
-00001db0: 0000 0700 0000 1300 0000 f336 0000 0067  ...........6...g
-00001dc0: 007c 005d 177d 0174 0088 006a 017c 0119  .|.].}.t...j.|..
-00001dd0: 0064 0019 0088 006a 017c 0119 0064 0119  .d.....j.|...d..
-00001de0: 0088 006a 017c 0119 0064 0219 0083 0391  ...j.|...d......
-00001df0: 0271 0253 0029 0372 9f00 0000 7218 0000  .q.S.).r....r...
-00001e00: 0072 a100 0000 72a8 0000 0072 aa00 0000  .r....r....r....
-00001e10: 72ab 0000 0072 3000 0000 7231 0000 0072  r....r0...r1...r
-00001e20: 3e00 0000 1801 0000 f302 0000 0036 0063  >............6.c
-00001e30: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001e40: 0700 0000 1300 0000 7322 0000 0067 007c  ........s"...g.|
-00001e50: 005d 0d7d 0174 0088 006a 017c 0164 0064  .].}.t...j.|.d.d
-00001e60: 018d 0264 0219 0083 0191 0271 0253 0029  ...d.......q.S.)
-00001e70: 03da 0270 7429 01da 0e72 6574 7572 6e5f  ...pt)...return_
-00001e80: 7465 6e73 6f72 7372 0100 0000 2902 722a  tensorsr....).r*
-00001e90: 0000 00da 0665 6e63 6f64 6529 0272 3b00  .....encode).r;.
-00001ea0: 0000 7274 0000 00a9 0172 7800 0000 7230  ..rt.....rx...r0
-00001eb0: 0000 0072 3100 0000 723e 0000 0019 0100  ...r1...r>......
-00001ec0: 0073 0200 0000 2200 5a0a 546f 6b65 6e69  .s....".Z.Tokeni
-00001ed0: 7a69 6e67 2901 da04 6465 7363 5a0c 746f  zing)...descZ.to
-00001ee0: 6b65 6e5f 6c65 6e67 7468 724e 0000 0029  ken_lengthrN...)
-00001ef0: 08da 0270 64da 0872 6561 645f 6373 76da  ...pd..read_csv.
-00001f00: 056e 6f74 6e61 da06 7361 6d70 6c65 722a  .notna..sampler*
-00001f10: 0000 00da 0572 616e 6765 7212 0000 00da  .....ranger.....
-00001f20: 0f64 726f 705f 6475 706c 6963 6174 6573  .drop_duplicates
-00001f30: 2904 7284 0000 0072 9200 0000 7278 0000  ).r....r....rx..
-00001f40: 0072 5600 0000 7230 0000 0029 0272 ac00  .rV...r0...).r..
-00001f50: 0000 7278 0000 0072 3100 0000 da17 616e  ..rx...r1.....an
-00001f60: 616c 797a 655f 616e 645f 7265 706f 7274  alyze_and_report
-00001f70: 5f64 6174 61f8 0000 0073 2400 0000 0e02  _data....s$.....
-00001f80: 0802 0c01 0c01 0c01 1007 1001 1001 1001  ................
-00001f90: 1001 1201 080a 2001 1e02 2201 0c01 1007  ...... ...".....
-00001fa0: 0402 72bc 0000 0063 0300 0000 0000 0000  ..r....c........
-00001fb0: 0000 0000 0500 0000 0600 0000 0300 0000  ................
-00001fc0: 7360 0100 007c 007d 0374 006a 017c 0164  s`...|.}.t.j.|.d
-00001fd0: 0164 028d 0289 0088 0064 0319 0088 0064  .d.......d.....d
-00001fe0: 043c 0088 0064 0519 006a 02a0 03a1 0088  .<...d...j......
-00001ff0: 0064 053c 0088 0088 0064 0519 006a 02a0  .d.<.....d...j..
-00002000: 04a1 0064 066b 0419 0089 0088 0088 007c  ...d.k.........|
-00002010: 0219 00a0 05a1 0019 0089 007c 0364 0719  ...........|.d..
-00002020: 00a0 0674 02a1 016a 02a0 03a1 007c 0364  ...t...j.....|.d
-00002030: 073c 007c 037c 0364 0719 006a 02a0 04a1  .<.|.|.d...j....
-00002040: 0064 066b 0419 007d 037c 037c 037c 0219  .d.k...}.|.|.|..
-00002050: 00a0 05a1 0019 007d 0364 087c 0276 0072  .......}.d.|.v.r
-00002060: 5e87 0066 0164 0964 0a84 0874 0774 0488  ^..f.d.d...t.t..
-00002070: 0083 0183 0144 0083 0188 0064 0b3c 006e  .....D.....d.<.n
-00002080: 0f87 0066 0164 0c64 0a84 0874 0774 0488  ...f.d.d...t.t..
-00002090: 0083 0183 0144 0083 0188 0064 0b3c 007c  .....D.....d.<.|
-000020a0: 03a0 0864 0b67 01a1 017d 0388 00a0 0864  ...d.g...}.....d
-000020b0: 0b67 01a1 0189 0064 0d7c 0276 0072 ac74  .g.....d.|.v.r.t
-000020c0: 0964 0e83 0101 007c 037c 0364 0f19 00a0  .d.....|.|.d....
-000020d0: 05a1 0019 007d 037c 037c 0364 1019 00a0  .....}.|.|.d....
-000020e0: 05a1 0019 007d 0367 0064 11a2 017d 047c  .....}.g.d...}.|
-000020f0: 0364 1219 00a0 0674 02a1 017c 0364 123c  .d.....t...|.d.<
-00002100: 007c 037c 0364 1219 006a 02a0 0a64 13a0  .|.|.d...j...d..
-00002110: 0b7c 04a1 01a1 010f 0019 007d 037c 0388  .|.........}.|..
-00002120: 0066 0253 0029 144e 721d 0000 0072 9b00  .f.S.).Nr....r..
-00002130: 0000 729e 0000 00da 0851 7565 7374 696f  ..r......Questio
-00002140: 6e72 a200 0000 7222 0000 0072 1800 0000  nr....r"...r....
-00002150: 72a6 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00002160: 0000 0200 0000 0600 0000 1300 0000 72a7  ..............r.
-00002170: 0000 0029 0272 bd00 0000 72a2 0000 0072  ...).r....r....r
-00002180: a800 0000 72aa 0000 00a9 01da 0874 6573  ....r........tes
-00002190: 745f 7365 7472 3000 0000 7231 0000 0072  t_setr0...r1...r
-000021a0: 3e00 0000 3601 0000 72ad 0000 007a 2274  >...6...r....z"t
-000021b0: 7261 6e73 666f 726d 5f64 6174 612e 3c6c  ransform_data.<l
-000021c0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-000021d0: 3e72 ae00 0000 6301 0000 0000 0000 0000  >r....c.........
-000021e0: 0000 0002 0000 0007 0000 0013 0000 0072  ...............r
-000021f0: af00 0000 2903 72bd 0000 0072 a200 0000  ....).r....r....
-00002200: 72a0 0000 0072 a800 0000 72aa 0000 0072  r....r....r....r
-00002210: be00 0000 7230 0000 0072 3100 0000 723e  ....r0...r1...r>
-00002220: 0000 0038 0100 0072 b000 0000 5a05 4661  ...8...r....Z.Fa
-00002230: 6974 687a 3552 6566 696e 696e 6720 6461  ithz5Refining da
-00002240: 7461 2066 6f72 2041 6e73 7765 725f 4661  ta for Answer_Fa
-00002250: 6974 6866 756c 6e65 7373 2063 6c61 7373  ithfulness class
-00002260: 6966 6963 6174 696f 6e21 da17 436f 6e74  ification!..Cont
-00002270: 6578 745f 5265 6c65 7661 6e63 655f 4c61  ext_Relevance_La
-00002280: 6265 6cda 1941 6e73 7765 725f 4661 6974  bel..Answer_Fait
-00002290: 6866 756c 6e65 7373 5f4c 6162 656c 290a  hfulness_Label).
-000022a0: 722e 0000 005a 0763 6f6e 7472 6164 da05  r....Z.contrad..
-000022b0: 6661 6c73 655a 0b69 6e66 6f72 6d61 7469  falseZ.informati
-000022c0: 6f6e 5a08 756e 616e 7377 6572 72a0 0000  onZ.unanswerr...
-000022d0: 005a 0743 6f6e 7472 6164 da05 4661 6c73  .Z.Contrad..Fals
-000022e0: 655a 0b49 6e66 6f72 6d61 7469 6f6e 5a08  eZ.InformationZ.
-000022f0: 556e 616e 7377 6572 72a1 0000 00da 017c  Unanswerr......|
-00002300: 290c 72b6 0000 0072 b700 0000 722d 0000  ).r....r....r-..
-00002310: 0072 2700 0000 722a 0000 0072 b800 0000  .r'...r*...r....
-00002320: da06 6173 7479 7065 72ba 0000 0072 bb00  ..astyper....r..
-00002330: 0000 722c 0000 00da 0863 6f6e 7461 696e  ..r,.....contain
-00002340: 7372 2800 0000 2905 72ac 0000 0072 9300  sr(...).r....r..
-00002350: 0000 7292 0000 00da 0874 7261 696e 5f64  ..r......train_d
-00002360: 665a 0d65 7272 6f72 5f73 7472 696e 6773  fZ.error_strings
-00002370: 7230 0000 0072 be00 0000 7231 0000 00da  r0...r....r1....
-00002380: 0e74 7261 6e73 666f 726d 5f64 6174 6127  .transform_data'
-00002390: 0100 0073 2c00 0000 0402 0e02 0c01 1201  ...s,...........
-000023a0: 1601 1001 1802 1601 1001 0802 2001 1e02  ............ ...
-000023b0: 0c02 0c01 0802 0801 1001 1001 0801 1201  ................
-000023c0: 1c01 0802 72c8 0000 0063 0400 0000 0000  ....r....c......
-000023d0: 0000 0000 0000 0b00 0000 0700 0000 0300  ................
-000023e0: 0000 7306 0100 0064 0164 0264 039c 0289  ..s....d.d.d....
-000023f0: 0087 0366 0164 0464 0584 0874 0074 0188  ...f.d.d...t.t..
-00002400: 0383 0183 0144 0083 017d 0464 067c 0176  .....D...}.d.|.v
-00002410: 0172 2687 0087 0187 0366 0364 0764 0584  .r&......f.d.d..
-00002420: 0874 0074 0188 0383 0183 0144 0083 017d  .t.t.......D...}
-00002430: 056e 0e87 0187 0366 0264 0864 0584 0874  .n.....f.d.d...t
-00002440: 0074 0188 0383 0183 0144 0083 017d 0587  .t.......D...}..
-00002450: 0266 0164 0964 0584 0874 0074 0188 0283  .f.d.d...t.t....
-00002460: 0183 0144 0083 017d 0687 0187 0266 0264  ...D...}.....f.d
-00002470: 0a64 0584 0874 0074 0188 0283 0183 0144  .d...t.t.......D
-00002480: 0083 017d 0787 0266 0164 0b64 0584 0874  ...}...f.d.d...t
-00002490: 0074 0188 0283 0183 0144 0083 017d 0887  .t.......D...}..
-000024a0: 0187 0266 0264 0c64 0584 0874 0074 0188  ...f.d.d...t.t..
-000024b0: 0283 0183 0144 0083 017d 0974 0264 0d83  .....D...}.t.d..
-000024c0: 0101 0074 0374 0474 057c 057c 0717 007c  ...t.t.t.|.|...|
-000024d0: 0917 0083 0183 0183 017d 0a7c 047c 057c  .........}.|.|.|
-000024e0: 067c 077c 087c 097c 0a66 0753 0029 0e4e  .|.|.|.|.f.S.).N
-000024f0: 7239 0000 0072 0100 0000 2902 da03 5965  r9...r....)...Ye
-00002500: 73da 024e 6f63 0100 0000 0000 0000 0000  s..Noc..........
-00002510: 0000 0200 0000 0400 0000 1300 0000 f31a  ................
-00002520: 0000 0067 007c 005d 097d 0188 006a 007c  ...g.|.].}...j.|
-00002530: 0119 0064 0019 0091 0271 0253 00a9 0172  ...d.....q.S...r
-00002540: ae00 0000 a901 72a9 0000 0072 aa00 0000  ......r....r....
-00002550: 2901 72c7 0000 0072 3000 0000 7231 0000  ).r....r0...r1..
-00002560: 0072 3e00 0000 4b01 0000 f302 0000 001a  .r>...K.........
-00002570: 007a 2173 706c 6974 5f64 6174 6173 6574  .z!split_dataset
-00002580: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00002590: 6f6d 703e 729d 0000 0063 0100 0000 0000  omp>r....c......
-000025a0: 0000 0000 0000 0200 0000 0500 0000 1300  ................
-000025b0: 0000 731e 0000 0067 007c 005d 0b7d 0188  ..s....g.|.].}..
-000025c0: 0088 026a 007c 0119 0088 0119 0019 0091  ...j.|..........
-000025d0: 0271 0253 0072 3000 0000 72cd 0000 0072  .q.S.r0...r....r
-000025e0: aa00 0000 2903 da0f 636f 6e76 6572 7369  ....)...conversi
-000025f0: 6f6e 5f64 6963 7472 9200 0000 72c7 0000  on_dictr....r...
-00002600: 0072 3000 0000 7231 0000 0072 3e00 0000  .r0...r1...r>...
-00002610: 4d01 0000 f302 0000 001e 0063 0100 0000  M..........c....
-00002620: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00002630: 1300 0000 f31e 0000 0067 007c 005d 0b7d  .........g.|.].}
-00002640: 0174 0088 016a 017c 0119 0088 0019 0083  .t...j.|........
-00002650: 0191 0271 0253 0072 3000 0000 a902 723a  ...q.S.r0.....r:
-00002660: 0000 0072 a900 0000 72aa 0000 0029 0272  ...r....r....).r
-00002670: 9200 0000 72c7 0000 0072 3000 0000 7231  ....r....r0...r1
-00002680: 0000 0072 3e00 0000 4f01 0000 72d0 0000  ...r>...O...r...
-00002690: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-000026a0: 0000 0400 0000 1300 0000 72cb 0000 0072  ..........r....r
-000026b0: cc00 0000 72cd 0000 0072 aa00 0000 72be  ....r....r....r.
-000026c0: 0000 0072 3000 0000 7231 0000 0072 3e00  ...r0...r1...r>.
-000026d0: 0000 5301 0000 72ce 0000 0063 0100 0000  ..S...r....c....
-000026e0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-000026f0: 1300 0000 72d1 0000 0072 3000 0000 72d2  ....r....r0...r.
-00002700: 0000 0072 aa00 0000 a902 7292 0000 0072  ...r......r....r
-00002710: bf00 0000 7230 0000 0072 3100 0000 723e  ....r0...r1...r>
-00002720: 0000 0054 0100 0072 d000 0000 6301 0000  ...T...r....c...
-00002730: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00002740: 0013 0000 0072 cb00 0000 72cc 0000 0072  .....r....r....r
-00002750: cd00 0000 72aa 0000 0072 be00 0000 7230  ....r....r....r0
-00002760: 0000 0072 3100 0000 723e 0000 0058 0100  ...r1...r>...X..
-00002770: 0072 ce00 0000 6301 0000 0000 0000 0000  .r....c.........
-00002780: 0000 0002 0000 0005 0000 0013 0000 0072  ...............r
-00002790: d100 0000 7230 0000 0072 d200 0000 72aa  ....r0...r....r.
-000027a0: 0000 0072 d300 0000 7230 0000 0072 3100  ...r....r0...r1.
-000027b0: 0000 723e 0000 0059 0100 0072 d000 0000  ..r>...Y...r....
-000027c0: 7a33 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  z3--------------
-000027d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000027e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000027f0: 2d2d 2d2d 2d29 0672 ba00 0000 722a 0000  -----).r....r*..
-00002800: 0072 2c00 0000 da06 736f 7274 6564 da04  .r,.....sorted..
-00002810: 6c69 7374 da03 7365 7429 0b72 c700 0000  list..set).r....
-00002820: 7284 0000 0072 bf00 0000 7292 0000 00da  r....r....r.....
-00002830: 0e74 7261 696e 5f73 6574 5f74 6578 74da  .train_set_text.
-00002840: 0f74 7261 696e 5f73 6574 5f6c 6162 656c  .train_set_label
-00002850: da0c 6465 765f 7365 745f 7465 7874 da0d  ..dev_set_text..
-00002860: 6465 765f 7365 745f 6c61 6265 6cda 0d74  dev_set_label..t
-00002870: 6573 745f 7365 745f 7465 7874 da0e 7465  est_set_text..te
-00002880: 7374 5f73 6574 5f6c 6162 656c da0b 6c61  st_set_label..la
-00002890: 6265 6c73 5f6c 6973 7472 3000 0000 2904  bels_listr0...).
-000028a0: 72cf 0000 0072 9200 0000 72bf 0000 0072  r....r....r....r
-000028b0: c700 0000 7231 0000 00da 0d73 706c 6974  ....r1.....split
-000028c0: 5f64 6174 6173 6574 4901 0000 7318 0000  _datasetI...s...
-000028d0: 000a 011a 0108 0120 011c 021a 041c 011a  ....... ........
-000028e0: 041c 0108 0218 0b12 0872 de00 0000 6305  .........r....c.
-000028f0: 0000 0000 0000 0000 0000 000b 0000 0005  ................
-00002900: 0000 0043 0000 0073 fc00 0000 7c00 6401  ...C...s....|.d.
-00002910: 6b02 723e 7400 a001 7c01 7c02 6402 9c02  k.r>t...|.|.d...
-00002920: a101 7d05 7402 6a03 a004 7c05 a101 7d06  ..}.t.j...|...}.
-00002930: 7405 a006 7c06 a101 7d06 7400 a001 7c03  t...|...}.t...|.
-00002940: 7c04 6402 9c02 a101 7d07 7402 6a03 a004  |.d.....}.t.j...
-00002950: 7c07 a101 7d08 7405 a006 7c08 a101 7d08  |...}.t...|...}.
-00002960: 7400 a001 7c03 7c04 6402 9c02 a101 7d09  t...|.|.d.....}.
-00002970: 7402 6a03 a004 7c09 a101 7d0a 7405 a006  t.j...|...}.t...
-00002980: 7c0a a101 7d0a 6e39 7400 a001 7c01 7c02  |...}.n9t...|.|.
-00002990: 6402 9c02 a101 7d05 7402 6a03 a004 7c05  d.....}.t.j...|.
-000029a0: a101 7d06 7405 a006 7c06 a101 7d06 7400  ..}.t...|...}.t.
-000029b0: a001 7c03 7c04 6402 9c02 a101 7d07 7402  ..|.|.d.....}.t.
-000029c0: 6a03 a004 7c07 a101 7d08 7405 a006 7c08  j...|...}.t...|.
-000029d0: a101 7d08 7400 a001 7407 7408 6402 9c02  ..}.t...t.t.d...
-000029e0: a101 7d09 7402 6a03 a004 7c09 a101 7d0a  ..}.t.j...|...}.
-000029f0: 7405 a006 7c0a a101 7d0a 7c05 7c06 7c08  t...|...}.|.|.|.
-00002a00: 7c0a 7c09 6605 5300 2903 4e54 2902 da05  |.|.f.S.).NT)...
-00002a10: 6c61 6265 6c72 7400 0000 2909 72b6 0000  labelrt...).r...
-00002a20: 00da 0944 6174 6146 7261 6d65 da02 7061  ...DataFrame..pa
-00002a30: da05 5461 626c 65da 0b66 726f 6d5f 7061  ..Table..from_pa
-00002a40: 6e64 6173 da08 6461 7461 7365 7473 da07  ndas..datasets..
-00002a50: 4461 7461 7365 7472 dc00 0000 72db 0000  Datasetr....r...
-00002a60: 0029 0b72 9100 0000 72d8 0000 0072 d700  .).r....r....r..
-00002a70: 0000 72da 0000 0072 d900 0000 da17 7472  ..r....r......tr
-00002a80: 6169 6e69 6e67 5f64 6174 6173 6574 5f70  aining_dataset_p
-00002a90: 616e 6461 73da 1674 7261 696e 696e 675f  andas..training_
-00002aa0: 6461 7461 7365 745f 6172 726f 775a 1976  dataset_arrowZ.v
-00002ab0: 616c 6964 6174 696f 6e5f 6461 7461 7365  alidation_datase
-00002ac0: 745f 7061 6e64 6173 da18 7661 6c69 6461  t_pandas..valida
-00002ad0: 7469 6f6e 5f64 6174 6173 6574 5f61 7272  tion_dataset_arr
-00002ae0: 6f77 da13 7465 7374 5f64 6174 6173 6574  ow..test_dataset
-00002af0: 5f70 616e 6461 73da 1274 6573 745f 6461  _pandas..test_da
-00002b00: 7461 7365 745f 6172 726f 7772 3000 0000  taset_arrowr0...
-00002b10: 7230 0000 0072 3100 0000 da0f 7072 6570  r0...r1.....prep
-00002b20: 6172 655f 6461 7461 7365 7472 0100 0073  are_datasetr...s
-00002b30: 2800 0000 0801 1002 0c01 0a01 1002 0c01  (...............
-00002b40: 0a01 1002 0c01 0c01 1004 0c01 0a01 1002  ................
-00002b50: 0c01 0a01 1002 0c01 0a01 0e02 72eb 0000  ............r...
-00002b60: 0063 0400 0000 0000 0000 0000 0000 0600  .c..............
-00002b70: 0000 0600 0000 0300 0000 734e 0000 0074  ..........sN...t
-00002b80: 00a0 017c 017c 027c 0364 019c 03a1 017d  ...|.|.|.d.....}
-00002b90: 047c 046a 0287 0066 0164 0264 0384 0864  .|.j...f.d.d...d
-00002ba0: 0464 058d 027d 057c 05a0 0364 0667 01a1  .d...}.|...d.g..
-00002bb0: 017d 057c 05a0 0464 0764 08a1 027d 057c  .}.|...d.d...}.|
-00002bc0: 05a0 0564 09a1 0101 007c 0553 0029 0a4e  ...d.....|.S.).N
-00002bd0: 2903 da05 7472 6169 6eda 0a76 616c 6964  )...train..valid
-00002be0: 6174 696f 6eda 0474 6573 7463 0100 0000  ation..testc....
-00002bf0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00002c00: 1300 0000 730a 0000 0074 0088 007c 0083  ....s....t...|..
-00002c10: 0253 00a9 014e 2901 727a 0000 0029 0172  .S...N).rz...).r
-00002c20: 7900 0000 72b4 0000 0072 3000 0000 7231  y...r....r0...r1
-00002c30: 0000 00da 083c 6c61 6d62 6461 3e98 0100  .....<lambda>...
-00002c40: 0073 0200 0000 0a00 7a34 696e 6974 616c  .s......z4inital
-00002c50: 697a 655f 6461 7461 7365 745f 666f 725f  ize_dataset_for_
-00002c60: 746f 6b65 6e69 7a61 7469 6f6e 2e3c 6c6f  tokenization.<lo
-00002c70: 6361 6c73 3e2e 3c6c 616d 6264 613e 5429  cals>.<lambda>T)
-00002c80: 01da 0762 6174 6368 6564 7274 0000 0072  ...batchedrt...r
-00002c90: df00 0000 726d 0000 0072 5800 0000 2906  ....rm...rX...).
-00002ca0: 72e4 0000 00da 0b44 6174 6173 6574 4469  r......DatasetDi
-00002cb0: 6374 da03 6d61 70da 0e72 656d 6f76 655f  ct..map..remove_
-00002cc0: 636f 6c75 6d6e 73da 0d72 656e 616d 655f  columns..rename_
-00002cd0: 636f 6c75 6d6e da0a 7365 745f 666f 726d  column..set_form
-00002ce0: 6174 2906 7278 0000 0072 e700 0000 72e8  at).rx...r....r.
-00002cf0: 0000 0072 ea00 0000 7283 0000 00da 1274  ...r....r......t
-00002d00: 6f6b 656e 697a 6564 5f64 6174 6173 6574  okenized_dataset
-00002d10: 7372 3000 0000 72b4 0000 0072 3100 0000  sr0...r....r1...
-00002d20: da22 696e 6974 616c 697a 655f 6461 7461  ."initalize_data
-00002d30: 7365 745f 666f 725f 746f 6b65 6e69 7a61  set_for_tokeniza
-00002d40: 7469 6f6e 9201 0000 7312 0000 0006 0202  tion....s.......
-00002d50: 0102 0108 fe16 040c 020c 010a 0104 0272  ...............r
-00002d60: f800 0000 630c 0000 0000 0000 0000 0000  ....c...........
-00002d70: 002b 0000 000b 0000 0043 0000 0073 ac03  .+.......C...s..
-00002d80: 0000 6700 7d0c 6700 7d0d 6700 7d0e 7400  ..g.}.g.}.g.}.t.
-00002d90: 6401 7c00 8302 4400 9001 5dc7 7d0f 7401  d.|...D...].}.t.
-00002da0: a001 a100 7d10 7402 6402 8301 0100 7403  ....}.t.d.....t.
-00002db0: 7c01 6403 1900 7c02 6404 8d02 7d11 7403  |.d...|.d...}.t.
-00002dc0: 7c01 6405 1900 7c02 6404 8d02 7d12 7403  |.d...|.d...}.t.
-00002dd0: 7c01 6406 1900 7c02 6404 8d02 7d13 7404  |.d...|.d...}.t.
-00002de0: 7405 7406 7c03 8301 8301 7c04 8302 7d14  t.t.|.....|...}.
-00002df0: 7c14 a007 7c06 a101 0100 7408 a009 a100  |...|.....t.....
-00002e00: 7d15 740a 7c14 a00b a100 7c05 6407 8d02  }.t.|.....|.d...
-00002e10: 7d16 7c09 7405 7c11 8301 1400 7d17 740c  }.|.t.|.....}.t.
-00002e20: 6408 7c16 7c0a 7c17 6409 8d04 7d18 6700  d.|.|.|.d...}.g.
-00002e30: 7d19 6700 7d1a 6700 7d1b 6700 7d1c 6401  }.g.}.g.}.g.}.d.
-00002e40: 640a 6c0d 6d0e 7d1d 0100 7c1d 7c08 640b  d.l.m.}...|.|.d.
-00002e50: 7c07 640c 8d03 7d1e 7402 640d 7c07 1700  |.d...}.t.d.|...
-00002e60: 8301 0100 7402 640e 8301 0100 6401 7d1f  ....t.d.....d.}.
-00002e70: 7400 7c09 8301 4400 9001 5d4e 7d20 7c1f  t.|...D...]N} |.
-00002e80: 640f 3700 7d1f 7402 6410 740f 7c20 8301  d.7.}.t.d.t.| ..
-00002e90: 1700 8301 0100 7410 7400 7405 7c11 8301  ......t.t.t.|...
-00002ea0: 8301 8301 7d21 6401 7d22 7c14 a011 a100  ....}!d.}"|.....
-00002eb0: 0100 7c11 4400 5d5e 7d23 7c04 6411 7600  ..|.D.]^}#|.d.v.
-00002ec0: 72b2 7c23 6412 1900 a007 7c06 a101 7c23  r.|#d.....|...|#
-00002ed0: 6413 1900 a012 a100 a007 7c06 a101 6414  d.........|...d.
-00002ee0: 9c02 7d24 6e0f 7c23 6412 1900 a007 7c06  ..}$n.|#d.....|.
-00002ef0: a101 7c23 6413 1900 a007 7c06 a101 6414  ..|#d.....|...d.
-00002f00: 9c02 7d24 7c14 6421 6900 7c24 a401 8e01  ..}$|.d!i.|$....
-00002f10: 7d25 7c15 7c25 7c23 6415 1900 a007 7c06  }%|.|%|#d.....|.
-00002f20: a101 8302 7d26 7c26 a013 a100 0100 7c22  ....}&|&......|"
-00002f30: 640f 3700 7d22 7c22 7c0b 1600 6401 6b02  d.7.}"|"|...d.k.
-00002f40: 72ec 7c16 a014 a100 0100 7c18 a014 a100  r.|.......|.....
-00002f50: 0100 7c16 a015 a100 0100 7c21 a016 640f  ..|.......|!..d.
-00002f60: a101 0100 7c19 a017 7c26 a018 a100 a101  ....|...|&......
-00002f70: 0100 719a 7410 7400 7405 7c12 8301 8301  ..q.t.t.t.|.....
-00002f80: 8301 7d21 7c14 a019 a100 0100 7c12 4400  ..}!|.......|.D.
-00002f90: 5d73 7d23 741a a01b a100 8f63 0100 7c04  ]s}#t......c..|.
-00002fa0: 6411 7600 9001 7225 7c23 6412 1900 a007  d.v...r%|#d.....
-00002fb0: 7c06 a101 7c23 6413 1900 a012 a100 a007  |...|#d.........
-00002fc0: 7c06 a101 6414 9c02 7d24 6e0f 7c23 6412  |...d...}$n.|#d.
-00002fd0: 1900 a007 7c06 a101 7c23 6413 1900 a007  ....|...|#d.....
-00002fe0: 7c06 a101 6414 9c02 7d24 7c04 6416 7600  |...d...}$|.d.v.
-00002ff0: 9001 724c 7c23 6415 1900 a01c 7c23 6415  ..rL|#d.....|#d.
-00003000: 1900 6a1d 6401 1900 640f a102 a007 7c06  ..j.d...d.....|.
-00003010: a101 6601 7c24 6417 3c00 7c14 6421 6900  ..f.|$d.<.|.d!i.
-00003020: 7c24 a401 8e01 7d25 7c15 7c25 7c23 6415  |$....}%|.|%|#d.
-00003030: 1900 a007 7c06 a101 8302 7d26 7c21 a016  ....|.....}&|!..
-00003040: 640f a101 0100 7c1a a017 7c26 a018 a100  d.....|...|&....
-00003050: a101 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00003060: 6e09 3100 9001 7374 7701 0100 0100 0100  n.1...stw.......
-00003070: 5900 0100 9001 7107 741e a01f 7c19 a101  Y.....q.t...|...
-00003080: 7d27 741e a01f 7c1a a101 7d28 7c1b a017  }'t...|...}(|...
-00003090: 7c27 a101 0100 7c1c a017 7c28 a101 0100  |'....|...|(....
-000030a0: 7405 740f 7c09 8301 8301 7d29 6418 7c20  t.t.|.....})d.| 
-000030b0: 6419 7c29 9b00 9d02 9b04 641a 7c09 6419  d.|)......d.|.d.
-000030c0: 7c29 9b00 9d02 9b04 641b 9d05 641c 7c27  |)......d...d.|'
-000030d0: 641d 9b04 641e 9d03 1700 641f 7c28 641d  d...d.....d.|(d.
-000030e0: 9b04 9d02 1700 7d2a 7402 7c2a 8301 0100  ......}*t.|*....
-000030f0: 6700 7d19 6700 7d1a 7c1e 7c28 7c14 8302  g.}.g.}.|.|(|...
-00003100: 0100 7c1e 6a20 9001 72ca 7402 6420 8301  ..|.j ..r.t.d ..
-00003110: 0100 0100 6e01 717b 7c14 7c1b 7c1c 7c13  ....n.q{|.|.|.|.
-00003120: 7c0e 6605 0200 0100 5300 6400 5300 2922  |.f.....S.d.S.)"
-00003130: 4e72 0100 0000 7a0d 4c6f 6164 696e 6720  Nr....z.Loading 
-00003140: 4d6f 6465 6c72 ec00 0000 2901 da0a 6261  Modelr....)...ba
-00003150: 7463 685f 7369 7a65 72ed 0000 0072 ee00  tch_sizer....r..
-00003160: 0000 2901 da02 6c72 da06 6c69 6e65 6172  ..)...lr..linear
-00003170: 2904 da04 6e61 6d65 da09 6f70 7469 6d69  )...name..optimi
-00003180: 7a65 7272 9600 0000 da12 6e75 6d5f 7472  zerr......num_tr
-00003190: 6169 6e69 6e67 5f73 7465 7073 2901 da0d  aining_steps)...
-000031a0: 4561 726c 7953 746f 7070 696e 6754 2903  EarlyStoppingT).
-000031b0: da08 7061 7469 656e 6365 da07 7665 7262  ..patience..verb
-000031c0: 6f73 6572 7f00 0000 7289 0000 007a 1242  oser....r....z.B
-000031d0: 6567 696e 6e69 6e67 2054 7261 696e 696e  eginning Trainin
-000031e0: 6772 3900 0000 7a0f 4375 7272 656e 7420  gr9...z.Current 
-000031f0: 4570 6f63 683a 2072 4c00 0000 7267 0000  Epoch: rL...rg..
-00003200: 0072 6800 0000 a902 726b 0000 0072 6c00  .rh.....rk...rl.
-00003210: 0000 726d 0000 00a9 0372 6600 0000 7250  ..rm.....rf...rP
-00003220: 0000 0072 4f00 0000 726e 0000 00da 015b  ...rO...rn.....[
-00003230: da01 3e72 7c00 0000 7a02 5d20 7a0c 7472  ..>r|...z.] z.tr
-00003240: 6169 6e5f 6c6f 7373 3a20 7a03 2e35 6672  ain_loss: z..5fr
-00003250: 1c00 0000 7a0c 7661 6c69 645f 6c6f 7373  ....z.valid_loss
-00003260: 3a20 7a0e 4561 726c 7920 7374 6f70 7069  : z.Early stoppi
-00003270: 6e67 7230 0000 0029 2172 ba00 0000 728d  ngr0...)!r....r.
-00003280: 0000 0072 2c00 0000 720d 0000 0072 4500  ...r,...r....rE.
-00003290: 0000 722a 0000 0072 d600 0000 da02 746f  ..r*...r......to
-000032a0: 725d 0000 00da 1043 726f 7373 456e 7472  r].....CrossEntr
-000032b0: 6f70 794c 6f73 7372 0c00 0000 da0a 7061  opyLossr......pa
-000032c0: 7261 6d65 7465 7273 720e 0000 005a 2b61  rametersr....Z+a
-000032d0: 7265 732e 4c4c 4d5f 6173 5f61 5f4a 7564  res.LLM_as_a_Jud
-000032e0: 6765 5f41 6461 7074 6174 696f 6e2e 7079  ge_Adaptation.py
-000032f0: 746f 7263 6874 6f6f 6c73 72ff 0000 0072  torchtoolsr....r
-00003300: 2d00 0000 7212 0000 0072 ec00 0000 da04  -...r....r......
-00003310: 626f 6f6c da08 6261 636b 7761 7264 da04  bool..backward..
-00003320: 7374 6570 da09 7a65 726f 5f67 7261 64da  step..zero_grad.
-00003330: 0675 7064 6174 65da 0661 7070 656e 64da  .update..append.
-00003340: 0469 7465 6dda 0465 7661 6c72 5800 0000  .item..evalrX...
-00003350: da07 6e6f 5f67 7261 64da 0772 6573 6861  ..no_grad..resha
-00003360: 7065 da05 7368 6170 65da 026e 70da 0761  pe..shape..np..a
-00003370: 7665 7261 6765 5a0a 6561 726c 795f 7374  verageZ.early_st
-00003380: 6f70 292b 7290 0000 0072 f700 0000 7298  op)+r....r....r.
-00003390: 0000 0072 d800 0000 7252 0000 0072 8f00  ...r....rR...r..
-000033a0: 0000 da06 6465 7669 6365 7299 0000 0072  ....devicer....r
-000033b0: 9400 0000 7295 0000 0072 9600 0000 7297  ....r....r....r.
-000033c0: 0000 005a 0e6d 6963 726f 5f61 7665 7261  ...Z.micro_avera
-000033d0: 6765 735a 0e6d 6163 726f 5f61 7665 7261  gesZ.macro_avera
-000033e0: 6765 73da 0f69 6e66 6572 656e 6365 5f74  ges..inference_t
-000033f0: 696d 6573 723c 0000 005a 0972 756e 5f73  imesr<...Z.run_s
-00003400: 7461 7274 5a10 7472 6169 6e5f 6461 7461  tartZ.train_data
-00003410: 6c6f 6164 6572 5a15 7661 6c69 6461 7469  loaderZ.validati
-00003420: 6f6e 5f64 6174 616c 6f61 6465 72da 0f65  on_dataloader..e
-00003430: 7661 6c5f 6461 7461 6c6f 6164 6572 da05  val_dataloader..
-00003440: 6d6f 6465 6c5a 0963 7269 7465 7269 6f6e  modelZ.criterion
-00003450: 72fd 0000 0072 fe00 0000 da0c 6c72 5f73  r....r......lr_s
-00003460: 6368 6564 756c 6572 5a0c 7472 6169 6e5f  chedulerZ.train_
-00003470: 6c6f 7373 6573 5a0c 7661 6c69 645f 6c6f  lossesZ.valid_lo
-00003480: 7373 6573 da10 6176 675f 7472 6169 6e5f  sses..avg_train_
-00003490: 6c6f 7373 6573 da10 6176 675f 7661 6c69  losses..avg_vali
-000034a0: 645f 6c6f 7373 6573 72ff 0000 00da 0e65  d_lossesr......e
-000034b0: 6172 6c79 5f73 746f 7070 696e 675a 1674  arly_stoppingZ.t
-000034c0: 6f74 616c 5f65 706f 6368 735f 7065 7266  otal_epochs_perf
-000034d0: 6f72 6d65 64da 0565 706f 6368 da0c 7072  ormed..epoch..pr
-000034e0: 6f67 7265 7373 5f62 6172 5a1b 6772 6164  ogress_barZ.grad
-000034f0: 6965 6e74 5f61 6363 756d 756c 6174 696f  ient_accumulatio
-00003500: 6e5f 636f 756e 74da 0562 6174 6368 da09  n_count..batch..
-00003510: 6e65 775f 6261 7463 68da 076f 7574 7075  new_batch..outpu
-00003520: 7473 da04 6c6f 7373 5a0a 7472 6169 6e5f  ts..lossZ.train_
-00003530: 6c6f 7373 5a0a 7661 6c69 645f 6c6f 7373  lossZ.valid_loss
-00003540: 5a09 6570 6f63 685f 6c65 6e5a 0970 7269  Z.epoch_lenZ.pri
-00003550: 6e74 5f6d 7367 7230 0000 0072 3000 0000  nt_msgr0...r0...
-00003560: 7231 0000 00da 1874 7261 696e 5f61 6e64  r1.....train_and
-00003570: 5f65 7661 6c75 6174 655f 6d6f 6465 6ca2  _evaluate_model.
-00003580: 0100 0073 a400 0000 0403 0401 0401 1002  ...s............
-00003590: 0802 0802 1002 1001 1001 1206 0a02 0804  ................
-000035a0: 1001 0c02 0202 0801 06ff 0407 0402 0402  ................
-000035b0: 0402 0c03 0e03 0c03 0802 0402 0e02 0802  ................
-000035c0: 1002 1002 0402 0802 0801 0802 2401 1e02  ............$...
-000035d0: 0e02 1402 0802 0802 0c01 0801 0801 0801  ................
-000035e0: 0a02 1001 1004 0802 0801 0a02 0a02 2401  ..............$.
-000035f0: 1e02 0a02 2601 0e02 1402 0a01 1002 1ef1  ....&...........
-00003600: 0480 0a13 0a01 0a01 0a01 0c02 2002 0c01  ............ ...
-00003610: 02ff 0a02 04fe 0804 0403 0401 0a04 0802  ................
-00003620: 0801 0401 02fe 1204 0081 04f6 7224 0100  ............r$..
-00003630: 0063 0600 0000 0000 0000 0000 0000 1200  .c..............
-00003640: 0000 0900 0000 4300 0000 7398 0100 0074  ......C...s....t
-00003650: 0064 0183 0101 007c 00a0 0174 02a0 037c  .d.....|...t...|
-00003660: 02a1 01a1 0101 0074 0064 0283 0101 0074  .......t.d.....t
-00003670: 0464 0383 017d 0674 02a0 0567 00a1 01a0  .d...}.t...g....
-00003680: 067c 03a1 017d 0774 02a0 0567 00a1 01a0  .|...}.t...g....
-00003690: 067c 03a1 017d 0874 07a0 07a1 007d 0974  .|...}.t.....}.t
-000036a0: 0874 0974 0a7c 0483 0183 0183 017d 0a7c  .t.t.|.......}.|
-000036b0: 0444 005d 877d 0b74 02a0 0ba1 008f 7901  .D.].}.t......y.
-000036c0: 007c 0164 0476 0072 4f7c 0b64 0519 00a0  .|.d.v.rO|.d....
-000036d0: 067c 03a1 017c 0b64 0619 00a0 0ca1 00a0  .|...|.d........
-000036e0: 067c 03a1 0164 079c 027d 0c6e 0f7c 0b64  .|...d...}.n.|.d
-000036f0: 0519 00a0 067c 03a1 017c 0b64 0619 00a0  .....|...|.d....
-00003700: 067c 03a1 0164 079c 027d 0c7c 0164 0876  .|...d...}.|.d.v
-00003710: 0072 747c 0b64 0919 00a0 0d7c 0b64 0919  .rt|.d.....|.d..
-00003720: 006a 0e64 0a19 0064 0ba1 02a0 067c 03a1  .j.d...d.....|..
-00003730: 017c 0c64 0c3c 007c 0064 1069 007c 0ca4  .|.d.<.|.d.i.|..
-00003740: 018e 017d 0d7c 0d7d 0e74 026a 0f7c 0e64  ...}.|.}.t.j.|.d
-00003750: 0d64 0e8d 027d 0f7c 066a 107c 0f7c 0b64  .d...}.|.j.|.|.d
-00003760: 0919 00a0 067c 03a1 0164 0f8d 0201 0074  .....|...d.....t
-00003770: 02a0 117c 077c 0f66 0264 0aa1 027d 0774  ...|.|.f.d...}.t
-00003780: 02a0 117c 087c 0b64 0919 00a0 067c 03a1  ...|.|.d.....|..
-00003790: 0166 0264 0aa1 027d 087c 0aa0 1264 0ba1  .f.d...}.|...d..
-000037a0: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-000037b0: 0831 0073 b477 0101 0001 0001 0059 0001  .1.s.w.......Y..
-000037c0: 0071 3274 07a0 07a1 007d 107c 107c 0918  .q2t.....}.|.|..
-000037d0: 007d 117c 05a0 137c 11a1 0101 007c 077c  .}.|...|.....|.|
-000037e0: 087c 0666 0353 0029 114e 7a16 4c6f 6164  .|.f.S.).Nz.Load
-000037f0: 696e 6720 7468 6520 4265 7374 204d 6f64  ing the Best Mod
-00003800: 656c 7a14 4265 6769 6e6e 696e 6720 4576  elz.Beginning Ev
-00003810: 616c 7561 7469 6f6e da08 6163 6375 7261  aluation..accura
-00003820: 6379 724c 0000 0072 6700 0000 7268 0000  cyrL...rg...rh..
-00003830: 0072 0201 0000 7203 0100 0072 6d00 0000  .r....r....rm...
-00003840: 7201 0000 0072 3900 0000 726e 0000 0072  r....r9...rn...r
-00003850: 3800 0000 2901 da03 6469 6d29 02da 0b70  8...)...dim)...p
-00003860: 7265 6469 6374 696f 6e73 da0a 7265 6665  redictions..refe
-00003870: 7265 6e63 6573 7230 0000 0029 1472 2c00  rencesr0...).r,.
-00003880: 0000 da0f 6c6f 6164 5f73 7461 7465 5f64  ....load_state_d
-00003890: 6963 7472 5800 0000 da04 6c6f 6164 7209  ictrX.....loadr.
-000038a0: 0000 00da 0b46 6c6f 6174 5465 6e73 6f72  .....FloatTensor
-000038b0: 7206 0100 0072 8d00 0000 7212 0000 0072  r....r....r....r
-000038c0: ba00 0000 722a 0000 0072 1101 0000 7209  ....r*...r....r.
-000038d0: 0100 0072 1201 0000 7213 0100 00da 0661  ...r....r......a
-000038e0: 7267 6d61 78da 0961 6464 5f62 6174 6368  rgmax..add_batch
-000038f0: da03 6361 7472 0d01 0000 720e 0100 0029  ..catr....r....)
-00003900: 1272 1901 0000 7252 0000 0072 9900 0000  .r....rR...r....
-00003910: 7216 0100 0072 1801 0000 7217 0100 00da  r....r....r.....
-00003920: 066d 6574 7269 63da 1174 6f74 616c 5f70  .metric..total_p
-00003930: 7265 6469 6374 696f 6e73 da10 746f 7461  redictions..tota
-00003940: 6c5f 7265 6665 7265 6e63 6573 5a0f 696e  l_referencesZ.in
-00003950: 6665 7265 6e63 655f 7374 6172 7472 1f01  ference_startr..
-00003960: 0000 7220 0100 0072 2101 0000 7222 0100  ..r ...r!...r"..
-00003970: 0072 6900 0000 7227 0100 005a 0d69 6e66  .ri...r'...Z.inf
-00003980: 6572 656e 6365 5f65 6e64 5a14 746f 7461  erence_endZ.tota
-00003990: 6c5f 696e 6665 7265 6e63 655f 7469 6d65  l_inference_time
-000039a0: 7230 0000 0072 3000 0000 7231 0000 00da  r0...r0...r1....
-000039b0: 0e65 7661 6c75 6174 655f 6d6f 6465 6c36  .evaluate_model6
-000039c0: 0200 0073 3800 0000 0802 1002 0804 0802  ...s8...........
-000039d0: 1002 1001 0802 1004 0801 0a02 0802 2401  ..............$.
-000039e0: 1e02 0802 2401 0e02 0402 0e01 1801 1002  ....$...........
-000039f0: 1a01 0c02 1ced 0280 0817 0801 0a01 0a02  ................
-00003a00: 7232 0100 0063 0400 0000 0000 0000 0000  r2...c..........
-00003a10: 0000 0800 0000 0800 0000 4300 0000 73e2  ..........C...s.
-00003a20: 0000 0074 0064 0183 0101 0074 0064 0283  ...t.d.....t.d..
-00003a30: 0101 0074 007c 006a 0183 0101 0074 007c  ...t.|.j.....t.|
-00003a40: 016a 0183 0101 007c 036a 027c 017c 0064  .j.....|.j.|.|.d
-00003a50: 038d 027d 0474 0064 0474 037c 0464 0519  ...}.t.d.t.|.d..
-00003a60: 0083 0117 0083 0101 0074 0464 0664 0764  .........t.d.d.d
-00003a70: 088d 027d 057c 056a 0264 097c 017c 0064  ...}.|.j.d.|.|.d
-00003a80: 0a8d 037d 0674 0064 0b74 037c 0664 0619  ...}.t.d.t.|.d..
-00003a90: 0064 0c14 0083 0117 0083 0101 007c 056a  .d...........|.j
-00003aa0: 0264 0d7c 017c 0064 0a8d 037d 0774 0064  .d.|.|.d...}.t.d
-00003ab0: 0e74 037c 0764 0619 0064 0c14 0083 0117  .t.|.d...d......
-00003ac0: 0083 0101 0074 0064 0f74 0374 057c 01a0  .....t.d.t.t.|..
-00003ad0: 06a1 00a0 0764 10a1 0174 087c 01a0 06a1  .....d...t.|....
-00003ae0: 0083 011b 0064 1183 0283 0117 0083 0101  .....d..........
-00003af0: 0074 0064 1274 037c 0283 0117 0083 0101  .t.d.t.|........
-00003b00: 0064 0053 0029 134e 7a1a 2d2d 2d2d 2d2d  .d.S.).Nz.------
-00003b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003b20: 2d2d 2d2d 7a20 5072 6564 6963 7469 6f6e  ----z Prediction
-00003b30: 7320 616e 6420 5265 6665 7265 6e63 6520  s and Reference 
-00003b40: 5368 6170 6573 2902 7228 0100 0072 2701  Shapes).r(...r'.
-00003b50: 0000 7a17 4163 6375 7261 6379 2066 6f72  ..z.Accuracy for
-00003b60: 2054 6573 7420 5365 743a 2072 2501 0000   Test Set: r%...
-00003b70: da02 6631 5472 4600 0000 da05 6d61 6372  ..f1TrF.....macr
-00003b80: 6f29 0372 1501 0000 7228 0100 0072 2701  o).r....r(...r'.
-00003b90: 0000 7a17 4d61 6372 6f20 4631 2066 6f72  ..z.Macro F1 for
-00003ba0: 2054 6573 7420 5365 743a 2072 2200 0000   Test Set: r"...
-00003bb0: da05 6d69 6372 6f7a 174d 6963 726f 2046  ..microz.Micro F
-00003bc0: 3120 666f 7220 5465 7374 2053 6574 3a20  1 for Test Set: 
-00003bd0: 7a25 506f 7369 7469 7665 202f 204e 6567  z%Positive / Neg
-00003be0: 6174 6976 6520 5265 6665 7265 6e63 6520  ative Reference 
-00003bf0: 5261 7469 6f3a 2072 3900 0000 e903 0000  Ratio: r9.......
-00003c00: 007a 2453 6176 6564 2063 6c61 7373 6966  .z$Saved classif
-00003c10: 6963 6174 696f 6e20 6368 6563 6b70 6f69  ication checkpoi
-00003c20: 6e74 2074 6f3a 2029 0972 2c00 0000 7213  nt to: ).r,...r.
-00003c30: 0100 00da 0763 6f6d 7075 7465 722d 0000  .....computer-..
-00003c40: 0072 0900 0000 da05 726f 756e 64da 0674  .r......round..t
-00003c50: 6f6c 6973 74da 0563 6f75 6e74 722a 0000  olist..countr*..
-00003c60: 0029 0872 3001 0000 7231 0100 0072 9900  .).r0...r1...r..
-00003c70: 0000 722f 0100 00da 0772 6573 756c 7473  ..r/.....results
-00003c80: 5a0a 665f 315f 6d65 7472 6963 5a11 6d61  Z.f_1_metricZ.ma
-00003c90: 6372 6f5f 665f 315f 7265 7375 6c74 735a  cro_f_1_resultsZ
-00003ca0: 116d 6963 726f 5f66 5f31 5f72 6573 756c  .micro_f_1_resul
-00003cb0: 7473 7230 0000 0072 3000 0000 7231 0000  tsr0...r0...r1..
-00003cc0: 00da 1470 7269 6e74 5f61 6e64 5f73 6176  ...print_and_sav
-00003cd0: 655f 6d6f 6465 6c6b 0200 0073 1a00 0000  e_modelk...s....
-00003ce0: 0801 0801 0a01 0a01 0e02 1401 0c02 1001  ................
-00003cf0: 1801 1001 1801 2c02 1402 723c 0100 00da  ......,...r<....
-00003d00: 085f 5f6d 6169 6e5f 5f7a 182d 2d63 6c61  .__main__z.--cla
-00003d10: 7373 6966 6963 6174 696f 6e5f 6461 7461  ssification_data
-00003d20: 7365 7454 2902 da04 7479 7065 da08 7265  setT)...type..re
-00003d30: 7175 6972 6564 7a14 2d2d 7465 7374 5f73  quiredz.--test_s
-00003d40: 6574 5f73 656c 6563 7469 6f6e 7a0e 2d2d  et_selectionz.--
-00003d50: 6c61 6265 6c5f 636f 6c75 6d6e 7a0c 2d2d  label_columnz.--
-00003d60: 6e75 6d5f 6570 6f63 6873 7a10 2d2d 7061  num_epochsz.--pa
-00003d70: 7469 656e 6365 5f76 616c 7565 7a0f 2d2d  tience_valuez.--
-00003d80: 6c65 6172 6e69 6e67 5f72 6174 657a 0663  learning_ratez.c
-00003d90: 7564 613a 3072 3900 0000 e920 0000 0072  uda:0r9.... ...r
-00003da0: 2200 0000 72ef 0000 0029 5dda 0874 6f72  "...r....)]..tor
-00003db0: 6368 2e6e 6e72 5d00 0000 da0c 7472 616e  ch.nnr].....tran
-00003dc0: 7366 6f72 6d65 7273 7202 0000 0072 0300  sformersr....r..
-00003dd0: 0000 7204 0000 0072 0500 0000 7206 0000  ..r....r....r...
-00003de0: 0072 0700 0000 7208 0000 00da 0670 616e  .r....r......pan
-00003df0: 6461 7372 b600 0000 da05 6e75 6d70 7972  dasr......numpyr
-00003e00: 1401 0000 da03 6173 7472 e400 0000 7209  ......astr....r.
-00003e10: 0000 0072 0a00 0000 720b 0000 00da 0770  ...r....r......p
-00003e20: 7961 7272 6f77 72e1 0000 00da 0f70 7961  yarrowr......pya
-00003e30: 7272 6f77 2e64 6174 6173 6574 7284 0000  rrow.datasetr...
-00003e40: 00da 0264 735a 0b74 6f72 6368 2e6f 7074  ...dsZ.torch.opt
-00003e50: 696d 720c 0000 00da 1074 6f72 6368 2e75  imr......torch.u
-00003e60: 7469 6c73 2e64 6174 6172 0d00 0000 720e  tils.datar....r.
-00003e70: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
-00003e80: 0000 7258 0000 00da 0974 7164 6d2e 6175  ..rX.....tqdm.au
-00003e90: 746f 7212 0000 00da 0a73 7461 7469 7374  tor......statist
-00003ea0: 6963 7372 8d00 0000 da0a 7375 6270 726f  icsr......subpro
-00003eb0: 6365 7373 723f 0000 0072 7e00 0000 da17  cessr?...r~.....
-00003ec0: 736b 6c65 6172 6e2e 6d6f 6465 6c5f 7365  sklearn.model_se
-00003ed0: 6c65 6374 696f 6e72 1300 0000 da04 6a73  lectionr......js
-00003ee0: 6f6e da06 7261 6e64 6f6d 7224 0000 00da  on..randomr$....
-00003ef0: 0861 7267 7061 7273 6572 1400 0000 da08  .argparser......
-00003f00: 7761 726e 696e 6773 da0e 6669 6c74 6572  warnings..filter
-00003f10: 7761 726e 696e 6773 722d 0000 0072 3200  warningsr-...r2.
-00003f20: 0000 7235 0000 0072 a500 0000 da04 7365  ..r5...r......se
-00003f30: 6564 da0b 6d61 6e75 616c 5f73 6565 64da  ed..manual_seed.
-00003f40: 0765 6e76 6972 6f6e 7244 0000 00da 064d  .environrD.....M
-00003f50: 6f64 756c 6572 4500 0000 727a 0000 0072  odulerE...rz...r
-00003f60: 8500 0000 7287 0000 0072 9a00 0000 72bc  ....r....r....r.
-00003f70: 0000 0072 c800 0000 72de 0000 0072 eb00  ...r....r....r..
-00003f80: 0000 72f8 0000 0072 2401 0000 7232 0100  ..r....r$...r2..
-00003f90: 0072 3c01 0000 7270 0000 00da 0e41 7267  .r<...rp.....Arg
-00003fa0: 756d 656e 7450 6172 7365 72da 0670 6172  umentParser..par
-00003fb0: 7365 72da 0c61 6464 5f61 7267 756d 656e  ser..add_argumen
-00003fc0: 7472 3a00 0000 da05 666c 6f61 74da 0a70  tr:.....float..p
-00003fd0: 6172 7365 5f61 7267 73da 0461 7267 7372  arse_args..argsr
-00003fe0: 8300 0000 7282 0000 005a 1274 6573 745f  ....r....Z.test_
-00003ff0: 7365 745f 7365 6c65 6374 696f 6e72 9200  set_selectionr..
-00004000: 0000 7295 0000 0072 9400 0000 da0d 6c65  ..r....r......le
-00004010: 6172 6e69 6e67 5f72 6174 6572 8e00 0000  arning_rater....
-00004020: 7216 0100 0072 9100 0000 7298 0000 0072  r....r....r....r
-00004030: 9700 0000 7290 0000 0072 9600 0000 7230  ....r....r....r0
-00004040: 0000 0072 3000 0000 7230 0000 0072 3100  ...r0...r0...r1.
-00004050: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00004060: 7392 0000 000c 0214 0118 0108 0308 0108  s...............
-00004070: 0108 010c 0110 0108 020c 010c 020c 0118  ................
-00004080: 0108 020c 0108 0108 0108 0208 010c 0208  ................
-00004090: 0108 0108 0208 0110 0208 020e 0114 0312  ................
-000040a0: 1604 120c 020a 010a 010e 0108 0412 0808  ................
-000040b0: 4c08 0508 1308 0808 2808 2f08 2208 2908  L.......(./.".).
-000040c0: 2008 1000 7f08 1508 350a 1408 0210 0210   .......5.......
-000040d0: 0110 0110 0110 0110 0108 0208 0206 0106  ................
-000040e0: 0106 0106 0108 0104 040a 0104 0204 0104  ................
-000040f0: 0104 0208 0104 e2                        .......
+00001840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001870: 2d2d 2d2d 2d2d 2d2d 2d7a 1c53 7461 7274  ---------z.Start
+00001880: 696e 6720 6e65 7720 6c65 6172 6e69 6e67  ing new learning
+00001890: 2072 6174 653a 2072 0100 0000 7a11 2559   rate: r....z.%Y
+000018a0: 2d25 6d2d 2564 5f25 483a 254d 3a25 5372  -%m-%d_%H:%M:%Sr
+000018b0: 7a00 0000 727b 0000 0072 1f00 0000 7a26  z...r{...r....z&
+000018c0: 4372 6561 7469 6e67 2070 6172 656e 7420  Creating parent 
+000018d0: 6368 6563 6b70 6f69 6e74 2064 6972 6563  checkpoint direc
+000018e0: 746f 7279 3a20 da01 5f72 3800 0000 7a04  tory: .._r8...z.
+000018f0: 2e74 7376 727c 0000 007a 032e 7074 7a09  .tsvr|...z..ptz.
+00001900: 4461 7461 7365 743a 207a 074d 6f64 656c  Dataset: z.Model
+00001910: 3a20 7a14 5465 7374 2053 6574 2053 656c  : z.Test Set Sel
+00001920: 6563 7469 6f6e 3a20 7a10 4e75 6d62 6572  ection: z.Number
+00001930: 206f 6620 5275 6e73 3a20 7a0f 4c65 6172   of Runs: z.Lear
+00001940: 6e69 6e67 2052 6174 653a 20fa 1143 6865  ning Rate: ..Che
+00001950: 636b 706f 696e 7420 5061 7468 3a20 7a0a  ckpoint Path: z.
+00001960: 5061 7469 656e 6365 3a20 7a17 5661 6c69  Patience: z.Vali
+00001970: 6461 7469 6f6e 2053 6574 2043 686f 6963  dation Set Choic
+00001980: 653a 207a 124e 756d 6265 7220 6f66 2045  e: z.Number of E
+00001990: 706f 6368 733a 207a 184e 756d 6265 7220  pochs: z.Number 
+000019a0: 6f66 2077 6172 6d75 7020 7374 6570 733a  of warmup steps:
+000019b0: 2029 0c72 2c00 0000 722d 0000 00da 0864   ).r,...r-.....d
+000019c0: 6174 6574 696d 65da 036e 6f77 da08 7374  atetime..now..st
+000019d0: 7266 7469 6d65 7226 0000 0072 7d00 0000  rftimer&...r}...
+000019e0: 727e 0000 00da 0665 7869 7374 73da 086d  r~.....exists..m
+000019f0: 616b 6564 6972 7372 2900 0000 da04 7469  akedirsr).....ti
+00001a00: 6d65 2913 7283 0000 00da 156c 6561 726e  me).r......learn
+00001a10: 696e 675f 7261 7465 5f63 686f 6963 6573  ing_rate_choices
+00001a20: da14 6368 6f73 656e 5f6c 6561 726e 696e  ..chosen_learnin
+00001a30: 675f 7261 7465 7252 0000 00da 0e6e 756d  g_raterR.....num
+00001a40: 6265 725f 6f66 5f72 756e 73da 1676 616c  ber_of_runs..val
+00001a50: 6964 6174 696f 6e5f 7365 745f 7363 6f72  idation_set_scor
+00001a60: 696e 67da 0c6c 6162 656c 5f63 6f6c 756d  ing..label_colum
+00001a70: 6eda 0e76 616c 6964 6174 696f 6e5f 7365  n..validation_se
+00001a80: 74da 0e70 6174 6965 6e63 655f 7661 6c75  t..patience_valu
+00001a90: 65da 0a6e 756d 5f65 706f 6368 73da 106e  e..num_epochs..n
+00001aa0: 756d 5f77 6172 6d75 705f 7374 6570 73da  um_warmup_steps.
+00001ab0: 2067 7261 6469 656e 745f 6163 6375 6d75   gradient_accumu
+00001ac0: 6c61 7469 6f6e 5f6d 756c 7469 706c 6965  lation_multiplie
+00001ad0: 72da 1361 7373 6967 6e65 645f 6261 7463  r..assigned_batc
+00001ae0: 685f 7369 7a65 7277 0000 0072 8900 0000  h_sizerw...r....
+00001af0: 5a10 6375 7272 656e 745f 6461 7465 7469  Z.current_dateti
+00001b00: 6d65 da0a 7061 7265 6e74 5f64 6972 da0f  me..parent_dir..
+00001b10: 6368 6563 6b70 6f69 6e74 5f70 6174 685a  checkpoint_pathZ
+00001b20: 0f65 7865 6375 7469 6f6e 5f73 7461 7274  .execution_start
+00001b30: 7230 0000 0072 3000 0000 7231 0000 00da  r0...r0...r1....
+00001b40: 1670 7265 7061 7265 5f61 6e64 5f63 6c65  .prepare_and_cle
+00001b50: 616e 5f64 6174 61d0 0000 0073 2e00 0000  an_data....s....
+00001b60: 0806 1001 0801 0802 1002 1002 0c02 0e01  ................
+00001b70: 0a01 4202 0808 0c02 0c01 0c01 1001 1001  ..B.............
+00001b80: 0c01 1001 1001 1001 1001 0801 0802 729c  ..............r.
+00001b90: 0000 0063 0400 0000 0000 0000 0000 0000  ...c............
+00001ba0: 0400 0000 0500 0000 0300 0000 7324 0100  ............s$..
+00001bb0: 0074 006a 017c 0064 0164 028d 0289 0064  .t.j.|.d.d.....d
+00001bc0: 037c 0076 0072 1d88 0064 0419 0088 0064  .|.v.r...d.....d
+00001bd0: 053c 0088 0064 0619 0088 0064 073c 0088  .<...d.....d.<..
+00001be0: 0064 0819 0088 0064 093c 0088 0088 007c  .d.....d.<.....|
+00001bf0: 0119 0064 0a6b 0319 0089 0088 0088 0064  ...d.k.........d
+00001c00: 0519 00a0 02a1 0019 0089 0088 0088 0064  ...............d
+00001c10: 0919 00a0 02a1 0019 0089 0088 0088 0064  ...............d
+00001c20: 0719 00a0 02a1 0019 0089 0088 0088 007c  ...............|
+00001c30: 0119 00a0 02a1 0019 0089 0088 006a 0374  .............j.t
+00001c40: 0488 0083 0164 0b64 0c8d 0289 0064 0d7c  .....d.d.....d.|
+00001c50: 0176 0072 6287 0066 0164 0e64 0f84 0874  .v.rb..f.d.d...t
+00001c60: 0574 0488 0083 0183 0144 0083 0188 0064  .t.......D.....d
+00001c70: 103c 006e 0f87 0066 0164 1164 0f84 0874  .<.n...f.d.d...t
+00001c80: 0574 0488 0083 0183 0144 0083 0188 0064  .t.......D.....d
+00001c90: 103c 0087 0166 0164 1264 0f84 0874 0688  .<...f.d.d...t..
+00001ca0: 0064 1019 0064 1364 148d 0244 0083 0188  .d...d.d...D....
+00001cb0: 0064 153c 0088 00a0 0764 1067 01a1 0189  .d.<.....d.g....
+00001cc0: 0088 0088 0064 1519 0064 166b 0119 0089  .....d...d.k....
+00001cd0: 0088 0053 0029 174e 721d 0000 00a9 01da  ...S.).Nr.......
+00001ce0: 0373 6570 da0e 6e71 5f72 6566 6f72 6d61  .sep..nq_reforma
+00001cf0: 7474 6564 da05 5175 6572 79da 0f73 796e  tted..Query..syn
+00001d00: 7468 6574 6963 5f71 7565 7279 da06 416e  thetic_query..An
+00001d10: 7377 6572 da10 6765 6e65 7261 7465 645f  swer..generated_
+00001d20: 616e 7377 6572 da08 446f 6375 6d65 6e74  answer..Document
+00001d30: 7218 0000 00da 034e 614e 7236 0000 0029  r......NaNr6...)
+00001d40: 02da 016e da0c 7261 6e64 6f6d 5f73 7461  ...n..random_sta
+00001d50: 7465 da07 436f 6e74 6578 7463 0100 0000  te..Contextc....
+00001d60: 0000 0000 0000 0000 0200 0000 0600 0000  ................
+00001d70: 1300 0000 f32a 0000 0067 007c 005d 117d  .....*...g.|.].}
+00001d80: 0174 0088 006a 017c 0119 0064 0019 0088  .t...j.|...d....
+00001d90: 006a 017c 0119 0064 0119 0083 0291 0271  .j.|...d.......q
+00001da0: 0253 0029 0272 a100 0000 7218 0000 00a9  .S.).r....r.....
+00001db0: 0272 3200 0000 da04 696c 6f63 a902 723b  .r2.....iloc..r;
+00001dc0: 0000 0072 3c00 0000 a901 da0d 7379 6e74  ...r<.......synt
+00001dd0: 685f 7175 6572 6965 7372 3000 0000 7231  h_queriesr0...r1
+00001de0: 0000 0072 3e00 0000 1c01 0000 f302 0000  ...r>...........
+00001df0: 002a 007a 2b61 6e61 6c79 7a65 5f61 6e64  .*.z+analyze_and
+00001e00: 5f72 6570 6f72 745f 6461 7461 2e3c 6c6f  _report_data.<lo
+00001e10: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00001e20: da0b 636f 6e63 6174 5f74 6578 7463 0100  ..concat_textc..
+00001e30: 0000 0000 0000 0000 0000 0200 0000 0700  ................
+00001e40: 0000 1300 0000 f336 0000 0067 007c 005d  .......6...g.|.]
+00001e50: 177d 0174 0088 006a 017c 0119 0064 0019  .}.t...j.|...d..
+00001e60: 0088 006a 017c 0119 0064 0119 0088 006a  ...j.|...d.....j
+00001e70: 017c 0119 0064 0219 0083 0391 0271 0253  .|...d.......q.S
+00001e80: 0029 0372 a100 0000 7218 0000 0072 a300  .).r....r....r..
+00001e90: 0000 72aa 0000 0072 ac00 0000 72ad 0000  ..r....r....r...
+00001ea0: 0072 3000 0000 7231 0000 0072 3e00 0000  .r0...r1...r>...
+00001eb0: 1e01 0000 f302 0000 0036 0063 0100 0000  .........6.c....
+00001ec0: 0000 0000 0000 0000 0200 0000 0700 0000  ................
+00001ed0: 1300 0000 7322 0000 0067 007c 005d 0d7d  ....s"...g.|.].}
+00001ee0: 0174 0088 006a 017c 0164 0064 018d 0264  .t...j.|.d.d...d
+00001ef0: 0219 0083 0191 0271 0253 0029 03da 0270  .......q.S.)...p
+00001f00: 7429 01da 0e72 6574 7572 6e5f 7465 6e73  t)...return_tens
+00001f10: 6f72 7372 0100 0000 2902 722a 0000 00da  orsr....).r*....
+00001f20: 0665 6e63 6f64 6529 0272 3b00 0000 7273  .encode).r;...rs
+00001f30: 0000 00a9 0172 7700 0000 7230 0000 0072  .....rw...r0...r
+00001f40: 3100 0000 723e 0000 001f 0100 0073 0200  1...r>.......s..
+00001f50: 0000 2200 5a0a 546f 6b65 6e69 7a69 6e67  ..".Z.Tokenizing
+00001f60: 2901 da04 6465 7363 5a0c 746f 6b65 6e5f  )...descZ.token_
+00001f70: 6c65 6e67 7468 724e 0000 0029 08da 0270  lengthrN...)...p
+00001f80: 64da 0872 6561 645f 6373 76da 056e 6f74  d..read_csv..not
+00001f90: 6e61 da06 7361 6d70 6c65 722a 0000 00da  na..sampler*....
+00001fa0: 0572 616e 6765 7212 0000 00da 0f64 726f  .ranger......dro
+00001fb0: 705f 6475 706c 6963 6174 6573 2904 7283  p_duplicates).r.
+00001fc0: 0000 0072 9300 0000 7277 0000 0072 5600  ...r....rw...rV.
+00001fd0: 0000 7230 0000 0029 0272 ae00 0000 7277  ..r0...).r....rw
+00001fe0: 0000 0072 3100 0000 da17 616e 616c 797a  ...r1.....analyz
+00001ff0: 655f 616e 645f 7265 706f 7274 5f64 6174  e_and_report_dat
+00002000: 61fe 0000 0073 2400 0000 0e02 0802 0c01  a....s$.........
+00002010: 0c01 0c01 1007 1001 1001 1001 1001 1201  ................
+00002020: 080a 2001 1e02 2201 0c01 1007 0402 72be  .. ...".......r.
+00002030: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+00002040: 0500 0000 0600 0000 0300 0000 7360 0100  ............s`..
+00002050: 007c 007d 0374 006a 017c 0164 0164 028d  .|.}.t.j.|.d.d..
+00002060: 0289 0088 0064 0319 0088 0064 043c 0088  .....d.....d.<..
+00002070: 0064 0519 006a 02a0 03a1 0088 0064 053c  .d...j.......d.<
+00002080: 0088 0088 0064 0519 006a 02a0 04a1 0064  .....d...j.....d
+00002090: 066b 0419 0089 0088 0088 007c 0219 00a0  .k.........|....
+000020a0: 05a1 0019 0089 007c 0364 0719 00a0 0674  .......|.d.....t
+000020b0: 02a1 016a 02a0 03a1 007c 0364 073c 007c  ...j.....|.d.<.|
+000020c0: 037c 0364 0719 006a 02a0 04a1 0064 066b  .|.d...j.....d.k
+000020d0: 0419 007d 037c 037c 037c 0219 00a0 05a1  ...}.|.|.|......
+000020e0: 0019 007d 0364 087c 0276 0072 5e87 0066  ...}.d.|.v.r^..f
+000020f0: 0164 0964 0a84 0874 0774 0488 0083 0183  .d.d...t.t......
+00002100: 0144 0083 0188 0064 0b3c 006e 0f87 0066  .D.....d.<.n...f
+00002110: 0164 0c64 0a84 0874 0774 0488 0083 0183  .d.d...t.t......
+00002120: 0144 0083 0188 0064 0b3c 007c 03a0 0864  .D.....d.<.|...d
+00002130: 0b67 01a1 017d 0388 00a0 0864 0b67 01a1  .g...}.....d.g..
+00002140: 0189 0064 0d7c 0276 0072 ac74 0964 0e83  ...d.|.v.r.t.d..
+00002150: 0101 007c 037c 0364 0f19 00a0 05a1 0019  ...|.|.d........
+00002160: 007d 037c 037c 0364 1019 00a0 05a1 0019  .}.|.|.d........
+00002170: 007d 0367 0064 11a2 017d 047c 0364 1219  .}.g.d...}.|.d..
+00002180: 00a0 0674 02a1 017c 0364 123c 007c 037c  ...t...|.d.<.|.|
+00002190: 0364 1219 006a 02a0 0a64 13a0 0b7c 04a1  .d...j...d...|..
+000021a0: 01a1 010f 0019 007d 037c 0388 0066 0253  .......}.|...f.S
+000021b0: 0029 144e 721d 0000 0072 9d00 0000 72a0  .).Nr....r....r.
+000021c0: 0000 00da 0851 7565 7374 696f 6e72 a400  .....Questionr..
+000021d0: 0000 7222 0000 0072 1800 0000 72a8 0000  ..r"...r....r...
+000021e0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+000021f0: 0000 0600 0000 1300 0000 72a9 0000 0029  ..........r....)
+00002200: 0272 bf00 0000 72a4 0000 0072 aa00 0000  .r....r....r....
+00002210: 72ac 0000 00a9 01da 0874 6573 745f 7365  r........test_se
+00002220: 7472 3000 0000 7231 0000 0072 3e00 0000  tr0...r1...r>...
+00002230: 3c01 0000 72af 0000 007a 2274 7261 6e73  <...r....z"trans
+00002240: 666f 726d 5f64 6174 612e 3c6c 6f63 616c  form_data.<local
+00002250: 733e 2e3c 6c69 7374 636f 6d70 3e72 b000  s>.<listcomp>r..
+00002260: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00002270: 0000 0007 0000 0013 0000 0072 b100 0000  ...........r....
+00002280: 2903 72bf 0000 0072 a400 0000 72a2 0000  ).r....r....r...
+00002290: 0072 aa00 0000 72ac 0000 0072 c000 0000  .r....r....r....
+000022a0: 7230 0000 0072 3100 0000 723e 0000 003e  r0...r1...r>...>
+000022b0: 0100 0072 b200 0000 5a05 4661 6974 687a  ...r....Z.Faithz
+000022c0: 3552 6566 696e 696e 6720 6461 7461 2066  5Refining data f
+000022d0: 6f72 2041 6e73 7765 725f 4661 6974 6866  or Answer_Faithf
+000022e0: 756c 6e65 7373 2063 6c61 7373 6966 6963  ulness classific
+000022f0: 6174 696f 6e21 da17 436f 6e74 6578 745f  ation!..Context_
+00002300: 5265 6c65 7661 6e63 655f 4c61 6265 6cda  Relevance_Label.
+00002310: 1941 6e73 7765 725f 4661 6974 6866 756c  .Answer_Faithful
+00002320: 6e65 7373 5f4c 6162 656c 290a 722e 0000  ness_Label).r...
+00002330: 005a 0763 6f6e 7472 6164 da05 6661 6c73  .Z.contrad..fals
+00002340: 65da 0b69 6e66 6f72 6d61 7469 6f6e 5a08  e..informationZ.
+00002350: 756e 616e 7377 6572 72a2 0000 005a 0743  unanswerr....Z.C
+00002360: 6f6e 7472 6164 da05 4661 6c73 655a 0b49  ontrad..FalseZ.I
+00002370: 6e66 6f72 6d61 7469 6f6e 5a08 556e 616e  nformationZ.Unan
+00002380: 7377 6572 72a3 0000 00da 017c 290c 72b8  swerr......|).r.
+00002390: 0000 0072 b900 0000 722d 0000 0072 2700  ...r....r-...r'.
+000023a0: 0000 722a 0000 0072 ba00 0000 da06 6173  ..r*...r......as
+000023b0: 7479 7065 72bc 0000 0072 bd00 0000 722c  typer....r....r,
+000023c0: 0000 00da 0863 6f6e 7461 696e 7372 2800  .....containsr(.
+000023d0: 0000 2905 72ae 0000 0072 9400 0000 7293  ..).r....r....r.
+000023e0: 0000 00da 0874 7261 696e 5f64 665a 0d65  .....train_dfZ.e
+000023f0: 7272 6f72 5f73 7472 696e 6773 7230 0000  rror_stringsr0..
+00002400: 0072 c000 0000 7231 0000 00da 0e74 7261  .r....r1.....tra
+00002410: 6e73 666f 726d 5f64 6174 612d 0100 0073  nsform_data-...s
+00002420: 2c00 0000 0402 0e02 0c01 1201 1601 1001  ,...............
+00002430: 1802 1601 1001 0802 2001 1e02 0c02 0c01  ........ .......
+00002440: 0802 0801 1001 1001 0801 1201 1c01 0802  ................
+00002450: 72cb 0000 0063 0400 0000 0000 0000 0000  r....c..........
+00002460: 0000 0b00 0000 0700 0000 0300 0000 7306  ..............s.
+00002470: 0100 0064 0164 0264 039c 0289 0087 0366  ...d.d.d.......f
+00002480: 0164 0464 0584 0874 0074 0188 0383 0183  .d.d...t.t......
+00002490: 0144 0083 017d 0464 067c 0176 0172 2687  .D...}.d.|.v.r&.
+000024a0: 0087 0187 0366 0364 0764 0584 0874 0074  .....f.d.d...t.t
+000024b0: 0188 0383 0183 0144 0083 017d 056e 0e87  .......D...}.n..
+000024c0: 0187 0366 0264 0864 0584 0874 0074 0188  ...f.d.d...t.t..
+000024d0: 0383 0183 0144 0083 017d 0587 0266 0164  .....D...}...f.d
+000024e0: 0964 0584 0874 0074 0188 0283 0183 0144  .d...t.t.......D
+000024f0: 0083 017d 0687 0187 0266 0264 0a64 0584  ...}.....f.d.d..
+00002500: 0874 0074 0188 0283 0183 0144 0083 017d  .t.t.......D...}
+00002510: 0787 0266 0164 0b64 0584 0874 0074 0188  ...f.d.d...t.t..
+00002520: 0283 0183 0144 0083 017d 0887 0187 0266  .....D...}.....f
+00002530: 0264 0c64 0584 0874 0074 0188 0283 0183  .d.d...t.t......
+00002540: 0144 0083 017d 0974 0264 0d83 0101 0074  .D...}.t.d.....t
+00002550: 0374 0474 057c 057c 0717 007c 0917 0083  .t.t.|.|...|....
+00002560: 0183 0183 017d 0a7c 047c 057c 067c 077c  .....}.|.|.|.|.|
+00002570: 087c 097c 0a66 0753 0029 0e4e 7239 0000  .|.|.f.S.).Nr9..
+00002580: 0072 0100 0000 2902 da03 5965 73da 024e  .r....)...Yes..N
+00002590: 6f63 0100 0000 0000 0000 0000 0000 0200  oc..............
+000025a0: 0000 0400 0000 1300 0000 f31a 0000 0067  ...............g
+000025b0: 007c 005d 097d 0188 006a 007c 0119 0064  .|.].}...j.|...d
+000025c0: 0019 0091 0271 0253 00a9 0172 b000 0000  .....q.S...r....
+000025d0: a901 72ab 0000 0072 ac00 0000 2901 72ca  ..r....r....).r.
+000025e0: 0000 0072 3000 0000 7231 0000 0072 3e00  ...r0...r1...r>.
+000025f0: 0000 5101 0000 f302 0000 001a 007a 2173  ..Q..........z!s
+00002600: 706c 6974 5f64 6174 6173 6574 2e3c 6c6f  plit_dataset.<lo
+00002610: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00002620: 729f 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00002630: 0000 0200 0000 0500 0000 1300 0000 731e  ..............s.
+00002640: 0000 0067 007c 005d 0b7d 0188 0088 026a  ...g.|.].}.....j
+00002650: 007c 0119 0088 0119 0019 0091 0271 0253  .|...........q.S
+00002660: 0072 3000 0000 72d0 0000 0072 ac00 0000  .r0...r....r....
+00002670: 2903 da0f 636f 6e76 6572 7369 6f6e 5f64  )...conversion_d
+00002680: 6963 7472 9300 0000 72ca 0000 0072 3000  ictr....r....r0.
+00002690: 0000 7231 0000 0072 3e00 0000 5301 0000  ..r1...r>...S...
+000026a0: f302 0000 001e 0063 0100 0000 0000 0000  .......c........
+000026b0: 0000 0000 0200 0000 0500 0000 1300 0000  ................
+000026c0: f31e 0000 0067 007c 005d 0b7d 0174 0088  .....g.|.].}.t..
+000026d0: 016a 017c 0119 0088 0019 0083 0191 0271  .j.|...........q
+000026e0: 0253 0072 3000 0000 a902 723a 0000 0072  .S.r0.....r:...r
+000026f0: ab00 0000 72ac 0000 0029 0272 9300 0000  ....r....).r....
+00002700: 72ca 0000 0072 3000 0000 7231 0000 0072  r....r0...r1...r
+00002710: 3e00 0000 5501 0000 72d3 0000 0063 0100  >...U...r....c..
+00002720: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00002730: 0000 1300 0000 72ce 0000 0072 cf00 0000  ......r....r....
+00002740: 72d0 0000 0072 ac00 0000 72c0 0000 0072  r....r....r....r
+00002750: 3000 0000 7231 0000 0072 3e00 0000 5901  0...r1...r>...Y.
+00002760: 0000 72d1 0000 0063 0100 0000 0000 0000  ..r....c........
+00002770: 0000 0000 0200 0000 0500 0000 1300 0000  ................
+00002780: 72d4 0000 0072 3000 0000 72d5 0000 0072  r....r0...r....r
+00002790: ac00 0000 a902 7293 0000 0072 c100 0000  ......r....r....
+000027a0: 7230 0000 0072 3100 0000 723e 0000 005a  r0...r1...r>...Z
+000027b0: 0100 0072 d300 0000 6301 0000 0000 0000  ...r....c.......
+000027c0: 0000 0000 0002 0000 0004 0000 0013 0000  ................
+000027d0: 0072 ce00 0000 72cf 0000 0072 d000 0000  .r....r....r....
+000027e0: 72ac 0000 0072 c000 0000 7230 0000 0072  r....r....r0...r
+000027f0: 3100 0000 723e 0000 005e 0100 0072 d100  1...r>...^...r..
+00002800: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00002810: 0000 0005 0000 0013 0000 0072 d400 0000  ...........r....
+00002820: 7230 0000 0072 d500 0000 72ac 0000 0072  r0...r....r....r
+00002830: d600 0000 7230 0000 0072 3100 0000 723e  ....r0...r1...r>
+00002840: 0000 005f 0100 0072 d300 0000 7a33 2d2d  ..._...r....z3--
+00002850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002880: 2d29 0672 bc00 0000 722a 0000 0072 2c00  -).r....r*...r,.
+00002890: 0000 da06 736f 7274 6564 da04 6c69 7374  ....sorted..list
+000028a0: da03 7365 7429 0b72 ca00 0000 7283 0000  ..set).r....r...
+000028b0: 0072 c100 0000 7293 0000 00da 0e74 7261  .r....r......tra
+000028c0: 696e 5f73 6574 5f74 6578 74da 0f74 7261  in_set_text..tra
+000028d0: 696e 5f73 6574 5f6c 6162 656c da0c 6465  in_set_label..de
+000028e0: 765f 7365 745f 7465 7874 da0d 6465 765f  v_set_text..dev_
+000028f0: 7365 745f 6c61 6265 6cda 0d74 6573 745f  set_label..test_
+00002900: 7365 745f 7465 7874 da0e 7465 7374 5f73  set_text..test_s
+00002910: 6574 5f6c 6162 656c da0b 6c61 6265 6c73  et_label..labels
+00002920: 5f6c 6973 7472 3000 0000 2904 72d2 0000  _listr0...).r...
+00002930: 0072 9300 0000 72c1 0000 0072 ca00 0000  .r....r....r....
+00002940: 7231 0000 00da 0d73 706c 6974 5f64 6174  r1.....split_dat
+00002950: 6173 6574 4f01 0000 7318 0000 000a 011a  asetO...s.......
+00002960: 0108 0120 011c 021a 041c 011a 041c 0108  ... ............
+00002970: 0218 0b12 0872 e100 0000 6305 0000 0000  .....r....c.....
+00002980: 0000 0000 0000 000b 0000 0005 0000 0043  ...............C
+00002990: 0000 0073 fc00 0000 7c00 6401 6b02 723e  ...s....|.d.k.r>
+000029a0: 7400 a001 7c01 7c02 6402 9c02 a101 7d05  t...|.|.d.....}.
+000029b0: 7402 6a03 a004 7c05 a101 7d06 7405 a006  t.j...|...}.t...
+000029c0: 7c06 a101 7d06 7400 a001 7c03 7c04 6402  |...}.t...|.|.d.
+000029d0: 9c02 a101 7d07 7402 6a03 a004 7c07 a101  ....}.t.j...|...
+000029e0: 7d08 7405 a006 7c08 a101 7d08 7400 a001  }.t...|...}.t...
+000029f0: 7c03 7c04 6402 9c02 a101 7d09 7402 6a03  |.|.d.....}.t.j.
+00002a00: a004 7c09 a101 7d0a 7405 a006 7c0a a101  ..|...}.t...|...
+00002a10: 7d0a 6e39 7400 a001 7c01 7c02 6402 9c02  }.n9t...|.|.d...
+00002a20: a101 7d05 7402 6a03 a004 7c05 a101 7d06  ..}.t.j...|...}.
+00002a30: 7405 a006 7c06 a101 7d06 7400 a001 7c03  t...|...}.t...|.
+00002a40: 7c04 6402 9c02 a101 7d07 7402 6a03 a004  |.d.....}.t.j...
+00002a50: 7c07 a101 7d08 7405 a006 7c08 a101 7d08  |...}.t...|...}.
+00002a60: 7400 a001 7407 7408 6402 9c02 a101 7d09  t...t.t.d.....}.
+00002a70: 7402 6a03 a004 7c09 a101 7d0a 7405 a006  t.j...|...}.t...
+00002a80: 7c0a a101 7d0a 7c05 7c06 7c08 7c0a 7c09  |...}.|.|.|.|.|.
+00002a90: 6605 5300 2903 4e54 2902 da05 6c61 6265  f.S.).NT)...labe
+00002aa0: 6c72 7300 0000 2909 72b8 0000 00da 0944  lrs...).r......D
+00002ab0: 6174 6146 7261 6d65 da02 7061 da05 5461  ataFrame..pa..Ta
+00002ac0: 626c 65da 0b66 726f 6d5f 7061 6e64 6173  ble..from_pandas
+00002ad0: da08 6461 7461 7365 7473 da07 4461 7461  ..datasets..Data
+00002ae0: 7365 7472 df00 0000 72de 0000 0029 0b72  setr....r....).r
+00002af0: 9200 0000 72db 0000 0072 da00 0000 72dd  ....r....r....r.
+00002b00: 0000 0072 dc00 0000 da17 7472 6169 6e69  ...r......traini
+00002b10: 6e67 5f64 6174 6173 6574 5f70 616e 6461  ng_dataset_panda
+00002b20: 73da 1674 7261 696e 696e 675f 6461 7461  s..training_data
+00002b30: 7365 745f 6172 726f 775a 1976 616c 6964  set_arrowZ.valid
+00002b40: 6174 696f 6e5f 6461 7461 7365 745f 7061  ation_dataset_pa
+00002b50: 6e64 6173 da18 7661 6c69 6461 7469 6f6e  ndas..validation
+00002b60: 5f64 6174 6173 6574 5f61 7272 6f77 da13  _dataset_arrow..
+00002b70: 7465 7374 5f64 6174 6173 6574 5f70 616e  test_dataset_pan
+00002b80: 6461 73da 1274 6573 745f 6461 7461 7365  das..test_datase
+00002b90: 745f 6172 726f 7772 3000 0000 7230 0000  t_arrowr0...r0..
+00002ba0: 0072 3100 0000 da0f 7072 6570 6172 655f  .r1.....prepare_
+00002bb0: 6461 7461 7365 7478 0100 0073 2800 0000  datasetx...s(...
+00002bc0: 0801 1002 0c01 0a01 1002 0c01 0a01 1002  ................
+00002bd0: 0c01 0c01 1004 0c01 0a01 1002 0c01 0a01  ................
+00002be0: 1002 0c01 0a01 0e02 72ee 0000 0063 0400  ........r....c..
+00002bf0: 0000 0000 0000 0000 0000 0600 0000 0600  ................
+00002c00: 0000 0300 0000 734e 0000 0074 00a0 017c  ......sN...t...|
+00002c10: 017c 027c 0364 019c 03a1 017d 047c 046a  .|.|.d.....}.|.j
+00002c20: 0287 0066 0164 0264 0384 0864 0464 058d  ...f.d.d...d.d..
+00002c30: 027d 057c 05a0 0364 0667 01a1 017d 057c  .}.|...d.g...}.|
+00002c40: 05a0 0464 0764 08a1 027d 057c 05a0 0564  ...d.d...}.|...d
+00002c50: 09a1 0101 007c 0553 0029 0a4e 2903 da05  .....|.S.).N)...
+00002c60: 7472 6169 6eda 0a76 616c 6964 6174 696f  train..validatio
+00002c70: 6eda 0474 6573 7463 0100 0000 0000 0000  n..testc........
+00002c80: 0000 0000 0100 0000 0300 0000 1300 0000  ................
+00002c90: 730a 0000 0074 0088 007c 0083 0253 00a9  s....t...|...S..
+00002ca0: 014e 2901 7279 0000 0029 0172 7800 0000  .N).ry...).rx...
+00002cb0: 72b6 0000 0072 3000 0000 7231 0000 00da  r....r0...r1....
+00002cc0: 083c 6c61 6d62 6461 3e9e 0100 0073 0200  .<lambda>....s..
+00002cd0: 0000 0a00 7a34 696e 6974 616c 697a 655f  ....z4initalize_
+00002ce0: 6461 7461 7365 745f 666f 725f 746f 6b65  dataset_for_toke
+00002cf0: 6e69 7a61 7469 6f6e 2e3c 6c6f 6361 6c73  nization.<locals
+00002d00: 3e2e 3c6c 616d 6264 613e 5429 01da 0762  >.<lambda>T)...b
+00002d10: 6174 6368 6564 7273 0000 0072 e200 0000  atchedrs...r....
+00002d20: 726c 0000 0072 5700 0000 2906 72e7 0000  rl...rW...).r...
+00002d30: 00da 0b44 6174 6173 6574 4469 6374 da03  ...DatasetDict..
+00002d40: 6d61 70da 0e72 656d 6f76 655f 636f 6c75  map..remove_colu
+00002d50: 6d6e 73da 0d72 656e 616d 655f 636f 6c75  mns..rename_colu
+00002d60: 6d6e da0a 7365 745f 666f 726d 6174 2906  mn..set_format).
+00002d70: 7277 0000 0072 ea00 0000 72eb 0000 0072  rw...r....r....r
+00002d80: ed00 0000 7282 0000 00da 1274 6f6b 656e  ....r......token
+00002d90: 697a 6564 5f64 6174 6173 6574 7372 3000  ized_datasetsr0.
+00002da0: 0000 72b6 0000 0072 3100 0000 da22 696e  ..r....r1...."in
+00002db0: 6974 616c 697a 655f 6461 7461 7365 745f  italize_dataset_
+00002dc0: 666f 725f 746f 6b65 6e69 7a61 7469 6f6e  for_tokenization
+00002dd0: 9801 0000 7312 0000 0006 0202 0102 0108  ....s...........
+00002de0: fe16 040c 020c 010a 0104 0272 fb00 0000  ...........r....
+00002df0: 630c 0000 0000 0000 0000 0000 002b 0000  c............+..
+00002e00: 000b 0000 0043 0000 0073 ae03 0000 6700  .....C...s....g.
+00002e10: 7d0c 6700 7d0d 6700 7d0e 7400 6401 7c00  }.g.}.g.}.t.d.|.
+00002e20: 8302 4400 9001 5dc8 7d0f 7401 a001 a100  ..D...].}.t.....
+00002e30: 7d10 7402 6402 8301 0100 7403 7c01 6403  }.t.d.....t.|.d.
+00002e40: 1900 7c02 6404 8d02 7d11 7403 7c01 6405  ..|.d...}.t.|.d.
+00002e50: 1900 7c02 6404 8d02 7d12 7403 7c01 6406  ..|.d...}.t.|.d.
+00002e60: 1900 7c02 6404 8d02 7d13 7404 7405 7406  ..|.d...}.t.t.t.
+00002e70: 7c03 8301 8301 7c04 8302 7d14 7c14 a007  |.....|...}.|...
+00002e80: 7c06 a101 0100 7408 a009 a100 7d15 740a  |.....t.....}.t.
+00002e90: 7c14 a00b a100 7c05 6407 8d02 7d16 7c09  |.....|.d...}.|.
+00002ea0: 7405 7c11 8301 1400 7d17 740c 6408 7c16  t.|.....}.t.d.|.
+00002eb0: 7c0a 7c17 6409 8d04 7d18 6700 7d19 6700  |.|.d...}.g.}.g.
+00002ec0: 7d1a 6700 7d1b 6700 7d1c 6401 640a 6c0d  }.g.}.g.}.d.d.l.
+00002ed0: 6d0e 7d1d 0100 7c1d 7c08 640b 7c07 640c  m.}...|.|.d.|.d.
+00002ee0: 8d03 7d1e 7402 640d 7c07 1700 8301 0100  ..}.t.d.|.......
+00002ef0: 7402 640e 8301 0100 6401 7d1f 7400 7c09  t.d.....d.}.t.|.
+00002f00: 8301 4400 9001 5d4f 7d20 7c1f 640f 3700  ..D...]O} |.d.7.
+00002f10: 7d1f 7402 6410 740f 7c20 8301 1700 8301  }.t.d.t.| ......
+00002f20: 0100 7410 7400 7405 7c11 8301 8301 8301  ..t.t.t.|.......
+00002f30: 7d21 6401 7d22 7c14 a011 a100 0100 7c11  }!d.}"|.......|.
+00002f40: 4400 5d5e 7d23 7c04 6411 7600 72b2 7c23  D.]^}#|.d.v.r.|#
+00002f50: 6412 1900 a007 7c06 a101 7c23 6413 1900  d.....|...|#d...
+00002f60: a012 a100 a007 7c06 a101 6414 9c02 7d24  ......|...d...}$
+00002f70: 6e0f 7c23 6412 1900 a007 7c06 a101 7c23  n.|#d.....|...|#
+00002f80: 6413 1900 a007 7c06 a101 6414 9c02 7d24  d.....|...d...}$
+00002f90: 7c14 6421 6900 7c24 a401 8e01 7d25 7c15  |.d!i.|$....}%|.
+00002fa0: 7c25 7c23 6415 1900 a007 7c06 a101 8302  |%|#d.....|.....
+00002fb0: 7d26 7c26 a013 a100 0100 7c22 640f 3700  }&|&......|"d.7.
+00002fc0: 7d22 7c22 7c0b 1600 6401 6b02 72ec 7c16  }"|"|...d.k.r.|.
+00002fd0: a014 a100 0100 7c18 a014 a100 0100 7c16  ......|.......|.
+00002fe0: a015 a100 0100 7c21 a016 640f a101 0100  ......|!..d.....
+00002ff0: 7c19 a017 7c26 a018 a100 a101 0100 719a  |...|&........q.
+00003000: 7410 7400 7405 7c12 8301 8301 8301 7d21  t.t.t.|.......}!
+00003010: 7c14 a019 a100 0100 7c12 4400 5d73 7d23  |.......|.D.]s}#
+00003020: 741a a01b a100 8f63 0100 7c04 6411 7600  t......c..|.d.v.
+00003030: 9001 7225 7c23 6412 1900 a007 7c06 a101  ..r%|#d.....|...
+00003040: 7c23 6413 1900 a012 a100 a007 7c06 a101  |#d.........|...
+00003050: 6414 9c02 7d24 6e0f 7c23 6412 1900 a007  d...}$n.|#d.....
+00003060: 7c06 a101 7c23 6413 1900 a007 7c06 a101  |...|#d.....|...
+00003070: 6414 9c02 7d24 7c04 6416 7600 9001 724c  d...}$|.d.v...rL
+00003080: 7c23 6415 1900 a01c 7c23 6415 1900 6a1d  |#d.....|#d...j.
+00003090: 6401 1900 640f a102 a007 7c06 a101 6601  d...d.....|...f.
+000030a0: 7c24 6417 3c00 7c14 6421 6900 7c24 a401  |$d.<.|.d!i.|$..
+000030b0: 8e01 7d25 7c15 7c25 7c23 6415 1900 a007  ..}%|.|%|#d.....
+000030c0: 7c06 a101 8302 7d26 7c21 a016 640f a101  |.....}&|!..d...
+000030d0: 0100 7c1a a017 7c26 a018 a100 a101 0100  ..|...|&........
+000030e0: 5700 6400 0400 0400 8303 0100 6e09 3100  W.d.........n.1.
+000030f0: 9001 7374 7701 0100 0100 0100 5900 0100  ..stw.......Y...
+00003100: 9001 7107 741e a01f 7c19 a101 7d27 741e  ..q.t...|...}'t.
+00003110: a01f 7c1a a101 7d28 7c1b a017 7c27 a101  ..|...}(|...|'..
+00003120: 0100 7c1c a017 7c28 a101 0100 7405 740f  ..|...|(....t.t.
+00003130: 7c09 8301 8301 7d29 6418 7c20 6419 7c29  |.....})d.| d.|)
+00003140: 9b00 9d02 9b04 641a 7c09 6419 7c29 9b00  ......d.|.d.|)..
+00003150: 9d02 9b04 641b 9d05 641c 7c27 641d 9b04  ....d...d.|'d...
+00003160: 641e 9d03 1700 641f 7c28 641d 9b04 9d02  d.....d.|(d.....
+00003170: 1700 7d2a 7402 7c2a 8301 0100 6700 7d19  ..}*t.|*....g.}.
+00003180: 6700 7d1a 7c1e 7c28 7c14 8302 0100 7c1e  g.}.|.|(|.....|.
+00003190: 6a20 9001 72cb 7402 6420 8301 0100 0100  j ..r.t.d ......
+000031a0: 9001 71cc 717b 7c14 7c1b 7c1c 7c13 7c0e  ..q.q{|.|.|.|.|.
+000031b0: 6605 0200 0100 5300 6400 5300 2922 4e72  f.....S.d.S.)"Nr
+000031c0: 0100 0000 7a0d 4c6f 6164 696e 6720 4d6f  ....z.Loading Mo
+000031d0: 6465 6c72 ef00 0000 2901 da0a 6261 7463  delr....)...batc
+000031e0: 685f 7369 7a65 72f0 0000 0072 f100 0000  h_sizer....r....
+000031f0: 2901 da02 6c72 da06 6c69 6e65 6172 2904  )...lr..linear).
+00003200: da04 6e61 6d65 da09 6f70 7469 6d69 7a65  ..name..optimize
+00003210: 7272 9700 0000 da12 6e75 6d5f 7472 6169  rr......num_trai
+00003220: 6e69 6e67 5f73 7465 7073 2901 da0d 4561  ning_steps)...Ea
+00003230: 726c 7953 746f 7070 696e 6754 2903 da08  rlyStoppingT)...
+00003240: 7061 7469 656e 6365 da07 7665 7262 6f73  patience..verbos
+00003250: 6572 7e00 0000 7288 0000 007a 1242 6567  er~...r....z.Beg
+00003260: 696e 6e69 6e67 2054 7261 696e 696e 6772  inning Trainingr
+00003270: 3900 0000 7a0f 4375 7272 656e 7420 4570  9...z.Current Ep
+00003280: 6f63 683a 2072 4c00 0000 7266 0000 0072  och: rL...rf...r
+00003290: 6700 0000 a902 726a 0000 0072 6b00 0000  g.....rj...rk...
+000032a0: 726c 0000 00a9 0372 6500 0000 7250 0000  rl.....re...rP..
+000032b0: 0072 4f00 0000 726d 0000 00da 015b da01  .rO...rm.....[..
+000032c0: 3e72 7b00 0000 7a02 5d20 7a0c 7472 6169  >r{...z.] z.trai
+000032d0: 6e5f 6c6f 7373 3a20 7a03 2e35 6672 1c00  n_loss: z..5fr..
+000032e0: 0000 7a0c 7661 6c69 645f 6c6f 7373 3a20  ..z.valid_loss: 
+000032f0: 7a0e 4561 726c 7920 7374 6f70 7069 6e67  z.Early stopping
+00003300: 7230 0000 0029 2172 bc00 0000 728e 0000  r0...)!r....r...
+00003310: 0072 2c00 0000 720d 0000 0072 4500 0000  .r,...r....rE...
+00003320: 722a 0000 0072 d900 0000 da02 746f 725c  r*...r......tor\
+00003330: 0000 00da 1043 726f 7373 456e 7472 6f70  .....CrossEntrop
+00003340: 794c 6f73 7372 0c00 0000 da0a 7061 7261  yLossr......para
+00003350: 6d65 7465 7273 720e 0000 005a 2b61 7265  metersr....Z+are
+00003360: 732e 4c4c 4d5f 6173 5f61 5f4a 7564 6765  s.LLM_as_a_Judge
+00003370: 5f41 6461 7074 6174 696f 6e2e 7079 746f  _Adaptation.pyto
+00003380: 7263 6874 6f6f 6c73 7202 0100 0072 2d00  rchtoolsr....r-.
+00003390: 0000 7212 0000 0072 ef00 0000 da04 626f  ..r....r......bo
+000033a0: 6f6c da08 6261 636b 7761 7264 da04 7374  ol..backward..st
+000033b0: 6570 da09 7a65 726f 5f67 7261 64da 0675  ep..zero_grad..u
+000033c0: 7064 6174 65da 0661 7070 656e 64da 0469  pdate..append..i
+000033d0: 7465 6dda 0465 7661 6c72 5700 0000 da07  tem..evalrW.....
+000033e0: 6e6f 5f67 7261 64da 0772 6573 6861 7065  no_grad..reshape
+000033f0: da05 7368 6170 65da 026e 70da 0761 7665  ..shape..np..ave
+00003400: 7261 6765 5a0a 6561 726c 795f 7374 6f70  rageZ.early_stop
+00003410: 292b 7291 0000 0072 fa00 0000 7299 0000  )+r....r....r...
+00003420: 0072 db00 0000 7252 0000 0072 9000 0000  .r....rR...r....
+00003430: da06 6465 7669 6365 729b 0000 0072 9500  ..devicer....r..
+00003440: 0000 7296 0000 0072 9700 0000 7298 0000  ..r....r....r...
+00003450: 005a 0e6d 6963 726f 5f61 7665 7261 6765  .Z.micro_average
+00003460: 735a 0e6d 6163 726f 5f61 7665 7261 6765  sZ.macro_average
+00003470: 73da 0f69 6e66 6572 656e 6365 5f74 696d  s..inference_tim
+00003480: 6573 723c 0000 005a 0972 756e 5f73 7461  esr<...Z.run_sta
+00003490: 7274 5a10 7472 6169 6e5f 6461 7461 6c6f  rtZ.train_datalo
+000034a0: 6164 6572 5a15 7661 6c69 6461 7469 6f6e  aderZ.validation
+000034b0: 5f64 6174 616c 6f61 6465 72da 0f65 7661  _dataloader..eva
+000034c0: 6c5f 6461 7461 6c6f 6164 6572 da05 6d6f  l_dataloader..mo
+000034d0: 6465 6c5a 0963 7269 7465 7269 6f6e 7200  delZ.criterionr.
+000034e0: 0100 0072 0101 0000 da0c 6c72 5f73 6368  ...r......lr_sch
+000034f0: 6564 756c 6572 5a0c 7472 6169 6e5f 6c6f  edulerZ.train_lo
+00003500: 7373 6573 5a0c 7661 6c69 645f 6c6f 7373  ssesZ.valid_loss
+00003510: 6573 da10 6176 675f 7472 6169 6e5f 6c6f  es..avg_train_lo
+00003520: 7373 6573 da10 6176 675f 7661 6c69 645f  sses..avg_valid_
+00003530: 6c6f 7373 6573 7202 0100 00da 0e65 6172  lossesr......ear
+00003540: 6c79 5f73 746f 7070 696e 675a 1674 6f74  ly_stoppingZ.tot
+00003550: 616c 5f65 706f 6368 735f 7065 7266 6f72  al_epochs_perfor
+00003560: 6d65 64da 0565 706f 6368 da0c 7072 6f67  med..epoch..prog
+00003570: 7265 7373 5f62 6172 5a1b 6772 6164 6965  ress_barZ.gradie
+00003580: 6e74 5f61 6363 756d 756c 6174 696f 6e5f  nt_accumulation_
+00003590: 636f 756e 74da 0562 6174 6368 da09 6e65  count..batch..ne
+000035a0: 775f 6261 7463 68da 076f 7574 7075 7473  w_batch..outputs
+000035b0: da04 6c6f 7373 5a0a 7472 6169 6e5f 6c6f  ..lossZ.train_lo
+000035c0: 7373 5a0a 7661 6c69 645f 6c6f 7373 5a09  ssZ.valid_lossZ.
+000035d0: 6570 6f63 685f 6c65 6e5a 0970 7269 6e74  epoch_lenZ.print
+000035e0: 5f6d 7367 7230 0000 0072 3000 0000 7231  _msgr0...r0...r1
+000035f0: 0000 00da 1874 7261 696e 5f61 6e64 5f65  .....train_and_e
+00003600: 7661 6c75 6174 655f 6d6f 6465 6ca8 0100  valuate_model...
+00003610: 0073 a400 0000 0403 0401 0401 1002 0802  .s..............
+00003620: 0802 1002 1001 1001 1206 0a02 0804 1001  ................
+00003630: 0c02 0202 0801 06ff 0407 0402 0402 0402  ................
+00003640: 0c03 0e03 0c03 0802 0402 0e02 0802 1002  ................
+00003650: 1002 0402 0802 0801 0802 2401 1e02 0e02  ..........$.....
+00003660: 1402 0802 0802 0c01 0801 0801 0801 0a02  ................
+00003670: 1001 1004 0802 0801 0a02 0a02 2401 1e02  ............$...
+00003680: 0a02 2601 0e02 1402 0a01 1002 1ef1 0480  ..&.............
+00003690: 0a13 0a01 0a01 0a01 0c02 2002 0c01 02ff  .......... .....
+000036a0: 0a02 04fe 0804 0403 0401 0a04 0802 0801  ................
+000036b0: 0601 02fe 1204 0081 04f6 7227 0100 0063  ..........r'...c
+000036c0: 0600 0000 0000 0000 0000 0000 1200 0000  ................
+000036d0: 0900 0000 4300 0000 7398 0100 0074 0064  ....C...s....t.d
+000036e0: 0183 0101 007c 00a0 0174 02a0 037c 02a1  .....|...t...|..
+000036f0: 01a1 0101 0074 0064 0283 0101 0074 0464  .....t.d.....t.d
+00003700: 0383 017d 0674 02a0 0567 00a1 01a0 067c  ...}.t...g.....|
+00003710: 03a1 017d 0774 02a0 0567 00a1 01a0 067c  ...}.t...g.....|
+00003720: 03a1 017d 0874 07a0 07a1 007d 0974 0874  ...}.t.....}.t.t
+00003730: 0974 0a7c 0483 0183 0183 017d 0a7c 0444  .t.|.......}.|.D
+00003740: 005d 877d 0b74 02a0 0ba1 008f 7901 007c  .].}.t......y..|
+00003750: 0164 0476 0072 4f7c 0b64 0519 00a0 067c  .d.v.rO|.d.....|
+00003760: 03a1 017c 0b64 0619 00a0 0ca1 00a0 067c  ...|.d.........|
+00003770: 03a1 0164 079c 027d 0c6e 0f7c 0b64 0519  ...d...}.n.|.d..
+00003780: 00a0 067c 03a1 017c 0b64 0619 00a0 067c  ...|...|.d.....|
+00003790: 03a1 0164 079c 027d 0c7c 0164 0876 0072  ...d...}.|.d.v.r
+000037a0: 747c 0b64 0919 00a0 0d7c 0b64 0919 006a  t|.d.....|.d...j
+000037b0: 0e64 0a19 0064 0ba1 02a0 067c 03a1 017c  .d...d.....|...|
+000037c0: 0c64 0c3c 007c 0064 1069 007c 0ca4 018e  .d.<.|.d.i.|....
+000037d0: 017d 0d7c 0d7d 0e74 026a 0f7c 0e64 0d64  .}.|.}.t.j.|.d.d
+000037e0: 0e8d 027d 0f7c 066a 107c 0f7c 0b64 0919  ...}.|.j.|.|.d..
+000037f0: 00a0 067c 03a1 0164 0f8d 0201 0074 02a0  ...|...d.....t..
+00003800: 117c 077c 0f66 0264 0aa1 027d 0774 02a0  .|.|.f.d...}.t..
+00003810: 117c 087c 0b64 0919 00a0 067c 03a1 0166  .|.|.d.....|...f
+00003820: 0264 0aa1 027d 087c 0aa0 1264 0ba1 0101  .d...}.|...d....
+00003830: 0057 0064 0004 0004 0083 0301 006e 0831  .W.d.........n.1
+00003840: 0073 b477 0101 0001 0001 0059 0001 0071  .s.w.......Y...q
+00003850: 3274 07a0 07a1 007d 107c 107c 0918 007d  2t.....}.|.|...}
+00003860: 117c 05a0 137c 11a1 0101 007c 077c 087c  .|...|.....|.|.|
+00003870: 0666 0353 0029 114e 7a16 4c6f 6164 696e  .f.S.).Nz.Loadin
+00003880: 6720 7468 6520 4265 7374 204d 6f64 656c  g the Best Model
+00003890: 7a14 4265 6769 6e6e 696e 6720 4576 616c  z.Beginning Eval
+000038a0: 7561 7469 6f6e da08 6163 6375 7261 6379  uation..accuracy
+000038b0: 724c 0000 0072 6600 0000 7267 0000 0072  rL...rf...rg...r
+000038c0: 0501 0000 7206 0100 0072 6c00 0000 7201  ....r....rl...r.
+000038d0: 0000 0072 3900 0000 726d 0000 0072 3800  ...r9...rm...r8.
+000038e0: 0000 2901 da03 6469 6d29 02da 0b70 7265  ..)...dim)...pre
+000038f0: 6469 6374 696f 6e73 da0a 7265 6665 7265  dictions..refere
+00003900: 6e63 6573 7230 0000 0029 1472 2c00 0000  ncesr0...).r,...
+00003910: da0f 6c6f 6164 5f73 7461 7465 5f64 6963  ..load_state_dic
+00003920: 7472 5700 0000 da04 6c6f 6164 7209 0000  trW.....loadr...
+00003930: 00da 0b46 6c6f 6174 5465 6e73 6f72 7209  ...FloatTensorr.
+00003940: 0100 0072 8e00 0000 7212 0000 0072 bc00  ...r....r....r..
+00003950: 0000 722a 0000 0072 1401 0000 720c 0100  ..r*...r....r...
+00003960: 0072 1501 0000 7216 0100 00da 0661 7267  .r....r......arg
+00003970: 6d61 78da 0961 6464 5f62 6174 6368 da03  max..add_batch..
+00003980: 6361 7472 1001 0000 7211 0100 0029 1272  catr....r....).r
+00003990: 1c01 0000 7252 0000 0072 9b00 0000 7219  ....rR...r....r.
+000039a0: 0100 0072 1b01 0000 721a 0100 00da 066d  ...r....r......m
+000039b0: 6574 7269 63da 1174 6f74 616c 5f70 7265  etric..total_pre
+000039c0: 6469 6374 696f 6e73 da10 746f 7461 6c5f  dictions..total_
+000039d0: 7265 6665 7265 6e63 6573 5a0f 696e 6665  referencesZ.infe
+000039e0: 7265 6e63 655f 7374 6172 7472 2201 0000  rence_startr"...
+000039f0: 7223 0100 0072 2401 0000 7225 0100 0072  r#...r$...r%...r
+00003a00: 6800 0000 722a 0100 005a 0d69 6e66 6572  h...r*...Z.infer
+00003a10: 656e 6365 5f65 6e64 5a14 746f 7461 6c5f  ence_endZ.total_
+00003a20: 696e 6665 7265 6e63 655f 7469 6d65 7230  inference_timer0
+00003a30: 0000 0072 3000 0000 7231 0000 00da 0e65  ...r0...r1.....e
+00003a40: 7661 6c75 6174 655f 6d6f 6465 6c3c 0200  valuate_model<..
+00003a50: 0073 3800 0000 0802 1002 0804 0802 1002  .s8.............
+00003a60: 1001 0802 1004 0801 0a02 0802 2401 1e02  ............$...
+00003a70: 0802 2401 0e02 0402 0e01 1801 1002 1a01  ..$.............
+00003a80: 0c02 1ced 0280 0817 0801 0a01 0a02 7235  ..............r5
+00003a90: 0100 0063 0400 0000 0000 0000 0000 0000  ...c............
+00003aa0: 0800 0000 0800 0000 4300 0000 73e2 0000  ........C...s...
+00003ab0: 0074 0064 0183 0101 0074 0064 0283 0101  .t.d.....t.d....
+00003ac0: 0074 007c 006a 0183 0101 0074 007c 016a  .t.|.j.....t.|.j
+00003ad0: 0183 0101 007c 036a 027c 017c 0064 038d  .....|.j.|.|.d..
+00003ae0: 027d 0474 0064 0474 037c 0464 0519 0083  .}.t.d.t.|.d....
+00003af0: 0117 0083 0101 0074 0464 0664 0764 088d  .......t.d.d.d..
+00003b00: 027d 057c 056a 0264 097c 017c 0064 0a8d  .}.|.j.d.|.|.d..
+00003b10: 037d 0674 0064 0b74 037c 0664 0619 0064  .}.t.d.t.|.d...d
+00003b20: 0c14 0083 0117 0083 0101 007c 056a 0264  ...........|.j.d
+00003b30: 0d7c 017c 0064 0a8d 037d 0774 0064 0e74  .|.|.d...}.t.d.t
+00003b40: 037c 0764 0619 0064 0c14 0083 0117 0083  .|.d...d........
+00003b50: 0101 0074 0064 0f74 0374 057c 01a0 06a1  ...t.d.t.t.|....
+00003b60: 00a0 0764 10a1 0174 087c 01a0 06a1 0083  ...d...t.|......
+00003b70: 011b 0064 1183 0283 0117 0083 0101 0074  ...d...........t
+00003b80: 0064 1274 037c 0283 0117 0083 0101 0064  .d.t.|.........d
+00003b90: 0053 0029 134e 7a1a 2d2d 2d2d 2d2d 2d2d  .S.).Nz.--------
+00003ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003bb0: 2d2d 7a20 5072 6564 6963 7469 6f6e 7320  --z Predictions 
+00003bc0: 616e 6420 5265 6665 7265 6e63 6520 5368  and Reference Sh
+00003bd0: 6170 6573 2902 722b 0100 0072 2a01 0000  apes).r+...r*...
+00003be0: 7a17 4163 6375 7261 6379 2066 6f72 2054  z.Accuracy for T
+00003bf0: 6573 7420 5365 743a 2072 2801 0000 da02  est Set: r(.....
+00003c00: 6631 5472 4600 0000 da05 6d61 6372 6f29  f1TrF.....macro)
+00003c10: 0372 1801 0000 722b 0100 0072 2a01 0000  .r....r+...r*...
+00003c20: 7a17 4d61 6372 6f20 4631 2066 6f72 2054  z.Macro F1 for T
+00003c30: 6573 7420 5365 743a 2072 2200 0000 da05  est Set: r".....
+00003c40: 6d69 6372 6f7a 174d 6963 726f 2046 3120  microz.Micro F1 
+00003c50: 666f 7220 5465 7374 2053 6574 3a20 7a25  for Test Set: z%
+00003c60: 506f 7369 7469 7665 202f 204e 6567 6174  Positive / Negat
+00003c70: 6976 6520 5265 6665 7265 6e63 6520 5261  ive Reference Ra
+00003c80: 7469 6f3a 2072 3900 0000 e903 0000 007a  tio: r9........z
+00003c90: 2453 6176 6564 2063 6c61 7373 6966 6963  $Saved classific
+00003ca0: 6174 696f 6e20 6368 6563 6b70 6f69 6e74  ation checkpoint
+00003cb0: 2074 6f3a 2029 0972 2c00 0000 7216 0100   to: ).r,...r...
+00003cc0: 00da 0763 6f6d 7075 7465 722d 0000 0072  ...computer-...r
+00003cd0: 0900 0000 da05 726f 756e 64da 0674 6f6c  ......round..tol
+00003ce0: 6973 74da 0563 6f75 6e74 722a 0000 0029  ist..countr*...)
+00003cf0: 0872 3301 0000 7234 0100 0072 9b00 0000  .r3...r4...r....
+00003d00: 7232 0100 00da 0772 6573 756c 7473 5a0a  r2.....resultsZ.
+00003d10: 665f 315f 6d65 7472 6963 5a11 6d61 6372  f_1_metricZ.macr
+00003d20: 6f5f 665f 315f 7265 7375 6c74 735a 116d  o_f_1_resultsZ.m
+00003d30: 6963 726f 5f66 5f31 5f72 6573 756c 7473  icro_f_1_results
+00003d40: 7230 0000 0072 3000 0000 7231 0000 00da  r0...r0...r1....
+00003d50: 1470 7269 6e74 5f61 6e64 5f73 6176 655f  .print_and_save_
+00003d60: 6d6f 6465 6c71 0200 0073 1a00 0000 0801  modelq...s......
+00003d70: 0801 0a01 0a01 0e02 1401 0c02 1001 1801  ................
+00003d80: 1001 1801 2c02 1402 723f 0100 00da 085f  ....,...r?....._
+00003d90: 5f6d 6169 6e5f 5f7a 182d 2d63 6c61 7373  _main__z.--class
+00003da0: 6966 6963 6174 696f 6e5f 6461 7461 7365  ification_datase
+00003db0: 7454 2902 da04 7479 7065 da08 7265 7175  tT)...type..requ
+00003dc0: 6972 6564 7a14 2d2d 7465 7374 5f73 6574  iredz.--test_set
+00003dd0: 5f73 656c 6563 7469 6f6e 7a0e 2d2d 6c61  _selectionz.--la
+00003de0: 6265 6c5f 636f 6c75 6d6e 7a0c 2d2d 6e75  bel_columnz.--nu
+00003df0: 6d5f 6570 6f63 6873 7a10 2d2d 7061 7469  m_epochsz.--pati
+00003e00: 656e 6365 5f76 616c 7565 7a0f 2d2d 6c65  ence_valuez.--le
+00003e10: 6172 6e69 6e67 5f72 6174 657a 0663 7564  arning_ratez.cud
+00003e20: 613a 3072 3900 0000 e920 0000 0072 2200  a:0r9.... ...r".
+00003e30: 0000 72f2 0000 0029 5dda 0874 6f72 6368  ..r....)]..torch
+00003e40: 2e6e 6e72 5c00 0000 da0c 7472 616e 7366  .nnr\.....transf
+00003e50: 6f72 6d65 7273 7202 0000 0072 0300 0000  ormersr....r....
+00003e60: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
+00003e70: 0700 0000 7208 0000 00da 0670 616e 6461  ....r......panda
+00003e80: 7372 b800 0000 da05 6e75 6d70 7972 1701  sr......numpyr..
+00003e90: 0000 da03 6173 7472 e700 0000 7209 0000  ....astr....r...
+00003ea0: 0072 0a00 0000 720b 0000 00da 0770 7961  .r....r......pya
+00003eb0: 7272 6f77 72e4 0000 00da 0f70 7961 7272  rrowr......pyarr
+00003ec0: 6f77 2e64 6174 6173 6574 7283 0000 00da  ow.datasetr.....
+00003ed0: 0264 735a 0b74 6f72 6368 2e6f 7074 696d  .dsZ.torch.optim
+00003ee0: 720c 0000 00da 1074 6f72 6368 2e75 7469  r......torch.uti
+00003ef0: 6c73 2e64 6174 6172 0d00 0000 720e 0000  ls.datar....r...
+00003f00: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
+00003f10: 7257 0000 00da 0974 7164 6d2e 6175 746f  rW.....tqdm.auto
+00003f20: 7212 0000 00da 0a73 7461 7469 7374 6963  r......statistic
+00003f30: 7372 8e00 0000 da0a 7375 6270 726f 6365  sr......subproce
+00003f40: 7373 723f 0000 0072 7d00 0000 da17 736b  ssr?...r}.....sk
+00003f50: 6c65 6172 6e2e 6d6f 6465 6c5f 7365 6c65  learn.model_sele
+00003f60: 6374 696f 6e72 1300 0000 da04 6a73 6f6e  ctionr......json
+00003f70: da06 7261 6e64 6f6d 7224 0000 00da 0861  ..randomr$.....a
+00003f80: 7267 7061 7273 6572 1400 0000 da08 7761  rgparser......wa
+00003f90: 726e 696e 6773 da0e 6669 6c74 6572 7761  rnings..filterwa
+00003fa0: 726e 696e 6773 722d 0000 0072 3200 0000  rningsr-...r2...
+00003fb0: 7235 0000 0072 a700 0000 da04 7365 6564  r5...r......seed
+00003fc0: da0b 6d61 6e75 616c 5f73 6565 64da 0765  ..manual_seed..e
+00003fd0: 6e76 6972 6f6e 7244 0000 00da 064d 6f64  nvironrD.....Mod
+00003fe0: 756c 6572 4500 0000 7279 0000 0072 8400  ulerE...ry...r..
+00003ff0: 0000 7286 0000 0072 9c00 0000 72be 0000  ..r....r....r...
+00004000: 0072 cb00 0000 72e1 0000 0072 ee00 0000  .r....r....r....
+00004010: 72fb 0000 0072 2701 0000 7235 0100 0072  r....r'...r5...r
+00004020: 3f01 0000 726f 0000 00da 0e41 7267 756d  ?...ro.....Argum
+00004030: 656e 7450 6172 7365 72da 0670 6172 7365  entParser..parse
+00004040: 72da 0c61 6464 5f61 7267 756d 656e 7472  r..add_argumentr
+00004050: 3a00 0000 da05 666c 6f61 74da 0a70 6172  :.....float..par
+00004060: 7365 5f61 7267 73da 0461 7267 7372 8200  se_args..argsr..
+00004070: 0000 7281 0000 005a 1274 6573 745f 7365  ..r....Z.test_se
+00004080: 745f 7365 6c65 6374 696f 6e72 9300 0000  t_selectionr....
+00004090: 7296 0000 0072 9500 0000 da0d 6c65 6172  r....r......lear
+000040a0: 6e69 6e67 5f72 6174 6572 8f00 0000 7219  ning_rater....r.
+000040b0: 0100 0072 9200 0000 7299 0000 0072 9800  ...r....r....r..
+000040c0: 0000 7291 0000 0072 9700 0000 7230 0000  ..r....r....r0..
+000040d0: 0072 3000 0000 7230 0000 0072 3100 0000  .r0...r0...r1...
+000040e0: da08 3c6d 6f64 756c 653e 0100 0000 7392  ..<module>....s.
+000040f0: 0000 000c 0214 0118 0108 0308 0108 0108  ................
+00004100: 010c 0110 0108 020c 010c 020c 0118 0108  ................
+00004110: 020c 0108 0108 0108 0208 010c 0208 0108  ................
+00004120: 0108 0208 0110 0208 020e 0114 0312 1604  ................
+00004130: 120c 020a 010a 010e 0108 0412 0808 4c08  ..............L.
+00004140: 0508 1308 0808 2e08 2f08 2208 2908 2008  ......../.".). .
+00004150: 1000 7f08 1508 350a 1408 0210 0210 0110  ......5.........
+00004160: 0110 0110 0110 0108 0208 0206 0106 0106  ................
+00004170: 0106 0108 0104 040a 0104 0204 0104 0104  ................
+00004180: 0208 0104 e2                             .....
```

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py` & `ares_ai-0.5.6/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/RAG_Automatic_Evaluation/ppi.py` & `ares_ai-0.5.6/ares/RAG_Automatic_Evaluation/ppi.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/__pycache__/ares.cpython-310.pyc` & `ares_ai-0.5.6/ares/__pycache__/ares.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/__pycache__/ares.cpython-311.pyc` & `ares_ai-0.5.6/ares/__pycache__/ares.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/__pycache__/binary_classifier.cpython-310.pyc` & `ares_ai-0.5.6/ares/__pycache__/binary_classifier.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/__pycache__/binary_classifier.cpython-311.pyc` & `ares_ai-0.5.6/ares/__pycache__/binary_classifier.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/__pycache__/rag_scoring.cpython-310.pyc` & `ares_ai-0.5.6/ares/__pycache__/rag_scoring.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/__pycache__/rag_scoring.cpython-311.pyc` & `ares_ai-0.5.6/ares/__pycache__/rag_scoring.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/__pycache__/synthetic_generator.cpython-310.pyc` & `ares_ai-0.5.6/ares/__pycache__/synthetic_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/__pycache__/synthetic_generator.cpython-311.pyc` & `ares_ai-0.5.6/ares/__pycache__/synthetic_generator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/__pycache__/ues_idp.cpython-310.pyc` & `ares_ai-0.5.6/ares/__pycache__/ues_idp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/__pycache__/ues_idp.cpython-311.pyc` & `ares_ai-0.5.6/ares/__pycache__/ues_idp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/ares.py` & `ares_ai-0.5.6/ares/ares.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/ares_ai.egg-info/PKG-INFO` & `ares_ai-0.5.6/ares/ares_ai.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/ares_ai.egg-info/requires.txt` & `ares_ai-0.5.6/ares/ares_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/binary_classifier.py` & `ares_ai-0.5.6/ares/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/ppi/.DS_Store` & `ares_ai-0.5.6/ares/ppi/.DS_Store`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/ppi/ppi.py` & `ares_ai-0.5.6/ares/ppi/ppi.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/ppi/ppi_testing.py` & `ares_ai-0.5.6/ares/ppi/ppi_testing.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/rag_scoring.py` & `ares_ai-0.5.6/ares/rag_scoring.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/synthetic_generator.py` & `ares_ai-0.5.6/ares/synthetic_generator.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares/ues_idp.py` & `ares_ai-0.5.6/ares/ues_idp.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/ares_ai.egg-info/PKG-INFO` & `ares_ai-0.5.6/ares_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ares-ai
-Version: 0.5.5
+Version: 0.5.6
 Summary: ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 Author-email: Jon Saad-Falcon <jonsaadfalcon@stanford.edu>, Robby Manihani <manihani@stanford.edu>, Omar Khattab <okhattab@stanford.edu>, Christopher Potts <cgpotts@stanford.edu>, Matei Zaharia <matei@berkeley.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ares_ai-0.5.5/ares_ai.egg-info/SOURCES.txt` & `ares_ai-0.5.6/ares_ai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -81,9 +81,8 @@
 ares/ppi/ppi_testing.py
 ares_ai.egg-info/PKG-INFO
 ares_ai.egg-info/SOURCES.txt
 ares_ai.egg-info/dependency_links.txt
 ares_ai.egg-info/entry_points.txt
 ares_ai.egg-info/requires.txt
 ares_ai.egg-info/top_level.txt
-checkpoints/.gitignore
 tests/.gitignore
```

### Comparing `ares_ai-0.5.5/ares_ai.egg-info/requires.txt` & `ares_ai-0.5.6/ares_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.5/pyproject.toml` & `ares_ai-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ares-ai"
-version = "0.5.5"
+version = "0.5.6"
 description = """ 
 ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 utilizing fine-tuned classifiers and synthetic data to assess performance efficiently. It streamlines 
 the evaluation of context relevance, answer faithfulness, and answer relevance with minimal human annotations.
 """
 readme = "README.md"
 authors = [
```

### Comparing `ares_ai-0.5.5/requirements.txt` & `ares_ai-0.5.6/requirements.txt`

 * *Files identical despite different names*

