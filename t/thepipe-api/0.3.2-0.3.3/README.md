# Comparing `tmp/thepipe_api-0.3.2.tar.gz` & `tmp/thepipe_api-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.3.2.tar", last modified: Sat Apr 27 02:15:42 2024, max compression
+gzip compressed data, was "thepipe_api-0.3.3.tar", last modified: Sun Apr 28 06:43:18 2024, max compression
```

## Comparing `thepipe_api-0.3.2.tar` & `thepipe_api-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 02:15:42.861469 thepipe_api-0.3.2/
--rw-rw-rw-   0        0        0     1094 2024-04-18 07:46:31.000000 thepipe_api-0.3.2/LICENSE
--rw-rw-rw-   0        0        0    11534 2024-04-27 02:15:42.860469 thepipe_api-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    10752 2024-04-25 19:05:20.000000 thepipe_api-0.3.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 02:15:42.861469 thepipe_api-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-27 02:15:18.000000 thepipe_api-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 02:15:42.820461 thepipe_api-0.3.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-18 07:46:31.000000 thepipe_api-0.3.2/tests/__init__.py
--rw-rw-rw-   0        0        0     9265 2024-04-18 07:46:31.000000 thepipe_api-0.3.2/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-27 02:15:42.833462 thepipe_api-0.3.2/thepipe_api/
--rw-rw-rw-   0        0        0       86 2024-04-18 07:46:31.000000 thepipe_api-0.3.2/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4821 2024-04-18 07:46:31.000000 thepipe_api-0.3.2/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2799 2024-04-23 05:54:32.000000 thepipe_api-0.3.2/thepipe_api/core.py
--rw-rw-rw-   0        0        0    21490 2024-04-27 02:14:52.000000 thepipe_api-0.3.2/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3704 2024-04-20 03:49:35.000000 thepipe_api-0.3.2/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-27 02:15:42.858478 thepipe_api-0.3.2/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0    11534 2024-04-27 02:15:42.000000 thepipe_api-0.3.2/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-27 02:15:42.000000 thepipe_api-0.3.2/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 02:15:42.000000 thepipe_api-0.3.2/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-27 02:15:42.000000 thepipe_api-0.3.2/thepipe_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2024-04-27 02:15:42.000000 thepipe_api-0.3.2/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-27 02:15:42.000000 thepipe_api-0.3.2/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 06:43:18.445625 thepipe_api-0.3.3/
+-rw-rw-rw-   0        0        0     1094 2024-04-18 07:46:31.000000 thepipe_api-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0    12404 2024-04-28 06:43:18.444634 thepipe_api-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11622 2024-04-28 06:43:08.000000 thepipe_api-0.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 06:43:18.445625 thepipe_api-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-28 06:43:08.000000 thepipe_api-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:43:18.410585 thepipe_api-0.3.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-18 07:46:31.000000 thepipe_api-0.3.3/tests/__init__.py
+-rw-rw-rw-   0        0        0    11487 2024-04-28 06:43:08.000000 thepipe_api-0.3.3/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:43:18.417632 thepipe_api-0.3.3/thepipe_api/
+-rw-rw-rw-   0        0        0       86 2024-04-18 07:46:31.000000 thepipe_api-0.3.3/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4362 2024-04-28 03:24:11.000000 thepipe_api-0.3.3/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2878 2024-04-28 06:43:08.000000 thepipe_api-0.3.3/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    24815 2024-04-28 06:43:08.000000 thepipe_api-0.3.3/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3704 2024-04-20 03:49:35.000000 thepipe_api-0.3.3/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:43:18.443627 thepipe_api-0.3.3/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0    12404 2024-04-28 06:43:18.000000 thepipe_api-0.3.3/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-28 06:43:18.000000 thepipe_api-0.3.3/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 06:43:18.000000 thepipe_api-0.3.3/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-28 06:43:18.000000 thepipe_api-0.3.3/thepipe_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      127 2024-04-28 06:43:18.000000 thepipe_api-0.3.3/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-28 06:43:18.000000 thepipe_api-0.3.3/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.3.2/LICENSE` & `thepipe_api-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.3.2/PKG-INFO` & `thepipe_api-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.3.2
+Version: 0.3.3
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,27 +26,28 @@
 
 
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
 <p>
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
-[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
+[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-access-blue)</a>
 
-### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
+### Feed PDFs, web pages, word docs, slides, videos, CSV, and more into Vision-LLMs with one line of code ⚡
 
 The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. 
 
-![Demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/grader.py%20(6).png)
+![Science assistant demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/science_assistantpy2.png)
+
 
 ## Features 🌟
 
 - Extracts text and visuals from files or web pages 📚
-- Outputs chunks optimized for multimodal LLMs 🖼️
-- Interpret complex PDFs, web pages, slides, CSVs, and more 🧠
+- Outputs chunks optimized for multimodal LLMs and RAG frameworks 🖼️
+- Interpret complex PDFs, web pages, docs, videos, data, and more 🧠
 - Auto-compress prompts exceeding your chosen token limit 📦
 - Works even with missing file extensions, in-memory data streams 💾
 - Works with codebases, git repos, and custom integrations 🌐
 - Multi-threaded ⚡️
 
 ## Getting Started  🚀
 
@@ -60,15 +61,15 @@
 The Pipe is available as a hosted API, or it can be set up locally. An API key is recommended for out-of-the-box functionality (alternatively, see the local installation section). Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have a key yet? [Get one here](https://thepi.pe).
 
 Now you can extract comprehensive text and visuals from any file:
 ```python
 from thepipe_api import thepipe
 messages = thepipe.extract("example.pdf")
 ```
-Or any website:
+Or websites:
 ```python
 messages = thepipe.extract("https://example.com")
 ```
 Then feed it into GPT-4-Vision:
 ```python
 response = client.chat.completions.create(
     model="gpt-4-vision-preview",
@@ -79,29 +80,33 @@
 ![Just call OpenAI](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/IMG_0180.jpg)
 
 You can also use The Pipe from the command line. Here's how to recursively extract from a directory, matching only files containing a substring (in this example, typescript files) and ignore files containing other substrings (in this example, anything in the "tests" folder):
 ```bash
 thepipe path/to/folder --match tsx --ignore tests
 ```
 
+
 ## Supported File Types 📚
 
 | Source Type                           | Input types        | Token Compression 🗜️ | Image Extraction 👁️ | Notes 📌                                                  |
 |---------------------------------------|------------------------------------------|-------------------|------------------|---------------------------------------------------------|
 | Directory                             | Any `/path/to/directory`                 | ✔️               | ✔️               | Extracts from all files in directory, supports match and ignore patterns |
 | Code                                  | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | ✔️ (varies)   | ❌               | Combines all code files. `.c`, `.cpp`, `.py` are compressible with ctags, others are not |
 | Plaintext                             | `.txt`, `.md`, `.rtf`, etc               | ✔️               | ❌               | Regular text files                                                      |
 | PDF                                   | `.pdf`                                  | ✔️               | ✔️    | Extracts text and images of each page; can use AI for extraction of table data and  images within pages |
 | Image                                 | `.jpg`, `.jpeg`, `.png` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
 | Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
+| Video                                 | `.mp4`, `.avi`, `.mov`, `.wmv`     | ✔️               | ✔️                | Extracts frames from video files; supports frame extraction and OCR for text extraction from frames |
+| Audio                                 | `.mp3`, `.wav`          | ✔️               | ❌                | Extracts text from audio files; supports speech-to-text conversion        | 
 | Website                               | URLs (inputs containing `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
+| YouTube Video                         | YouTube video URLs                      | ✔️               | ✔️                | Extracts text from YouTube videos; supports subtitles extraction          |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
 ## How it works 🛠️
 
 The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible list of multimodal messages representing chunks of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned should look like this:
 ```json
 [
@@ -119,20 +124,22 @@
         }
       }
     ]
   }
 ]
 ```
 If you want to feed these messages directly into the model, it is important to be mindful of the token limit.
-OpenAI does not allow too many images in the prompt (see discussion [here](https://community.openai.com/t/gpt-4-vision-maximum-amount-of-images/573110/6)), so long files should be extracted with `text_only=True` to avoid this issue. 
+OpenAI does not allow too many images in the prompt (see discussion [here](https://community.openai.com/t/gpt-4-vision-maximum-amount-of-images/573110/6)), so long files should be extracted with `text_only=True` to avoid this issue, while long text files should either be compressed or embedded in a RAG framework.
 
 The text and images from these messages may also be prepared for a vector database with `thepipe.core.create_chunks_from_messages` or for downstream use with RAG frameworks. [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider. 
 
 It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), opt-in AI [table, equation, and figure extraction](https://thepi.pe/pricing), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
 
+![Demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/grader.py%20(6).png)
+
 
 ## Local Installation 🛠️
 
 The Pipe handles a wide array of complex filetypes, and thus requires installation of many different packages to function. It also requires a very capable machine for good response times. For this reason, we host it as an API that works out-of-the-box. To use The Pipe locally for free instead, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements:
 
 ```bash
 git clone https://github.com/emcf/thepipe
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.3.2 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.3.3 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
@@ -11,100 +11,108 @@
 _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
 _E_n_g_l_i_s_h | _ä_¸_­_æ__
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/
 badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
 action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
-_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
-docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
-Pipe is a multimodal-first tool for feeding files and web pages into vision-
-language models such as GPT-4V. It is best for LLM and RAG applications that
-require a deep understanding of tricky data sources. The Pipe is available as a
-hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. !
-[Demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/
-assets/grader.py%20(6).png) ## Features ð - Extracts text and visuals from
-files or web pages ð - Outputs chunks optimized for multimodal LLMs ð¼ï¸
-- Interpret complex PDFs, web pages, slides, CSVs, and more ð§  - Auto-
-compress prompts exceeding your chosen token limit ð¦ - Works even with
-missing file extensions, in-memory data streams ð¾ - Works with codebases,
-git repos, and custom integrations ð - Multi-threaded â¡ï¸ ## Getting
-Started ð The Pipe handles a wide array of complex filetypes, and thus has
-many dependencies that must be installed separately. It also requires a strong
-machine for good response times. For this reason, we host it as an API that
-works out-of-the-box. First, install The Pipe. ``` pip install thepipe_api ```
-The Pipe is available as a hosted API, or it can be set up locally. An API key
-is recommended for out-of-the-box functionality (alternatively, see the local
-installation section). Ensure the `THEPIPE_API_KEY` environment variable is
-set. Don't have a key yet? [Get one here](https://thepi.pe). Now you can
-extract comprehensive text and visuals from any file: ```python from
-thepipe_api import thepipe messages = thepipe.extract("example.pdf") ``` Or any
-website: ```python messages = thepipe.extract("https://example.com") ``` Then
-feed it into GPT-4-Vision: ```python response = client.chat.completions.create
-( model="gpt-4-vision-preview", messages = messages, ) ``` ![Just call OpenAI]
-(https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/
-IMG_0180.jpg) You can also use The Pipe from the command line. Here's how to
-recursively extract from a directory, matching only files containing a
-substring (in this example, typescript files) and ignore files containing other
-substrings (in this example, anything in the "tests" folder): ```bash thepipe
-path/to/folder --match tsx --ignore tests ``` ## Supported File Types ð |
-Source Type | Input types | Token Compression ðï¸ | Image Extraction
-ðï¸ | Notes ð | |---------------------------------------|---------------
----------------------------|-------------------|------------------|------------
----------------------------------------------| | Directory | Any `/path/to/
-directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
-match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
-`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
-`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
-`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
-âï¸ | âï¸ | Extracts text and images of each page; can use AI for
-extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
-`.png` | â | âï¸ | Extracts images, uses OCR if text_only | | Data Table |
-`.csv`, `.xls`, `.xlsx` | âï¸ | â | Extracts data from spreadsheets;
-converts to text representation. For very large datasets, will only extract
-column names and types | | Jupyter Notebook | `.ipynb` | â | âï¸ |
-Extracts code, markdown, and images from Jupyter notebooks | | Microsoft Word
-Document | `.docx` | âï¸ | âï¸ | Extracts text and images from Word
-documents | | Microsoft PowerPoint Presentation | `.pptx` | âï¸ | âï¸ |
-Extracts text and images from PowerPoint presentations | | Website | URLs
-(inputs containing `http`, `https`, `ftp`) | âï¸ | âï¸ | Extracts text
-from web page along with image (or images if scrollable); text-only extraction
-available | | GitHub Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts
-from GitHub repositories; supports branch specification | | ZIP File | `.zip` |
-âï¸ | âï¸ | Extracts contents of ZIP files; supports nested directory
-extraction | ## How it works ð ï¸ The input source is either a file path, a
-URL, or a directory. The pipe will extract information from the source and
-process it for downstream use with [language models](https://en.wikipedia.org/
-wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/
-wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/
-2304.00685). The output from the pipe is a sensible list of multimodal messages
-representing chunks of the extracted information, carefully crafted to fit
-within context windows for any models from [gemma-7b](https://huggingface.co/
-google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned
-should look like this: ```json [ { "role": "user", "content": [ { "type":
-"text", "text": "..." }, { "type": "image_url", "image_url": { "url": "data:
-image/jpeg;base64,..." } } ] } ] ``` If you want to feed these messages
-directly into the model, it is important to be mindful of the token limit.
-OpenAI does not allow too many images in the prompt (see discussion [here]
-(https://community.openai.com/t/gpt-4-vision-maximum-amount-of-images/573110/
-6)), so long files should be extracted with `text_only=True` to avoid this
-issue. The text and images from these messages may also be prepared for a
-vector database with `thepipe.core.create_chunks_from_messages` or for
-downstream use with RAG frameworks. [LiteLLM](https://github.com/BerriAI/
-litellm) can be used to easily integrate The Pipe with any LLM provider. It
-uses a variety of heuristics for optimal performance with vision-language
-models, including AI filetype detection with [filetype detection](https://
-opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-
-type-identification.html), opt-in AI [table, equation, and figure extraction]
-(https://thepi.pe/pricing), efficient [token compression](https://arxiv.org/
-abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/
-Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle]
-(https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work
-out-of-the-box. ## Local Installation ð ï¸ The Pipe handles a wide array of
-complex filetypes, and thus requires installation of many different packages to
+_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, web pages,
+word docs, slides, videos, CSV, and more into Vision-LLMs with one line of code
+â¡ The Pipe is a multimodal-first tool for feeding files and web pages into
+vision-language models such as GPT-4V. It is best for LLM and RAG applications
+that require a deep understanding of tricky data sources. The Pipe is available
+as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. !
+[Science assistant demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/
+object/public/assets/science_assistantpy2.png) ## Features ð - Extracts text
+and visuals from files or web pages ð - Outputs chunks optimized for
+multimodal LLMs and RAG frameworks ð¼ï¸ - Interpret complex PDFs, web pages,
+docs, videos, data, and more ð§  - Auto-compress prompts exceeding your chosen
+token limit ð¦ - Works even with missing file extensions, in-memory data
+streams ð¾ - Works with codebases, git repos, and custom integrations ð -
+Multi-threaded â¡ï¸ ## Getting Started ð The Pipe handles a wide array of
+complex filetypes, and thus has many dependencies that must be installed
+separately. It also requires a strong machine for good response times. For this
+reason, we host it as an API that works out-of-the-box. First, install The
+Pipe. ``` pip install thepipe_api ``` The Pipe is available as a hosted API, or
+it can be set up locally. An API key is recommended for out-of-the-box
+functionality (alternatively, see the local installation section). Ensure the
+`THEPIPE_API_KEY` environment variable is set. Don't have a key yet? [Get one
+here](https://thepi.pe). Now you can extract comprehensive text and visuals
+from any file: ```python from thepipe_api import thepipe messages =
+thepipe.extract("example.pdf") ``` Or websites: ```python messages =
+thepipe.extract("https://example.com") ``` Then feed it into GPT-4-Vision:
+```python response = client.chat.completions.create( model="gpt-4-vision-
+preview", messages = messages, ) ``` ![Just call OpenAI](https://
+rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/IMG_0180.jpg)
+You can also use The Pipe from the command line. Here's how to recursively
+extract from a directory, matching only files containing a substring (in this
+example, typescript files) and ignore files containing other substrings (in
+this example, anything in the "tests" folder): ```bash thepipe path/to/folder -
+-match tsx --ignore tests ``` ## Supported File Types ð | Source Type |
+Input types | Token Compression ðï¸ | Image Extraction ðï¸ | Notes ð
+| |---------------------------------------|------------------------------------
+------|-------------------|------------------|---------------------------------
+------------------------| | Directory | Any `/path/to/directory` | âï¸ |
+âï¸ | Extracts from all files in directory, supports match and ignore
+patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | âï¸
+(varies) | â | Combines all code files. `.c`, `.cpp`, `.py` are compressible
+with ctags, others are not | | Plaintext | `.txt`, `.md`, `.rtf`, etc | âï¸
+| â | Regular text files | | PDF | `.pdf` | âï¸ | âï¸ | Extracts text
+and images of each page; can use AI for extraction of table data and images
+within pages | | Image | `.jpg`, `.jpeg`, `.png` | â | âï¸ | Extracts
+images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx` | âï¸
+| â | Extracts data from spreadsheets; converts to text representation. For
+very large datasets, will only extract column names and types | | Jupyter
+Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown, and images from
+Jupyter notebooks | | Microsoft Word Document | `.docx` | âï¸ | âï¸ |
+Extracts text and images from Word documents | | Microsoft PowerPoint
+Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images from
+PowerPoint presentations | | Video | `.mp4`, `.avi`, `.mov`, `.wmv` | âï¸ |
+âï¸ | Extracts frames from video files; supports frame extraction and OCR
+for text extraction from frames | | Audio | `.mp3`, `.wav` | âï¸ | â |
+Extracts text from audio files; supports speech-to-text conversion | | Website
+| URLs (inputs containing `http`, `https`, `ftp`) | âï¸ | âï¸ | Extracts
+text from web page along with image (or images if scrollable); text-only
+extraction available | | GitHub Repository | GitHub repo URLs | âï¸ | âï¸
+| Extracts from GitHub repositories; supports branch specification | | YouTube
+Video | YouTube video URLs | âï¸ | âï¸ | Extracts text from YouTube
+videos; supports subtitles extraction | | ZIP File | `.zip` | âï¸ | âï¸ |
+Extracts contents of ZIP files; supports nested directory extraction | ## How
+it works ð ï¸ The input source is either a file path, a URL, or a directory.
+The pipe will extract information from the source and process it for downstream
+use with [language models](https://en.wikipedia.org/wiki/Large_language_model),
+[vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or
+[vision-language models](https://arxiv.org/abs/2304.00685). The output from the
+pipe is a sensible list of multimodal messages representing chunks of the
+extracted information, carefully crafted to fit within context windows for any
+models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4]
+(https://openai.com/gpt-4). The messages returned should look like this:
+```json [ { "role": "user", "content": [ { "type": "text", "text": "..." },
+{ "type": "image_url", "image_url": { "url": "data:image/jpeg;base64,..." } } ]
+} ] ``` If you want to feed these messages directly into the model, it is
+important to be mindful of the token limit. OpenAI does not allow too many
+images in the prompt (see discussion [here](https://community.openai.com/t/gpt-
+4-vision-maximum-amount-of-images/573110/6)), so long files should be extracted
+with `text_only=True` to avoid this issue, while long text files should either
+be compressed or embedded in a RAG framework. The text and images from these
+messages may also be prepared for a vector database with
+`thepipe.core.create_chunks_from_messages` or for downstream use with RAG
+frameworks. [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily
+integrate The Pipe with any LLM provider. It uses a variety of heuristics for
+optimal performance with vision-language models, including AI filetype
+detection with [filetype detection](https://opensource.googleblog.com/2024/02/
+magika-ai-powered-fast-and-efficient-file-type-identification.html), opt-in AI
+[table, equation, and figure extraction](https://thepi.pe/pricing), efficient
+[token compression](https://arxiv.org/abs/2403.12968), automatic [image
+encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/
+abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172)
+effects, and more, all pre-built to work out-of-the-box. ![Demo](https://
+rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/grader.py%20
+(6).png) ## Local Installation ð ï¸ The Pipe handles a wide array of complex
+filetypes, and thus requires installation of many different packages to
 function. It also requires a very capable machine for good response times. For
 this reason, we host it as an API that works out-of-the-box. To use The Pipe
 locally for free instead, you will need [playwright](https://github.com/
 microsoft/playwright), [ctags](https://github.com/universal-ctags/),
 [pytesseract](https://github.com/h/pytesseract), and the local python
 requirements, which differ from the more lightweight API requirements: ```bash
 git clone https://github.com/emcf/thepipe pip install -r requirements_local.txt
```

### Comparing `thepipe_api-0.3.2/README.md` & `thepipe_api-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -45,628 +45,683 @@
 000002c0: 3246 2532 4674 6865 7069 7065 2e75 702e  2F%2Fthepipe.up.
 000002d0: 7261 696c 7761 792e 6170 7025 3246 266c  railway.app%2F&l
 000002e0: 6162 656c 3d41 5049 2532 3073 7461 7475  abel=API%20statu
 000002f0: 7329 3c2f 613e 203c 6120 6872 6566 3d22  s)</a> <a href="
 00000300: 6874 7470 733a 2f2f 7468 6570 692e 7065  https://thepi.pe
 00000310: 2f22 3e21 5b67 6574 2041 5049 5d28 6874  /">![get API](ht
 00000320: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000330: 732e 696f 2f62 6164 6765 2f41 5049 2d67  s.io/badge/API-g
-00000340: 6574 2532 3061 6363 6573 732d 626c 7565  et%20access-blue
-00000350: 293c 2f61 3e0d 0a0d 0a23 2323 2046 6565  )</a>....### Fee
-00000360: 6420 5044 4673 2c20 776f 7264 2064 6f63  d PDFs, word doc
-00000370: 732c 2073 6c69 6465 732c 2077 6562 2070  s, slides, web p
-00000380: 6167 6573 2061 6e64 206d 6f72 6520 696e  ages and more in
-00000390: 746f 2056 6973 696f 6e2d 4c4c 4d73 2077  to Vision-LLMs w
-000003a0: 6974 6820 6f6e 6520 6c69 6e65 206f 6620  ith one line of 
-000003b0: 636f 6465 20e2 9aa1 0d0a 0d0a 5468 6520  code .......The 
-000003c0: 5069 7065 2069 7320 6120 6d75 6c74 696d  Pipe is a multim
-000003d0: 6f64 616c 2d66 6972 7374 2074 6f6f 6c20  odal-first tool 
-000003e0: 666f 7220 6665 6564 696e 6720 6669 6c65  for feeding file
-000003f0: 7320 616e 6420 7765 6220 7061 6765 7320  s and web pages 
-00000400: 696e 746f 2076 6973 696f 6e2d 6c61 6e67  into vision-lang
-00000410: 7561 6765 206d 6f64 656c 7320 7375 6368  uage models such
-00000420: 2061 7320 4750 542d 3456 2e20 4974 2069   as GPT-4V. It i
-00000430: 7320 6265 7374 2066 6f72 204c 4c4d 2061  s best for LLM a
-00000440: 6e64 2052 4147 2061 7070 6c69 6361 7469  nd RAG applicati
-00000450: 6f6e 7320 7468 6174 2072 6571 7569 7265  ons that require
-00000460: 2061 2064 6565 7020 756e 6465 7273 7461   a deep understa
-00000470: 6e64 696e 6720 6f66 2074 7269 636b 7920  nding of tricky 
-00000480: 6461 7461 2073 6f75 7263 6573 2e20 5468  data sources. Th
-00000490: 6520 5069 7065 2069 7320 6176 6169 6c61  e Pipe is availa
-000004a0: 626c 6520 6173 2061 2068 6f73 7465 6420  ble as a hosted 
-000004b0: 4150 4920 6174 205b 7468 6570 692e 7065  API at [thepi.pe
-000004c0: 5d28 6874 7470 733a 2f2f 7468 6570 692e  ](https://thepi.
-000004d0: 7065 292c 206f 7220 6974 2063 616e 2062  pe), or it can b
-000004e0: 6520 7365 7420 7570 206c 6f63 616c 6c79  e set up locally
-000004f0: 2e20 0d0a 0d0a 215b 4465 6d6f 5d28 6874  . ....![Demo](ht
-00000500: 7470 733a 2f2f 7270 6e75 747a 656d 7574  tps://rpnutzemut
-00000510: 6272 756d 637a 7776 7565 2e73 7570 6162  brumczwvue.supab
-00000520: 6173 652e 636f 2f73 746f 7261 6765 2f76  ase.co/storage/v
-00000530: 312f 6f62 6a65 6374 2f70 7562 6c69 632f  1/object/public/
-00000540: 6173 7365 7473 2f67 7261 6465 722e 7079  assets/grader.py
-00000550: 2532 3028 3629 2e70 6e67 290d 0a0d 0a23  %20(6).png)....#
-00000560: 2320 4665 6174 7572 6573 20f0 9f8c 9f0d  # Features .....
-00000570: 0a0d 0a2d 2045 7874 7261 6374 7320 7465  ...- Extracts te
-00000580: 7874 2061 6e64 2076 6973 7561 6c73 2066  xt and visuals f
-00000590: 726f 6d20 6669 6c65 7320 6f72 2077 6562  rom files or web
-000005a0: 2070 6167 6573 20f0 9f93 9a0d 0a2d 204f   pages ......- O
-000005b0: 7574 7075 7473 2063 6875 6e6b 7320 6f70  utputs chunks op
-000005c0: 7469 6d69 7a65 6420 666f 7220 6d75 6c74  timized for mult
-000005d0: 696d 6f64 616c 204c 4c4d 7320 f09f 96bc  imodal LLMs ....
-000005e0: efb8 8f0d 0a2d 2049 6e74 6572 7072 6574  .....- Interpret
-000005f0: 2063 6f6d 706c 6578 2050 4446 732c 2077   complex PDFs, w
-00000600: 6562 2070 6167 6573 2c20 736c 6964 6573  eb pages, slides
-00000610: 2c20 4353 5673 2c20 616e 6420 6d6f 7265  , CSVs, and more
-00000620: 20f0 9fa7 a00d 0a2d 2041 7574 6f2d 636f   ......- Auto-co
-00000630: 6d70 7265 7373 2070 726f 6d70 7473 2065  mpress prompts e
-00000640: 7863 6565 6469 6e67 2079 6f75 7220 6368  xceeding your ch
-00000650: 6f73 656e 2074 6f6b 656e 206c 696d 6974  osen token limit
-00000660: 20f0 9f93 a60d 0a2d 2057 6f72 6b73 2065   ......- Works e
-00000670: 7665 6e20 7769 7468 206d 6973 7369 6e67  ven with missing
-00000680: 2066 696c 6520 6578 7465 6e73 696f 6e73   file extensions
-00000690: 2c20 696e 2d6d 656d 6f72 7920 6461 7461  , in-memory data
-000006a0: 2073 7472 6561 6d73 20f0 9f92 be0d 0a2d   streams ......-
-000006b0: 2057 6f72 6b73 2077 6974 6820 636f 6465   Works with code
-000006c0: 6261 7365 732c 2067 6974 2072 6570 6f73  bases, git repos
-000006d0: 2c20 616e 6420 6375 7374 6f6d 2069 6e74  , and custom int
-000006e0: 6567 7261 7469 6f6e 7320 f09f 8c90 0d0a  egrations ......
-000006f0: 2d20 4d75 6c74 692d 7468 7265 6164 6564  - Multi-threaded
-00000700: 20e2 9aa1 efb8 8f0d 0a0d 0a23 2320 4765   ..........## Ge
-00000710: 7474 696e 6720 5374 6172 7465 6420 20f0  tting Started  .
-00000720: 9f9a 800d 0a0d 0a54 6865 2050 6970 6520  .......The Pipe 
-00000730: 6861 6e64 6c65 7320 6120 7769 6465 2061  handles a wide a
-00000740: 7272 6179 206f 6620 636f 6d70 6c65 7820  rray of complex 
-00000750: 6669 6c65 7479 7065 732c 2061 6e64 2074  filetypes, and t
-00000760: 6875 7320 6861 7320 6d61 6e79 2064 6570  hus has many dep
-00000770: 656e 6465 6e63 6965 7320 7468 6174 206d  endencies that m
-00000780: 7573 7420 6265 2069 6e73 7461 6c6c 6564  ust be installed
-00000790: 2073 6570 6172 6174 656c 792e 2049 7420   separately. It 
-000007a0: 616c 736f 2072 6571 7569 7265 7320 6120  also requires a 
-000007b0: 7374 726f 6e67 206d 6163 6869 6e65 2066  strong machine f
-000007c0: 6f72 2067 6f6f 6420 7265 7370 6f6e 7365  or good response
-000007d0: 2074 696d 6573 2e20 466f 7220 7468 6973   times. For this
-000007e0: 2072 6561 736f 6e2c 2077 6520 686f 7374   reason, we host
-000007f0: 2069 7420 6173 2061 6e20 4150 4920 7468   it as an API th
-00000800: 6174 2077 6f72 6b73 206f 7574 2d6f 662d  at works out-of-
-00000810: 7468 652d 626f 782e 200d 0a0d 0a46 6972  the-box. ....Fir
-00000820: 7374 2c20 696e 7374 616c 6c20 5468 6520  st, install The 
-00000830: 5069 7065 2e20 0d0a 6060 600d 0a70 6970  Pipe. ..```..pip
-00000840: 2069 6e73 7461 6c6c 2074 6865 7069 7065   install thepipe
-00000850: 5f61 7069 0d0a 6060 600d 0a0d 0a54 6865  _api..```....The
-00000860: 2050 6970 6520 6973 2061 7661 696c 6162   Pipe is availab
-00000870: 6c65 2061 7320 6120 686f 7374 6564 2041  le as a hosted A
-00000880: 5049 2c20 6f72 2069 7420 6361 6e20 6265  PI, or it can be
-00000890: 2073 6574 2075 7020 6c6f 6361 6c6c 792e   set up locally.
-000008a0: 2041 6e20 4150 4920 6b65 7920 6973 2072   An API key is r
-000008b0: 6563 6f6d 6d65 6e64 6564 2066 6f72 206f  ecommended for o
-000008c0: 7574 2d6f 662d 7468 652d 626f 7820 6675  ut-of-the-box fu
-000008d0: 6e63 7469 6f6e 616c 6974 7920 2861 6c74  nctionality (alt
-000008e0: 6572 6e61 7469 7665 6c79 2c20 7365 6520  ernatively, see 
-000008f0: 7468 6520 6c6f 6361 6c20 696e 7374 616c  the local instal
-00000900: 6c61 7469 6f6e 2073 6563 7469 6f6e 292e  lation section).
-00000910: 2045 6e73 7572 6520 7468 6520 6054 4845   Ensure the `THE
-00000920: 5049 5045 5f41 5049 5f4b 4559 6020 656e  PIPE_API_KEY` en
-00000930: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00000940: 6c65 2069 7320 7365 742e 2044 6f6e 2774  le is set. Don't
-00000950: 2068 6176 6520 6120 6b65 7920 7965 743f   have a key yet?
-00000960: 205b 4765 7420 6f6e 6520 6865 7265 5d28   [Get one here](
-00000970: 6874 7470 733a 2f2f 7468 6570 692e 7065  https://thepi.pe
-00000980: 292e 0d0a 0d0a 4e6f 7720 796f 7520 6361  ).....Now you ca
-00000990: 6e20 6578 7472 6163 7420 636f 6d70 7265  n extract compre
-000009a0: 6865 6e73 6976 6520 7465 7874 2061 6e64  hensive text and
-000009b0: 2076 6973 7561 6c73 2066 726f 6d20 616e   visuals from an
-000009c0: 7920 6669 6c65 3a0d 0a60 6060 7079 7468  y file:..```pyth
-000009d0: 6f6e 0d0a 6672 6f6d 2074 6865 7069 7065  on..from thepipe
-000009e0: 5f61 7069 2069 6d70 6f72 7420 7468 6570  _api import thep
-000009f0: 6970 650d 0a6d 6573 7361 6765 7320 3d20  ipe..messages = 
-00000a00: 7468 6570 6970 652e 6578 7472 6163 7428  thepipe.extract(
-00000a10: 2265 7861 6d70 6c65 2e70 6466 2229 0d0a  "example.pdf")..
-00000a20: 6060 600d 0a4f 7220 616e 7920 7765 6273  ```..Or any webs
-00000a30: 6974 653a 0d0a 6060 6070 7974 686f 6e0d  ite:..```python.
-00000a40: 0a6d 6573 7361 6765 7320 3d20 7468 6570  .messages = thep
-00000a50: 6970 652e 6578 7472 6163 7428 2268 7474  ipe.extract("htt
-00000a60: 7073 3a2f 2f65 7861 6d70 6c65 2e63 6f6d  ps://example.com
-00000a70: 2229 0d0a 6060 600d 0a54 6865 6e20 6665  ")..```..Then fe
-00000a80: 6564 2069 7420 696e 746f 2047 5054 2d34  ed it into GPT-4
-00000a90: 2d56 6973 696f 6e3a 0d0a 6060 6070 7974  -Vision:..```pyt
-00000aa0: 686f 6e0d 0a72 6573 706f 6e73 6520 3d20  hon..response = 
-00000ab0: 636c 6965 6e74 2e63 6861 742e 636f 6d70  client.chat.comp
-00000ac0: 6c65 7469 6f6e 732e 6372 6561 7465 280d  letions.create(.
-00000ad0: 0a20 2020 206d 6f64 656c 3d22 6770 742d  .    model="gpt-
-00000ae0: 342d 7669 7369 6f6e 2d70 7265 7669 6577  4-vision-preview
-00000af0: 222c 0d0a 2020 2020 6d65 7373 6167 6573  ",..    messages
-00000b00: 203d 206d 6573 7361 6765 732c 0d0a 290d   = messages,..).
-00000b10: 0a60 6060 0d0a 0d0a 215b 4a75 7374 2063  .```....![Just c
-00000b20: 616c 6c20 4f70 656e 4149 5d28 6874 7470  all OpenAI](http
-00000b30: 733a 2f2f 7270 6e75 747a 656d 7574 6272  s://rpnutzemutbr
-00000b40: 756d 637a 7776 7565 2e73 7570 6162 6173  umczwvue.supabas
-00000b50: 652e 636f 2f73 746f 7261 6765 2f76 312f  e.co/storage/v1/
-00000b60: 6f62 6a65 6374 2f70 7562 6c69 632f 6173  object/public/as
-00000b70: 7365 7473 2f49 4d47 5f30 3138 302e 6a70  sets/IMG_0180.jp
-00000b80: 6729 0d0a 0d0a 596f 7520 6361 6e20 616c  g)....You can al
-00000b90: 736f 2075 7365 2054 6865 2050 6970 6520  so use The Pipe 
-00000ba0: 6672 6f6d 2074 6865 2063 6f6d 6d61 6e64  from the command
-00000bb0: 206c 696e 652e 2048 6572 6527 7320 686f   line. Here's ho
-00000bc0: 7720 746f 2072 6563 7572 7369 7665 6c79  w to recursively
-00000bd0: 2065 7874 7261 6374 2066 726f 6d20 6120   extract from a 
-00000be0: 6469 7265 6374 6f72 792c 206d 6174 6368  directory, match
-00000bf0: 696e 6720 6f6e 6c79 2066 696c 6573 2063  ing only files c
-00000c00: 6f6e 7461 696e 696e 6720 6120 7375 6273  ontaining a subs
-00000c10: 7472 696e 6720 2869 6e20 7468 6973 2065  tring (in this e
-00000c20: 7861 6d70 6c65 2c20 7479 7065 7363 7269  xample, typescri
-00000c30: 7074 2066 696c 6573 2920 616e 6420 6967  pt files) and ig
-00000c40: 6e6f 7265 2066 696c 6573 2063 6f6e 7461  nore files conta
-00000c50: 696e 696e 6720 6f74 6865 7220 7375 6273  ining other subs
-00000c60: 7472 696e 6773 2028 696e 2074 6869 7320  trings (in this 
-00000c70: 6578 616d 706c 652c 2061 6e79 7468 696e  example, anythin
-00000c80: 6720 696e 2074 6865 2022 7465 7374 7322  g in the "tests"
-00000c90: 2066 6f6c 6465 7229 3a0d 0a60 6060 6261   folder):..```ba
-00000ca0: 7368 0d0a 7468 6570 6970 6520 7061 7468  sh..thepipe path
-00000cb0: 2f74 6f2f 666f 6c64 6572 202d 2d6d 6174  /to/folder --mat
-00000cc0: 6368 2074 7378 202d 2d69 676e 6f72 6520  ch tsx --ignore 
-00000cd0: 7465 7374 730d 0a60 6060 0d0a 0d0a 2323  tests..```....##
-00000ce0: 2053 7570 706f 7274 6564 2046 696c 6520   Supported File 
-00000cf0: 5479 7065 7320 f09f 939a 0d0a 0d0a 7c20  Types ........| 
-00000d00: 536f 7572 6365 2054 7970 6520 2020 2020  Source Type     
-00000d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d20: 2020 2020 2020 7c20 496e 7075 7420 7479        | Input ty
-00000d30: 7065 7320 2020 2020 2020 207c 2054 6f6b  pes        | Tok
-00000d40: 656e 2043 6f6d 7072 6573 7369 6f6e 20f0  en Compression .
-00000d50: 9f97 9cef b88f 207c 2049 6d61 6765 2045  ...... | Image E
-00000d60: 7874 7261 6374 696f 6e20 f09f 9181 efb8  xtraction ......
-00000d70: 8f20 7c20 4e6f 7465 7320 f09f 938c 2020  . | Notes ....  
-00000d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000db0: 7c0d 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |..|------------
-00000dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
-00000de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000330: 732e 696f 2f62 6164 6765 2f41 5049 2d61  s.io/badge/API-a
+00000340: 6363 6573 732d 626c 7565 293c 2f61 3e0d  ccess-blue)</a>.
+00000350: 0a0d 0a23 2323 2046 6565 6420 5044 4673  ...### Feed PDFs
+00000360: 2c20 7765 6220 7061 6765 732c 2077 6f72  , web pages, wor
+00000370: 6420 646f 6373 2c20 736c 6964 6573 2c20  d docs, slides, 
+00000380: 7669 6465 6f73 2c20 4353 562c 2061 6e64  videos, CSV, and
+00000390: 206d 6f72 6520 696e 746f 2056 6973 696f   more into Visio
+000003a0: 6e2d 4c4c 4d73 2077 6974 6820 6f6e 6520  n-LLMs with one 
+000003b0: 6c69 6e65 206f 6620 636f 6465 20e2 9aa1  line of code ...
+000003c0: 0d0a 0d0a 5468 6520 5069 7065 2069 7320  ....The Pipe is 
+000003d0: 6120 6d75 6c74 696d 6f64 616c 2d66 6972  a multimodal-fir
+000003e0: 7374 2074 6f6f 6c20 666f 7220 6665 6564  st tool for feed
+000003f0: 696e 6720 6669 6c65 7320 616e 6420 7765  ing files and we
+00000400: 6220 7061 6765 7320 696e 746f 2076 6973  b pages into vis
+00000410: 696f 6e2d 6c61 6e67 7561 6765 206d 6f64  ion-language mod
+00000420: 656c 7320 7375 6368 2061 7320 4750 542d  els such as GPT-
+00000430: 3456 2e20 4974 2069 7320 6265 7374 2066  4V. It is best f
+00000440: 6f72 204c 4c4d 2061 6e64 2052 4147 2061  or LLM and RAG a
+00000450: 7070 6c69 6361 7469 6f6e 7320 7468 6174  pplications that
+00000460: 2072 6571 7569 7265 2061 2064 6565 7020   require a deep 
+00000470: 756e 6465 7273 7461 6e64 696e 6720 6f66  understanding of
+00000480: 2074 7269 636b 7920 6461 7461 2073 6f75   tricky data sou
+00000490: 7263 6573 2e20 5468 6520 5069 7065 2069  rces. The Pipe i
+000004a0: 7320 6176 6169 6c61 626c 6520 6173 2061  s available as a
+000004b0: 2068 6f73 7465 6420 4150 4920 6174 205b   hosted API at [
+000004c0: 7468 6570 692e 7065 5d28 6874 7470 733a  thepi.pe](https:
+000004d0: 2f2f 7468 6570 692e 7065 292c 206f 7220  //thepi.pe), or 
+000004e0: 6974 2063 616e 2062 6520 7365 7420 7570  it can be set up
+000004f0: 206c 6f63 616c 6c79 2e20 0d0a 0d0a 215b   locally. ....![
+00000500: 5363 6965 6e63 6520 6173 7369 7374 616e  Science assistan
+00000510: 7420 6465 6d6f 5d28 6874 7470 733a 2f2f  t demo](https://
+00000520: 7270 6e75 747a 656d 7574 6272 756d 637a  rpnutzemutbrumcz
+00000530: 7776 7565 2e73 7570 6162 6173 652e 636f  wvue.supabase.co
+00000540: 2f73 746f 7261 6765 2f76 312f 6f62 6a65  /storage/v1/obje
+00000550: 6374 2f70 7562 6c69 632f 6173 7365 7473  ct/public/assets
+00000560: 2f73 6369 656e 6365 5f61 7373 6973 7461  /science_assista
+00000570: 6e74 7079 322e 706e 6729 0d0a 0d0a 0d0a  ntpy2.png)......
+00000580: 2323 2046 6561 7475 7265 7320 f09f 8c9f  ## Features ....
+00000590: 0d0a 0d0a 2d20 4578 7472 6163 7473 2074  ....- Extracts t
+000005a0: 6578 7420 616e 6420 7669 7375 616c 7320  ext and visuals 
+000005b0: 6672 6f6d 2066 696c 6573 206f 7220 7765  from files or we
+000005c0: 6220 7061 6765 7320 f09f 939a 0d0a 2d20  b pages ......- 
+000005d0: 4f75 7470 7574 7320 6368 756e 6b73 206f  Outputs chunks o
+000005e0: 7074 696d 697a 6564 2066 6f72 206d 756c  ptimized for mul
+000005f0: 7469 6d6f 6461 6c20 4c4c 4d73 2061 6e64  timodal LLMs and
+00000600: 2052 4147 2066 7261 6d65 776f 726b 7320   RAG frameworks 
+00000610: f09f 96bc efb8 8f0d 0a2d 2049 6e74 6572  .........- Inter
+00000620: 7072 6574 2063 6f6d 706c 6578 2050 4446  pret complex PDF
+00000630: 732c 2077 6562 2070 6167 6573 2c20 646f  s, web pages, do
+00000640: 6373 2c20 7669 6465 6f73 2c20 6461 7461  cs, videos, data
+00000650: 2c20 616e 6420 6d6f 7265 20f0 9fa7 a00d  , and more .....
+00000660: 0a2d 2041 7574 6f2d 636f 6d70 7265 7373  .- Auto-compress
+00000670: 2070 726f 6d70 7473 2065 7863 6565 6469   prompts exceedi
+00000680: 6e67 2079 6f75 7220 6368 6f73 656e 2074  ng your chosen t
+00000690: 6f6b 656e 206c 696d 6974 20f0 9f93 a60d  oken limit .....
+000006a0: 0a2d 2057 6f72 6b73 2065 7665 6e20 7769  .- Works even wi
+000006b0: 7468 206d 6973 7369 6e67 2066 696c 6520  th missing file 
+000006c0: 6578 7465 6e73 696f 6e73 2c20 696e 2d6d  extensions, in-m
+000006d0: 656d 6f72 7920 6461 7461 2073 7472 6561  emory data strea
+000006e0: 6d73 20f0 9f92 be0d 0a2d 2057 6f72 6b73  ms ......- Works
+000006f0: 2077 6974 6820 636f 6465 6261 7365 732c   with codebases,
+00000700: 2067 6974 2072 6570 6f73 2c20 616e 6420   git repos, and 
+00000710: 6375 7374 6f6d 2069 6e74 6567 7261 7469  custom integrati
+00000720: 6f6e 7320 f09f 8c90 0d0a 2d20 4d75 6c74  ons ......- Mult
+00000730: 692d 7468 7265 6164 6564 20e2 9aa1 efb8  i-threaded .....
+00000740: 8f0d 0a0d 0a23 2320 4765 7474 696e 6720  .....## Getting 
+00000750: 5374 6172 7465 6420 20f0 9f9a 800d 0a0d  Started  .......
+00000760: 0a54 6865 2050 6970 6520 6861 6e64 6c65  .The Pipe handle
+00000770: 7320 6120 7769 6465 2061 7272 6179 206f  s a wide array o
+00000780: 6620 636f 6d70 6c65 7820 6669 6c65 7479  f complex filety
+00000790: 7065 732c 2061 6e64 2074 6875 7320 6861  pes, and thus ha
+000007a0: 7320 6d61 6e79 2064 6570 656e 6465 6e63  s many dependenc
+000007b0: 6965 7320 7468 6174 206d 7573 7420 6265  ies that must be
+000007c0: 2069 6e73 7461 6c6c 6564 2073 6570 6172   installed separ
+000007d0: 6174 656c 792e 2049 7420 616c 736f 2072  ately. It also r
+000007e0: 6571 7569 7265 7320 6120 7374 726f 6e67  equires a strong
+000007f0: 206d 6163 6869 6e65 2066 6f72 2067 6f6f   machine for goo
+00000800: 6420 7265 7370 6f6e 7365 2074 696d 6573  d response times
+00000810: 2e20 466f 7220 7468 6973 2072 6561 736f  . For this reaso
+00000820: 6e2c 2077 6520 686f 7374 2069 7420 6173  n, we host it as
+00000830: 2061 6e20 4150 4920 7468 6174 2077 6f72   an API that wor
+00000840: 6b73 206f 7574 2d6f 662d 7468 652d 626f  ks out-of-the-bo
+00000850: 782e 200d 0a0d 0a46 6972 7374 2c20 696e  x. ....First, in
+00000860: 7374 616c 6c20 5468 6520 5069 7065 2e20  stall The Pipe. 
+00000870: 0d0a 6060 600d 0a70 6970 2069 6e73 7461  ..```..pip insta
+00000880: 6c6c 2074 6865 7069 7065 5f61 7069 0d0a  ll thepipe_api..
+00000890: 6060 600d 0a0d 0a54 6865 2050 6970 6520  ```....The Pipe 
+000008a0: 6973 2061 7661 696c 6162 6c65 2061 7320  is available as 
+000008b0: 6120 686f 7374 6564 2041 5049 2c20 6f72  a hosted API, or
+000008c0: 2069 7420 6361 6e20 6265 2073 6574 2075   it can be set u
+000008d0: 7020 6c6f 6361 6c6c 792e 2041 6e20 4150  p locally. An AP
+000008e0: 4920 6b65 7920 6973 2072 6563 6f6d 6d65  I key is recomme
+000008f0: 6e64 6564 2066 6f72 206f 7574 2d6f 662d  nded for out-of-
+00000900: 7468 652d 626f 7820 6675 6e63 7469 6f6e  the-box function
+00000910: 616c 6974 7920 2861 6c74 6572 6e61 7469  ality (alternati
+00000920: 7665 6c79 2c20 7365 6520 7468 6520 6c6f  vely, see the lo
+00000930: 6361 6c20 696e 7374 616c 6c61 7469 6f6e  cal installation
+00000940: 2073 6563 7469 6f6e 292e 2045 6e73 7572   section). Ensur
+00000950: 6520 7468 6520 6054 4845 5049 5045 5f41  e the `THEPIPE_A
+00000960: 5049 5f4b 4559 6020 656e 7669 726f 6e6d  PI_KEY` environm
+00000970: 656e 7420 7661 7269 6162 6c65 2069 7320  ent variable is 
+00000980: 7365 742e 2044 6f6e 2774 2068 6176 6520  set. Don't have 
+00000990: 6120 6b65 7920 7965 743f 205b 4765 7420  a key yet? [Get 
+000009a0: 6f6e 6520 6865 7265 5d28 6874 7470 733a  one here](https:
+000009b0: 2f2f 7468 6570 692e 7065 292e 0d0a 0d0a  //thepi.pe).....
+000009c0: 4e6f 7720 796f 7520 6361 6e20 6578 7472  Now you can extr
+000009d0: 6163 7420 636f 6d70 7265 6865 6e73 6976  act comprehensiv
+000009e0: 6520 7465 7874 2061 6e64 2076 6973 7561  e text and visua
+000009f0: 6c73 2066 726f 6d20 616e 7920 6669 6c65  ls from any file
+00000a00: 3a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  :..```python..fr
+00000a10: 6f6d 2074 6865 7069 7065 5f61 7069 2069  om thepipe_api i
+00000a20: 6d70 6f72 7420 7468 6570 6970 650d 0a6d  mport thepipe..m
+00000a30: 6573 7361 6765 7320 3d20 7468 6570 6970  essages = thepip
+00000a40: 652e 6578 7472 6163 7428 2265 7861 6d70  e.extract("examp
+00000a50: 6c65 2e70 6466 2229 0d0a 6060 600d 0a4f  le.pdf")..```..O
+00000a60: 7220 7765 6273 6974 6573 3a0d 0a60 6060  r websites:..```
+00000a70: 7079 7468 6f6e 0d0a 6d65 7373 6167 6573  python..messages
+00000a80: 203d 2074 6865 7069 7065 2e65 7874 7261   = thepipe.extra
+00000a90: 6374 2822 6874 7470 733a 2f2f 6578 616d  ct("https://exam
+00000aa0: 706c 652e 636f 6d22 290d 0a60 6060 0d0a  ple.com")..```..
+00000ab0: 5468 656e 2066 6565 6420 6974 2069 6e74  Then feed it int
+00000ac0: 6f20 4750 542d 342d 5669 7369 6f6e 3a0d  o GPT-4-Vision:.
+00000ad0: 0a60 6060 7079 7468 6f6e 0d0a 7265 7370  .```python..resp
+00000ae0: 6f6e 7365 203d 2063 6c69 656e 742e 6368  onse = client.ch
+00000af0: 6174 2e63 6f6d 706c 6574 696f 6e73 2e63  at.completions.c
+00000b00: 7265 6174 6528 0d0a 2020 2020 6d6f 6465  reate(..    mode
+00000b10: 6c3d 2267 7074 2d34 2d76 6973 696f 6e2d  l="gpt-4-vision-
+00000b20: 7072 6576 6965 7722 2c0d 0a20 2020 206d  preview",..    m
+00000b30: 6573 7361 6765 7320 3d20 6d65 7373 6167  essages = messag
+00000b40: 6573 2c0d 0a29 0d0a 6060 600d 0a0d 0a21  es,..)..```....!
+00000b50: 5b4a 7573 7420 6361 6c6c 204f 7065 6e41  [Just call OpenA
+00000b60: 495d 2868 7474 7073 3a2f 2f72 706e 7574  I](https://rpnut
+00000b70: 7a65 6d75 7462 7275 6d63 7a77 7675 652e  zemutbrumczwvue.
+00000b80: 7375 7061 6261 7365 2e63 6f2f 7374 6f72  supabase.co/stor
+00000b90: 6167 652f 7631 2f6f 626a 6563 742f 7075  age/v1/object/pu
+00000ba0: 626c 6963 2f61 7373 6574 732f 494d 475f  blic/assets/IMG_
+00000bb0: 3031 3830 2e6a 7067 290d 0a0d 0a59 6f75  0180.jpg)....You
+00000bc0: 2063 616e 2061 6c73 6f20 7573 6520 5468   can also use Th
+00000bd0: 6520 5069 7065 2066 726f 6d20 7468 6520  e Pipe from the 
+00000be0: 636f 6d6d 616e 6420 6c69 6e65 2e20 4865  command line. He
+00000bf0: 7265 2773 2068 6f77 2074 6f20 7265 6375  re's how to recu
+00000c00: 7273 6976 656c 7920 6578 7472 6163 7420  rsively extract 
+00000c10: 6672 6f6d 2061 2064 6972 6563 746f 7279  from a directory
+00000c20: 2c20 6d61 7463 6869 6e67 206f 6e6c 7920  , matching only 
+00000c30: 6669 6c65 7320 636f 6e74 6169 6e69 6e67  files containing
+00000c40: 2061 2073 7562 7374 7269 6e67 2028 696e   a substring (in
+00000c50: 2074 6869 7320 6578 616d 706c 652c 2074   this example, t
+00000c60: 7970 6573 6372 6970 7420 6669 6c65 7329  ypescript files)
+00000c70: 2061 6e64 2069 676e 6f72 6520 6669 6c65   and ignore file
+00000c80: 7320 636f 6e74 6169 6e69 6e67 206f 7468  s containing oth
+00000c90: 6572 2073 7562 7374 7269 6e67 7320 2869  er substrings (i
+00000ca0: 6e20 7468 6973 2065 7861 6d70 6c65 2c20  n this example, 
+00000cb0: 616e 7974 6869 6e67 2069 6e20 7468 6520  anything in the 
+00000cc0: 2274 6573 7473 2220 666f 6c64 6572 293a  "tests" folder):
+00000cd0: 0d0a 6060 6062 6173 680d 0a74 6865 7069  ..```bash..thepi
+00000ce0: 7065 2070 6174 682f 746f 2f66 6f6c 6465  pe path/to/folde
+00000cf0: 7220 2d2d 6d61 7463 6820 7473 7820 2d2d  r --match tsx --
+00000d00: 6967 6e6f 7265 2074 6573 7473 0d0a 6060  ignore tests..``
+00000d10: 600d 0a0d 0a0d 0a23 2320 5375 7070 6f72  `......## Suppor
+00000d20: 7465 6420 4669 6c65 2054 7970 6573 20f0  ted File Types .
+00000d30: 9f93 9a0d 0a0d 0a7c 2053 6f75 7263 6520  .......| Source 
+00000d40: 5479 7065 2020 2020 2020 2020 2020 2020  Type            
+00000d50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00000d60: 2049 6e70 7574 2074 7970 6573 2020 2020   Input types    
+00000d70: 2020 2020 7c20 546f 6b65 6e20 436f 6d70      | Token Comp
+00000d80: 7265 7373 696f 6e20 f09f 979c efb8 8f20  ression ....... 
+00000d90: 7c20 496d 6167 6520 4578 7472 6163 7469  | Image Extracti
+00000da0: 6f6e 20f0 9f91 81ef b88f 207c 204e 6f74  on ....... | Not
+00000db0: 6573 20f0 9f93 8c20 2020 2020 2020 2020  es ....         
+00000dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000de0: 2020 2020 2020 2020 207c 0d0a 7c2d 2d2d           |..|---
 00000df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e00: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00000e10: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
-00000e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
-00000e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e10: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
+00000e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
 00000e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e60: 2d2d 2d2d 2d2d 2d7c 0d0a 7c20 4469 7265  -------|..| Dire
-00000e70: 6374 6f72 7920 2020 2020 2020 2020 2020  ctory           
-00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e90: 2020 7c20 416e 7920 602f 7061 7468 2f74    | Any `/path/t
-00000ea0: 6f2f 6469 7265 6374 6f72 7960 2020 2020  o/directory`    
-00000eb0: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
-00000ec0: 9c94 efb8 8f20 2020 2020 2020 2020 2020  .....           
-00000ed0: 2020 2020 7c20 e29c 94ef b88f 2020 2020      | ......    
-00000ee0: 2020 2020 2020 2020 2020 207c 2045 7874             | Ext
-00000ef0: 7261 6374 7320 6672 6f6d 2061 6c6c 2066  racts from all f
-00000f00: 696c 6573 2069 6e20 6469 7265 6374 6f72  iles in director
-00000f10: 792c 2073 7570 706f 7274 7320 6d61 7463  y, supports matc
-00000f20: 6820 616e 6420 6967 6e6f 7265 2070 6174  h and ignore pat
-00000f30: 7465 726e 7320 7c0d 0a7c 2043 6f64 6520  terns |..| Code 
-00000f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f60: 207c 2060 2e70 7960 2c20 602e 7473 7860   | `.py`, `.tsx`
-00000f70: 2c20 602e 6a73 602c 2060 2e68 746d 6c60  , `.js`, `.html`
-00000f80: 2c20 602e 6373 7360 2c20 602e 6370 7060  , `.css`, `.cpp`
-00000f90: 2c20 6574 6320 7c20 e29c 94ef b88f 2028  , etc | ...... (
-00000fa0: 7661 7269 6573 2920 2020 7c20 e29d 8c20  varies)   | ... 
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00000fc0: 436f 6d62 696e 6573 2061 6c6c 2063 6f64  Combines all cod
-00000fd0: 6520 6669 6c65 732e 2060 2e63 602c 2060  e files. `.c`, `
-00000fe0: 2e63 7070 602c 2060 2e70 7960 2061 7265  .cpp`, `.py` are
-00000ff0: 2063 6f6d 7072 6573 7369 626c 6520 7769   compressible wi
-00001000: 7468 2063 7461 6773 2c20 6f74 6865 7273  th ctags, others
-00001010: 2061 7265 206e 6f74 207c 0d0a 7c20 506c   are not |..| Pl
-00001020: 6169 6e74 6578 7420 2020 2020 2020 2020  aintext         
-00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001040: 2020 2020 7c20 602e 7478 7460 2c20 602e      | `.txt`, `.
-00001050: 6d64 602c 2060 2e72 7466 602c 2065 7463  md`, `.rtf`, etc
-00001060: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001070: 20e2 9c94 efb8 8f20 2020 2020 2020 2020   ......         
-00001080: 2020 2020 2020 7c20 e29d 8c20 2020 2020        | ...     
-00001090: 2020 2020 2020 2020 2020 7c20 5265 6775            | Regu
-000010a0: 6c61 7220 7465 7874 2066 696c 6573 2020  lar text files  
-000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010e0: 2020 2020 7c0d 0a7c 2050 4446 2020 2020      |..| PDF    
+00000e50: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
+00000e60: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
+00000e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ea0: 7c0d 0a7c 2044 6972 6563 746f 7279 2020  |..| Directory  
+00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ec0: 2020 2020 2020 2020 2020 207c 2041 6e79             | Any
+00000ed0: 2060 2f70 6174 682f 746f 2f64 6972 6563   `/path/to/direc
+00000ee0: 746f 7279 6020 2020 2020 2020 2020 2020  tory`           
+00000ef0: 2020 2020 2020 7c20 e29c 94ef b88f 2020        | ......  
+00000f00: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+00000f10: 9c94 efb8 8f20 2020 2020 2020 2020 2020  .....           
+00000f20: 2020 2020 7c20 4578 7472 6163 7473 2066      | Extracts f
+00000f30: 726f 6d20 616c 6c20 6669 6c65 7320 696e  rom all files in
+00000f40: 2064 6972 6563 746f 7279 2c20 7375 7070   directory, supp
+00000f50: 6f72 7473 206d 6174 6368 2061 6e64 2069  orts match and i
+00000f60: 676e 6f72 6520 7061 7474 6572 6e73 207c  gnore patterns |
+00000f70: 0d0a 7c20 436f 6465 2020 2020 2020 2020  ..| Code        
+00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f90: 2020 2020 2020 2020 2020 7c20 602e 7079            | `.py
+00000fa0: 602c 2060 2e74 7378 602c 2060 2e6a 7360  `, `.tsx`, `.js`
+00000fb0: 2c20 602e 6874 6d6c 602c 2060 2e63 7373  , `.html`, `.css
+00000fc0: 602c 2060 2e63 7070 602c 2065 7463 207c  `, `.cpp`, etc |
+00000fd0: 20e2 9c94 efb8 8f20 2876 6172 6965 7329   ...... (varies)
+00000fe0: 2020 207c 20e2 9d8c 2020 2020 2020 2020     | ...        
+00000ff0: 2020 2020 2020 207c 2043 6f6d 6269 6e65         | Combine
+00001000: 7320 616c 6c20 636f 6465 2066 696c 6573  s all code files
+00001010: 2e20 602e 6360 2c20 602e 6370 7060 2c20  . `.c`, `.cpp`, 
+00001020: 602e 7079 6020 6172 6520 636f 6d70 7265  `.py` are compre
+00001030: 7373 6962 6c65 2077 6974 6820 6374 6167  ssible with ctag
+00001040: 732c 206f 7468 6572 7320 6172 6520 6e6f  s, others are no
+00001050: 7420 7c0d 0a7c 2050 6c61 696e 7465 7874  t |..| Plaintext
+00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001070: 2020 2020 2020 2020 2020 2020 207c 2060               | `
+00001080: 2e74 7874 602c 2060 2e6d 6460 2c20 602e  .txt`, `.md`, `.
+00001090: 7274 6660 2c20 6574 6320 2020 2020 2020  rtf`, etc       
+000010a0: 2020 2020 2020 2020 7c20 e29c 94ef b88f          | ......
+000010b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000010c0: 20e2 9d8c 2020 2020 2020 2020 2020 2020   ...            
+000010d0: 2020 207c 2052 6567 756c 6172 2074 6578     | Regular tex
+000010e0: 7420 6669 6c65 7320 2020 2020 2020 2020  t files         
 000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001100: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001110: 2060 2e70 6466 6020 2020 2020 2020 2020   `.pdf`         
-00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001130: 2020 2020 2020 2020 207c 20e2 9c94 efb8           | .....
-00001140: 8f20 2020 2020 2020 2020 2020 2020 2020  .               
-00001150: 7c20 e29c 94ef b88f 2020 2020 7c20 4578  | ......    | Ex
-00001160: 7472 6163 7473 2074 6578 7420 616e 6420  tracts text and 
-00001170: 696d 6167 6573 206f 6620 6561 6368 2070  images of each p
-00001180: 6167 653b 2063 616e 2075 7365 2041 4920  age; can use AI 
-00001190: 666f 7220 6578 7472 6163 7469 6f6e 206f  for extraction o
-000011a0: 6620 7461 626c 6520 6461 7461 2061 6e64  f table data and
-000011b0: 2020 696d 6167 6573 2077 6974 6869 6e20    images within 
-000011c0: 7061 6765 7320 7c0d 0a7c 2049 6d61 6765  pages |..| Image
-000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011f0: 207c 2060 2e6a 7067 602c 2060 2e6a 7065   | `.jpg`, `.jpe
-00001200: 6760 2c20 602e 706e 6760 207c 20e2 9d8c  g`, `.png` | ...
+00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001110: 2020 2020 2020 2020 2020 2020 207c 0d0a               |..
+00001120: 7c20 5044 4620 2020 2020 2020 2020 2020  | PDF           
+00001130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001140: 2020 2020 2020 2020 7c20 602e 7064 6660          | `.pdf`
+00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
+00001180: 2020 2020 2020 2020 207c 20e2 9c94 efb8           | .....
+00001190: 8f20 2020 207c 2045 7874 7261 6374 7320  .    | Extracts 
+000011a0: 7465 7874 2061 6e64 2069 6d61 6765 7320  text and images 
+000011b0: 6f66 2065 6163 6820 7061 6765 3b20 6361  of each page; ca
+000011c0: 6e20 7573 6520 4149 2066 6f72 2065 7874  n use AI for ext
+000011d0: 7261 6374 696f 6e20 6f66 2074 6162 6c65  raction of table
+000011e0: 2064 6174 6120 616e 6420 2069 6d61 6765   data and  image
+000011f0: 7320 7769 7468 696e 2070 6167 6573 207c  s within pages |
+00001200: 0d0a 7c20 496d 6167 6520 2020 2020 2020  ..| Image       
 00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001220: 7c20 e29c 94ef b88f 2020 2020 2020 2020  | ......        
-00001230: 2020 2020 2020 7c20 4578 7472 6163 7473        | Extracts
-00001240: 2069 6d61 6765 732c 2075 7365 7320 4f43   images, uses OC
-00001250: 5220 6966 2074 6578 745f 6f6e 6c79 2020  R if text_only  
-00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001270: 2020 2020 2020 7c0d 0a7c 2044 6174 6120        |..| Data 
-00001280: 5461 626c 6520 2020 2020 2020 2020 2020  Table           
-00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012a0: 7c20 602e 6373 7660 2c20 602e 786c 7360  | `.csv`, `.xls`
-000012b0: 2c20 602e 786c 7378 6020 2020 2020 2020  , `.xlsx`       
-000012c0: 2020 2020 2020 7c20 e29c 94ef b88f 2020        | ......  
-000012d0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000012e0: e29d 8c20 2020 2020 2020 2020 2020 2020  ...             
-000012f0: 2020 7c20 4578 7472 6163 7473 2064 6174    | Extracts dat
-00001300: 6120 6672 6f6d 2073 7072 6561 6473 6865  a from spreadshe
-00001310: 6574 733b 2063 6f6e 7665 7274 7320 746f  ets; converts to
-00001320: 2074 6578 7420 7265 7072 6573 656e 7461   text representa
-00001330: 7469 6f6e 2e20 466f 7220 7665 7279 206c  tion. For very l
-00001340: 6172 6765 2064 6174 6173 6574 732c 2077  arge datasets, w
-00001350: 696c 6c20 6f6e 6c79 2065 7874 7261 6374  ill only extract
-00001360: 2063 6f6c 756d 6e20 6e61 6d65 7320 616e   column names an
-00001370: 6420 7479 7065 7320 2020 2020 2020 2020  d types         
-00001380: 7c0d 0a7c 204a 7570 7974 6572 204e 6f74  |..| Jupyter Not
-00001390: 6562 6f6f 6b20 2020 2020 2020 2020 2020  ebook           
-000013a0: 2020 2020 2020 2020 2020 207c 2060 2e69             | `.i
-000013b0: 7079 6e62 6020 2020 2020 2020 2020 2020  pynb`           
-000013c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013d0: 2020 2020 207c 20e2 9d8c 2020 2020 2020       | ...      
-000013e0: 2020 2020 2020 2020 207c 20e2 9c94 efb8           | .....
-000013f0: 8f20 2020 2020 2020 2020 2020 2020 2020  .               
-00001400: 7c20 4578 7472 6163 7473 2063 6f64 652c  | Extracts code,
-00001410: 206d 6172 6b64 6f77 6e2c 2061 6e64 2069   markdown, and i
-00001420: 6d61 6765 7320 6672 6f6d 204a 7570 7974  mages from Jupyt
-00001430: 6572 206e 6f74 6562 6f6f 6b73 2020 2020  er notebooks    
-00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001450: 2020 2020 2020 2020 2020 2020 2020 7c0d                |.
-00001460: 0a7c 204d 6963 726f 736f 6674 2057 6f72  .| Microsoft Wor
-00001470: 6420 446f 6375 6d65 6e74 2020 2020 2020  d Document      
-00001480: 2020 2020 2020 2020 207c 2060 2e64 6f63           | `.doc
-00001490: 7860 2020 2020 2020 2020 2020 2020 2020  x`              
-000014a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014b0: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
-000014c0: 2020 2020 2020 2020 2020 7c20 e29c 94ef            | ....
-000014d0: b88f 2020 2020 2020 2020 2020 2020 2020  ..              
-000014e0: 207c 2045 7874 7261 6374 7320 7465 7874   | Extracts text
-000014f0: 2061 6e64 2069 6d61 6765 7320 6672 6f6d   and images from
-00001500: 2057 6f72 6420 646f 6375 6d65 6e74 7320   Word documents 
-00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001530: 2020 2020 2020 207c 0d0a 7c20 4d69 6372         |..| Micr
-00001540: 6f73 6f66 7420 506f 7765 7250 6f69 6e74  osoft PowerPoint
-00001550: 2050 7265 7365 6e74 6174 696f 6e20 2020   Presentation   
-00001560: 2020 7c20 602e 7070 7478 6020 2020 2020    | `.pptx`     
-00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001580: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
-00001590: 94ef b88f 2020 2020 2020 2020 2020 2020  ....            
-000015a0: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
-000015b0: 2020 2020 2020 2020 2020 7c20 4578 7472            | Extr
-000015c0: 6163 7473 2074 6578 7420 616e 6420 696d  acts text and im
-000015d0: 6167 6573 2066 726f 6d20 506f 7765 7250  ages from PowerP
-000015e0: 6f69 6e74 2070 7265 7365 6e74 6174 696f  oint presentatio
-000015f0: 6e73 2020 2020 2020 2020 2020 2020 2020  ns              
-00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001610: 7c0d 0a7c 2057 6562 7369 7465 2020 2020  |..| Website    
-00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 2020 2020 2020 2020 2020 207c 2055 524c             | URL
-00001640: 7320 2869 6e70 7574 7320 636f 6e74 6169  s (inputs contai
-00001650: 6e69 6e67 2060 6874 7470 602c 2060 6874  ning `http`, `ht
-00001660: 7470 7360 2c20 6066 7470 6029 2020 2020  tps`, `ftp`)    
-00001670: 2020 2020 2020 2020 207c 20e2 9c94 efb8           | .....
-00001680: 8f20 2020 2020 2020 2020 2020 2020 2020  .               
-00001690: 207c 20e2 9c94 efb8 8f20 2020 207c 2045   | ......    | E
-000016a0: 7874 7261 6374 7320 7465 7874 2066 726f  xtracts text fro
-000016b0: 6d20 7765 6220 7061 6765 2061 6c6f 6e67  m web page along
-000016c0: 2077 6974 6820 696d 6167 6520 286f 7220   with image (or 
-000016d0: 696d 6167 6573 2069 6620 7363 726f 6c6c  images if scroll
-000016e0: 6162 6c65 293b 2074 6578 742d 6f6e 6c79  able); text-only
-000016f0: 2065 7874 7261 6374 696f 6e20 6176 6169   extraction avai
-00001700: 6c61 626c 6520 2020 2020 2020 2020 207c  lable          |
-00001710: 0d0a 7c20 4769 7448 7562 2052 6570 6f73  ..| GitHub Repos
-00001720: 6974 6f72 7920 2020 2020 2020 2020 2020  itory           
-00001730: 2020 2020 2020 2020 2020 7c20 4769 7448            | GitH
-00001740: 7562 2072 6570 6f20 5552 4c73 2020 2020  ub repo URLs    
-00001750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001760: 2020 2020 207c 20e2 9c94 efb8 8f20 2020       | ......   
-00001770: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
-00001780: 94ef b88f 2020 2020 2020 2020 2020 2020  ....            
-00001790: 2020 2020 7c20 4578 7472 6163 7473 2066      | Extracts f
-000017a0: 726f 6d20 4769 7448 7562 2072 6570 6f73  rom GitHub repos
-000017b0: 6974 6f72 6965 733b 2073 7570 706f 7274  itories; support
-000017c0: 7320 6272 616e 6368 2073 7065 6369 6669  s branch specifi
-000017d0: 6361 7469 6f6e 2020 2020 2020 2020 207c  cation         |
-000017e0: 0d0a 7c20 5a49 5020 4669 6c65 2020 2020  ..| ZIP File    
-000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001800: 2020 2020 2020 2020 2020 7c20 602e 7a69            | `.zi
-00001810: 7060 2020 2020 2020 2020 2020 2020 2020  p`              
-00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001830: 2020 2020 7c20 e29c 94ef b88f 2020 2020      | ......    
-00001840: 2020 2020 2020 2020 2020 207c 20e2 9c94             | ...
-00001850: efb8 8f20 2020 2020 2020 2020 2020 2020  ...             
-00001860: 2020 207c 2045 7874 7261 6374 7320 636f     | Extracts co
-00001870: 6e74 656e 7473 206f 6620 5a49 5020 6669  ntents of ZIP fi
-00001880: 6c65 733b 2073 7570 706f 7274 7320 6e65  les; supports ne
-00001890: 7374 6564 2064 6972 6563 746f 7279 2065  sted directory e
-000018a0: 7874 7261 6374 696f 6e20 2020 2020 7c0d  xtraction     |.
-000018b0: 0a0d 0a23 2320 486f 7720 6974 2077 6f72  ...## How it wor
-000018c0: 6b73 20f0 9f9b a0ef b88f 0d0a 0d0a 5468  ks ...........Th
-000018d0: 6520 696e 7075 7420 736f 7572 6365 2069  e input source i
-000018e0: 7320 6569 7468 6572 2061 2066 696c 6520  s either a file 
-000018f0: 7061 7468 2c20 6120 5552 4c2c 206f 7220  path, a URL, or 
-00001900: 6120 6469 7265 6374 6f72 792e 2054 6865  a directory. The
-00001910: 2070 6970 6520 7769 6c6c 2065 7874 7261   pipe will extra
-00001920: 6374 2069 6e66 6f72 6d61 7469 6f6e 2066  ct information f
-00001930: 726f 6d20 7468 6520 736f 7572 6365 2061  rom the source a
-00001940: 6e64 2070 726f 6365 7373 2069 7420 666f  nd process it fo
-00001950: 7220 646f 776e 7374 7265 616d 2075 7365  r downstream use
-00001960: 2077 6974 6820 5b6c 616e 6775 6167 6520   with [language 
-00001970: 6d6f 6465 6c73 5d28 6874 7470 733a 2f2f  models](https://
-00001980: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
-00001990: 2f77 696b 692f 4c61 7267 655f 6c61 6e67  /wiki/Large_lang
-000019a0: 7561 6765 5f6d 6f64 656c 292c 205b 7669  uage_model), [vi
-000019b0: 7369 6f6e 2074 7261 6e73 666f 726d 6572  sion transformer
-000019c0: 735d 2868 7474 7073 3a2f 2f65 6e2e 7769  s](https://en.wi
-000019d0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-000019e0: 2f56 6973 696f 6e5f 7472 616e 7366 6f72  /Vision_transfor
-000019f0: 6d65 7229 2c20 6f72 205b 7669 7369 6f6e  mer), or [vision
-00001a00: 2d6c 616e 6775 6167 6520 6d6f 6465 6c73  -language models
-00001a10: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
-00001a20: 6f72 672f 6162 732f 3233 3034 2e30 3036  org/abs/2304.006
-00001a30: 3835 292e 2054 6865 206f 7574 7075 7420  85). The output 
-00001a40: 6672 6f6d 2074 6865 2070 6970 6520 6973  from the pipe is
-00001a50: 2061 2073 656e 7369 626c 6520 6c69 7374   a sensible list
-00001a60: 206f 6620 6d75 6c74 696d 6f64 616c 206d   of multimodal m
-00001a70: 6573 7361 6765 7320 7265 7072 6573 656e  essages represen
-00001a80: 7469 6e67 2063 6875 6e6b 7320 6f66 2074  ting chunks of t
-00001a90: 6865 2065 7874 7261 6374 6564 2069 6e66  he extracted inf
-00001aa0: 6f72 6d61 7469 6f6e 2c20 6361 7265 6675  ormation, carefu
-00001ab0: 6c6c 7920 6372 6166 7465 6420 746f 2066  lly crafted to f
-00001ac0: 6974 2077 6974 6869 6e20 636f 6e74 6578  it within contex
-00001ad0: 7420 7769 6e64 6f77 7320 666f 7220 616e  t windows for an
-00001ae0: 7920 6d6f 6465 6c73 2066 726f 6d20 5b67  y models from [g
-00001af0: 656d 6d61 2d37 625d 2868 7474 7073 3a2f  emma-7b](https:/
-00001b00: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00001b10: 676f 6f67 6c65 2f67 656d 6d61 2d37 6229  google/gemma-7b)
-00001b20: 2074 6f20 5b47 5054 2d34 5d28 6874 7470   to [GPT-4](http
-00001b30: 733a 2f2f 6f70 656e 6169 2e63 6f6d 2f67  s://openai.com/g
-00001b40: 7074 2d34 292e 2054 6865 206d 6573 7361  pt-4). The messa
-00001b50: 6765 7320 7265 7475 726e 6564 2073 686f  ges returned sho
-00001b60: 756c 6420 6c6f 6f6b 206c 696b 6520 7468  uld look like th
-00001b70: 6973 3a0d 0a60 6060 6a73 6f6e 0d0a 5b0d  is:..```json..[.
-00001b80: 0a20 207b 0d0a 2020 2020 2272 6f6c 6522  .  {..    "role"
-00001b90: 3a20 2275 7365 7222 2c0d 0a20 2020 2022  : "user",..    "
-00001ba0: 636f 6e74 656e 7422 3a20 5b0d 0a20 2020  content": [..   
-00001bb0: 2020 207b 0d0a 2020 2020 2020 2020 2274     {..        "t
-00001bc0: 7970 6522 3a20 2274 6578 7422 2c0d 0a20  ype": "text",.. 
-00001bd0: 2020 2020 2020 2022 7465 7874 223a 2022         "text": "
-00001be0: 2e2e 2e22 0d0a 2020 2020 2020 7d2c 0d0a  ..."..      },..
-00001bf0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00001c00: 2022 7479 7065 223a 2022 696d 6167 655f   "type": "image_
-00001c10: 7572 6c22 2c0d 0a20 2020 2020 2020 2022  url",..        "
-00001c20: 696d 6167 655f 7572 6c22 3a20 7b0d 0a20  image_url": {.. 
-00001c30: 2020 2020 2020 2020 2022 7572 6c22 3a20           "url": 
-00001c40: 2264 6174 613a 696d 6167 652f 6a70 6567  "data:image/jpeg
-00001c50: 3b62 6173 6536 342c 2e2e 2e22 0d0a 2020  ;base64,..."..  
-00001c60: 2020 2020 2020 7d0d 0a20 2020 2020 207d        }..      }
-00001c70: 0d0a 2020 2020 5d0d 0a20 207d 0d0a 5d0d  ..    ]..  }..].
-00001c80: 0a60 6060 0d0a 4966 2079 6f75 2077 616e  .```..If you wan
-00001c90: 7420 746f 2066 6565 6420 7468 6573 6520  t to feed these 
-00001ca0: 6d65 7373 6167 6573 2064 6972 6563 746c  messages directl
-00001cb0: 7920 696e 746f 2074 6865 206d 6f64 656c  y into the model
-00001cc0: 2c20 6974 2069 7320 696d 706f 7274 616e  , it is importan
-00001cd0: 7420 746f 2062 6520 6d69 6e64 6675 6c20  t to be mindful 
-00001ce0: 6f66 2074 6865 2074 6f6b 656e 206c 696d  of the token lim
-00001cf0: 6974 2e0d 0a4f 7065 6e41 4920 646f 6573  it...OpenAI does
-00001d00: 206e 6f74 2061 6c6c 6f77 2074 6f6f 206d   not allow too m
-00001d10: 616e 7920 696d 6167 6573 2069 6e20 7468  any images in th
-00001d20: 6520 7072 6f6d 7074 2028 7365 6520 6469  e prompt (see di
-00001d30: 7363 7573 7369 6f6e 205b 6865 7265 5d28  scussion [here](
-00001d40: 6874 7470 733a 2f2f 636f 6d6d 756e 6974  https://communit
-00001d50: 792e 6f70 656e 6169 2e63 6f6d 2f74 2f67  y.openai.com/t/g
-00001d60: 7074 2d34 2d76 6973 696f 6e2d 6d61 7869  pt-4-vision-maxi
-00001d70: 6d75 6d2d 616d 6f75 6e74 2d6f 662d 696d  mum-amount-of-im
-00001d80: 6167 6573 2f35 3733 3131 302f 3629 292c  ages/573110/6)),
-00001d90: 2073 6f20 6c6f 6e67 2066 696c 6573 2073   so long files s
-00001da0: 686f 756c 6420 6265 2065 7874 7261 6374  hould be extract
-00001db0: 6564 2077 6974 6820 6074 6578 745f 6f6e  ed with `text_on
-00001dc0: 6c79 3d54 7275 6560 2074 6f20 6176 6f69  ly=True` to avoi
-00001dd0: 6420 7468 6973 2069 7373 7565 2e20 0d0a  d this issue. ..
-00001de0: 0d0a 5468 6520 7465 7874 2061 6e64 2069  ..The text and i
-00001df0: 6d61 6765 7320 6672 6f6d 2074 6865 7365  mages from these
-00001e00: 206d 6573 7361 6765 7320 6d61 7920 616c   messages may al
-00001e10: 736f 2062 6520 7072 6570 6172 6564 2066  so be prepared f
-00001e20: 6f72 2061 2076 6563 746f 7220 6461 7461  or a vector data
-00001e30: 6261 7365 2077 6974 6820 6074 6865 7069  base with `thepi
-00001e40: 7065 2e63 6f72 652e 6372 6561 7465 5f63  pe.core.create_c
-00001e50: 6875 6e6b 735f 6672 6f6d 5f6d 6573 7361  hunks_from_messa
-00001e60: 6765 7360 206f 7220 666f 7220 646f 776e  ges` or for down
-00001e70: 7374 7265 616d 2075 7365 2077 6974 6820  stream use with 
-00001e80: 5241 4720 6672 616d 6577 6f72 6b73 2e20  RAG frameworks. 
-00001e90: 5b4c 6974 654c 4c4d 5d28 6874 7470 733a  [LiteLLM](https:
-00001ea0: 2f2f 6769 7468 7562 2e63 6f6d 2f42 6572  //github.com/Ber
-00001eb0: 7269 4149 2f6c 6974 656c 6c6d 2920 6361  riAI/litellm) ca
-00001ec0: 6e20 6265 2075 7365 6420 746f 2065 6173  n be used to eas
-00001ed0: 696c 7920 696e 7465 6772 6174 6520 5468  ily integrate Th
-00001ee0: 6520 5069 7065 2077 6974 6820 616e 7920  e Pipe with any 
-00001ef0: 4c4c 4d20 7072 6f76 6964 6572 2e20 0d0a  LLM provider. ..
-00001f00: 0d0a 4974 2075 7365 7320 6120 7661 7269  ..It uses a vari
-00001f10: 6574 7920 6f66 2068 6575 7269 7374 6963  ety of heuristic
-00001f20: 7320 666f 7220 6f70 7469 6d61 6c20 7065  s for optimal pe
-00001f30: 7266 6f72 6d61 6e63 6520 7769 7468 2076  rformance with v
-00001f40: 6973 696f 6e2d 6c61 6e67 7561 6765 206d  ision-language m
-00001f50: 6f64 656c 732c 2069 6e63 6c75 6469 6e67  odels, including
-00001f60: 2041 4920 6669 6c65 7479 7065 2064 6574   AI filetype det
-00001f70: 6563 7469 6f6e 2077 6974 6820 5b66 696c  ection with [fil
-00001f80: 6574 7970 6520 6465 7465 6374 696f 6e5d  etype detection]
-00001f90: 2868 7474 7073 3a2f 2f6f 7065 6e73 6f75  (https://opensou
-00001fa0: 7263 652e 676f 6f67 6c65 626c 6f67 2e63  rce.googleblog.c
-00001fb0: 6f6d 2f32 3032 342f 3032 2f6d 6167 696b  om/2024/02/magik
-00001fc0: 612d 6169 2d70 6f77 6572 6564 2d66 6173  a-ai-powered-fas
-00001fd0: 742d 616e 642d 6566 6669 6369 656e 742d  t-and-efficient-
-00001fe0: 6669 6c65 2d74 7970 652d 6964 656e 7469  file-type-identi
-00001ff0: 6669 6361 7469 6f6e 2e68 746d 6c29 2c20  fication.html), 
-00002000: 6f70 742d 696e 2041 4920 5b74 6162 6c65  opt-in AI [table
-00002010: 2c20 6571 7561 7469 6f6e 2c20 616e 6420  , equation, and 
-00002020: 6669 6775 7265 2065 7874 7261 6374 696f  figure extractio
-00002030: 6e5d 2868 7474 7073 3a2f 2f74 6865 7069  n](https://thepi
-00002040: 2e70 652f 7072 6963 696e 6729 2c20 6566  .pe/pricing), ef
-00002050: 6669 6369 656e 7420 5b74 6f6b 656e 2063  ficient [token c
-00002060: 6f6d 7072 6573 7369 6f6e 5d28 6874 7470  ompression](http
-00002070: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-00002080: 732f 3234 3033 2e31 3239 3638 292c 2061  s/2403.12968), a
-00002090: 7574 6f6d 6174 6963 205b 696d 6167 6520  utomatic [image 
-000020a0: 656e 636f 6469 6e67 5d28 6874 7470 733a  encoding](https:
-000020b0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-000020c0: 7267 2f77 696b 692f 4261 7365 3634 292c  rg/wiki/Base64),
-000020d0: 205b 7265 7261 6e6b 696e 675d 2868 7474   [reranking](htt
-000020e0: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-000020f0: 6273 2f32 3331 302e 3036 3833 3929 2066  bs/2310.06839) f
-00002100: 6f72 205b 6c6f 7374 2d69 6e2d 7468 652d  or [lost-in-the-
-00002110: 6d69 6464 6c65 5d28 6874 7470 733a 2f2f  middle](https://
-00002120: 6172 7869 762e 6f72 672f 6162 732f 3233  arxiv.org/abs/23
-00002130: 3037 2e30 3331 3732 2920 6566 6665 6374  07.03172) effect
-00002140: 732c 2061 6e64 206d 6f72 652c 2061 6c6c  s, and more, all
-00002150: 2070 7265 2d62 7569 6c74 2074 6f20 776f   pre-built to wo
-00002160: 726b 206f 7574 2d6f 662d 7468 652d 626f  rk out-of-the-bo
-00002170: 782e 0d0a 0d0a 0d0a 2323 204c 6f63 616c  x.......## Local
-00002180: 2049 6e73 7461 6c6c 6174 696f 6e20 f09f   Installation ..
-00002190: 9ba0 efb8 8f0d 0a0d 0a54 6865 2050 6970  .........The Pip
-000021a0: 6520 6861 6e64 6c65 7320 6120 7769 6465  e handles a wide
-000021b0: 2061 7272 6179 206f 6620 636f 6d70 6c65   array of comple
-000021c0: 7820 6669 6c65 7479 7065 732c 2061 6e64  x filetypes, and
-000021d0: 2074 6875 7320 7265 7175 6972 6573 2069   thus requires i
-000021e0: 6e73 7461 6c6c 6174 696f 6e20 6f66 206d  nstallation of m
-000021f0: 616e 7920 6469 6666 6572 656e 7420 7061  any different pa
-00002200: 636b 6167 6573 2074 6f20 6675 6e63 7469  ckages to functi
-00002210: 6f6e 2e20 4974 2061 6c73 6f20 7265 7175  on. It also requ
-00002220: 6972 6573 2061 2076 6572 7920 6361 7061  ires a very capa
-00002230: 626c 6520 6d61 6368 696e 6520 666f 7220  ble machine for 
-00002240: 676f 6f64 2072 6573 706f 6e73 6520 7469  good response ti
-00002250: 6d65 732e 2046 6f72 2074 6869 7320 7265  mes. For this re
-00002260: 6173 6f6e 2c20 7765 2068 6f73 7420 6974  ason, we host it
-00002270: 2061 7320 616e 2041 5049 2074 6861 7420   as an API that 
-00002280: 776f 726b 7320 6f75 742d 6f66 2d74 6865  works out-of-the
-00002290: 2d62 6f78 2e20 546f 2075 7365 2054 6865  -box. To use The
-000022a0: 2050 6970 6520 6c6f 6361 6c6c 7920 666f   Pipe locally fo
-000022b0: 7220 6672 6565 2069 6e73 7465 6164 2c20  r free instead, 
-000022c0: 796f 7520 7769 6c6c 206e 6565 6420 5b70  you will need [p
-000022d0: 6c61 7977 7269 6768 745d 2868 7474 7073  laywright](https
-000022e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d69  ://github.com/mi
-000022f0: 6372 6f73 6f66 742f 706c 6179 7772 6967  crosoft/playwrig
-00002300: 6874 292c 205b 6374 6167 735d 2868 7474  ht), [ctags](htt
-00002310: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002320: 756e 6976 6572 7361 6c2d 6374 6167 732f  universal-ctags/
-00002330: 292c 205b 7079 7465 7373 6572 6163 745d  ), [pytesseract]
-00002340: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002350: 636f 6d2f 682f 7079 7465 7373 6572 6163  com/h/pytesserac
-00002360: 7429 2c20 616e 6420 7468 6520 6c6f 6361  t), and the loca
-00002370: 6c20 7079 7468 6f6e 2072 6571 7569 7265  l python require
-00002380: 6d65 6e74 732c 2077 6869 6368 2064 6966  ments, which dif
-00002390: 6665 7220 6672 6f6d 2074 6865 206d 6f72  fer from the mor
-000023a0: 6520 6c69 6768 7477 6569 6768 7420 4150  e lightweight AP
-000023b0: 4920 7265 7175 6972 656d 656e 7473 3a0d  I requirements:.
-000023c0: 0a0d 0a60 6060 6261 7368 0d0a 6769 7420  ...```bash..git 
-000023d0: 636c 6f6e 6520 6874 7470 733a 2f2f 6769  clone https://gi
-000023e0: 7468 7562 2e63 6f6d 2f65 6d63 662f 7468  thub.com/emcf/th
-000023f0: 6570 6970 650d 0a70 6970 2069 6e73 7461  epipe..pip insta
-00002400: 6c6c 202d 7220 7265 7175 6972 656d 656e  ll -r requiremen
-00002410: 7473 5f6c 6f63 616c 2e74 7874 0d0a 6060  ts_local.txt..``
-00002420: 600d 0a0d 0a54 6970 2066 6f72 2077 696e  `....Tip for win
-00002430: 646f 7773 2075 7365 7273 3a20 496e 7374  dows users: Inst
-00002440: 616c 6c20 7468 6520 7079 7468 6f6e 2d6c  all the python-l
-00002450: 6962 6d61 6769 6320 6269 6e61 7269 6573  ibmagic binaries
-00002460: 2077 6974 6820 6070 6970 2069 6e73 7461   with `pip insta
-00002470: 6c6c 2070 7974 686f 6e2d 6d61 6769 632d  ll python-magic-
-00002480: 6269 6e60 2e20 456e 7375 7265 2074 6865  bin`. Ensure the
-00002490: 2060 7465 7373 6572 6163 742d 6f63 7260   `tesseract-ocr`
-000024a0: 2062 696e 6172 6965 7320 616e 6420 7468   binaries and th
-000024b0: 6520 6063 7461 6773 6020 6269 6e61 7269  e `ctags` binari
-000024c0: 6573 2061 7265 2069 6e20 796f 7572 2050  es are in your P
-000024d0: 4154 482e 0d0a 0d0a 4e6f 7720 796f 7520  ATH.....Now you 
-000024e0: 6361 6e20 7573 6520 5468 6520 5069 7065  can use The Pipe
-000024f0: 2077 6974 6820 5079 7468 6f6e 3a0d 0a60   with Python:..`
-00002500: 6060 6261 7368 0d0a 6672 6f6d 2074 6865  ``bash..from the
-00002510: 7069 7065 5f61 7069 2069 6d70 6f72 7420  pipe_api import 
-00002520: 7468 6570 6970 650d 0a63 6875 6e6b 7320  thepipe..chunks 
-00002530: 3d20 7468 6570 6970 652e 6578 7472 6163  = thepipe.extrac
-00002540: 7428 2265 7861 6d70 6c65 2e70 6466 222c  t("example.pdf",
-00002550: 206c 6f63 616c 3d54 7275 6529 0d0a 6060   local=True)..``
-00002560: 600d 0a0d 0a6f 7220 6672 6f6d 2074 6865  `....or from the
-00002570: 2063 6f6d 6d61 6e64 206c 696e 653a 0d0a   command line:..
-00002580: 6060 6062 6173 680d 0a74 6865 7069 7065  ```bash..thepipe
-00002590: 2070 6174 682f 746f 2f66 6f6c 6465 7220   path/to/folder 
-000025a0: 2d2d 6c6f 6361 6c0d 0a60 6060 0d0a 0d0a  --local..```....
-000025b0: 4172 6775 6d65 6e74 7320 6172 653a 0d0a  Arguments are:..
-000025c0: 2d20 6073 6f75 7263 6560 2028 7265 7175  - `source` (requ
-000025d0: 6972 6564 293a 2063 616e 2062 6520 6120  ired): can be a 
-000025e0: 6669 6c65 2070 6174 682c 2061 2055 524c  file path, a URL
-000025f0: 2c20 6f72 2061 2064 6972 6563 746f 7279  , or a directory
-00002600: 2070 6174 682e 0d0a 2d20 606c 6f63 616c   path...- `local
-00002610: 6020 286f 7074 696f 6e61 6c29 3a20 5573  ` (optional): Us
-00002620: 6520 7468 6520 6c6f 6361 6c20 7665 7273  e the local vers
-00002630: 696f 6e20 6f66 2054 6865 2050 6970 6520  ion of The Pipe 
-00002640: 696e 7374 6561 6420 6f66 2074 6865 2068  instead of the h
-00002650: 6f73 7465 6420 4150 492e 0d0a 2d20 606d  osted API...- `m
-00002660: 6174 6368 6020 286f 7074 696f 6e61 6c29  atch` (optional)
-00002670: 3a20 5375 6273 7472 696e 6720 746f 206d  : Substring to m
-00002680: 6174 6368 2066 696c 6573 2069 6e20 7468  atch files in th
-00002690: 6520 6469 7265 6374 6f72 792e 2052 6567  e directory. Reg
-000026a0: 6578 2069 7320 6e6f 7420 7965 7420 7375  ex is not yet su
-000026b0: 7070 6f72 7465 642e 0d0a 2d20 6069 676e  pported...- `ign
-000026c0: 6f72 6560 2028 6f70 7469 6f6e 616c 293a  ore` (optional):
-000026d0: 2053 7562 7374 7269 6e67 2074 6f20 6967   Substring to ig
-000026e0: 6e6f 7265 2066 696c 6573 2069 6e20 7468  nore files in th
-000026f0: 6520 6469 7265 6374 6f72 792e 2052 6567  e directory. Reg
-00002700: 6578 2069 7320 6e6f 7420 7965 7420 7375  ex is not yet su
-00002710: 7070 6f72 7465 642e 0d0a 2d20 606c 696d  pported...- `lim
-00002720: 6974 6020 286f 7074 696f 6e61 6c29 3a20  it` (optional): 
-00002730: 5468 6520 746f 6b65 6e20 6c69 6d69 7420  The token limit 
-00002740: 666f 7220 7468 6520 6f75 7470 7574 2070  for the output p
-00002750: 726f 6d70 742c 2064 6566 6175 6c74 7320  rompt, defaults 
-00002760: 746f 2031 3030 4b2e 2050 726f 6d70 7473  to 100K. Prompts
-00002770: 2065 7863 6565 6469 6e67 2074 6865 206c   exceeding the l
-00002780: 696d 6974 2077 696c 6c20 6265 2063 6f6d  imit will be com
-00002790: 7072 6573 7365 642e 2054 6869 7320 6d61  pressed. This ma
-000027a0: 7920 6e6f 7420 776f 726b 2061 7320 6578  y not work as ex
-000027b0: 7065 6374 6564 2077 6974 6820 7468 6520  pected with the 
-000027c0: 4150 492c 2061 7320 6974 2069 7320 696e  API, as it is in
-000027d0: 2061 6374 6976 6520 6465 7665 6c6f 706d   active developm
-000027e0: 656e 742e 0d0a 2d20 6061 695f 6578 7472  ent...- `ai_extr
-000027f0: 6163 7469 6f6e 6020 286f 7074 696f 6e61  action` (optiona
-00002800: 6c29 3a20 4578 7472 6163 7420 7461 626c  l): Extract tabl
-00002810: 6573 2c20 6669 6775 7265 732c 2061 6e64  es, figures, and
-00002820: 206d 6174 6820 6672 6f6d 2050 4446 7320   math from PDFs 
-00002830: 7573 696e 6720 6f75 7220 6578 7472 6163  using our extrac
-00002840: 746f 722e 2049 6e63 7572 7320 6578 7472  tor. Incurs extr
-00002850: 6120 636f 7374 732e 0d0a 2d20 6074 6578  a costs...- `tex
-00002860: 745f 6f6e 6c79 6020 286f 7074 696f 6e61  t_only` (optiona
-00002870: 6c29 3a20 446f 206e 6f74 2065 7874 7261  l): Do not extra
-00002880: 6374 2069 6d61 6765 7320 6672 6f6d 2064  ct images from d
-00002890: 6f63 756d 656e 7473 206f 7220 7765 6273  ocuments or webs
-000028a0: 6974 6573 2e20 4164 6469 7469 6f6e 616c  ites. Additional
-000028b0: 6c79 2c20 696d 6167 6520 6669 6c65 7320  ly, image files 
-000028c0: 7769 6c6c 2062 6520 7265 7072 6573 656e  will be represen
-000028d0: 7465 6420 7769 7468 204f 4352 2069 6e73  ted with OCR ins
-000028e0: 7465 6164 206f 6620 6173 2069 6d61 6765  tead of as image
-000028f0: 732e 0d0a 0d0a 2320 5370 6f6e 736f 7273  s.....# Sponsors
-00002900: 0d0a 0d0a 3c61 2068 7265 663d 2268 7474  ....<a href="htt
-00002910: 7073 3a2f 2f63 616c 2e63 6f6d 2f65 6d6d  ps://cal.com/emm
-00002920: 6574 742d 6d63 662f 3330 6d69 6e22 3e3c  ett-mcf/30min"><
-00002930: 696d 6720 616c 743d 2242 6f6f 6b20 7573  img alt="Book us
-00002940: 2077 6974 6820 4361 6c2e 636f 6d22 2073   with Cal.com" s
-00002950: 7263 3d22 6874 7470 733a 2f2f 6361 6c2e  rc="https://cal.
-00002960: 636f 6d2f 626f 6f6b 2d77 6974 682d 6361  com/book-with-ca
-00002970: 6c2d 6461 726b 2e73 7667 2220 2f3e 3c2f  l-dark.svg" /></
-00002980: 613e 0d0a 0d0a 5468 616e 6b20 796f 7520  a>....Thank you 
-00002990: 746f 205b 4361 6c2e 636f 6d5d 2868 7474  to [Cal.com](htt
-000029a0: 7073 3a2f 2f63 616c 2e63 6f6d 2f29 2066  ps://cal.com/) f
-000029b0: 6f72 2073 706f 6e73 6f72 696e 6720 7468  or sponsoring th
-000029c0: 6973 2070 726f 6a65 6374 2e20 436f 6e74  is project. Cont
-000029d0: 6163 7420 656d 6d65 7474 4074 6865 7069  act emmett@thepi
-000029e0: 2e70 6520 666f 7220 7370 6f6e 736f 7273  .pe for sponsors
-000029f0: 6869 7020 696e 666f 726d 6174 696f 6e2e  hip information.
+00001220: 2020 2020 2020 2020 2020 7c20 602e 6a70            | `.jp
+00001230: 6760 2c20 602e 6a70 6567 602c 2060 2e70  g`, `.jpeg`, `.p
+00001240: 6e67 6020 7c20 e29d 8c20 2020 2020 2020  ng` | ...       
+00001250: 2020 2020 2020 2020 207c 20e2 9c94 efb8           | .....
+00001260: 8f20 2020 2020 2020 2020 2020 2020 207c  .              |
+00001270: 2045 7874 7261 6374 7320 696d 6167 6573   Extracts images
+00001280: 2c20 7573 6573 204f 4352 2069 6620 7465  , uses OCR if te
+00001290: 7874 5f6f 6e6c 7920 2020 2020 2020 2020  xt_only         
+000012a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000012b0: 0d0a 7c20 4461 7461 2054 6162 6c65 2020  ..| Data Table  
+000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012d0: 2020 2020 2020 2020 207c 2060 2e63 7376           | `.csv
+000012e0: 602c 2060 2e78 6c73 602c 2060 2e78 6c73  `, `.xls`, `.xls
+000012f0: 7860 2020 2020 2020 2020 2020 2020 207c  x`             |
+00001300: 20e2 9c94 efb8 8f20 2020 2020 2020 2020   ......         
+00001310: 2020 2020 2020 207c 20e2 9d8c 2020 2020         | ...    
+00001320: 2020 2020 2020 2020 2020 207c 2045 7874             | Ext
+00001330: 7261 6374 7320 6461 7461 2066 726f 6d20  racts data from 
+00001340: 7370 7265 6164 7368 6565 7473 3b20 636f  spreadsheets; co
+00001350: 6e76 6572 7473 2074 6f20 7465 7874 2072  nverts to text r
+00001360: 6570 7265 7365 6e74 6174 696f 6e2e 2046  epresentation. F
+00001370: 6f72 2076 6572 7920 6c61 7267 6520 6461  or very large da
+00001380: 7461 7365 7473 2c20 7769 6c6c 206f 6e6c  tasets, will onl
+00001390: 7920 6578 7472 6163 7420 636f 6c75 6d6e  y extract column
+000013a0: 206e 616d 6573 2061 6e64 2074 7970 6573   names and types
+000013b0: 2020 2020 2020 2020 207c 0d0a 7c20 4a75           |..| Ju
+000013c0: 7079 7465 7220 4e6f 7465 626f 6f6b 2020  pyter Notebook  
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013e0: 2020 2020 7c20 602e 6970 796e 6260 2020      | `.ipynb`  
+000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001400: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00001410: e29d 8c20 2020 2020 2020 2020 2020 2020  ...             
+00001420: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
+00001430: 2020 2020 2020 2020 207c 2045 7874 7261           | Extra
+00001440: 6374 7320 636f 6465 2c20 6d61 726b 646f  cts code, markdo
+00001450: 776e 2c20 616e 6420 696d 6167 6573 2066  wn, and images f
+00001460: 726f 6d20 4a75 7079 7465 7220 6e6f 7465  rom Jupyter note
+00001470: 626f 6f6b 7320 2020 2020 2020 2020 2020  books           
+00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001490: 2020 2020 2020 207c 0d0a 7c20 4d69 6372         |..| Micr
+000014a0: 6f73 6f66 7420 576f 7264 2044 6f63 756d  osoft Word Docum
+000014b0: 656e 7420 2020 2020 2020 2020 2020 2020  ent             
+000014c0: 2020 7c20 602e 646f 6378 6020 2020 2020    | `.docx`     
+000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014e0: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
+000014f0: 94ef b88f 2020 2020 2020 2020 2020 2020  ....            
+00001500: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
+00001510: 2020 2020 2020 2020 2020 7c20 4578 7472            | Extr
+00001520: 6163 7473 2074 6578 7420 616e 6420 696d  acts text and im
+00001530: 6167 6573 2066 726f 6d20 576f 7264 2064  ages from Word d
+00001540: 6f63 756d 656e 7473 2020 2020 2020 2020  ocuments        
+00001550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001570: 7c0d 0a7c 204d 6963 726f 736f 6674 2050  |..| Microsoft P
+00001580: 6f77 6572 506f 696e 7420 5072 6573 656e  owerPoint Presen
+00001590: 7461 7469 6f6e 2020 2020 207c 2060 2e70  tation     | `.p
+000015a0: 7074 7860 2020 2020 2020 2020 2020 2020  ptx`            
+000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015c0: 2020 2020 207c 20e2 9c94 efb8 8f20 2020       | ......   
+000015d0: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
+000015e0: 94ef b88f 2020 2020 2020 2020 2020 2020  ....            
+000015f0: 2020 207c 2045 7874 7261 6374 7320 7465     | Extracts te
+00001600: 7874 2061 6e64 2069 6d61 6765 7320 6672  xt and images fr
+00001610: 6f6d 2050 6f77 6572 506f 696e 7420 7072  om PowerPoint pr
+00001620: 6573 656e 7461 7469 6f6e 7320 2020 2020  esentations     
+00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001640: 2020 2020 2020 2020 207c 0d0a 7c20 5669           |..| Vi
+00001650: 6465 6f20 2020 2020 2020 2020 2020 2020  deo             
+00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001670: 2020 2020 7c20 602e 6d70 3460 2c20 602e      | `.mp4`, `.
+00001680: 6176 6960 2c20 602e 6d6f 7660 2c20 602e  avi`, `.mov`, `.
+00001690: 776d 7660 2020 2020 207c 20e2 9c94 efb8  wmv`     | .....
+000016a0: 8f20 2020 2020 2020 2020 2020 2020 2020  .               
+000016b0: 7c20 e29c 94ef b88f 2020 2020 2020 2020  | ......        
+000016c0: 2020 2020 2020 2020 7c20 4578 7472 6163          | Extrac
+000016d0: 7473 2066 7261 6d65 7320 6672 6f6d 2076  ts frames from v
+000016e0: 6964 656f 2066 696c 6573 3b20 7375 7070  ideo files; supp
+000016f0: 6f72 7473 2066 7261 6d65 2065 7874 7261  orts frame extra
+00001700: 6374 696f 6e20 616e 6420 4f43 5220 666f  ction and OCR fo
+00001710: 7220 7465 7874 2065 7874 7261 6374 696f  r text extractio
+00001720: 6e20 6672 6f6d 2066 7261 6d65 7320 7c0d  n from frames |.
+00001730: 0a7c 2041 7564 696f 2020 2020 2020 2020  .| Audio        
+00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001750: 2020 2020 2020 2020 207c 2060 2e6d 7033           | `.mp3
+00001760: 602c 2060 2e77 6176 6020 2020 2020 2020  `, `.wav`       
+00001770: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
+00001780: 2020 2020 2020 2020 2020 7c20 e29d 8c20            | ... 
+00001790: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000017a0: 2045 7874 7261 6374 7320 7465 7874 2066   Extracts text f
+000017b0: 726f 6d20 6175 6469 6f20 6669 6c65 733b  rom audio files;
+000017c0: 2073 7570 706f 7274 7320 7370 6565 6368   supports speech
+000017d0: 2d74 6f2d 7465 7874 2063 6f6e 7665 7273  -to-text convers
+000017e0: 696f 6e20 2020 2020 2020 207c 200d 0a7c  ion        | ..|
+000017f0: 2057 6562 7369 7465 2020 2020 2020 2020   Website        
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 2020 2020 2020 207c 2055 524c 7320 2869         | URLs (i
+00001820: 6e70 7574 7320 636f 6e74 6169 6e69 6e67  nputs containing
+00001830: 2060 6874 7470 602c 2060 6874 7470 7360   `http`, `https`
+00001840: 2c20 6066 7470 6029 2020 2020 2020 2020  , `ftp`)        
+00001850: 2020 2020 207c 20e2 9c94 efb8 8f20 2020       | ......   
+00001860: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+00001870: 9c94 efb8 8f20 2020 207c 2045 7874 7261  .....    | Extra
+00001880: 6374 7320 7465 7874 2066 726f 6d20 7765  cts text from we
+00001890: 6220 7061 6765 2061 6c6f 6e67 2077 6974  b page along wit
+000018a0: 6820 696d 6167 6520 286f 7220 696d 6167  h image (or imag
+000018b0: 6573 2069 6620 7363 726f 6c6c 6162 6c65  es if scrollable
+000018c0: 293b 2074 6578 742d 6f6e 6c79 2065 7874  ); text-only ext
+000018d0: 7261 6374 696f 6e20 6176 6169 6c61 626c  raction availabl
+000018e0: 6520 2020 2020 2020 2020 207c 0d0a 7c20  e          |..| 
+000018f0: 4769 7448 7562 2052 6570 6f73 6974 6f72  GitHub Repositor
+00001900: 7920 2020 2020 2020 2020 2020 2020 2020  y               
+00001910: 2020 2020 2020 7c20 4769 7448 7562 2072        | GitHub r
+00001920: 6570 6f20 5552 4c73 2020 2020 2020 2020  epo URLs        
+00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001940: 207c 20e2 9c94 efb8 8f20 2020 2020 2020   | ......       
+00001950: 2020 2020 2020 2020 7c20 e29c 94ef b88f          | ......
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 7c20 4578 7472 6163 7473 2066 726f 6d20  | Extracts from 
+00001980: 4769 7448 7562 2072 6570 6f73 6974 6f72  GitHub repositor
+00001990: 6965 733b 2073 7570 706f 7274 7320 6272  ies; supports br
+000019a0: 616e 6368 2073 7065 6369 6669 6361 7469  anch specificati
+000019b0: 6f6e 2020 2020 2020 2020 207c 0d0a 7c20  on         |..| 
+000019c0: 596f 7554 7562 6520 5669 6465 6f20 2020  YouTube Video   
+000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019e0: 2020 2020 2020 7c20 596f 7554 7562 6520        | YouTube 
+000019f0: 7669 6465 6f20 5552 4c73 2020 2020 2020  video URLs      
+00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a10: 7c20 e29c 94ef b88f 2020 2020 2020 2020  | ......        
+00001a20: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
+00001a30: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001a40: 2045 7874 7261 6374 7320 7465 7874 2066   Extracts text f
+00001a50: 726f 6d20 596f 7554 7562 6520 7669 6465  rom YouTube vide
+00001a60: 6f73 3b20 7375 7070 6f72 7473 2073 7562  os; supports sub
+00001a70: 7469 746c 6573 2065 7874 7261 6374 696f  titles extractio
+00001a80: 6e20 2020 2020 2020 2020 207c 0d0a 7c20  n          |..| 
+00001a90: 5a49 5020 4669 6c65 2020 2020 2020 2020  ZIP File        
+00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ab0: 2020 2020 2020 7c20 602e 7a69 7060 2020        | `.zip`  
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ae0: 7c20 e29c 94ef b88f 2020 2020 2020 2020  | ......        
+00001af0: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
+00001b00: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001b10: 2045 7874 7261 6374 7320 636f 6e74 656e   Extracts conten
+00001b20: 7473 206f 6620 5a49 5020 6669 6c65 733b  ts of ZIP files;
+00001b30: 2073 7570 706f 7274 7320 6e65 7374 6564   supports nested
+00001b40: 2064 6972 6563 746f 7279 2065 7874 7261   directory extra
+00001b50: 6374 696f 6e20 2020 2020 7c0d 0a0d 0a23  ction     |....#
+00001b60: 2320 486f 7720 6974 2077 6f72 6b73 20f0  # How it works .
+00001b70: 9f9b a0ef b88f 0d0a 0d0a 5468 6520 696e  ..........The in
+00001b80: 7075 7420 736f 7572 6365 2069 7320 6569  put source is ei
+00001b90: 7468 6572 2061 2066 696c 6520 7061 7468  ther a file path
+00001ba0: 2c20 6120 5552 4c2c 206f 7220 6120 6469  , a URL, or a di
+00001bb0: 7265 6374 6f72 792e 2054 6865 2070 6970  rectory. The pip
+00001bc0: 6520 7769 6c6c 2065 7874 7261 6374 2069  e will extract i
+00001bd0: 6e66 6f72 6d61 7469 6f6e 2066 726f 6d20  nformation from 
+00001be0: 7468 6520 736f 7572 6365 2061 6e64 2070  the source and p
+00001bf0: 726f 6365 7373 2069 7420 666f 7220 646f  rocess it for do
+00001c00: 776e 7374 7265 616d 2075 7365 2077 6974  wnstream use wit
+00001c10: 6820 5b6c 616e 6775 6167 6520 6d6f 6465  h [language mode
+00001c20: 6c73 5d28 6874 7470 733a 2f2f 656e 2e77  ls](https://en.w
+00001c30: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
+00001c40: 692f 4c61 7267 655f 6c61 6e67 7561 6765  i/Large_language
+00001c50: 5f6d 6f64 656c 292c 205b 7669 7369 6f6e  _model), [vision
+00001c60: 2074 7261 6e73 666f 726d 6572 735d 2868   transformers](h
+00001c70: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00001c80: 6469 612e 6f72 672f 7769 6b69 2f56 6973  dia.org/wiki/Vis
+00001c90: 696f 6e5f 7472 616e 7366 6f72 6d65 7229  ion_transformer)
+00001ca0: 2c20 6f72 205b 7669 7369 6f6e 2d6c 616e  , or [vision-lan
+00001cb0: 6775 6167 6520 6d6f 6465 6c73 5d28 6874  guage models](ht
+00001cc0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
+00001cd0: 6162 732f 3233 3034 2e30 3036 3835 292e  abs/2304.00685).
+00001ce0: 2054 6865 206f 7574 7075 7420 6672 6f6d   The output from
+00001cf0: 2074 6865 2070 6970 6520 6973 2061 2073   the pipe is a s
+00001d00: 656e 7369 626c 6520 6c69 7374 206f 6620  ensible list of 
+00001d10: 6d75 6c74 696d 6f64 616c 206d 6573 7361  multimodal messa
+00001d20: 6765 7320 7265 7072 6573 656e 7469 6e67  ges representing
+00001d30: 2063 6875 6e6b 7320 6f66 2074 6865 2065   chunks of the e
+00001d40: 7874 7261 6374 6564 2069 6e66 6f72 6d61  xtracted informa
+00001d50: 7469 6f6e 2c20 6361 7265 6675 6c6c 7920  tion, carefully 
+00001d60: 6372 6166 7465 6420 746f 2066 6974 2077  crafted to fit w
+00001d70: 6974 6869 6e20 636f 6e74 6578 7420 7769  ithin context wi
+00001d80: 6e64 6f77 7320 666f 7220 616e 7920 6d6f  ndows for any mo
+00001d90: 6465 6c73 2066 726f 6d20 5b67 656d 6d61  dels from [gemma
+00001da0: 2d37 625d 2868 7474 7073 3a2f 2f68 7567  -7b](https://hug
+00001db0: 6769 6e67 6661 6365 2e63 6f2f 676f 6f67  gingface.co/goog
+00001dc0: 6c65 2f67 656d 6d61 2d37 6229 2074 6f20  le/gemma-7b) to 
+00001dd0: 5b47 5054 2d34 5d28 6874 7470 733a 2f2f  [GPT-4](https://
+00001de0: 6f70 656e 6169 2e63 6f6d 2f67 7074 2d34  openai.com/gpt-4
+00001df0: 292e 2054 6865 206d 6573 7361 6765 7320  ). The messages 
+00001e00: 7265 7475 726e 6564 2073 686f 756c 6420  returned should 
+00001e10: 6c6f 6f6b 206c 696b 6520 7468 6973 3a0d  look like this:.
+00001e20: 0a60 6060 6a73 6f6e 0d0a 5b0d 0a20 207b  .```json..[..  {
+00001e30: 0d0a 2020 2020 2272 6f6c 6522 3a20 2275  ..    "role": "u
+00001e40: 7365 7222 2c0d 0a20 2020 2022 636f 6e74  ser",..    "cont
+00001e50: 656e 7422 3a20 5b0d 0a20 2020 2020 207b  ent": [..      {
+00001e60: 0d0a 2020 2020 2020 2020 2274 7970 6522  ..        "type"
+00001e70: 3a20 2274 6578 7422 2c0d 0a20 2020 2020  : "text",..     
+00001e80: 2020 2022 7465 7874 223a 2022 2e2e 2e22     "text": "..."
+00001e90: 0d0a 2020 2020 2020 7d2c 0d0a 2020 2020  ..      },..    
+00001ea0: 2020 7b0d 0a20 2020 2020 2020 2022 7479    {..        "ty
+00001eb0: 7065 223a 2022 696d 6167 655f 7572 6c22  pe": "image_url"
+00001ec0: 2c0d 0a20 2020 2020 2020 2022 696d 6167  ,..        "imag
+00001ed0: 655f 7572 6c22 3a20 7b0d 0a20 2020 2020  e_url": {..     
+00001ee0: 2020 2020 2022 7572 6c22 3a20 2264 6174       "url": "dat
+00001ef0: 613a 696d 6167 652f 6a70 6567 3b62 6173  a:image/jpeg;bas
+00001f00: 6536 342c 2e2e 2e22 0d0a 2020 2020 2020  e64,..."..      
+00001f10: 2020 7d0d 0a20 2020 2020 207d 0d0a 2020    }..      }..  
+00001f20: 2020 5d0d 0a20 207d 0d0a 5d0d 0a60 6060    ]..  }..]..```
+00001f30: 0d0a 4966 2079 6f75 2077 616e 7420 746f  ..If you want to
+00001f40: 2066 6565 6420 7468 6573 6520 6d65 7373   feed these mess
+00001f50: 6167 6573 2064 6972 6563 746c 7920 696e  ages directly in
+00001f60: 746f 2074 6865 206d 6f64 656c 2c20 6974  to the model, it
+00001f70: 2069 7320 696d 706f 7274 616e 7420 746f   is important to
+00001f80: 2062 6520 6d69 6e64 6675 6c20 6f66 2074   be mindful of t
+00001f90: 6865 2074 6f6b 656e 206c 696d 6974 2e0d  he token limit..
+00001fa0: 0a4f 7065 6e41 4920 646f 6573 206e 6f74  .OpenAI does not
+00001fb0: 2061 6c6c 6f77 2074 6f6f 206d 616e 7920   allow too many 
+00001fc0: 696d 6167 6573 2069 6e20 7468 6520 7072  images in the pr
+00001fd0: 6f6d 7074 2028 7365 6520 6469 7363 7573  ompt (see discus
+00001fe0: 7369 6f6e 205b 6865 7265 5d28 6874 7470  sion [here](http
+00001ff0: 733a 2f2f 636f 6d6d 756e 6974 792e 6f70  s://community.op
+00002000: 656e 6169 2e63 6f6d 2f74 2f67 7074 2d34  enai.com/t/gpt-4
+00002010: 2d76 6973 696f 6e2d 6d61 7869 6d75 6d2d  -vision-maximum-
+00002020: 616d 6f75 6e74 2d6f 662d 696d 6167 6573  amount-of-images
+00002030: 2f35 3733 3131 302f 3629 292c 2073 6f20  /573110/6)), so 
+00002040: 6c6f 6e67 2066 696c 6573 2073 686f 756c  long files shoul
+00002050: 6420 6265 2065 7874 7261 6374 6564 2077  d be extracted w
+00002060: 6974 6820 6074 6578 745f 6f6e 6c79 3d54  ith `text_only=T
+00002070: 7275 6560 2074 6f20 6176 6f69 6420 7468  rue` to avoid th
+00002080: 6973 2069 7373 7565 2c20 7768 696c 6520  is issue, while 
+00002090: 6c6f 6e67 2074 6578 7420 6669 6c65 7320  long text files 
+000020a0: 7368 6f75 6c64 2065 6974 6865 7220 6265  should either be
+000020b0: 2063 6f6d 7072 6573 7365 6420 6f72 2065   compressed or e
+000020c0: 6d62 6564 6465 6420 696e 2061 2052 4147  mbedded in a RAG
+000020d0: 2066 7261 6d65 776f 726b 2e0d 0a0d 0a54   framework.....T
+000020e0: 6865 2074 6578 7420 616e 6420 696d 6167  he text and imag
+000020f0: 6573 2066 726f 6d20 7468 6573 6520 6d65  es from these me
+00002100: 7373 6167 6573 206d 6179 2061 6c73 6f20  ssages may also 
+00002110: 6265 2070 7265 7061 7265 6420 666f 7220  be prepared for 
+00002120: 6120 7665 6374 6f72 2064 6174 6162 6173  a vector databas
+00002130: 6520 7769 7468 2060 7468 6570 6970 652e  e with `thepipe.
+00002140: 636f 7265 2e63 7265 6174 655f 6368 756e  core.create_chun
+00002150: 6b73 5f66 726f 6d5f 6d65 7373 6167 6573  ks_from_messages
+00002160: 6020 6f72 2066 6f72 2064 6f77 6e73 7472  ` or for downstr
+00002170: 6561 6d20 7573 6520 7769 7468 2052 4147  eam use with RAG
+00002180: 2066 7261 6d65 776f 726b 732e 205b 4c69   frameworks. [Li
+00002190: 7465 4c4c 4d5d 2868 7474 7073 3a2f 2f67  teLLM](https://g
+000021a0: 6974 6875 622e 636f 6d2f 4265 7272 6941  ithub.com/BerriA
+000021b0: 492f 6c69 7465 6c6c 6d29 2063 616e 2062  I/litellm) can b
+000021c0: 6520 7573 6564 2074 6f20 6561 7369 6c79  e used to easily
+000021d0: 2069 6e74 6567 7261 7465 2054 6865 2050   integrate The P
+000021e0: 6970 6520 7769 7468 2061 6e79 204c 4c4d  ipe with any LLM
+000021f0: 2070 726f 7669 6465 722e 200d 0a0d 0a49   provider. ....I
+00002200: 7420 7573 6573 2061 2076 6172 6965 7479  t uses a variety
+00002210: 206f 6620 6865 7572 6973 7469 6373 2066   of heuristics f
+00002220: 6f72 206f 7074 696d 616c 2070 6572 666f  or optimal perfo
+00002230: 726d 616e 6365 2077 6974 6820 7669 7369  rmance with visi
+00002240: 6f6e 2d6c 616e 6775 6167 6520 6d6f 6465  on-language mode
+00002250: 6c73 2c20 696e 636c 7564 696e 6720 4149  ls, including AI
+00002260: 2066 696c 6574 7970 6520 6465 7465 6374   filetype detect
+00002270: 696f 6e20 7769 7468 205b 6669 6c65 7479  ion with [filety
+00002280: 7065 2064 6574 6563 7469 6f6e 5d28 6874  pe detection](ht
+00002290: 7470 733a 2f2f 6f70 656e 736f 7572 6365  tps://opensource
+000022a0: 2e67 6f6f 676c 6562 6c6f 672e 636f 6d2f  .googleblog.com/
+000022b0: 3230 3234 2f30 322f 6d61 6769 6b61 2d61  2024/02/magika-a
+000022c0: 692d 706f 7765 7265 642d 6661 7374 2d61  i-powered-fast-a
+000022d0: 6e64 2d65 6666 6963 6965 6e74 2d66 696c  nd-efficient-fil
+000022e0: 652d 7479 7065 2d69 6465 6e74 6966 6963  e-type-identific
+000022f0: 6174 696f 6e2e 6874 6d6c 292c 206f 7074  ation.html), opt
+00002300: 2d69 6e20 4149 205b 7461 626c 652c 2065  -in AI [table, e
+00002310: 7175 6174 696f 6e2c 2061 6e64 2066 6967  quation, and fig
+00002320: 7572 6520 6578 7472 6163 7469 6f6e 5d28  ure extraction](
+00002330: 6874 7470 733a 2f2f 7468 6570 692e 7065  https://thepi.pe
+00002340: 2f70 7269 6369 6e67 292c 2065 6666 6963  /pricing), effic
+00002350: 6965 6e74 205b 746f 6b65 6e20 636f 6d70  ient [token comp
+00002360: 7265 7373 696f 6e5d 2868 7474 7073 3a2f  ression](https:/
+00002370: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00002380: 3430 332e 3132 3936 3829 2c20 6175 746f  403.12968), auto
+00002390: 6d61 7469 6320 5b69 6d61 6765 2065 6e63  matic [image enc
+000023a0: 6f64 696e 675d 2868 7474 7073 3a2f 2f65  oding](https://e
+000023b0: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+000023c0: 7769 6b69 2f42 6173 6536 3429 2c20 5b72  wiki/Base64), [r
+000023d0: 6572 616e 6b69 6e67 5d28 6874 7470 733a  eranking](https:
+000023e0: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
+000023f0: 3233 3130 2e30 3638 3339 2920 666f 7220  2310.06839) for 
+00002400: 5b6c 6f73 742d 696e 2d74 6865 2d6d 6964  [lost-in-the-mid
+00002410: 646c 655d 2868 7474 7073 3a2f 2f61 7278  dle](https://arx
+00002420: 6976 2e6f 7267 2f61 6273 2f32 3330 372e  iv.org/abs/2307.
+00002430: 3033 3137 3229 2065 6666 6563 7473 2c20  03172) effects, 
+00002440: 616e 6420 6d6f 7265 2c20 616c 6c20 7072  and more, all pr
+00002450: 652d 6275 696c 7420 746f 2077 6f72 6b20  e-built to work 
+00002460: 6f75 742d 6f66 2d74 6865 2d62 6f78 2e0d  out-of-the-box..
+00002470: 0a0d 0a21 5b44 656d 6f5d 2868 7474 7073  ...![Demo](https
+00002480: 3a2f 2f72 706e 7574 7a65 6d75 7462 7275  ://rpnutzemutbru
+00002490: 6d63 7a77 7675 652e 7375 7061 6261 7365  mczwvue.supabase
+000024a0: 2e63 6f2f 7374 6f72 6167 652f 7631 2f6f  .co/storage/v1/o
+000024b0: 626a 6563 742f 7075 626c 6963 2f61 7373  bject/public/ass
+000024c0: 6574 732f 6772 6164 6572 2e70 7925 3230  ets/grader.py%20
+000024d0: 2836 292e 706e 6729 0d0a 0d0a 0d0a 2323  (6).png)......##
+000024e0: 204c 6f63 616c 2049 6e73 7461 6c6c 6174   Local Installat
+000024f0: 696f 6e20 f09f 9ba0 efb8 8f0d 0a0d 0a54  ion ...........T
+00002500: 6865 2050 6970 6520 6861 6e64 6c65 7320  he Pipe handles 
+00002510: 6120 7769 6465 2061 7272 6179 206f 6620  a wide array of 
+00002520: 636f 6d70 6c65 7820 6669 6c65 7479 7065  complex filetype
+00002530: 732c 2061 6e64 2074 6875 7320 7265 7175  s, and thus requ
+00002540: 6972 6573 2069 6e73 7461 6c6c 6174 696f  ires installatio
+00002550: 6e20 6f66 206d 616e 7920 6469 6666 6572  n of many differ
+00002560: 656e 7420 7061 636b 6167 6573 2074 6f20  ent packages to 
+00002570: 6675 6e63 7469 6f6e 2e20 4974 2061 6c73  function. It als
+00002580: 6f20 7265 7175 6972 6573 2061 2076 6572  o requires a ver
+00002590: 7920 6361 7061 626c 6520 6d61 6368 696e  y capable machin
+000025a0: 6520 666f 7220 676f 6f64 2072 6573 706f  e for good respo
+000025b0: 6e73 6520 7469 6d65 732e 2046 6f72 2074  nse times. For t
+000025c0: 6869 7320 7265 6173 6f6e 2c20 7765 2068  his reason, we h
+000025d0: 6f73 7420 6974 2061 7320 616e 2041 5049  ost it as an API
+000025e0: 2074 6861 7420 776f 726b 7320 6f75 742d   that works out-
+000025f0: 6f66 2d74 6865 2d62 6f78 2e20 546f 2075  of-the-box. To u
+00002600: 7365 2054 6865 2050 6970 6520 6c6f 6361  se The Pipe loca
+00002610: 6c6c 7920 666f 7220 6672 6565 2069 6e73  lly for free ins
+00002620: 7465 6164 2c20 796f 7520 7769 6c6c 206e  tead, you will n
+00002630: 6565 6420 5b70 6c61 7977 7269 6768 745d  eed [playwright]
+00002640: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00002650: 636f 6d2f 6d69 6372 6f73 6f66 742f 706c  com/microsoft/pl
+00002660: 6179 7772 6967 6874 292c 205b 6374 6167  aywright), [ctag
+00002670: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00002680: 622e 636f 6d2f 756e 6976 6572 7361 6c2d  b.com/universal-
+00002690: 6374 6167 732f 292c 205b 7079 7465 7373  ctags/), [pytess
+000026a0: 6572 6163 745d 2868 7474 7073 3a2f 2f67  eract](https://g
+000026b0: 6974 6875 622e 636f 6d2f 682f 7079 7465  ithub.com/h/pyte
+000026c0: 7373 6572 6163 7429 2c20 616e 6420 7468  sseract), and th
+000026d0: 6520 6c6f 6361 6c20 7079 7468 6f6e 2072  e local python r
+000026e0: 6571 7569 7265 6d65 6e74 732c 2077 6869  equirements, whi
+000026f0: 6368 2064 6966 6665 7220 6672 6f6d 2074  ch differ from t
+00002700: 6865 206d 6f72 6520 6c69 6768 7477 6569  he more lightwei
+00002710: 6768 7420 4150 4920 7265 7175 6972 656d  ght API requirem
+00002720: 656e 7473 3a0d 0a0d 0a60 6060 6261 7368  ents:....```bash
+00002730: 0d0a 6769 7420 636c 6f6e 6520 6874 7470  ..git clone http
+00002740: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00002750: 6d63 662f 7468 6570 6970 650d 0a70 6970  mcf/thepipe..pip
+00002760: 2069 6e73 7461 6c6c 202d 7220 7265 7175   install -r requ
+00002770: 6972 656d 656e 7473 5f6c 6f63 616c 2e74  irements_local.t
+00002780: 7874 0d0a 6060 600d 0a0d 0a54 6970 2066  xt..```....Tip f
+00002790: 6f72 2077 696e 646f 7773 2075 7365 7273  or windows users
+000027a0: 3a20 496e 7374 616c 6c20 7468 6520 7079  : Install the py
+000027b0: 7468 6f6e 2d6c 6962 6d61 6769 6320 6269  thon-libmagic bi
+000027c0: 6e61 7269 6573 2077 6974 6820 6070 6970  naries with `pip
+000027d0: 2069 6e73 7461 6c6c 2070 7974 686f 6e2d   install python-
+000027e0: 6d61 6769 632d 6269 6e60 2e20 456e 7375  magic-bin`. Ensu
+000027f0: 7265 2074 6865 2060 7465 7373 6572 6163  re the `tesserac
+00002800: 742d 6f63 7260 2062 696e 6172 6965 7320  t-ocr` binaries 
+00002810: 616e 6420 7468 6520 6063 7461 6773 6020  and the `ctags` 
+00002820: 6269 6e61 7269 6573 2061 7265 2069 6e20  binaries are in 
+00002830: 796f 7572 2050 4154 482e 0d0a 0d0a 4e6f  your PATH.....No
+00002840: 7720 796f 7520 6361 6e20 7573 6520 5468  w you can use Th
+00002850: 6520 5069 7065 2077 6974 6820 5079 7468  e Pipe with Pyth
+00002860: 6f6e 3a0d 0a60 6060 6261 7368 0d0a 6672  on:..```bash..fr
+00002870: 6f6d 2074 6865 7069 7065 5f61 7069 2069  om thepipe_api i
+00002880: 6d70 6f72 7420 7468 6570 6970 650d 0a63  mport thepipe..c
+00002890: 6875 6e6b 7320 3d20 7468 6570 6970 652e  hunks = thepipe.
+000028a0: 6578 7472 6163 7428 2265 7861 6d70 6c65  extract("example
+000028b0: 2e70 6466 222c 206c 6f63 616c 3d54 7275  .pdf", local=Tru
+000028c0: 6529 0d0a 6060 600d 0a0d 0a6f 7220 6672  e)..```....or fr
+000028d0: 6f6d 2074 6865 2063 6f6d 6d61 6e64 206c  om the command l
+000028e0: 696e 653a 0d0a 6060 6062 6173 680d 0a74  ine:..```bash..t
+000028f0: 6865 7069 7065 2070 6174 682f 746f 2f66  hepipe path/to/f
+00002900: 6f6c 6465 7220 2d2d 6c6f 6361 6c0d 0a60  older --local..`
+00002910: 6060 0d0a 0d0a 4172 6775 6d65 6e74 7320  ``....Arguments 
+00002920: 6172 653a 0d0a 2d20 6073 6f75 7263 6560  are:..- `source`
+00002930: 2028 7265 7175 6972 6564 293a 2063 616e   (required): can
+00002940: 2062 6520 6120 6669 6c65 2070 6174 682c   be a file path,
+00002950: 2061 2055 524c 2c20 6f72 2061 2064 6972   a URL, or a dir
+00002960: 6563 746f 7279 2070 6174 682e 0d0a 2d20  ectory path...- 
+00002970: 606c 6f63 616c 6020 286f 7074 696f 6e61  `local` (optiona
+00002980: 6c29 3a20 5573 6520 7468 6520 6c6f 6361  l): Use the loca
+00002990: 6c20 7665 7273 696f 6e20 6f66 2054 6865  l version of The
+000029a0: 2050 6970 6520 696e 7374 6561 6420 6f66   Pipe instead of
+000029b0: 2074 6865 2068 6f73 7465 6420 4150 492e   the hosted API.
+000029c0: 0d0a 2d20 606d 6174 6368 6020 286f 7074  ..- `match` (opt
+000029d0: 696f 6e61 6c29 3a20 5375 6273 7472 696e  ional): Substrin
+000029e0: 6720 746f 206d 6174 6368 2066 696c 6573  g to match files
+000029f0: 2069 6e20 7468 6520 6469 7265 6374 6f72   in the director
+00002a00: 792e 2052 6567 6578 2069 7320 6e6f 7420  y. Regex is not 
+00002a10: 7965 7420 7375 7070 6f72 7465 642e 0d0a  yet supported...
+00002a20: 2d20 6069 676e 6f72 6560 2028 6f70 7469  - `ignore` (opti
+00002a30: 6f6e 616c 293a 2053 7562 7374 7269 6e67  onal): Substring
+00002a40: 2074 6f20 6967 6e6f 7265 2066 696c 6573   to ignore files
+00002a50: 2069 6e20 7468 6520 6469 7265 6374 6f72   in the director
+00002a60: 792e 2052 6567 6578 2069 7320 6e6f 7420  y. Regex is not 
+00002a70: 7965 7420 7375 7070 6f72 7465 642e 0d0a  yet supported...
+00002a80: 2d20 606c 696d 6974 6020 286f 7074 696f  - `limit` (optio
+00002a90: 6e61 6c29 3a20 5468 6520 746f 6b65 6e20  nal): The token 
+00002aa0: 6c69 6d69 7420 666f 7220 7468 6520 6f75  limit for the ou
+00002ab0: 7470 7574 2070 726f 6d70 742c 2064 6566  tput prompt, def
+00002ac0: 6175 6c74 7320 746f 2031 3030 4b2e 2050  aults to 100K. P
+00002ad0: 726f 6d70 7473 2065 7863 6565 6469 6e67  rompts exceeding
+00002ae0: 2074 6865 206c 696d 6974 2077 696c 6c20   the limit will 
+00002af0: 6265 2063 6f6d 7072 6573 7365 642e 2054  be compressed. T
+00002b00: 6869 7320 6d61 7920 6e6f 7420 776f 726b  his may not work
+00002b10: 2061 7320 6578 7065 6374 6564 2077 6974   as expected wit
+00002b20: 6820 7468 6520 4150 492c 2061 7320 6974  h the API, as it
+00002b30: 2069 7320 696e 2061 6374 6976 6520 6465   is in active de
+00002b40: 7665 6c6f 706d 656e 742e 0d0a 2d20 6061  velopment...- `a
+00002b50: 695f 6578 7472 6163 7469 6f6e 6020 286f  i_extraction` (o
+00002b60: 7074 696f 6e61 6c29 3a20 4578 7472 6163  ptional): Extrac
+00002b70: 7420 7461 626c 6573 2c20 6669 6775 7265  t tables, figure
+00002b80: 732c 2061 6e64 206d 6174 6820 6672 6f6d  s, and math from
+00002b90: 2050 4446 7320 7573 696e 6720 6f75 7220   PDFs using our 
+00002ba0: 6578 7472 6163 746f 722e 2049 6e63 7572  extractor. Incur
+00002bb0: 7320 6578 7472 6120 636f 7374 732e 0d0a  s extra costs...
+00002bc0: 2d20 6074 6578 745f 6f6e 6c79 6020 286f  - `text_only` (o
+00002bd0: 7074 696f 6e61 6c29 3a20 446f 206e 6f74  ptional): Do not
+00002be0: 2065 7874 7261 6374 2069 6d61 6765 7320   extract images 
+00002bf0: 6672 6f6d 2064 6f63 756d 656e 7473 206f  from documents o
+00002c00: 7220 7765 6273 6974 6573 2e20 4164 6469  r websites. Addi
+00002c10: 7469 6f6e 616c 6c79 2c20 696d 6167 6520  tionally, image 
+00002c20: 6669 6c65 7320 7769 6c6c 2062 6520 7265  files will be re
+00002c30: 7072 6573 656e 7465 6420 7769 7468 204f  presented with O
+00002c40: 4352 2069 6e73 7465 6164 206f 6620 6173  CR instead of as
+00002c50: 2069 6d61 6765 732e 0d0a 0d0a 2320 5370   images.....# Sp
+00002c60: 6f6e 736f 7273 0d0a 0d0a 3c61 2068 7265  onsors....<a hre
+00002c70: 663d 2268 7474 7073 3a2f 2f63 616c 2e63  f="https://cal.c
+00002c80: 6f6d 2f65 6d6d 6574 742d 6d63 662f 3330  om/emmett-mcf/30
+00002c90: 6d69 6e22 3e3c 696d 6720 616c 743d 2242  min"><img alt="B
+00002ca0: 6f6f 6b20 7573 2077 6974 6820 4361 6c2e  ook us with Cal.
+00002cb0: 636f 6d22 2073 7263 3d22 6874 7470 733a  com" src="https:
+00002cc0: 2f2f 6361 6c2e 636f 6d2f 626f 6f6b 2d77  //cal.com/book-w
+00002cd0: 6974 682d 6361 6c2d 6461 726b 2e73 7667  ith-cal-dark.svg
+00002ce0: 2220 2f3e 3c2f 613e 0d0a 0d0a 5468 616e  " /></a>....Than
+00002cf0: 6b20 796f 7520 746f 205b 4361 6c2e 636f  k you to [Cal.co
+00002d00: 6d5d 2868 7474 7073 3a2f 2f63 616c 2e63  m](https://cal.c
+00002d10: 6f6d 2f29 2066 6f72 2073 706f 6e73 6f72  om/) for sponsor
+00002d20: 696e 6720 7468 6973 2070 726f 6a65 6374  ing this project
+00002d30: 2e20 436f 6e74 6163 7420 656d 6d65 7474  . Contact emmett
+00002d40: 4074 6865 7069 2e70 6520 666f 7220 7370  @thepi.pe for sp
+00002d50: 6f6e 736f 7273 6869 7020 696e 666f 726d  onsorship inform
+00002d60: 6174 696f 6e2e                           ation.
```

### Comparing `thepipe_api-0.3.2/setup.py` & `thepipe_api-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.3.2',
+    version='0.3.3',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
```

### Comparing `thepipe_api-0.3.2/tests/test_thepipe.py` & `thepipe_api-0.3.3/tests/test_thepipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,51 @@
     def tearDown(self):
         # clean up outputs
         if os.path.exists(self.outputs_directory):
             for file in os.listdir(self.outputs_directory):
                 os.remove(os.path.join(self.outputs_directory, file))
             os.rmdir(self.outputs_directory)
 
+    def test_extract_video(self):
+        chunks = extractor.extract_from_source(source=self.files_directory+"/example.mp4")
+        # verify it extracted the video file into chunks
+        self.assertEqual(type(chunks), list)
+        self.assertNotEqual(len(chunks), 0)
+        self.assertEqual(type(chunks[0]), core.Chunk)
+        # verify it extracted visual data
+        self.assertTrue(any(chunk.image for chunk in chunks))
+        # verify it extracted audio data
+        self.assertTrue(any(chunk.text for chunk in chunks))
+        # verify it transcribed the audio correctly, i.e., 'citizens' is in the extracted text
+        self.assertTrue(any('citizens' in chunk.text.lower() for chunk in chunks if chunk.text is not None))
+
+    def test_extract_audio(self):
+        chunks = extractor.extract_from_source(source=self.files_directory+"/example.mp3")
+        # verify it extracted the audio file into chunks
+        self.assertEqual(type(chunks), list)
+        self.assertNotEqual(len(chunks), 0)
+        self.assertEqual(type(chunks[0]), core.Chunk)
+        # verify it extracted audio data
+        self.assertTrue(any(chunk.text for chunk in chunks))
+        # verify it transcribed the audio correctly, i.e., 'citizens' is in the extracted text
+        self.assertTrue(any('citizens' in chunk.text.lower() for chunk in chunks if chunk.text is not None))
+    
+    def test_extract_youtube(self):
+        chunks = extractor.extract_from_source("https://www.youtube.com/watch?v=wUEr7TayrmU")
+        # verify it extracted the youtube video into chunks
+        self.assertEqual(type(chunks), list)
+        self.assertNotEqual(len(chunks), 0)
+        self.assertEqual(type(chunks[0]), core.Chunk)
+        # verify it extracted visual data
+        self.assertTrue(any(chunk.image for chunk in chunks))
+        # verify it extracted audio data
+        self.assertTrue(any(chunk.text for chunk in chunks))
+        # verify it transcribed the audio correctly, i.e., 'citizens' is in the extracted text
+        self.assertTrue(any('eliminated' in chunk.text.lower() for chunk in chunks if chunk.text is not None))
+    
     def test_image_to_base64(self):
         image = Image.open(os.path.join(self.files_directory, 'example.jpg'))
         image.load() # needed to close the file
         base64_string = core.image_to_base64(image)
         self.assertEqual(type(base64_string), str)
         # converting back should be the same
         image_data = base64.b64decode(base64_string)
@@ -109,17 +146,18 @@
             elif chunks[i].source_type == core.SourceTypes.IMAGE:
                 # verify extraction contains image
                 self.assertIsNotNone(chunks[i].image)
                 
     def test_compress_spreadsheet(self):
         chunks = extractor.extract_from_source(source=self.files_directory+"/example.xlsx")
         new_chunks = compressor.compress_chunks(chunks=chunks, limit=30)
-        self.assertEqual(len(new_chunks), 1)
         # verify that the compressed text is shorter than the original
-        self.assertLess(len(new_chunks[0].text.replace("Column names and types: ","")), len(chunks[0].text))
+        all_text = ''.join([chunk.text for chunk in chunks if chunk.text])
+        all_new_text = ''.join([chunk.text for chunk in new_chunks if chunk.text])
+        self.assertLess(len(all_new_text), len(all_text))
     
     def test_compress_with_llmlingua(self):
         chunks = extractor.extract_from_source(source=self.files_directory+"/example.md")
         new_chunks = compressor.compress_chunks(chunks=chunks, limit=30)
         # verify that the compressed text is shorter than the original
         old_chunktext = sum([len(chunk.text) for chunk in chunks if chunk.text is not None])
         new_chunktext = sum([len(chunk.text) for chunk in new_chunks if chunk.text is not None])
```

### Comparing `thepipe_api-0.3.2/thepipe_api/compressor.py` & `thepipe_api-0.3.3/thepipe_api/compressor.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,25 +64,14 @@
         window_text = chunk.text[i:i+WINDOW_SIZE]
         result = llm_lingua.compress_prompt(window_text, rate=0.5)
         new_window_text = result['compressed_prompt']
         new_chunk_text += new_window_text
     new_chunk = Chunk(path=chunk.path, text=new_chunk_text, image=chunk.image, source_type=chunk.source_type)
     return new_chunk
 
-def compress_spreadsheet(chunk: Chunk) -> Chunk:
-    loaded_json = json.loads(chunk.text)
-    row_one = loaded_json[0]
-    colnames = []
-    coltypes = []
-    for key, value in row_one.items():
-        colnames.append(key)
-        coltypes.append(type(value))
-    new_chunk_text = "Column names and types: " + str(list(zip(colnames, coltypes)))
-    return Chunk(path=chunk.path, text=new_chunk_text, image=chunk.image, source_type=chunk.source_type)
-
 def compress_chunks(chunks: List[Chunk], verbose: bool = False, limit: int = 1e5) -> List[Chunk]:
     new_chunks = chunks
     for _ in range(MAX_COMPRESSION_ATTEMPTS):
         if count_tokens(new_chunks) <= limit:
             break
         if verbose: print_status(f"Compressing prompt ({count_tokens(chunks)} tokens / {limit} limit)", status='info')
         new_chunks = []
@@ -92,15 +81,15 @@
                 new_chunk = chunk
             elif chunk.source_type == SourceTypes.COMPRESSIBLE_CODE:
                 extension = chunk.path.split('.')[-1]
                 new_chunk = compress_with_ctags(chunk, extension=extension)
             elif chunk.source_type in {SourceTypes.PLAINTEXT, SourceTypes.PDF, SourceTypes.DOCX, SourceTypes.PPTX, SourceTypes.URL}:
                 new_chunk = compress_with_llmlingua(chunk)
             elif chunk.source_type == SourceTypes.SPREADSHEET:
-                new_chunk = compress_spreadsheet(chunk)
+                new_chunk = compress_with_llmlingua(chunk)
             else:
                 # if the chunk is not compressible, keep the original text
                 new_chunk = chunk
             new_chunks.append(new_chunk)
     if count_tokens(new_chunks) > limit and verbose: 
         print_status("Failed to compress within limit, continuing", status='error')
     return new_chunks
```

### Comparing `thepipe_api-0.3.2/thepipe_api/core.py` & `thepipe_api-0.3.3/thepipe_api/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     SPREADSHEET = "spreadsheet"
     IPYNB = "ipynb"
     DOCX = "docx"
     PPTX = "pptx"
     URL = "website"
     GITHUB = "github repository"
     ZIP = "zip"
+    VIDEO = "video"
+    AUDIO = "audio"
+    YOUTUBE_VIDEO = "youtube video"
 
 class Chunk:
     def __init__(self, path: str, text: Optional[str] = None, image: Optional[Image.Image] = None, source_type: Optional[SourceTypes] = None):
         self.path = path
         self.text = text
         self.image = image
         self.source_type = source_type
```

### Comparing `thepipe_api-0.3.2/thepipe_api/extractor.py` & `thepipe_api-0.3.3/thepipe_api/extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import base64
 from concurrent.futures import ThreadPoolExecutor
 from io import BytesIO
+import math
 import re
 from typing import Dict, List, Optional
 import glob
 import os
 import tempfile
 from urllib.parse import urlparse
 import zipfile
@@ -28,14 +29,16 @@
 FILES_TO_IGNORE = {'package-lock.json', '.gitignore', '.bin', '.pyc', '.pyo', '.exe', '.bat', '.dll', '.obj', '.o', '.a', '.lib', '.so', '.dylib', '.ncb', '.sdf', '.suo', '.pdb', '.idb', '.pyd', '.ipynb_checkpoints', '.npy', '.pth'} # Files to ignore, please feel free to customize!
 CODE_EXTENSIONS = {'.h', '.json', '.js', '.jsx', '.ts', '.tsx',  '.cs', '.java', '.html', '.css', '.ini', '.xml', '.yaml', '.xaml', '.sh'} # Plaintext files that should not be compressed with LLMLingua
 CTAGS_CODE_EXTENSIONS = {'.c', '.cpp', '.py'} # code files that work with ctags
 PLAINTEXT_EXTENSIONS = {'.txt', '.md', '.rtf'}
 IMAGE_EXTENSIONS = {'.jpg', '.jpeg', '.png'}
 SPREADSHEET_EXTENSIONS = {'.csv', '.xls', '.xlsx'}
 DOCUMENT_EXTENSIONS = {'.pdf', '.docx', '.pptx'}
+VIDEO_EXTENSIONS = {'.mp4', '.avi', '.mov', '.mkv'}
+AUDIO_EXTENSIONS = {'.mp3', '.wav'}
 OTHER_EXTENSIONS = {'.zip', '.ipynb'}
 KNOWN_EXTENSIONS = IMAGE_EXTENSIONS.union(CODE_EXTENSIONS).union(CTAGS_CODE_EXTENSIONS).union(PLAINTEXT_EXTENSIONS).union(IMAGE_EXTENSIONS).union(SPREADSHEET_EXTENSIONS).union(DOCUMENT_EXTENSIONS).union(OTHER_EXTENSIONS)
 GITHUB_TOKEN: str = os.getenv("GITHUB_TOKEN")
 THEPIPE_API_KEY: str = os.getenv("THEPIPE_API_KEY")
 
 def extract_from_source(source: str, match: Optional[str] = None, ignore: Optional[str] = None, limit: int = None, verbose: bool = False, ai_extraction: bool = False, text_only: bool = False, local: bool = True) -> List[Chunk]:
     source_type = detect_type(source)
@@ -44,18 +47,18 @@
     if verbose: print_status(f"Extracting from {source_type.value}", status='info')
     if source_type == SourceTypes.DIR or source == '.' or source == './':
         if source == '.' or source == './':
             source = os.getcwd()
         return extract_from_directory(dir_path=source, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only, limit=limit, local=local)
     elif source_type == SourceTypes.GITHUB:
         return extract_github(github_url=source, file_path='', match=match, ignore=ignore, text_only=text_only, verbose=verbose, ai_extraction=ai_extraction, branch='master')
+    elif source_type == SourceTypes.YOUTUBE_VIDEO:
+        return extract_youtube(youtube_url=source, text_only=text_only, verbose=verbose)
     elif source_type == SourceTypes.URL:
         return extract_url(url=source, text_only=text_only, local=local)
-    elif source_type == SourceTypes.ZIP:
-        return extract_zip(file_path=source, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only)
     return extract_from_file(file_path=source, source_type=source_type, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only, local=local)
 
 def extract_from_file(file_path: str, source_type: str, verbose: bool = False, ai_extraction: bool = False, text_only: bool = False, local: bool = True, limit: int = None) -> List[Chunk]:
     if not local:
         try:
             with open(file_path, 'rb') as f:
                 response = requests.post(
@@ -82,34 +85,42 @@
         elif source_type == SourceTypes.DOCX:
             extraction = extract_docx(file_path=file_path, verbose=verbose, text_only=text_only)
         elif source_type == SourceTypes.PPTX:
             extraction = extract_pptx(file_path=file_path, verbose=verbose, text_only=text_only)
         elif source_type == SourceTypes.IMAGE:
             extraction = [extract_image(file_path=file_path, text_only=text_only)]
         elif source_type == SourceTypes.SPREADSHEET:
-            extraction = [extract_spreadsheet(file_path=file_path)]
+            extraction = extract_spreadsheet(file_path=file_path)
         elif source_type == SourceTypes.PLAINTEXT:
             extraction = [extract_plaintext(file_path=file_path)]
         elif source_type == SourceTypes.UNCOMPRESSIBLE_CODE:
             extraction = [extract_plaintext(file_path=file_path)]
             extraction = [Chunk(path=e.path, text=e.text, image=None, source_type=SourceTypes.UNCOMPRESSIBLE_CODE) for e in extraction] # change types to code
         elif source_type == SourceTypes.COMPRESSIBLE_CODE:
             extraction = [extract_plaintext(file_path=file_path)]
             extraction = [Chunk(path=e.path, text=e.text, image=None, source_type=SourceTypes.COMPRESSIBLE_CODE) for e in extraction]
         elif source_type == SourceTypes.IPYNB:
             extraction = extract_from_ipynb(file_path=file_path, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only)
+        elif source_type == SourceTypes.ZIP:
+            extraction = extract_zip(file_path=file_path, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only)
+        elif source_type == SourceTypes.VIDEO:
+            extraction = extract_video(file_path=file_path, verbose=verbose, text_only=text_only)
+        elif source_type == SourceTypes.AUDIO:
+            extraction = extract_audio(file_path=file_path, verbose=verbose)
         else:
             extraction = [extract_plaintext(file_path=file_path)]
         if verbose: print_status(f"Extracted from {file_path}", status='success')
         return extraction
     except Exception as e:
         if verbose: print_status(f"Failed to extract from {file_path}: {e}", status='error')
         return [Chunk(path=file_path)]
 
 def detect_type(source: str) -> Optional[SourceTypes]:
+    if source.startswith("https://www.youtube.com"):
+        return SourceTypes.YOUTUBE_VIDEO
     if source.startswith("https://github.com"):
         return SourceTypes.GITHUB
     elif source.startswith("http") or source.startswith("ftp."):
         return SourceTypes.URL
     elif source.endswith(".zip"):
         return SourceTypes.ZIP
     elif os.path.isdir(source) or source == '.' or source == './':
@@ -142,14 +153,20 @@
         return SourceTypes.PDF
     elif extension == '.ipynb':
         return SourceTypes.IPYNB
     elif extension == '.docx':
         return SourceTypes.DOCX
     elif extension == '.pptx':
         return SourceTypes.PPTX
+    elif extension == '.zip':
+        return SourceTypes.ZIP
+    elif extension in VIDEO_EXTENSIONS:
+        return SourceTypes.VIDEO
+    elif extension in AUDIO_EXTENSIONS:
+        return SourceTypes.AUDIO
     elif extension in PLAINTEXT_EXTENSIONS:
         return SourceTypes.PLAINTEXT
     return None
 
 def extract_plaintext(file_path: str) -> List[Chunk]:
     with open(file_path, 'r', encoding='utf-8') as file:
         text = file.read()
@@ -241,23 +258,26 @@
     if text_only:
         import pytesseract # import only if needed
         text = pytesseract.image_to_string(img)
         return Chunk(path=file_path, text=text, image=None, source_type=SourceTypes.IMAGE)
     else:
         return Chunk(path=file_path, text=None, image=img, source_type=SourceTypes.IMAGE)
     
-def extract_spreadsheet(file_path: str) -> Chunk:
+def extract_spreadsheet(file_path: str) -> List[Chunk]:
     import pandas as pd # import only if needed
     if file_path.endswith(".csv"):
         df = pd.read_csv(file_path)
     elif file_path.endswith(".xls") or file_path.endswith(".xlsx"):
         df = pd.read_excel(file_path)
-    dict = df.to_dict(orient='records')
-    json_dict = json.dumps(dict, indent=4, cls=JSONDateEncoder)
-    return Chunk(path=file_path, text=json_dict, image=None, source_type=SourceTypes.SPREADSHEET)
+    dicts = df.to_dict(orient='records')
+    chunks = []
+    for item in dicts:
+        item_json = json.dumps(item, indent=4, cls=JSONDateEncoder)
+        chunks.append(Chunk(path=file_path, text=item_json, image=None, source_type=SourceTypes.SPREADSHEET))
+    return chunks
     
 def extract_url(url: str, text_only: bool = False, local: bool = True, limit: int = None) -> List[Chunk]:
     if not local:
         try:
             response = requests.post(
                 url=API_URL,
                 data={'url': url, 'api_key': THEPIPE_API_KEY, 'text_only': text_only, 'limit': limit}
@@ -308,14 +328,63 @@
             if text:
                 chunks.append(Chunk(path=url, text=text, image=None, source_type=SourceTypes.URL))
             browser.close()
     if not chunks:
         raise ValueError("No content extracted from URL.")
     return chunks
 
+def extract_video(file_path: str, verbose: bool = False, text_only: bool = False) -> List[Chunk]:
+    from moviepy.editor import VideoFileClip # import only if needed
+    import whisper # import only if needed
+    model = whisper.load_model("base")
+    video = VideoFileClip(file_path)
+    chunk_duration = 60
+    num_chunks = math.ceil(video.duration / chunk_duration)
+    chunks = []
+    for i in range(num_chunks):
+        # calculate start and end time for the current chunk
+        start_time = i * chunk_duration
+        end_time = start_time + chunk_duration
+        if end_time > video.duration:
+            end_time = video.duration
+        # extract frame at the middle of the chunk
+        frame_time = (start_time + end_time) / 2
+        frame = video.get_frame(frame_time)
+        image = Image.fromarray(frame)
+        # extract and transcribe audio for the current chunk
+        audio_path = os.path.join(tempfile.gettempdir(), f"temp_audio_{i}.wav")
+        video.subclip(start_time, end_time).audio.write_audiofile(audio_path, codec='pcm_s16le')
+        result = model.transcribe(audio_path, verbose=verbose)
+        transcription = result['text']
+        # add chunk
+        if not text_only:
+            chunks.append(Chunk(path=file_path, text=transcription, image=image, source_type=SourceTypes.VIDEO))
+        else:
+            chunks.append(Chunk(path=file_path, text=transcription, image=None, source_type=SourceTypes.VIDEO))
+        os.remove(audio_path)
+    return chunks
+
+def extract_youtube(youtube_url: str, text_only: bool = False, verbose: bool = False) -> List[Chunk]:
+    from pytube import YouTube # import only if needed
+    temp_dir = "youtube_temp"
+    filename = "temp_video.mp4"
+    yt = YouTube(youtube_url)
+    stream = yt.streams.filter(progressive=True, file_extension='mp4').first()
+    stream.download(temp_dir, filename=filename)
+    video_path = os.path.join(temp_dir, filename)
+    chunks = extract_video(file_path=video_path, verbose=verbose, text_only=text_only)
+    return chunks
+
+def extract_audio(file_path: str, verbose: bool = False) -> List[Chunk]:
+    import whisper # import only if needed
+    model = whisper.load_model("base")
+    result = model.transcribe(file_path, verbose=verbose)
+    transcription = result['text']
+    return [Chunk(path=file_path, text=transcription, image=None, source_type=SourceTypes.AUDIO)]
+
 def extract_github(github_url: str, file_path: str = '', match: Optional[str] = None, ignore: Optional[str] = None, text_only: bool = False, ai_extraction: bool = False, branch: str = 'main', verbose: bool = False) -> List[Chunk]:
     files_contents = []
     if not GITHUB_TOKEN:
         raise ValueError("GITHUB_TOKEN environment variable is not set.")
     # make new tempdir for cloned repo
     with tempfile.TemporaryDirectory() as temp_dir:
         os.system(f"git clone {github_url} {temp_dir} --quiet")
```

### Comparing `thepipe_api-0.3.2/thepipe_api/thepipe.py` & `thepipe_api-0.3.3/thepipe_api/thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.3.2/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.3.3/thepipe_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.3.2
+Version: 0.3.3
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,27 +26,28 @@
 
 
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
 <p>
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
-[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
+[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-access-blue)</a>
 
-### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
+### Feed PDFs, web pages, word docs, slides, videos, CSV, and more into Vision-LLMs with one line of code ⚡
 
 The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. 
 
-![Demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/grader.py%20(6).png)
+![Science assistant demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/science_assistantpy2.png)
+
 
 ## Features 🌟
 
 - Extracts text and visuals from files or web pages 📚
-- Outputs chunks optimized for multimodal LLMs 🖼️
-- Interpret complex PDFs, web pages, slides, CSVs, and more 🧠
+- Outputs chunks optimized for multimodal LLMs and RAG frameworks 🖼️
+- Interpret complex PDFs, web pages, docs, videos, data, and more 🧠
 - Auto-compress prompts exceeding your chosen token limit 📦
 - Works even with missing file extensions, in-memory data streams 💾
 - Works with codebases, git repos, and custom integrations 🌐
 - Multi-threaded ⚡️
 
 ## Getting Started  🚀
 
@@ -60,15 +61,15 @@
 The Pipe is available as a hosted API, or it can be set up locally. An API key is recommended for out-of-the-box functionality (alternatively, see the local installation section). Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have a key yet? [Get one here](https://thepi.pe).
 
 Now you can extract comprehensive text and visuals from any file:
 ```python
 from thepipe_api import thepipe
 messages = thepipe.extract("example.pdf")
 ```
-Or any website:
+Or websites:
 ```python
 messages = thepipe.extract("https://example.com")
 ```
 Then feed it into GPT-4-Vision:
 ```python
 response = client.chat.completions.create(
     model="gpt-4-vision-preview",
@@ -79,29 +80,33 @@
 ![Just call OpenAI](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/IMG_0180.jpg)
 
 You can also use The Pipe from the command line. Here's how to recursively extract from a directory, matching only files containing a substring (in this example, typescript files) and ignore files containing other substrings (in this example, anything in the "tests" folder):
 ```bash
 thepipe path/to/folder --match tsx --ignore tests
 ```
 
+
 ## Supported File Types 📚
 
 | Source Type                           | Input types        | Token Compression 🗜️ | Image Extraction 👁️ | Notes 📌                                                  |
 |---------------------------------------|------------------------------------------|-------------------|------------------|---------------------------------------------------------|
 | Directory                             | Any `/path/to/directory`                 | ✔️               | ✔️               | Extracts from all files in directory, supports match and ignore patterns |
 | Code                                  | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | ✔️ (varies)   | ❌               | Combines all code files. `.c`, `.cpp`, `.py` are compressible with ctags, others are not |
 | Plaintext                             | `.txt`, `.md`, `.rtf`, etc               | ✔️               | ❌               | Regular text files                                                      |
 | PDF                                   | `.pdf`                                  | ✔️               | ✔️    | Extracts text and images of each page; can use AI for extraction of table data and  images within pages |
 | Image                                 | `.jpg`, `.jpeg`, `.png` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
 | Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
+| Video                                 | `.mp4`, `.avi`, `.mov`, `.wmv`     | ✔️               | ✔️                | Extracts frames from video files; supports frame extraction and OCR for text extraction from frames |
+| Audio                                 | `.mp3`, `.wav`          | ✔️               | ❌                | Extracts text from audio files; supports speech-to-text conversion        | 
 | Website                               | URLs (inputs containing `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
+| YouTube Video                         | YouTube video URLs                      | ✔️               | ✔️                | Extracts text from YouTube videos; supports subtitles extraction          |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
 ## How it works 🛠️
 
 The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible list of multimodal messages representing chunks of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned should look like this:
 ```json
 [
@@ -119,20 +124,22 @@
         }
       }
     ]
   }
 ]
 ```
 If you want to feed these messages directly into the model, it is important to be mindful of the token limit.
-OpenAI does not allow too many images in the prompt (see discussion [here](https://community.openai.com/t/gpt-4-vision-maximum-amount-of-images/573110/6)), so long files should be extracted with `text_only=True` to avoid this issue. 
+OpenAI does not allow too many images in the prompt (see discussion [here](https://community.openai.com/t/gpt-4-vision-maximum-amount-of-images/573110/6)), so long files should be extracted with `text_only=True` to avoid this issue, while long text files should either be compressed or embedded in a RAG framework.
 
 The text and images from these messages may also be prepared for a vector database with `thepipe.core.create_chunks_from_messages` or for downstream use with RAG frameworks. [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider. 
 
 It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), opt-in AI [table, equation, and figure extraction](https://thepi.pe/pricing), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
 
+![Demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/grader.py%20(6).png)
+
 
 ## Local Installation 🛠️
 
 The Pipe handles a wide array of complex filetypes, and thus requires installation of many different packages to function. It also requires a very capable machine for good response times. For this reason, we host it as an API that works out-of-the-box. To use The Pipe locally for free instead, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements:
 
 ```bash
 git clone https://github.com/emcf/thepipe
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.3.2 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.3.3 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
@@ -11,100 +11,108 @@
 _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
 _E_n_g_l_i_s_h | _ä_¸_­_æ__
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/
 badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
 action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
-_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
-docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
-Pipe is a multimodal-first tool for feeding files and web pages into vision-
-language models such as GPT-4V. It is best for LLM and RAG applications that
-require a deep understanding of tricky data sources. The Pipe is available as a
-hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. !
-[Demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/
-assets/grader.py%20(6).png) ## Features ð - Extracts text and visuals from
-files or web pages ð - Outputs chunks optimized for multimodal LLMs ð¼ï¸
-- Interpret complex PDFs, web pages, slides, CSVs, and more ð§  - Auto-
-compress prompts exceeding your chosen token limit ð¦ - Works even with
-missing file extensions, in-memory data streams ð¾ - Works with codebases,
-git repos, and custom integrations ð - Multi-threaded â¡ï¸ ## Getting
-Started ð The Pipe handles a wide array of complex filetypes, and thus has
-many dependencies that must be installed separately. It also requires a strong
-machine for good response times. For this reason, we host it as an API that
-works out-of-the-box. First, install The Pipe. ``` pip install thepipe_api ```
-The Pipe is available as a hosted API, or it can be set up locally. An API key
-is recommended for out-of-the-box functionality (alternatively, see the local
-installation section). Ensure the `THEPIPE_API_KEY` environment variable is
-set. Don't have a key yet? [Get one here](https://thepi.pe). Now you can
-extract comprehensive text and visuals from any file: ```python from
-thepipe_api import thepipe messages = thepipe.extract("example.pdf") ``` Or any
-website: ```python messages = thepipe.extract("https://example.com") ``` Then
-feed it into GPT-4-Vision: ```python response = client.chat.completions.create
-( model="gpt-4-vision-preview", messages = messages, ) ``` ![Just call OpenAI]
-(https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/
-IMG_0180.jpg) You can also use The Pipe from the command line. Here's how to
-recursively extract from a directory, matching only files containing a
-substring (in this example, typescript files) and ignore files containing other
-substrings (in this example, anything in the "tests" folder): ```bash thepipe
-path/to/folder --match tsx --ignore tests ``` ## Supported File Types ð |
-Source Type | Input types | Token Compression ðï¸ | Image Extraction
-ðï¸ | Notes ð | |---------------------------------------|---------------
----------------------------|-------------------|------------------|------------
----------------------------------------------| | Directory | Any `/path/to/
-directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
-match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
-`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
-`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
-`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
-âï¸ | âï¸ | Extracts text and images of each page; can use AI for
-extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
-`.png` | â | âï¸ | Extracts images, uses OCR if text_only | | Data Table |
-`.csv`, `.xls`, `.xlsx` | âï¸ | â | Extracts data from spreadsheets;
-converts to text representation. For very large datasets, will only extract
-column names and types | | Jupyter Notebook | `.ipynb` | â | âï¸ |
-Extracts code, markdown, and images from Jupyter notebooks | | Microsoft Word
-Document | `.docx` | âï¸ | âï¸ | Extracts text and images from Word
-documents | | Microsoft PowerPoint Presentation | `.pptx` | âï¸ | âï¸ |
-Extracts text and images from PowerPoint presentations | | Website | URLs
-(inputs containing `http`, `https`, `ftp`) | âï¸ | âï¸ | Extracts text
-from web page along with image (or images if scrollable); text-only extraction
-available | | GitHub Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts
-from GitHub repositories; supports branch specification | | ZIP File | `.zip` |
-âï¸ | âï¸ | Extracts contents of ZIP files; supports nested directory
-extraction | ## How it works ð ï¸ The input source is either a file path, a
-URL, or a directory. The pipe will extract information from the source and
-process it for downstream use with [language models](https://en.wikipedia.org/
-wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/
-wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/
-2304.00685). The output from the pipe is a sensible list of multimodal messages
-representing chunks of the extracted information, carefully crafted to fit
-within context windows for any models from [gemma-7b](https://huggingface.co/
-google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned
-should look like this: ```json [ { "role": "user", "content": [ { "type":
-"text", "text": "..." }, { "type": "image_url", "image_url": { "url": "data:
-image/jpeg;base64,..." } } ] } ] ``` If you want to feed these messages
-directly into the model, it is important to be mindful of the token limit.
-OpenAI does not allow too many images in the prompt (see discussion [here]
-(https://community.openai.com/t/gpt-4-vision-maximum-amount-of-images/573110/
-6)), so long files should be extracted with `text_only=True` to avoid this
-issue. The text and images from these messages may also be prepared for a
-vector database with `thepipe.core.create_chunks_from_messages` or for
-downstream use with RAG frameworks. [LiteLLM](https://github.com/BerriAI/
-litellm) can be used to easily integrate The Pipe with any LLM provider. It
-uses a variety of heuristics for optimal performance with vision-language
-models, including AI filetype detection with [filetype detection](https://
-opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-
-type-identification.html), opt-in AI [table, equation, and figure extraction]
-(https://thepi.pe/pricing), efficient [token compression](https://arxiv.org/
-abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/
-Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle]
-(https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work
-out-of-the-box. ## Local Installation ð ï¸ The Pipe handles a wide array of
-complex filetypes, and thus requires installation of many different packages to
+_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, web pages,
+word docs, slides, videos, CSV, and more into Vision-LLMs with one line of code
+â¡ The Pipe is a multimodal-first tool for feeding files and web pages into
+vision-language models such as GPT-4V. It is best for LLM and RAG applications
+that require a deep understanding of tricky data sources. The Pipe is available
+as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. !
+[Science assistant demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/
+object/public/assets/science_assistantpy2.png) ## Features ð - Extracts text
+and visuals from files or web pages ð - Outputs chunks optimized for
+multimodal LLMs and RAG frameworks ð¼ï¸ - Interpret complex PDFs, web pages,
+docs, videos, data, and more ð§  - Auto-compress prompts exceeding your chosen
+token limit ð¦ - Works even with missing file extensions, in-memory data
+streams ð¾ - Works with codebases, git repos, and custom integrations ð -
+Multi-threaded â¡ï¸ ## Getting Started ð The Pipe handles a wide array of
+complex filetypes, and thus has many dependencies that must be installed
+separately. It also requires a strong machine for good response times. For this
+reason, we host it as an API that works out-of-the-box. First, install The
+Pipe. ``` pip install thepipe_api ``` The Pipe is available as a hosted API, or
+it can be set up locally. An API key is recommended for out-of-the-box
+functionality (alternatively, see the local installation section). Ensure the
+`THEPIPE_API_KEY` environment variable is set. Don't have a key yet? [Get one
+here](https://thepi.pe). Now you can extract comprehensive text and visuals
+from any file: ```python from thepipe_api import thepipe messages =
+thepipe.extract("example.pdf") ``` Or websites: ```python messages =
+thepipe.extract("https://example.com") ``` Then feed it into GPT-4-Vision:
+```python response = client.chat.completions.create( model="gpt-4-vision-
+preview", messages = messages, ) ``` ![Just call OpenAI](https://
+rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/IMG_0180.jpg)
+You can also use The Pipe from the command line. Here's how to recursively
+extract from a directory, matching only files containing a substring (in this
+example, typescript files) and ignore files containing other substrings (in
+this example, anything in the "tests" folder): ```bash thepipe path/to/folder -
+-match tsx --ignore tests ``` ## Supported File Types ð | Source Type |
+Input types | Token Compression ðï¸ | Image Extraction ðï¸ | Notes ð
+| |---------------------------------------|------------------------------------
+------|-------------------|------------------|---------------------------------
+------------------------| | Directory | Any `/path/to/directory` | âï¸ |
+âï¸ | Extracts from all files in directory, supports match and ignore
+patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | âï¸
+(varies) | â | Combines all code files. `.c`, `.cpp`, `.py` are compressible
+with ctags, others are not | | Plaintext | `.txt`, `.md`, `.rtf`, etc | âï¸
+| â | Regular text files | | PDF | `.pdf` | âï¸ | âï¸ | Extracts text
+and images of each page; can use AI for extraction of table data and images
+within pages | | Image | `.jpg`, `.jpeg`, `.png` | â | âï¸ | Extracts
+images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx` | âï¸
+| â | Extracts data from spreadsheets; converts to text representation. For
+very large datasets, will only extract column names and types | | Jupyter
+Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown, and images from
+Jupyter notebooks | | Microsoft Word Document | `.docx` | âï¸ | âï¸ |
+Extracts text and images from Word documents | | Microsoft PowerPoint
+Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images from
+PowerPoint presentations | | Video | `.mp4`, `.avi`, `.mov`, `.wmv` | âï¸ |
+âï¸ | Extracts frames from video files; supports frame extraction and OCR
+for text extraction from frames | | Audio | `.mp3`, `.wav` | âï¸ | â |
+Extracts text from audio files; supports speech-to-text conversion | | Website
+| URLs (inputs containing `http`, `https`, `ftp`) | âï¸ | âï¸ | Extracts
+text from web page along with image (or images if scrollable); text-only
+extraction available | | GitHub Repository | GitHub repo URLs | âï¸ | âï¸
+| Extracts from GitHub repositories; supports branch specification | | YouTube
+Video | YouTube video URLs | âï¸ | âï¸ | Extracts text from YouTube
+videos; supports subtitles extraction | | ZIP File | `.zip` | âï¸ | âï¸ |
+Extracts contents of ZIP files; supports nested directory extraction | ## How
+it works ð ï¸ The input source is either a file path, a URL, or a directory.
+The pipe will extract information from the source and process it for downstream
+use with [language models](https://en.wikipedia.org/wiki/Large_language_model),
+[vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or
+[vision-language models](https://arxiv.org/abs/2304.00685). The output from the
+pipe is a sensible list of multimodal messages representing chunks of the
+extracted information, carefully crafted to fit within context windows for any
+models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4]
+(https://openai.com/gpt-4). The messages returned should look like this:
+```json [ { "role": "user", "content": [ { "type": "text", "text": "..." },
+{ "type": "image_url", "image_url": { "url": "data:image/jpeg;base64,..." } } ]
+} ] ``` If you want to feed these messages directly into the model, it is
+important to be mindful of the token limit. OpenAI does not allow too many
+images in the prompt (see discussion [here](https://community.openai.com/t/gpt-
+4-vision-maximum-amount-of-images/573110/6)), so long files should be extracted
+with `text_only=True` to avoid this issue, while long text files should either
+be compressed or embedded in a RAG framework. The text and images from these
+messages may also be prepared for a vector database with
+`thepipe.core.create_chunks_from_messages` or for downstream use with RAG
+frameworks. [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily
+integrate The Pipe with any LLM provider. It uses a variety of heuristics for
+optimal performance with vision-language models, including AI filetype
+detection with [filetype detection](https://opensource.googleblog.com/2024/02/
+magika-ai-powered-fast-and-efficient-file-type-identification.html), opt-in AI
+[table, equation, and figure extraction](https://thepi.pe/pricing), efficient
+[token compression](https://arxiv.org/abs/2403.12968), automatic [image
+encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/
+abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172)
+effects, and more, all pre-built to work out-of-the-box. ![Demo](https://
+rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/grader.py%20
+(6).png) ## Local Installation ð ï¸ The Pipe handles a wide array of complex
+filetypes, and thus requires installation of many different packages to
 function. It also requires a very capable machine for good response times. For
 this reason, we host it as an API that works out-of-the-box. To use The Pipe
 locally for free instead, you will need [playwright](https://github.com/
 microsoft/playwright), [ctags](https://github.com/universal-ctags/),
 [pytesseract](https://github.com/h/pytesseract), and the local python
 requirements, which differ from the more lightweight API requirements: ```bash
 git clone https://github.com/emcf/thepipe pip install -r requirements_local.txt
```

