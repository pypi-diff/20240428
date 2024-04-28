# Comparing `tmp/langtrace_python_sdk-2.0.0.tar.gz` & `tmp/langtrace_python_sdk-2.0.1.tar.gz`

## Comparing `langtrace_python_sdk-2.0.0.tar` & `langtrace_python_sdk-2.0.1.tar`

### file list

```diff
@@ -1,107 +1,122 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/cohere_example/__init__.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/cohere_example/chat.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/cohere_example/chat_stream.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/cohere_example/embed.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/cohere_example/rerank.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/cohere_example/tools.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/fastapi_example/basic_route.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/hiveagent_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/agent.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/__init__.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/async_tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/async_tool_calling_streaming.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/chat_completion.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/embeddings_create.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/function_calling.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/images_generate.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/tool_calling.py
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/openai_example/tool_calling_streaming.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/perplexity_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/cohere.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0    26381 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/cohere/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    36773 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/conftest.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/utils.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/anthropic/conftest.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/anthropic/test_anthropic.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/anthropic/cassettes/test_anthropic.yaml
--rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/langchain/test_langchain.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/langchain/test_langchain_community.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/langchain/test_langchain_core.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/conftest.py
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/test_embeddings.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_async_image_generation.yaml
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_image_generation.yaml
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/LICENSE
--rw-r--r--   0        0        0     8031 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/README.md
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     9243 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/cohere_example/embed.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/cohere_example/rerank.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/cohere_example/tools.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/hiveagent_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/langchain_example/groq_example.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/langchain_example/langgraph_example.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/agent.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/__init__.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/async_tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/async_tool_calling_streaming.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/chat_completion.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/embeddings_create.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/function_calling.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/images_generate.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/tool_calling.py
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/tool_calling_streaming.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/qdrant_example/__init__.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/qdrant_example/basic.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/groq.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    26381 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
+-rw-r--r--   0        0        0    25572 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/groq/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    36773 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/conftest.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/utils.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/anthropic/conftest.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/anthropic/cassettes/test_anthropic.yaml
+-rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/langchain/test_langchain_community.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/langchain/test_langchain_core.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/conftest.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/test_embeddings.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_async_image_generation.yaml
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_image_generation.yaml
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/LICENSE
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/README.md
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/PKG-INFO
```

### Comparing `langtrace_python_sdk-2.0.0/src/run_example.py` & `langtrace_python_sdk-2.0.1/src/run_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-2.0.1/src/examples/anthropic_example/completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-2.0.1/src/examples/chroma_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/cohere_example/chat.py` & `langtrace_python_sdk-2.0.1/src/examples/cohere_example/chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/cohere_example/chat_stream.py` & `langtrace_python_sdk-2.0.1/src/examples/cohere_example/chat_stream.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/cohere_example/embed.py` & `langtrace_python_sdk-2.0.1/src/examples/cohere_example/embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/cohere_example/rerank.py` & `langtrace_python_sdk-2.0.1/src/examples/cohere_example/rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/cohere_example/tools.py` & `langtrace_python_sdk-2.0.1/src/examples/cohere_example/tools.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/fastapi_example/basic_route.py` & `langtrace_python_sdk-2.0.1/src/examples/fastapi_example/basic_route.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-2.0.1/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-2.0.1/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/agent.py` & `langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/agent.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/openai_example/async_tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.1/src/examples/openai_example/async_tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/openai_example/async_tool_calling_streaming.py` & `langtrace_python_sdk-2.0.1/src/examples/openai_example/async_tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/openai_example/chat_completion.py` & `langtrace_python_sdk-2.0.1/src/examples/openai_example/chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/openai_example/function_calling.py` & `langtrace_python_sdk-2.0.1/src/examples/openai_example/function_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/openai_example/tool_calling.py` & `langtrace_python_sdk-2.0.1/src/examples/openai_example/tool_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/openai_example/tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.1/src/examples/openai_example/tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/openai_example/tool_calling_streaming.py` & `langtrace_python_sdk-2.0.1/src/examples/openai_example/tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/perplexity_example/basic.py` & `langtrace_python_sdk-2.0.1/src/examples/perplexity_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-2.0.1/src/examples/pinecone_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/__init__.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/langtrace.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/langtrace.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,26 +26,32 @@
     LangTraceExporter
 from langtrace_python_sdk.instrumentation.anthropic.instrumentation import \
     AnthropicInstrumentation
 from langtrace_python_sdk.instrumentation.chroma.instrumentation import \
     ChromaInstrumentation
 from langtrace_python_sdk.instrumentation.cohere.instrumentation import \
     CohereInstrumentation
+from langtrace_python_sdk.instrumentation.groq.instrumentation import \
+    GroqInstrumentation
 from langtrace_python_sdk.instrumentation.langchain.instrumentation import \
     LangchainInstrumentation
 from langtrace_python_sdk.instrumentation.langchain_community.instrumentation import \
     LangchainCommunityInstrumentation
 from langtrace_python_sdk.instrumentation.langchain_core.instrumentation import \
     LangchainCoreInstrumentation
+from langtrace_python_sdk.instrumentation.langgraph.instrumentation import \
+    LanggraphInstrumentation
 from langtrace_python_sdk.instrumentation.llamaindex.instrumentation import \
     LlamaindexInstrumentation
 from langtrace_python_sdk.instrumentation.openai.instrumentation import \
     OpenAIInstrumentation
 from langtrace_python_sdk.instrumentation.pinecone.instrumentation import \
     PineconeInstrumentation
+from langtrace_python_sdk.instrumentation.qdrant.instrumentation import \
+    QdrantInstrumentation
 
 
 def init(
     api_key: str = None,
     batch: bool = True,
     write_to_langtrace_cloud: bool = True,
     custom_remote_exporter=None,
@@ -77,26 +83,32 @@
         else:
             provider.add_span_processor(simple_processor_console)
 
     # Initialize tracer
     trace.set_tracer_provider(provider)
 
     openai_instrumentation = OpenAIInstrumentation()
+    groq_instrumentation = GroqInstrumentation()
     pinecone_instrumentation = PineconeInstrumentation()
     llamaindex_instrumentation = LlamaindexInstrumentation()
     chroma_instrumentation = ChromaInstrumentation()
+    qdrant_instrumentation = QdrantInstrumentation()
     langchain_instrumentation = LangchainInstrumentation()
     langchain_core_instrumentation = LangchainCoreInstrumentation()
     langchain_community_instrumentation = LangchainCommunityInstrumentation()
+    langgraph_instrumentation = LanggraphInstrumentation()
     anthropic_instrumentation = AnthropicInstrumentation()
     cohere_instrumentation = CohereInstrumentation()
 
     # Call the instrument method with some arguments
     openai_instrumentation.instrument()
+    groq_instrumentation.instrument()
     pinecone_instrumentation.instrument()
     llamaindex_instrumentation.instrument()
     chroma_instrumentation.instrument()
+    qdrant_instrumentation.instrument()
     langchain_instrumentation.instrument()
     langchain_core_instrumentation.instrument()
     langchain_community_instrumentation.instrument()
+    langgraph_instrumentation.instrument()
     anthropic_instrumentation.instrument()
     cohere_instrumentation.instrument()
```

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/cohere.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/cohere.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,18 +6,21 @@
     "gpt-4-1106-vision-preview": "cl100k_base",
 }
 
 SERVICE_PROVIDERS = {
     "ANTHROPIC": "Anthropic",
     "AZURE": "Azure",
     "CHROMA": "Chroma",
+    "GROQ": "Groq",
     "LANGCHAIN": "Langchain",
     "LANGCHAIN_COMMUNITY": "Langchain Community",
     "LANGCHAIN_CORE": "Langchain Core",
+    "LANGGRAPH": "Langgraph",
     "LLAMAINDEX": "LlamaIndex",
     "OPENAI": "OpenAI",
     "PINECONE": "Pinecone",
     "COHERE": "Cohere",
     "PPLX": "Perplexity",
+    "QDRANT": "Qdrant",
 }
 
 LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY = "langtrace_additional_attributes"
```

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/cohere/patch.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/cohere/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/utils/llm.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/langtrace_python_sdk/utils/with_root_span.py` & `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/utils/with_root_span.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/conftest.py` & `langtrace_python_sdk-2.0.1/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/utils.py` & `langtrace_python_sdk-2.0.1/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/anthropic/conftest.py` & `langtrace_python_sdk-2.0.1/src/tests/anthropic/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/anthropic/test_anthropic.py` & `langtrace_python_sdk-2.0.1/src/tests/anthropic/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/anthropic/cassettes/test_anthropic.yaml` & `langtrace_python_sdk-2.0.1/src/tests/anthropic/cassettes/test_anthropic.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml` & `langtrace_python_sdk-2.0.1/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml` & `langtrace_python_sdk-2.0.1/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-2.0.1/src/tests/chroma/test_chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/langchain/test_langchain.py` & `langtrace_python_sdk-2.0.1/src/tests/langchain/test_langchain.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/langchain/test_langchain_community.py` & `langtrace_python_sdk-2.0.1/src/tests/langchain/test_langchain_community.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/langchain/test_langchain_core.py` & `langtrace_python_sdk-2.0.1/src/tests/langchain/test_langchain_core.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/openai/conftest.py` & `langtrace_python_sdk-2.0.1/src/tests/openai/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-2.0.1/src/tests/openai/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-2.0.1/src/tests/openai/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_async_image_generation.yaml` & `langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_async_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_chat_completion.yaml` & `langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_chat_completion.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/openai/cassettes/test_image_generation.yaml` & `langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/src/tests/pinecone/test_pinecone.py` & `langtrace_python_sdk-2.0.1/src/tests/pinecone/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/.gitignore` & `langtrace_python_sdk-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/LICENSE` & `langtrace_python_sdk-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.0/README.md` & `langtrace_python_sdk-2.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -184,24 +184,26 @@
    api_call2()
 ```
 
 ## Supported integrations
 
 Langtrace automatically captures traces from the following vendors:
 
-| Vendor | Type | Typescript SDK | Python SDK
-| ------ | ------ | ------ | ------ |
-| OpenAI | LLM | :white_check_mark: | :white_check_mark: |
-| Anthropic | LLM | :white_check_mark: | :white_check_mark: |
-| Cohere | LLM | :x: | :white_check_mark: |
-| Azure OpenAI | LLM | :white_check_mark: | :white_check_mark: |
-| Langchain | Framework | :x: | :white_check_mark: |
-| LlamaIndex | Framework | :white_check_mark: | :white_check_mark: |
-| Pinecone | Vector Database | :white_check_mark: | :white_check_mark: |
-| ChromaDB | Vector Database | :white_check_mark: | :white_check_mark: |
+| Vendor       | Type            | Typescript SDK     | Python SDK         |
+| ------------ | --------------- | ------------------ | ------------------ |
+| OpenAI       | LLM             | :white_check_mark: | :white_check_mark: |
+| Anthropic    | LLM             | :white_check_mark: | :white_check_mark: |
+| Azure OpenAI | LLM             | :white_check_mark: | :white_check_mark: |
+| Cohere       | LLM             | :white_check_mark: | :white_check_mark: |
+| Groq         | LLM             | :x:                | :white_check_mark: |
+| Langchain    | Framework       | :x:                | :white_check_mark: |
+| LlamaIndex   | Framework       | :white_check_mark: | :white_check_mark: |
+| Pinecone     | Vector Database | :white_check_mark: | :white_check_mark: |
+| ChromaDB     | Vector Database | :white_check_mark: | :white_check_mark: |
+| QDrant       | Vector Database | :x:                | :white_check_mark: |
 
 ---
 
 ## Feature Requests and Issues
 
 - To request for features, head over [here to start a discussion](https://github.com/Scale3-Labs/langtrace/discussions/categories/feature-requests).
 - To raise an issue, head over [here and create an issue](https://github.com/Scale3-Labs/langtrace/issues).
```

### Comparing `langtrace_python_sdk-2.0.0/pyproject.toml` & `langtrace_python_sdk-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 license = "Apache-2.0"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  'trace-attributes==3.0.2',
+  'trace-attributes==3.0.5',
   'opentelemetry-api',
   'opentelemetry-sdk',
   'opentelemetry-instrumentation',
   'pinecone-client',
   'tiktoken'
 ]
```

### Comparing `langtrace_python_sdk-2.0.0/PKG-INFO` & `langtrace_python_sdk-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-sdk
 Requires-Dist: pinecone-client
 Requires-Dist: tiktoken
-Requires-Dist: trace-attributes==3.0.2
+Requires-Dist: trace-attributes==3.0.5
 Provides-Extra: dev
 Requires-Dist: anthropic; extra == 'dev'
 Requires-Dist: chromadb; extra == 'dev'
 Requires-Dist: cohere; extra == 'dev'
 Requires-Dist: langchain; extra == 'dev'
 Requires-Dist: langchain-openai; extra == 'dev'
 Requires-Dist: llama-index; extra == 'dev'
@@ -217,24 +217,26 @@
    api_call2()
 ```
 
 ## Supported integrations
 
 Langtrace automatically captures traces from the following vendors:
 
-| Vendor | Type | Typescript SDK | Python SDK
-| ------ | ------ | ------ | ------ |
-| OpenAI | LLM | :white_check_mark: | :white_check_mark: |
-| Anthropic | LLM | :white_check_mark: | :white_check_mark: |
-| Cohere | LLM | :x: | :white_check_mark: |
-| Azure OpenAI | LLM | :white_check_mark: | :white_check_mark: |
-| Langchain | Framework | :x: | :white_check_mark: |
-| LlamaIndex | Framework | :white_check_mark: | :white_check_mark: |
-| Pinecone | Vector Database | :white_check_mark: | :white_check_mark: |
-| ChromaDB | Vector Database | :white_check_mark: | :white_check_mark: |
+| Vendor       | Type            | Typescript SDK     | Python SDK         |
+| ------------ | --------------- | ------------------ | ------------------ |
+| OpenAI       | LLM             | :white_check_mark: | :white_check_mark: |
+| Anthropic    | LLM             | :white_check_mark: | :white_check_mark: |
+| Azure OpenAI | LLM             | :white_check_mark: | :white_check_mark: |
+| Cohere       | LLM             | :white_check_mark: | :white_check_mark: |
+| Groq         | LLM             | :x:                | :white_check_mark: |
+| Langchain    | Framework       | :x:                | :white_check_mark: |
+| LlamaIndex   | Framework       | :white_check_mark: | :white_check_mark: |
+| Pinecone     | Vector Database | :white_check_mark: | :white_check_mark: |
+| ChromaDB     | Vector Database | :white_check_mark: | :white_check_mark: |
+| QDrant       | Vector Database | :x:                | :white_check_mark: |
 
 ---
 
 ## Feature Requests and Issues
 
 - To request for features, head over [here to start a discussion](https://github.com/Scale3-Labs/langtrace/discussions/categories/feature-requests).
 - To raise an issue, head over [here and create an issue](https://github.com/Scale3-Labs/langtrace/issues).
```

