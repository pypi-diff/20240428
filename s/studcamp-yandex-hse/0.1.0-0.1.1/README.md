# Comparing `tmp/studcamp_yandex_hse-0.1.0.tar.gz` & `tmp/studcamp_yandex_hse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "studcamp_yandex_hse-0.1.0.tar", max compression
+gzip compressed data, was "studcamp_yandex_hse-0.1.1.tar", max compression
```

## Comparing `studcamp_yandex_hse-0.1.0.tar` & `studcamp_yandex_hse-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     3863 2024-04-27 23:37:33.783951 studcamp_yandex_hse-0.1.0/README.md
--rw-r--r--   0        0        0      919 2024-04-28 09:35:25.914937 studcamp_yandex_hse-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-27 13:13:54.534284 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/__init__.py
--rw-r--r--   0        0        0      249 2024-04-28 08:47:53.048597 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/__init__.py
--rw-r--r--   0        0        0      133 2024-04-27 23:37:33.787449 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/attention_based_model/__init__.py
--rw-r--r--   0        0        0     3648 2024-04-27 23:37:33.787823 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/attention_based_model/attention_extractor.py
--rw-r--r--   0        0        0     1299 2024-04-27 23:37:33.788140 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/attention_based_model/tags_extractor.py
--rw-r--r--   0        0        0       66 2024-04-27 23:37:33.788566 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/bart_based_model/__init__.py
--rw-r--r--   0        0        0     3148 2024-04-27 23:37:33.788881 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/bart_based_model/tag_sum_extractor.py
--rw-r--r--   0        0        0      801 2024-04-27 23:37:33.789296 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/base_extractor.py
--rw-r--r--   0        0        0       84 2024-04-27 23:37:33.789591 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/clusterizer_based_model/__init__.py
--rw-r--r--   0        0        0     2018 2024-04-28 08:47:12.675338 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/clusterizer_based_model/clusterizer.py
--rw-r--r--   0        0        0     1330 2024-04-27 23:37:33.790132 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/clusterizer_based_model/faiss.py
--rw-r--r--   0        0        0     1230 2024-04-27 23:37:33.790398 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/metrics.py
--rw-r--r--   0        0        0      205 2024-04-27 23:37:33.790656 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/rake_based_model/__init__.py
--rw-r--r--   0        0        0     1398 2024-04-27 23:37:33.790916 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/rake_based_model/keyphrases_extractor.py
--rw-r--r--   0        0        0     3082 2024-04-27 23:37:33.791175 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/rake_based_model/tags_extractor.py
--rw-r--r--   0        0        0       58 2024-04-28 08:50:50.032597 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/rut5_based_model/__init__.py
--rw-r--r--   0        0        0     1067 2024-04-28 09:43:12.655490 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/rut5_based_model/rut5_extractor.py
--rw-r--r--   0        0        0        0 2024-04-27 23:37:33.791220 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/__init__.py
--rw-r--r--   0        0        0      138 2024-04-27 23:37:33.791733 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/embedder/__init__.py
--rw-r--r--   0        0        0      803 2024-04-27 23:37:33.791972 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/embedder/base_embedder.py
--rw-r--r--   0        0        0     1071 2024-04-27 23:37:33.792207 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/embedder/fasttext_embedder.py
--rw-r--r--   0        0        0     1378 2024-04-27 23:37:33.792453 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/embedder/rubert_embedder.py
--rw-r--r--   0        0        0      210 2024-04-27 23:37:33.792695 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/normalizers/__init__.py
--rw-r--r--   0        0        0      308 2024-04-27 23:37:33.792946 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/normalizers/base_normalizer.py
--rw-r--r--   0        0        0      956 2024-04-27 23:37:33.793212 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/normalizers/nouns_keeper.py
--rw-r--r--   0        0        0      818 2024-04-27 23:37:33.793493 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/normalizers/pipe.py
--rw-r--r--   0        0        0      694 2024-04-27 23:37:33.793749 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/normalizers/punctuation_deleter.py
--rw-r--r--   0        0        0      850 2024-04-27 23:37:33.794009 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/normalizers/stopwords_deleter.py
--rw-r--r--   0        0        0      130 2024-04-27 23:37:33.794376 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/ranker/__init__.py
--rw-r--r--   0        0        0     1686 2024-04-27 23:37:33.794642 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/ranker/base_ranker.py
--rw-r--r--   0        0        0     1183 2024-04-27 23:37:33.794908 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/ranker/max_distance_ranker.py
--rw-r--r--   0        0        0      933 2024-04-27 23:37:33.795293 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/ranker/text_sim_ranker.py
--rw-r--r--   0        0        0       50 2024-04-27 23:37:33.795681 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/summarizator/__init__.py
--rw-r--r--   0        0        0     1331 2024-04-27 23:37:33.795945 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/summarizator/bart_summarization.py
--rw-r--r--   0        0        0       58 2024-04-27 23:37:33.796180 studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/utils.py
--rw-r--r--   0        0        0     4854 1970-01-01 00:00:00.000000 studcamp_yandex_hse-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4076 2024-04-28 13:09:29.174808 studcamp_yandex_hse-0.1.1/README.md
+-rw-r--r--   0        0        0      919 2024-04-28 13:15:29.182566 studcamp_yandex_hse-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-27 13:13:54.534284 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/__init__.py
+-rw-r--r--   0        0        0      249 2024-04-28 12:14:43.071215 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-27 23:37:33.787449 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/attention_based_model/__init__.py
+-rw-r--r--   0        0        0     3648 2024-04-27 23:37:33.787823 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/attention_based_model/attention_extractor.py
+-rw-r--r--   0        0        0     1299 2024-04-27 23:37:33.788140 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/attention_based_model/tags_extractor.py
+-rw-r--r--   0        0        0       66 2024-04-27 23:37:33.788566 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/bart_based_model/__init__.py
+-rw-r--r--   0        0        0     3148 2024-04-27 23:37:33.788881 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/bart_based_model/tag_sum_extractor.py
+-rw-r--r--   0        0        0      801 2024-04-27 23:37:33.789296 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/base_extractor.py
+-rw-r--r--   0        0        0       84 2024-04-27 23:37:33.789591 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/clusterizer_based_model/__init__.py
+-rw-r--r--   0        0        0     2018 2024-04-28 12:14:43.072641 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/clusterizer_based_model/clusterizer.py
+-rw-r--r--   0        0        0     1330 2024-04-27 23:37:33.790132 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/clusterizer_based_model/faiss.py
+-rw-r--r--   0        0        0     1230 2024-04-27 23:37:33.790398 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/metrics.py
+-rw-r--r--   0        0        0      205 2024-04-27 23:37:33.790656 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rake_based_model/__init__.py
+-rw-r--r--   0        0        0     1398 2024-04-27 23:37:33.790916 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rake_based_model/keyphrases_extractor.py
+-rw-r--r--   0        0        0     3082 2024-04-27 23:37:33.791175 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rake_based_model/tags_extractor.py
+-rw-r--r--   0        0        0       58 2024-04-28 12:14:43.072825 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rut5_based_model/__init__.py
+-rw-r--r--   0        0        0     1067 2024-04-28 12:14:43.073098 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rut5_based_model/rut5_extractor.py
+-rw-r--r--   0        0        0        0 2024-04-27 23:37:33.791220 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/__init__.py
+-rw-r--r--   0        0        0      138 2024-04-27 23:37:33.791733 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/__init__.py
+-rw-r--r--   0        0        0      803 2024-04-27 23:37:33.791972 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/base_embedder.py
+-rw-r--r--   0        0        0     1071 2024-04-27 23:37:33.792207 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/fasttext_embedder.py
+-rw-r--r--   0        0        0     1378 2024-04-27 23:37:33.792453 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/rubert_embedder.py
+-rw-r--r--   0        0        0      210 2024-04-27 23:37:33.792695 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/__init__.py
+-rw-r--r--   0        0        0      308 2024-04-27 23:37:33.792946 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/base_normalizer.py
+-rw-r--r--   0        0        0      956 2024-04-27 23:37:33.793212 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/nouns_keeper.py
+-rw-r--r--   0        0        0      818 2024-04-27 23:37:33.793493 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/pipe.py
+-rw-r--r--   0        0        0      694 2024-04-27 23:37:33.793749 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/punctuation_deleter.py
+-rw-r--r--   0        0        0      850 2024-04-27 23:37:33.794009 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/stopwords_deleter.py
+-rw-r--r--   0        0        0      130 2024-04-27 23:37:33.794376 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/__init__.py
+-rw-r--r--   0        0        0     1686 2024-04-27 23:37:33.794642 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/base_ranker.py
+-rw-r--r--   0        0        0     1183 2024-04-27 23:37:33.794908 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/max_distance_ranker.py
+-rw-r--r--   0        0        0      933 2024-04-27 23:37:33.795293 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/text_sim_ranker.py
+-rw-r--r--   0        0        0       50 2024-04-27 23:37:33.795681 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/summarizator/__init__.py
+-rw-r--r--   0        0        0     1331 2024-04-27 23:37:33.795945 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/summarizator/bart_summarization.py
+-rw-r--r--   0        0        0       58 2024-04-27 23:37:33.796180 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/utils.py
+-rw-r--r--   0        0        0     5067 1970-01-01 00:00:00.000000 studcamp_yandex_hse-0.1.1/PKG-INFO
```

### Comparing `studcamp_yandex_hse-0.1.0/README.md` & `studcamp_yandex_hse-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <h1 align="center" id="title">Studcamp Yandex x HSE</h1>
 
 <h2 align="center" id="title">Text Tagging</h2>
 
-<h3 align='left'> My team and I developed a whole module for "Text Tagging" problem, in terms of keywords extraction. </h3>
+<h3 align='left'> My team and I, within machine learning studcamp by Yandex and HSE, developed a whole module for "Text Tagging" problem, in terms of keywords extraction. </h3>
 
 <h3 align='left'> We had a big research. We've tried several extractive and abstractive methods. We will discuss it further.</h3>
 
 <h2>🚀 Demo</h2>
 
 <p align="center"> Streamlit  </p>
 
@@ -19,15 +19,15 @@
 
 <h2>🤖 Models</h2>
 
 ### Exctractive models
 *   **RakeBasedTagger:** This is a model which based on a well-known Rake algorithm, that extract meaningful words from text. It's very fast and can be used online. After extracting meaningful words, we should normalize such words and performing filtering with taking only top_n words with the largest distance between query word and other meaningful words. This algorithm supposes that keywords should be as far as possible from each other to represent different domains of the text.
 *   **BartBasedTagger:** This is a rubert-based model which makes an assumption that we could find the most significat words to our text as such with the best cosine similarity. During the pipeline, firstly we need to summarize our text with MBart model, then we should extract the most significant words with cosine similarity for text embedding with each word embedding of the text via rubert represenation. This model is very slow and can be used offline, as we need to summarize text before main processing.
 *   **AttentionBasedTagger:** This is a very interesting model. We assumed that all the algorithms above couldn't catch bigram keywords. So, we decided to use attention mechanism. Let's compute attention activation for every pair of tokens. The biggest activation means, that such words are meaningful to each other. The other problem was that Mbart uses bpe tokenizer and we should perform some post-processing to construct interpretable keywords.
-*   **ClustrizationBasedTagger:** Experimental extractitve model. We used DBSCAN on embeddings of words from normalized text to get clusters of words with similar meaning. Each cluster centroid embedding is a potential keyword. So, we can convert it's embedding to the nearest fasttext word embedding.
+*   **ClusterizationBasedTagger:** Experimental extractitve model. We used DBSCAN on embeddings of words from normalized text to get clusters of words with similar meaning. Each cluster centroid embedding is a potential keyword. So, we can convert it's embedding to the nearest fasttext word embedding.
 
 ### Abstractive models
 *   **RuT5Tagger:** Model that was trained on an aggregated dataset from different sources like 'Живой журнал', 'Пикабу' etc. It needs to be mentioned that this model is abstractive, so it can generate new keywords that are not present in the text. Moreover, such model need to be trained on a big dataset further to be able to give good results.
 
 <h2>🧐 Features</h2>
 
 Here're some of the project's best features:
@@ -39,24 +39,25 @@
 
 <p>1. Installation</p>
 
 ```
 pip install studcamp-yandex-hse
 ```
 
-<p>2. Download russian FastText embeddings with link below and paste it in the root of your repository</p>
+<p>2. Download russian FastText embeddings and RuT5 weights with the links below and paste it at the same level as your source .py file</p>
 
 ```
-https://fasttext.cc/docs/en/crawl-vectors.html
+FastText embeddings: https://fasttext.cc/docs/en/crawl-vectors.html
+Weights: https://drive.google.com/file/d/1aqVtoNRX3xDokthxuBNFwfcXQfkKeAMa/view?usp=sharing
 ```
 
 <p>3. Import</p>
 
 ```
-from studcamp_yandex_hse.models import RakeBasedTagger, BartBasedTagger, AttentionBasedTagger, ClustrizationBasedTagger
+from studcamp_yandex_hse.models import RakeBasedTagger, BartBasedTagger, AttentionBasedTagger, ClusterizationBasedTagger, RuT5Tagger
 ```
 
 <p>3. Init tagger</p>
 
 ```
 tagger = RakeBasedTagger()
 ```
```

### Comparing `studcamp_yandex_hse-0.1.0/pyproject.toml` & `studcamp_yandex_hse-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "studcamp-yandex-hse"
-version = "0.1.0"
+version = "0.1.1"
 description = "Text-tagging project within Yandex x HSE StudCamp event"
 authors = ["deniskazhekin <deniskazhekin@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "studcamp_yandex_hse" }]
 
 [tool.poetry.dependencies]
```

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/attention_based_model/attention_extractor.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/attention_based_model/attention_extractor.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/attention_based_model/tags_extractor.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/attention_based_model/tags_extractor.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/bart_based_model/tag_sum_extractor.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/bart_based_model/tag_sum_extractor.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/base_extractor.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/base_extractor.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/clusterizer_based_model/clusterizer.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/clusterizer_based_model/clusterizer.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/clusterizer_based_model/faiss.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/clusterizer_based_model/faiss.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/metrics.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/metrics.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/rake_based_model/keyphrases_extractor.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rake_based_model/keyphrases_extractor.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/rake_based_model/tags_extractor.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rake_based_model/tags_extractor.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/models/rut5_based_model/rut5_extractor.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rut5_based_model/rut5_extractor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import warnings
+
 warnings.filterwarnings("ignore")
 
-from transformers import T5ForConditionalGeneration, T5Tokenizer
 from peft import PeftModel
+from transformers import T5ForConditionalGeneration, T5Tokenizer
 
 
 class RuT5Tagger:
-
     def __init__(self):
-        model_path = 'sarahai/ruT5-base-summarizer'
-        saved_model_dir = './weights'
+        model_path = "sarahai/ruT5-base-summarizer"
+        saved_model_dir = "./weights"
 
-        model = T5ForConditionalGeneration.from_pretrained(model_path, device_map='cpu', offload_state_dict=True)
+        model = T5ForConditionalGeneration.from_pretrained(model_path, device_map="cpu", offload_state_dict=True)
         self.peft_model = PeftModel.from_pretrained(model, saved_model_dir)
         self.tokenizer = T5Tokenizer.from_pretrained(saved_model_dir)
 
     def extract(self, text: str, top_p: int = 0.9, temperature: float = 0.5):
-        tokenized = self.tokenizer(text, padding='longest', truncation=True, max_length=2048, return_tensors='pt')
+        tokenized = self.tokenizer(text, padding="longest", truncation=True, max_length=2048, return_tensors="pt")
         output = self.peft_model.generate(
             **tokenized,
             do_sample=True,
             temperature=temperature,
             top_p=top_p,
-
         )
-        decoded = set(self.tokenizer.decode(output[0], skip_special_tokens=True).split(';'))
-        tags = [tag for tag in decoded if tag != '']
-        return tags
+        decoded = set(self.tokenizer.decode(output[0], skip_special_tokens=True).split(";"))
+        tags = [tag for tag in decoded if tag != ""]
+        return tags
```

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/embedder/base_embedder.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/base_embedder.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/embedder/fasttext_embedder.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/fasttext_embedder.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/embedder/rubert_embedder.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/rubert_embedder.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/normalizers/nouns_keeper.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/nouns_keeper.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/normalizers/pipe.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/pipe.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/normalizers/punctuation_deleter.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/punctuation_deleter.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/normalizers/stopwords_deleter.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/stopwords_deleter.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/ranker/base_ranker.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/base_ranker.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/ranker/max_distance_ranker.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/max_distance_ranker.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/ranker/text_sim_ranker.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/text_sim_ranker.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/studcamp_yandex_hse/processing/summarizator/bart_summarization.py` & `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/summarizator/bart_summarization.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.0/PKG-INFO` & `studcamp_yandex_hse-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: studcamp-yandex-hse
-Version: 0.1.0
+Version: 0.1.1
 Summary: Text-tagging project within Yandex x HSE StudCamp event
 License: MIT
 Author: deniskazhekin
 Author-email: deniskazhekin@yandex.ru
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
 Requires-Dist: transformers (>=4.40.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center" id="title">Studcamp Yandex x HSE</h1>
 
 <h2 align="center" id="title">Text Tagging</h2>
 
-<h3 align='left'> My team and I developed a whole module for "Text Tagging" problem, in terms of keywords extraction. </h3>
+<h3 align='left'> My team and I, within machine learning studcamp by Yandex and HSE, developed a whole module for "Text Tagging" problem, in terms of keywords extraction. </h3>
 
 <h3 align='left'> We had a big research. We've tried several extractive and abstractive methods. We will discuss it further.</h3>
 
 <h2>🚀 Demo</h2>
 
 <p align="center"> Streamlit  </p>
 
@@ -45,15 +45,15 @@
 
 <h2>🤖 Models</h2>
 
 ### Exctractive models
 *   **RakeBasedTagger:** This is a model which based on a well-known Rake algorithm, that extract meaningful words from text. It's very fast and can be used online. After extracting meaningful words, we should normalize such words and performing filtering with taking only top_n words with the largest distance between query word and other meaningful words. This algorithm supposes that keywords should be as far as possible from each other to represent different domains of the text.
 *   **BartBasedTagger:** This is a rubert-based model which makes an assumption that we could find the most significat words to our text as such with the best cosine similarity. During the pipeline, firstly we need to summarize our text with MBart model, then we should extract the most significant words with cosine similarity for text embedding with each word embedding of the text via rubert represenation. This model is very slow and can be used offline, as we need to summarize text before main processing.
 *   **AttentionBasedTagger:** This is a very interesting model. We assumed that all the algorithms above couldn't catch bigram keywords. So, we decided to use attention mechanism. Let's compute attention activation for every pair of tokens. The biggest activation means, that such words are meaningful to each other. The other problem was that Mbart uses bpe tokenizer and we should perform some post-processing to construct interpretable keywords.
-*   **ClustrizationBasedTagger:** Experimental extractitve model. We used DBSCAN on embeddings of words from normalized text to get clusters of words with similar meaning. Each cluster centroid embedding is a potential keyword. So, we can convert it's embedding to the nearest fasttext word embedding.
+*   **ClusterizationBasedTagger:** Experimental extractitve model. We used DBSCAN on embeddings of words from normalized text to get clusters of words with similar meaning. Each cluster centroid embedding is a potential keyword. So, we can convert it's embedding to the nearest fasttext word embedding.
 
 ### Abstractive models
 *   **RuT5Tagger:** Model that was trained on an aggregated dataset from different sources like 'Живой журнал', 'Пикабу' etc. It needs to be mentioned that this model is abstractive, so it can generate new keywords that are not present in the text. Moreover, such model need to be trained on a big dataset further to be able to give good results.
 
 <h2>🧐 Features</h2>
 
 Here're some of the project's best features:
@@ -65,24 +65,25 @@
 
 <p>1. Installation</p>
 
 ```
 pip install studcamp-yandex-hse
 ```
 
-<p>2. Download russian FastText embeddings with link below and paste it in the root of your repository</p>
+<p>2. Download russian FastText embeddings and RuT5 weights with the links below and paste it at the same level as your source .py file</p>
 
 ```
-https://fasttext.cc/docs/en/crawl-vectors.html
+FastText embeddings: https://fasttext.cc/docs/en/crawl-vectors.html
+Weights: https://drive.google.com/file/d/1aqVtoNRX3xDokthxuBNFwfcXQfkKeAMa/view?usp=sharing
 ```
 
 <p>3. Import</p>
 
 ```
-from studcamp_yandex_hse.models import RakeBasedTagger, BartBasedTagger, AttentionBasedTagger, ClustrizationBasedTagger
+from studcamp_yandex_hse.models import RakeBasedTagger, BartBasedTagger, AttentionBasedTagger, ClusterizationBasedTagger, RuT5Tagger
 ```
 
 <p>3. Init tagger</p>
 
 ```
 tagger = RakeBasedTagger()
 ```
```

