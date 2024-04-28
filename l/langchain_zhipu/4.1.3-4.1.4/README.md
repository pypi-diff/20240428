# Comparing `tmp/langchain_zhipu-4.1.3.tar.gz` & `tmp/langchain_zhipu-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_zhipu-4.1.3.tar", max compression
+gzip compressed data, was "langchain_zhipu-4.1.4.tar", max compression
```

## Comparing `langchain_zhipu-4.1.3.tar` & `langchain_zhipu-4.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     4221 2024-04-19 01:27:50.154822 langchain_zhipu-4.1.3/README.md
--rw-r--r--   0        0        0      971 2024-04-20 11:17:13.232062 langchain_zhipu-4.1.3/langchain_zhipu/__init__.py
--rw-r--r--   0        0        0       23 2024-04-26 14:01:10.986554 langchain_zhipu-4.1.3/langchain_zhipu/__version__.py
--rw-r--r--   0        0        0        0 2024-03-28 15:37:31.905694 langchain_zhipu-4.1.3/langchain_zhipu/http/__init__.py
--rw-r--r--   0        0        0     4844 2024-04-20 11:05:25.768200 langchain_zhipu-4.1.3/langchain_zhipu/http/api.py
--rw-r--r--   0        0        0    13692 2024-04-26 13:59:03.840626 langchain_zhipu-4.1.3/langchain_zhipu/http/base.py
--rw-r--r--   0        0        0     7825 2024-04-13 06:21:17.673386 langchain_zhipu-4.1.3/langchain_zhipu/http/chat.py
--rw-r--r--   0        0        0     1714 2024-04-13 03:17:37.336032 langchain_zhipu-4.1.3/langchain_zhipu/http/embeddings.py
--rw-r--r--   0        0        0      500 2024-04-02 14:02:48.067993 langchain_zhipu-4.1.3/langchain_zhipu/http/enum.py
--rw-r--r--   0        0        0      382 2024-04-09 02:22:51.583321 langchain_zhipu-4.1.3/langchain_zhipu/http/env.py
--rw-r--r--   0        0        0     8994 2024-04-09 02:58:49.863351 langchain_zhipu-4.1.3/langchain_zhipu/http/manager.py
--rw-r--r--   0        0        0     4099 2024-04-06 13:39:34.256771 langchain_zhipu-4.1.3/langchain_zhipu/http/types.py
--rw-r--r--   0        0        0     1721 2024-03-26 15:19:10.785090 langchain_zhipu-4.1.3/langchain_zhipu/utils.py
--rw-r--r--   0        0        0      750 2024-04-26 14:01:14.853856 langchain_zhipu-4.1.3/pyproject.toml
--rw-r--r--   0        0        0     5066 1970-01-01 00:00:00.000000 langchain_zhipu-4.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-04-27 10:59:34.588160 langchain_zhipu-4.1.4/README.md
+-rw-r--r--   0        0        0      971 2024-04-20 11:17:13.232062 langchain_zhipu-4.1.4/langchain_zhipu/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-28 12:05:07.296315 langchain_zhipu-4.1.4/langchain_zhipu/__version__.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:37:31.905694 langchain_zhipu-4.1.4/langchain_zhipu/http/__init__.py
+-rw-r--r--   0        0        0     4844 2024-04-20 11:05:25.768200 langchain_zhipu-4.1.4/langchain_zhipu/http/api.py
+-rw-r--r--   0        0        0    13692 2024-04-26 13:59:03.840626 langchain_zhipu-4.1.4/langchain_zhipu/http/base.py
+-rw-r--r--   0        0        0     7825 2024-04-13 06:21:17.673386 langchain_zhipu-4.1.4/langchain_zhipu/http/chat.py
+-rw-r--r--   0        0        0     1714 2024-04-13 03:17:37.336032 langchain_zhipu-4.1.4/langchain_zhipu/http/embeddings.py
+-rw-r--r--   0        0        0      500 2024-04-02 14:02:48.067993 langchain_zhipu-4.1.4/langchain_zhipu/http/enum.py
+-rw-r--r--   0        0        0      382 2024-04-09 02:22:51.583321 langchain_zhipu-4.1.4/langchain_zhipu/http/env.py
+-rw-r--r--   0        0        0     8994 2024-04-09 02:58:49.863351 langchain_zhipu-4.1.4/langchain_zhipu/http/manager.py
+-rw-r--r--   0        0        0     4099 2024-04-06 13:39:34.256771 langchain_zhipu-4.1.4/langchain_zhipu/http/types.py
+-rw-r--r--   0        0        0     1721 2024-03-26 15:19:10.785090 langchain_zhipu-4.1.4/langchain_zhipu/utils.py
+-rw-r--r--   0        0        0      788 2024-04-28 12:04:59.434736 langchain_zhipu-4.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5163 1970-01-01 00:00:00.000000 langchain_zhipu-4.1.4/PKG-INFO
```

### Comparing `langchain_zhipu-4.1.3/README.md` & `langchain_zhipu-4.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 
 # 使用
 
 ## 配置
 
 可以将申请到的 `API_KEY` 配置到环境变量 `ZHIPUAI_API_KEY`。
 
-建议使用 `.env` 文件来管理环境变量，这可能安装 `dotenv` 包：
+建议使用 `.env` 文件来管理环境变量，这需要安装 `python_dotenv` 包：
 
 ```bash
-pip install dotenv
+pip install python_dotenv
 ```
 
 你的 .env 文件：
 
 ```
 ZHIPUAI_API_KEY="你的KEY"
 ```
```

### Comparing `langchain_zhipu-4.1.3/langchain_zhipu/__init__.py` & `langchain_zhipu-4.1.4/langchain_zhipu/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.3/langchain_zhipu/http/api.py` & `langchain_zhipu-4.1.4/langchain_zhipu/http/api.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.3/langchain_zhipu/http/base.py` & `langchain_zhipu-4.1.4/langchain_zhipu/http/base.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.3/langchain_zhipu/http/chat.py` & `langchain_zhipu-4.1.4/langchain_zhipu/http/chat.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.3/langchain_zhipu/http/embeddings.py` & `langchain_zhipu-4.1.4/langchain_zhipu/http/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.3/langchain_zhipu/http/manager.py` & `langchain_zhipu-4.1.4/langchain_zhipu/http/manager.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.3/langchain_zhipu/http/types.py` & `langchain_zhipu-4.1.4/langchain_zhipu/http/types.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.3/langchain_zhipu/utils.py` & `langchain_zhipu-4.1.4/langchain_zhipu/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.3/PKG-INFO` & `langchain_zhipu-4.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_zhipu
-Version: 4.1.3
+Version: 4.1.4
 Summary: 将智谱AI集成到LangChain
 Home-page: https://github.com/arcstep/langchain_zhipuai
 License: MIT
 Author: arcstep
 Author-email: 43801@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cachetools (==4.2.2)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: langchain (>=0.1.0,<0.2.0)
 Requires-Dist: pydantic (>=1,<3)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
+Requires-Dist: regex (>=2024.4.16,<2025.0.0)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Project-URL: Repository, https://github.com/arcstep/langchain_zhipuai.git
 Description-Content-Type: text/markdown
 
 # 为什么要开发这个包？
 [![PyPI version](https://img.shields.io/pypi/v/langchain_zhipu.svg)](https://pypi.org/project/langchain_zhipu/)
 
 为了方便在 langchain 中使用，langchain_zhipu 直接使用官方HTTP接口实现，并避免了如下的现存问题：
@@ -54,18 +56,18 @@
 
 # 使用
 
 ## 配置
 
 可以将申请到的 `API_KEY` 配置到环境变量 `ZHIPUAI_API_KEY`。
 
-建议使用 `.env` 文件来管理环境变量，这可能安装 `dotenv` 包：
+建议使用 `.env` 文件来管理环境变量，这需要安装 `python_dotenv` 包：
 
 ```bash
-pip install dotenv
+pip install python_dotenv
 ```
 
 你的 .env 文件：
 
 ```
 ZHIPUAI_API_KEY="你的KEY"
 ```
```

