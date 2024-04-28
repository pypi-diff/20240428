# Comparing `tmp/termax-0.1.3.tar.gz` & `tmp/termax-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termax-0.1.3.tar", last modified: Tue Apr 23 19:51:49 2024, max compression
+gzip compressed data, was "termax-0.1.4.tar", last modified: Sun Apr 28 02:51:48 2024, max compression
```

## Comparing `termax-0.1.3.tar` & `termax-0.1.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.172725 termax-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-23 19:51:40.000000 termax-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-23 19:51:49.172725 termax-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-23 19:51:40.000000 termax-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.164724 termax-0.1.3/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:41.000000 termax-0.1.3/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-23 19:51:49.172725 termax-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-23 19:51:41.000000 termax-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.164724 termax-0.1.3/termax/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 19:51:41.000000 termax-0.1.3/termax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.168725 termax-0.1.3/termax/agent/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_qianfan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/_qianwen.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-23 19:51:41.000000 termax-0.1.3/termax/agent/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.168725 termax-0.1.3/termax/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:41.000000 termax-0.1.3/termax/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-04-23 19:51:41.000000 termax-0.1.3/termax/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-23 19:51:41.000000 termax-0.1.3/termax/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.168725 termax-0.1.3/termax/function/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.168725 termax-0.1.3/termax/function/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/openai/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/openai/macos.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/openai/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-23 19:51:41.000000 termax-0.1.3/termax/function/openai/win.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.168725 termax-0.1.3/termax/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/install.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.168725 termax-0.1.3/termax/plugin/shell/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/shell/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/shell/fish.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/shell/zsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-23 19:51:41.000000 termax-0.1.3/termax/plugin/uninstall.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.172725 termax-0.1.3/termax/pricing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:41.000000 termax-0.1.3/termax/pricing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.172725 termax-0.1.3/termax/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 19:51:41.000000 termax-0.1.3/termax/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-23 19:51:41.000000 termax-0.1.3/termax/prompt/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14350 2024-04-23 19:51:41.000000 termax-0.1.3/termax/prompt/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-23 19:51:41.000000 termax-0.1.3/termax/prompt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.172725 termax-0.1.3/termax/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 19:51:41.000000 termax-0.1.3/termax/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-23 19:51:41.000000 termax-0.1.3/termax/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 19:51:41.000000 termax-0.1.3/termax/utils/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    14173 2024-04-23 19:51:41.000000 termax-0.1.3/termax/utils/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-23 19:51:41.000000 termax-0.1.3/termax/utils/qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-23 19:51:41.000000 termax-0.1.3/termax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.172725 termax-0.1.3/termax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-23 19:51:49.000000 termax-0.1.3/termax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-23 19:51:49.000000 termax-0.1.3/termax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:51:49.000000 termax-0.1.3/termax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 19:51:49.000000 termax-0.1.3/termax.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-23 19:51:49.000000 termax-0.1.3/termax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 19:51:49.000000 termax-0.1.3/termax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:49.172725 termax-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:51:41.000000 termax-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:48.004968 termax-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-28 02:51:38.000000 termax-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-28 02:51:48.004968 termax-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-28 02:51:38.000000 termax-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:47.996968 termax-0.1.4/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:38.000000 termax-0.1.4/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-28 02:51:48.004968 termax-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-28 02:51:38.000000 termax-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:47.996968 termax-0.1.4/termax/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-28 02:51:38.000000 termax-0.1.4/termax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:48.000968 termax-0.1.4/termax/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-28 02:51:38.000000 termax-0.1.4/termax/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-28 02:51:38.000000 termax-0.1.4/termax/agent/_claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-28 02:51:38.000000 termax-0.1.4/termax/agent/_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-28 02:51:38.000000 termax-0.1.4/termax/agent/_mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-28 02:51:38.000000 termax-0.1.4/termax/agent/_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-28 02:51:38.000000 termax-0.1.4/termax/agent/_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-28 02:51:38.000000 termax-0.1.4/termax/agent/_qianfan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-28 02:51:38.000000 termax-0.1.4/termax/agent/_qianwen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-28 02:51:38.000000 termax-0.1.4/termax/agent/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:48.000968 termax-0.1.4/termax/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:38.000000 termax-0.1.4/termax/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-28 02:51:38.000000 termax-0.1.4/termax/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-28 02:51:38.000000 termax-0.1.4/termax/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:48.000968 termax-0.1.4/termax/function/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-28 02:51:38.000000 termax-0.1.4/termax/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-28 02:51:38.000000 termax-0.1.4/termax/function/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:48.000968 termax-0.1.4/termax/function/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-28 02:51:38.000000 termax-0.1.4/termax/function/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-28 02:51:38.000000 termax-0.1.4/termax/function/openai/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-28 02:51:38.000000 termax-0.1.4/termax/function/openai/macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-28 02:51:38.000000 termax-0.1.4/termax/function/openai/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-28 02:51:38.000000 termax-0.1.4/termax/function/openai/win.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:48.004968 termax-0.1.4/termax/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-28 02:51:38.000000 termax-0.1.4/termax/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-28 02:51:38.000000 termax-0.1.4/termax/plugin/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:48.004968 termax-0.1.4/termax/plugin/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-28 02:51:38.000000 termax-0.1.4/termax/plugin/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-28 02:51:38.000000 termax-0.1.4/termax/plugin/shell/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-28 02:51:38.000000 termax-0.1.4/termax/plugin/shell/fish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-28 02:51:38.000000 termax-0.1.4/termax/plugin/shell/zsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-28 02:51:38.000000 termax-0.1.4/termax/plugin/uninstall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:48.004968 termax-0.1.4/termax/pricing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:38.000000 termax-0.1.4/termax/pricing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:48.004968 termax-0.1.4/termax/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-28 02:51:38.000000 termax-0.1.4/termax/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-28 02:51:38.000000 termax-0.1.4/termax/prompt/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-04-28 02:51:38.000000 termax-0.1.4/termax/prompt/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-28 02:51:38.000000 termax-0.1.4/termax/prompt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:48.004968 termax-0.1.4/termax/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-28 02:51:38.000000 termax-0.1.4/termax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-28 02:51:38.000000 termax-0.1.4/termax/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-28 02:51:38.000000 termax-0.1.4/termax/utils/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14173 2024-04-28 02:51:38.000000 termax-0.1.4/termax/utils/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-28 02:51:38.000000 termax-0.1.4/termax/utils/qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-28 02:51:38.000000 termax-0.1.4/termax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:48.004968 termax-0.1.4/termax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-28 02:51:47.000000 termax-0.1.4/termax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-28 02:51:47.000000 termax-0.1.4/termax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 02:51:47.000000 termax-0.1.4/termax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 02:51:47.000000 termax-0.1.4/termax.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-28 02:51:47.000000 termax-0.1.4/termax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-28 02:51:47.000000 termax-0.1.4/termax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:48.004968 termax-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 02:51:38.000000 termax-0.1.4/tests/__init__.py
```

### Comparing `termax-0.1.3/LICENSE` & `termax-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/PKG-INFO` & `termax-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termax
-Version: 0.1.3
+Version: 0.1.4
 Summary: Boost your terminal's intelligence with LLM: intuitive command assistance, seamless customization, and predictive next steps at your fingertips.
 Home-page: https://github.com/huangyz0918/termax
 Download-URL: https://github.com/huangyz0918/termax/archive/refs/heads/main.zip
 Author: Yizheng Huang
 Author-email: huangyz0918@gmail.com
 Keywords: LLM,deep learning,MLOps,shell,neural networks,command line,terminal,autocomplete
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai
 Requires-Dist: rich~=13.7.1
 Requires-Dist: click~=8.1.7
 Requires-Dist: inquirer~=3.2.4
+Requires-Dist: pyperclip~=1.8.2
 Requires-Dist: chromadb~=0.4.24
 Requires-Dist: psutil~=5.9.8
 Requires-Dist: instructor~=0.6.8
 Requires-Dist: pydantic~=2.6.4
 Requires-Dist: setuptools~=68.2.2
 
 # Termax
```

### Comparing `termax-0.1.3/README.md` & `termax-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/setup.py` & `termax-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/agent/_claude.py` & `termax-0.1.4/termax/agent/_claude.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,31 +27,14 @@
             )
 
         self.version = version
         self.model_type = CONFIG_SEC_CLAUDE
         self.client = self.anthropic.Anthropic(api_key=api_key)
         self.generation_config = generation_config
 
-    def guess_command(self, history, prompt):
-        """
-        Guess the command based on the prompt.
-        """
-        message = self.client.messages.create(
-            model=self.version,
-            system=prompt,
-            max_tokens=self.generation_config['max_tokens'],
-            temperature=self.generation_config['temperature'],
-            top_k=self.generation_config['top_k'],
-            top_p=self.generation_config['top_p'],
-            stop_sequences=self.generation_config['stop_sequences'],
-            messages=[{"role": "user", "content": history}]
-        )
-        response = message.content[0].text
-        return extract_shell_commands(response)
-
     def to_command(self, prompt, text):
         """
         Generate a command based on the prompt and text.
         Args:
             prompt (str): The prompt.
             text (str): The text.
         """
```

### Comparing `termax-0.1.3/termax/agent/_gemini.py` & `termax-0.1.4/termax/agent/_gemini.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,29 +35,14 @@
             stop_sequences=generation_config['stop_sequences'],
             temperature=generation_config['temperature'],
             top_p=generation_config['top_p'],
             top_k=generation_config['top_k'],
             candidate_count=generation_config['candidate_count'],
             max_output_tokens=generation_config['max_output_tokens'])
 
-    def guess_command(self, history, prompt):
-        """
-        Guess the command based on the prompt.
-        Args:
-            history (str): The history.
-            prompt (str): The prompt.
-        """
-        model = self.genai.GenerativeModel(self.version)
-        chat = model.start_chat(history=[
-            self.glm.Content(parts=[self.glm.Part(text=prompt)], role="user"),
-            self.glm.Content(parts=[self.glm.Part(text="understand")], role="model")
-        ])
-        response = chat.send_message(history, generation_config=self.generation_config).text
-        return extract_shell_commands(response)
-
     def to_command(self, prompt, text):
         """
         Generate a command based on the prompt and text.
         Args:
             prompt (str): The prompt.
             text (str): The text.
         """
```

### Comparing `termax-0.1.3/termax/agent/_mistral.py` & `termax-0.1.4/termax/agent/_mistral.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,34 +29,14 @@
             )
 
         self.version = version
         self.model_type = CONFIG_SEC_MISTRAL
         self.client = self.MistralClient(api_key=api_key)
         self.generation_config = generation_config
 
-    def guess_command(self, history, prompt):
-        """
-        Guess the command based on the prompt.
-        Args:
-            history (str): The history.
-            prompt (str): The prompt.
-        """
-        chat_response = self.client.chat(
-            model=self.version,
-            messages=[
-                self.ChatMessage(role="system", content=prompt),
-                self.ChatMessage(role="user", content=history)
-            ],
-            temperature=self.generation_config['temperature'],
-            top_p=self.generation_config['top_p'],
-            max_tokens=self.generation_config['max_tokens']
-        )
-        response = chat_response.choices[0].message.content
-        return extract_shell_commands(response)
-
     def to_command(self, prompt, text):
         """
         Generate a command based on the prompt and text.
         Args:
             prompt (str): The prompt.
             text (str): The text.
         """
```

### Comparing `termax-0.1.3/termax/agent/_ollama.py` & `termax-0.1.4/termax/agent/_ollama.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,40 +29,14 @@
 
         self.version = version
         if is_url(host_url):
             self.client = self.Client(host=host_url)
         else:
             self.client = self.Client()
 
-    def guess_command(self, history, prompt):
-        """
-        Guess the command based on the prompt.
-        Args:
-            history (str): The history.
-            prompt (str): The prompt.
-        """
-        try:
-            chat_history = [
-                {"role": "system", "content": prompt},
-                {"role": "user", "content": history}
-            ]
-
-            completion = self.client.chat(
-                model=self.version,
-                messages=chat_history,
-            )
-
-            response = completion['message']['content']
-            return extract_shell_commands(response)
-        except self.ResponseError as e:
-            print(f"Ollama Error: {e.error}")
-        except Exception as e:
-            print("Ollama error occurred.")
-            print(f"Error message: {e}")
-
     def to_command(self, prompt, text):
         """
         Generate a command based on the prompt and text.
         Args:
             prompt (str): The prompt.
             text (str): The text.
         """
```

### Comparing `termax-0.1.3/termax/agent/_openai.py` & `termax-0.1.4/termax/agent/_openai.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,45 +32,14 @@
         self.version = version
         self.temperature = temperature
         if is_url(base_url):
             self.client = self.OpenAI(api_key=api_key, base_url=base_url)
         else:
             self.client = self.OpenAI(api_key=api_key)
 
-    def guess_command(self, history, prompt):
-        """
-        Guess the command based on the prompt.
-        Args:
-            history (str): The history.
-            prompt (str): The prompt.
-        """
-        try:
-            completion = self.client.chat.completions.create(
-                model=self.version,
-                messages=[
-                    {
-                        "role": "system",
-                        "content": prompt
-                    },
-                    {
-                        "role": "user",
-                        "content": history,
-                    }
-                ],
-                temperature=self.temperature
-            )
-            response = completion.choices[0].message.content
-            return extract_shell_commands(response)
-        except self.RateLimitError as e:
-            print("Rate limit exceeded. Please try again later.")
-            print(f"Error message: {e}")
-        except Exception as e:
-            print("OpenAI error occurred.")
-            print(f"Error message: {e}")
-
     def to_command(self, prompt, text):
         """
         Generate a command based on the prompt and text.
         Args:
             prompt (str): The prompt.
             text (str): The text.
         """
```

### Comparing `termax-0.1.3/termax/agent/_qianfan.py` & `termax-0.1.4/termax/agent/_qianfan.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,32 +29,14 @@
             )
 
         self.model_type = CONFIG_SEC_QIANFAN
         self.client = self.qianfan.ChatCompletion(ak=api_key, sk=secret_key)
         self.version = version
         self.generation_config = generation_config
 
-    def guess_command(self, history, prompt):
-        """
-        Guess the command based on the prompt.
-        Args:
-            history (str): The history.
-            prompt (str): The prompt.
-        """
-        message = self.client.do(
-            model=self.version,
-            messages=[{"role": "user", "content": history}],
-            system=prompt,
-            temperature=self.generation_config['temperature'],
-            top_p=self.generation_config['top_p'],
-            max_output_tokens=self.generation_config['max_output_tokens']
-        )
-        response = message['body']['result']
-        return extract_shell_commands(response)
-
     def to_command(self, prompt, text):
         """
         Generate a command based on the prompt and request.
         Args:
             prompt (str): The prompt.
             text (str): The request text.
         """
```

### Comparing `termax-0.1.3/termax/agent/_qianwen.py` & `termax-0.1.4/termax/agent/_qianwen.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,36 +30,14 @@
             )
 
         self.version = version
         self.model_type = CONFIG_SEC_QIANWEN
         self.dashscope.api_key = api_key
         self.generation_config = generation_config
 
-    def guess_command(self, history, prompt):
-        """
-        Guess the command based on the prompt.
-        Args:
-            history (str): The history.
-            prompt (str): The prompt.
-        """
-        message = self.dashscope.Generation.call(
-            model=self.version,
-            messages=[
-                {'role': 'system', 'content': prompt},
-                {'role': 'user', 'content': history}
-            ],
-            max_tokens=self.generation_config['max_tokens'],
-            temperature=self.generation_config['temperature'],
-            top_k=self.generation_config['top_k'],
-            top_p=self.generation_config['top_p'],
-            stop=self.generation_config['stop'],
-        )
-        response = message['output'].text
-        return extract_shell_commands(response)
-
     def to_command(self, prompt, text):
         """
         Generate a command based on the prompt and text.
         Args:
             prompt (str): The prompt.
             text (str): The text.
         """
```

### Comparing `termax-0.1.3/termax/cli/cli.py` & `termax-0.1.4/termax/cli/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from rich.console import Console
 
 import termax
 from .utils import *
 from termax.utils.const import *
 from termax.prompt import Prompt, Memory
 from termax.plugin import install_plugin, uninstall_plugin
-from termax.utils import Config, CONFIG_PATH, qa_confirm
+from termax.utils import Config, CONFIG_PATH, qa_confirm, qa_action, qa_prompt, qa_revise
 
 memory = Memory()
 # avoid the tokenizers parallelism issue
 os.environ['TOKENIZERS_PARALLELISM'] = 'false'
 
 
 class DefaultCommandGroup(click.Group):
@@ -62,69 +62,65 @@
 def guess():
     """
     Guess the next command based on the information provided.
     """
     console = Console()
     prompt = Prompt(memory)
     configuration = Config()
-
+    
     config_dict = configuration.read()
     if not configuration.config.has_section(CONFIG_SEC_GENERAL):
         click.echo(f"General section not found. Running config setup...")
         build_config(general=True)
         config_dict = configuration.read()
 
     platform = config_dict['general']['platform']
     if not configuration.config.has_section(platform):
         click.echo(f"Platform {platform} section not found. Running config setup...")
         build_config()
         config_dict = configuration.read()
 
     model, platform = load_model()
     # generate the commands from the model, and execute if auto_execute is True
+    intent = qa_prompt()
     with console.status(f"[cyan]Guessing..."):
-        # Filter and format history excluding certain commands
-        initial_history = filter_and_format_history(
-            prompt.command_history["shell_command_history"],
-            lambda entry: entry['command'] not in ("t guess", "termax guess"),
-            COMMAND_HISTORY_COUNT
-        )
-        # Guess the intent based on the initial history
-        prompt_intent = prompt.intent_detect()
-        intent = model.guess_command(initial_history, prompt_intent)
-        if not intent: return
-
-        # Filter and format history including commands related to the guessed intent
-        related_history = filter_and_format_history(
-            prompt.command_history["shell_command_history"],
-            lambda entry: intent in entry['command'],
-            COMMAND_HISTORY_COUNT // 3
-        )
-
-        # Generate suggestions and guess the final command
-        prompt_guess = prompt.gen_suggestions(intent)
-        command = model.guess_command(related_history, prompt_guess)
-        if not command: return
-
-    if config_dict['general']['show_command'] == "True":
-        console.log(command, style="purple")
-
+        primary, description = intent['primary'], intent['description']
+        guess_prompt = prompt.gen_suggestions(primary, platform)
+        command = model.to_command(prompt=guess_prompt, text=description)
+    
+    click.echo(f"\nSuggestion:\n")
+    console.log(f"{command}\n", style="purple") if command else console.log("Suggestion not readily available. Please revise for better results.\n", style="purple")
     try:
-        if config_dict['general']['auto_execute'] == "True":
-            execute_command(command)
-        else:
-            choice = qa_confirm()
+        choice = qa_action() if command else 3
+        while True:
             if choice == 0:
-                execute_command(command)
-            elif choice == 2:
+                copy_success =  copy_command(command)
+                print("Command copied to clipboard.") if copy_success else print("Failed to copy the command.")
+                break
+            elif choice == 1:
                 with console.status(f"[cyan]Generating..."):
                     description = model.to_description(prompt.explain_commands(), command)
                 console.log(f"{description}")
+                break
+            elif choice == 2:
+                command_success = execute_command(command)
+                break
+            elif choice == 3:
+                description += f" Revised Command: {qa_revise()}"
+                command = model.to_command(prompt=guess_prompt, text=description)
+                click.echo()
+                console.log(f"{command}\n", style="purple")
+            else:
+                return
+            choice = qa_action()
     except KeyboardInterrupt:
-        pass
+        command_success = True
+    finally:
+        if choice == 2 and command_success:
+                save_command(command, description, config_dict, memory)
 
 
 @cli.command(default_command=True)
 @click.argument('text', nargs=-1)
 @click.option('--print_cmd', '-p', is_flag=True, help="Print the generated command only.")
 def generate(text, print_cmd=False):
     """
```

### Comparing `termax-0.1.3/termax/cli/utils.py` & `termax-0.1.4/termax/cli/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import platform
 import subprocess
+import pyperclip
 
 from termax.prompt import Memory
 from termax.agent import OpenAIModel, OllamaModel, GeminiModel, ClaudeModel, QianFanModel, MistralModel, QianWenModel
 from termax.utils import Config, qa_general, qa_platform
 from termax.utils.const import *
 
 
@@ -159,7 +160,21 @@
 
 def filter_and_format_history(command_history, filter_condition, max_count):
     """Filter and format command history based on a condition and maximum count."""
     filtered_history = [f"Command: {entry['command']}\nExecution Date: {entry['time']}\n" for entry in
                         command_history if filter_condition(entry)][:max_count]
 
     return "Command History: \n" + "\n".join(filtered_history)
+
+
+def copy_command(command: str):
+    """
+    copy_command: copy the command to the clipboard.
+    Args:
+        command: the command to copy.
+    """
+    try:
+        pyperclip.copy(command)
+        return True
+    except pyperclip.PyperclipException:
+        return False
+
```

### Comparing `termax-0.1.3/termax/function/base.py` & `termax-0.1.4/termax/function/base.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/function/openai/git.py` & `termax-0.1.4/termax/function/openai/git.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/function/openai/macos.py` & `termax-0.1.4/termax/function/openai/macos.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/function/openai/win.py` & `termax-0.1.4/termax/function/openai/win.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/plugin/install.py` & `termax-0.1.4/termax/plugin/install.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/plugin/shell/bash.py` & `termax-0.1.4/termax/plugin/shell/bash.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/plugin/shell/fish.py` & `termax-0.1.4/termax/plugin/shell/fish.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/plugin/shell/zsh.py` & `termax-0.1.4/termax/plugin/shell/zsh.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/plugin/uninstall.py` & `termax-0.1.4/termax/plugin/uninstall.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/prompt/memory.py` & `termax-0.1.4/termax/prompt/memory.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/prompt/prompt.py` & `termax-0.1.4/termax/prompt/prompt.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,119 +12,44 @@
         Prompt for Termax: the prompt for the LLMs.
         Args:
             memory: the memory instance.
         """
         # TODO: make the sync of system related metadata once happened at the initialization
         self.system_metadata = get_system_metadata()
         self.path_metadata = get_path_metadata()
-        self.command_history = get_command_history()
+        # self.command_history = get_command_history()
 
         # share the same memory instance.
         if memory is None:
             self.memory = Memory()
         else:
             self.memory = memory
 
-    def intent_detect(self, model: str = CONFIG_SEC_OPENAI):
-        """
-        [Prompt] Detect the intent of code type based on the command history.
-        Args:
-            model: the model to use, default is OpenAI.
-        """
-        files = get_file_metadata()
-        if model == CONFIG_SEC_OPENAI:
-            return textwrap.dedent(
-                f"""\
-                Analyze the provided list of command history entries and infer the primary command or tool being
-                utilized based on the pattern, context, and sequence of these commands.
-                The term "primary command" refers to the main or leading command in a sequence
-                of operations or instructions.
-
-                [INFORMATION] The user's current system information:
-                
-                1. OS: {self.system_metadata['platform']}
-                2. OS Version: {self.system_metadata['platform_version']}
-                3. Architecture: {self.system_metadata['architecture']}
-                
-                [INFORMATION] The user's current PATH information:
-                
-                1. User: {self.path_metadata['user']}
-                2. Current PATH: {self.path_metadata['current_directory']}
-                3. Files under the current directory: {files['files']}
-                4. Directories under the current directory: {files['directory']}
-                5. Invisible files under the current directory: {files['invisible_files']}
-                6. Invisible directories under the current directory: {files['invisible_directory']}
-
-                [INFORMATION] The current time: {datetime.now().isoformat()}
-
-                Here are some rules you need to follow:
-                1. Don't include Subcommand/Argument in the output.
-                
-                The output shell primary command is (please replace the `{{primary_command}}` with the primary command):
-                
-                Command: ${{primary_command}}
-                """
-            )
-        else:
-            # TODO: add more models specific prompt
-            return textwrap.dedent(
-                f"""\
-                Analyze the provided list of command history entries and infer the primary command or tool being
-                utilized based on the pattern, context, and sequence of these commands.
-                The term "primary command" refers to the main or leading command in a sequence of
-                operations or instructions.
-                
-                [INFORMATION] The user's current system information:
-                
-                1. OS: {self.system_metadata['platform']}
-                2. OS Version: {self.system_metadata['platform_version']}
-                3. Architecture: {self.system_metadata['architecture']}
-                
-                [INFORMATION] The user's current PATH information:
-                
-                1. User: {self.path_metadata['user']}
-                2. Current PATH: {self.path_metadata['current_directory']}
-                3. Files under the current directory: {files['files']}
-                4. Directories under the current directory: {files['directory']}
-                5. Invisible files under the current directory: {files['invisible_files']}
-                6. Invisible directories under the current directory: {files['invisible_directory']}
-                
-                [INFORMATION] The current time: {datetime.now().isoformat()}
-
-                Here are some rules you need to follow:
-                1. Don't include Subcommand/Argument in the output.
-                
-                The output shell primary command is (please replace the `{{primary_command}}` with the primary command):
-                
-                Command: ${{primary_command}}
-                """
-            )
-
     def gen_suggestions(self, primary: str, model: str = CONFIG_SEC_OPENAI):
         """
         [Prompt] Generate the suggestions based on the environment and the history.
         Args:
             primary: the primary data source, could be git or docker.
             model: the model to use, default is OpenAI.
         """
         if primary == 'git':
             primary_data = "\n".join(
                 f"{index + 1}. {key}: {value}" for index, (key, value) in enumerate(get_git_metadata().items()))
         elif primary == 'docker':
             primary_data = "\n".join(
                 f"{index + 1}. {key}: {value}" for index, (key, value) in enumerate(get_docker_metadata().items()))
         else:
-            primary_data = 'None'
+            primary_data = 'No primary data source available'
 
         files = get_file_metadata()
         if model == CONFIG_SEC_OPENAI:
             return textwrap.dedent(
                 f"""\
-                You are an shell expert, you need to infer the next command based on the provided list
-                of command history entries.
+                You are an shell expert, you need to assist user to infer the next command based on
+                 user's given intent description.
                 
                 [INFORMATION] The user's current system information:
                 
                 1. OS: {self.system_metadata['platform']}
                 2. OS Version: {self.system_metadata['platform_version']}
                 3. Architecture: {self.system_metadata['architecture']}
                 
@@ -139,28 +64,28 @@
                 
                 [INFORMATION] The current time: {datetime.now().isoformat()}
 
                 [INFORMATION] The primary command information:
                 {primary_data}
                 
                 Here are some rules you need to follow:
-                1. Please provide only shell commands for os without any description.
+                1. Please provide only shell commands as the format below for os without any description.
                 2. Ensure the output is a valid shell command.
                 
                 The output shell commands is (please replace the `{{commands}}` with the actual commands):
 
                 Commands: ${{commands}}
                 """
             )
         else:
             # TODO: add more models specific prompt
             return textwrap.dedent(
                 f"""\
-                You are an shell expert, you need to infer the next command based on the provided list of
-                command history entries.
+                You are an shell expert, you need to assist user to infer the next command based on
+                 user's given intent description.
                 
                 [INFORMATION] The user's current system information:
                 
                 1. OS: {self.system_metadata['platform']}
                 2. OS Version: {self.system_metadata['platform_version']}
                 3. Architecture: {self.system_metadata['architecture']}
                 
@@ -168,26 +93,26 @@
 
                 1. User: {self.path_metadata['user']}
                 2. Current PATH: {self.path_metadata['current_directory']}
                 3. Files under the current directory: {files['files']}
                 4. Directories under the current directory: {files['directory']}
                 5. Invisible files under the current directory: {files['invisible_files']}
                 6. Invisible directories under the current directory: {files['invisible_directory']}
-
-                [INFORMATION] The current time: {datetime.now().isoformat()}
                 
+                [INFORMATION] The current time: {datetime.now().isoformat()}
+
                 [INFORMATION] The primary command information:
                 {primary_data}
                 
                 Here are some rules you need to follow:
-                1. Please provide only shell commands for os without any description.
+                1. Please provide only shell commands as the format below for os without any description.
                 2. Ensure the output is a valid shell command.
                 
                 The output shell commands is (please replace the `{{commands}}` with the actual commands):
-                
+
                 Commands: ${{commands}}
                 """
             )
 
     def explain_commands(self, model: str = CONFIG_SEC_OPENAI):
         """
         [Prompt] Explain the shell commands.
```

### Comparing `termax-0.1.3/termax/prompt/utils.py` & `termax-0.1.4/termax/prompt/utils.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/utils/config.py` & `termax-0.1.4/termax/utils/config.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/utils/const.py` & `termax-0.1.4/termax/utils/const.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax/utils/metadata.py` & `termax-0.1.4/termax/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `termax-0.1.3/termax.egg-info/PKG-INFO` & `termax-0.1.4/termax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termax
-Version: 0.1.3
+Version: 0.1.4
 Summary: Boost your terminal's intelligence with LLM: intuitive command assistance, seamless customization, and predictive next steps at your fingertips.
 Home-page: https://github.com/huangyz0918/termax
 Download-URL: https://github.com/huangyz0918/termax/archive/refs/heads/main.zip
 Author: Yizheng Huang
 Author-email: huangyz0918@gmail.com
 Keywords: LLM,deep learning,MLOps,shell,neural networks,command line,terminal,autocomplete
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai
 Requires-Dist: rich~=13.7.1
 Requires-Dist: click~=8.1.7
 Requires-Dist: inquirer~=3.2.4
+Requires-Dist: pyperclip~=1.8.2
 Requires-Dist: chromadb~=0.4.24
 Requires-Dist: psutil~=5.9.8
 Requires-Dist: instructor~=0.6.8
 Requires-Dist: pydantic~=2.6.4
 Requires-Dist: setuptools~=68.2.2
 
 # Termax
```

### Comparing `termax-0.1.3/termax.egg-info/SOURCES.txt` & `termax-0.1.4/termax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

