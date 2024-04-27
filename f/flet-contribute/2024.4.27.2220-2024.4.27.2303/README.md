# Comparing `tmp/flet_contribute-2024.4.27.2220.tar.gz` & `tmp/flet_contribute-2024.4.27.2303.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_contribute-2024.4.27.2220.tar", max compression
+gzip compressed data, was "flet_contribute-2024.4.27.2303.tar", max compression
```

## Comparing `flet_contribute-2024.4.27.2220.tar` & `flet_contribute-2024.4.27.2303.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     2144 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/README.md
--rw-r--r--   0        0        0     1052 2024-04-27 22:20:17.712744 flet_contribute-2024.4.27.2220/pyproject.toml
--rw-r--r--   0        0        0       27 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/__init__.py
--rw-r--r--   0        0        0       72 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/__pyinstaller/__init__.py
--rw-r--r--   0        0        0      338 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/__pyinstaller/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      192 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/__pyinstaller/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0       20 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/__pyinstaller/config.py
--rw-r--r--   0        0        0      378 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/__pyinstaller/hook-flet.py
--rw-r--r--   0        0        0     2991 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/__pyinstaller/macos_utils.py
--rw-r--r--   0        0        0      187 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
--rw-r--r--   0        0        0       61 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/__pyinstaller/rthooks.dat
--rw-r--r--   0        0        0      540 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/__pyinstaller/utils.py
--rw-r--r--   0        0        0     3620 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/__pyinstaller/win_utils.py
--rw-r--r--   0        0        0       32 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/auth/__init__.py
--rw-r--r--   0        0        0       42 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/auth/providers/__init__.py
--rw-r--r--   0        0        0       31 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     2005 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/__pycache__/cli.cpython-39.pyc
--rw-r--r--   0        0        0     3145 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/cli.py
--rw-r--r--   0        0        0     2205 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0    18007 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/build.cpython-39.pyc
--rw-r--r--   0        0        0     2438 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/create.cpython-39.pyc
--rw-r--r--   0        0        0     1237 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/options.cpython-39.pyc
--rw-r--r--   0        0        0     6382 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/pack.cpython-39.pyc
--rw-r--r--   0        0        0     5285 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/publish.cpython-39.pyc
--rw-r--r--   0        0        0     8416 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/run.cpython-39.pyc
--rw-r--r--   0        0        0     1953 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/base.py
--rw-r--r--   0        0        0    32888 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/build.py
--rw-r--r--   0        0        0     2874 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/create.py
--rw-r--r--   0        0        0      673 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/options.py
--rw-r--r--   0        0        0    11450 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/pack.py
--rw-r--r--   0        0        0     7561 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/publish.py
--rw-r--r--   0        0        0    12195 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/cli/commands/run.py
--rw-r--r--   0        0        0     4181 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/README.md
--rw-r--r--   0        0        0      282 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/__init__.py
--rw-r--r--   0        0        0      521 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4347 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/app.cpython-39.pyc
--rw-r--r--   0        0        0    13116 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/flet_app.cpython-39.pyc
--rw-r--r--   0        0        0     6200 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/flet_app_manager.cpython-39.pyc
--rw-r--r--   0        0        0     3443 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/flet_fastapi.cpython-39.pyc
--rw-r--r--   0        0        0     2072 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/flet_oauth.cpython-39.pyc
--rw-r--r--   0        0        0     5563 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/flet_static_files.cpython-39.pyc
--rw-r--r--   0        0        0     2559 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/flet_upload.cpython-39.pyc
--rw-r--r--   0        0        0      645 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/oauth_state.cpython-39.pyc
--rw-r--r--   0        0        0     2205 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/serve_fastapi_web_app.cpython-39.pyc
--rw-r--r--   0        0        0     4862 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/app.py
--rw-r--r--   0        0        0    17266 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/flet_app.py
--rw-r--r--   0        0        0     5522 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/flet_app_manager.py
--rw-r--r--   0        0        0     4333 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/flet_fastapi.py
--rw-r--r--   0        0        0     2105 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/flet_oauth.py
--rw-r--r--   0        0        0     7318 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/flet_static_files.py
--rw-r--r--   0        0        0     3115 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/flet_upload.py
--rw-r--r--   0        0        0      308 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/oauth_state.py
--rw-r--r--   0        0        0     2275 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/fastapi/serve_fastapi_web_app.py
--rw-r--r--   0        0        0       55 2024-04-27 22:19:34.516564 flet_contribute-2024.4.27.2220/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2024-04-27 22:19:34.520564 flet_contribute-2024.4.27.2220/src/flet/plotly_chart.py
--rw-r--r--   0        0        0       36 2024-04-27 22:19:34.520564 flet_contribute-2024.4.27.2220/src/flet/security/__init__.py
--rw-r--r--   0        0        0      145 2024-04-27 22:19:34.520564 flet_contribute-2024.4.27.2220/src/flet/utils/__init__.py
--rw-r--r--   0        0        0      423 2024-04-27 22:19:34.520564 flet_contribute-2024.4.27.2220/src/flet/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1501 2024-04-27 22:19:34.520564 flet_contribute-2024.4.27.2220/src/flet/version.py
--rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 flet_contribute-2024.4.27.2220/PKG-INFO
+-rw-r--r--   0        0        0     2144 2024-04-27 23:03:01.623865 flet_contribute-2024.4.27.2303/README.md
+-rw-r--r--   0        0        0     1052 2024-04-27 23:03:53.599585 flet_contribute-2024.4.27.2303/pyproject.toml
+-rw-r--r--   0        0        0       27 2024-04-27 23:03:01.623865 flet_contribute-2024.4.27.2303/src/flet/__init__.py
+-rw-r--r--   0        0        0       72 2024-04-27 23:03:01.623865 flet_contribute-2024.4.27.2303/src/flet/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0      338 2024-04-27 23:03:01.623865 flet_contribute-2024.4.27.2303/src/flet/__pyinstaller/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      192 2024-04-27 23:03:01.623865 flet_contribute-2024.4.27.2303/src/flet/__pyinstaller/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0       20 2024-04-27 23:03:01.623865 flet_contribute-2024.4.27.2303/src/flet/__pyinstaller/config.py
+-rw-r--r--   0        0        0      378 2024-04-27 23:03:01.623865 flet_contribute-2024.4.27.2303/src/flet/__pyinstaller/hook-flet.py
+-rw-r--r--   0        0        0     2991 2024-04-27 23:03:01.623865 flet_contribute-2024.4.27.2303/src/flet/__pyinstaller/macos_utils.py
+-rw-r--r--   0        0        0      187 2024-04-27 23:03:01.623865 flet_contribute-2024.4.27.2303/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
+-rw-r--r--   0        0        0       61 2024-04-27 23:03:01.623865 flet_contribute-2024.4.27.2303/src/flet/__pyinstaller/rthooks.dat
+-rw-r--r--   0        0        0      540 2024-04-27 23:03:01.623865 flet_contribute-2024.4.27.2303/src/flet/__pyinstaller/utils.py
+-rw-r--r--   0        0        0     3620 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/__pyinstaller/win_utils.py
+-rw-r--r--   0        0        0       32 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/auth/__init__.py
+-rw-r--r--   0        0        0       42 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/auth/providers/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     2005 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/__pycache__/cli.cpython-39.pyc
+-rw-r--r--   0        0        0     3145 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/cli.py
+-rw-r--r--   0        0        0     2205 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0    18007 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/build.cpython-39.pyc
+-rw-r--r--   0        0        0     2438 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/create.cpython-39.pyc
+-rw-r--r--   0        0        0     1237 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/options.cpython-39.pyc
+-rw-r--r--   0        0        0     6382 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/pack.cpython-39.pyc
+-rw-r--r--   0        0        0     5285 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/publish.cpython-39.pyc
+-rw-r--r--   0        0        0     8416 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0        0        0     1953 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/base.py
+-rw-r--r--   0        0        0    32888 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/build.py
+-rw-r--r--   0        0        0     2874 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/create.py
+-rw-r--r--   0        0        0      673 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/options.py
+-rw-r--r--   0        0        0    11450 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/pack.py
+-rw-r--r--   0        0        0     7561 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/publish.py
+-rw-r--r--   0        0        0    12195 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/cli/commands/run.py
+-rw-r--r--   0        0        0     4181 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/README.md
+-rw-r--r--   0        0        0      282 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/__init__.py
+-rw-r--r--   0        0        0      521 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4347 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/app.cpython-39.pyc
+-rw-r--r--   0        0        0    13116 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/flet_app.cpython-39.pyc
+-rw-r--r--   0        0        0     6200 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/flet_app_manager.cpython-39.pyc
+-rw-r--r--   0        0        0     3443 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/flet_fastapi.cpython-39.pyc
+-rw-r--r--   0        0        0     2072 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/flet_oauth.cpython-39.pyc
+-rw-r--r--   0        0        0     5563 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/flet_static_files.cpython-39.pyc
+-rw-r--r--   0        0        0     2559 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/flet_upload.cpython-39.pyc
+-rw-r--r--   0        0        0      645 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/oauth_state.cpython-39.pyc
+-rw-r--r--   0        0        0     2205 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/serve_fastapi_web_app.cpython-39.pyc
+-rw-r--r--   0        0        0     4862 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/app.py
+-rw-r--r--   0        0        0    17266 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/flet_app.py
+-rw-r--r--   0        0        0     5522 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/flet_app_manager.py
+-rw-r--r--   0        0        0     4333 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/flet_fastapi.py
+-rw-r--r--   0        0        0     2105 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/flet_oauth.py
+-rw-r--r--   0        0        0     7318 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/flet_static_files.py
+-rw-r--r--   0        0        0     3115 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/flet_upload.py
+-rw-r--r--   0        0        0      308 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/oauth_state.py
+-rw-r--r--   0        0        0     2275 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/fastapi/serve_fastapi_web_app.py
+-rw-r--r--   0        0        0       55 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0       36 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/security/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/utils/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1501 2024-04-27 23:03:01.627864 flet_contribute-2024.4.27.2303/src/flet/version.py
+-rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 flet_contribute-2024.4.27.2303/PKG-INFO
```

### Comparing `flet_contribute-2024.4.27.2220/README.md` & `flet_contribute-2024.4.27.2303/README.md`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/pyproject.toml` & `flet_contribute-2024.4.27.2303/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet_contribute"
-version = "2024.04.27.2220"
+version = "2024.04.27.2303"
 description = "Flet for Python - easily build interactive multi-platform apps in Python"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -13,15 +13,15 @@
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-flet-contrib-runtime = "2024.04.27.2220"
+flet-contrib-runtime = "2024.04.27.2303"
 watchdog = "^4.0.0"
 packaging = "^23.1"
 qrcode = "^7.4.2"
 cookiecutter = "^2.6.0"
 fastapi = "^0"
 uvicorn = {extras = ["standard"], version = "^0"}
```

### Comparing `flet_contribute-2024.4.27.2220/src/flet/__pyinstaller/macos_utils.py` & `flet_contribute-2024.4.27.2303/src/flet/__pyinstaller/macos_utils.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/__pyinstaller/utils.py` & `flet_contribute-2024.4.27.2303/src/flet/__pyinstaller/utils.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/__pyinstaller/win_utils.py` & `flet_contribute-2024.4.27.2303/src/flet/__pyinstaller/win_utils.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/__pycache__/cli.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/cli/__pycache__/cli.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/cli.py` & `flet_contribute-2024.4.27.2303/src/flet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/base.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/build.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/build.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/create.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/create.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/options.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/options.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/pack.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/pack.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/publish.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/publish.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/__pycache__/run.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/__pycache__/run.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/base.py` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/build.py` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/create.py` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/options.py` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/options.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/pack.py` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/pack.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/publish.py` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/cli/commands/run.py` & `flet_contribute-2024.4.27.2303/src/flet/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/README.md` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/README.md`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/__init__.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/app.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/app.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/flet_app.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/flet_app.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/flet_app_manager.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/flet_app_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/flet_fastapi.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/flet_fastapi.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/flet_oauth.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/flet_oauth.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/flet_static_files.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/flet_static_files.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/flet_upload.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/flet_upload.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/oauth_state.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/oauth_state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/__pycache__/serve_fastapi_web_app.cpython-39.pyc` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/__pycache__/serve_fastapi_web_app.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/app.py` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/app.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/flet_app.py` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/flet_app.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/flet_app_manager.py` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/flet_app_manager.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/flet_fastapi.py` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/flet_fastapi.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/flet_oauth.py` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/flet_oauth.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/flet_static_files.py` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/flet_static_files.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/flet_upload.py` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/flet_upload.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/fastapi/serve_fastapi_web_app.py` & `flet_contribute-2024.4.27.2303/src/flet/fastapi/serve_fastapi_web_app.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/src/flet/version.py` & `flet_contribute-2024.4.27.2303/src/flet/version.py`

 * *Files identical despite different names*

### Comparing `flet_contribute-2024.4.27.2220/PKG-INFO` & `flet_contribute-2024.4.27.2303/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flet_contribute
-Version: 2024.4.27.2220
+Version: 2024.4.27.2303
 Summary: Flet for Python - easily build interactive multi-platform apps in Python
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cookiecutter (>=2.6.0,<3.0.0)
 Requires-Dist: fastapi (>=0,<1)
-Requires-Dist: flet-contrib-runtime (==2024.04.27.2220)
+Requires-Dist: flet-contrib-runtime (==2024.04.27.2303)
 Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Requires-Dist: uvicorn[standard] (>=0,<1)
 Requires-Dist: watchdog (>=4.0.0,<5.0.0)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
```

