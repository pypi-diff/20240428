# Comparing `tmp/autorag-0.1.6.tar.gz` & `tmp/autorag-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autorag-0.1.6.tar", last modified: Sat Apr 27 07:42:44 2024, max compression
+gzip compressed data, was "autorag-0.1.7.tar", last modified: Sun Apr 28 11:59:17 2024, max compression
```

## Comparing `autorag-0.1.6.tar` & `autorag-0.1.7.tar`

### file list

```diff
@@ -1,517 +1,515 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.145281 autorag-0.1.6/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.880763 autorag-0.1.6/.github/
--rw-r--r--   0 jeffrey    (501) staff       (20)      501 2024-01-13 07:55:28.000000 autorag-0.1.6/.github/dependabot.yml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.881645 autorag-0.1.6/.github/workflows/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1486 2024-04-27 07:08:56.000000 autorag-0.1.6/.github/workflows/publish.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-03-25 06:37:01.000000 autorag-0.1.6/.github/workflows/sphinx.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)      927 2024-04-27 01:36:13.000000 autorag-0.1.6/.github/workflows/test.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)     3088 2024-01-13 07:55:28.000000 autorag-0.1.6/.gitignore
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.144420 autorag-0.1.6/AutoRAG.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)    24168 2024-04-27 07:42:43.000000 autorag-0.1.6/AutoRAG.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)    19936 2024-04-27 07:42:43.000000 autorag-0.1.6/AutoRAG.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2024-04-27 07:42:43.000000 autorag-0.1.6/AutoRAG.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       44 2024-04-27 07:42:43.000000 autorag-0.1.6/AutoRAG.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      519 2024-04-27 07:42:43.000000 autorag-0.1.6/AutoRAG.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        8 2024-04-27 07:42:43.000000 autorag-0.1.6/AutoRAG.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     2936 2024-04-27 01:36:13.000000 autorag-0.1.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     6374 2024-04-27 01:36:13.000000 autorag-0.1.6/CONTRIBUTING.md
--rw-r--r--   0 jeffrey    (501) staff       (20)    11357 2024-01-13 07:55:28.000000 autorag-0.1.6/LICENSE
--rw-r--r--   0 jeffrey    (501) staff       (20)    24168 2024-04-27 07:42:44.144996 autorag-0.1.6/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     9161 2024-04-15 08:09:03.000000 autorag-0.1.6/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.884851 autorag-0.1.6/autorag/
--rw-r--r--   0 jeffrey    (501) staff       (20)        5 2024-04-27 06:36:55.000000 autorag-0.1.6/autorag/VERSION
--rw-r--r--   0 jeffrey    (501) staff       (20)     2686 2024-03-27 16:56:49.000000 autorag-0.1.6/autorag/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4400 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/cli.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.885204 autorag-0.1.6/autorag/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-04-01 09:28:42.000000 autorag-0.1.6/autorag/data/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.885881 autorag-0.1.6/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      134 2024-03-22 04:27:08.000000 autorag-0.1.6/autorag/data/corpus/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1538 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/data/corpus/langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3645 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/data/corpus/llama_index.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.887636 autorag-0.1.6/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-04-11 07:54:19.000000 autorag-0.1.6/autorag/data/qacreation/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3123 2024-04-15 08:09:03.000000 autorag-0.1.6/autorag/data/qacreation/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7473 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/data/qacreation/llama_index.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3190 2024-03-23 03:44:06.000000 autorag-0.1.6/autorag/data/qacreation/llama_index_default_prompt.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     2924 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/data/qacreation/ragas.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3289 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/data/qacreation/simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.888022 autorag-0.1.6/autorag/data/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/data/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1496 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/data/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8871 2024-03-06 00:03:36.000000 autorag-0.1.6/autorag/deploy.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.889442 autorag-0.1.6/autorag/evaluate/
--rw-r--r--   0 jeffrey    (501) staff       (20)      146 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/evaluate/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2603 2024-04-05 14:53:42.000000 autorag-0.1.6/autorag/evaluate/generation.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.890933 autorag-0.1.6/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)      252 2024-04-05 14:53:42.000000 autorag-0.1.6/autorag/evaluate/metric/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.893597 autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-02-23 11:07:36.000000 autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1015 2024-02-23 11:07:40.000000 autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-02-23 11:07:43.000000 autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1005 2024-02-23 11:07:46.000000 autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)    12720 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/evaluate/metric/generation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1671 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/evaluate/metric/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2310 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/evaluate/metric/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      224 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/evaluate/metric/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2052 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/evaluate/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2099 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/evaluate/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1290 2024-02-18 20:58:37.000000 autorag-0.1.6/autorag/evaluate/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    17379 2024-04-27 06:36:55.000000 autorag-0.1.6/autorag/evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/node_line.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.893887 autorag-0.1.6/autorag/nodes/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/nodes/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.895035 autorag-0.1.6/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)       68 2024-03-07 23:12:39.000000 autorag-0.1.6/autorag/nodes/generator/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2215 2024-03-07 22:31:53.000000 autorag-0.1.6/autorag/nodes/generator/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1641 2024-03-30 16:26:48.000000 autorag-0.1.6/autorag/nodes/generator/llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4532 2024-03-31 04:56:43.000000 autorag-0.1.6/autorag/nodes/generator/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2810 2024-03-08 18:01:40.000000 autorag-0.1.6/autorag/nodes/generator/vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.896087 autorag-0.1.6/autorag/nodes/passageaugmenter/
--rw-r--r--   0 jeffrey    (501) staff       (20)      112 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passageaugmenter/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4688 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passageaugmenter/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      388 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passageaugmenter/prev_next_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3555 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passageaugmenter/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.898797 autorag-0.1.6/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)      115 2024-04-15 08:09:03.000000 autorag-0.1.6/autorag/nodes/passagecompressor/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2445 2024-04-15 08:09:03.000000 autorag-0.1.6/autorag/nodes/passagecompressor/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      242 2024-02-22 15:32:30.000000 autorag-0.1.6/autorag/nodes/passagecompressor/pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2857 2024-04-15 08:09:03.000000 autorag-0.1.6/autorag/nodes/passagecompressor/refine.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6075 2024-02-15 17:28:32.000000 autorag-0.1.6/autorag/nodes/passagecompressor/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3028 2024-02-14 10:09:21.000000 autorag-0.1.6/autorag/nodes/passagecompressor/tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.900483 autorag-0.1.6/autorag/nodes/passagefilter/
--rw-r--r--   0 jeffrey    (501) staff       (20)      207 2024-04-15 08:09:03.000000 autorag-0.1.6/autorag/nodes/passagefilter/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2242 2024-04-15 08:09:03.000000 autorag-0.1.6/autorag/nodes/passagefilter/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      417 2024-04-11 14:32:56.000000 autorag-0.1.6/autorag/nodes/passagefilter/pass_passage_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3922 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/nodes/passagefilter/percentile_cutoff.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2399 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagefilter/recency.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4119 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagefilter/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4022 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/nodes/passagefilter/threshold_cutoff.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.905128 autorag-0.1.6/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      504 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/nodes/passagereranker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2236 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/nodes/passagereranker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3979 2024-03-17 04:13:16.000000 autorag-0.1.6/autorag/nodes/passagereranker/cohere.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5376 2024-04-27 06:36:55.000000 autorag-0.1.6/autorag/nodes/passagereranker/colbert.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2722 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagereranker/flag_embedding.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2397 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagereranker/flag_embedding_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3713 2024-04-06 14:23:40.000000 autorag-0.1.6/autorag/nodes/passagereranker/jina.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4186 2024-03-06 19:44:35.000000 autorag-0.1.6/autorag/nodes/passagereranker/koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5697 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagereranker/monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      618 2024-04-10 15:52:33.000000 autorag-0.1.6/autorag/nodes/passagereranker/pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4712 2024-04-05 03:16:26.000000 autorag-0.1.6/autorag/nodes/passagereranker/rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4335 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagereranker/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2884 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagereranker/sentence_transformer.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.905919 autorag-0.1.6/autorag/nodes/passagereranker/tart/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/nodes/passagereranker/tart/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4983 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3832 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/passagereranker/tart/tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4201 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5371 2024-04-27 02:56:02.000000 autorag-0.1.6/autorag/nodes/passagereranker/temp_new_colbert.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7555 2024-04-27 01:40:21.000000 autorag-0.1.6/autorag/nodes/passagereranker/temp_old_upr.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-12 13:21:50.000000 autorag-0.1.6/autorag/nodes/passagereranker/time_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7555 2024-04-27 06:36:55.000000 autorag-0.1.6/autorag/nodes/passagereranker/upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.907317 autorag-0.1.6/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)       84 2024-04-09 15:31:49.000000 autorag-0.1.6/autorag/nodes/promptmaker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1379 2024-04-09 15:31:49.000000 autorag-0.1.6/autorag/nodes/promptmaker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1162 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/nodes/promptmaker/fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2290 2024-04-09 15:31:49.000000 autorag-0.1.6/autorag/nodes/promptmaker/long_context_reorder.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8925 2024-03-31 10:20:41.000000 autorag-0.1.6/autorag/nodes/promptmaker/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.908988 autorag-0.1.6/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      123 2024-02-22 15:32:30.000000 autorag-0.1.6/autorag/nodes/queryexpansion/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1663 2024-03-06 19:11:31.000000 autorag-0.1.6/autorag/nodes/queryexpansion/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1572 2024-02-14 10:09:21.000000 autorag-0.1.6/autorag/nodes/queryexpansion/hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-22 15:32:30.000000 autorag-0.1.6/autorag/nodes/queryexpansion/pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3491 2024-02-14 10:09:21.000000 autorag-0.1.6/autorag/nodes/queryexpansion/query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7932 2024-02-15 17:29:26.000000 autorag-0.1.6/autorag/nodes/queryexpansion/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.911868 autorag-0.1.6/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      227 2024-04-11 14:29:33.000000 autorag-0.1.6/autorag/nodes/retrieval/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6444 2024-04-11 14:29:33.000000 autorag-0.1.6/autorag/nodes/retrieval/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5637 2024-03-25 04:14:52.000000 autorag-0.1.6/autorag/nodes/retrieval/bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3122 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/nodes/retrieval/hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3221 2024-04-11 14:29:33.000000 autorag-0.1.6/autorag/nodes/retrieval/hybrid_dbsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2957 2024-02-13 22:39:30.000000 autorag-0.1.6/autorag/nodes/retrieval/hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4148 2024-04-11 14:29:33.000000 autorag-0.1.6/autorag/nodes/retrieval/hybrid_rsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    10949 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/retrieval/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4907 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/nodes/retrieval/vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.912599 autorag-0.1.6/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)       50 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/schema/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      722 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/schema/module.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4158 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/schema/node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3996 2024-02-13 20:12:31.000000 autorag-0.1.6/autorag/strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4202 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/support.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.913384 autorag-0.1.6/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)      237 2024-04-27 06:36:55.000000 autorag-0.1.6/autorag/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4020 2024-04-27 06:36:55.000000 autorag-0.1.6/autorag/utils/preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    12038 2024-04-27 01:36:13.000000 autorag-0.1.6/autorag/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2563 2024-03-06 00:03:36.000000 autorag-0.1.6/autorag/web.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       73 2024-04-27 01:36:13.000000 autorag-0.1.6/dev_requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.914188 autorag-0.1.6/docs/
--rw-r--r--   0 jeffrey    (501) staff       (20)      638 2024-01-17 16:38:11.000000 autorag-0.1.6/docs/Makefile
--rw-r--r--   0 jeffrey    (501) staff       (20)      804 2024-01-17 11:55:21.000000 autorag-0.1.6/docs/make.bat
--rw-r--r--   0 jeffrey    (501) staff       (20)      125 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.916159 autorag-0.1.6/docs/source/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.922714 autorag-0.1.6/docs/source/_static/
--rw-r--r--   0 jeffrey    (501) staff       (20)    57124 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/data_creation.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    30770 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/data_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    31538 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/node_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    18941 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/node_line_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    42589 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/node_line_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    92939 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/node_lines.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    95669 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/node_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    36728 2024-02-07 10:54:42.000000 autorag-0.1.6/docs/source/_static/project_folder_example.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    19853 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/project_folders.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    22432 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/resources_folder.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.927026 autorag-0.1.6/docs/source/_static/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)   159068 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/_static/roadmap/RAG_paradigms.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    38568 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/_static/roadmap/advanced_RAG.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    62853 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/_static/roadmap/cycle.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    75826 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/_static/roadmap/merger.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    82200 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/_static/roadmap/node_line_modular.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    69999 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/_static/roadmap/policy.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   567356 2024-02-07 10:54:42.000000 autorag-0.1.6/docs/source/_static/samsung_sundae.jpeg
--rw-r--r--   0 jeffrey    (501) staff       (20)    37348 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/trial_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    25499 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/trial_json.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   177107 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/_static/trial_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   269046 2024-03-06 00:03:36.000000 autorag-0.1.6/docs/source/_static/web_interface.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.934553 autorag-0.1.6/docs/source/api_spec/
--rw-r--r--   0 jeffrey    (501) staff       (20)      563 2024-03-22 04:34:21.000000 autorag-0.1.6/docs/source/api_spec/autorag.data.corpus.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      939 2024-04-14 04:49:44.000000 autorag-0.1.6/docs/source/api_spec/autorag.data.qacreation.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      287 2024-03-22 04:34:21.000000 autorag-0.1.6/docs/source/api_spec/autorag.data.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      358 2024-03-22 04:34:21.000000 autorag-0.1.6/docs/source/api_spec/autorag.data.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      984 2024-02-10 14:23:30.000000 autorag-0.1.6/docs/source/api_spec/autorag.evaluate.metric.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      962 2024-02-10 14:23:30.000000 autorag-0.1.6/docs/source/api_spec/autorag.evaluate.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      941 2024-03-17 04:13:16.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.generator.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      864 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1294 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagecompressor.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1471 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagefilter.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     3434 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagereranker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      952 2024-02-01 16:32:39.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      995 2024-04-09 15:31:49.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.promptmaker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1254 2024-02-22 15:32:30.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.queryexpansion.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1896 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.retrieval.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      466 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/api_spec/autorag.nodes.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1239 2024-03-07 15:58:42.000000 autorag-0.1.6/docs/source/api_spec/autorag.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      486 2024-01-17 15:59:52.000000 autorag-0.1.6/docs/source/api_spec/autorag.schema.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      489 2024-01-17 15:59:52.000000 autorag-0.1.6/docs/source/api_spec/autorag.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-01-17 15:59:52.000000 autorag-0.1.6/docs/source/api_spec/modules.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1454 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/conf.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.935406 autorag-0.1.6/docs/source/data_creation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     5072 2024-02-18 20:58:37.000000 autorag-0.1.6/docs/source/data_creation/data_format.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2206 2024-04-12 13:21:50.000000 autorag-0.1.6/docs/source/data_creation/ragas.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     5543 2024-03-25 11:47:15.000000 autorag-0.1.6/docs/source/data_creation/tutorial.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.935908 autorag-0.1.6/docs/source/deploy/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1473 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/deploy/api_endpoint.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      912 2024-03-06 00:03:36.000000 autorag-0.1.6/docs/source/deploy/web.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4124 2024-04-12 13:21:50.000000 autorag-0.1.6/docs/source/index.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1891 2024-02-15 09:50:25.000000 autorag-0.1.6/docs/source/install.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     6153 2024-04-12 13:21:50.000000 autorag-0.1.6/docs/source/local_model.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.936241 autorag-0.1.6/docs/source/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.936941 autorag-0.1.6/docs/source/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2703 2024-04-05 14:53:42.000000 autorag-0.1.6/docs/source/nodes/generator/generator.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1306 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/generator/llama_index_llm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1358 2024-03-14 09:00:38.000000 autorag-0.1.6/docs/source/nodes/generator/vllm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      172 2024-04-11 14:29:33.000000 autorag-0.1.6/docs/source/nodes/index.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.937410 autorag-0.1.6/docs/source/nodes/passage_augmenter/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1591 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/nodes/passage_augmenter/passage_augmenter.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      727 2024-04-27 01:36:13.000000 autorag-0.1.6/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.938562 autorag-0.1.6/docs/source/nodes/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3046 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/nodes/passage_compressor/passage_compressor.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1182 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/nodes/passage_compressor/refine.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1252 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/passage_compressor/tree_summarize.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.939786 autorag-0.1.6/docs/source/nodes/passage_filter/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1765 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/nodes/passage_filter/passage_filter.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1127 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/nodes/passage_filter/recency_filter.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1028 2024-04-12 13:21:50.000000 autorag-0.1.6/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1085 2024-04-10 13:46:46.000000 autorag-0.1.6/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.945094 autorag-0.1.6/docs/source/nodes/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1151 2024-03-17 04:13:16.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/cohere.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      521 2024-04-08 12:04:54.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/colbert.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      675 2024-04-11 14:29:33.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      654 2024-04-11 14:29:33.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1232 2024-04-06 14:23:40.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/jina_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      366 2024-02-22 16:33:58.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/koreranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1567 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/monot5.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2372 2024-04-15 08:09:03.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/passage_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-04-05 03:16:26.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/rankgpt.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      645 2024-04-08 08:26:20.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      515 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/tart.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      561 2024-04-12 13:21:50.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/time_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1435 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/passage_reranker/upr.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.946003 autorag-0.1.6/docs/source/nodes/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      585 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/prompt_maker/fstring.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      815 2024-04-09 15:31:49.000000 autorag-0.1.6/docs/source/nodes/prompt_maker/long_context_reorder.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2689 2024-04-09 15:31:49.000000 autorag-0.1.6/docs/source/nodes/prompt_maker/prompt_maker.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.946535 autorag-0.1.6/docs/source/nodes/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1178 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/query_expansion/hyde.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1330 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/query_expansion/query_decompose.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3272 2024-02-22 15:32:30.000000 autorag-0.1.6/docs/source/nodes/query_expansion/query_expansion.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.948424 autorag-0.1.6/docs/source/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      625 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/retrieval/bm25.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-10 06:33:52.000000 autorag-0.1.6/docs/source/nodes/retrieval/hybrid_cc.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2294 2024-04-11 14:29:33.000000 autorag-0.1.6/docs/source/nodes/retrieval/hybrid_dbsf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2053 2024-04-10 06:33:52.000000 autorag-0.1.6/docs/source/nodes/retrieval/hybrid_rrf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2304 2024-04-10 06:33:52.000000 autorag-0.1.6/docs/source/nodes/retrieval/hybrid_rsf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1910 2024-04-11 14:29:33.000000 autorag-0.1.6/docs/source/nodes/retrieval/retrieval.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1223 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/nodes/retrieval/vectordb.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.949443 autorag-0.1.6/docs/source/optimization/
--rw-r--r--   0 jeffrey    (501) staff       (20)     4160 2024-02-15 10:23:20.000000 autorag-0.1.6/docs/source/optimization/custom_config.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3779 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/optimization/folder_structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4596 2024-02-07 21:46:19.000000 autorag-0.1.6/docs/source/optimization/optimization.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2580 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/optimization/sample_full_config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.949655 autorag-0.1.6/docs/source/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)     6735 2024-02-07 21:45:07.000000 autorag-0.1.6/docs/source/roadmap/modular_rag.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3032 2024-02-08 11:27:02.000000 autorag-0.1.6/docs/source/structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3121 2024-02-18 20:58:37.000000 autorag-0.1.6/docs/source/troubleshooting.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     8338 2024-03-29 05:05:10.000000 autorag-0.1.6/docs/source/tutorial.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1529 2024-04-26 05:39:23.000000 autorag-0.1.6/pyproject.toml
--rw-r--r--   0 jeffrey    (501) staff       (20)     1156 2024-04-27 01:36:13.000000 autorag-0.1.6/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.951739 autorag-0.1.6/sample_config/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2101 2024-03-14 09:00:38.000000 autorag-0.1.6/sample_config/compact_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2420 2024-03-17 04:13:16.000000 autorag-0.1.6/sample_config/compact_openai.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     1222 2024-03-17 04:13:16.000000 autorag-0.1.6/sample_config/config_korean.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      976 2024-03-06 00:03:36.000000 autorag-0.1.6/sample_config/extracted_sample.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     4769 2024-04-27 01:36:13.000000 autorag-0.1.6/sample_config/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      896 2024-03-14 09:00:38.000000 autorag-0.1.6/sample_config/simple_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      863 2024-02-08 11:27:02.000000 autorag-0.1.6/sample_config/simple_openai.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.951958 autorag-0.1.6/sample_dataset/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1404 2024-02-05 20:46:09.000000 autorag-0.1.6/sample_dataset/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.952387 autorag-0.1.6/sample_dataset/eli5/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1109 2024-02-05 20:46:09.000000 autorag-0.1.6/sample_dataset/eli5/load_eli5_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.952667 autorag-0.1.6/sample_dataset/msmarco/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1167 2024-02-05 20:46:09.000000 autorag-0.1.6/sample_dataset/msmarco/load_msmarco_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.952980 autorag-0.1.6/sample_dataset/triviaqa/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1171 2024-02-07 10:54:45.000000 autorag-0.1.6/sample_dataset/triviaqa/load_triviaqa_dataset.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2024-04-27 07:42:44.145331 autorag-0.1.6/setup.cfg
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.954226 autorag-0.1.6/tests/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.955873 autorag-0.1.6/tests/autorag/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.875777 autorag-0.1.6/tests/autorag/data/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.956785 autorag-0.1.6/tests/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      620 2024-03-22 04:29:06.000000 autorag-0.1.6/tests/autorag/data/corpus/test_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      646 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/data/corpus/test_langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1317 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/data/corpus/test_llama_index_corpus.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.958163 autorag-0.1.6/tests/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/data/qacreation/test_base_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3129 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/data/qacreation/test_llama_index_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      897 2024-04-12 13:21:50.000000 autorag-0.1.6/tests/autorag/data/qacreation/test_ragas_qa_creation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2097 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/data/qacreation/test_simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.959217 autorag-0.1.6/tests/autorag/evaluate/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.959937 autorag-0.1.6/tests/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3551 2024-04-05 14:53:42.000000 autorag-0.1.6/tests/autorag/evaluate/metric/test_generation_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1731 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1634 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/evaluate/metric/test_retrieval_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1263 2024-03-08 17:59:53.000000 autorag-0.1.6/tests/autorag/evaluate/test_evaluate_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4701 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/evaluate/test_generation_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1460 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2007 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/evaluate/test_retrieval_evaluate.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.876452 autorag-0.1.6/tests/autorag/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.961058 autorag-0.1.6/tests/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)      687 2024-03-08 18:01:40.000000 autorag-0.1.6/tests/autorag/nodes/generator/test_generator_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1372 2024-03-08 17:13:58.000000 autorag-0.1.6/tests/autorag/nodes/generator/test_llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3263 2024-03-31 05:05:12.000000 autorag-0.1.6/tests/autorag/nodes/generator/test_run_generator_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1004 2024-03-08 18:15:21.000000 autorag-0.1.6/tests/autorag/nodes/generator/test_vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.961918 autorag-0.1.6/tests/autorag/nodes/passageaugmenter/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1159 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      751 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2594 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3080 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.963308 autorag-0.1.6/tests/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-04-15 08:09:03.000000 autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      820 2024-02-22 15:32:30.000000 autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1852 2024-04-15 08:09:03.000000 autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_refine.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5073 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1933 2024-04-15 08:09:03.000000 autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.965582 autorag-0.1.6/tests/autorag/nodes/passagefilter/
--rw-r--r--   0 jeffrey    (501) staff       (20)      710 2024-04-11 14:32:56.000000 autorag-0.1.6/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3615 2024-04-15 08:09:03.000000 autorag-0.1.6/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2999 2024-04-10 13:46:46.000000 autorag-0.1.6/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      981 2024-04-12 13:21:50.000000 autorag-0.1.6/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4380 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagefilter/test_recency_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      860 2024-04-10 13:46:46.000000 autorag-0.1.6/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.970081 autorag-0.1.6/tests/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1160 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3283 2024-04-27 06:36:55.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1994 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_flag_embedding.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2213 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1881 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_jina_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-02-22 16:33:58.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1407 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-02-22 15:32:30.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4364 2024-04-27 06:36:55.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4830 2024-02-18 20:58:37.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2230 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1604 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1371 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1210 2024-04-12 13:21:50.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_time_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      956 2024-04-27 06:36:55.000000 autorag-0.1.6/tests/autorag/nodes/passagereranker/test_upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.972069 autorag-0.1.6/tests/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1373 2024-04-09 15:31:49.000000 autorag-0.1.6/tests/autorag/nodes/promptmaker/test_fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1798 2024-04-09 15:31:49.000000 autorag-0.1.6/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      580 2024-04-09 15:31:49.000000 autorag-0.1.6/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8310 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.973767 autorag-0.1.6/tests/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      813 2024-02-22 15:48:12.000000 autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      544 2024-02-22 15:32:30.000000 autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-22 15:56:28.000000 autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1586 2024-02-15 09:47:24.000000 autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6880 2024-02-22 16:17:25.000000 autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.977232 autorag-0.1.6/tests/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2906 2024-03-25 03:54:12.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4013 2024-04-11 14:29:33.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1525 2024-04-11 14:29:33.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      879 2024-04-11 14:29:33.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2989 2024-04-10 06:33:52.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      780 2024-04-11 14:29:33.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2976 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_retrieval_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    11185 2024-03-23 14:00:14.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4692 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/nodes/retrieval/test_vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.977962 autorag-0.1.6/tests/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1033 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/schema/test_module_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5515 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/schema/test_node_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3118 2024-03-29 05:05:10.000000 autorag-0.1.6/tests/autorag/test_cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6869 2024-04-10 13:46:46.000000 autorag-0.1.6/tests/autorag/test_deploy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    14669 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/test_evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2081 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/test_strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      306 2024-02-13 20:13:32.000000 autorag-0.1.6/tests/autorag/test_support.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      878 2024-03-06 00:03:36.000000 autorag-0.1.6/tests/autorag/test_web.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.978741 autorag-0.1.6/tests/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3773 2024-04-27 06:36:55.000000 autorag-0.1.6/tests/autorag/utils/test_preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     9970 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/autorag/utils/test_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-23 03:44:06.000000 autorag-0.1.6/tests/conftest.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      672 2024-02-18 20:58:37.000000 autorag-0.1.6/tests/delete_tests.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2641 2024-02-22 16:04:39.000000 autorag-0.1.6/tests/mock.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.982321 autorag-0.1.6/tests/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-03-23 03:44:06.000000 autorag-0.1.6/tests/resources/README.md
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.6/tests/resources/corpus_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.876758 autorag-0.1.6/tests/resources/data_creation/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.983395 autorag-0.1.6/tests/resources/data_creation/raw_dir/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3379 2024-02-08 11:27:05.000000 autorag-0.1.6/tests/resources/data_creation/raw_dir/sample1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3243 2024-02-08 11:27:05.000000 autorag-0.1.6/tests/resources/data_creation/raw_dir/sample2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     4563 2024-02-08 11:27:05.000000 autorag-0.1.6/tests/resources/data_creation/raw_dir/sample3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3235 2024-04-12 16:43:24.000000 autorag-0.1.6/tests/resources/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.6/tests/resources/qa_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.984480 autorag-0.1.6/tests/resources/qa_gen_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)      198 2024-04-17 01:53:11.000000 autorag-0.1.6/tests/resources/qa_gen_prompts/prompt1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      186 2024-03-23 03:44:06.000000 autorag-0.1.6/tests/resources/qa_gen_prompts/prompt2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      202 2024-03-23 03:44:06.000000 autorag-0.1.6/tests/resources/qa_gen_prompts/prompt3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     5910 2024-02-07 10:54:45.000000 autorag-0.1.6/tests/resources/qa_test_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.985179 autorag-0.1.6/tests/resources/result_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.985978 autorag-0.1.6/tests/resources/result_project/0/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2297 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.986524 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.990866 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)    23516 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    26448 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    33716 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14618 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14683 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    13278 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    54234 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     1155 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.996673 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     8443 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    41557 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      513 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.997050 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.999166 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.999506 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.000654 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.002820 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.004956 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      845 2024-02-18 14:46:34.000000 autorag-0.1.6/tests/resources/result_project/0/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.005203 autorag-0.1.6/tests/resources/result_project/1/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.005881 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.008094 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.878005 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.008413 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.009614 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.116036 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.116512 autorag-0.1.6/tests/resources/result_project/2/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.878189 autorag-0.1.6/tests/resources/result_project/2/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.117092 autorag-0.1.6/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.117494 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.122495 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.122821 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.124069 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.126726 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.129135 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.129399 autorag-0.1.6/tests/resources/result_project/3/
--rw-r--r--   0 jeffrey    (501) staff       (20)      682 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/3/config.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2307 2024-03-29 05:05:10.000000 autorag-0.1.6/tests/resources/result_project/best.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.131748 autorag-0.1.6/tests/resources/result_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.132082 autorag-0.1.6/tests/resources/result_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-02-03 19:10:47.000000 autorag-0.1.6/tests/resources/result_project/resources/bm25.pkl
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.132422 autorag-0.1.6/tests/resources/result_project/resources/chroma/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.141537 autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
--rw-r--r--   0 jeffrey    (501) staff       (20)  6284000 2024-02-18 14:41:41.000000 autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)      100 2024-02-18 14:41:00.000000 autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)     4000 2024-02-18 14:41:41.000000 autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-18 14:41:00.000000 autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)   352256 2024-02-18 14:41:41.000000 autorag-0.1.6/tests/resources/result_project/resources/chroma/chroma.sqlite3
--rw-r--r--   0 jeffrey    (501) staff       (20)      338 2024-03-25 11:47:36.000000 autorag-0.1.6/tests/resources/result_project/trial.json
--rw-r--r--   0 jeffrey    (501) staff       (20)     8439 2024-03-23 03:44:06.000000 autorag-0.1.6/tests/resources/sample_contents_nqa.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:43.879104 autorag-0.1.6/tests/resources/sample_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.142756 autorag-0.1.6/tests/resources/sample_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   115302 2024-04-27 01:36:13.000000 autorag-0.1.6/tests/resources/sample_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.6/tests/resources/sample_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-27 07:42:44.143471 autorag-0.1.6/tests/resources/sample_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-01-13 07:56:04.000000 autorag-0.1.6/tests/resources/sample_project/resources/bm25.pkl
--rw-r--r--   0 jeffrey    (501) staff       (20)      893 2024-04-10 13:46:46.000000 autorag-0.1.6/tests/resources/simple.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)    26773 2024-01-13 07:56:04.000000 autorag-0.1.6/tests/resources/test_bm25_retrieval.pkl
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.515210 autorag-0.1.7/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.395358 autorag-0.1.7/.github/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      501 2024-01-13 07:55:28.000000 autorag-0.1.7/.github/dependabot.yml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.395939 autorag-0.1.7/.github/workflows/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1486 2024-04-28 11:59:07.000000 autorag-0.1.7/.github/workflows/publish.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-03-25 06:37:01.000000 autorag-0.1.7/.github/workflows/sphinx.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      927 2024-04-27 01:36:13.000000 autorag-0.1.7/.github/workflows/test.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3088 2024-01-13 07:55:28.000000 autorag-0.1.7/.gitignore
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.514309 autorag-0.1.7/AutoRAG.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    24187 2024-04-28 11:59:17.000000 autorag-0.1.7/AutoRAG.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)    19840 2024-04-28 11:59:17.000000 autorag-0.1.7/AutoRAG.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2024-04-28 11:59:17.000000 autorag-0.1.7/AutoRAG.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       44 2024-04-28 11:59:17.000000 autorag-0.1.7/AutoRAG.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      523 2024-04-28 11:59:17.000000 autorag-0.1.7/AutoRAG.egg-info/requires.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        8 2024-04-28 11:59:17.000000 autorag-0.1.7/AutoRAG.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2936 2024-04-27 01:36:13.000000 autorag-0.1.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6374 2024-04-27 01:36:13.000000 autorag-0.1.7/CONTRIBUTING.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11357 2024-01-13 07:55:28.000000 autorag-0.1.7/LICENSE
+-rw-r--r--   0 jeffrey    (501) staff       (20)    24187 2024-04-28 11:59:17.514924 autorag-0.1.7/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9161 2024-04-15 08:09:03.000000 autorag-0.1.7/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.399209 autorag-0.1.7/autorag/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        5 2024-04-28 09:01:51.000000 autorag-0.1.7/autorag/VERSION
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2686 2024-04-27 14:09:04.000000 autorag-0.1.7/autorag/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4400 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/cli.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.399448 autorag-0.1.7/autorag/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-04-01 09:28:42.000000 autorag-0.1.7/autorag/data/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.400100 autorag-0.1.7/autorag/data/corpus/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      134 2024-03-22 04:27:08.000000 autorag-0.1.7/autorag/data/corpus/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1538 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/data/corpus/langchain.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3645 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/data/corpus/llama_index.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.401971 autorag-0.1.7/autorag/data/qacreation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-04-11 07:54:19.000000 autorag-0.1.7/autorag/data/qacreation/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3123 2024-04-15 08:09:03.000000 autorag-0.1.7/autorag/data/qacreation/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7473 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/data/qacreation/llama_index.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3190 2024-03-23 03:44:06.000000 autorag-0.1.7/autorag/data/qacreation/llama_index_default_prompt.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2924 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/data/qacreation/ragas.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3289 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/data/qacreation/simple.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.402377 autorag-0.1.7/autorag/data/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/data/utils/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1496 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/data/utils/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8871 2024-03-06 00:03:36.000000 autorag-0.1.7/autorag/deploy.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.403838 autorag-0.1.7/autorag/evaluate/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      146 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/evaluate/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2603 2024-04-05 14:53:42.000000 autorag-0.1.7/autorag/evaluate/generation.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.405407 autorag-0.1.7/autorag/evaluate/metric/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      252 2024-04-05 14:53:42.000000 autorag-0.1.7/autorag/evaluate/metric/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.406447 autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-02-23 11:07:36.000000 autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1015 2024-02-23 11:07:40.000000 autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-02-23 11:07:43.000000 autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1005 2024-02-23 11:07:46.000000 autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)    12720 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/evaluate/metric/generation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1671 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/evaluate/metric/retrieval.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2310 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/evaluate/metric/retrieval_contents.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      224 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/evaluate/metric/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2052 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/evaluate/retrieval.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2099 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/evaluate/retrieval_contents.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1290 2024-02-18 20:58:37.000000 autorag-0.1.7/autorag/evaluate/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    17379 2024-04-27 15:42:07.000000 autorag-0.1.7/autorag/evaluator.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/node_line.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.406684 autorag-0.1.7/autorag/nodes/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/nodes/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.407779 autorag-0.1.7/autorag/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       68 2024-03-07 23:12:39.000000 autorag-0.1.7/autorag/nodes/generator/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2215 2024-03-07 22:31:53.000000 autorag-0.1.7/autorag/nodes/generator/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1641 2024-03-30 16:26:48.000000 autorag-0.1.7/autorag/nodes/generator/llama_index_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4532 2024-03-31 04:56:43.000000 autorag-0.1.7/autorag/nodes/generator/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2810 2024-03-08 18:01:40.000000 autorag-0.1.7/autorag/nodes/generator/vllm.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.408670 autorag-0.1.7/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      112 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passageaugmenter/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4688 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passageaugmenter/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      388 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passageaugmenter/prev_next_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3555 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/nodes/passageaugmenter/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.410248 autorag-0.1.7/autorag/nodes/passagecompressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      115 2024-04-15 08:09:03.000000 autorag-0.1.7/autorag/nodes/passagecompressor/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2445 2024-04-15 08:09:03.000000 autorag-0.1.7/autorag/nodes/passagecompressor/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      242 2024-02-22 15:32:30.000000 autorag-0.1.7/autorag/nodes/passagecompressor/pass_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2857 2024-04-15 08:09:03.000000 autorag-0.1.7/autorag/nodes/passagecompressor/refine.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6075 2024-02-15 17:28:32.000000 autorag-0.1.7/autorag/nodes/passagecompressor/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3028 2024-02-14 10:09:21.000000 autorag-0.1.7/autorag/nodes/passagecompressor/tree_summarize.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.411861 autorag-0.1.7/autorag/nodes/passagefilter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      207 2024-04-15 08:09:03.000000 autorag-0.1.7/autorag/nodes/passagefilter/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2242 2024-04-15 08:09:03.000000 autorag-0.1.7/autorag/nodes/passagefilter/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      417 2024-04-11 14:32:56.000000 autorag-0.1.7/autorag/nodes/passagefilter/pass_passage_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3922 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/nodes/passagefilter/percentile_cutoff.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2399 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passagefilter/recency.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4119 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/nodes/passagefilter/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4022 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/nodes/passagefilter/threshold_cutoff.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.416033 autorag-0.1.7/autorag/nodes/passagereranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      504 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/nodes/passagereranker/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2236 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/nodes/passagereranker/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3979 2024-03-17 04:13:16.000000 autorag-0.1.7/autorag/nodes/passagereranker/cohere.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5376 2024-04-27 15:42:07.000000 autorag-0.1.7/autorag/nodes/passagereranker/colbert.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2722 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passagereranker/flag_embedding.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2397 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passagereranker/flag_embedding_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3713 2024-04-06 14:23:40.000000 autorag-0.1.7/autorag/nodes/passagereranker/jina.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4186 2024-03-06 19:44:35.000000 autorag-0.1.7/autorag/nodes/passagereranker/koreranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5697 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passagereranker/monot5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      618 2024-04-10 15:52:33.000000 autorag-0.1.7/autorag/nodes/passagereranker/pass_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4712 2024-04-05 03:16:26.000000 autorag-0.1.7/autorag/nodes/passagereranker/rankgpt.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4335 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/nodes/passagereranker/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2884 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passagereranker/sentence_transformer.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.416836 autorag-0.1.7/autorag/nodes/passagereranker/tart/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/nodes/passagereranker/tart/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4983 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3832 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/nodes/passagereranker/tart/tart.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4201 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-12 13:21:50.000000 autorag-0.1.7/autorag/nodes/passagereranker/time_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5867 2024-04-27 15:32:19.000000 autorag-0.1.7/autorag/nodes/passagereranker/upr.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.418124 autorag-0.1.7/autorag/nodes/promptmaker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       84 2024-04-09 15:31:49.000000 autorag-0.1.7/autorag/nodes/promptmaker/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1379 2024-04-09 15:31:49.000000 autorag-0.1.7/autorag/nodes/promptmaker/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1162 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/nodes/promptmaker/fstring.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2290 2024-04-09 15:31:49.000000 autorag-0.1.7/autorag/nodes/promptmaker/long_context_reorder.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8925 2024-03-31 10:20:41.000000 autorag-0.1.7/autorag/nodes/promptmaker/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.419532 autorag-0.1.7/autorag/nodes/queryexpansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      123 2024-02-22 15:32:30.000000 autorag-0.1.7/autorag/nodes/queryexpansion/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1663 2024-03-06 19:11:31.000000 autorag-0.1.7/autorag/nodes/queryexpansion/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1572 2024-02-14 10:09:21.000000 autorag-0.1.7/autorag/nodes/queryexpansion/hyde.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-22 15:32:30.000000 autorag-0.1.7/autorag/nodes/queryexpansion/pass_query_expansion.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3491 2024-02-14 10:09:21.000000 autorag-0.1.7/autorag/nodes/queryexpansion/query_decompose.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7932 2024-02-15 17:29:26.000000 autorag-0.1.7/autorag/nodes/queryexpansion/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.421741 autorag-0.1.7/autorag/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      227 2024-04-11 14:29:33.000000 autorag-0.1.7/autorag/nodes/retrieval/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6444 2024-04-11 14:29:33.000000 autorag-0.1.7/autorag/nodes/retrieval/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5637 2024-03-25 04:14:52.000000 autorag-0.1.7/autorag/nodes/retrieval/bm25.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3122 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/nodes/retrieval/hybrid_cc.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3221 2024-04-11 14:29:33.000000 autorag-0.1.7/autorag/nodes/retrieval/hybrid_dbsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2957 2024-02-13 22:39:30.000000 autorag-0.1.7/autorag/nodes/retrieval/hybrid_rrf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4148 2024-04-11 14:29:33.000000 autorag-0.1.7/autorag/nodes/retrieval/hybrid_rsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    10949 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/nodes/retrieval/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4907 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/nodes/retrieval/vectordb.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.422437 autorag-0.1.7/autorag/schema/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       50 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/schema/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      722 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/schema/module.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4158 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/schema/node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3996 2024-02-13 20:12:31.000000 autorag-0.1.7/autorag/strategy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4202 2024-04-27 01:36:13.000000 autorag-0.1.7/autorag/support.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.423221 autorag-0.1.7/autorag/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      237 2024-04-27 15:42:07.000000 autorag-0.1.7/autorag/utils/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4020 2024-04-27 15:42:07.000000 autorag-0.1.7/autorag/utils/preprocess.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    12038 2024-04-27 07:48:36.000000 autorag-0.1.7/autorag/utils/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2563 2024-03-06 00:03:36.000000 autorag-0.1.7/autorag/web.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)       73 2024-04-27 01:36:13.000000 autorag-0.1.7/dev_requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.424160 autorag-0.1.7/docs/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      638 2024-01-17 16:38:11.000000 autorag-0.1.7/docs/Makefile
+-rw-r--r--   0 jeffrey    (501) staff       (20)      804 2024-01-17 11:55:21.000000 autorag-0.1.7/docs/make.bat
+-rw-r--r--   0 jeffrey    (501) staff       (20)      125 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.426113 autorag-0.1.7/docs/source/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.434500 autorag-0.1.7/docs/source/_static/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    57124 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/data_creation.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    30770 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/data_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31538 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/node_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    18941 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/node_line_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    42589 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/node_line_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    92939 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/node_lines.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    95669 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/node_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    36728 2024-02-07 10:54:42.000000 autorag-0.1.7/docs/source/_static/project_folder_example.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    19853 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/project_folders.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    22432 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/resources_folder.png
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.438167 autorag-0.1.7/docs/source/_static/roadmap/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   159068 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/_static/roadmap/RAG_paradigms.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    38568 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/_static/roadmap/advanced_RAG.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    62853 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/_static/roadmap/cycle.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    75826 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/_static/roadmap/merger.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    82200 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/_static/roadmap/node_line_modular.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    69999 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/_static/roadmap/policy.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   567356 2024-02-07 10:54:42.000000 autorag-0.1.7/docs/source/_static/samsung_sundae.jpeg
+-rw-r--r--   0 jeffrey    (501) staff       (20)    37348 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/trial_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    25499 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/trial_json.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   177107 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/_static/trial_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   269046 2024-03-06 00:03:36.000000 autorag-0.1.7/docs/source/_static/web_interface.png
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.443566 autorag-0.1.7/docs/source/api_spec/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      563 2024-03-22 04:34:21.000000 autorag-0.1.7/docs/source/api_spec/autorag.data.corpus.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      939 2024-04-14 04:49:44.000000 autorag-0.1.7/docs/source/api_spec/autorag.data.qacreation.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      287 2024-03-22 04:34:21.000000 autorag-0.1.7/docs/source/api_spec/autorag.data.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      358 2024-03-22 04:34:21.000000 autorag-0.1.7/docs/source/api_spec/autorag.data.utils.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      984 2024-02-10 14:23:30.000000 autorag-0.1.7/docs/source/api_spec/autorag.evaluate.metric.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      962 2024-02-10 14:23:30.000000 autorag-0.1.7/docs/source/api_spec/autorag.evaluate.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      941 2024-03-17 04:13:16.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.generator.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      864 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1294 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagecompressor.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1471 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagefilter.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3434 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagereranker.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      952 2024-02-01 16:32:39.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      995 2024-04-09 15:31:49.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.promptmaker.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1254 2024-02-22 15:32:30.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.queryexpansion.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1896 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.retrieval.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      466 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/api_spec/autorag.nodes.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1239 2024-03-07 15:58:42.000000 autorag-0.1.7/docs/source/api_spec/autorag.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      486 2024-01-17 15:59:52.000000 autorag-0.1.7/docs/source/api_spec/autorag.schema.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      489 2024-01-17 15:59:52.000000 autorag-0.1.7/docs/source/api_spec/autorag.utils.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-01-17 15:59:52.000000 autorag-0.1.7/docs/source/api_spec/modules.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1454 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/conf.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.444432 autorag-0.1.7/docs/source/data_creation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5072 2024-02-18 20:58:37.000000 autorag-0.1.7/docs/source/data_creation/data_format.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2206 2024-04-12 13:21:50.000000 autorag-0.1.7/docs/source/data_creation/ragas.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5543 2024-03-25 11:47:15.000000 autorag-0.1.7/docs/source/data_creation/tutorial.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.444902 autorag-0.1.7/docs/source/deploy/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1473 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/deploy/api_endpoint.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      912 2024-03-06 00:03:36.000000 autorag-0.1.7/docs/source/deploy/web.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4124 2024-04-12 13:21:50.000000 autorag-0.1.7/docs/source/index.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1891 2024-02-15 09:50:25.000000 autorag-0.1.7/docs/source/install.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6153 2024-04-12 13:21:50.000000 autorag-0.1.7/docs/source/local_model.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.445102 autorag-0.1.7/docs/source/nodes/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.445737 autorag-0.1.7/docs/source/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2703 2024-04-05 14:53:42.000000 autorag-0.1.7/docs/source/nodes/generator/generator.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1306 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/generator/llama_index_llm.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1358 2024-03-14 09:00:38.000000 autorag-0.1.7/docs/source/nodes/generator/vllm.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      172 2024-04-11 14:29:33.000000 autorag-0.1.7/docs/source/nodes/index.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.446169 autorag-0.1.7/docs/source/nodes/passage_augmenter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1591 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/nodes/passage_augmenter/passage_augmenter.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      727 2024-04-27 01:36:13.000000 autorag-0.1.7/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.446653 autorag-0.1.7/docs/source/nodes/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3046 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/nodes/passage_compressor/passage_compressor.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1182 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/nodes/passage_compressor/refine.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1252 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/passage_compressor/tree_summarize.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.447345 autorag-0.1.7/docs/source/nodes/passage_filter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1765 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/nodes/passage_filter/passage_filter.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1127 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/nodes/passage_filter/recency_filter.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1028 2024-04-12 13:21:50.000000 autorag-0.1.7/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1085 2024-04-10 13:46:46.000000 autorag-0.1.7/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.450206 autorag-0.1.7/docs/source/nodes/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1151 2024-03-17 04:13:16.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/cohere.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      521 2024-04-08 12:04:54.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/colbert.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      675 2024-04-11 14:29:33.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      654 2024-04-11 14:29:33.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1232 2024-04-06 14:23:40.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/jina_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      366 2024-02-22 16:33:58.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/koreranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1567 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/monot5.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2372 2024-04-15 08:09:03.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/passage_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-04-05 03:16:26.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/rankgpt.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      645 2024-04-08 08:26:20.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      515 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/tart.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      561 2024-04-12 13:21:50.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/time_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1491 2024-04-28 04:56:07.000000 autorag-0.1.7/docs/source/nodes/passage_reranker/upr.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.450868 autorag-0.1.7/docs/source/nodes/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      585 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/prompt_maker/fstring.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      815 2024-04-09 15:31:49.000000 autorag-0.1.7/docs/source/nodes/prompt_maker/long_context_reorder.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2689 2024-04-09 15:31:49.000000 autorag-0.1.7/docs/source/nodes/prompt_maker/prompt_maker.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.451481 autorag-0.1.7/docs/source/nodes/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1178 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/query_expansion/hyde.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1330 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/query_expansion/query_decompose.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3272 2024-02-22 15:32:30.000000 autorag-0.1.7/docs/source/nodes/query_expansion/query_expansion.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.453053 autorag-0.1.7/docs/source/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      625 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/retrieval/bm25.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-10 06:33:52.000000 autorag-0.1.7/docs/source/nodes/retrieval/hybrid_cc.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2294 2024-04-11 14:29:33.000000 autorag-0.1.7/docs/source/nodes/retrieval/hybrid_dbsf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2053 2024-04-10 06:33:52.000000 autorag-0.1.7/docs/source/nodes/retrieval/hybrid_rrf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2304 2024-04-10 06:33:52.000000 autorag-0.1.7/docs/source/nodes/retrieval/hybrid_rsf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1910 2024-04-11 14:29:33.000000 autorag-0.1.7/docs/source/nodes/retrieval/retrieval.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1223 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/nodes/retrieval/vectordb.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.454033 autorag-0.1.7/docs/source/optimization/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4160 2024-02-15 10:23:20.000000 autorag-0.1.7/docs/source/optimization/custom_config.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3779 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/optimization/folder_structure.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4596 2024-02-07 21:46:19.000000 autorag-0.1.7/docs/source/optimization/optimization.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2580 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/optimization/sample_full_config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.454241 autorag-0.1.7/docs/source/roadmap/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6735 2024-02-07 21:45:07.000000 autorag-0.1.7/docs/source/roadmap/modular_rag.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3032 2024-02-08 11:27:02.000000 autorag-0.1.7/docs/source/structure.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3121 2024-02-18 20:58:37.000000 autorag-0.1.7/docs/source/troubleshooting.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8338 2024-03-29 05:05:10.000000 autorag-0.1.7/docs/source/tutorial.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1529 2024-04-26 05:39:23.000000 autorag-0.1.7/pyproject.toml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-04-27 07:55:59.000000 autorag-0.1.7/requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.455947 autorag-0.1.7/sample_config/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2101 2024-03-14 09:00:38.000000 autorag-0.1.7/sample_config/compact_local.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2420 2024-03-17 04:13:16.000000 autorag-0.1.7/sample_config/compact_openai.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1222 2024-03-17 04:13:16.000000 autorag-0.1.7/sample_config/config_korean.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      976 2024-03-06 00:03:36.000000 autorag-0.1.7/sample_config/extracted_sample.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4769 2024-04-27 01:36:13.000000 autorag-0.1.7/sample_config/full.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      896 2024-03-14 09:00:38.000000 autorag-0.1.7/sample_config/simple_local.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      863 2024-02-08 11:27:02.000000 autorag-0.1.7/sample_config/simple_openai.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.456149 autorag-0.1.7/sample_dataset/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1404 2024-02-05 20:46:09.000000 autorag-0.1.7/sample_dataset/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.456375 autorag-0.1.7/sample_dataset/eli5/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1109 2024-02-05 20:46:09.000000 autorag-0.1.7/sample_dataset/eli5/load_eli5_dataset.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.456541 autorag-0.1.7/sample_dataset/msmarco/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1167 2024-02-05 20:46:09.000000 autorag-0.1.7/sample_dataset/msmarco/load_msmarco_dataset.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.456807 autorag-0.1.7/sample_dataset/triviaqa/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1171 2024-02-07 10:54:45.000000 autorag-0.1.7/sample_dataset/triviaqa/load_triviaqa_dataset.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2024-04-28 11:59:17.515262 autorag-0.1.7/setup.cfg
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.457702 autorag-0.1.7/tests/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.459267 autorag-0.1.7/tests/autorag/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.389040 autorag-0.1.7/tests/autorag/data/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.460016 autorag-0.1.7/tests/autorag/data/corpus/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      620 2024-03-22 04:29:06.000000 autorag-0.1.7/tests/autorag/data/corpus/test_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      646 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/data/corpus/test_langchain.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1317 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/data/corpus/test_llama_index_corpus.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.461164 autorag-0.1.7/tests/autorag/data/qacreation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/data/qacreation/test_base_qacreation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3129 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/data/qacreation/test_llama_index_qacreation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      897 2024-04-12 13:21:50.000000 autorag-0.1.7/tests/autorag/data/qacreation/test_ragas_qa_creation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2097 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/data/qacreation/test_simple.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.462139 autorag-0.1.7/tests/autorag/evaluate/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.462939 autorag-0.1.7/tests/autorag/evaluate/metric/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3551 2024-04-05 14:53:42.000000 autorag-0.1.7/tests/autorag/evaluate/metric/test_generation_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1731 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1634 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/evaluate/metric/test_retrieval_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1263 2024-03-08 17:59:53.000000 autorag-0.1.7/tests/autorag/evaluate/test_evaluate_util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4701 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/evaluate/test_generation_evaluate.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1460 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2007 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/evaluate/test_retrieval_evaluate.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.389819 autorag-0.1.7/tests/autorag/nodes/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.463813 autorag-0.1.7/tests/autorag/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      687 2024-03-08 18:01:40.000000 autorag-0.1.7/tests/autorag/nodes/generator/test_generator_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1372 2024-03-08 17:13:58.000000 autorag-0.1.7/tests/autorag/nodes/generator/test_llama_index_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3263 2024-03-31 05:05:12.000000 autorag-0.1.7/tests/autorag/nodes/generator/test_run_generator_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1004 2024-03-08 18:15:21.000000 autorag-0.1.7/tests/autorag/nodes/generator/test_vllm.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.464417 autorag-0.1.7/tests/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1159 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      751 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2594 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3080 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.465423 autorag-0.1.7/tests/autorag/nodes/passagecompressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-04-15 08:09:03.000000 autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      820 2024-02-22 15:32:30.000000 autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1852 2024-04-15 08:09:03.000000 autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_refine.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5073 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1933 2024-04-15 08:09:03.000000 autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.466823 autorag-0.1.7/tests/autorag/nodes/passagefilter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      710 2024-04-11 14:32:56.000000 autorag-0.1.7/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3615 2024-04-15 08:09:03.000000 autorag-0.1.7/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2999 2024-04-10 13:46:46.000000 autorag-0.1.7/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      981 2024-04-12 13:21:50.000000 autorag-0.1.7/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4380 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagefilter/test_recency_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      860 2024-04-10 13:46:46.000000 autorag-0.1.7/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.470557 autorag-0.1.7/tests/autorag/nodes/passagereranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1160 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3283 2024-04-27 15:42:07.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1994 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_flag_embedding.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2213 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1881 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_jina_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-02-22 16:33:58.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_koreranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1407 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_monot5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-02-22 15:32:30.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_pass_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4580 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4830 2024-02-18 20:58:37.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2230 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_rankgpt.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1604 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1371 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_tart.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1210 2024-04-12 13:21:50.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_time_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      992 2024-04-27 15:25:25.000000 autorag-0.1.7/tests/autorag/nodes/passagereranker/test_upr.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.471377 autorag-0.1.7/tests/autorag/nodes/promptmaker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1373 2024-04-09 15:31:49.000000 autorag-0.1.7/tests/autorag/nodes/promptmaker/test_fstring.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1798 2024-04-09 15:31:49.000000 autorag-0.1.7/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      580 2024-04-09 15:31:49.000000 autorag-0.1.7/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8310 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.472893 autorag-0.1.7/tests/autorag/nodes/queryexpansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      813 2024-02-22 15:48:12.000000 autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_hyde.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      544 2024-02-22 15:32:30.000000 autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-22 15:56:28.000000 autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_query_decompose.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1586 2024-02-15 09:47:24.000000 autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6880 2024-02-22 16:17:25.000000 autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.475144 autorag-0.1.7/tests/autorag/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2906 2024-03-25 03:54:12.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_bm25.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4013 2024-04-11 14:29:33.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1525 2024-04-11 14:29:33.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_cc.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      879 2024-04-11 14:29:33.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2989 2024-04-10 06:33:52.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      780 2024-04-11 14:29:33.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2976 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_retrieval_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11185 2024-03-23 14:00:14.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4692 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/nodes/retrieval/test_vectordb.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.475678 autorag-0.1.7/tests/autorag/schema/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1033 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/schema/test_module_schema.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5515 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/schema/test_node_schema.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3118 2024-03-29 05:05:10.000000 autorag-0.1.7/tests/autorag/test_cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6869 2024-04-10 13:46:46.000000 autorag-0.1.7/tests/autorag/test_deploy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14669 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/autorag/test_evaluator.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2081 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/test_strategy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      306 2024-02-13 20:13:32.000000 autorag-0.1.7/tests/autorag/test_support.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      878 2024-03-06 00:03:36.000000 autorag-0.1.7/tests/autorag/test_web.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.476276 autorag-0.1.7/tests/autorag/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3773 2024-04-27 15:42:07.000000 autorag-0.1.7/tests/autorag/utils/test_preprocess.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9970 2024-04-27 07:48:36.000000 autorag-0.1.7/tests/autorag/utils/test_util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-23 03:44:06.000000 autorag-0.1.7/tests/conftest.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      672 2024-02-18 20:58:37.000000 autorag-0.1.7/tests/delete_tests.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2641 2024-02-22 16:04:39.000000 autorag-0.1.7/tests/mock.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.478582 autorag-0.1.7/tests/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-03-23 03:44:06.000000 autorag-0.1.7/tests/resources/README.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.7/tests/resources/corpus_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.390192 autorag-0.1.7/tests/resources/data_creation/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.479388 autorag-0.1.7/tests/resources/data_creation/raw_dir/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3379 2024-02-08 11:27:05.000000 autorag-0.1.7/tests/resources/data_creation/raw_dir/sample1.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3243 2024-02-08 11:27:05.000000 autorag-0.1.7/tests/resources/data_creation/raw_dir/sample2.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4563 2024-02-08 11:27:05.000000 autorag-0.1.7/tests/resources/data_creation/raw_dir/sample3.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3235 2024-04-12 16:43:24.000000 autorag-0.1.7/tests/resources/full.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.7/tests/resources/qa_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.480070 autorag-0.1.7/tests/resources/qa_gen_prompts/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      198 2024-04-17 01:53:11.000000 autorag-0.1.7/tests/resources/qa_gen_prompts/prompt1.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      186 2024-03-23 03:44:06.000000 autorag-0.1.7/tests/resources/qa_gen_prompts/prompt2.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      202 2024-03-23 03:44:06.000000 autorag-0.1.7/tests/resources/qa_gen_prompts/prompt3.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5910 2024-02-07 10:54:45.000000 autorag-0.1.7/tests/resources/qa_test_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.480642 autorag-0.1.7/tests/resources/result_project/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.481080 autorag-0.1.7/tests/resources/result_project/0/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2297 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.481286 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.484147 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    23516 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    26448 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    33716 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14618 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14683 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    13278 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    54234 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1155 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.485087 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8443 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    41557 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      513 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.485346 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.486803 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.486956 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.488121 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.489822 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.491320 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      845 2024-02-18 14:46:34.000000 autorag-0.1.7/tests/resources/result_project/0/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.491535 autorag-0.1.7/tests/resources/result_project/1/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.491746 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.493290 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.391872 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.493446 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.494530 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.496375 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.496757 autorag-0.1.7/tests/resources/result_project/2/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.392087 autorag-0.1.7/tests/resources/result_project/2/post_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.497053 autorag-0.1.7/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.497572 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.499282 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.499423 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.500005 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.501822 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.503556 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.503776 autorag-0.1.7/tests/resources/result_project/3/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      682 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/3/config.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2307 2024-03-29 05:05:10.000000 autorag-0.1.7/tests/resources/result_project/best.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.504771 autorag-0.1.7/tests/resources/result_project/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/data/corpus.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/data/qa.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.505019 autorag-0.1.7/tests/resources/result_project/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-02-03 19:10:47.000000 autorag-0.1.7/tests/resources/result_project/resources/bm25.pkl
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.505282 autorag-0.1.7/tests/resources/result_project/resources/chroma/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.511817 autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
+-rw-r--r--   0 jeffrey    (501) staff       (20)  6284000 2024-02-18 14:41:41.000000 autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)      100 2024-02-18 14:41:00.000000 autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4000 2024-02-18 14:41:41.000000 autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-18 14:41:00.000000 autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)   352256 2024-02-18 14:41:41.000000 autorag-0.1.7/tests/resources/result_project/resources/chroma/chroma.sqlite3
+-rw-r--r--   0 jeffrey    (501) staff       (20)      338 2024-03-25 11:47:36.000000 autorag-0.1.7/tests/resources/result_project/trial.json
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8439 2024-03-23 03:44:06.000000 autorag-0.1.7/tests/resources/sample_contents_nqa.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.393226 autorag-0.1.7/tests/resources/sample_project/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.512727 autorag-0.1.7/tests/resources/sample_project/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   115302 2024-04-27 01:36:13.000000 autorag-0.1.7/tests/resources/sample_project/data/corpus.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.7/tests/resources/sample_project/data/qa.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-28 11:59:17.513445 autorag-0.1.7/tests/resources/sample_project/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-01-13 07:56:04.000000 autorag-0.1.7/tests/resources/sample_project/resources/bm25.pkl
+-rw-r--r--   0 jeffrey    (501) staff       (20)      893 2024-04-10 13:46:46.000000 autorag-0.1.7/tests/resources/simple.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)    26773 2024-01-13 07:56:04.000000 autorag-0.1.7/tests/resources/test_bm25_retrieval.pkl
```

### Comparing `autorag-0.1.6/.github/workflows/publish.yml` & `autorag-0.1.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/.github/workflows/sphinx.yml` & `autorag-0.1.7/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/.github/workflows/test.yml` & `autorag-0.1.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/.gitignore` & `autorag-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/AutoRAG.egg-info/PKG-INFO` & `autorag-0.1.7/AutoRAG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.6
+Version: 0.1.7
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -244,14 +244,15 @@
 Requires-Dist: cohere>=5.0.0a9
 Requires-Dist: tokenlog>=0.0.2
 Requires-Dist: aiohttp
 Requires-Dist: bert_score
 Requires-Dist: sentence-transformers
 Requires-Dist: FlagEmbedding
 Requires-Dist: ragas
+Requires-Dist: ray
 Requires-Dist: llama-index>=0.10.1
 Requires-Dist: llama-index-core>=0.10.1
 Requires-Dist: llama-index-embeddings-openai
 Requires-Dist: llama-index-embeddings-huggingface
 Requires-Dist: llama-index-llms-openai
 Requires-Dist: llama-index-llms-huggingface
 Requires-Dist: llama-index-llms-openai-like
```

### Comparing `autorag-0.1.6/AutoRAG.egg-info/SOURCES.txt` & `autorag-0.1.7/AutoRAG.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -84,16 +84,14 @@
 autorag/nodes/passagereranker/jina.py
 autorag/nodes/passagereranker/koreranker.py
 autorag/nodes/passagereranker/monot5.py
 autorag/nodes/passagereranker/pass_reranker.py
 autorag/nodes/passagereranker/rankgpt.py
 autorag/nodes/passagereranker/run.py
 autorag/nodes/passagereranker/sentence_transformer.py
-autorag/nodes/passagereranker/temp_new_colbert.py
-autorag/nodes/passagereranker/temp_old_upr.py
 autorag/nodes/passagereranker/time_reranker.py
 autorag/nodes/passagereranker/upr.py
 autorag/nodes/passagereranker/tart/__init__.py
 autorag/nodes/passagereranker/tart/modeling_enc_t5.py
 autorag/nodes/passagereranker/tart/tart.py
 autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
 autorag/nodes/promptmaker/__init__.py
```

### Comparing `autorag-0.1.6/AutoRAG.egg-info/requires.txt` & `autorag-0.1.7/AutoRAG.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 cohere>=5.0.0a9
 tokenlog>=0.0.2
 aiohttp
 bert_score
 sentence-transformers
 FlagEmbedding
 ragas
+ray
 llama-index>=0.10.1
 llama-index-core>=0.10.1
 llama-index-embeddings-openai
 llama-index-embeddings-huggingface
 llama-index-llms-openai
 llama-index-llms-huggingface
 llama-index-llms-openai-like
```

### Comparing `autorag-0.1.6/CODE_OF_CONDUCT.md` & `autorag-0.1.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/CONTRIBUTING.md` & `autorag-0.1.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/LICENSE` & `autorag-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/PKG-INFO` & `autorag-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.6
+Version: 0.1.7
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -244,14 +244,15 @@
 Requires-Dist: cohere>=5.0.0a9
 Requires-Dist: tokenlog>=0.0.2
 Requires-Dist: aiohttp
 Requires-Dist: bert_score
 Requires-Dist: sentence-transformers
 Requires-Dist: FlagEmbedding
 Requires-Dist: ragas
+Requires-Dist: ray
 Requires-Dist: llama-index>=0.10.1
 Requires-Dist: llama-index-core>=0.10.1
 Requires-Dist: llama-index-embeddings-openai
 Requires-Dist: llama-index-embeddings-huggingface
 Requires-Dist: llama-index-llms-openai
 Requires-Dist: llama-index-llms-huggingface
 Requires-Dist: llama-index-llms-openai-like
```

### Comparing `autorag-0.1.6/README.md` & `autorag-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/__init__.py` & `autorag-0.1.7/autorag/__init__.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/cli.py` & `autorag-0.1.7/autorag/cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/data/corpus/langchain.py` & `autorag-0.1.7/autorag/data/corpus/langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/data/corpus/llama_index.py` & `autorag-0.1.7/autorag/data/corpus/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/data/qacreation/base.py` & `autorag-0.1.7/autorag/data/qacreation/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/data/qacreation/llama_index.py` & `autorag-0.1.7/autorag/data/qacreation/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/data/qacreation/llama_index_default_prompt.txt` & `autorag-0.1.7/autorag/data/qacreation/llama_index_default_prompt.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/data/qacreation/ragas.py` & `autorag-0.1.7/autorag/data/qacreation/ragas.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/data/qacreation/simple.py` & `autorag-0.1.7/autorag/data/qacreation/simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/data/utils/util.py` & `autorag-0.1.7/autorag/data/utils/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/deploy.py` & `autorag-0.1.7/autorag/deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/evaluate/generation.py` & `autorag-0.1.7/autorag/evaluate/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt` & `autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt` & `autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt` & `autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt` & `autorag-0.1.7/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/evaluate/metric/generation.py` & `autorag-0.1.7/autorag/evaluate/metric/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/evaluate/metric/retrieval.py` & `autorag-0.1.7/autorag/evaluate/metric/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/evaluate/metric/retrieval_contents.py` & `autorag-0.1.7/autorag/evaluate/metric/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/evaluate/retrieval.py` & `autorag-0.1.7/autorag/evaluate/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/evaluate/retrieval_contents.py` & `autorag-0.1.7/autorag/evaluate/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/evaluate/util.py` & `autorag-0.1.7/autorag/evaluate/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/evaluator.py` & `autorag-0.1.7/autorag/evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/node_line.py` & `autorag-0.1.7/autorag/node_line.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/generator/base.py` & `autorag-0.1.7/autorag/nodes/generator/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/generator/llama_index_llm.py` & `autorag-0.1.7/autorag/nodes/generator/llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/generator/run.py` & `autorag-0.1.7/autorag/nodes/generator/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/generator/vllm.py` & `autorag-0.1.7/autorag/nodes/generator/vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passageaugmenter/base.py` & `autorag-0.1.7/autorag/nodes/passageaugmenter/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passageaugmenter/prev_next_augmenter.py` & `autorag-0.1.7/autorag/nodes/passageaugmenter/prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passageaugmenter/run.py` & `autorag-0.1.7/autorag/nodes/passageaugmenter/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagecompressor/base.py` & `autorag-0.1.7/autorag/nodes/passagecompressor/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagecompressor/refine.py` & `autorag-0.1.7/autorag/nodes/passagecompressor/refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagecompressor/run.py` & `autorag-0.1.7/autorag/nodes/passagecompressor/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagecompressor/tree_summarize.py` & `autorag-0.1.7/autorag/nodes/passagecompressor/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagefilter/base.py` & `autorag-0.1.7/autorag/nodes/passagefilter/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagefilter/percentile_cutoff.py` & `autorag-0.1.7/autorag/nodes/passagefilter/percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagefilter/recency.py` & `autorag-0.1.7/autorag/nodes/passagefilter/recency.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagefilter/run.py` & `autorag-0.1.7/autorag/nodes/passagefilter/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagefilter/threshold_cutoff.py` & `autorag-0.1.7/autorag/nodes/passagefilter/threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/base.py` & `autorag-0.1.7/autorag/nodes/passagereranker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/cohere.py` & `autorag-0.1.7/autorag/nodes/passagereranker/cohere.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/colbert.py` & `autorag-0.1.7/autorag/nodes/passagereranker/colbert.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/flag_embedding.py` & `autorag-0.1.7/autorag/nodes/passagereranker/flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/flag_embedding_llm.py` & `autorag-0.1.7/autorag/nodes/passagereranker/flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/jina.py` & `autorag-0.1.7/autorag/nodes/passagereranker/jina.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/koreranker.py` & `autorag-0.1.7/autorag/nodes/passagereranker/koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/monot5.py` & `autorag-0.1.7/autorag/nodes/passagereranker/monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/pass_reranker.py` & `autorag-0.1.7/autorag/nodes/passagereranker/pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/rankgpt.py` & `autorag-0.1.7/autorag/nodes/passagereranker/rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/run.py` & `autorag-0.1.7/autorag/nodes/passagereranker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/sentence_transformer.py` & `autorag-0.1.7/autorag/nodes/passagereranker/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/tart/modeling_enc_t5.py` & `autorag-0.1.7/autorag/nodes/passagereranker/tart/modeling_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/tart/tart.py` & `autorag-0.1.7/autorag/nodes/passagereranker/tart/tart.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py` & `autorag-0.1.7/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/temp_new_colbert.py` & `autorag-0.1.7/autorag/nodes/retrieval/vectordb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,103 @@
+import asyncio
 from typing import List, Tuple
 
-import numpy as np
+import chromadb
 import pandas as pd
-import torch
-from transformers import AutoModel, AutoTokenizer
+from chromadb.utils.batch_utils import create_batches
+from llama_index.core.embeddings import BaseEmbedding
+from llama_index.embeddings.openai import OpenAIEmbedding
+
+from autorag.nodes.retrieval.base import retrieval_node, evenly_distribute_passages
+from autorag.utils import validate_corpus_dataset
+from autorag.utils.util import process_batch, openai_truncate_by_token
 
-from autorag.nodes.passagereranker.base import passage_reranker_node
-from autorag.utils.util import flatten_apply, sort_by_scores, select_top_k
 
+@retrieval_node
+def vectordb(queries: List[List[str]], top_k: int, collection: chromadb.Collection,
+             embedding_model: BaseEmbedding,
+             batch: int = 128) -> Tuple[List[List[str]], List[List[float]]]:
+    """
+    VectorDB retrieval function.
+    You have to get a chroma collection that is already ingested.
+    You have to get an embedding model that is already used in ingesting.
+
+    :param queries: 2-d list of query strings.
+        Each element of the list is a query strings of each row.
+    :param top_k: The number of passages to be retrieved.
+    :param collection: A chroma collection instance that will be used to retrieve passages.
+    :param embedding_model: An embedding model instance that will be used to embed queries.
+    :param batch: The number of queries to be processed in parallel.
+        This is used to prevent API error at the query embedding.
+        Default is 128.
 
-@passage_reranker_node
-def colbert_reranker(queries: List[str], contents_list: List[List[str]],
-                     scores_list: List[List[float]], ids_list: List[List[str]],
-                     top_k: int, batch: int = 64,
-                     model_name: str = "colbert-ir/colbertv2.0",
-                     ) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
+    :return: The 2-d list contains a list of passage ids that retrieved from vectordb and 2-d list of its scores.
+        It will be a length of queries. And each element has a length of top_k.
     """
-    Rerank a list of contents with Colbert rerank models.
-    You can get more information about a Colbert model at https://huggingface.co/colbert-ir/colbertv2.0.
-    It uses BERT-based model, so recommend using CUDA gpu for faster reranking.
-
-    :param queries: The list of queries to use for reranking
-    :param contents_list: The list of lists of contents to rerank
-    :param scores_list: The list of lists of scores retrieved from the initial ranking
-    :param ids_list: The list of lists of ids retrieved from the initial ranking
-    :param top_k: The number of passages to be retrieved
-    :param batch: The number of queries to be processed in a batch
-        Default is 64.
-    :param model_name: The model name for Colbert rerank.
-        You can choose colbert model for reranking.
-        Default is "colbert-ir/colbertv2.0".
-    :return: Tuple of lists containing the reranked contents, ids, and scores
+    # check if bm25_corpus is valid
+    assert (collection.count() > 0), \
+        "collection must contain at least one document. Please check you ingested collection correctly."
+    # run async vector_db_pure function
+    tasks = [vectordb_pure(input_queries, top_k, collection, embedding_model) for input_queries in queries]
+    loop = asyncio.get_event_loop()
+    results = loop.run_until_complete(process_batch(tasks, batch_size=batch))
+    id_result = list(map(lambda x: x[0], results))
+    score_result = list(map(lambda x: x[1], results))
+    return id_result, score_result
+
+
+async def vectordb_pure(queries: List[str], top_k: int, collection: chromadb.Collection,
+                        embedding_model: BaseEmbedding) -> Tuple[List[str], List[float]]:
     """
-    device = "cuda" if torch.cuda.is_available() else "cpu"
-    model = AutoModel.from_pretrained(model_name).to(device)
-    tokenizer = AutoTokenizer.from_pretrained(model_name)
-
-    # get query and content embeddings
-    query_embedding_list = get_colbert_embedding_batch(queries, model, tokenizer, batch)
-    content_embedding_list = flatten_apply(get_colbert_embedding_batch, contents_list, model=model, tokenizer=tokenizer,
-                                           batch_size=batch)
-
-    del model
-    if torch.cuda.is_available():
-        torch.cuda.empty_cache()
-
-    df = pd.DataFrame({
-        'ids': ids_list,
-        'query_embedding': query_embedding_list,
-        'contents': contents_list,
-        'content_embedding': content_embedding_list,
-    })
-    temp_df = df.explode('content_embedding')
-    temp_df['score'] = temp_df.apply(lambda x: get_colbert_score(x['query_embedding'], x['content_embedding']), axis=1)
-    df['scores'] = temp_df.groupby(level=0, sort=False)['score'].apply(list).tolist()
-    df[['contents', 'ids', 'scores']] = df.apply(sort_by_scores, axis=1, result_type='expand')
-    results = select_top_k(df, ['contents', 'ids', 'scores'], top_k)
-
-    return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
-
-
-def get_colbert_embedding_batch(input_strings: List[str],
-                                model, tokenizer, batch_size: int) -> List[np.array]:
-    encoding = tokenizer(input_strings, return_tensors="pt", padding=True, truncation=True,
-                         max_length=model.config.max_position_embeddings)
-    input_batches = slice_tokenizer_result(encoding, batch_size)
-    result_embedding = []
-    for encoding in input_batches:
-        result_embedding.append(model(**encoding).last_hidden_state)
-    total_tensor = torch.cat(result_embedding, dim=0)  # shape [batch_size, token_length, embedding_dim]
-    tensor_results = list(total_tensor.chunk(total_tensor.size()[0]))
-    if torch.cuda.is_available():
-        return list(map(lambda x: x.detach().cpu().numpy(), tensor_results))
-    else:
-        return list(map(lambda x: x.detach().numpy(), tensor_results))
-
-
-def slice_tokenizer_result(tokenizer_output, batch_size):
-    input_ids_batches = slice_tensor(tokenizer_output["input_ids"], batch_size)
-    attention_mask_batches = slice_tensor(tokenizer_output["attention_mask"], batch_size)
-    token_type_ids_batches = slice_tensor(tokenizer_output.get("token_type_ids", None), batch_size)
-    return [{"input_ids": input_ids, "attention_mask": attention_mask, "token_type_ids": token_type_ids}
-            for input_ids, attention_mask, token_type_ids in
-            zip(input_ids_batches, attention_mask_batches, token_type_ids_batches)]
-
-
-def slice_tensor(input_tensor, batch_size):
-    # Calculate the number of full batches
-    num_full_batches = input_tensor.size(0) // batch_size
-
-    # Slice the tensor into batches
-    tensor_list = [input_tensor[i * batch_size:(i + 1) * batch_size] for i in range(num_full_batches)]
-
-    # Handle the last batch if it's smaller than batch_size
-    remainder = input_tensor.size(0) % batch_size
-    if remainder:
-        tensor_list.append(input_tensor[-remainder:])
-    device = "cuda" if torch.cuda.is_available() else "cpu"
-    tensor_list = list(map(lambda x: x.to(device), tensor_list))
-    return tensor_list
-
-
-def get_colbert_score(query_embedding: np.array, content_embedding: np.array) -> float:
-    query_tensor = torch.tensor(query_embedding)
-    content_tensor = torch.tensor(content_embedding)
-    sim_matrix = torch.nn.functional.cosine_similarity(
-        query_tensor.unsqueeze(2), content_tensor.unsqueeze(1), dim=-1
-    )
-    max_sim_scores, _ = torch.max(sim_matrix, dim=2)
-    return float(torch.mean(max_sim_scores, dim=1))
+    Async VectorDB retrieval function.
+    Its usage is for async retrieval of vector_db row by row.
+
+    :param queries: A list of query strings.
+    :param top_k: The number of passages to be retrieved.
+    :param collection: A chroma collection instance that will be used to retrieve passages.
+    :param embedding_model: An embedding model instance that will be used to embed queries.
+
+    :return: The tuple contains a list of passage ids that retrieved from vectordb and a list of its scores.
+    """
+    # embed query
+    embedded_queries = list(map(embedding_model.get_query_embedding, queries))
+
+    id_result, score_result = [], []
+    for embedded_query in embedded_queries:
+        result = collection.query(query_embeddings=embedded_query, n_results=top_k)
+        id_result.extend(result['ids'])
+        score_result.extend(result['distances'])
+
+    # Distribute passages evenly
+    id_result, score_result = evenly_distribute_passages(id_result, score_result, top_k)
+    # sort id_result and score_result by score
+    result = [(_id, score) for score, _id in
+              sorted(zip(score_result, id_result), key=lambda pair: pair[0], reverse=True)]
+    id_result, score_result = zip(*result)
+    return list(id_result), list(score_result)
+
+
+def vectordb_ingest(collection: chromadb.Collection, corpus_data: pd.DataFrame, embedding_model: BaseEmbedding,
+                    batch: int = 128):
+    embedding_model.embed_batch_size = batch
+    validate_corpus_dataset(corpus_data)
+    ids = corpus_data['doc_id'].tolist()
+
+    # Query the collection to check if IDs already exist
+    existing_ids = set(collection.get(ids=ids)['ids'])  # Assuming 'ids' is the key in the response
+    new_passage = corpus_data[~corpus_data['doc_id'].isin(existing_ids)]
+
+    if not new_passage.empty:
+        new_contents = new_passage['contents'].tolist()
+
+        # truncate by token if embedding_model is OpenAIEmbedding
+        if isinstance(embedding_model, OpenAIEmbedding):
+            openai_embedding_limit = 8191
+            new_contents = openai_truncate_by_token(new_contents, openai_embedding_limit, embedding_model.model_name)
+
+        new_ids = new_passage['doc_id'].tolist()
+        embedded_contents = embedding_model.get_text_embedding_batch(new_contents, show_progress=True)
+        input_batches = create_batches(api=collection._client, ids=new_ids, embeddings=embedded_contents)
+        for batch in input_batches:
+            ids = batch[0]
+            embed_content = batch[1]
+            collection.add(ids=ids, embeddings=embed_content)
```

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/temp_old_upr.py` & `autorag-0.1.7/autorag/nodes/passagereranker/upr.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,154 +1,112 @@
-import asyncio
-from typing import List, Tuple
-
+import logging
+import os
+from typing import List, Tuple, Dict
+
+import numpy as np
+import pandas as pd
+import ray
 import torch
 from transformers import T5Tokenizer, T5ForConditionalGeneration
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
+from autorag.utils.util import select_top_k, sort_by_scores
+
+logger = logging.getLogger("AutoRAG")
 
 
 @passage_reranker_node
 def upr(queries: List[str], contents_list: List[List[str]],
         scores_list: List[List[float]], ids_list: List[List[str]],
-        top_k: int, shard_size: int = 16, use_bf16: bool = False,
+        top_k: int, use_bf16: bool = False,
         prefix_prompt: str = "Passage: ",
-        suffix_prompt: str = "Please write a question based on this passage.") \
+        suffix_prompt: str = "Please write a question based on this passage.",
+        num_gpus: int = 1) \
         -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
     """
     Rerank a list of contents based on their relevance to a query using UPR.
     UPR is a reranker based on UPR (https://github.com/DevSinghSachan/unsupervised-passage-reranking).
     The language model will make a question based on the passage and rerank the passages by the likelihood of the question.
     The default model is t5-large.
 
     :param queries: The list of queries to use for reranking
     :param contents_list: The list of lists of contents to rerank
     :param scores_list: The list of lists of scores retrieved from the initial ranking
     :param ids_list: The list of lists of ids retrieved from the initial ranking
     :param top_k: The number of passages to be retrieved
-    :param shard_size: The shard size for the model.
-        The larger the shard size, the faster the reranking speed.
-        But it will consume more memory and compute power.
-        Default is 16.
     :param use_bf16: Whether to use bfloat16 for the model. Default is False.
     :param prefix_prompt: The prefix prompt for the language model that generates question for reranking.
         Default is "Passage: ".
         The prefix prompt serves as the initial context or instruction for the language model.
         It sets the stage for what is expected in the output
     :param suffix_prompt: The suffix prompt for the language model that generates question for reranking.
         Default is "Please write a question based on this passage.".
         The suffix prompt provides a cue or a closing instruction to the language model,
             signaling how to conclude the generated text or what format to follow at the end.
+    :param num_gpus: The number of GPUs that you want to use. Default is 1.
+        Set to 1 if you use a CPU or a single GPU.
     :return: tuple of lists containing the reranked contents, ids, and scores
     """
-    # Load the tokenizer and model
-    model_name = "t5-large"
-    tokenizer = T5Tokenizer.from_pretrained(model_name)
-    model = T5ForConditionalGeneration.from_pretrained(model_name,
-                                                       torch_dtype=torch.bfloat16 if use_bf16 else torch.float32)
-    # Determine the device to run the model on (GPU if available, otherwise CPU)
-    device = ("cuda" if torch.cuda.is_available() else "cpu")
-    # Run async upr_rerank_pure function
-    tasks = [upr_pure(query, contents, scores,
-                      ids, top_k, model, device, tokenizer,
-                      shard_size, prefix_prompt, suffix_prompt)
-             for query, contents, scores, ids in
-             zip(queries, contents_list, scores_list, ids_list)]
-    loop = asyncio.get_event_loop()
-    results = loop.run_until_complete(asyncio.gather(*tasks))
-
-    content_result = list(map(lambda x: x[0], results))
-    id_result = list(map(lambda x: x[1], results))
-    score_result = list(map(lambda x: x[2], results))
+    df = pd.DataFrame({
+        'query': queries,
+        'contents': contents_list,
+        'ids': ids_list,
+    })
+    ds = ray.data.from_pandas(df)
 
-    del model
-    del tokenizer
     if torch.cuda.is_available():
-        torch.cuda.empty_cache()
-
-    return content_result, id_result, score_result
-
-
-async def upr_pure(query: str, contents: List[str], scores: List[float],
-                   ids: List[str], top_k: int, model, device, tokenizer,
-                   shard_size: int, prefix_prompt: str, suffix_prompt: str) \
-        -> Tuple[List[str], List[str], List[float]]:
-    """
-    Rerank a list of contents based on their relevance to a query using UPR.
-
-    :param query: The query to use for reranking
-    :param contents: The list of contents to rerank
-    :param scores: The list of scores retrieved from the initial ranking
-    :param ids: The list of ids retrieved from the initial ranking
-    :param top_k: The number of passages to be retrieved
-    :param model: The UPR model to use for reranking
-    :param device: The device to run the model on (GPU if available, otherwise CPU)
-    :param tokenizer: The tokenizer to use for the model
-    :param shard_size: The shard size for the model.
-    :param prefix_prompt: The prefix prompt for the language model that generates question for reranking.
-    :param suffix_prompt: The suffix prompt for the language model that generates question for reranking.
-    :return: tuple of lists containing the reranked contents, ids, and scores
-    """
-    indexes, scores = calculate_likelihood(query, contents, prefix_prompt, suffix_prompt,
-                                           tokenizer, device, model, shard_size)
-    reranked_contents, reranked_ids = zip(*[(contents[idx], ids[idx]) for idx in indexes])
-
-    # crop with top_k
-    if len(reranked_contents) < top_k:
-        top_k = len(reranked_contents)
-    reranked_contents, reranked_ids, scores = reranked_contents[:top_k], reranked_ids[:top_k], scores[:top_k]
-
-    return list(reranked_contents), list(reranked_ids), list(scores)
-
-
-def calculate_likelihood(query: str, contents: List[str],
-                         prefix_prompt: str, suffix_prompt: str,
-                         tokenizer, device, model, shard_size: int)\
-        -> tuple[List[int], List[float]]:
-    # create prompts
-    prompts = [f"{prefix_prompt} {content} {suffix_prompt}" for content in contents]
-
-    # tokenize contexts and instruction prompts
-    context_tokens = tokenizer(prompts,
-                               padding='longest',
-                               max_length=512,
-                               pad_to_multiple_of=8,
-                               truncation=True,
-                               return_tensors='pt')
-    context_tensor, context_attention_mask = context_tokens.input_ids, context_tokens.attention_mask
-    if device == 'cuda':
-        context_tensor, context_attention_mask = context_tensor.cuda(), context_attention_mask.cuda()
-
-    # tokenize question
-    question_tokens = tokenizer([query],
-                                max_length=128,
-                                truncation=True,
-                                return_tensors='pt')
-    question_tensor = question_tokens.input_ids
-    if device == 'cuda':
-        question_tensor = question_tensor.cuda()
-    question_tensor = torch.repeat_interleave(question_tensor, len(contents), dim=0)
-
-    if device == 'cuda':
-        model = model.to(device)
-
-    sharded_nll_list = []
-
-    # calculate log likelihood
-    for i in range(0, len(context_tensor), shard_size):
-        encoder_tensor_view = context_tensor[i: i + shard_size]
-        attention_mask_view = context_attention_mask[i: i + shard_size]
-        decoder_tensor_view = question_tensor[i: i + shard_size]
-        with torch.no_grad():
-            logits = model(input_ids=encoder_tensor_view,
-                           attention_mask=attention_mask_view,
-                           labels=decoder_tensor_view).logits
-
+        score_batch = ds.map_batches(UPRScorer(suffix_prompt=suffix_prompt,
+                                               prefix_prompt=prefix_prompt, use_bf16=use_bf16), batch_size=1,
+                                     concurrency=num_gpus, num_gpus=1)
+    else:
+        score_batch = ds.map_batches(UPRScorer(suffix_prompt=suffix_prompt,
+                                               prefix_prompt=prefix_prompt, use_bf16=use_bf16),
+                                     batch_size=1,
+                                     concurrency=min(len(df), os.cpu_count()), num_cpus=os.cpu_count())
+    scores = score_batch.to_pandas()['output'].tolist()  # converted to a flatten list of scores
+
+    explode_df = df.explode('contents')
+    explode_df['scores'] = scores
+    df['scores'] = explode_df.groupby(level=0, sort=False)['scores'].apply(list).tolist()
+    df[['contents', 'ids', 'scores']] = df.apply(lambda x: sort_by_scores(x, reverse=False), axis=1,
+                                                 result_type='expand')
+    results = select_top_k(df, ['contents', 'ids', 'scores'], top_k)
+    return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
+
+
+class UPRScorer:
+    def __init__(self, suffix_prompt: str, prefix_prompt: str,
+                 use_bf16: bool = False):
+        model_name = "t5-large"
+        self.device = "cuda" if torch.cuda.is_available() else "cpu"
+        self.tokenizer = T5Tokenizer.from_pretrained(model_name)
+        self.model = T5ForConditionalGeneration.from_pretrained(model_name,
+                                                                torch_dtype=torch.bfloat16
+                                                                if use_bf16 else torch.float32).to(self.device)
+        self.suffix_prompt = suffix_prompt
+        self.prefix_prompt = prefix_prompt
+
+    def __call__(self, batch: Dict[str, np.ndarray]):
+        query_token = self.tokenizer(batch['query'][0], max_length=128, truncation=True, return_tensors='pt')
+        contents = batch['contents'][0]
+        prompts = list(map(lambda content: f"{self.prefix_prompt} {content} {self.suffix_prompt}", contents))
+        prompt_token_outputs = self.tokenizer(prompts, padding='longest',
+                                              max_length=512,
+                                              pad_to_multiple_of=8,
+                                              truncation=True,
+                                              return_tensors='pt')
+
+        query_input_ids = torch.repeat_interleave(query_token['input_ids'], len(contents),
+                                                  dim=0).to(self.device)
+
+        logits = self.model(input_ids=prompt_token_outputs['input_ids'].to(self.device),
+                            attention_mask=prompt_token_outputs['attention_mask'].to(self.device),
+                            labels=query_input_ids).logits
         log_softmax = torch.nn.functional.log_softmax(logits, dim=-1)
-        nll = -log_softmax.gather(2, decoder_tensor_view.unsqueeze(2)).squeeze(2)
-
+        nll = -log_softmax.gather(2, query_input_ids.unsqueeze(2)).squeeze(2)
         avg_nll = torch.sum(nll, dim=1)
-        sharded_nll_list.append(avg_nll)
-
-    topk_scores, indexes = torch.topk(-torch.cat(sharded_nll_list), k=len(context_tensor))
+        return {"output": avg_nll.tolist()}
 
-    return indexes.tolist(), topk_scores.tolist()
+    def __del__(self):
+        del self.model
+        if torch.cuda.is_available():
+            torch.cuda.empty_cache()
```

### Comparing `autorag-0.1.6/autorag/nodes/passagereranker/time_reranker.py` & `autorag-0.1.7/autorag/nodes/passagereranker/time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/promptmaker/base.py` & `autorag-0.1.7/autorag/nodes/promptmaker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/promptmaker/fstring.py` & `autorag-0.1.7/autorag/nodes/promptmaker/fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/promptmaker/long_context_reorder.py` & `autorag-0.1.7/autorag/nodes/promptmaker/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/promptmaker/run.py` & `autorag-0.1.7/autorag/nodes/promptmaker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/queryexpansion/base.py` & `autorag-0.1.7/autorag/nodes/queryexpansion/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/queryexpansion/hyde.py` & `autorag-0.1.7/autorag/nodes/queryexpansion/hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/queryexpansion/query_decompose.py` & `autorag-0.1.7/autorag/nodes/queryexpansion/query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/queryexpansion/run.py` & `autorag-0.1.7/autorag/nodes/queryexpansion/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/retrieval/base.py` & `autorag-0.1.7/autorag/nodes/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/retrieval/bm25.py` & `autorag-0.1.7/autorag/nodes/retrieval/bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/retrieval/hybrid_cc.py` & `autorag-0.1.7/autorag/nodes/retrieval/hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/retrieval/hybrid_dbsf.py` & `autorag-0.1.7/autorag/nodes/retrieval/hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/retrieval/hybrid_rrf.py` & `autorag-0.1.7/autorag/nodes/retrieval/hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/retrieval/hybrid_rsf.py` & `autorag-0.1.7/autorag/nodes/retrieval/hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/nodes/retrieval/run.py` & `autorag-0.1.7/autorag/nodes/retrieval/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/schema/module.py` & `autorag-0.1.7/autorag/schema/module.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/schema/node.py` & `autorag-0.1.7/autorag/schema/node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/strategy.py` & `autorag-0.1.7/autorag/strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/support.py` & `autorag-0.1.7/autorag/support.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/utils/preprocess.py` & `autorag-0.1.7/autorag/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/utils/util.py` & `autorag-0.1.7/autorag/utils/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/autorag/web.py` & `autorag-0.1.7/autorag/web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/Makefile` & `autorag-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/make.bat` & `autorag-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/data_creation.png` & `autorag-0.1.7/docs/source/_static/data_creation.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/data_folder.png` & `autorag-0.1.7/docs/source/_static/data_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/node_folder.png` & `autorag-0.1.7/docs/source/_static/node_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/node_line_folder.png` & `autorag-0.1.7/docs/source/_static/node_line_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/node_line_summary.png` & `autorag-0.1.7/docs/source/_static/node_line_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/node_lines.png` & `autorag-0.1.7/docs/source/_static/node_lines.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/node_summary.png` & `autorag-0.1.7/docs/source/_static/node_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/project_folder_example.png` & `autorag-0.1.7/docs/source/_static/project_folder_example.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/project_folders.png` & `autorag-0.1.7/docs/source/_static/project_folders.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/resources_folder.png` & `autorag-0.1.7/docs/source/_static/resources_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/roadmap/RAG_paradigms.png` & `autorag-0.1.7/docs/source/_static/roadmap/RAG_paradigms.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/roadmap/advanced_RAG.png` & `autorag-0.1.7/docs/source/_static/roadmap/advanced_RAG.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/roadmap/cycle.png` & `autorag-0.1.7/docs/source/_static/roadmap/cycle.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/roadmap/merger.png` & `autorag-0.1.7/docs/source/_static/roadmap/merger.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/roadmap/node_line_modular.png` & `autorag-0.1.7/docs/source/_static/roadmap/node_line_modular.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/roadmap/policy.png` & `autorag-0.1.7/docs/source/_static/roadmap/policy.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/samsung_sundae.jpeg` & `autorag-0.1.7/docs/source/_static/samsung_sundae.jpeg`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/trial_folder.png` & `autorag-0.1.7/docs/source/_static/trial_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/trial_json.png` & `autorag-0.1.7/docs/source/_static/trial_json.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/trial_summary.png` & `autorag-0.1.7/docs/source/_static/trial_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/_static/web_interface.png` & `autorag-0.1.7/docs/source/_static/web_interface.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.data.corpus.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.data.corpus.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.data.qacreation.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.data.qacreation.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.evaluate.metric.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.evaluate.metric.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.evaluate.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.evaluate.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.nodes.generator.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.nodes.generator.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.nodes.passageaugmenter.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.nodes.passageaugmenter.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagecompressor.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagecompressor.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagefilter.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagefilter.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagereranker.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagereranker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.nodes.promptmaker.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.nodes.promptmaker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.nodes.queryexpansion.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.nodes.queryexpansion.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.nodes.retrieval.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.nodes.retrieval.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/api_spec/autorag.rst` & `autorag-0.1.7/docs/source/api_spec/autorag.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/conf.py` & `autorag-0.1.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/data_creation/data_format.md` & `autorag-0.1.7/docs/source/data_creation/data_format.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/data_creation/ragas.md` & `autorag-0.1.7/docs/source/data_creation/ragas.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/data_creation/tutorial.md` & `autorag-0.1.7/docs/source/data_creation/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/deploy/api_endpoint.md` & `autorag-0.1.7/docs/source/deploy/api_endpoint.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/deploy/web.md` & `autorag-0.1.7/docs/source/deploy/web.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/index.rst` & `autorag-0.1.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/install.md` & `autorag-0.1.7/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/local_model.md` & `autorag-0.1.7/docs/source/local_model.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/generator/generator.md` & `autorag-0.1.7/docs/source/nodes/generator/generator.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/generator/llama_index_llm.md` & `autorag-0.1.7/docs/source/nodes/generator/llama_index_llm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/generator/vllm.md` & `autorag-0.1.7/docs/source/nodes/generator/vllm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_augmenter/passage_augmenter.md` & `autorag-0.1.7/docs/source/nodes/passage_augmenter/passage_augmenter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_augmenter/prev_next_augmenter.md` & `autorag-0.1.7/docs/source/nodes/passage_augmenter/prev_next_augmenter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_compressor/passage_compressor.md` & `autorag-0.1.7/docs/source/nodes/passage_compressor/passage_compressor.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_compressor/refine.md` & `autorag-0.1.7/docs/source/nodes/passage_compressor/refine.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_compressor/tree_summarize.md` & `autorag-0.1.7/docs/source/nodes/passage_compressor/tree_summarize.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_filter/passage_filter.md` & `autorag-0.1.7/docs/source/nodes/passage_filter/passage_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_filter/recency_filter.md` & `autorag-0.1.7/docs/source/nodes/passage_filter/recency_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md` & `autorag-0.1.7/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md` & `autorag-0.1.7/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_reranker/cohere.md` & `autorag-0.1.7/docs/source/nodes/passage_reranker/cohere.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_reranker/colbert.md` & `autorag-0.1.7/docs/source/nodes/passage_reranker/colbert.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md` & `autorag-0.1.7/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_reranker/flag_embedding_reranker.md` & `autorag-0.1.7/docs/source/nodes/passage_reranker/flag_embedding_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_reranker/jina_reranker.md` & `autorag-0.1.7/docs/source/nodes/passage_reranker/jina_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_reranker/monot5.md` & `autorag-0.1.7/docs/source/nodes/passage_reranker/monot5.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_reranker/passage_reranker.md` & `autorag-0.1.7/docs/source/nodes/passage_reranker/passage_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_reranker/rankgpt.md` & `autorag-0.1.7/docs/source/nodes/passage_reranker/rankgpt.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md` & `autorag-0.1.7/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_reranker/tart.md` & `autorag-0.1.7/docs/source/nodes/passage_reranker/tart.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_reranker/time_reranker.md` & `autorag-0.1.7/docs/source/nodes/passage_reranker/time_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/passage_reranker/upr.md` & `autorag-0.1.7/docs/source/nodes/passage_reranker/upr.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # UPR
 
 The `UPR` module is a reranker based on paper called "[Improving Passage Retrieval with Zero-shot Question Generation](https://arxiv.org/abs/2204.07496)". It uses a language model to generate a question based on the passage and reranks the passages by the likelihood of the question. It can enhance accuracy because it calculates likelihood original passages and related passages (generated) with user's question. 
 
 ## **Module Parameters**
 
-Configure the UPR module with parameters like 
-- (Optional)`shard_size` (integer): 
-  - The larger the shard size, the faster the reranking speed.
-          But it will consume more memory and compute power.
-  - Default is `16`.
+Configure the UPR module with parameters like
 - (Optional) `use_bf16` (boolean):
   - Whether to use bfloat16 for the model. 
   - Default is `False`.
+- (Optional) `num_gpus` (int):
+    - Number of GPUs in your machine.
+    - Default is 1.
+    - If you use CPU, just keep this parameter as 1.
 - (Optional) `prefix_prompt` (strings):
   - The prefix prompt serves as the initial context or instruction for the language model.
         It sets the stage for what is expected in the output 
   - Default is `Passage: `
 - (Optional) `suffix_prompt` (strings):
   - The suffix prompt provides a cue or a closing instruction to the language model,
               signaling how to conclude the generated text or what format to follow at the end.
@@ -23,10 +23,12 @@
 
 for customizing the reranking behavior.
 
 ## **Example config.yaml**
 ```yaml
 modules:
   - module_type: upr
-    shard_size: 8
     use_bf16: False
+    num_gpus: 1
+    prefix_prompt: "Passage: "
+    suffix_prompt: "Please write a question based on this passage."
 ```
```

### Comparing `autorag-0.1.6/docs/source/nodes/prompt_maker/fstring.md` & `autorag-0.1.7/docs/source/nodes/prompt_maker/fstring.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/prompt_maker/long_context_reorder.md` & `autorag-0.1.7/docs/source/nodes/prompt_maker/long_context_reorder.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/prompt_maker/prompt_maker.md` & `autorag-0.1.7/docs/source/nodes/prompt_maker/prompt_maker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/query_expansion/hyde.md` & `autorag-0.1.7/docs/source/nodes/query_expansion/hyde.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/query_expansion/query_decompose.md` & `autorag-0.1.7/docs/source/nodes/query_expansion/query_decompose.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/query_expansion/query_expansion.md` & `autorag-0.1.7/docs/source/nodes/query_expansion/query_expansion.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/retrieval/bm25.md` & `autorag-0.1.7/docs/source/nodes/retrieval/bm25.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/retrieval/hybrid_cc.md` & `autorag-0.1.7/docs/source/nodes/retrieval/hybrid_cc.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/retrieval/hybrid_dbsf.md` & `autorag-0.1.7/docs/source/nodes/retrieval/hybrid_dbsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/retrieval/hybrid_rrf.md` & `autorag-0.1.7/docs/source/nodes/retrieval/hybrid_rrf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/retrieval/hybrid_rsf.md` & `autorag-0.1.7/docs/source/nodes/retrieval/hybrid_rsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/retrieval/retrieval.md` & `autorag-0.1.7/docs/source/nodes/retrieval/retrieval.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/nodes/retrieval/vectordb.md` & `autorag-0.1.7/docs/source/nodes/retrieval/vectordb.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/optimization/custom_config.md` & `autorag-0.1.7/docs/source/optimization/custom_config.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/optimization/folder_structure.md` & `autorag-0.1.7/docs/source/optimization/folder_structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/optimization/optimization.md` & `autorag-0.1.7/docs/source/optimization/optimization.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/optimization/sample_full_config.yaml` & `autorag-0.1.7/docs/source/optimization/sample_full_config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/roadmap/modular_rag.md` & `autorag-0.1.7/docs/source/roadmap/modular_rag.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/structure.md` & `autorag-0.1.7/docs/source/structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/troubleshooting.md` & `autorag-0.1.7/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/docs/source/tutorial.md` & `autorag-0.1.7/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/pyproject.toml` & `autorag-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/requirements.txt` & `autorag-0.1.7/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 cohere>=5.0.0a9 # for cohere services
 tokenlog>=0.0.2 # for token logging
 aiohttp # for async http requests
 bert_score # for bert score
 sentence-transformers # for sentence transformer reranker
 FlagEmbedding # for flag embedding reranker
 ragas # evaluation data generation & evaluation
+ray # for parallel processing
 
 ### LlamaIndex ###
 llama-index>=0.10.1
 llama-index-core>=0.10.1
 # Embeddings
 llama-index-embeddings-openai
 llama-index-embeddings-huggingface
```

### Comparing `autorag-0.1.6/sample_config/compact_local.yaml` & `autorag-0.1.7/sample_config/compact_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/sample_config/compact_openai.yaml` & `autorag-0.1.7/sample_config/compact_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/sample_config/config_korean.yaml` & `autorag-0.1.7/sample_config/config_korean.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/sample_config/extracted_sample.yaml` & `autorag-0.1.7/sample_config/extracted_sample.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/sample_config/full.yaml` & `autorag-0.1.7/sample_config/full.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/sample_config/simple_local.yaml` & `autorag-0.1.7/sample_config/simple_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/sample_config/simple_openai.yaml` & `autorag-0.1.7/sample_config/simple_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/sample_dataset/README.md` & `autorag-0.1.7/sample_dataset/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/sample_dataset/eli5/load_eli5_dataset.py` & `autorag-0.1.7/sample_dataset/eli5/load_eli5_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/sample_dataset/msmarco/load_msmarco_dataset.py` & `autorag-0.1.7/sample_dataset/msmarco/load_msmarco_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/sample_dataset/triviaqa/load_triviaqa_dataset.py` & `autorag-0.1.7/sample_dataset/triviaqa/load_triviaqa_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/data/corpus/test_base.py` & `autorag-0.1.7/tests/autorag/data/corpus/test_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/data/corpus/test_langchain.py` & `autorag-0.1.7/tests/autorag/data/corpus/test_langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/data/corpus/test_llama_index_corpus.py` & `autorag-0.1.7/tests/autorag/data/corpus/test_llama_index_corpus.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/data/qacreation/test_base_qacreation.py` & `autorag-0.1.7/tests/autorag/data/qacreation/test_base_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/data/qacreation/test_llama_index_qacreation.py` & `autorag-0.1.7/tests/autorag/data/qacreation/test_llama_index_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/data/qacreation/test_ragas_qa_creation.py` & `autorag-0.1.7/tests/autorag/data/qacreation/test_ragas_qa_creation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/data/qacreation/test_simple.py` & `autorag-0.1.7/tests/autorag/data/qacreation/test_simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/evaluate/metric/test_generation_metric.py` & `autorag-0.1.7/tests/autorag/evaluate/metric/test_generation_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py` & `autorag-0.1.7/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/evaluate/metric/test_retrieval_metric.py` & `autorag-0.1.7/tests/autorag/evaluate/metric/test_retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/evaluate/test_evaluate_util.py` & `autorag-0.1.7/tests/autorag/evaluate/test_evaluate_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/evaluate/test_generation_evaluate.py` & `autorag-0.1.7/tests/autorag/evaluate/test_generation_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/evaluate/test_retrieval_contents_evaluate.py` & `autorag-0.1.7/tests/autorag/evaluate/test_retrieval_contents_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/evaluate/test_retrieval_evaluate.py` & `autorag-0.1.7/tests/autorag/evaluate/test_retrieval_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/generator/test_generator_base.py` & `autorag-0.1.7/tests/autorag/nodes/generator/test_generator_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/generator/test_llama_index_llm.py` & `autorag-0.1.7/tests/autorag/nodes/generator/test_llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/generator/test_run_generator_node.py` & `autorag-0.1.7/tests/autorag/nodes/generator/test_run_generator_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/generator/test_vllm.py` & `autorag-0.1.7/tests/autorag/nodes/generator/test_vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py` & `autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py` & `autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py` & `autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py` & `autorag-0.1.7/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py` & `autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_pass_compressor.py` & `autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_pass_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_refine.py` & `autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py` & `autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagecompressor/test_tree_summarize.py` & `autorag-0.1.7/tests/autorag/nodes/passagecompressor/test_tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py` & `autorag-0.1.7/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagefilter/test_passage_filter_base.py` & `autorag-0.1.7/tests/autorag/nodes/passagefilter/test_passage_filter_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagefilter/test_passage_filter_run.py` & `autorag-0.1.7/tests/autorag/nodes/passagefilter/test_passage_filter_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py` & `autorag-0.1.7/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagefilter/test_recency_filter.py` & `autorag-0.1.7/tests/autorag/nodes/passagefilter/test_recency_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py` & `autorag-0.1.7/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_cohere_reranker.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_cohere_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_colbert_reranker.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_flag_embedding.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_jina_reranker.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_jina_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_koreranker.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_monot5.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_pass_reranker.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,44 +37,48 @@
 previous_result['retrieval_recall'] = recall_example
 
 ko_previous_result = previous_result.copy(deep=True)
 ko_previous_result['query'] = ko_queries_example
 ko_previous_result['retrieved_contents'] = ko_contents_example
 
 
-def base_reranker_test(contents, ids, scores, top_k, use_ko=False):
+def base_reranker_test(contents, ids, scores, top_k, use_ko=False, descending=True):
     assert len(contents) == len(ids) == len(scores) == 2
     assert len(contents[0]) == len(ids[0]) == len(scores[0]) == top_k
     for content_list, id_list, score_list in zip(contents, ids, scores):
         assert isinstance(content_list, list)
         assert isinstance(id_list, list)
         assert isinstance(score_list, list)
         for content, _id, score in zip(content_list, id_list, score_list):
             assert isinstance(content, str)
             assert isinstance(_id, str)
             assert isinstance(score, float)
-        for i in range(1, len(score_list)):
-            assert score_list[i - 1] >= score_list[i]
+        if descending is True:
+            for i in range(1, len(score_list)):
+                assert score_list[i - 1] >= score_list[i]
+        else:
+            for i in range(1, len(score_list)):
+                assert score_list[i - 1] <= score_list[i]
     if use_ko is True:
         assert contents[0][0] == "프랑스의 수도는 파리 입니다."
         assert ids[0][0] in ids_example[0][1]
         assert contents[1][0] == "뉴진스의 멤버는 5명 입니다."
         assert ids[1][0] in ids_example[1][2]
     else:
         assert contents[0][0] == "Paris is the capital of France."
         assert ids[0][0] in ids_example[0][1]
         assert contents[1][0] == "Newjeans has 5 members."
         assert ids[1][0] in ids_example[1][2]
 
 
-def base_reranker_node_test(result_df, top_k, use_ko=False):
+def base_reranker_node_test(result_df, top_k, use_ko=False, descending=True):
     contents = result_df["retrieved_contents"].tolist()
     ids = result_df["retrieved_ids"].tolist()
     scores = result_df["retrieve_scores"].tolist()
-    base_reranker_test(contents, ids, scores, top_k, use_ko)
+    base_reranker_test(contents, ids, scores, top_k, use_ko, descending=descending)
 
 
 @pytest.fixture
 def project_dir_with_corpus():
     with tempfile.TemporaryDirectory() as temp_dir:
         data_dir = os.path.join(temp_dir, "data")
         os.makedirs(data_dir, exist_ok=True)
```

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_rankgpt.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_sentence_transformer.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_tart.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_tart.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_time_reranker.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/passagereranker/test_upr.py` & `autorag-0.1.7/tests/autorag/nodes/passagereranker/test_upr.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 @pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
 def test_upr():
     top_k = 1
     original_upr = upr.__wrapped__
     contents_result, id_result, score_result \
         = original_upr(queries_example, contents_example, scores_example, ids_example, top_k)
-    base_reranker_test(contents_result, id_result, score_result, top_k)
+    base_reranker_test(contents_result, id_result, score_result, top_k, descending=False)
 
 
 @pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
 def test_upr_node():
-    top_k = 1
+    top_k = 3
     result_df = upr(project_dir=project_dir, previous_result=previous_result, top_k=top_k)
-    base_reranker_node_test(result_df, top_k)
+    base_reranker_node_test(result_df, top_k, descending=False)
```

### Comparing `autorag-0.1.6/tests/autorag/nodes/promptmaker/test_fstring.py` & `autorag-0.1.7/tests/autorag/nodes/promptmaker/test_fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/promptmaker/test_long_context_reorder.py` & `autorag-0.1.7/tests/autorag/nodes/promptmaker/test_long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py` & `autorag-0.1.7/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py` & `autorag-0.1.7/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_hyde.py` & `autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py` & `autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_query_decompose.py` & `autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py` & `autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py` & `autorag-0.1.7/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/retrieval/test_bm25.py` & `autorag-0.1.7/tests/autorag/nodes/retrieval/test_bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_base.py` & `autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_cc.py` & `autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py` & `autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_rrf.py` & `autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/retrieval/test_hybrid_rsf.py` & `autorag-0.1.7/tests/autorag/nodes/retrieval/test_hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/retrieval/test_retrieval_base.py` & `autorag-0.1.7/tests/autorag/nodes/retrieval/test_retrieval_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/retrieval/test_run_retrieval_node.py` & `autorag-0.1.7/tests/autorag/nodes/retrieval/test_run_retrieval_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/nodes/retrieval/test_vectordb.py` & `autorag-0.1.7/tests/autorag/nodes/retrieval/test_vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/schema/test_module_schema.py` & `autorag-0.1.7/tests/autorag/schema/test_module_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/schema/test_node_schema.py` & `autorag-0.1.7/tests/autorag/schema/test_node_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/test_cli.py` & `autorag-0.1.7/tests/autorag/test_cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/test_deploy.py` & `autorag-0.1.7/tests/autorag/test_deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/test_evaluator.py` & `autorag-0.1.7/tests/autorag/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/test_strategy.py` & `autorag-0.1.7/tests/autorag/test_strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/test_web.py` & `autorag-0.1.7/tests/autorag/test_web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/utils/test_preprocess.py` & `autorag-0.1.7/tests/autorag/utils/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/autorag/utils/test_util.py` & `autorag-0.1.7/tests/autorag/utils/test_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/delete_tests.py` & `autorag-0.1.7/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/mock.py` & `autorag-0.1.7/tests/mock.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/README.md` & `autorag-0.1.7/tests/resources/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/corpus_data_sample.parquet` & `autorag-0.1.7/tests/resources/corpus_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/data_creation/raw_dir/sample1.txt` & `autorag-0.1.7/tests/resources/data_creation/raw_dir/sample1.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/data_creation/raw_dir/sample2.txt` & `autorag-0.1.7/tests/resources/data_creation/raw_dir/sample2.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/data_creation/raw_dir/sample3.txt` & `autorag-0.1.7/tests/resources/data_creation/raw_dir/sample3.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/full.yaml` & `autorag-0.1.7/tests/resources/full.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/qa_data_sample.parquet` & `autorag-0.1.7/tests/resources/qa_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/qa_test_data_sample.parquet` & `autorag-0.1.7/tests/resources/qa_test_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/config.yaml` & `autorag-0.1.7/tests/resources/result_project/0/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet` & `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet` & `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet` & `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet` & `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet` & `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet` & `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet` & `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv` & `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet` & `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet` & `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv` & `autorag-0.1.7/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.7/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.7/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/0/summary.csv` & `autorag-0.1.7/tests/resources/result_project/0/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/1/config.yaml` & `autorag-0.1.7/tests/resources/result_project/1/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.7/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.7/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/config.yaml` & `autorag-0.1.7/tests/resources/result_project/2/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.7/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.7/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.7/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/3/config.yaml` & `autorag-0.1.7/tests/resources/result_project/3/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/best.yaml` & `autorag-0.1.7/tests/resources/result_project/best.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/data/corpus.parquet` & `autorag-0.1.7/tests/resources/result_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/data/qa.parquet` & `autorag-0.1.7/tests/resources/result_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/resources/bm25.pkl` & `autorag-0.1.7/tests/resources/result_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin` & `autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin` & `autorag-0.1.7/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/result_project/resources/chroma/chroma.sqlite3` & `autorag-0.1.7/tests/resources/result_project/resources/chroma/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/sample_contents_nqa.csv` & `autorag-0.1.7/tests/resources/sample_contents_nqa.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/sample_project/data/corpus.parquet` & `autorag-0.1.7/tests/resources/sample_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/sample_project/data/qa.parquet` & `autorag-0.1.7/tests/resources/sample_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/sample_project/resources/bm25.pkl` & `autorag-0.1.7/tests/resources/sample_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/simple.yaml` & `autorag-0.1.7/tests/resources/simple.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.6/tests/resources/test_bm25_retrieval.pkl` & `autorag-0.1.7/tests/resources/test_bm25_retrieval.pkl`

 * *Files identical despite different names*

