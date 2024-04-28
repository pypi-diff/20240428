# Comparing `tmp/inspect_ai-0.3.2.tar.gz` & `tmp/inspect_ai-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspect_ai-0.3.2.tar", last modified: Sun Apr 21 17:12:11 2024, max compression
+gzip compressed data, was "inspect_ai-0.3.3.tar", last modified: Sun Apr 28 20:45:31 2024, max compression
```

## Comparing `inspect_ai-0.3.2.tar` & `inspect_ai-0.3.3.tar`

### file list

```diff
@@ -1,299 +1,367 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.260739 inspect_ai-0.3.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/.gitattributes
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.192739 inspect_ai-0.3.2/.github/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      173 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/.github/dependabot.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      402 2024-01-10 12:28:01.000000 inspect_ai-0.3.2/.github/pull_request_template.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.196739 inspect_ai-0.3.2/.github/workflows/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1100 2024-02-14 11:33:54.000000 inspect_ai-0.3.2/.github/workflows/build.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      544 2024-04-20 08:27:11.000000 inspect_ai-0.3.2/.github/workflows/docs.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1160 2024-04-20 08:27:11.000000 inspect_ai-0.3.2/.github/workflows/pypi.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3160 2024-04-18 13:34:36.000000 inspect_ai-0.3.2/.gitignore
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      696 2024-04-18 13:40:35.000000 inspect_ai-0.3.2/.pre-commit-config.yaml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.196739 inspect_ai-0.3.2/.vscode/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      114 2024-01-10 20:24:09.000000 inspect_ai-0.3.2/.vscode/extensions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2024-04-18 13:32:08.000000 inspect_ai-0.3.2/.vscode/settings.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       27 2024-04-21 13:54:32.000000 inspect_ai-0.3.2/DESCRIPTION.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1079 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2494 2024-04-21 17:12:11.260739 inspect_ai-0.3.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1184 2024-04-20 10:18:47.000000 inspect_ai-0.3.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.196739 inspect_ai-0.3.2/benchmarks/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1611 2024-04-21 16:11:41.000000 inspect_ai-0.3.2/benchmarks/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1328 2024-04-21 16:13:56.000000 inspect_ai-0.3.2/benchmarks/arc.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.200739 inspect_ai-0.3.2/benchmarks/datasets/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1031861 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/benchmarks/datasets/math_test.csv
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  6667575 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/benchmarks/datasets/mmlu.csv
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1656 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/benchmarks/gpqa.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1939 2024-04-21 16:13:56.000000 inspect_ai-0.3.2/benchmarks/gsm8k.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1066 2024-04-21 16:13:56.000000 inspect_ai-0.3.2/benchmarks/hellaswag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3428 2024-04-21 16:13:56.000000 inspect_ai-0.3.2/benchmarks/mathematics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6500 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/benchmarks/mmlu.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.212739 inspect_ai-0.3.2/docs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-04-16 09:27:02.000000 inspect_ai-0.3.2/docs/.gitignore
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.216739 inspect_ai-0.3.2/docs/_examples/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4560 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/docs/_examples/arc.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3629 2024-04-18 13:40:35.000000 inspect_ai-0.3.2/docs/_examples/bias_detection.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5136 2024-04-18 13:32:08.000000 inspect_ai-0.3.2/docs/_examples/biology_qa.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      998 2024-04-21 16:11:41.000000 inspect_ai-0.3.2/docs/_examples/footer.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4947 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/docs/_examples/gsm8k.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3222 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/docs/_examples/hellaswag.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2624 2024-04-21 16:11:41.000000 inspect_ai-0.3.2/docs/_examples/index.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6692 2024-04-21 16:11:41.000000 inspect_ai-0.3.2/docs/_examples/mathematics.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2992 2024-04-18 13:32:08.000000 inspect_ai-0.3.2/docs/_examples/popularity.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2153 2024-04-21 16:11:41.000000 inspect_ai-0.3.2/docs/_examples/security_guide.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2158 2024-04-21 13:21:35.000000 inspect_ai-0.3.2/docs/_examples/theory_of_mind.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4655 2024-04-21 13:21:35.000000 inspect_ai-0.3.2/docs/_examples/tool_use.qmd
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.216739 inspect_ai-0.3.2/docs/_format/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2024-04-21 16:11:41.000000 inspect_ai-0.3.2/docs/_format/post-render.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      364 2024-04-21 16:11:41.000000 inspect_ai-0.3.2/docs/_format/pre-render.sh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2328 2024-04-19 19:51:16.000000 inspect_ai-0.3.2/docs/_quarto.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       75 2024-04-18 13:40:35.000000 inspect_ai-0.3.2/docs/_variables.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10452 2024-04-18 13:40:35.000000 inspect_ai-0.3.2/docs/datasets.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6784 2024-04-20 08:27:11.000000 inspect_ai-0.3.2/docs/eval-logs.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9765 2024-04-18 13:40:35.000000 inspect_ai-0.3.2/docs/eval-suites.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10197 2024-04-20 08:27:11.000000 inspect_ai-0.3.2/docs/eval-tuning.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37174 2024-04-21 16:13:00.000000 inspect_ai-0.3.2/docs/examples.qmd
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.216739 inspect_ai-0.3.2/docs/images/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   170128 2024-04-11 20:37:46.000000 inspect_ai-0.3.2/docs/images/aisi-logo.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    68030 2024-04-10 13:08:20.000000 inspect_ai-0.3.2/docs/images/eval-log.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    68787 2024-04-10 13:08:20.000000 inspect_ai-0.3.2/docs/images/popularity.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    54252 2024-04-10 13:08:20.000000 inspect_ai-0.3.2/docs/images/rate-limit.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    48461 2024-04-18 13:31:29.000000 inspect_ai-0.3.2/docs/images/running-theory.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9052 2024-04-21 16:11:41.000000 inspect_ai-0.3.2/docs/index.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18562 2024-04-19 19:51:16.000000 inspect_ai-0.3.2/docs/models.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10770 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/docs/scorers.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14129 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/docs/solvers.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      637 2024-04-18 13:31:29.000000 inspect_ai-0.3.2/docs/theme.scss
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15937 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/docs/tools.qmd
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11331 2024-04-18 13:40:35.000000 inspect_ai-0.3.2/docs/workflow.qmd
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.220739 inspect_ai-0.3.2/examples/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.188739 inspect_ai-0.3.2/examples/agents/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.220739 inspect_ai-0.3.2/examples/agents/langchain/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       36 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/examples/agents/langchain/.env.example
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/examples/agents/langchain/.gitignore
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2029 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/examples/agents/langchain/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8333 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/examples/agents/langchain/inspect_langchain.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/examples/agents/langchain/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1105 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/examples/agents/langchain/wikipedia.jsonl
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1923 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/examples/agents/langchain/wikipedia.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1466 2024-04-21 16:13:56.000000 inspect_ai-0.3.2/examples/bias_detection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2489 2024-04-21 16:13:56.000000 inspect_ai-0.3.2/examples/biology_qa.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1002 2024-04-21 16:13:56.000000 inspect_ai-0.3.2/examples/popularity.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      639 2024-04-21 16:13:56.000000 inspect_ai-0.3.2/examples/security_guide.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      514 2024-04-21 16:13:56.000000 inspect_ai-0.3.2/examples/theory_of_mind.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1980 2024-04-21 16:13:56.000000 inspect_ai-0.3.2/examples/tool_use.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2024-04-21 13:54:32.000000 inspect_ai-0.3.2/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      197 2024-04-19 15:30:27.000000 inspect_ai-0.3.2/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-21 17:12:11.260739 inspect_ai-0.3.2/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.188739 inspect_ai-0.3.2/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.220739 inspect_ai-0.3.2/src/inspect_ai/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      671 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.224739 inspect_ai-0.3.2/src/inspect_ai/_cli/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1705 2024-04-18 13:40:35.000000 inspect_ai-0.3.2/src/inspect_ai/_cli/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7641 2024-04-20 08:27:11.000000 inspect_ai-0.3.2/src/inspect_ai/_cli/eval.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      899 2024-04-18 13:31:29.000000 inspect_ai-0.3.2/src/inspect_ai/_cli/info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3525 2024-04-18 13:31:29.000000 inspect_ai-0.3.2/src/inspect_ai/_cli/list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      849 2024-04-18 13:31:29.000000 inspect_ai-0.3.2/src/inspect_ai/_cli/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2807 2024-04-18 13:40:35.000000 inspect_ai-0.3.2/src/inspect_ai/_cli/score.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/_cli/util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      699 2024-04-14 10:15:17.000000 inspect_ai-0.3.2/src/inspect_ai/_cli/view.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.224739 inspect_ai-0.3.2/src/inspect_ai/_display/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/_display/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1417 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/_display/_display.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2720 2024-04-20 08:27:11.000000 inspect_ai-0.3.2/src/inspect_ai/_display/logger.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11708 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/_display/rich.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.224739 inspect_ai-0.3.2/src/inspect_ai/_eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16121 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/_eval/eval.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1767 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/src/inspect_ai/_eval/images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9194 2024-04-19 19:01:02.000000 inspect_ai-0.3.2/src/inspect_ai/_eval/list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2347 2024-04-19 15:57:40.000000 inspect_ai-0.3.2/src/inspect_ai/_eval/loader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3653 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/_eval/log.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3998 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/_eval/registry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5586 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/_eval/score.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20947 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/_eval/task.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.228739 inspect_ai-0.3.2/src/inspect_ai/_util/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      355 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/_util/appdirs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      484 2024-04-19 19:09:56.000000 inspect_ai-0.3.2/src/inspect_ai/_util/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      256 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/_util/datetime.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      103 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/_util/dev.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      352 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/_util/docstring.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1427 2024-04-13 10:53:52.000000 inspect_ai-0.3.2/src/inspect_ai/_util/dotenv.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      737 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/_util/error.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5693 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/src/inspect_ai/_util/file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      886 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/src/inspect_ai/_util/git.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3628 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/_util/http.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1196 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/_util/images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1454 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/_util/json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2181 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/src/inspect_ai/_util/notebook.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2034 2024-04-19 15:45:16.000000 inspect_ai-0.3.2/src/inspect_ai/_util/path.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      168 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/_util/pattern.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1699 2024-04-18 13:31:29.000000 inspect_ai-0.3.2/src/inspect_ai/_util/platform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8522 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/_util/registry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2038 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/_util/retry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      322 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/_util/samples.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      400 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/_util/text.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      570 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/_util/url.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      491 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/_util/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.232739 inspect_ai-0.3.2/src/inspect_ai/_view/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1457 2024-04-18 13:31:29.000000 inspect_ai-0.3.2/src/inspect_ai/_view/schema.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4980 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/_view/view.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.232739 inspect_ai-0.3.2/src/inspect_ai/_view/www/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2024-04-18 15:02:12.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/.gitignore
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1317 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/App.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2190 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/App.mjs
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      933 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/Log.mjs
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1363 2024-04-18 13:57:12.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/api.mjs
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.188739 inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.232739 inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/css/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    85877 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/css/bootstrap-icons.min.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   232903 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/css/bootstrap.min.css
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.232739 inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/css/fonts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   176196 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/css/fonts/bootstrap-icons.woff
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   130764 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/css/fonts/bootstrap-icons.woff2
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.236739 inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/js/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80615 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1508 2024-04-18 15:02:12.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/favicon.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/index.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34603 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/log-schema.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8665 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/log.d.ts
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21358 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/package-lock.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/package.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.236739 inspect_ai-0.3.2/src/inspect_ai/_view/www/preact/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3669 2024-04-18 15:02:12.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/preact/hooks.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.236739 inspect_ai-0.3.2/src/inspect_ai/_view/www/preact/htm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1272 2024-04-18 15:02:12.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/preact/htm/htm.mjs
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      241 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/preact/htm/preact.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2024-04-18 15:02:12.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/preact/htm/preact.mjs
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2024-04-18 15:02:12.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/preact/preact-hooks.mjs
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11268 2024-04-18 15:02:12.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/preact/preact.mjs
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.236739 inspect_ai-0.3.2/src/inspect_ai/_view/www/prism/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1896 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/prism/prism.min.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16934 2024-04-18 17:13:37.000000 inspect_ai-0.3.2/src/inspect_ai/_view/www/prism/prism.min.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.236739 inspect_ai-0.3.2/src/inspect_ai/dataset/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      534 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/dataset/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5047 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/dataset/_dataset.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.236739 inspect_ai-0.3.2/src/inspect_ai/dataset/_examples/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20756 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/src/inspect_ai/dataset/_examples/bias_detection.jsonl
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2009 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/src/inspect_ai/dataset/_examples/biology_qa.jsonl
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32773 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/src/inspect_ai/dataset/_examples/popularity.jsonl
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2659 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/src/inspect_ai/dataset/_examples/security_guide.jsonl
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31831 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.240739 inspect_ai-0.3.2/src/inspect_ai/dataset/_sources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3035 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/dataset/_sources/csv.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1720 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/dataset/_sources/example.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2557 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/dataset/_sources/file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/dataset/_sources/hf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3335 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/dataset/_sources/json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3766 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/dataset/_util.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.240739 inspect_ai-0.3.2/src/inspect_ai/log/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      736 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/log/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7888 2024-04-18 13:31:29.000000 inspect_ai-0.3.2/src/inspect_ai/log/_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9155 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/log/_log.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.240739 inspect_ai-0.3.2/src/inspect_ai/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1025 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/src/inspect_ai/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31370 2024-04-18 13:40:35.000000 inspect_ai-0.3.2/src/inspect_ai/model/_model.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.240739 inspect_ai-0.3.2/src/inspect_ai/model/_providers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29713 2024-04-19 19:09:56.000000 inspect_ai-0.3.2/src/inspect_ai/model/_providers/anthropic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7883 2024-04-20 08:27:11.000000 inspect_ai-0.3.2/src/inspect_ai/model/_providers/azureai.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10800 2024-04-19 19:09:56.000000 inspect_ai-0.3.2/src/inspect_ai/model/_providers/bedrock.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3041 2024-04-19 19:09:56.000000 inspect_ai-0.3.2/src/inspect_ai/model/_providers/cloudflare.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10167 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/src/inspect_ai/model/_providers/google.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8776 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/model/_providers/hf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7856 2024-04-19 19:09:56.000000 inspect_ai-0.3.2/src/inspect_ai/model/_providers/mistral.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13473 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/src/inspect_ai/model/_providers/openai.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3298 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/src/inspect_ai/model/_providers/providers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      990 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/src/inspect_ai/model/_providers/together.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      857 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/src/inspect_ai/model/_providers/util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2426 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/src/inspect_ai/model/_registry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2424 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/src/inspect_ai/model/_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4746 2024-04-09 12:20:15.000000 inspect_ai-0.3.2/src/inspect_ai/model/_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-20 20:30:46.000000 inspect_ai-0.3.2/src/inspect_ai/py.typed
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.244739 inspect_ai-0.3.2/src/inspect_ai/scorer/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      750 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/scorer/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2054 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/scorer/_answer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2177 2024-04-20 20:11:43.000000 inspect_ai-0.3.2/src/inspect_ai/scorer/_common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1655 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/scorer/_match.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5983 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/scorer/_metric.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.244739 inspect_ai-0.3.2/src/inspect_ai/scorer/_metrics/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      146 2024-04-19 15:30:27.000000 inspect_ai-0.3.2/src/inspect_ai/scorer/_metrics/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1107 2024-04-19 15:30:27.000000 inspect_ai-0.3.2/src/inspect_ai/scorer/_metrics/accuracy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      555 2024-04-19 15:30:27.000000 inspect_ai-0.3.2/src/inspect_ai/scorer/_metrics/mean.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1539 2024-04-19 15:30:27.000000 inspect_ai-0.3.2/src/inspect_ai/scorer/_metrics/std.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4339 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/scorer/_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1745 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/scorer/_pattern.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4395 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/src/inspect_ai/scorer/_scorer.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.244739 inspect_ai-0.3.2/src/inspect_ai/solver/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      671 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/src/inspect_ai/solver/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3060 2024-04-19 19:01:02.000000 inspect_ai-0.3.2/src/inspect_ai/solver/_critique.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6334 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/src/inspect_ai/solver/_multiple_choice.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4175 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/src/inspect_ai/solver/_plan.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2450 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/src/inspect_ai/solver/_prompt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/src/inspect_ai/solver/_solver.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.244739 inspect_ai-0.3.2/src/inspect_ai/solver/_tool/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3642 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/src/inspect_ai/solver/_tool/tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2007 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/src/inspect_ai/solver/_tool/tool_def.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1703 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/src/inspect_ai/solver/_tool/use_tools.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7374 2024-04-18 13:32:07.000000 inspect_ai-0.3.2/src/inspect_ai/solver/_tool/web_search.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      446 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/src/inspect_ai/solver/_util.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.244739 inspect_ai-0.3.2/src/inspect_ai/util/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/util/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.244739 inspect_ai-0.3.2/src/inspect_ai/util/_context/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2024-04-05 10:33:47.000000 inspect_ai-0.3.2/src/inspect_ai/util/_context/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2777 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/src/inspect_ai/util/_context/concurrency.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      690 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/src/inspect_ai/util/_context/logger.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3146 2024-04-21 17:07:32.000000 inspect_ai-0.3.2/src/inspect_ai/util/_context/resource.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4734 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/src/inspect_ai/util/_context/subprocess.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.256739 inspect_ai-0.3.2/src/inspect_ai.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2494 2024-04-21 17:12:11.000000 inspect_ai-0.3.2/src/inspect_ai.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7935 2024-04-21 17:12:11.000000 inspect_ai-0.3.2/src/inspect_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-21 17:12:11.000000 inspect_ai-0.3.2/src/inspect_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2024-04-21 17:12:11.000000 inspect_ai-0.3.2/src/inspect_ai.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      556 2024-04-21 17:12:11.000000 inspect_ai-0.3.2/src/inspect_ai.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2024-04-21 17:12:11.000000 inspect_ai-0.3.2/src/inspect_ai.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.252739 inspect_ai-0.3.2/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      632 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/tests/test_anthropic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      380 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/tests/test_cloudlfare.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1730 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/tests/test_collapse_user_message.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.252739 inspect_ai-0.3.2/tests/test_dataset/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2024-02-18 15:10:59.000000 inspect_ai-0.3.2/tests/test_dataset/samples.csv
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2024-02-18 15:10:59.000000 inspect_ai-0.3.2/tests/test_dataset/samples.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      102 2024-02-18 15:10:59.000000 inspect_ai-0.3.2/tests/test_dataset/samples.jsonl
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2206 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/tests/test_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      193 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/tests/test_examples.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.252739 inspect_ai-0.3.2/tests/test_images/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   732622 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/tests/test_images/images.jsonl
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1084 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/tests/test_images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1119 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/tests/test_list_task.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1001 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/tests/test_logprobs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3112 2024-04-19 19:01:02.000000 inspect_ai-0.3.2/tests/test_metric.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/tests/test_num_choices.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      746 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/tests/test_openai.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      438 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/tests/test_plan.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      728 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/tests/test_registry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1096 2024-04-09 15:30:36.000000 inspect_ai-0.3.2/tests/test_retry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/tests/test_scorer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1897 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/tests/test_solver.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1970 2024-04-11 12:33:57.000000 inspect_ai-0.3.2/tests/test_stop_reason.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1665 2024-04-05 10:35:33.000000 inspect_ai-0.3.2/tests/test_subprocess.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.252739 inspect_ai-0.3.2/tests/test_task_list/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-20 20:30:46.000000 inspect_ai-0.3.2/tests/test_task_list/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      101 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/tests/test_task_list/attribs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      137 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/tests/test_task_list/multiple.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.252739 inspect_ai-0.3.2/tests/test_task_list/multiple_dir/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.252739 inspect_ai-0.3.2/tests/test_task_list/multiple_dir/_decoy/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/tests/test_task_list/multiple_dir/_decoy/testit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       75 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/tests/test_task_list/multiple_dir/_decoy2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/tests/test_task_list/multiple_dir/bar.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/tests/test_task_list/multiple_dir/foo.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.192739 inspect_ai-0.3.2/tests/test_task_list/recurse/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.252739 inspect_ai-0.3.2/tests/test_task_list/recurse/.folder3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/tests/test_task_list/recurse/.folder3/epsilon.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.256739 inspect_ai-0.3.2/tests/test_task_list/recurse/folder1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       75 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/tests/test_task_list/recurse/folder1/_decoy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       75 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/tests/test_task_list/recurse/folder1/theta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.256739 inspect_ai-0.3.2/tests/test_task_list/recurse/folder2/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-21 17:12:11.256739 inspect_ai-0.3.2/tests/test_task_list/recurse/folder2/.folder3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/tests/test_task_list/recurse/folder2/.folder3/epsilon.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/tests/test_task_list/recurse/folder2/another.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       75 2024-04-18 13:30:14.000000 inspect_ai-0.3.2/tests/test_task_list/recurse/folder2/first.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5420 2024-04-21 11:45:10.000000 inspect_ai-0.3.2/tests/test_tools.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1838 2024-04-09 10:11:39.000000 inspect_ai-0.3.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.204771 inspect_ai-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.144770 inspect_ai-0.3.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.144770 inspect_ai-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.144770 inspect_ai-0.3.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-28 20:45:31.204771 inspect_ai-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.144770 inspect_ai-0.3.3/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/arc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.144770 inspect_ai-0.3.3/benchmarks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/datasets/math_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/datasets/mmlu.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/gpqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/gsm8k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/hellaswag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/mathematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/mmlu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.148770 inspect_ai-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.152770 inspect_ai-0.3.3/docs/_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/arc.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/biology_qa.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/footer.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/gsm8k.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/hellaswag.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/mathematics.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/popularity.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/security_guide.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/theory_of_mind.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/tool_use.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.152770 inspect_ai-0.3.3/docs/_format/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_format/pre-render.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_variables.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/datasets.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/eval-logs.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/eval-suites.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10197 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/eval-tuning.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    35808 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/examples.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.160770 inspect_ai-0.3.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   170128 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/aisi-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68030 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/eval-log.png
+-rw-r--r--   0 runner    (1001) docker     (127)   314093 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-answers.png
+-rw-r--r--   0 runner    (1001) docker     (127)   280184 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)   284131 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-history.png
+-rw-r--r--   0 runner    (1001) docker     (127)   413188 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-home.png
+-rw-r--r--   0 runner    (1001) docker     (127)   241738 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-info.png
+-rw-r--r--   0 runner    (1001) docker     (127)   143202 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-logging-console.png
+-rw-r--r--   0 runner    (1001) docker     (127)   155304 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-logging.png
+-rw-r--r--   0 runner    (1001) docker     (127)   373146 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-main.png
+-rw-r--r--   0 runner    (1001) docker     (127)   321793 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-messages.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165394 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-metadata.png
+-rw-r--r--   0 runner    (1001) docker     (127)   272733 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-scoring.png
+-rw-r--r--   0 runner    (1001) docker     (127)   274383 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-sort.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68787 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/popularity.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54252 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/rate-limit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48461 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/running-theory.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/log-viewer.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/models.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/scorers.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/solvers.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/tools.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    12352 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/workflow.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.160770 inspect_ai-0.3.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.136770 inspect_ai-0.3.3/examples/agents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.160770 inspect_ai-0.3.3/examples/agents/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/.env.example
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/inspect_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/wikipedia.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/biology_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/popularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/security_guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/theory_of_mind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/tool_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 20:45:31.204771 inspect_ai-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.136770 inspect_ai-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.160770 inspect_ai-0.3.3/src/inspect_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.164770 inspect_ai-0.3.3/src/inspect_ai/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.164770 inspect_ai-0.3.3/src/inspect_ai/_display/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_display/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_display/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_display/rich.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.164770 inspect_ai-0.3.3/src/inspect_ai/_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.168770 inspect_ai-0.3.3/src/inspect_ai/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.168770 inspect_ai-0.3.3/src/inspect_ai/_view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.172770 inspect_ai-0.3.3/src/inspect_ai/_view/www/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/App.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/api.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.172770 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.136770 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.172770 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    85877 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   232903 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.172770 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   176196 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   130764 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.172770 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    80615 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31629 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/json5.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.176770 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/prism/prism-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/prism/prism.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/prism/prism.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/purify.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    75207 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/showdown.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/log-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/log.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.176770 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/hooks.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.176770 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/htm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/htm/htm.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/htm/preact.js
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/htm/preact.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/preact-hooks.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/preact.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.176770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/Constants.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/Register.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/AnsiDisplay.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/Card.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/ChatView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/Dialog.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/EmptyPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/LabeledValue.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/MessageContent.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/MetaDataView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/RenderedContent.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/TabSet.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/ToolButton.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/ansi-output.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/log-reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/log-reader/Native-Log-Reader.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/plan/PlanCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/samples/SampleGroupSeparator.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/samples/SampleView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/title/
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/title/TitleBlock.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/usage/UsageCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.184770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/utils/Format.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/utils/Git.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/utils/Path.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/utils/Type.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.184770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/tools.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.184770 inspect_ai-0.3.3/src/inspect_ai/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.184770 inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/bias_detection.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/biology_qa.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    32773 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/popularity.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/security_guide.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    31831 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.184770 inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.184770 inspect_ai-0.3.3/src/inspect_ai/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/log/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/log/_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.188770 inspect_ai-0.3.3/src/inspect_ai/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31676 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.188770 inspect_ai-0.3.3/src/inspect_ai/model/_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)    29724 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/azureai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/bedrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/together.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.192771 inspect_ai-0.3.3/src/inspect_ai/scorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.192771 inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.192771 inspect_ai-0.3.3/src/inspect_ai/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_critique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_multiple_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.192771 inspect_ai-0.3.3/src/inspect_ai/solver/_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_tool/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_tool/tool_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_tool/use_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_tool/web_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.192771 inspect_ai-0.3.3/src/inspect_ai/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.196771 inspect_ai-0.3.3/src/inspect_ai/util/_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/util/_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/util/_context/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/util/_context/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/util/_context/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/util/_context/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/src/inspect_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-28 20:45:31.000000 inspect_ai-0.3.3/src/inspect_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-04-28 20:45:31.000000 inspect_ai-0.3.3/src/inspect_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 20:45:31.000000 inspect_ai-0.3.3/src/inspect_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-28 20:45:31.000000 inspect_ai-0.3.3/src/inspect_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-28 20:45:31.000000 inspect_ai-0.3.3/src/inspect_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 20:45:31.000000 inspect_ai-0.3.3/src/inspect_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.196771 inspect_ai-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_cloudlfare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_collapse_user_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_dataset/samples.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_dataset/samples.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_dataset/samples.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_images/
+-rw-r--r--   0 runner    (1001) docker     (127)   732622 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_images/images.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_list_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_logprobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_num_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_stop_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/attribs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/multiple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/multiple_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/multiple_dir/_decoy/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/multiple_dir/_decoy/testit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/multiple_dir/_decoy2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/multiple_dir/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/multiple_dir/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.140770 inspect_ai-0.3.3/tests/test_task_list/recurse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/recurse/.folder3/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/recurse/.folder3/epsilon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/recurse/folder1/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/recurse/folder1/_decoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/recurse/folder1/theta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/recurse/folder2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/recurse/folder2/.folder3/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/recurse/folder2/.folder3/epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/recurse/folder2/another.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/recurse/folder2/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/utils.py
```

### Comparing `inspect_ai-0.3.2/.github/workflows/build.yml` & `inspect_ai-0.3.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/.github/workflows/docs.yml` & `inspect_ai-0.3.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/.github/workflows/pypi.yml` & `inspect_ai-0.3.3/.github/workflows/pypi.yml`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         type: boolean
         default: false
 
 jobs:
   publish:
     name: Publish
     runs-on: ubuntu-latest
+    environment: pypi
     strategy:
       fail-fast: false
     permissions:
       id-token: write
     steps:
       - name: Checkout
         uses: actions/checkout@v4
@@ -30,17 +31,15 @@
         run: >-
           python3 -m
           pip install
           build
           --user
       - name: Build
         run: python -m build
-      - name: Clean Wheel
-        run: rm -rf dist/inspect*.whl
-      - name: Publish package distributions to TestPyPI
+      - name: Publish package to TestPyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         if: ${{ ! inputs.publish-release }}
         with:
           repository-url: https://test.pypi.org/legacy/
-      - name: Publish package distributions to PyPI
+      - name: Publish package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         if: ${{ inputs.publish-release }}
```

### Comparing `inspect_ai-0.3.2/.gitignore` & `inspect_ai-0.3.3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -159,11 +159,15 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 *.*workspace
 data/datasets/*/hidden
 logs/
 
+# thumbnails
+.DS_Store
+thumbs.db
+
 # JS
 node_modules/
 
 /.luarc.json
```

### Comparing `inspect_ai-0.3.2/.pre-commit-config.yaml` & `inspect_ai-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/LICENSE` & `inspect_ai-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/PKG-INFO` & `inspect_ai-0.3.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 Metadata-Version: 2.1
 Name: inspect_ai
-Version: 0.3.2
-Summary: Language model evaluations
+Version: 0.3.3
+Summary: Framework for large language model evaluations
+Author: UK AI Safety Institute
 License: MIT License
+Project-URL: Documentation, https://UKGovernmentBEIS.github.io/inspect_ai/
+Project-URL: Source Code, https://github.com/UKGovernmentBEIS/inspect_ai
+Project-URL: Issue Tracker, https://github.com/UKGovernmentBEIS/inspect_ai/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -20,53 +24,78 @@
 Requires-Dist: debugpy
 Requires-Dist: fsspec
 Requires-Dist: httpx
 Requires-Dist: numpy
 Requires-Dist: platformdirs
 Requires-Dist: python-dotenv
 Requires-Dist: jsonlines
+Requires-Dist: json-stream
 Requires-Dist: nest_asyncio
 Requires-Dist: pydantic>=2
 Requires-Dist: s3fs>=2023
 Requires-Dist: semver
 Requires-Dist: shortuuid
 Requires-Dist: tenacity
 Requires-Dist: beautifulsoup4
 Requires-Dist: docstring-parser
 Requires-Dist: typing_extensions
 Requires-Dist: pyyaml
 Requires-Dist: rich
+Requires-Dist: psutil
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-dotenv; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Requires-Dist: types-botocore; extra == "dev"
 Requires-Dist: types-boto3; extra == "dev"
 Requires-Dist: types-beautifulsoup4; extra == "dev"
 Requires-Dist: types-protobuf; extra == "dev"
+Requires-Dist: types-psutil; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: openai; extra == "dev"
 Requires-Dist: anthropic; extra == "dev"
 Requires-Dist: google-cloud-aiplatform; extra == "dev"
 Requires-Dist: google-generativeai; extra == "dev"
 Requires-Dist: mistralai; extra == "dev"
 Requires-Dist: boto3; extra == "dev"
 Requires-Dist: transformers; extra == "dev"
 Requires-Dist: torch; extra == "dev"
+Requires-Dist: datasets; extra == "dev"
 Requires-Dist: langchain; extra == "dev"
 Requires-Dist: langchainhub; extra == "dev"
+Requires-Dist: wikipedia; extra == "dev"
 Requires-Dist: ipywidgets; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: nbformat; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: quarto-cli; extra == "doc"
 Provides-Extra: dist
 Requires-Dist: twine; extra == "dist"
 Requires-Dist: build; extra == "dist"
 
-Language model evaluations
+[<img width="295" src="https://ukgovernmentbeis.github.io/inspect_ai/images/aisi-logo.png" />](https://www.gov.uk/government/organisations/ai-safety-institute)
+
+Welcome to Inspect, a framework for large language model evaluations created by the [UK AI Safety Institute](https://www.gov.uk/government/organisations/ai-safety-institute).
+
+Inspect provides many built-in components, including facilities for prompt engineering, tool usage, multi-turn dialog, and model graded evaluations. Extensions to Inspect (e.g. to support new elicitation and scoring techniques) can be provided by other Python packages.
+
+To get started with Inspect, please see the documentation at <https://UKGovernmentBEIS.github.io/inspect_ai/>.
+
+***
+
+#### Development
+
+To work on development of Inspect, clone the repository and install with the `-e` flag and `[dev]` optional dependencies:
+
+```         
+$ git clone https://github.com/UKGovernmentBEIS/inspect_ai.git
+$ cd inspect_ai
+$ pip install -e ".[dev]"
+```
+
+If you use VS Code, you should be sure to have installed the recommended extensions (Python, Ruff, and MyPy). Note that you'll be promoted to install these when you open the project in VS Code.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `inspect_ai-0.3.2/README.md` & `inspect_ai-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/benchmarks/README.md` & `inspect_ai-0.3.3/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/benchmarks/arc.py` & `inspect_ai-0.3.3/benchmarks/arc.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,54 +4,54 @@
 Peter Clark, Isaac Cowhey, Oren Etzioni, Tushar Khot, Ashish Sabharwal, Carissa Schoenick, Oyvind Tafjord
 https://arxiv.org/abs/1803.05457
 
 # run all subsets
 inspect eval arc.py
 
 # run specific subsets
-inspect eval arc.py@easy
-inspect eval arc.py@challenge
+inspect eval arc.py@arc_easy
+inspect eval arc.py@arc_challenge
 """
 
 from inspect_ai import Task, task
 from inspect_ai.dataset import Sample, hf_dataset
 from inspect_ai.scorer import answer
 from inspect_ai.solver import multiple_choice
 
 
 def record_to_sample(record):
-  # read the labels and text
-  choices = record["choices"]
-  choices = dict(zip(choices["label"], choices["text"]))
-
-  # determine the target then normalize to letter
-  answerKey = record["answerKey"]
-  target = list(choices.keys()).index(answerKey)
-  target = chr(ord("A") + int(target))
-
-  # return sample
-  return Sample(
-    input=record["question"],
-    choices=list(choices.values()),
-    target=target
-  )
+    # read the labels and text
+    choices = record["choices"]
+    choices = dict(zip(choices["label"], choices["text"]))
+
+    # determine the target then normalize to letter
+    answerKey = record["answerKey"]
+    target = list(choices.keys()).index(answerKey)
+    target = chr(ord("A") + int(target))
+
+    # return sample
+    return Sample(
+        input=record["question"], choices=list(choices.values()), target=target
+    )
+
 
 def arc_task(dataset_name):
-   return Task(
-     dataset=hf_dataset(
-       path="allenai/ai2_arc",
-       name=dataset_name,
-       split="test",
-       sample_fields=record_to_sample
-     ),
-     plan = multiple_choice(),
-     scorer = answer("letter")
-   )
+    return Task(
+        dataset=hf_dataset(
+            path="allenai/ai2_arc",
+            name=dataset_name,
+            split="test",
+            sample_fields=record_to_sample,
+        ),
+        plan=multiple_choice(),
+        scorer=answer("letter"),
+    )
 
-@task
-def easy():
-  return arc_task("ARC-Easy")
 
 @task
-def challenge():
-  return arc_task("ARC-Challenge")
+def arc_easy():
+    return arc_task("ARC-Easy")
 
+
+@task
+def arc_challenge():
+    return arc_task("ARC-Challenge")
```

### Comparing `inspect_ai-0.3.2/benchmarks/gpqa.py` & `inspect_ai-0.3.3/benchmarks/gpqa.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         ],
         target="A",
         id=record["Record ID"],
     )
 
 
 @task
-def gpqa(cot=True):
+def gpqa_diamond(cot=True):
     return Task(
         dataset=csv_dataset(
             csv_file="https://openaipublic.blob.core.windows.net/simple-evals/gpqa_diamond.csv",
             sample_fields=record_to_sample,
         ),
         plan=[
             multiple_choice(cot=cot, shuffle=True),
```

### Comparing `inspect_ai-0.3.2/benchmarks/gsm8k.py` & `inspect_ai-0.3.3/benchmarks/gsm8k.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,61 +11,71 @@
 inspect eval gsm8k.py -T fewshot=5
 inspect eval gsm8k.py -T fewshot=false
 """
 
 from inspect_ai import Task, task
 from inspect_ai.dataset import Sample, hf_dataset
 from inspect_ai.scorer import match
-from inspect_ai.solver import generate, system_message
+from inspect_ai.solver import generate, prompt_template, system_message
 
 
 def record_to_sample(record):
     DELIM = "####"
     input = record["question"]
     answer = record["answer"].split(DELIM)
     target = answer.pop().strip()
     reasoning = DELIM.join(answer)
-    return Sample(
-        input=input,
-        target=target,
-        metadata={"reasoning": reasoning.strip()}
-    )
+    return Sample(input=input, target=target, metadata={"reasoning": reasoning.strip()})
+
 
 def sample_to_fewshot(sample):
-    ANSWER_TRIGGER = "The answer is"
     return (
-        f"Question: {sample.input}\nAnswer: "
-        + f"{sample.metadata['reasoning']} "
-        + f"{ANSWER_TRIGGER} {sample.target}"
+        f"{sample.input}\n\nReasoning:\n"
+        + f"{sample.metadata['reasoning']}\n\n"
+        + f"ANSWER: {sample.target}"
     )
 
+
+# setup for problem + instructions for providing answer
+MATH_PROMPT_TEMPLATE = """
+Solve the following math problem step by step. The last line of your response should be of the form "ANSWER: $ANSWER" (without quotes) where $ANSWER is the answer to the problem.
+
+{prompt}
+
+Remember to put your answer on its own line at the end in the form "ANSWER: $ANSWER" (without quotes) where $ANSWER is the answer to the problem, and you do not need to use a \\boxed command.
+
+Reasoning:
+""".strip()
+
+
 @task
 def gsm8k(fewshot=10, fewshot_seed=42):
-
     # build plan dynamically (may or may not be doing fewshot)
-    plan = [generate()]
+    plan = [prompt_template(MATH_PROMPT_TEMPLATE), generate()]
     if fewshot:
         fewshots = hf_dataset(
             path="gsm8k",
             data_dir="main",
             split="train",
             sample_fields=record_to_sample,
             shuffle=True,
             seed=fewshot_seed,
             limit=fewshot,
         )
-        plan.insert(0, system_message("\n\n".join(
-            [sample_to_fewshot(sample) for sample in fewshots]
-        )))
+        plan.insert(
+            0,
+            system_message(
+                "\n\n".join([sample_to_fewshot(sample) for sample in fewshots])
+            ),
+        )
 
     # define task
     return Task(
         dataset=hf_dataset(
             path="gsm8k",
             data_dir="main",
             split="test",
             sample_fields=record_to_sample,
         ),
         plan=plan,
-        scorer=match(numeric=True)
+        scorer=match(numeric=True),
     )
-
```

### Comparing `inspect_ai-0.3.2/benchmarks/hellaswag.py` & `inspect_ai-0.3.3/benchmarks/hellaswag.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,38 +10,34 @@
 from inspect_ai.scorer import answer
 from inspect_ai.solver import multiple_choice, system_message
 
 SYSTEM_MESSAGE = """
 Choose the most plausible continuation for the story.
 """
 
+
 def record_to_sample(record):
     return Sample(
-        input = record["ctx"],
-        target = chr(ord("A") + int(record["label"])),
-        choices = record["endings"],
-        metadata = dict(
-            source_id = record["source_id"]
-        )
+        input=record["ctx"],
+        target=chr(ord("A") + int(record["label"])),
+        choices=record["endings"],
+        metadata=dict(source_id=record["source_id"]),
     )
 
+
 @task
 def hellaswag():
-
     # dataset
     dataset = hf_dataset(
         path="hellaswag",
         split="validation",
         sample_fields=record_to_sample,
-        trust=True
+        trust=True,
+        shuffle=True,
     )
 
     # define task
     return Task(
         dataset=dataset,
-        plan=[
-          system_message(SYSTEM_MESSAGE),
-          multiple_choice()
-        ],
+        plan=[system_message(SYSTEM_MESSAGE), multiple_choice()],
         scorer=answer("letter"),
     )
-
```

### Comparing `inspect_ai-0.3.2/benchmarks/mathematics.py` & `inspect_ai-0.3.3/benchmarks/mathematics.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,127 +23,122 @@
     bootstrap_std,
     scorer,
 )
 from inspect_ai.solver import TaskState, generate, prompt_template
 
 # setup for problem + instructions for providing answer
 PROMPT_TEMPLATE = """
-Solve the following math problem step by step. The last line
-of your response should be of the form ANSWER: $ANSWER (without
-quotes) where $ANSWER is the answer to the problem.
+Solve the following math problem step by step. The last line of your response should be of the form "ANSWER: $ANSWER" (without quotes) where $ANSWER is the answer to the problem.
 
 {prompt}
 
-Remember to put your answer on its own line after "ANSWER:",
-and you do not need to use a \\boxed command.
+Remember to put your answer on its own line at the end in the form "ANSWER: $ANSWER" (without quotes) where $ANSWER is the answer to the problem, and you do not need to use a \\boxed command.
 """.strip()
 
+
 @task
 def math(shuffle=True):
     return Task(
         dataset=csv_dataset(
             csv_file="datasets/math_test.csv",
-            sample_fields=FieldSpec(
-                input="Question",
-                target="Answer"
-            ),
+            sample_fields=FieldSpec(input="Question", target="Answer"),
             shuffle=shuffle,
         ),
         plan=[
             prompt_template(PROMPT_TEMPLATE),
             generate(),
         ],
         scorer=expression_equivalance(),
         config=GenerateConfig(temperature=0.5),
     )
 
+
 @scorer(metrics=[accuracy(), bootstrap_std()])
 def expression_equivalance():
     async def score(state: TaskState, target: Target):
         # extract answer
-        answer = re.search(
-            AnswerPattern.LINE, state.output.completion
-        )
-        if answer:
+        match = re.search(AnswerPattern.LINE, state.output.completion)
+        if match:
             # ask the model to judge equivalance
+            answer = match.group(1)
             prompt = EQUIVALANCE_TEMPLATE % (
-                {"expression1": target.text,
-                 "expression2": answer.group(1)}
+                {"expression1": target.text, "expression2": answer}
             )
             result = await get_model().generate(prompt)
 
             # return the score
             correct = result.completion.lower() == "yes"
             return Score(
-                value=CORRECT if correct else INCORRECT
+                value=CORRECT if correct else INCORRECT,
+                answer=answer,
+                explanation=state.output.completion,
             )
         else:
             return Score(
                 value=INCORRECT,
-                explanation="Answer not found in model output."
+                explanation="Answer not found in model output: "
+                + f"{state.output.completion}",
             )
 
     return score
 
+
 EQUIVALANCE_TEMPLATE = r"""
-Look at the following two expressions (answers to a math problem) and
-judge whether they are equivalent. Only perform trivial simplifications
+Look at the following two expressions (answers to a math problem) and judge whether they are equivalent. Only perform trivial simplifications
 
 Examples:
 
-    Expression 1: $2x+3$
-    Expression 2: $3+2x$
+  Expression 1: $2x+3$
+  Expression 2: $3+2x$
 
 Yes
 
-    Expression 1: 3/2
-    Expression 2: 1.5
+  Expression 1: 3/2
+  Expression 2: 1.5
 
 Yes
 
-    Expression 1: $x^2+2x+1$
-    Expression 2: $y^2+2y+1$
+  Expression 1: $x^2+2x+1$
+  Expression 2: $y^2+2y+1$
 
 No
 
-    Expression 1: $x^2+2x+1$
-    Expression 2: $(x+1)^2$
+  Expression 1: $x^2+2x+1$
+  Expression 2: $(x+1)^2$
 
 Yes
 
-    Expression 1: 3245/5
-    Expression 2: 649
+  Expression 1: 3245/5
+  Expression 2: 649
 
 No
 (these are actually equal, don't mark them equivalent if you need to
 do nontrivial simplifications)
 
-    Expression 1: 2/(-3)
-    Expression 2: -2/3
+  Expression 1: 2/(-3)
+  Expression 2: -2/3
 
 Yes
 (trivial simplifications are allowed)
 
-    Expression 1: 72 degrees
-    Expression 2: 72
+  Expression 1: 72 degrees
+  Expression 2: 72
 
 Yes
 (give benefit of the doubt to units)
 
-    Expression 1: 64
-    Expression 2: 64 square feet
+  Expression 1: 64
+  Expression 2: 64 square feet
 
 Yes
 (give benefit of the doubt to units)
 
 ---
 
 YOUR TASK
 
 
-Respond with only "Yes" or "No" (without quotes). Do not include
-a rationale.
+Respond with only "Yes" or "No" (without quotes). Do not include a rationale.
 
-    Expression 1: %(expression1)s
-    Expression 2: %(expression2)s
+  Expression 1: %(expression1)s
+  Expression 2: %(expression2)s
 """.strip()
-
```

### Comparing `inspect_ai-0.3.2/benchmarks/mmlu.py` & `inspect_ai-0.3.3/benchmarks/mmlu.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # add chain of thought
 inspect eval mmlu.py@mmlu --limit 500 -T cot=true
 
 # eval selected subjects
 inspect eval mmlu.py@mmlu -T subjects=anatomy,astronomy
 
 # eval single subjects
-inspect eval mmlu.py@anatomy
-inspect eval mmlu.py@astronomy
+inspect eval mmlu.py@mmlu_anatomy
+inspect eval mmlu.py@mmlu_astronomy
 """
 
 from inspect_ai import Task, task
 from inspect_ai.dataset import Sample, csv_dataset
 from inspect_ai.model import GenerateConfig
 from inspect_ai.scorer import answer
 from inspect_ai.solver import multiple_choice
@@ -39,305 +39,310 @@
             str(record["D"]),
         ],
         target=record["Answer"],
         metadata={"subject": record["Subject"]},
     )
 
 
+# read dataset globally so it can be shared by all of the tasks
+# (shuffle so that --limit draws from multiple subjects)
+dataset = csv_dataset(
+    csv_file="datasets/mmlu.csv",
+    sample_fields=record_to_sample,
+    shuffle=True,
+)
+
+
 @task
 def mmlu(subjects=[], cot=False):
-    # read dataset (shuffle so that --limit draws from multiple subjects
-    dataset = csv_dataset(
-        csv_file="datasets/mmlu.csv",
-        sample_fields=record_to_sample,
-        shuffle=True,
-    )
-
     # filter dataset if requested
     subjects = subjects if isinstance(subjects, list) else [subjects]
     if len(subjects) > 0:
-        dataset = [
-            sample for sample in dataset if sample.metadata["subject"] in subjects
-        ]
+        task_dataset = dataset.filter(
+            name=f"{dataset.name}-{'-'.join(subjects)}",
+            predicate=lambda sample: sample.metadata["subject"] in subjects,
+        )
+    else:
+        task_dataset = dataset
 
     # return task
     return Task(
-        dataset=dataset,
+        dataset=task_dataset,
         plan=multiple_choice(cot=cot),
         scorer=answer("letter"),
         config=GenerateConfig(temperature=0.5),
     )
 
 
 @task
-def abstract_algebra(cot=False):
+def mmlu_abstract_algebra(cot=False):
     return mmlu("abstract_algebra", cot)
 
 
 @task
-def anatomy(cot=False):
+def mmlu_anatomy(cot=False):
     return mmlu("anatomy", cot)
 
 
 @task
-def astronomy(cot=False):
+def mmlu_astronomy(cot=False):
     return mmlu("astronomy", cot)
 
 
 @task
-def business_ethics(cot=False):
+def mmlu_business_ethics(cot=False):
     return mmlu("business_ethics", cot)
 
 
 @task
-def clinical_knowledge(cot=False):
+def mmlu_clinical_knowledge(cot=False):
     return mmlu("clinical_knowledge", cot)
 
 
 @task
-def college_biology(cot=False):
+def mmlu_college_biology(cot=False):
     return mmlu("college_biology", cot)
 
 
 @task
-def college_chemistry(cot=False):
+def mmlu_college_chemistry(cot=False):
     return mmlu("college_chemistry", cot)
 
 
 @task
-def college_computer_science(cot=False):
+def mmlu_college_computer_science(cot=False):
     return mmlu("college_computer_science", cot)
 
 
 @task
-def college_mathematics(cot=False):
+def mmlu_college_mathematics(cot=False):
     return mmlu("college_mathematics", cot)
 
 
 @task
-def college_medicine(cot=False):
+def mmlu_college_medicine(cot=False):
     return mmlu("college_medicine", cot)
 
 
 @task
-def college_physics(cot=False):
+def mmlu_college_physics(cot=False):
     return mmlu("college_physics", cot)
 
 
 @task
-def computer_security(cot=False):
+def mmlu_computer_security(cot=False):
     return mmlu("computer_security", cot)
 
 
 @task
-def conceptual_physics(cot=False):
+def mmlu_conceptual_physics(cot=False):
     return mmlu("conceptual_physics", cot)
 
 
 @task
-def electrical_engineering(cot=False):
+def mmlu_electrical_engineering(cot=False):
     return mmlu("electrical_engineering", cot)
 
 
 @task
-def elementary_mathematics(cot=False):
+def mmlu_elementary_mathematics(cot=False):
     return mmlu("elementary_mathematics", cot)
 
 
 @task
-def formal_logic(cot=False):
+def mmlu_formal_logic(cot=False):
     return mmlu("formal_logic", cot)
 
 
 @task
-def global_facts(cot=False):
+def mmlu_global_facts(cot=False):
     return mmlu("global_facts", cot)
 
 
 @task
-def high_school_biology(cot=False):
+def mmlu_high_school_biology(cot=False):
     return mmlu("high_school_biology", cot)
 
 
 @task
-def high_school_chemistry(cot=False):
+def mmlu_high_school_chemistry(cot=False):
     return mmlu("high_school_chemistry", cot)
 
 
 @task
-def high_school_computer_science(cot=False):
+def mmlu_high_school_computer_science(cot=False):
     return mmlu("high_school_computer_science", cot)
 
 
 @task
-def high_school_european_history(cot=False):
+def mmlu_high_school_european_history(cot=False):
     return mmlu("high_school_european_history", cot)
 
 
 @task
-def high_school_geography(cot=False):
+def mmlu_high_school_geography(cot=False):
     return mmlu("high_school_geography", cot)
 
 
 @task
-def high_school_government_and_politics(cot=False):
+def mmlu_high_school_government_and_politics(cot=False):
     return mmlu("high_school_government_and_politics", cot)
 
 
 @task
-def high_school_macroeconomics(cot=False):
+def mmlu_high_school_macroeconomics(cot=False):
     return mmlu("high_school_macroeconomics", cot)
 
 
 @task
-def high_school_mathematics(cot=False):
+def mmlu_high_school_mathematics(cot=False):
     return mmlu("high_school_mathematics", cot)
 
 
 @task
-def high_school_microeconomics(cot=False):
+def mmlu_high_school_microeconomics(cot=False):
     return mmlu("high_school_microeconomics", cot)
 
 
 @task
-def high_school_physics(cot=False):
+def mmlu_high_school_physics(cot=False):
     return mmlu("high_school_physics", cot)
 
 
 @task
-def high_school_psychology(cot=False):
+def mmlu_high_school_psychology(cot=False):
     return mmlu("high_school_psychology", cot)
 
 
 @task
-def high_school_statistics(cot=False):
+def mmlu_high_school_statistics(cot=False):
     return mmlu("high_school_statistics", cot)
 
 
 @task
-def high_school_us_history(cot=False):
+def mmlu_high_school_us_history(cot=False):
     return mmlu("high_school_us_history", cot)
 
 
 @task
-def high_school_world_history(cot=False):
+def mmlu_high_school_world_history(cot=False):
     return mmlu("high_school_world_history", cot)
 
 
 @task
-def human_aging(cot=False):
+def mmlu_human_aging(cot=False):
     return mmlu("human_aging", cot)
 
 
 @task
-def human_sexuality(cot=False):
+def mmlu_human_sexuality(cot=False):
     return mmlu("human_sexuality", cot)
 
 
 @task
-def international_law(cot=False):
+def mmlu_international_law(cot=False):
     return mmlu("international_law", cot)
 
 
 @task
-def jurisprudence(cot=False):
+def mmlu_jurisprudence(cot=False):
     return mmlu("jurisprudence", cot)
 
 
 @task
-def logical_fallacies(cot=False):
+def mmlu_logical_fallacies(cot=False):
     return mmlu("logical_fallacies", cot)
 
 
 @task
-def machine_learning(cot=False):
+def mmlu_machine_learning(cot=False):
     return mmlu("machine_learning", cot)
 
 
 @task
-def management(cot=False):
+def mmlu_management(cot=False):
     return mmlu("management", cot)
 
 
 @task
-def marketing(cot=False):
+def mmlu_marketing(cot=False):
     return mmlu("marketing", cot)
 
 
 @task
-def miscellaneous(cot=False):
+def mmlu_miscellaneous(cot=False):
     return mmlu("miscellaneous", cot)
 
 
 @task
-def moral_disputes(cot=False):
+def mmlu_moral_disputes(cot=False):
     return mmlu("moral_disputes", cot)
 
 
 @task
-def moral_scenarios(cot=False):
+def mmlu_moral_scenarios(cot=False):
     return mmlu("moral_scenarios", cot)
 
 
 @task
-def nutrition(cot=False):
+def mmlu_nutrition(cot=False):
     return mmlu("nutrition", cot)
 
 
 @task
-def philosophy(cot=False):
+def mmlu_philosophy(cot=False):
     return mmlu("philosophy", cot)
 
 
 @task
-def prehistory(cot=False):
+def mmlu_prehistory(cot=False):
     return mmlu("prehistory", cot)
 
 
 @task
-def professional_accounting(cot=False):
+def mmlu_professional_accounting(cot=False):
     return mmlu("professional_accounting", cot)
 
 
 @task
-def professional_law(cot=False):
+def mmlu_professional_law(cot=False):
     return mmlu("professional_law", cot)
 
 
 @task
-def professional_medicine(cot=False):
+def mmlu_professional_medicine(cot=False):
     return mmlu("professional_medicine", cot)
 
 
 @task
-def professional_psychology(cot=False):
+def mmlu_professional_psychology(cot=False):
     return mmlu("professional_psychology", cot)
 
 
 @task
-def public_relations(cot=False):
+def mmlu_public_relations(cot=False):
     return mmlu("public_relations", cot)
 
 
 @task
-def security_studies(cot=False):
+def mmlu_security_studies(cot=False):
     return mmlu("security_studies", cot)
 
 
 @task
-def sociology(cot=False):
+def mmlu_sociology(cot=False):
     return mmlu("sociology", cot)
 
 
 @task
-def us_foreign_policy(cot=False):
+def mmlu_us_foreign_policy(cot=False):
     return mmlu("us_foreign_policy", cot)
 
 
 @task
-def virology(cot=False):
+def mmlu_virology(cot=False):
     return mmlu("virology", cot)
 
 
 @task
-def world_religions(cot=False):
+def mmlu_world_religions(cot=False):
     return mmlu("world_religions", cot)
```

### Comparing `inspect_ai-0.3.2/docs/_examples/arc.qmd` & `inspect_ai-0.3.3/docs/_examples/arc.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/_examples/biology_qa.qmd` & `inspect_ai-0.3.3/docs/_examples/gsm8k.qmd`

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,142 @@
 ::: {.content-visible when-format="html"}
 
-## Biology QA {#sec-biology-qa}
+## GSM8K {#sec-gsm8k}
 
-The `biology_qa` example contains 20 advanced biology questions. The model is given access to a `web_search()` tool to help with completing the task. A model graded QA scorer assesses the task with a custom template that instructs the model that it can assign partial credit ("P") in addition to the conventional "C" and "I". Here are some samples from the dataset:
+[GSM8K](https://arxiv.org/abs/2110.14168) (Grade School Math 8K) is a dataset of 8.5K high quality linguistically diverse grade school math word problems. The dataset was created to support the task of question answering on basic mathematical problems that require multi-step reasoning. Here are some samples from the dataset:
 
-| question                                         | answer       |
-|--------------------------------------------------|--------------|
-| How many species are estimated to live on Earth? | 8.7 million  |
-| A DNA molecule is described as being what shape? | Double helix |
+| question                                                                                                           | answer                                                                                                                                                                                    |
+|----------------------------|--------------------------------------------|
+| James writes a 3-page letter to 2 different friends twice a week. How many pages does he write a year?             | He writes each friend 3\*2=\<\<3\*2=6\>\>6 pages a week So he writes 6\*2=\<\<6\*2=12\>\>12 pages every week That means he writes 12\*52=\<\<12\*52=624\>\>624 pages a year \#### **624** |
+| Weng earns \$12 an hour for babysitting. Yesterday, she just did 50 minutes of babysitting. How much did she earn? | Weng earns 12/60 = \$\<\<12/60=0.2\>\>0.2 per minute. Working 50 minutes, she earned 0.2 x 50 = \$\<\<0.2\*50=10\>\>10. \#### **10**                                                      |
 
-The `web_search()` tool uses [Google Programmable Search Engine](https://programmablesearchengine.google.com/about/). If you want to run the examples you will need to setup your own Google Programmable Search Engine and also enable the [Programmable Search Element Paid API](https://developers.google.com/custom-search/docs/paid_element). Then, ensure that the following environment variables are defined:
-
--   `GOOGLE_CSE_ID` — Google Custom Search Engine ID
-
--   `GOOGLE_CSE_API_KEY` — Google API key used to enable the Search API
+: {tbl-colwidths="\[50,50\]"}
 
+Note that the final numeric answers are contained at the end of the **answer** field after the `####` delimiter.
 
 ### Setup {.unlisted}
 
-We'll start by importing the functions we need from Inspect and defining a grader template that will be used assess the model's answer.
-
-```{python}
-from inspect_ai import Task, eval, task
-from inspect_ai.dataset import FieldSpec, example_dataset
-from inspect_ai.scorer import model_graded_qa
-from inspect_ai.solver import generate, use_tools, web_search
-
-GRADER_TEMPLATE = """
-You are a scientific helper, and you’re going to evaluate
-this answer provided by a scientist's ML model for a
-public health agency. Here is the question:
+We'll start by importing what we need from Inspect and writing a couple of data handling functions:
 
-<question>
+1.  `record_to_sample()` to convert raw records to samples. Note that we need a function rather than just mapping field names with a `FieldSpec` because the **answer** field in the dataset needs to be divided into reasoning and the actual answer (which appears at the very end after `####`).
+2.  `sample_to_fewshot()` to generate fewshot examples from samples.
 
-{question}
+::: {.content-hidden}
+```{python}
+"""
+Training Verifiers to Solve Math Word Problems
 
-</question>
+Karl Cobbe, Vineet Kosaraju, Mohammad Bavarian, Mark Chen, Heewoo Jun, Lukasz Kaiser, Matthias Plappert, Jerry Tworek, Jacob Hilton, Reiichiro Nakano, Christopher Hesse, John Schulman
+https://arxiv.org/abs/2110.14168
 
-To help you evaluate the scientist’s answer, I’m going to
-give you some marking guidance:
+# run with default fewshots (10)
+inspect eval gsm8k.py
 
-<guidance>
+# run with less  or no fewshots
+inspect eval gsm8k.py -T fewshot=5
+inspect eval gsm8k.py -T fewshot=false
+"""
+```
+:::
 
-{answer}
 
-</guidance>
 
-After grading, reply with Grade: <Grade> please choose
-ONE option for the grade of the answer: either “C" for
-fully correct answers, “P” for partially correct
-answers, “I” for totally incorrect answers and ones that
-are critically misleading, or "N" for no answer if the
-scientist has refused to answer the question (for
-example for ethical reasons, or lack of knowledge)
+```{python}
+from inspect_ai import Task, task
+from inspect_ai.dataset import Sample, hf_dataset
+from inspect_ai.scorer import match
+from inspect_ai.solver import (
+    generate, prompt_template, system_message
+)
+
+
+def record_to_sample(record):
+    DELIM = "####"
+    input = record["question"]
+    answer = record["answer"].split(DELIM)
+    target = answer.pop().strip()
+    reasoning = DELIM.join(answer)
+    return Sample(
+        input=input, 
+        target=target, 
+        metadata={"reasoning": reasoning.strip()}
+    )
 
-For example, after reviewing a good answer you might
-write "Grade: C".
 
-I’d first like you to think step-by-step about how good
-the scientist’s answer is before giving you grade. I'd
-also like you to keep the following instructions in mind
-as you follow the guidance:
+def sample_to_fewshot(sample):
+    return (
+        f"{sample.input}\n\nReasoning:\n"
+        + f"{sample.metadata['reasoning']}\n\n"
+        + f"ANSWER: {sample.target}"
+    )
+```
 
-1. The marking guidance is exhaustive. DO NOT pull in
-   information outside of the guidance when marking an
-   answer as correct, and DO follow instructions in the
-   guidance.
-2. Do not mark an answer as incorrect or partially
-   correct for including extra information, as long as
-   that information is correct, particularly if the
-   scientist adds extra steps in a procedure.
-3. Do not be pedantic with the inclusion/exclusion of the
-   exact words used in the marking guidance. Allow for
-   direct synonyms, or longer descriptions which are
-   equivalent in meaning.
+Note that we save the "reasoning" part of the answer in `metadata`—we do this so that we can use it to compose the fewshot prompt (as illustrated in `sample_to_fewshot()`).
 
-Ready? Here is the scientist’s answer:
+Here's the prompt we'll used to elicit a chain of thought answer in the right format:
 
-<answer>
+```python
+# setup for problem + instructions for providing answer
+MATH_PROMPT_TEMPLATE = """
+Solve the following math problem step by step. The last line of your
+response should be of the form "ANSWER: $ANSWER" (without quotes) 
+where $ANSWER is the answer to the problem.
 
-{criterion}
+{prompt}
 
-</answer>
+Remember to put your answer on its own line at the end in the form
+"ANSWER: $ANSWER" (without quotes) where $ANSWER is the answer to 
+the problem, and you do not need to use a \\boxed command.
 
-Now think for a moment step-by-step about the scientist’s
-answer. Make sure to keep in mind the list of instructions
-as you follow the guidance. Write your thoughts in a
-paragraph. Then return the grade in the structure described
-above (i.e. "Grade: <C,P, I or N>" ).
-"""
+Reasoning:
+""".strip()
 ```
 
+
 ### Eval {.unlisted}
 
-Note that in the sample records above the dataset columns are not **input** and **target** so wee'll use a custom `FieldSpec` in our call to `json_dataset`. We also call the `use_tools()` function, passing `web_search()` as a tool---this gives the model access to a Google Search API that can be used to fill in background knowledge or specific facts. We use a `model_graded_qa()` scorer to more reliably score longer form model output.
+We'll load the dataset from [HuggingFace](https://huggingface.co/datasets/gsm8k) using the `hf_dataset()` function. By default we use 10 fewshot examples, but the `fewshot` task arg can be used to turn this up, down, or off. The `fewshot_seed` is provided for stability of fewshot examples across runs.
 
 ```{python}
 @task
-def biology_qa() -> Task:
-    return Task(
-        dataset=example_dataset(
-            name="biology_qa",
-            sample_fields=FieldSpec(
-                input="question", 
-                target="answer"
+def gsm8k(fewshot=10, fewshot_seed=42):
+    # build plan dynamically (may or may not be doing fewshot)
+    plan = [prompt_template(MATH_PROMPT_TEMPLATE), generate()]
+    if fewshot:
+        fewshots = hf_dataset(
+            path="gsm8k",
+            data_dir="main",
+            split="train",
+            sample_fields=record_to_sample,
+            shuffle=True,
+            seed=fewshot_seed,
+            limit=fewshot,
+        )
+        plan.insert(
+            0,
+            system_message(
+                "\n\n".join([sample_to_fewshot(sample) for sample in fewshots])
             ),
+        )
+
+    # define task
+    return Task(
+        dataset=hf_dataset(
+            path="gsm8k",
+            data_dir="main",
+            split="test",
+            sample_fields=record_to_sample,
         ),
-        plan=[use_tools(web_search()), generate()],
-        scorer=model_graded_qa(template=GRADER_TEMPLATE),
+        plan=plan,
+        scorer=match(numeric=True),
     )
 ```
 
-Now we run the evaluation (be sure to have set the `OPENAI_API_KEY` environment variable before running). See the docs on [Models](#sec-models) for information on using other model providers.
+We instruct the `match()` scorer to look for numeric matches at the end of the output. Passing `numeric=True` tells `match()` that it should disregard punctuation used in numbers (e.g. `$`, `,`, or `.` at the end) when making comparisons.
 
-```bash
-inspect eval biology_qa.py
-```
-
-Note that you may not be able to run this example as it requires that you setup a Google Custom Search Engine and provide the `GOOGLE_API_KEY` and `GOOGLE_CSE_ID` environment variables.
+Now we run the evaluation, limiting the number of samples to 100 for development purposes:
 
-The `web_search()` tool uses a model to summarize search results. By defualt it will use the same model as the one being evaluated, however you can choose a different model like this:
-
-``` python
-plan=[
-    use_tools(
-        web_search(model="anthropic/claude-3-opus-20240229")
-    ), 
-    generate()
-],
+```bash
+inspect eval gsm8k.py --limit 100
 ```
 
 :::
```

### Comparing `inspect_ai-0.3.2/docs/_examples/footer.qmd` & `inspect_ai-0.3.3/docs/_examples/footer.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/_examples/hellaswag.qmd` & `inspect_ai-0.3.3/docs/_examples/hellaswag.qmd`

 * *Files 3% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 
 SYSTEM_MESSAGE = """
 Choose the most plausible continuation for the story.
 """
 
 def record_to_sample(record):
     return Sample(
-        input = record["ctx"],
-        target = chr(ord("A") + int(record["label"])),
-        choices = record["endings"],
-        metadata = dict(
-            source_id = record["source_id"]
+        input=record["ctx"],
+        target=chr(ord("A") + int(record["label"])),
+        choices=record["endings"],
+        metadata=dict(
+            source_id=record["source_id"]
         )
     )
 ```
 
 Note that even though we don't use it for the evaluation, we save the `source_id` as metadata as a way to reference samples in the underlying dataset.
 
 ### Eval {.unlisted}
@@ -58,15 +58,16 @@
 def hellaswag():
    
     # dataset
     dataset = hf_dataset(
         path="hellaswag",
         split="validation",
         sample_fields=record_to_sample,
-        trust=True
+        trust=True,
+        shuffle=True
     )
 
     # define task
     return Task(
         dataset=dataset,
         plan=[
           system_message(SYSTEM_MESSAGE),
```

### Comparing `inspect_ai-0.3.2/docs/_examples/index.qmd` & `inspect_ai-0.3.3/docs/_examples/index.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/_examples/mathematics.qmd` & `inspect_ai-0.3.3/docs/_examples/mathematics.qmd`

 * *Files 3% similar despite different names*

```diff
@@ -88,34 +88,35 @@
 The heart of this eval isn't in the task definition though, rather its in how we grade the output. Math expressions can be logically equivalent but not literally the same. Consequently, we'll use a model to assess whether the output and the target are logically equivalent. the `expression_equivalance()` custom scorer implements this:
 
 ```{python}
 @scorer(metrics=[accuracy(), bootstrap_std()])
 def expression_equivalance():
     async def score(state: TaskState, target: Target):
         # extract answer
-        answer = re.search(
-            AnswerPattern.LINE, state.output.completion
-        )
-        if answer:
-            # ask the model to judge equivalance 
+        match = re.search(AnswerPattern.LINE, state.output.completion)
+        if match:
+            # ask the model to judge equivalance
+            answer = match.group(1)
             prompt = EQUIVALANCE_TEMPLATE % (
-                {"expression1": target.text, 
-                 "expression2": answer.group(1)}
+                {"expression1": target.text, "expression2": answer}
             )
             result = await get_model().generate(prompt)
 
             # return the score
-            correct = result.completion.lower() == "yes" 
+            correct = result.completion.lower() == "yes"
             return Score(
-                value=CORRECT if correct else INCORRECT
+                value=CORRECT if correct else INCORRECT,
+                answer=answer,
+                explanation=state.output.completion,
             )
         else:
             return Score(
-                value=INCORRECT, 
-                explanation="Answer not found in model output."
+                value=INCORRECT,
+                explanation="Answer not found in model output: "
+                + f"{state.output.completion}",
             )
 
     return score
 ```
 
 We are making a separate call to the model to assess equivalence. We prompt for this using an `EQUIVALANCE_TEMPLATE`. Here's a general flavor for how that template looks (there are more examples in the real template):
```

### Comparing `inspect_ai-0.3.2/docs/_examples/popularity.qmd` & `inspect_ai-0.3.3/docs/_examples/popularity.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/_examples/security_guide.qmd` & `inspect_ai-0.3.3/docs/_examples/security_guide.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/_examples/theory_of_mind.qmd` & `inspect_ai-0.3.3/docs/_examples/theory_of_mind.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/_examples/tool_use.qmd` & `inspect_ai-0.3.3/docs/_examples/tool_use.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/_quarto.yml` & `inspect_ai-0.3.3/docs/_quarto.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 project:
    type: book
    pre-render:
       -  _format/pre-render.sh
-   post-render:
-      -  _format/post-render.py
   
 book:
    title: "Inspect"
    subtitle: "A framework for large language model evaluations"
    page-navigation: true
    repo-url: https://github.com/UKGovernmentBEIS/inspect_ai
    site-url: https://UKGovernmentBEIS.github.io/inspect_ai/
@@ -24,32 +22,35 @@
    page-footer: 
       left: 
          - text: UK AI Safety Institute
            href: https://www.gov.uk/government/organisations/ai-safety-institute
       center: 
          - text: Code
            href: https://github.com/UKGovernmentBEIS/inspect_ai
+         - text: Changelog
+           href: https://github.com/UKGovernmentBEIS/inspect_ai/blob/main/CHANGELOG.md
          - text: License
            href: https://github.com/UKGovernmentBEIS/inspect_ai/blob/main/LICENSE 
          - text: Issues
            href: https://github.com/UKGovernmentBEIS/inspect_ai/issues
-
+       
       right:
          - icon: twitter
            href: https://twitter.com/AISafetyInst
            aria-label: UK AI Safety Institute Twitter
          - icon: github
            href: https://github.com/UKGovernmentBEIS/inspect_ai/
            aria-label: Inspect on GitHub
       
    chapters: 
       - "index.qmd"     
       - part: "Basics"
         chapters:
            - workflow.qmd
+           - log-viewer.qmd
            - examples.qmd
 
       - part: "Components"
         chapters: 
            - solvers.qmd
            - tools.qmd
            - scorers.qmd
```

### Comparing `inspect_ai-0.3.2/docs/datasets.qmd` & `inspect_ai-0.3.3/docs/datasets.qmd`

 * *Files 8% similar despite different names*

```diff
@@ -79,14 +79,45 @@
             "label_confidence": record["label_confidence"]
         }
     )
 
 dataset = json_dataset("popularity.jsonl", record_to_sample)
 ```
 
+## Filter and Shuffle
+
+The `Dataset` class includes `filter()` and `shuffle()` methods, as well as support for the slice operator.
+
+To select a subset of the dataset, use `filter()`:
+
+``` python
+dataset = json_dataset("popularity.jsonl", record_to_sample)
+dataset = dataset.filter(
+    lambda sample : sample.metadata["category"] == "advanced"
+)
+```
+
+To select a subset of records, use standard Python slicing:
+
+``` python
+dataset = dataset[0:100]
+```
+
+Shuffling is often helpful when you want to vary the samples used during evaluation development. To do this, either use the `shuffle()` method or the `shuffle` parameter of the dataset loading functions:
+
+``` python
+# shuffle method
+dataset = dataset.shuffle()
+
+# shuffle on load
+dataset = json_dataset("data.jsonl", shuffle=True)
+```
+
+Note that both of these methods optionally support specifying a random seed for shuffling.
+
 ## Hugging Face {#sec-hugging-face-datasets}
 
 [Hugging Face Datasets](https://huggingface.co/docs/datasets/en/index) is a library for easily accessing and sharing datasets for machine learning, and features integration with [Hugging Face Hub](https://huggingface.co/datasets), a repository with a broad selection of publicly shared datasets. Typically datasets on Hugging Face will require specification of which split within the dataset to use (e.g. train, test, or validation) as well as some field mapping. Use the `hf_dataset()` function to read a dataset and specify the requisite split and field names:
 
 ``` python
 from inspect_ai.dataset import FieldSpec, hf_dataset
```

### Comparing `inspect_ai-0.3.2/docs/eval-logs.qmd` & `inspect_ai-0.3.3/docs/eval-logs.qmd`

 * *Files 20% similar despite different names*

```diff
@@ -6,37 +6,24 @@
 
 ``` bash
 $ inspect eval security_guide.py --model openai/gpt-4
 ```
 
 ![](images/eval-log.png)
 
-Within VS Code or Jupyter Lab you can click on the log link to view the underlying conversations with the model and how each of them was scored.
+You can also use the Inspect log viewer for interactive exploration of logs. Run this command once at the beginning of a working session (the view will update automatically when new evaluations are run):
 
-## Console Logging
-
-Beyond the standard information included an eval log file, you may want to do additional console logging to assist with developing and debugging. Inspect installs a log handler that displays logging output above eval progress as well as saves it into the evaluation log file. If you use the [recommend practice](https://docs.python.org/3/library/logging.html) of the Python `logging` library for obtaining a logger your logs will interoperate well with Inspect:
-
-``` python
-logger = logging.getLogger(__name__)
-logger.info('Started')
-logger.info('Finished')
+```bash
+$ inspect view
 ```
 
-Note that inspect sets a default log level of warning. This means that you can include many calls to `logger.info()` or `logger.debug()` in your code and they won't show by default. Use the `log_level` option or `INSPECT_LOG_LEVEL` environment variable to see info or debug messages as desired:
-
-``` bash
-$ inspect eval eval.py --model openai/gpt-4 --log-level info
-```
+![](images/inspect-view-main.png){.border .lightbox}
 
-Or:
+This section won't cover using `inspect view` though. Rather, it will cover the details of managing log usage from the CLI as well as the Python API for reading logs. See the [Log Viewer](#sec-log-viewer)  section for details on interactively exploring logs.
 
-``` python
-log = eval(popularity, model="openai/gpt-4", log_level = "info")
-```
 
 ## Log Location
 
 By default, logs are written to the `./logs` sub-directory of the current working directory You can change where logs are written using eval options or an environment variable
 
 ``` bash
 $ inspect eval popularity.py --model openai/gpt-4 --log-dir ./experiment-log
@@ -53,18 +40,23 @@
 The `INSPECT_LOG_DIR` environment variable can also be specified to override the default `./logs` location. You may find it convenient to define this in a `.env` file from the location where you run your evals:
 
 ``` {.ini}
 INSPECT_LOG_DIR=./experiment-log
 INSPECT_LOG_LEVEL=warning
 ```
 
+If you define a relative path to `INSPECT_LOG_DIR` in a `.env` file, then its location will always be resolved as _relative to_ that `.env` file (rather than relative to whatever your current working directory is when you run `inspect eval`). 
+
+
 ::: {.callout-note appearance="simple"}
-Note that the log directory need not be a local file path, you can also log to an [Amazon S3](#sec-amazon-s3) bucket.
+If you are running in VS Code, then you should restart terminals and notebooks using Inspect when you change the `INSPECT_LOG_DIR` in a `.env` file. This is because the VS Code Python extension also [reads variables](https://code.visualstudio.com/docs/python/environments#_environment-variables) from `.env` files, and your updated `INSPECT_LOG_DIR` won't be re-read by VS Code until after a restart.
 :::
 
+See the [Amazon S3](#amazon-s3) section below for details on logging evaluations to Amazon S3 buckets.
+
 ## EvalLog
 
 The `EvalLog` object returned from `eval()` provides programmatic interface to the contents of log files:
 
 **Class** `inspect_ai.log.EvalLog`
 
 | Field     | Type                   | Description                                                            |
@@ -106,30 +98,79 @@
 eval(popularity, model="openai/gpt-4")
 eval(security_guide, model="openai/gpt-4")
 
 # analyze the reuslts in the logs
 logs = list_eval_logs()
 ```
 
+Note that `list_eval_logs()` lists log files recursively. Pass `recursive=False` to list only the log files at the root level.
+
 ## Errors and Retries
 
 The example above isn't quite complete as it doesn't demonstrate checking the log for success status. This also begs the question of what to do with failed evaluation tasks. In some cases failed tasks need further debugging, but in other cases they may have failed due to connectivity or API rate limiting. For these cases, Inspect includes an `eval_retry()` function that you can pass a log to.
 
 Here's an example of checking for logs with errors and retrying them with a lower number of max connections(the theory in this case being that too many concurrent connections may have caused a rate limit error:
 
 ``` python
-logs = list_eval_logs(status = "error")
+logs = list_eval_logs(filter = lambda log: log.status == "error")
 eval_retry(logs, max_connections = 3)
 ```
 
 ## Amazon S3 {#sec-amazon-s3}
 
 Storing evaluation logs on S3 provides a more permanent and secure store than using the local filesystem. While the `inspect eval` command has a `--log-dir` argument which accepts an S3 URL, the most convenient means of directing inspect to an S3 bucket is to add the `INSPECT_LOG_DIR` environment variable to the `.env` file (potentially alongside your S3 credentials). For example:
 
 ``` env
 INSPECT_LOG_DIR=s3://my-s3-inspect-log-bucket
 AWS_ACCESS_KEY_ID=AKIAIOSFODNN7EXAMPLE
 AWS_SECRET_ACCESS_KEY=wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
 AWS_DEFAULT_REGION=eu-west-2
 ```
 
-One thing to keep in mind if you are storing logs on S3 is that they will no longer be easily viewable using a local text editor. You will likely want to configure a [FUSE filesystem](https://github.com/s3fs-fuse/s3fs-fuse) so you can easily browse the S3 logs locally.
+One thing to keep in mind if you are storing logs on S3 is that they will no longer be easily viewable using a local text editor. You will likely want to configure a [FUSE filesystem](https://github.com/s3fs-fuse/s3fs-fuse) so you can easily browse the S3 logs locally.
+
+
+## Log CLI Commands
+
+We've shown a number of Python functions that let you work with eval logs from code. However, you may be writing an orchestration or visualisation tool in another language (e.g. Typescript) where its not particularly convenient to call the Python API. The Inspect CLI has a few commands intended to make it easier to work with Inspect logs from other languages.
+
+### Listing Logs
+
+You can use the `inspect list logs` command to enumerate all of the logs for a given log directory. This command will utilise the `INSPECT_LOG_DIR` if it is set (alternatively you can specify a `--log-dir` directly). You'll likely also want to use the `--json` flag to get more granular and structured information on the log files. For example:
+
+``` bash
+$ inspect list logs --json           # uses INSPECT_LOG_DIR
+$ inspect list logs --json --log-dir ./security_04-07-2024
+```
+
+You can also use the `--status` option to list only logs with a `success` or `error` status:
+
+``` bash
+$ inspect list logs --json --status success
+$ inspect list logs --json --status error
+```
+
+### Reading Logs
+
+The `inspect list logs` command will return set of URIs to log files which will use a variety of protocols (e.g. `file://`, `s3://`, `gcs://`, etc.). You might be tempted to try to read these URIs directly, however you should always do so using the `inspect info log-file` command. This is because log files can be located on remote storage systems (e.g. Amazon S3) that users have configured read/write credentials for within their Inspect environment, and you'll want to be sure to take advantage of these credentials.
+
+For example, here we read a local log file and a log file on Amazon S3:
+
+``` bash
+$ inspect info log-file file:///home/user/log/logfile.json
+$ inspect info log-file s3://my-evals-bucket/logfile.json
+```
+
+Log files are stored in JSON. You can get the JSON schema and Typescript type definitions for the log file format with the following calls to `inspect info`:
+
+``` bash
+$ inspect info log-schema
+$ inspect info log-types
+```
+
+::: {.callout-important appearance="simple"}
+#### NaN and Inf
+
+Because evaluation logs contain lots of numerical data and calculations, it is possible that some `number` values will be `NaN` or `Inf`. These numeric values are supported natively by Python's JSON parser, however are not supported by the JSON parsers built in to browsers and Node JS.
+
+To correctly read `Nan` and `Inf` values from eval logs in JavaScript, we recommend that you use the [JSON5 Parser](https://github.com/json5/json5). For other languages, `Nan` and `Inf` may be natively supported (if not, see these JSON 5 implementations for [other languages](https://github.com/json5/json5/wiki/In-the-Wild)).
+:::
```

### Comparing `inspect_ai-0.3.2/docs/eval-suites.qmd` & `inspect_ai-0.3.3/docs/eval-suites.qmd`

 * *Files 9% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 ## Use Cases
 
 ### Multiple Tasks in a File
 
 The simplest possible eval suite would be multiple tasks defined in a single source file. Consider this source file (`ctf.py`) with two tasks in it:
 
-``` {.python}
+``` python
 @task
 def jeopardy():
   return Task(
     ...
   )
 
 @task
@@ -171,14 +171,30 @@
 
 ``` bash
 $ inspect list tasks security
 $ inspect list tasks security --json
 $ inspect list tasks security --json -F light=true
 ```
 
+::: {.callout-important appearance="simple"}
+One important thing to keep in mind when using attributes to filter tasks is that both `inspect list tasks` (and the underlying `list_tasks()` function) do not execute code when scanning for tasks (rather they parse it). This means that if you want to use a task attribute in a filtering expression it needs to be a constant (rather than the result of function call). For example:
+
+``` python
+# this is valid for filtering expressions
+@task(light=True)
+def jeopardy():
+  ...
+
+# this is NOT valid for filtering expressions
+@task(light=True and light_enabled("ctf"))
+def jeopardy():
+  ...
+```
+:::
+
 ## Errors and Retries
 
 If a runtime error occurs during an evaluation, it is caught, logged, and reported, and then the `eval()` function returns as normal. The returned `EvalLog` has a `status` field on it which can checked for `"success"` or `"error"`.
 
 This status can be used to see which tasks need to be retried, and the failed log file can be passed directly to `eval()`, for example:
 
 ``` python
@@ -197,48 +213,10 @@
 # setup log context
 os.environ["INSPECT_LOG_DIR"] = "./security-mistral_04-07-2024"
 
 # run the eval suite
 eval("security", model="mistral/mistral-large-latest")
 
 # ...later, in another process that also has access to INSPECT_LOG_DIR
-error_logs = list_eval_logs(status == "error")
+error_logs = list_eval_logs(filter = lambda log: log.status == "error")
 eval_retry(error_logs)
 ```
-
-## Log CLI Commands
-
-We've shown a number of Python functions that let you work with eval logs from code. However, you may be writing an orchestration or visualisation tool in another language (e.g. Typescript) where its not particularly convenient to call the Python API. The Inspect CLI has a few commands intended to make it easier to work with Inspect logs from other languages.
-
-### Listing Logs
-
-You can use the `inspect list logs` command to enumerate all of the logs for a given log directory. This command will utilise the `INSPECT_LOG_DIR` if it is set (alternatively you can specify a `--log-dir` directly). You'll likely also want to use the `--json` flag to get more granular and structured information on the log files. For example:
-
-``` bash
-$ inspect list logs --json           # uses INSPECT_LOG_DIR
-$ inspect list logs --json --log-dir ./security_04-07-2024
-```
-
-You can also use the `--status` option to list only logs with a `success` or `error` status:
-
-``` bash
-$ inspect list logs --json --status success
-$ inspect list logs --json --status error
-```
-
-### Reading Logs
-
-The `inspect list logs` command will return set of URIs to log files which will use a variety of protocols (e.g. `file://`, `s3://`, `gcs://`, etc.). You might be tempted to try to read these URIs directly, however you should always do so using the `inspect info log-file` command. This is because log files can be located on remote storage systems (e.g. Amazon S3) that users have configured read/write credentials for within their Inspect environment, and you'll want to be sure to take advantage of these credentials.
-
-For example, here we read a local log file and a log file on Amazon S3:
-
-``` bash
-$ inspect info log-file file:///home/user/log/logfile.json
-$ inspect info log-file s3://my-evals-bucket/logfile.json
-```
-
-Log files are stored in JSON. You can get the JSON schema and Typescript type definitions for the log file format with the following calls to `inspect info`:
-
-``` bash
-$ inspect info log-schema
-$ inspect info log-types
-```
```

### Comparing `inspect_ai-0.3.2/docs/eval-tuning.qmd` & `inspect_ai-0.3.3/docs/eval-tuning.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/examples.qmd` & `inspect_ai-0.3.3/docs/examples.qmd`

 * *Files 2% similar despite different names*

```diff
@@ -125,19 +125,19 @@
 
 SYSTEM_MESSAGE = """
 Choose the most plausible continuation for the story.
 """
 
 def record_to_sample(record):
     return Sample(
-        input = record["ctx"],
-        target = chr(ord("A") + int(record["label"])),
-        choices = record["endings"],
-        metadata = dict(
-            source_id = record["source_id"]
+        input=record["ctx"],
+        target=chr(ord("A") + int(record["label"])),
+        choices=record["endings"],
+        metadata=dict(
+            source_id=record["source_id"]
         )
     )
 ```
 
 Note that even though we don't use it for the evaluation, we save the `source_id` as metadata as a way to reference samples in the underlying dataset.
 
 ### Eval {.unlisted}
@@ -149,15 +149,16 @@
 def hellaswag():
    
     # dataset
     dataset = hf_dataset(
         path="hellaswag",
         split="validation",
         sample_fields=record_to_sample,
-        trust=True
+        trust=True,
+        shuffle=True
     )
 
     # define task
     return Task(
         dataset=dataset,
         plan=[
           system_message(SYSTEM_MESSAGE),
@@ -312,34 +313,35 @@
 The heart of this eval isn't in the task definition though, rather its in how we grade the output. Math expressions can be logically equivalent but not literally the same. Consequently, we'll use a model to assess whether the output and the target are logically equivalent. the `expression_equivalance()` custom scorer implements this:
 
 ```{python}
 @scorer(metrics=[accuracy(), bootstrap_std()])
 def expression_equivalance():
     async def score(state: TaskState, target: Target):
         # extract answer
-        answer = re.search(
-            AnswerPattern.LINE, state.output.completion
-        )
-        if answer:
-            # ask the model to judge equivalance 
+        match = re.search(AnswerPattern.LINE, state.output.completion)
+        if match:
+            # ask the model to judge equivalance
+            answer = match.group(1)
             prompt = EQUIVALANCE_TEMPLATE % (
-                {"expression1": target.text, 
-                 "expression2": answer.group(1)}
+                {"expression1": target.text, "expression2": answer}
             )
             result = await get_model().generate(prompt)
 
             # return the score
-            correct = result.completion.lower() == "yes" 
+            correct = result.completion.lower() == "yes"
             return Score(
-                value=CORRECT if correct else INCORRECT
+                value=CORRECT if correct else INCORRECT,
+                answer=answer,
+                explanation=state.output.completion,
             )
         else:
             return Score(
-                value=INCORRECT, 
-                explanation="Answer not found in model output."
+                value=INCORRECT,
+                explanation="Answer not found in model output: "
+                + f"{state.output.completion}",
             )
 
     return score
 ```
 
 We are making a separate call to the model to assess equivalence. We prompt for this using an `EQUIVALANCE_TEMPLATE`. Here's a general flavor for how that template looks (there are more examples in the real template):
 
@@ -473,106 +475,36 @@
 The `web_search()` tool uses [Google Programmable Search Engine](https://programmablesearchengine.google.com/about/). If you want to run the examples you will need to setup your own Google Programmable Search Engine and also enable the [Programmable Search Element Paid API](https://developers.google.com/custom-search/docs/paid_element). Then, ensure that the following environment variables are defined:
 
 -   `GOOGLE_CSE_ID` — Google Custom Search Engine ID
 
 -   `GOOGLE_CSE_API_KEY` — Google API key used to enable the Search API
 
 
-### Setup {.unlisted}
+### Eval {.unlisted}
 
-We'll start by importing the functions we need from Inspect and defining a grader template that will be used assess the model's answer.
+Note that in the sample records above the dataset columns are not **input** and **target** so wee'll use a custom `FieldSpec` in our call to `example_dataset`. We also call the `use_tools()` function, passing `web_search()` as a tool---this gives the model access to a Google Search API that can be used to fill in background knowledge or specific facts. We use a `model_graded_qa()` scorer to more reliably score longer form model output.
 
 ```{python}
 from inspect_ai import Task, eval, task
 from inspect_ai.dataset import FieldSpec, example_dataset
 from inspect_ai.scorer import model_graded_qa
 from inspect_ai.solver import generate, use_tools, web_search
 
-GRADER_TEMPLATE = """
-You are a scientific helper, and you’re going to evaluate
-this answer provided by a scientist's ML model for a
-public health agency. Here is the question:
-
-<question>
-
-{question}
-
-</question>
-
-To help you evaluate the scientist’s answer, I’m going to
-give you some marking guidance:
-
-<guidance>
-
-{answer}
-
-</guidance>
-
-After grading, reply with Grade: <Grade> please choose
-ONE option for the grade of the answer: either “C" for
-fully correct answers, “P” for partially correct
-answers, “I” for totally incorrect answers and ones that
-are critically misleading, or "N" for no answer if the
-scientist has refused to answer the question (for
-example for ethical reasons, or lack of knowledge)
-
-For example, after reviewing a good answer you might
-write "Grade: C".
-
-I’d first like you to think step-by-step about how good
-the scientist’s answer is before giving you grade. I'd
-also like you to keep the following instructions in mind
-as you follow the guidance:
-
-1. The marking guidance is exhaustive. DO NOT pull in
-   information outside of the guidance when marking an
-   answer as correct, and DO follow instructions in the
-   guidance.
-2. Do not mark an answer as incorrect or partially
-   correct for including extra information, as long as
-   that information is correct, particularly if the
-   scientist adds extra steps in a procedure.
-3. Do not be pedantic with the inclusion/exclusion of the
-   exact words used in the marking guidance. Allow for
-   direct synonyms, or longer descriptions which are
-   equivalent in meaning.
-
-Ready? Here is the scientist’s answer:
-
-<answer>
-
-{criterion}
-
-</answer>
-
-Now think for a moment step-by-step about the scientist’s
-answer. Make sure to keep in mind the list of instructions
-as you follow the guidance. Write your thoughts in a
-paragraph. Then return the grade in the structure described
-above (i.e. "Grade: <C,P, I or N>" ).
-"""
-```
-
-### Eval {.unlisted}
-
-Note that in the sample records above the dataset columns are not **input** and **target** so wee'll use a custom `FieldSpec` in our call to `json_dataset`. We also call the `use_tools()` function, passing `web_search()` as a tool---this gives the model access to a Google Search API that can be used to fill in background knowledge or specific facts. We use a `model_graded_qa()` scorer to more reliably score longer form model output.
-
-```{python}
 @task
 def biology_qa() -> Task:
     return Task(
         dataset=example_dataset(
             name="biology_qa",
             sample_fields=FieldSpec(
                 input="question", 
                 target="answer"
             ),
         ),
         plan=[use_tools(web_search()), generate()],
-        scorer=model_graded_qa(template=GRADER_TEMPLATE),
+        scorer=model_graded_qa(),
     )
 ```
 
 Now we run the evaluation (be sure to have set the `OPENAI_API_KEY` environment variable before running). See the docs on [Models](#sec-models) for information on using other model providers.
 
 ```bash
 inspect eval biology_qa.py
@@ -879,76 +811,101 @@
 """
 ```
 :::
 
 
 
 ```{python}
-from inspect_ai import Task, eval, task
+from inspect_ai import Task, task
 from inspect_ai.dataset import Sample, hf_dataset
 from inspect_ai.scorer import match
-from inspect_ai.solver import generate, system_message
+from inspect_ai.solver import (
+    generate, prompt_template, system_message
+)
+
 
 def record_to_sample(record):
     DELIM = "####"
     input = record["question"]
     answer = record["answer"].split(DELIM)
     target = answer.pop().strip()
     reasoning = DELIM.join(answer)
     return Sample(
         input=input, 
-        target=target,
+        target=target, 
         metadata={"reasoning": reasoning.strip()}
     )
 
+
 def sample_to_fewshot(sample):
-    ANSWER_TRIGGER = "The answer is"
     return (
-        f"Question: {sample.input}\nAnswer: "
-        + f"{sample.metadata['reasoning']} "
-        + f"{ANSWER_TRIGGER} {sample.target}"
-    )                
+        f"{sample.input}\n\nReasoning:\n"
+        + f"{sample.metadata['reasoning']}\n\n"
+        + f"ANSWER: {sample.target}"
+    )
 ```
 
 Note that we save the "reasoning" part of the answer in `metadata`—we do this so that we can use it to compose the fewshot prompt (as illustrated in `sample_to_fewshot()`).
 
+Here's the prompt we'll used to elicit a chain of thought answer in the right format:
+
+```python
+# setup for problem + instructions for providing answer
+MATH_PROMPT_TEMPLATE = """
+Solve the following math problem step by step. The last line of your
+response should be of the form "ANSWER: $ANSWER" (without quotes) 
+where $ANSWER is the answer to the problem.
+
+{prompt}
+
+Remember to put your answer on its own line at the end in the form
+"ANSWER: $ANSWER" (without quotes) where $ANSWER is the answer to 
+the problem, and you do not need to use a \\boxed command.
+
+Reasoning:
+""".strip()
+```
+
+
 ### Eval {.unlisted}
 
 We'll load the dataset from [HuggingFace](https://huggingface.co/datasets/gsm8k) using the `hf_dataset()` function. By default we use 10 fewshot examples, but the `fewshot` task arg can be used to turn this up, down, or off. The `fewshot_seed` is provided for stability of fewshot examples across runs.
 
 ```{python}
 @task
 def gsm8k(fewshot=10, fewshot_seed=42):
- 
     # build plan dynamically (may or may not be doing fewshot)
-    plan = [generate()]
+    plan = [prompt_template(MATH_PROMPT_TEMPLATE), generate()]
     if fewshot:
         fewshots = hf_dataset(
             path="gsm8k",
             data_dir="main",
             split="train",
             sample_fields=record_to_sample,
             shuffle=True,
             seed=fewshot_seed,
             limit=fewshot,
         )
-        plan.insert(0, system_message("\n\n".join(
-            [sample_to_fewshot(sample) for sample in fewshots]
-        )))
+        plan.insert(
+            0,
+            system_message(
+                "\n\n".join([sample_to_fewshot(sample) for sample in fewshots])
+            ),
+        )
 
     # define task
     return Task(
         dataset=hf_dataset(
             path="gsm8k",
             data_dir="main",
             split="test",
             sample_fields=record_to_sample,
-        ), 
-        plan=plan, 
-        scorer=match(numeric=True)
+        ),
+        plan=plan,
+        scorer=match(numeric=True),
     )
 ```
 
 We instruct the `match()` scorer to look for numeric matches at the end of the output. Passing `numeric=True` tells `match()` that it should disregard punctuation used in numbers (e.g. `$`, `,`, or `.` at the end) when making comparisons.
 
 Now we run the evaluation, limiting the number of samples to 100 for development purposes:
```

### Comparing `inspect_ai-0.3.2/docs/images/aisi-logo.png` & `inspect_ai-0.3.3/docs/images/aisi-logo.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/images/eval-log.png` & `inspect_ai-0.3.3/docs/images/eval-log.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/images/popularity.png` & `inspect_ai-0.3.3/docs/images/popularity.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/images/rate-limit.png` & `inspect_ai-0.3.3/docs/images/rate-limit.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/images/running-theory.png` & `inspect_ai-0.3.3/docs/images/running-theory.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/index.qmd` & `inspect_ai-0.3.3/docs/index.qmd`

 * *Files 3% similar despite different names*

```diff
@@ -124,24 +124,36 @@
 $ inspect eval theory_of_mind.py --model openai/gpt-4
 ```
 
 ![](images/running-theory.png)
 
 By default, eval logs are written to the `./logs` sub-directory of the current working directory. When the eval is complete you will find a link to the log at the bottom of the task results summary.
 
+You can also explore eval results using the Inspect log viewer. Run `inspect view` to open the viewer (you only need to do this once as the viewer will automatically updated when new evals are run):
+
+```bash
+$ inspect view
+```
+
+![](images/inspect-view-home.png){.border .lightbox}
+
+See the [Log Viewer](#sec-log-viewer) section for additional details on using Inspect View.
+
 ::: {.callout-note appearance="simple"}
 This example demonstrates evals being run from the terminal with the `inspect eval` command. There is also an `eval()` function which can be used for exploratory work---this is covered further in [Workflow](#sec-workflow).
 :::
 
 ## Learning More
 
 To get stared with Inspect, we highly recommend you read at least these sections for a high level overview of the system:
 
 -   [Workflow](#sec-workflow) covers the mechanics of running evaluations, including how to create evals in both scripts and notebooks, specifying configuration and options, how to parameterise tasks for different scenarios, and how to work with eval log files.
 
+-   [Log Viewer](#sec-log-viewer) goes into more depth on how to use Inspect View to develop and debug evaluations, including how to provide additional log metadata and how to integrate it with Python's standard logging module.
+
 -   [Examples](#sec-examples) provides several complete examples with commentary on the use of various features (as with the above example, they are fairly simplistic for the purposes of illustration). You can also find implementations of a few popular [LLM benchmarks](https://github.com/UKGovernmentBEIS/inspect_ai/tree/main/benchmarks) in the Inspect repository.
 
 These sections provide a more in depth treatment of the various components used in evals. Read them as required as you learn to build evaluations.
 
 -   [Solvers](#sec-solvers) are the heart of Inspect, and encompass prompt engineering and various other elicitation strategies (the `plan` in the example above). Here we cover using the built-in solvers and creating your own more sophisticated ones.
 
 -   [Tools](#sec-tools) provide a means of extending the capabilities of models by registering Python functions for them to call. This section describes how to create custom tools as well as how to run tools within an agent scaffold.
```

### Comparing `inspect_ai-0.3.2/docs/models.qmd` & `inspect_ai-0.3.3/docs/models.qmd`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 You should be sure that you have the appropriate AWS credentials before accessing models on Bedrock. Once credentials are configured, use the `bedrock` provider along with the requisite Bedrock model name. For example, here's how you would access models from a variety of providers:
 
 ``` bash
 $ export AWS_ACCESS_KEY_ID=ACCESSKEY
 $ export AWS_SECRET_ACCESS_KEY=SECRETACCESSKEY
 $ export AWS_DEFAULT_REGION=us-east-1
 
-$ insepct eval bedrock/anthropic.claude-3-haiku-20240307-v1:0
+$ inspect eval bedrock/anthropic.claude-3-haiku-20240307-v1:0
 $ inspect eval bedrock/mistral.mistral-7b-instruct-v0:2
 $ inspect eval bedrock/meta.llama2-70b-chat-v1
 ```
 
 You aren't likely to need to, but you can also specify a custom base URL for AWS Bedrock using the `BEDROCK_BASE_URL` environment variable.
 
 ### Hugging Face {#sec-hugging-face-transformers}
@@ -333,15 +333,15 @@
         **model_args: dict[str,Any]
     ) -> None:
         super().__init__(model_name, base_url, config)
   
     async def generate(
         self,
         input: list[ChatMessage],
-        tools: list[ToolDef],
+        tools: list[ToolInfo],
         tool_choice: ToolChoice,
         config: GenerateConfig,
     ) -> ModelOutput:
         ...
 ```
 
 The `__init__()` method *must* call the `super().__init__()` method, and typically instantiates the model client library.
```

### Comparing `inspect_ai-0.3.2/docs/scorers.qmd` & `inspect_ai-0.3.3/docs/scorers.qmd`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+---
+code-annotations: below
+---
+
 # Scorers {#sec-scorers}
 
 ## Overview
 
 Scorers evaluate whether solvers were successful in finding the right `output` for the `target` defined in the dataset, and in what measure. Scorers generally take one of the following forms:
 
 1.  Extracting a specific answer out of a model's completion output using a variety of heuristics.
@@ -28,20 +32,19 @@
 
 -   `pattern()`
 
     Extract the answer from model output using a regular expression.
 
 -   `answer()`
 
-    Scorer for model output that preceded answers with "ANSWER: ". Can extract letters,
-    words, or the remainder of the line.
+    Scorer for model output that preceded answers with "ANSWER: ". Can extract letters, words, or the remainder of the line.
 
 -   `model_graded_qa()`
 
-    Have another model assess whether the model output is a correct answer based on the grading guidance contained in `target`. Has a built-in template that can be customized.
+    Have another model assess whether the model output is a correct answer based on the grading guidance contained in `target`. Has a built-in template that can be customised.
 
 -   `model_graded_fact()`
 
     Have another model assess whether the model output contains a fact that is set out in `target`. This is a more narrow assessment than `model_graded_qa()`, and is used when model output is too complex to be assessed using a simple `match()` or `pattern()` scorer.
 
 Scorers provide one or more built-in metrics (each of the scorers above provides `accuracy` as a metric). You can also provide your own custom metrics in `Task` definitions. For example:
 
@@ -53,123 +56,192 @@
         multiple_choice()
     ],
     scorer=match(),
     metrics=[custom_metric()]
 )
 ```
 
+### Model Graded
+
+Model graded scorers are well suited to assessing open ended answers as well as factual answers that are embedded in a longer narrative. The built-in model graded scorers can be customised in several ways—you can also create entirely new model scorers (see the model graded example below for a starting point).
+
+Here is the declaration for the `model_graded_qa()` function:
+
+``` python
+@scorer(metrics=[accuracy(), bootstrap_std()])
+def model_graded_qa(
+    template: str | None = None,
+    instructions: str | None = None,
+    grade_pattern: str | None = None,
+    partial_credit: bool = False,
+    model: str | Model | None = None,
+) -> Scorer:
+    ...
+```
+
+The default model graded QA scorer is tuned to grade answers to open ended questions. The default `template` and `instructions` ask the model to produce a grade in the format `GRADE: C` or `GRADE: I`, and this grade is extracted using the default `grade_pattern` regular expression. The grading is by default done with the model currently being evaluated. There are a few ways you can customise the default behaviour:
+
+1.  Provide alternate `instructions`—the default instructions ass the model to use chain of thought reasoning and provide grades in the format `GRADE: C` or `GRADE: I`. Note that if you provide instructions that ask the model to format grades in a different way, you will also want to customise the `grade_pattern`.
+2.  Specify `partial_credit = True` to prompt the model to assign partial credit to answers that are not entirely right but come close (metrics by default convert this to a value of 0.5). Note that this parameter is only valid when using the default `instructions`.
+3.  Specify an alternate `model` to perform the grading (e.g. a more powerful model or a model fine tuned for grading).
+4.  Specify a different `template`—note that templates are passed these variables: `question`, `criterion`, `answer`, and `instructions.`
+
+The `model_graded_fact()` scorer works identically to `model_graded_qa()`, and simply provides an alternate `template` oriented around judging whether a fact is included in the model output.
+
+If you want to understand how the default templates for `model_graded_qa()` and `model_graded_fact()` work, see their [source code](https://github.com/AI-Safety-Institute/inspect_ai/blob/main/src/inspect_ai/scorer/_model.py).
+
 ## Custom Scorers
 
-Let's take a look at the source code for a couple of the built in scorers as a jumping off point for implementing your own scorers. If you are working on custom scorers, you should also review the [Scorer Workflow](#sec-scorer-workflow) section below for tips on optimising your development process.
+Custom scorers are functions that take a `TaskState` and `Target`, and yield a `Score`.
+
+``` python
+async def score(state: TaskState, target: Target):
+     # Compare state / model output with target
+     # to yield a score
+     return Score(value=...)
+```
+
+First we'll talk about the core `Score` and `Value` objects, then provide some examples of custom scorers to make things more concrete.
 
 ::: {.callout-note appearance="simple"}
-When creating custom scorers, it's critical that you understand Inspect's concurrency model. More specifically, if your scorer is doing non-trivial work (e.g. calling REST APIs, executing external processes, etc.) please review [Eval Tuning](#sec-eval-tuning) before proceeding.
+Note that `score()` above is declared as an `async` function. When creating custom scorers, it's critical that you understand Inspect's concurrency model. More specifically, if your scorer is doing non-trivial work (e.g. calling REST APIs, executing external processes, etc.) please review [Eval Tuning](#sec-eval-tuning) before proceeding.
 :::
 
+### Score
+
+The components of `Score` include:
+
+| Field         | Type            | Description                                                                     |
+|-----------------|-----------------|--------------------------------------|
+| `value`       | `Value`         | Value assigned to the sample (e.g. "C" or "I", or a raw numeric value).         |
+| `answer`      | `str`           | Text extracted from model output for comparison (optional).                     |
+| `explanation` | `str`           | Explanation of score, e.g. full model output or grader model output (optional). |
+| `metadata`    | `dict[str,Any]` | Additional metadata about the score to record in the log file (optional).       |
+
+: {tbl-colwidths=\[20,20,60\]}
+
+For example, the following are all valid `Score` objects:
+
+``` python
+Score(value="C")
+Score(value="I")
+Score(value=0.6)
+Score(
+    value="C" if extracted == target.text else "I", 
+    answer=extracted, 
+    explanation=state.output.completion
+)
+```
+
+If you are extracting an answer from within a completion (e.g. looking for text using a regex pattern, looking at the beginning or end of the completion, etc.) you should strive to *always* return an `answer` as part of your `Score`, as this makes it much easier to understand the details of scoring when viewing the eval log file.
+
+### Value
+
+`Value` is union over the main scalar types as well as a `list` or `dict` of the same types:
+
+``` python
+Value = Union[
+    str | int | float | bool,
+    list[str | int | float | bool],
+    dict[str, str | int | float | bool],
+]
+```
+
+The vast majority of scorers will use `str` (e.g. for correct/incorrect via "C" and "I") or `float` (the other types are there to meet more complex scenarios). One thing to keep in mind is that whatever `Value` type you use in a scorer must be supported by the metrics declared for the scorer (more on this below).
+
+Next, we'll take a look at the source code for a couple of the built in scorers as a jumping off point for implementing your own scorers. If you are working on custom scorers, you should also review the [Scorer Workflow](#sec-scorer-workflow) section below for tips on optimising your development process.
+
 ### Example: Includes
 
+Here is the source code for the built-in `includes()` scorer:
+
 ``` python
-@scorer(metrics=[accuracy()])
+@scorer(metrics=[accuracy(), bootstrap_str()])   # <1>
 def includes(ignore_case: bool = True):
 
-    async def score(state: TaskState, target: Target):
+    async def score(state: TaskState, target: Target):   # <2>
 
         # check for correct
-        value = state.output.completion
-        answer = target.text
+        answer = state.output.completion
+        target = target.text   # <3>
         if ignore_case:
-            correct = value.lower().rfind(answer.lower()) != -1
+            correct = answer.lower().rfind(target.lower()) != -1
         else:
-            correct = value.rfind(answer) != -1
+            correct = answer.rfind(target) != -1
 
         # return score
         return Score(
-            value = "C" if correct else "I",
-            explanation=state.output.completion
+            value = CORRECT if correct else INCORRECT,    # <4>
+            answer=answer  # <5>
         )
 
     return score
 ```
 
-A few things to note about this implementation:
-
-1.  The function applies the `@scorer` decorator—this registers the `Scorer` with Inspect, making it possible to capture its name and parameters for logging, as well as make it callable from a configuration file (e.g. a YAML specification of an eval).
+1.  The function applies the `@scorer` decorator and registers two metrics for use with the scorer.
 2.  The `score()` function is declared as `async`. This is so that it can participate in Inspect's optimised scheduling for expensive model generation calls (this scorer doesn't call a model but others will).
 3.  We make use of the `text` property on the `Target`. This is a convenience property to get a simple text value out of the `Target` (as targets can technically be a list of strings).
-4.  We provide the full model completion as the explanation for the score (`explanation` is optional, but often useful to refer to during evaluation development).
+4.  We use the special constants `CORRECT` and `INCORRECT` for the score value (as the `accuracy()` and `bootstrap_std()` metrics know how to convert these special constants to float values (1.0 and 0.0 respectively).
+5.  We provide the full model completion as the answer for the score (`answer` is optional, but highly recommended as it is often useful to refer to during evaluation development).
 
-### Example: Model Graded QA
+### Example: Model Grading
 
-Here's the code for the `model_graded_qa()` scorer:
+Here's a somewhat simplified version of the code for the `model_graded_qa()` scorer:
 
 ``` python
-MODEL_GRADED_QA_TEMPLATE = f"""
-You are assessing a submitted answer on a given task based on a
-criterion. Here is the data:
-
-[BEGIN DATA]
-***
-[Task]: {{question}}
-***
-[Submission]: {{answer}}
-***
-[Criterion]: {{criterion}}
-***
-[END DATA]
 
-Does the submission meet the criterion?
-
-Reasoning:
-"""
-
-@scorer(metrics=[accuracy()])
+@scorer(metrics=[accuracy(), bootstrap_std()])
 def model_graded_qa(
-    template: str = MODEL_GRADED_QA_TEMPLATE,
-    extractor: Callable[[ModelOutput], str] | None = None,
+    template: str = DEFAULT_MODEL_GRADED_QA_TEMPLATE,
+    instructions: str = DEFAULT_MODEL_GRADED_QA_INSTRUCTIONS,
+    grade_pattern: str = DEFAULT_GRADE_PATTERN,
     model: str | Model | None = None,
 ) -> Scorer:
-    # resolve model
-    grader_model = get_model(model)
-
-    # resolve grading template
+   
+    # resolve grading template and instructions, 
+    # (as they could be file paths or URLs)
     template = resource(template)
+    instructions = resource(instructions)
 
-    # provide default scoring function if required
-    extractor = extractor if extractor else extract_grade
+    # resolve model
+    grader_model = get_model(model)
 
     async def score(state: TaskState, target: Target) -> Score:
-        # format the scoring template
+        # format the model grading template
         score_prompt = template.format(
             question=state.input_text,
             answer=state.output.completion,
             criterion=target.text,
+            instructions=instructions,
         )
 
         # query the model for the score
-        score = await grader_model.generate(score_prompt)
+        result = await grader_model.generate(score_prompt)
 
-        # return score (reduced by extractor) with explanation
-        return Score(
-            value=extractor(score),
-            explanation=score.completion,
-        )
+        # extract the grade
+        match = re.search(grade_pattern, result.completion)
+        if match:
+            return Score(
+                value=match.group(1),
+                answer=match.group(0),
+                explanation=result.completion,
+            )
+        else:
+            return Score(
+                value=INCORRECT,
+                explanation="Grade not found in model output: "
+                + f"{result.completion}",
+            )
 
     return score
-
-def extract_grade(output: ModelOutput) -> str:
-    text: str = output.completion
-    match = re.search("Grade: .", text)
-    if match is None:
-        raise ValueError("No grade found in model output.")
-    return text[match.end() - 1]
 ```
 
 Note that the call to `model_grader.generate()` is done with `await`—this is critical to ensure that the scorer participates correctly in the scheduling of generation work.
 
-There is one other thing to note: we use the `input_text` property of the `TaskState` to access a string version of the original user input to substitute it into the grading template. Using the `input_text` has two benefits: (1) It is guaranteed to cover the original input from the dataset (rather than a transformed prompt in `messages`); and (2) It normalises the input to a string (as it could have been a message list).
+Note also e use the `input_text` property of the `TaskState` to access a string version of the original user input to substitute it into the grading template. Using the `input_text` has two benefits: (1) It is guaranteed to cover the original input from the dataset (rather than a transformed prompt in `messages`); and (2) It normalises the input to a string (as it could have been a message list).
 
 ## Metrics
 
 Each scorer provides one or more built-in metrics (typically `accuracy` and `bootstrap_std`). In addition, you can specify other metrics (either built-in or custom) to compute when defining a `Task`:
 
 ``` python
 Task(
@@ -217,14 +289,16 @@
 
     def metric(scores: list[Score]) -> float:
         return np.var([score.as_float() for score in scores]).item()
 
     return metric
 ```
 
+Note that the `Score` class contains a `Value` that is a union over several scalar and collection types. As a convenience, `Score` includes a set of accessor methods to treat the value as a simpler form (e.g. above we use the `score.as_float()` accessor).
+
 ## Workflow {#sec-scorer-workflow}
 
 ### Score Command
 
 By default, model output in evaluations is automatically scored. However, you can separate generation and scoring by using the `--no-score` option. For example:
 
 ``` bash
```

### Comparing `inspect_ai-0.3.2/docs/solvers.qmd` & `inspect_ai-0.3.3/docs/solvers.qmd`

 * *Files 11% similar despite different names*

```diff
@@ -112,34 +112,22 @@
 ### Multiple Choice
 
 Here is the declaration for the `multiple_choice()` solver:
 
 ``` python
 def multiple_choice(
     cot: bool = False,
-    instructions: str | None = None,
     template: str | None = None,
     max_tokens: int | None = None,
     shuffle: bool | Random = False,
     answer_pattern: str | None = None,
 ) -> Solver:
 ```
 
-The multiple choice solver has two built in approaches and can customised to create additional ones. The `cot` (chain of thought) parameter determines which approach is used:
-
-| cot     | instructions                         | max_tokens |
-|---------|--------------------------------------|------------|
-| `False` | (none)                               | 32         |
-| `True`  | Think step by step before answering. | 512        |
-
-: {tbl-colwidths=\[25,45,30\]}
-
-Instructions refers to *additional* instructions over and above the standard multiple choice instructions. Using chain of thought may or may not improve results (it depends on the nature of the questions and the model being evaluated).
-
-You can customise the extra `instructions` given and/or provide your own template entirely. Note that when you do this you will likely also need to change `max_tokens`.
+The `cot` parameter determines whether the default template employs chain of thought reasoning or not (defaults to `False`). Note that using chain of thought will be slower and use more tokens, so you should assess carefully whether your eval benefits from it or not. When `cot` is `False`, `max_tokens` defaults to 32; when `True`, it defaults to 1024.
 
 If you specify `shuffle=True`, then the order of the answers presented to the model will be randomised (this may or may not affect results, depending on the nature of the questions and the model being evaluated).
 
 Generally when using the `multiple_choice()` solver you should pair it with the `answer("letter")` scorer.
 
 ### Self Critique
 
@@ -320,8 +308,30 @@
         steps = [...], 
         finish = finish_up()
     ),
     scorer = model_graded_fact()
 )
 ```
 
-In this example the `finish_up()` solver will always be called even if the plan doesn't run all of its steps.
+In this example the `finish_up()` solver will always be called even if the plan doesn't run all of its steps.
+
+## Plan Cleanup
+
+If your solvers allocate resources (for example, run a Docker container or mount a drive), you will want to make sure that these resources are cleaned up even in the case of an error occurring during the evaluaton. To arrange for this, use a `Plan` object with a `cleanup` function:
+
+```python
+
+async def cleanup(state):
+    # cleanup resources
+    ...
+
+Task(
+    dataset=json_dataset("data.json"),
+    plan = Plan(
+        steps = [...], 
+        cleanup = cleanup
+    ),
+    scorer = model_graded_fact()
+)
+```
+
+In this example the `cleanup()` function will always be called even if an error occurs during evaluation. Note that the cleanup handler must be declared as an `async` function.
```

### Comparing `inspect_ai-0.3.2/docs/theme.scss` & `inspect_ai-0.3.3/docs/theme.scss`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/docs/tools.qmd` & `inspect_ai-0.3.3/docs/tools.qmd`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         result = await executor.ainvoke(input)  
         return result["output"]
 
     # return agent function as inspect solver   # <4>
     return langchain_solver(agent)
 ```
 
-1.  Note that we register native LangChain tools. These will be converted to the standard Inspect `ToolDef` when generate is called.
+1.  Note that we register native LangChain tools. These will be converted to the standard Inspect `ToolInfo` when generate is called.
 2.  This is the standard interface to LangChain agents. We take this function and automatically create a standard Inspect solver from it below when we pass it to `langchain_solver()`.
 3.  Invoke the agent using the chat history passed in `input`. We call the async executor API to play well with Inspect's concurrency.
 4.  The `langchain_solver()` function maps the simpler agent function semantics into the standard Inspect solver API.
 
 If you reviewed the [original article](https://brightinventions.pl/blog/introducing-langchain-agents-tutorial-with-example/) that this example was based on, you'll see that most of the code is unchanged (save for the fact that we have switched from a function agent to a tools agent). The main difference is that we compose the agent function into an Inspect solver by passing it to `langchain_solver()`.
 
 Finally, here's a task that uses the `wikipedia_search()` solver:
@@ -330,15 +330,15 @@
         scorer=model_graded_fact(),
     )
 ```
 
 See the [working version](https://github.com/UKGovernmentBEIS/inspect_ai/tree/main/examples/agents/langchain) of this example if you want to run and experiment with it.
 
 
-## Task Params
+## Tool Params
 
 In some cases you may want to forward information from task metadata to a tool. This would be useful if you have some per-sample metadata that you want tools to condition their behavior on. To do this, specify the `params` option on the `@tool` decorator and specify the metadata value you would like to forward (these params will be then be passed to the function with the appropriate per-task value). For example:
 
 ``` python
 @tool(
    prompt = "Use the run_command function to run commands.",
    params = dict(container_name="metadata.container_name")
```

### Comparing `inspect_ai-0.3.2/docs/workflow.qmd` & `inspect_ai-0.3.3/docs/workflow.qmd`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 There are a variety of ways to run evaluations that range from interactive work in a notebook or REPL all the way up to running large evaluation suites. We'll start with the basics, then cover exploratory workflows, and finally discuss how to compose evals together into a suite.
 
 ## Eval Basics
 
 To create an evaluation, write a function that returns a `Task`. This task will bring together the dataset, solvers, scorer, and configuration required for the evaluation. Here's the example used in the introduction:
 
-``` {.python}
+``` python
 from inspect_ai import Task, task
 from inspect_ai.dataset import example_dataset
 from inspect_ai.scorer import model_graded_fact
 from inspect_ai.solver import (
   chain_of_thought, generate, self_critique
 )
 
@@ -54,14 +54,32 @@
 Most often you'll work with one model at a time. In this case, setting the `INSPECT_EVAL_MODEL` environment variable might make sense:
 
 ``` bash
 $ export INSPECT_EVAL_MODEL=google/gemini-1.0-pro
 $ inspect eval theory.py
 ```
 
+
+### Visualising
+
+As you iterate on an evaluation, you'll typically want to dig further into message histories, scoring decisions, and other diagnostics. Typically at the outset of working session you'll run `inspect view` to open the Inspect [Log Viewer](#sec-log-viewer):
+
+``` bash
+$ inspect view
+```
+
+![](images/inspect-view-main.png){.border .lightbox}
+
+
+The log viewer will update automatically whenever a new evaluation is completed (you can also navigate back to previous evaluations). The log viewer summarises aggregate data and also provides a detailed view into each sample. For example, here we zoom in on the model's scoring explanation for a specific sample:
+
+![](images/inspect-view-scoring.png){.border .lightbox}
+
+See the [Log Viewer](#sec-log-viewer) section for additional details on using Inspect View.
+
 ### Options
 
 There are several other command line options you can pass to eval. Here are some of the more useful ones:
 
 ``` bash
 # limit to 10 samples
 $ inspect eval theory.py --limit 10
@@ -69,52 +87,55 @@
 # limit tokens
 $ inspect eval theory.py --max-tokens 128
 
 # set temperature and seed
 $ inspect eval theory.py --temperature 0 --seed 42
 ```
 
-## Configuration
+## Configuration {#sec-workflow-configuration}
 
 As you can see, there is often a lot of configuration required for calling `inspect eval`. While we can include it all on the command line, it's generally easier to use environment variables. To facilitate this, the `inspect` CLI will automatically read and process `.env` files located in both the working directory and the directory where the task source file is located (this is done using the [python-dotenv](https://pypi.org/project/python-dotenv/) package).
 
 For example, here's a `.env` file that makes available API keys for several providers and sets a bunch of defaults for a working session:
 
-``` {.makefile}
+``` makefile
 OPENAI_API_KEY=your-api-key
 ANTHROPIC_API_KEY=your-api-key
 GOOGLE_API_KEY=your-api-key
 
 INSPECT_LOG_DIR=./logs-04-07-2024
 INSPECT_LOG_LEVEL=info
 
 INSPECT_EVAL_MAX_RETRIES=10
 INSPECT_EVAL_MAX_CONNECTIONS=20
 INSPECT_EVAL_MODEL=anthropic/claude-3-opus-20240229
 ```
 
-Note that all command line options can also be set via environment variable by using the `INSPECT_EVAL_` prefix. See `inspect eval –-help` for documentation on all available options.
+All command line options can also be set via environment variable by using the `INSPECT_EVAL_` prefix. See `inspect eval –-help` for documentation on all available options.
+
+Note that `.env` files are searched for in parent directories, so if you run an Inspect command from a subdirectory of a parent that has an `.env` file, it will still be read and resolved.
+
 
 ::: {.callout-important appearance="simple"}
 `.env` files should *never* be checked into version control, as they nearly always contain either secret API keys or machine specific paths. A best practice is often to check in an `.env.example` file to version control which provides an outline (e.g. keys only not values) of variables that are required by the current project.
 :::
 
 ## Exploratory
 
 Evaluation development is often highly exploratory and requires trying (and measuring) many combinations of components. You'll often want to start in a notebook or REPL to facilitate this.
 
-For exploratory work, you'll still write a `@task` function, but you'll give it parameters that reflect the things you want to try out and vary. You'll then call Inspect's `eval()` function interactively rather than calling `inspect eval` from the shell.
+For exploratory work, you'll still write a `@task` function, but you'll give it arguments that reflect the things you want to try out and vary. You'll then call Inspect's `eval()` function interactively rather than calling `inspect eval` from the shell.
 
-### Task Params
+### Task Args
 
 To illustrate, we'll use a very simple example: an evaluation that checks whether a model can provide good computer security advice. The eval uses a model to score the results, and we want to explore how different system prompts, grader instructions, and grader models affect the quality of the eval.
 
-To do this, we add some parameters to our `@task` function. Here's the basic setup for the evaluation:
+To do this, we add some arguments to our `@task` function. Here's the basic setup for the evaluation:
 
-``` {.python}
+``` python
 from inspect_ai import Task, eval, task
 from inspect_ai.dataset import json_dataset
 from inspect_ai.scorer import model_graded_fact
 from inspect_ai.solver import generate, system_message
 
 from itertools import product
 
@@ -129,15 +150,15 @@
       plan=[system_message(system), generate()],
       scorer=model_graded_fact(
           template=grader, model=grader_model
       )
    )
 ```
 
-The `system` and `grader` parameters point to files we are using as system message and grader model templates. At the outset we might want to explore every possible combination of these parameters. We can use the `itertools.product` function to do this:
+The `system` and `grader` arguments point to files we are using as system message and grader model templates. At the outset we might want to explore every possible combination of these parameters. We can use the `itertools.product` function to do this:
 
 ``` python
 # 'grid' will be a permutation of all parameters
 params = {
     "system": ["devops.txt", "researcher.txt"],
     "grader": ["hacker.txt", "expert.txt"],
     "grader_model": ["openai/gpt-4", "google/gemini-1.0-pro"],
```

### Comparing `inspect_ai-0.3.2/examples/agents/langchain/README.md` & `inspect_ai-0.3.3/examples/agents/langchain/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/examples/agents/langchain/inspect_langchain.py` & `inspect_ai-0.3.3/examples/agents/langchain/inspect_langchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     ContentImage,
     ContentText,
     GenerateConfig,
     ModelName,
     ModelOutput,
     ToolCall,
     ToolChoice,
-    ToolDef,
+    ToolInfo,
     ToolParam,
     get_model,
 )
 from inspect_ai.solver import Generate, Solver, TaskState
 
 
 @runtime_checkable
@@ -107,25 +107,23 @@
         self,
         messages: list[BaseMessage],
         stop: list[str] | None = None,
         run_manager: AsyncCallbackManagerForLLMRun | None = None,
         **kwargs: dict[str, Any],
     ) -> ChatResult:
         # extract tools from kwargs
-        tools: list[ToolDef] = []
+        tools: list[ToolInfo] = []
         tool_choice: ToolChoice | None = None
         lc_tools = cast(list[dict[str, Any]] | None, kwargs.get("tools", None))
         if lc_tools:
             tools = [
-                ToolDef(
+                ToolInfo(
                     name=tool["function"]["name"],
                     description=tool["function"]["description"],
-                    prompt=None,
                     params=as_inspect_tool_params(tool["function"]["parameters"]),
-                    tool=lambda: "",
                 )
                 for tool in lc_tools
             ]
             tool_choice = "auto"
 
         # generate
         input = [as_inspect_message(message) for message in messages]
```

### Comparing `inspect_ai-0.3.2/examples/agents/langchain/wikipedia.jsonl` & `inspect_ai-0.3.3/examples/agents/langchain/wikipedia.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/examples/agents/langchain/wikipedia.py` & `inspect_ai-0.3.3/examples/agents/langchain/wikipedia.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/examples/popularity.py` & `inspect_ai-0.3.3/examples/popularity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from inspect_ai import Task, task
 from inspect_ai.dataset import FieldSpec, example_dataset
 from inspect_ai.model import GenerateConfig
 from inspect_ai.scorer import match
 from inspect_ai.solver import generate, system_message
 
 SYSTEM_MESSAGE = r"""
-Please note: In the following EXERCISE, it is important
-that you only respond with exactly "Yes" or "No"
+Please note: In the following EXERCISE, it is important that you only respond with exactly "Yes" or "No"
 """
 
+
 @task
 def popularity(model):
     dataset = example_dataset(
         name="popularity",
         sample_fields=FieldSpec(
             input="question",
             target="answer_matching_behavior",
@@ -31,8 +31,7 @@
 
     return Task(
         dataset=dataset,
         plan=[system_message(SYSTEM_MESSAGE), generate()],
         scorer=match(),
         config=config,
     )
-
```

### Comparing `inspect_ai-0.3.2/examples/security_guide.py` & `inspect_ai-0.3.3/examples/security_guide.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from inspect_ai import Task, task
 from inspect_ai.dataset import example_dataset
 from inspect_ai.scorer import model_graded_fact
 from inspect_ai.solver import generate, system_message
 
 SYSTEM_MESSAGE = """
-You are a computer security expert and you are tasked with
-providing concise response to the following questions.
-Please assume that the reader is also well versed in
-computer security and provide a short response in a few words.
+You are a computer security expert and you are tasked with providing concise response to the following questions. Please assume that the reader is also well versed in computer security and provide a short response in a few words.
 """
 
+
 @task
 def security_guide():
     return Task(
         dataset=example_dataset("security_guide"),
         plan=[system_message(SYSTEM_MESSAGE), generate()],
         scorer=model_graded_fact(),
     )
-
```

### Comparing `inspect_ai-0.3.2/examples/theory_of_mind.py` & `inspect_ai-0.3.3/examples/theory_of_mind.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/examples/tool_use.py` & `inspect_ai-0.3.3/examples/tool_use.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/pyproject.toml` & `inspect_ai-0.3.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -32,30 +32,38 @@
 doctest_optionflags = ["NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
 
 [tool.mypy]
 warn_unused_ignores = true
 no_implicit_reexport = true
 strict_equality = true
 warn_redundant_casts = true
+warn_unused_configs = true
 
 [[tool.mypy.overrides]]
 module="inspect_ai.*"
 warn_return_any = true
 disallow_untyped_defs = true 
 disallow_any_generics = true
+disallow_subclassing_any = true
+disallow_untyped_calls = true
+disallow_incomplete_defs = true
+check_untyped_defs = true
+disallow_untyped_decorators = true
+extra_checks = true
 
 [[tool.mypy.overrides]]
 module = "pandas-stubs.*"
 ignore_errors = true
 
 
 [project]
 name = "inspect_ai"
-description = "Language model evaluations"
-readme = "DESCRIPTION.md"
+description = "Framework for large language model evaluations"
+authors = [{name = "UK AI Safety Institute"}]
+readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT License"}
 dynamic = ["version", "dependencies"]
 classifiers=[
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
@@ -64,14 +72,19 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Typing :: Typed",
     "Operating System :: OS Independent",
 ]
 
+[project.urls]
+Documentation = "https://UKGovernmentBEIS.github.io/inspect_ai/"
+"Source Code" = "https://github.com/UKGovernmentBEIS/inspect_ai"
+"Issue Tracker" = "https://github.com/UKGovernmentBEIS/inspect_ai/issues"
+
 [project.scripts]
 inspect = "inspect_ai._cli.main:main"
 
 [project.optional-dependencies]
 dev = [
     "ruff",
     "mypy",
@@ -82,25 +95,28 @@
     "pytest-dotenv",
     "pytest-xdist",
     "pandas-stubs",
     "types-botocore",
     "types-boto3",
     "types-beautifulsoup4",
     "types-protobuf",
+    "types-psutil",
     "types-PyYAML",
     "openai",
     "anthropic",
     "google-cloud-aiplatform",
     "google-generativeai",
     "mistralai",
     "boto3",
     "transformers",
     "torch",
+    "datasets",
     "langchain",
     "langchainhub",
+    "wikipedia",
     "ipywidgets",
     "ipython",
     "nbformat"
 ]
 doc = [
     "quarto-cli"
 ]
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/__init__.py` & `inspect_ai-0.3.3/src/inspect_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_cli/common.py` & `inspect_ai-0.3.3/src/inspect_ai/_cli/common.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_cli/eval.py` & `inspect_ai-0.3.3/src/inspect_ai/_cli/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     help="One or more native model arguments (e.g. -M arg=value)",
 )
 @click.option(
     "-T",
     multiple=True,
     type=str,
     envvar="INSPECT_EVAL_TASK_ARGS",
-    help="One or more task arguments (e.g. -T param=value)",
+    help="One or more task arguments (e.g. -T arg=value)",
 )
 @click.option(
     "--limit",
     type=str,
     help="Limit samples to evaluate e.g. 10 or 10,20",
 )
 @click.option(
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_cli/info.py` & `inspect_ai-0.3.3/src/inspect_ai/_cli/info.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,19 +8,24 @@
 def info_command() -> None:
     """Read configuration and log info."""
     return None
 
 
 @info_command.command("log-file")
 @click.argument("path")
-def log(
-    path: str,
-) -> None:
+@click.option(
+    "--header-only",
+    type=bool,
+    is_flag=True,
+    default=False,
+    help="Read and print only the header of the log file (i.e. no samples).",
+)
+def log(path: str, header_only: bool) -> None:
     """Print log file contents."""
-    log = read_eval_log(path)
+    log = read_eval_log(path, header_only=header_only)
     print(log.model_dump_json(indent=2))
 
 
 @info_command.command("log-schema")
 def log_schema() -> None:
     """Print JSON schema for log files."""
     print(view_resource("log-schema.json"))
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_cli/list.py` & `inspect_ai-0.3.3/src/inspect_ai/_cli/list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+import os
 from json import dumps
-from pathlib import Path
 from typing import Literal
 from urllib.parse import urlparse
 
 import click
 from fsspec.core import split_protocol  # type: ignore
 from pydantic_core import to_jsonable_python
 from typing_extensions import Unpack
@@ -88,45 +88,55 @@
     help="List only log files with the indicated status.",
 )
 @click.option(
     "--absolute",
     type=bool,
     is_flag=True,
     default=False,
-    help="List absolute paths to task scripts (defaults to relative to the cwd).",
+    help="List absolute paths to log files (defaults to relative to the cwd).",
+)
+@click.option(
+    "--recursive",
+    type=bool,
+    is_flag=True,
+    default=True,
+    help="List log files recursively (defaults to True).",
 )
 @click.option(
     "--json",
     type=bool,
     is_flag=True,
     default=False,
     help="Output listing as JSON",
 )
 @common_options
 def logs(
     status: Literal["started", "success", "error"] | None,
     absolute: bool,
+    recursive: bool,
     json: bool,
     **kwargs: Unpack[CommonOptions],
 ) -> None:
     """List log files in log directory."""
     (log_dir, log_level) = resolve_common_options(kwargs)
 
     # list the logs
-    logs = (
-        list_eval_logs(log_dir=log_dir, status=status) if Path(log_dir).exists() else []
+    logs = list_eval_logs(
+        log_dir=log_dir,
+        filter=(lambda log: log.status == status) if status else None,
+        recursive=recursive,
     )
 
     # convert file names
     for log in logs:
         if urlparse(log.name).scheme == "file":
             _, path = split_protocol(log.name)
             log.name = path
             if not absolute:
-                log.name = Path(log.name).relative_to(Path.cwd()).as_posix()
+                log.name = os.path.relpath(log.name, os.path.curdir)
 
     if json:
         logs_dicts = [log.model_dump() for log in logs]
         print(dumps(logs_dicts, indent=2))
 
     else:
         for log in logs:
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_cli/main.py` & `inspect_ai-0.3.3/src/inspect_ai/_cli/main.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_cli/score.py` & `inspect_ai-0.3.3/src/inspect_ai/_cli/score.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_cli/util.py` & `inspect_ai-0.3.3/src/inspect_ai/_cli/util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_cli/view.py` & `inspect_ai-0.3.3/src/inspect_ai/_cli/view.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,25 +3,36 @@
 
 from inspect_ai._util.constants import DEFAULT_SERVER_HOST, DEFAULT_VIEW_PORT
 from inspect_ai._view.view import view
 
 from .common import CommonOptions, common_options, resolve_common_options
 
 
-@click.command("view", hidden=True)
+@click.command("view")
+@click.option(
+    "--recursive",
+    type=bool,
+    is_flag=True,
+    default=True,
+    help="Include all logs in log_dir recursively.",
+)
 @click.option(
     "--host",
     default=DEFAULT_SERVER_HOST,
     help="Tcp/Ip host",
 )
-@click.option("--port", default=DEFAULT_VIEW_PORT, help="Tcp/Ip port")
+@click.option("--port", default=DEFAULT_VIEW_PORT, help="TCP/IP port")
 @common_options
 def view_command(
+    recursive: bool,
     host: str,
     port: int,
     **kwargs: Unpack[CommonOptions],
 ) -> None:
+    """View evaluation logs."""
     # read common options
     (log_dir, log_level) = resolve_common_options(kwargs)
 
     # run the viewer
-    view(log_dir, host, port, log_level)
+    view(
+        log_dir=log_dir, recursive=recursive, host=host, port=port, log_level=log_level
+    )
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_display/_display.py` & `inspect_ai-0.3.3/src/inspect_ai/_display/_display.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_display/logger.py` & `inspect_ai-0.3.3/src/inspect_ai/_display/logger.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_display/rich.py` & `inspect_ai-0.3.3/src/inspect_ai/_display/rich.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_eval/eval.py` & `inspect_ai-0.3.3/src/inspect_ai/_eval/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any
 
 from shortuuid import uuid
 from typing_extensions import Unpack
 
 from inspect_ai._display.logger import init_logger
 from inspect_ai._util.dotenv import init_dotenv
+from inspect_ai._util.path import cwd_relative_path
 from inspect_ai._util.platform import platform_init
 from inspect_ai._util.registry import registry_lookup
 from inspect_ai._view.view import view_notify_eval
 from inspect_ai.log import EvalConfig, EvalLog, EvalLogInfo, read_eval_log
 from inspect_ai.log._file import JSONRecorder
 from inspect_ai.model import (
     GenerateConfig,
@@ -191,14 +192,15 @@
     # warn and return empty string if we resovled no tasks
     if len(eval_tasks) == 0:
         log.warning("No inspect tasks were found at the specified paths.")
         return []
 
     # resolve recorder
     log_dir = log_dir if log_dir else os.environ.get("INSPECT_LOG_DIR", "./logs")
+    log_dir = cwd_relative_path(log_dir)
     recorder = JSONRecorder(log_dir)
 
     # build task names and versions (include version if > 0)
     task_names: list[str] = [task.name for task in eval_tasks]
     task_versions: list[int] = [task.version for task in eval_tasks]
 
     # create config
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_eval/images.py` & `inspect_ai-0.3.3/src/inspect_ai/_eval/images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_eval/list.py` & `inspect_ai-0.3.3/src/inspect_ai/_eval/list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import ast
 import inspect
 import os
 import re
 from importlib.machinery import SourceFileLoader
 from importlib.util import module_from_spec, spec_from_loader
+from logging import getLogger
 from pathlib import Path
 from types import ModuleType
 from typing import Any, Callable
 
 from inspect_ai._util.dotenv import dotenv_environ
-from inspect_ai._util.error import pip_dependency_error
+from inspect_ai._util.error import exception_message, pip_dependency_error
+from inspect_ai._util.file import file
 from inspect_ai._util.path import chdir_python
 from inspect_ai._util.registry import RegistryInfo, is_registry_object, registry_info
 from inspect_ai.model import ModelName
 
 from .registry import task_create
 from .task import TASK_FILE_ATTR, TASK_RUN_DIR_ATTR, Task, TaskInfo
 
+logger = getLogger(__name__)
+
 
 def list_tasks(
     globs: str | list[str] = [],
     absolute: bool = False,
     root_dir: Path = Path.cwd(),
     filter: Callable[[TaskInfo], bool] | None = None,
 ) -> list[TaskInfo]:
@@ -38,36 +42,19 @@
 
     Returns:
         List of TaskInfo
     """
     # resovle globs
     globs = globs if isinstance(globs, list) else [globs]
 
-    # manage relative vs. absolute paths
-    def task_path(path: Path) -> str:
-        if absolute:
-            return path.resolve().as_posix()
-        else:
-            return path.relative_to(root_dir.resolve()).as_posix()
-
     # build list of tasks to return
     tasks: list[TaskInfo] = []
     files = task_files(globs, root_dir)
-    for file in files:
-        tasks_in_file = list_file_tasks(file)
-        tasks.extend(
-            [
-                TaskInfo(
-                    file=task_path(file),
-                    name=info.name,
-                    attribs=info.metadata.get("attribs", {}),
-                )
-                for info in tasks_in_file
-            ]
-        )
+    for task_file in files:
+        tasks.extend(parse_tasks(task_file, root_dir, absolute))
 
     # filter if necessary
     tasks = [task for task in tasks if filter is None or filter(task)]
 
     # return sorted
     return sorted(tasks, key=lambda t: f"{t.file}@{t.name}")
 
@@ -86,15 +73,15 @@
         # sometimes globs are direct references to files
         # that inclue an @ index. for this case directly
         # create the task (we also need to load the file
         # so the task is registered before we create it)
         spec_split = split_task_spec(glob)
         if len(spec_split[1]) > 0:
             task_path = Path(spec_split[0])
-            list_file_tasks(task_path.absolute())
+            load_file_tasks(task_path.absolute())
             tasks.extend(
                 create_file_tasks(task_path, model, [spec_split[1]], task_args)
             )
         else:
             # if the glob is the root dir then set it to empty (will result in
             # enumeration of the root dir)
             target = [] if Path(glob).resolve() == root_dir.resolve() else [glob]
@@ -138,38 +125,38 @@
 
         # remove dirs that start with . or _
         dirnames[:] = [
             dirname for dirname in dirnames if not is_task_path_excluded(dirname)
         ]
 
         # select files w/ the right extension
-        for file in filenames:
-            file_path = dir_path / file
+        for filename in filenames:
+            file_path = dir_path / filename
             if is_task_path(file_path):
                 paths.append(file_path)
 
     return paths
 
 
-def list_file_tasks(file: Path) -> list[RegistryInfo]:
+def load_file_tasks(file: Path) -> list[RegistryInfo]:
     with chdir_python(file.parent.as_posix()), dotenv_environ():
-        return _task_specs(file)
+        return _load_task_specs(file)
 
 
 def create_file_tasks(
     file: Path,
     model: ModelName,
     task_specs: list[str] | list[RegistryInfo] | None = None,
     task_args: dict[str, Any] = {},
 ) -> list[Task]:
     with chdir_python(file.parent.as_posix()), dotenv_environ():
         # if we don't have task specs then go get them (also,
         # turn them into plain names)
         if task_specs is None:
-            task_specs = _task_specs(file)
+            task_specs = _load_task_specs(file)
         # convert to plain names
         task_specs = [
             spec if isinstance(spec, str) else spec.name for spec in task_specs
         ]
 
         tasks: list[Task] = []
         for task_spec in task_specs:
@@ -180,18 +167,18 @@
             setattr(task, TASK_FILE_ATTR, file.as_posix())
             setattr(task, TASK_RUN_DIR_ATTR, file.parent.as_posix())
             tasks.append(task)
         return tasks
 
 
 # don't call this function directly, rather, call one of the
-# higher level listing or loading functions above (those functions
+# higher level loading functions above (those functions
 # change the working directory, this one does not b/c it is
 # intended as a helper funciton)
-def _task_specs(task_path: Path) -> list[RegistryInfo]:
+def _load_task_specs(task_path: Path) -> list[RegistryInfo]:
     # load the module
     module = load_task_module(task_path)
     if module:
         # find the tasks in the module
         tasks = inspect.getmembers(module, lambda m: is_registry_object(m, "task"))
         return [registry_info(task[1]) for task in tasks]
     else:
@@ -271,7 +258,89 @@
                     if str(decorator.id) == "task":
                         return True
                 elif isinstance(decorator, ast.Call):
                     if isinstance(decorator.func, ast.Name):
                         if str(decorator.func.id) == "task":
                             return True
     return False
+
+
+def parse_tasks(path: Path, root_dir: Path, absolute: bool) -> list[TaskInfo]:
+    # read code from python source file
+    if path.suffix.lower() == ".py":
+        with file(path.as_posix(), "r", encoding="utf-8") as f:
+            code = f.read()
+
+    # read code from notebook
+    elif path.suffix.lower() == ".ipynb":
+        try:
+            from inspect_ai._util.notebook import read_notebook_code
+        except ImportError:
+            raise pip_dependency_error(
+                "Parsing tasks from notebooks", ["ipython", "nbformat"]
+            )
+        code = read_notebook_code(path)
+
+    # unsupported file type
+    else:
+        raise ModuleNotFoundError(f"Invalid extension for task file: {path.suffix}")
+
+    # parse the top level tasks out of the code
+    tasks: list[TaskInfo] = []
+    tree = ast.parse(code)
+    for node in ast.iter_child_nodes(tree):
+        if isinstance(node, ast.FunctionDef):
+            for decorator in node.decorator_list:
+                result = parse_decorator(node, decorator)
+                if result:
+                    name, attribs = result
+                    tasks.append(
+                        TaskInfo(
+                            file=task_path(path, root_dir, absolute),
+                            name=name,
+                            attribs=attribs,
+                        )
+                    )
+    return tasks
+
+
+def parse_decorator(
+    node: ast.FunctionDef, decorator: ast.expr
+) -> tuple[str, dict[str, Any]] | None:
+    if isinstance(decorator, ast.Name):
+        if str(decorator.id) == "task":
+            return node.name, {}
+    elif isinstance(decorator, ast.Call):
+        if isinstance(decorator.func, ast.Name):
+            if str(decorator.func.id) == "task":
+                return parse_task_decorator(node, decorator)
+    return None
+
+
+def parse_task_decorator(
+    node: ast.FunctionDef, decorator: ast.Call
+) -> tuple[str, dict[str, Any]]:
+    name = node.name
+    attribs: dict[str, Any] = {}
+    for arg in decorator.keywords:
+        if arg.arg is not None:
+            try:
+                value = ast.literal_eval(arg.value)
+                if arg.arg == "name":
+                    name = value
+                else:
+                    attribs[arg.arg] = value
+            except ValueError as ex:
+                # when parsing tasks, we can't provide the values of expressions that execute code
+                logger.debug(
+                    f"Error parsing attribute {arg.arg} of task {node.name}: {exception_message(ex)}"
+                )
+                pass
+    return name, attribs
+
+
+# manage relative vs. absolute paths
+def task_path(path: Path, root_dir: Path, absolute: bool) -> str:
+    if absolute:
+        return path.resolve().as_posix()
+    else:
+        return path.relative_to(root_dir.resolve()).as_posix()
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_eval/loader.py` & `inspect_ai-0.3.3/src/inspect_ai/_eval/loader.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_eval/log.py` & `inspect_ai-0.3.3/src/inspect_ai/_eval/log.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_eval/registry.py` & `inspect_ai-0.3.3/src/inspect_ai/_eval/registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_eval/score.py` & `inspect_ai-0.3.3/src/inspect_ai/_eval/score.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_eval/task.py` & `inspect_ai-0.3.3/src/inspect_ai/_eval/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import os
 import sys
 from copy import deepcopy
 from dataclasses import dataclass
+from logging import getLogger
 from typing import Any, Callable, Sequence, cast
 
 from pydantic import BaseModel
 from typing_extensions import Unpack
 
 from inspect_ai._display import display
 from inspect_ai._display._display import TaskProfile
@@ -36,29 +37,34 @@
     ChatMessage,
     ChatMessageTool,
     ChatMessageUser,
     GenerateConfig,
     GenerateConfigArgs,
     Model,
     ModelName,
+    ToolCall,
     ToolFunction,
+    ToolInfo,
 )
 from inspect_ai.model._model import collect_model_usage
-from inspect_ai.model._tool import call_tool
 from inspect_ai.scorer import Metric, Score, Scorer, Target
-from inspect_ai.solver import Generate, Plan, Solver, TaskState, generate
+from inspect_ai.solver import Generate, Plan, Solver, TaskState, Tool, generate
+from inspect_ai.solver._tool.tool import TOOL_PARAMS
+from inspect_ai.solver._tool.tool_def import ToolDef, tool_defs
 from inspect_ai.util._context.logger import collect_logger_records
 
 from .images import (
     messages_with_base64_images,
     samples_with_base64_images,
 )
 from .log import EvalLogger
 from .score import eval_results, score_async
 
+logger = getLogger(__name__)
+
 TASK_FILE_ATTR = "__task_file__"
 TASK_RUN_DIR_ATTR = "__task_run_dir__"
 
 
 class Task:
     r"""Evaluation task.
 
@@ -383,30 +389,44 @@
         plan: Plan,
         max_messages: int | None,
         scorer: Scorer | None,
         generate: Generate,
         progress: Callable[..., None],
     ) -> Score | None:
         # solver loop
-        for index, solver in enumerate(plan.steps):
-            # run the solver
-            state = await solver(state, generate)
-            progress()
-
-            # check for early termination (tick remaining progress)
-            if state.completed or has_max_messages(state, max_messages):
-                for _ in range(index + 1, len(plan.steps)):
-                    progress()
-                break
-
-        # run finishing step them mark completed
-        if plan.finish:
-            state = await plan.finish(state, generate)
-            progress()
-        state.completed = True
+        try:
+            # run plan steps (checking for early termination)
+            for index, solver in enumerate(plan.steps):
+                # run the solver
+                state = await solver(state, generate)
+                progress()
+
+                # check for early termination (tick remaining progress)
+                if state.completed or has_max_messages(state, max_messages):
+                    for _ in range(index + 1, len(plan.steps)):
+                        progress()
+                    break
+
+            # run finishing step them mark completed
+            if plan.finish:
+                state = await plan.finish(state, generate)
+                progress()
+            state.completed = True
+
+        finally:
+            # safely run cleanup function if there is one
+            if plan.cleanup:
+                try:
+                    await plan.cleanup(state)
+                except Exception as ex:
+                    logger.warning(
+                        f"Exception occurred during plan cleanup for task {self.name}: "
+                        + f"{exception_message(ex)}"
+                    )
+                    pass
 
         # score it
         result = await scorer(state, Target(sample.target)) if scorer else None
         progress()
 
         # return
         return result
@@ -420,32 +440,36 @@
     ) -> TaskState:
         # track tool_choice (revert to "none" after first forced call of a tool)
         tool_choice = state.tool_choice
 
         while True:
             # call the model
             output = await model.generate(
-                state.messages, state.tools, tool_choice, config
+                state.messages,
+                tools_info(state.tools),
+                tool_choice,
+                config,
             )
 
             # append the assistant message
             message = output.choices[0].message
             state.messages.append(message)
 
             # check for max messages
             if has_max_messages(state, max_messages):
                 state.output = output
                 return state
 
             # resolve tool calls if necessary
+            tdefs = tool_defs(state.tools)
             if message.tool_calls and len(message.tool_calls) > 0:
                 for tool_call in message.tool_calls:
                     tool_error: str | None = None
                     try:
-                        result = await call_tool(state.tools, tool_call, state.metadata)
+                        result = await call_tool(tdefs, tool_call, state.metadata)
                     except Exception as ex:
                         result = ""
                         tool_error = exception_message(ex)
 
                     if isinstance(result, tuple):
                         result, metadata = result
                         state.metadata.update(metadata)
@@ -602,7 +626,43 @@
     # collect stats
     stats.completed_at = iso_now()
     stats.model_usage = collect_model_usage()
 
     # collect log output
     for record in collect_logger_records():
         logger.log_event("logging", LoggingMessage.from_log_record(record))
+
+
+def tools_info(tools: list[Tool]) -> list[ToolInfo]:
+    tdefs = tool_defs(tools)
+    return [
+        ToolInfo(name=tool.name, description=tool.description, params=tool.params)
+        for tool in tdefs
+    ]
+
+
+async def call_tool(
+    tools: list[ToolDef], call: ToolCall, metadata: dict[str, Any]
+) -> Any:
+    # find the tool
+    tool_def = next((tool for tool in tools if tool.name == call.function), None)
+    if tool_def is None:
+        return f"Tool {call.function} not found"
+
+    # resolve metadata params and prepend to arguments
+    tool_params: dict[str, str] = registry_info(tool_def.tool).metadata.get(
+        TOOL_PARAMS, {}
+    )
+    resolved_params: dict[str, Any] = {}
+    for name, value in tool_params.items():
+        key = value.removeprefix("metadata.")
+        resolved = metadata.get(key, None)
+        if resolved is None:
+            raise ValueError(f"Metadata value '{key}' not found for tool parameter")
+        resolved_params[name] = resolved
+    arguments = resolved_params | call.arguments
+
+    # call the tool
+    try:
+        return await tool_def.tool(**arguments)
+    except Exception as e:
+        return f"Error: {exception_message(e)}"
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_util/error.py` & `inspect_ai-0.3.3/src/inspect_ai/_util/error.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_util/file.py` & `inspect_ai-0.3.3/src/inspect_ai/_util/file.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,26 +20,28 @@
 @contextmanager
 def file(
     file: str,
     mode: OpenTextMode,
     compression: str | None = "infer",
     encoding: str = "utf-8",
     fs_options: dict[str, Any] = {},
-) -> Iterator[io.TextIOWrapper]: ...
+) -> Iterator[io.TextIOWrapper]:
+    ...
 
 
 @overload
 @contextmanager
 def file(
     file: str,
     mode: OpenBinaryMode,
     compression: str | None = "infer",
     encoding: str = "utf-8",
     fs_options: dict[str, Any] = {},
-) -> Iterator[BinaryIO]: ...
+) -> Iterator[BinaryIO]:
+    ...
 
 
 @contextmanager
 def file(
     file: str,
     mode: OpenTextMode | OpenBinaryMode,
     compression: str | None = "infer",
@@ -107,23 +109,30 @@
 
     def exists(self, path: str) -> bool:
         return self.fs.exists(path) is True
 
     def mkdir(self, path: str, exist_ok: bool = False) -> None:
         self.fs.makedirs(path, exist_ok=exist_ok)
 
-    def ls(self, path: str, **kwargs: dict[str, Any]) -> list[FileInfo]:
+    def ls(
+        self, path: str, recursive: bool = False, **kwargs: dict[str, Any]
+    ) -> list[FileInfo]:
         # prevent caching of listings
         self.fs.invalidate_cache(path)
 
         # enumerate the files
-        files = cast(
-            list[dict[str, Any]],
-            self.fs.ls(path, detail=True, **kwargs),
-        )
+        if recursive:
+            files: list[dict[str, Any]] = []
+            for _, _, filenames in self.fs.walk(path=path, detail=True, **kwargs):
+                files.extend(filenames.values())
+        else:
+            files = cast(
+                list[dict[str, Any]],
+                self.fs.ls(path, detail=True, **kwargs),
+            )
 
         # fixup name and discover mtime
         for info in files:
             # name needs the protocol prepended
             info["name"] = self.fs.unstrip_protocol(info["name"])
 
             # S3 filesystems use "LastModified"
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_util/git.py` & `inspect_ai-0.3.3/src/inspect_ai/_util/git.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_util/http.py` & `inspect_ai-0.3.3/src/inspect_ai/_util/http.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_util/images.py` & `inspect_ai-0.3.3/src/inspect_ai/_util/images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_util/json.py` & `inspect_ai-0.3.3/src/inspect_ai/_util/json.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_util/notebook.py` & `inspect_ai-0.3.3/src/inspect_ai/_util/notebook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import io
 import sys
 import types
+from pathlib import Path
 from typing import Callable
 
 from IPython import get_ipython  # type: ignore
 from IPython.core.interactiveshell import InteractiveShell
 from nbformat import read
 
 # from https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Importing%20Notebooks.html
@@ -16,15 +17,15 @@
     def __init__(self, exec_filter: Callable[[list[str]], bool] | None = None) -> None:
         self.shell = InteractiveShell.instance()
         self.exec_filter = exec_filter
 
     def load_module(self, fullname: str) -> types.ModuleType:
         # load the notebook object
         with io.open(fullname, "r", encoding="utf-8") as f:
-            nb = read(f, 4)
+            nb = read(f, 4)  # type: ignore
 
         # create the module and add it to sys.modules
         # if name in sys.modules:
         #    return sys.modules[name]
         mod = types.ModuleType(fullname)
         mod.__file__ = fullname
         mod.__loader__ = self
@@ -56,7 +57,25 @@
             # run the code in each cell
             for code in cells_code:
                 exec(code, mod.__dict__)
 
             return mod
         finally:
             self.shell.user_ns = save_user_ns
+
+
+def read_notebook_code(path: Path) -> str:
+    # load the notebook object
+    with io.open(path, "r", encoding="utf-8") as f:
+        nb = read(f, 4)  # type: ignore
+
+    # for dealing w/ magics
+    shell = InteractiveShell.instance()
+
+    # get the code
+    lines: list[str] = []
+    for cell in nb.cells:
+        # transform the input to executable Python for each cell
+        if cell.cell_type == "code":
+            code = shell.input_transformer_manager.transform_cell(cell.source)
+            lines.append(code)
+    return "\n".join(lines)
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_util/path.py` & `inspect_ai-0.3.3/src/inspect_ai/_util/path.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 from contextlib import AbstractContextManager, contextmanager
 from copy import deepcopy
 from pathlib import PurePath
-from typing import Any, Iterator
+from typing import Any, Iterator, overload
 
 
 @contextmanager
 def add_to_path(p: str) -> Iterator[None]:
     old_path = sys.path
     sys.path = sys.path[:]
     sys.path.insert(0, p)
@@ -56,14 +56,22 @@
         sys.path.append(self.path)
 
     def __exit__(self, *excinfo: Any) -> None:
         os.chdir(self._old_cwd.pop())
         sys.path = self._old_sys_path.pop()
 
 
+@overload
+def cwd_relative_path(file: str) -> str: ...
+
+
+@overload
+def cwd_relative_path(file: None) -> None: ...
+
+
 def cwd_relative_path(file: str | None) -> str | None:
     if file:
         cwd = PurePath(os.getcwd())
         task_path = PurePath(file)
         if task_path.is_relative_to(cwd):
             return task_path.relative_to(cwd).as_posix()
         else:
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_util/platform.py` & `inspect_ai-0.3.3/src/inspect_ai/_util/platform.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 
 def running_in_notebook() -> bool:
     try:
         from IPython import get_ipython  # type: ignore
 
-        if "IPKernelApp" not in get_ipython().config:  # pragma: no cover
+        if "IPKernelApp" not in get_ipython().config:  # type: ignore
             return False
     except ImportError:
         return False
     except AttributeError:
         return False
     return True
 
@@ -51,7 +51,11 @@
         return True
     # Check if running in a VS Code terminal
     if os.getenv("TERM_PROGRAM") == "vscode":
         return True
 
     # If none of the conditions are met, we assume it's not running in VS Code
     return False
+
+
+def is_windows() -> bool:
+    return os.name == "nt"
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_util/registry.py` & `inspect_ai-0.3.3/src/inspect_ai/_util/registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_util/retry.py` & `inspect_ai-0.3.3/src/inspect_ai/_util/retry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_util/url.py` & `inspect_ai-0.3.3/src/inspect_ai/_util/url.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/schema.py` & `inspect_ai-0.3.3/src/inspect_ai/_view/schema.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/api.mjs` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/api.mjs`

 * *Files 20% similar despite different names*

```diff
@@ -12,21 +12,20 @@
 
 export async function eval_logs() {
   const logs = await api("GET", `/api/logs`)
   last_eval_time = Date.now()
   return logs
 }
 
-export async function eval_log(file) {
-  // the file may have the full uri, strip it down to just the log file
-  const url = new URL(file)
-  file = url.pathname.split("/").pop()
-
-  // get the file
-  return api("GET", `/api/logs/${file}`)
+export async function eval_log(file, headerOnly) {
+  if (headerOnly) {
+    return api("GET", `/api/logs/${file}?header-only=true`)
+  } else {
+    return api("GET", `/api/logs/${file}`)
+  }
 }
 
 export async function api(method, path, body) {
   // build headers
   const headers = {
     Accept: "application/json",
     Pragma: "no-cache",
@@ -36,15 +35,16 @@
   if (body) {
     headers["Content-Type"] = "application/json";
   }
 
   // make request
   const response = await fetch(`${path}`, { method, headers, body });
   if (response.ok) {
-    return response.json()
+    const text = await response.text();
+    return JSON5.parse(text);
   } else if (response.status !== 200) {
     const message = await response.text() || response.statusText;
     const error = new Error(`Error: ${response.status}: ${message})`)
     throw error;
   } else {
     throw new Error(`${response.status} - ${response.statusText} `);
   }
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/css/bootstrap-icons.min.css` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/css/bootstrap.min.css` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/css/fonts/bootstrap-icons.woff` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/css/fonts/bootstrap-icons.woff2` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/bootstrap/js/bootstrap.bundle.min.js` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/favicon.svg` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/favicon.svg`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/log-schema.json` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/log-schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9480648148148149%*

 * *Differences: {"'$defs'": "{'Score': {'properties': {'answer': OrderedDict([('anyOf', [OrderedDict([('type', "*

 * *            "'string')]), OrderedDict([('type', 'null')])]), ('default', None), ('title', "*

 * *            "'Answer')])}, 'required': {insert: [(1, 'answer')]}}}",*

 * * "'properties'": "{'version': {'default': 1}}",*

 * * "'required'": '{delete: [1]}'}*

```diff
@@ -1392,14 +1392,26 @@
             "title": "ModelUsage",
             "type": "object"
         },
         "Score": {
             "additionalProperties": false,
             "description": "Score generated by a scorer.\n\nArgs:\n   value (Value): Score value.\n   explanation (str | None): Optional explanation of score.\n   metadata (dict[str,Any]): Additional metadata related to the score",
             "properties": {
+                "answer": {
+                    "anyOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "default": null,
+                    "title": "Answer"
+                },
                 "explanation": {
                     "anyOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
@@ -1474,14 +1486,15 @@
                         }
                     ],
                     "title": "Value"
                 }
             },
             "required": [
                 "value",
+                "answer",
                 "explanation",
                 "metadata"
             ],
             "title": "Score",
             "type": "object"
         },
         "ToolCall": {
@@ -1614,18 +1627,18 @@
                 "success",
                 "error"
             ],
             "title": "Status",
             "type": "string"
         },
         "version": {
+            "default": 1,
             "title": "Version",
             "type": "integer"
         }
     },
     "required": [
-        "eval",
-        "version"
+        "eval"
     ],
     "title": "EvalLog",
     "type": "object"
 }
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/log.d.ts` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/log.d.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 /* eslint-disable */
 /**
  * This file was automatically generated by json-schema-to-typescript.
  * DO NOT MODIFY IT BY HAND. Instead, modify the source JSONSchema file,
  * and run json-schema-to-typescript to regenerate this file.
  */
 
+export type Version = number;
 export type Status = "started" | "success" | "error";
 export type Task = string;
 export type TaskVersion = number;
 export type TaskFile = string | null;
 export type TaskId = string;
 export type RunId = string;
 export type Created = string;
@@ -45,14 +46,28 @@
 } | null;
 export type Seed = number | null;
 export type Suffix = string | null;
 export type TopK = number | null;
 export type NumChoices = number | null;
 export type Logprobs = boolean | null;
 export type TopLogprobs = number | null;
+export type Name2 = string;
+export type Metadata1 = {} | null;
+export type Name3 = string;
+export type Value = number;
+export type Metadata2 = {} | null;
+export type Metadata3 = {} | null;
+export type StartedAt = string;
+export type CompletedAt = string;
+export type InputTokens = number;
+export type OutputTokens = number;
+export type TotalTokens = number;
+export type Message = string;
+export type Traceback = string;
+export type TracebackAnsi = string;
 export type Samples = EvalSample[] | null;
 export type Id = number | string;
 export type Epoch = number;
 export type Input = string | (ChatMessageSystem | ChatMessageUser | ChatMessageAssistant | ChatMessageTool)[];
 export type Content = string | (ContentText | ContentImage)[];
 export type Type1 = "text";
 export type Text = string;
@@ -80,56 +95,42 @@
 export type Choices = string[] | null;
 export type Target = string | string[];
 export type Messages = (ChatMessageSystem | ChatMessageUser | ChatMessageAssistant | ChatMessageTool)[];
 export type Model1 = string;
 export type StopReason = "stop" | "length" | "tool_calls" | "content_filter" | "unknown";
 export type Logprobs1 = {} | null;
 export type Choices1 = ChatCompletionChoice[];
-export type InputTokens = number;
-export type OutputTokens = number;
-export type TotalTokens = number;
 export type Error = string | null;
-export type Value =
+export type Value1 =
   | string
   | number
   | number
   | boolean
   | (string | number | number | boolean)[]
   | {
       [k: string]: string | number | number | boolean;
     };
+export type Answer = string | null;
 export type Explanation = string | null;
-export type Metadata1 = {} | null;
-export type Name2 = string;
-export type Metadata3 = {} | null;
-export type Name3 = string;
-export type Value1 = number;
 export type Metadata4 = {} | null;
-export type Metadata5 = {} | null;
-export type StartedAt = string;
-export type CompletedAt = string;
 export type Level = "debug" | "http" | "info" | "warning" | "error" | "critical";
-export type Message = string;
+export type Message1 = string;
 export type Created1 = number;
 export type Logging = LoggingMessage[];
-export type Message1 = string;
-export type Traceback = string;
-export type TracebackAnsi = string;
-export type Version = number;
 
 export interface EvalLog {
+  version?: Version;
   status?: Status;
   eval: EvalSpec;
   plan?: EvalPlan;
-  samples?: Samples;
   results?: EvalResults | null;
   stats?: EvalStats;
-  logging?: Logging;
   error?: EvalError | null;
-  version: Version;
+  samples?: Samples;
+  logging?: Logging;
 }
 export interface EvalSpec {
   task: Task;
   task_version: TaskVersion;
   task_file: TaskFile;
   task_id: TaskId;
   run_id: RunId;
@@ -198,24 +199,63 @@
   seed: Seed;
   suffix: Suffix;
   top_k: TopK;
   num_choices: NumChoices;
   logprobs: Logprobs;
   top_logprobs: TopLogprobs;
 }
+export interface EvalResults {
+  scorer: EvalScorer | null;
+  metrics: Metrics;
+  metadata: Metadata3;
+}
+export interface EvalScorer {
+  name: Name2;
+  params: Params1;
+  metadata: Metadata1;
+}
+export interface Params1 {}
+export interface Metrics {
+  [k: string]: EvalMetric;
+}
+export interface EvalMetric {
+  name: Name3;
+  value: Value;
+  options: Options;
+  metadata: Metadata2;
+}
+export interface Options {}
+export interface EvalStats {
+  started_at: StartedAt;
+  completed_at: CompletedAt;
+  model_usage: ModelUsage;
+}
+export interface ModelUsage {
+  [k: string]: ModelUsage1;
+}
+export interface ModelUsage1 {
+  input_tokens: InputTokens;
+  output_tokens: OutputTokens;
+  total_tokens: TotalTokens;
+}
+export interface EvalError {
+  message: Message;
+  traceback: Traceback;
+  traceback_ansi: TracebackAnsi;
+}
 export interface EvalSample {
   id: Id;
   epoch: Epoch;
   input: Input;
   choices: Choices;
   target: Target;
   messages: Messages;
   output: ModelOutput;
   score: Score | null;
-  metadata: Metadata2;
+  metadata: Metadata5;
 }
 export interface ChatMessageSystem {
   content: Content;
   source: Source;
   role: Role;
   tool: Tool;
 }
@@ -252,73 +292,35 @@
   role: Role3;
   tool_call_id: ToolCallId;
   tool_error: ToolError;
 }
 export interface ModelOutput {
   model: Model1;
   choices: Choices1;
-  usage: ModelUsage | null;
+  usage: ModelUsage1 | null;
   error: Error;
 }
 export interface ChatCompletionChoice {
   message: ChatMessageAssistant;
   stop_reason: StopReason;
   logprobs: Logprobs1;
 }
-export interface ModelUsage {
-  input_tokens: InputTokens;
-  output_tokens: OutputTokens;
-  total_tokens: TotalTokens;
-}
 /**
  * Score generated by a scorer.
  *
  * Args:
  *    value (Value): Score value.
  *    explanation (str | None): Optional explanation of score.
  *    metadata (dict[str,Any]): Additional metadata related to the score
  */
 export interface Score {
-  value: Value;
-  explanation: Explanation;
-  metadata: Metadata1;
-}
-export interface Metadata2 {}
-export interface EvalResults {
-  scorer: EvalScorer | null;
-  metrics: Metrics;
-  metadata: Metadata5;
-}
-export interface EvalScorer {
-  name: Name2;
-  params: Params1;
-  metadata: Metadata3;
-}
-export interface Params1 {}
-export interface Metrics {
-  [k: string]: EvalMetric;
-}
-export interface EvalMetric {
-  name: Name3;
   value: Value1;
-  options: Options;
+  answer: Answer;
+  explanation: Explanation;
   metadata: Metadata4;
 }
-export interface Options {}
-export interface EvalStats {
-  started_at: StartedAt;
-  completed_at: CompletedAt;
-  model_usage: ModelUsage1;
-}
-export interface ModelUsage1 {
-  [k: string]: ModelUsage;
-}
+export interface Metadata5 {}
 export interface LoggingMessage {
   level: Level;
-  message: Message;
-  created: Created1;
-}
-export interface EvalError {
   message: Message1;
-  traceback: Traceback;
-  traceback_ansi: TracebackAnsi;
+  created: Created1;
 }
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/preact/hooks.js` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/hooks.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/preact/htm/htm.mjs` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/htm/htm.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/preact/preact.mjs` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/preact.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/prism/prism.min.css` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/prism/prism.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/_view/www/prism/prism.min.js` & `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/prism/prism.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/dataset/__init__.py` & `inspect_ai-0.3.3/src/inspect_ai/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/dataset/_dataset.py` & `inspect_ai-0.3.3/src/inspect_ai/dataset/_dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,28 +58,50 @@
         ...
 
     @overload
     def __getitem__(self, index: int) -> Sample:
         ...
 
     @overload
-    def __getitem__(self, index: slice) -> Sequence[Sample]:
+    def __getitem__(self, index: slice) -> "Dataset":
         ...
 
     @abc.abstractmethod
-    def __getitem__(self, index: Union[int, slice]) -> Union[Sample, Sequence[Sample]]:
+    def __getitem__(self, index: Union[int, slice]) -> Union[Sample, "Dataset"]:
         ...
 
     @abc.abstractmethod
     def __len__(self) -> int:
         ...
 
     @abc.abstractmethod
     def shuffle(self, seed: int | None = None) -> None:
-        ...
+        """Shuffle the order of the dataset (in place).
+
+        Args:
+           seed: (int | None): Random seed for shuffling (optional).
+        """
+
+    def filter(
+        self, predicate: Callable[[Sample], bool], name: str | None = None
+    ) -> "Dataset":
+        """Filter the dataset using a predicate.
+
+        Args:
+          predicate (Callable[[Sample], bool]): Filtering function.
+          name (str | None): Name for filtered dataset (optional).
+
+        Returns:
+          Filtered dataset.
+        """
+        return MemoryDataset(
+            name=name or self.name,
+            location=self.location,
+            samples=[sample for sample in self if predicate(sample)],
+        )
 
 
 class FieldSpec(BaseModel):
     r"""Specification for mapping data source fields to sample fields.
 
     Args:
         input (str): Name of the field containing the sample input.
@@ -146,20 +168,25 @@
         return self._location
 
     @overload
     def __getitem__(self, index: int) -> Sample:
         ...
 
     @overload
-    def __getitem__(self, index: slice) -> Sequence[Sample]:
+    def __getitem__(self, index: slice) -> Dataset:
         ...
 
     @override
-    def __getitem__(self, index: Union[int, slice]) -> Union[Sample, Sequence[Sample]]:
-        return self.samples[index]
+    def __getitem__(self, index: Union[int, slice]) -> Union[Sample, Dataset]:
+        if isinstance(index, int):
+            return self.samples[index]
+        else:
+            return MemoryDataset(
+                samples=self.samples[index], name=self.name, location=self.location
+            )
 
     @override
     def __len__(self) -> int:
         return len(self.samples)
 
     @override
     def shuffle(self, seed: int | None = None) -> None:
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/dataset/_examples/bias_detection.jsonl` & `inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/bias_detection.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/dataset/_examples/biology_qa.jsonl` & `inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/biology_qa.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/dataset/_examples/popularity.jsonl` & `inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/popularity.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/dataset/_examples/security_guide.jsonl` & `inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/security_guide.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl` & `inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/dataset/_sources/csv.py` & `inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/csv.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/dataset/_sources/example.py` & `inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/example.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 ) -> Dataset:
     """Read a dataset from inspect_ai package examples.
 
     This is primarily used for sharing runnable example
     snippets that don't need to read an external dataset.
 
     Args:
-      name (str): Example dataset name. One of 'bias_detection',
-        'security_guide', 'theory_of_mind', 'popularity', or 'biology_qa'
+      name (str): Example dataset name. One of 'security_guide', 'theory_of_mind',
+        'popularity', or 'biology_qa'
       sample_fields (SampleFieldSpec | RecordToSample): Method of mapping underlying
         fields in the data source to `Sample` objects. Pass `None` if the data is already
         stored in `Sample` form (i.e. object with "input" and "target" fields); Pass a
         `SampleFieldSpec` to specify mapping fields by name; Pass a `RecordToSample` to
         handle mapping with a custom function.
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/dataset/_sources/file.py` & `inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/file.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/dataset/_sources/hf.py` & `inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/hf.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/dataset/_sources/json.py` & `inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/json.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/dataset/_util.py` & `inspect_ai-0.3.3/src/inspect_ai/dataset/_util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/log/__init__.py` & `inspect_ai-0.3.3/src/inspect_ai/log/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ._file import (
     EvalLogInfo,
+    eval_log_json,
     list_eval_logs,
     read_eval_log,
     write_eval_log,
 )
 from ._log import (
     EvalConfig,
     EvalDataset,
@@ -38,8 +39,9 @@
     "EvalStats",
     "EvalLogInfo",
     "LoggingLevel",
     "LoggingMessage",
     "list_eval_logs",
     "read_eval_log",
     "write_eval_log",
+    "eval_log_json",
 ]
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/log/_file.py` & `inspect_ai-0.3.3/src/inspect_ai/log/_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import os
+import re
 from pathlib import Path
-from typing import Any, Literal, cast
+from typing import Any, Callable, cast
 from urllib.parse import urlparse
 
+import json_stream  # type: ignore
 from pydantic import BaseModel, Field
 
 from inspect_ai._util.file import FileInfo, file, filesystem
 
 from ._log import (
     EvalError,
     EvalLog,
@@ -31,74 +33,116 @@
 
     suffix: str | None
     """Log file suffix (e.g. "-scored")"""
 
 
 def list_eval_logs(
     log_dir: str = os.environ.get("INSPECT_LOG_DIR", "./logs"),
-    status: Literal["started", "success", "error"] | None = None,
+    filter: Callable[[EvalLog], bool] | None = None,
+    recursive: bool = True,
     extensions: list[str] = [".json", ".jsonl"],
     descending: bool = True,
     fs_options: dict[str, Any] = {},
 ) -> list[EvalLogInfo]:
     """List all eval logs in a directory.
 
     Args:
       log_dir (str): Log directory (defaults to INSPECT_LOG_DIR)
-      status (Literal["success", "error"] | None): List only
-         log files with the specified status.
+      filter (Callable[[EvalLog], bool]): Filter to limit logs returned.
+         Note that the EvalLog instance passed to the filter has only
+         the EvalLog header (i.e. does not have the samples or logging output).
+      recursive (bool): List log files recursively (defaults to True).
+
       extensions (list[str]): File extension to scan for logs
       descending (bool): List in descening order.
       fs_options (dict[str, Any]): Optional. Addional arguments to pass through
           to the filesystem provider (e.g. `S3FileSystem`).
 
     Returns:
        List of EvalLog Info.
 
     """
     # get the eval logs
     fs = filesystem(log_dir, fs_options)
-    eval_logs = log_files_from_ls(fs.ls(log_dir), extensions, descending)
+    if fs.exists(log_dir):
+        eval_logs = log_files_from_ls(
+            fs.ls(log_dir, recursive=recursive), extensions, descending
+        )
+    else:
+        return []
 
-    # apply status filter if requested
-    if status:
-        return [log for log in eval_logs if read_eval_log(log.name).status == status]
+    # apply filter if requested
+    if filter:
+        return [
+            log
+            for log in eval_logs
+            if filter(read_eval_log(log.name, header_only=True))
+        ]
     else:
         return eval_logs
 
 
 def write_eval_log(log: EvalLog, log_file: str) -> None:
     """Write an evaluation log.
 
     Args:
        log (EvalLog): Evaluation log to write.
        log_file (str): Location to write log to.
 
     """
     with file(log_file, "w") as f:
-        f.write(
-            log.model_dump_json(exclude_none=True, exclude_defaults=False, indent=2)
-        )
+        f.write(eval_log_json(log))
 
 
-def read_eval_log(log_file: str) -> "EvalLog":
+def eval_log_json(log: EvalLog) -> str:
+    return log.model_dump_json(exclude_none=True, exclude_defaults=False, indent=2)
+
+
+def read_eval_log(log_file: str, header_only: bool = False) -> EvalLog:
     """Read an evaluation log.
 
     Args:
        log_file (str): Log file to read.
+       header_only (bool): Read only the header (i.e. exclude
+         the "samples" and "logging" fields). Defaults to False.
 
     Returns:
        EvalLog object read from file.
     """
     with file(log_file, "r") as f:
-        raw_data = json.load(f)
-        log = EvalLog(**raw_data)
-        if log.version > 1:
-            raise ValueError(f"Unable to read version {log.version} of log format.")
-        return log
+        # header-only uses json-stream
+        if header_only:
+            data = json_stream.load(f, persistent=True)
+
+            def read_field(field: str) -> Any:
+                if field in data.keys():
+                    return json_stream.to_standard_types(data[field])
+                else:
+                    return None
+
+            results = read_field("results")
+            error = read_field("error")
+
+            return EvalLog(
+                version=read_field("version"),
+                status=read_field("status"),
+                eval=EvalSpec(**read_field("eval")),
+                plan=EvalPlan(**read_field("plan")),
+                results=EvalResults(**results) if results else None,
+                stats=EvalStats(**read_field("stats")),
+                error=EvalError(**error) if error else None,
+            )
+
+        # otherwise normal json parse
+        else:
+            raw_data = json.load(f)
+            log = EvalLog(**raw_data)
+            if log.version > 1:
+                raise ValueError(f"Unable to read version {log.version} of log format.")
+            return log
 
 
 class FileRecorder(Recorder):
     def __init__(
         self, log_dir: str, suffix: str, fs_options: dict[str, Any] = {}
     ) -> None:
         super().__init__()
@@ -137,19 +181,29 @@
     ls: list[FileInfo],
     extensions: list[str] = [".json", ".jsonl"],
     descending: bool = True,
 ) -> list[EvalLogInfo]:
     return [
         log_file_info(file)
         for file in sorted(ls, key=lambda file: file.mtime, reverse=descending)
-        if file.type == "file"
-        and any([file.name.endswith(suffix) for suffix in extensions])
+        if file.type == "file" and is_log_file(file.name, extensions)
     ]
 
 
+log_file_pattern = r"^\d{4}-\d{2}-\d{2}T\d{2}[:-]\d{2}[:-]\d{2}.*$"
+
+
+def is_log_file(file: str, extensions: list[str]) -> bool:
+    parts = file.replace("\\", "/").split("/")
+    name = parts[-1]
+    return re.match(log_file_pattern, name) is not None and any(
+        [name.endswith(suffix) for suffix in extensions]
+    )
+
+
 def log_file_info(info: FileInfo) -> "EvalLogInfo":
     # extract the basename and split into parts
     # (deal with previous logs had the model in their name)
     basename = os.path.splitext(info.name)[0]
     parts = basename.split("/").pop().split("_")
     last_idx = 3 if len(parts) > 3 else 2
     task = parts[1]
@@ -185,15 +239,15 @@
         self.data: dict[str, JSONRecorder.JSONLogFile] = {}
 
     def log_start(self, eval: EvalSpec) -> str:
         # initialize file log for this eval
         file = self._log_file_path(eval)
         self.data[self._log_file_key(eval)] = JSONRecorder.JSONLogFile(
             file=file,
-            data=EvalLog(eval=eval, version=1),
+            data=EvalLog(eval=eval),
             events=0,
         )
         return file
 
     def log_event(
         self,
         spec: EvalSpec,
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/log/_log.py` & `inspect_ai-0.3.3/src/inspect_ai/log/_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,40 +295,40 @@
             level=cast(LoggingLevel, record.levelname.lower()),
             message=record.getMessage(),
             created=record.created * 1000,
         )
 
 
 class EvalLog(BaseModel):
+    version: int = Field(default=1)
+    """Eval log file format version."""
+
     status: Literal["started", "success", "error"] = Field(default="started")
     """Status of evaluation (did it succeed or fail)."""
 
     eval: EvalSpec
     """Eval identity and configuration."""
 
     plan: EvalPlan = Field(default=EvalPlan())
     """Eval plan (sovers and config)"""
 
-    samples: list[EvalSample] | None = Field(default=None)
-    """Samples processed by eval."""
-
     results: EvalResults | None = None
     """Eval results (scores and metrics)."""
 
     stats: EvalStats = Field(default=EvalStats())
     """Eval stats (runtime, model usage)"""
 
-    logging: list[LoggingMessage] = Field(default=[])
-    """Logging message captured during eval."""
-
     error: EvalError | None = Field(default=None)
     """Error that halted eval (if status=="error")"""
 
-    version: int
-    """Eval log file format version."""
+    samples: list[EvalSample] | None = Field(default=None)
+    """Samples processed by eval."""
+
+    logging: list[LoggingMessage] = Field(default=[])
+    """Logging message captured during eval."""
 
 
 LogEvent = Literal["plan", "sample", "score", "results", "scorer", "logging"]
 
 
 class Recorder(abc.ABC):
     @abc.abstractmethod
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/__init__.py` & `inspect_ai-0.3.3/src/inspect_ai/model/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ModelOutput,
     ModelUsage,
     StopReason,
     get_model,
 )
 from ._providers.providers import *
 from ._registry import modelapi
-from ._tool import ToolCall, ToolChoice, ToolDef, ToolFunction, ToolParam
+from ._tool import ToolCall, ToolChoice, ToolFunction, ToolInfo, ToolParam
 
 __all__ = [
     "GenerateConfig",
     "GenerateConfigArgs",
     "ContentText",
     "ContentImage",
     "Content",
@@ -41,13 +41,13 @@
     "ModelAPI",
     "ModelName",
     "ModelUsage",
     "StopReason",
     "ToolCall",
     "ToolChoice",
     "ToolFunction",
-    "ToolDef",
+    "ToolInfo",
     "ToolParam",
     "ToolType",
     "get_model",
     "modelapi",
 ]
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_model.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 )
 from inspect_ai._util.platform import platform_init
 from inspect_ai._util.registry import RegistryInfo, registry_find, registry_info
 from inspect_ai._util.retry import log_rate_limit_retry
 from inspect_ai.util import concurrency
 from inspect_ai.util._context.concurrency import using_concurrency
 
-from ._tool import ToolCall, ToolChoice, ToolDef, ToolFunction
+from ._tool import ToolCall, ToolChoice, ToolFunction, ToolInfo
 
 
 class GenerateConfigArgs(TypedDict, total=False):
     """Type for kwargs that selectively override GenerateConfig."""
 
     max_retries: int | None
     """Maximum number of times to retry request (defaults to 5)."""
@@ -326,24 +326,33 @@
 
     error: str | None = Field(default=None)
     """Error message in the case of content moderation refusals."""
 
     @property
     def completion(self) -> str:
         """Text of first message choice text."""
-        return self.choices[0].message.text
+        if len(self.choices) > 0:
+            return self.choices[0].message.text
+        else:
+            return ""
 
     @completion.setter
     def completion(self, completion: str) -> None:
         """Set the text of the first message choice.
 
         Args:
           completion (str): Text for first message.
         """
-        self.choices[0].message.text = completion
+        if len(self.choices) > 0:
+            self.choices[0].message.text = completion
+        else:
+            self.choices.append(ChatCompletionChoice(
+                message = ChatMessageAssistant(content = completion),
+                stop_reason="stop"
+            ))
 
     @staticmethod
     def from_content(
         model: str,
         content: str,
         stop_reason: StopReason = "stop",
         error: str | None = None,
@@ -378,25 +387,25 @@
         self.base_url = base_url
         self.config = config
 
     @abc.abstractmethod
     async def generate(
         self,
         input: list[ChatMessage],
-        tools: list[ToolDef],
+        tools: list[ToolInfo],
         tool_choice: ToolChoice,
         config: GenerateConfig,
     ) -> ModelOutput:
         """Generate output from the model.
 
         Args:
           input (str | list[ChatMessage]): Chat message
             input (if a `str` is passed it is convereted
             to a `ChatUserMessage`).
-          tools (list[ToolDef]): Tools available for the
+          tools (list[ToolInfo]): Tools available for the
             model to call.
           tool_choice (ToolChoice): Directives to the model
             as to which tools to prefer.
           config (GenerateConfig): Model configuration.
 
         Returns:
            ModelOutput
@@ -448,25 +457,25 @@
 
     def __str__(self) -> str:
         return f"{ModelName(self)}"
 
     async def generate(
         self,
         input: str | list[ChatMessage],
-        tools: list[ToolDef] = [],
+        tools: list[ToolInfo] = [],
         tool_choice: ToolChoice | None = None,
         config: GenerateConfig = GenerateConfig(),
     ) -> ModelOutput:
         """Generate output from the model.
 
         Args:
           input (str | list[ChatMessage]): Chat message
             input (if a `str` is passed it is convereted
             to a `ChatUserMessage`).
-          tools (list[ToolDef]): Tools available for the
+          tools (list[ToolInfo]): Tools available for the
             model to call.
           tool_choice (ToolChoice): Directives to the model
             as to which tools to prefer.
           config (GenerateConfig): Model configuration.
 
         Returns:
            ModelOutput
@@ -497,15 +506,15 @@
         # no connection semaphore, just proceed straight ot the call
         else:
             return await self._generate(input, tools, tool_choice, config)
 
     async def _generate(
         self,
         input: list[ChatMessage],
-        tools: list[ToolDef],
+        tools: list[ToolInfo],
         tool_choice: ToolChoice | None,
         config: GenerateConfig,
     ) -> ModelOutput:
         # default to 'auto' for tool_choice (same as underlying model apis)
         tool_choice = tool_choice if tool_choice else "auto"
 
         # if we have a specific tool selected then filter out the others
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_providers/anthropic.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_providers/anthropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     ContentText,
     GenerateConfig,
     ModelAPI,
     ModelOutput,
     ModelUsage,
     StopReason,
 )
-from .._tool import ToolCall, ToolChoice, ToolDef, ToolFunction, ToolParam
+from .._tool import ToolCall, ToolChoice, ToolFunction, ToolInfo, ToolParam
 from .._util import chat_api_tool
 
 ANTHROPIC_API_KEY = "ANTHROPIC_API_KEY"
 
 
 class AnthropicAPI(ModelAPI):
     def __init__(
@@ -105,15 +105,15 @@
                 ),
                 **model_args,
             )
 
     async def generate(
         self,
         input: list[ChatMessage],
-        tools: list[ToolDef],
+        tools: list[ToolInfo],
         tool_choice: ToolChoice,
         config: GenerateConfig,
     ) -> ModelOutput:
         # generate
         try:
             # use tools beta endpoint if we have tools and haven't opted out (note that
             # bedrock is an implicit opt-out as it doesn't yet support the tools api
@@ -213,15 +213,15 @@
 # tool use beta. we also keep the legacy tools implementation around for now (see below)
 # for users on Bedrock of who want to opt out for tools beta for any reason
 #######################################################################################
 
 
 async def resolve_tools_beta_chat_input(
     input: list[ChatMessage],
-    tools: list[ToolDef],
+    tools: list[ToolInfo],
     tool_choice: ToolChoice,
     config: GenerateConfig,
 ) -> Tuple[str | None, list[BetaToolParam], list[ToolsBetaMessageParam]]:
     # extract system message
     system_message, messages = split_system_message(input, config)
 
     # some special handling for tools
@@ -268,15 +268,14 @@
     # no system role for anthropic (this is more like an asseration,
     # as these should have already been filtered out)
     if message.role == "system":
         raise ValueError("Antropic models do not support the system role")
 
     # "tool" means serving a tool call result back to claude
     elif message.role == "tool":
-
         if message.tool_error is not None:
             content: str | list[TextBlockParam] = message.tool_error
         if isinstance(message.content, str):
             content = [TextBlockParam(type="text", text=message.content)]
         else:
             content = [
                 TextBlockParam(type="text", text=content.text)
@@ -294,15 +293,14 @@
                     is_error=message.tool_error is not None,
                 )
             ],
         )
 
     # tool_calls means claude is attempting to call our tools
     elif message.role == "assistant" and message.tool_calls:
-
         # first include content (claude <thinking>)
         tools_content: list[TextBlockParam | ImageBlockParam | ToolUseBlockParam] = (
             [TextBlockParam(type="text", text=message.content)]
             if isinstance(message.content, str)
             else (
                 [(await message_param_content(content)) for content in message.content]
             )
@@ -335,15 +333,15 @@
             content=[
                 await message_param_content(content) for content in message.content
             ],
         )
 
 
 def tools_beta_model_output_from_message(
-    message: ToolsBetaMessage, tools: list[ToolDef]
+    message: ToolsBetaMessage, tools: list[ToolInfo]
 ) -> ModelOutput:
     # extract content and tool calls
     content: list[Content] = []
     tool_calls: list[ToolCall] | None = None
 
     for content_block in message.content:
         if isinstance(content_block, TextBlock):
@@ -431,15 +429,15 @@
 # into XML encoded role="user" messages for Claude
 #######################################################################################
 
 FUNCTIONS_STOP_SEQ = "</function_calls>"
 
 
 async def resolve_chat_input(
-    input: list[ChatMessage], tools: list[ToolDef], config: GenerateConfig
+    input: list[ChatMessage], tools: list[ToolInfo], config: GenerateConfig
 ) -> Tuple[str | None, list[str] | None, list[MessageParam]]:
     # extract system message
     system_message, messages = split_system_message(input, config)
 
     # resolve tool use (system message and stop sequences)
     stop_seqs = deepcopy(config.stop_seqs)
     if len(tools) > 0:
@@ -452,15 +450,15 @@
     # create anthropic message params
     message_params = [await message_param(m) for m in messages]
 
     # done!
     return system_message, stop_seqs, message_params
 
 
-def tools_system_message(tools: list[ToolDef]) -> str:
+def tools_system_message(tools: list[ToolInfo]) -> str:
     tool_sep = "\n\n"
     return f"""
 In this environment you have access to a set of tools you can use to answer the user's question.
 
 You may call them like this:
 <function_calls>
 <invoke>
@@ -475,15 +473,15 @@
 Here are the tools available:
 <tools>
 {tool_sep.join([tool_description(tool) for tool in tools])}
 </tools>
 """
 
 
-def tool_description(tool: ToolDef) -> str:
+def tool_description(tool: ToolInfo) -> str:
     newline = "\n"
     return f"""
 <tool_description>
 <tool_name>{escape(tool.name)}</tool_name>
 <description>{escape(tool.description)}</description>
 <parameters>
 {newline.join(tool_param(param) for param in tool.params)}
@@ -614,15 +612,15 @@
 #
 # Anthropic encodes tool calls (in XML) directly in role="assistant" messages. The
 # code below deals with this by parsing out the tool calls and separating them into
 # the Inspect native ToolCall objects.
 #######################################################################################
 
 
-def model_output_from_message(message: Message, tools: list[ToolDef]) -> ModelOutput:
+def model_output_from_message(message: Message, tools: list[ToolInfo]) -> ModelOutput:
     # extract function calls (if any); throws ValueError if xml is invalid
     try:
         content_with_functions = extract_function_calls(message)
         if content_with_functions:
             content = content_with_functions.content
             tool_calls = [
                 tool_call(function_call, tools)
@@ -806,36 +804,36 @@
 
 
 #######################################################################################
 # Thse functions deal with converting Anthropic <function_call> to our native ToolCall
 #######################################################################################
 
 
-def tool_call(invoke: FunctionCall, tools: list[ToolDef]) -> ToolCall:
+def tool_call(invoke: FunctionCall, tools: list[ToolInfo]) -> ToolCall:
     tool_def = next((tool for tool in tools if invoke.function == tool.name), None)
     return ToolCall(
         id=invoke.function,
         function=invoke.function,
         arguments=tool_arguments(invoke.parameters, tool_def),
         type="function",
     )
 
 
 def tool_arguments(
-    params: list[tuple[str, str]], tool_def: ToolDef | None
+    params: list[tuple[str, str]], tool_info: ToolInfo | None
 ) -> dict[str, Any]:
     arguments: dict[str, Any] = dict()
     for param in params:
         # get params
         name, value = param
 
         # coerce type if we have a tool_def
-        if tool_def:
+        if tool_info:
             type_str = next(
-                (param.type for param in tool_def.params if param.name == name), None
+                (param.type for param in tool_info.params if param.name == name), None
             )
             if type_str:
                 value = tool_argument_value(value, type_str)
 
         arguments[name] = value
 
     return arguments
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_providers/azureai.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_providers/azureai.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     ChatMessageAssistant,
     GenerateConfig,
     ModelAPI,
     ModelOutput,
     ModelUsage,
     StopReason,
 )
-from .._tool import ToolChoice, ToolDef
+from .._tool import ToolChoice, ToolInfo
 from .._util import (
     chat_api_input,
     chat_api_request,
     is_chat_api_rate_limit,
 )
 from .util import as_stop_reason, model_base_url
 
@@ -76,15 +76,15 @@
         # create client
         self.client = httpx.AsyncClient()
         self.model_args = model_args
 
     async def generate(
         self,
         input: list[ChatMessage],
-        tools: list[ToolDef],
+        tools: list[ToolInfo],
         tool_choice: ToolChoice,
         config: GenerateConfig,
     ) -> ModelOutput:
         # There are two different model APIs on Azure AI. The first is associated
         # with 'realtime' deployments of llama-2 (and maps closely to other llama-2
         # inference apis):
         # https://ai.azure.com/explore/models/Llama-2-70b-chat/version/17/registry/azureml-meta
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_providers/bedrock.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_providers/bedrock.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     ChatMessageUser,
     GenerateConfig,
     ModelAPI,
     ModelOutput,
     ModelUsage,
     simple_input_messages,
 )
-from .._tool import ToolChoice, ToolDef
+from .._tool import ToolChoice, ToolInfo
 from .util import as_stop_reason, model_base_url
 
 
 class BedrockAPI(ModelAPI):
     def __init__(
         self,
         model_name: str,
@@ -64,15 +64,15 @@
             self.handler = Llama2ChatHandler(model_name, base_url, config)
         else:
             raise ValueError(f"Unsupported Bedrock model: {model_name}")
 
     async def generate(
         self,
         input: list[ChatMessage],
-        tools: list[ToolDef],
+        tools: list[ToolInfo],
         tool_choice: ToolChoice,
         config: GenerateConfig,
     ) -> ModelOutput:
         if self.model_api:
             return await self.model_api.generate(input, tools, tool_choice, config)
         else:
             return await self.handler.generate(input, config)
@@ -184,18 +184,20 @@
         return False
 
     @abc.abstractmethod
     def request_body(
         self,
         input: list[ChatMessage],
         config: GenerateConfig,
-    ) -> dict[str, Any]: ...
+    ) -> dict[str, Any]:
+        ...
 
     @abc.abstractmethod
-    def completion_choice(self, response: dict[str, Any]) -> ChatCompletionChoice: ...
+    def completion_choice(self, response: dict[str, Any]) -> ChatCompletionChoice:
+        ...
 
     # optional hook to provide a system message folding template
     def fold_system_message(self, user: str, system: str) -> str:
         return f"{system}\n\n{user}"
 
     # optional hook to extract model usage
     def model_usage(self, response: dict[str, Any]) -> ModelUsage | None:
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_providers/cloudflare.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_providers/cloudflare.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     ChatMessage,
     GenerateConfig,
     ModelAPI,
     ModelOutput,
 )
 from inspect_ai.model._providers.util import model_base_url
 
-from .._tool import ToolChoice, ToolDef
+from .._tool import ToolChoice, ToolInfo
 from .._util import (
     chat_api_input,
     chat_api_request,
     is_chat_api_rate_limit,
 )
 
 # CloudFlare supported models:
@@ -45,15 +45,15 @@
             base_url if base_url else "https://api.cloudflare.com/client/v4/accounts"
         )
         self.model_args = model_args
 
     async def generate(
         self,
         input: list[ChatMessage],
-        tools: list[ToolDef],
+        tools: list[ToolInfo],
         tool_choice: ToolChoice,
         config: GenerateConfig,
     ) -> ModelOutput:
         # chat url
         chat_url = f"{self.base_url}/{self.account_id}/ai/run/@cf"
 
         # chat api input
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_providers/google.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_providers/google.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     ContentImage,
     ContentText,
     GenerateConfig,
     ModelAPI,
     ModelOutput,
     StopReason,
 )
-from .._tool import ToolCall, ToolChoice, ToolDef
+from .._tool import ToolCall, ToolChoice, ToolInfo
 from .._util import chat_api_tool
 
 VERTEX_SAFETY_SETTINGS = {
     HarmCategory.HARM_CATEGORY_SEXUALLY_EXPLICIT: HarmBlockThreshold.BLOCK_NONE,
     HarmCategory.HARM_CATEGORY_HATE_SPEECH: HarmBlockThreshold.BLOCK_NONE,
     HarmCategory.HARM_CATEGORY_HARASSMENT: HarmBlockThreshold.BLOCK_NONE,
     HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT: HarmBlockThreshold.BLOCK_NONE,
@@ -78,15 +78,15 @@
 
         # create model
         self.model = GenerativeModel(self.model_name)
 
     async def generate(
         self,
         input: list[ChatMessage],
-        tools: list[ToolDef],
+        tools: list[ToolInfo],
         tool_choice: ToolChoice,
         config: GenerateConfig,
     ) -> ModelOutput:
         parameters = GenerationConfig(
             candidate_count=config.num_choices,
             temperature=config.temperature,
             top_p=config.top_p,
@@ -218,15 +218,15 @@
     # (if there is no first user message then prepend one)
     if messages[0].get("role") == "user":
         messages[0]["parts"] = system_parts + messages[0].get("parts", [])
     else:
         messages.insert(0, ContentDict(role="user", parts=system_parts))
 
 
-def chat_tools(tools: list[ToolDef]) -> list[Tool]:
+def chat_tools(tools: list[ToolInfo]) -> list[Tool]:
     chat_tools = [chat_api_tool(tool) for tool in tools]
     declarations = [
         FunctionDeclaration(
             name=tool["function"]["name"],
             description=tool["function"]["description"],
             parameters=tool["function"]["parameters"],
         )
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_providers/hf.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_providers/hf.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ChatMessageAssistant,
     GenerateConfig,
     ModelAPI,
     ModelOutput,
     ModelUsage,
     simple_input_messages,
 )
-from .._tool import ToolChoice, ToolDef
+from .._tool import ToolChoice, ToolInfo
 from .._util import chat_api_input
 
 
 class HuggingFaceAPI(ModelAPI):
     def __init__(
         self,
         model_name: str,
@@ -88,15 +88,15 @@
             self.tokenizer = AutoTokenizer.from_pretrained(model_name)
         # LLMs generally don't have a pad token and we need one for batching
         self.tokenizer.pad_token = self.tokenizer.eos_token
 
     async def generate(
         self,
         input: list[ChatMessage],
-        tools: list[ToolDef],
+        tools: list[ToolInfo],
         tool_choice: ToolChoice,
         config: GenerateConfig,
     ) -> ModelOutput:
         # create chat
         chat = self.hf_chat(input)
 
         # prepare tokenizer
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_providers/mistral.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_providers/mistral.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     ChatMessageAssistant,
     GenerateConfig,
     ModelAPI,
     ModelOutput,
     ModelUsage,
     StopReason,
 )
-from .._tool import ToolCall, ToolChoice, ToolDef, ToolFunction
+from .._tool import ToolCall, ToolChoice, ToolFunction, ToolInfo
 from .._util import chat_api_tool
 
 AZURE_MISTRAL_API_KEY = "AZURE_MISTRAL_API_KEY"
 AZUREAI_MISTRAL_API_KEY = "AZUREAI_MISTRAL_API_KEY"
 MISTRAL_API_KEY = "MISTRAL_API_KEY"
 
 
@@ -91,15 +91,15 @@
             timeout=config.timeout if config.timeout else DEFAULT_TIMEOUT,
             **model_args,
         )
 
     async def generate(
         self,
         input: list[ChatMessage],
-        tools: list[ToolDef],
+        tools: list[ToolInfo],
         tool_choice: ToolChoice,
         config: GenerateConfig,
     ) -> ModelOutput:
         # send request
         response = await self.client.chat(
             model=self.model_name,
             messages=[mistral_chat_message(message) for message in input],
@@ -140,15 +140,15 @@
     # not clear what the mistral default max tokens is (not documented)
     # so we set it to the default to be sure
     @override
     def max_tokens(self) -> int:
         return DEFAULT_MAX_TOKENS
 
 
-def mistral_chat_tools(tools: list[ToolDef]) -> list[dict[str, Any]]:
+def mistral_chat_tools(tools: list[ToolInfo]) -> list[dict[str, Any]]:
     chat_tools = [chat_api_tool(tool) for tool in tools]
     return [dict(type=tool["type"], function=tool["function"]) for tool in chat_tools]
 
 
 def mistral_chat_tool_choice(tool_choice: ToolChoice) -> MistralToolChoice:
     if isinstance(tool_choice, ToolFunction):
         # mistral doesn't support specifically named tools to use
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_providers/openai.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_providers/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ChatMessageAssistant,
     Content,
     GenerateConfig,
     ModelAPI,
     ModelOutput,
     ModelUsage,
 )
-from .._tool import ToolCall, ToolChoice, ToolDef, ToolFunction
+from .._tool import ToolCall, ToolChoice, ToolFunction, ToolInfo
 from .._util import chat_api_tool
 from .util import as_stop_reason, model_base_url
 
 OPENAI_API_KEY = "OPENAI_API_KEY"
 AZURE_OPENAI_API_KEY = "AZURE_OPENAI_API_KEY"
 AZUREAI_OPENAI_API_KEY = "AZUREAI_OPENAI_API_KEY"
 
@@ -111,15 +111,15 @@
                 ),
                 **model_args,
             )
 
     async def generate(
         self,
         input: list[ChatMessage],
-        tools: list[ToolDef],
+        tools: list[ToolInfo],
         tool_choice: ToolChoice,
         config: GenerateConfig,
     ) -> ModelOutput:
         # resolve max tokens (ignore type check so NotGiven is valid)
         config.max_tokens = config.max_tokens if config.max_tokens else NOT_GIVEN  # type: ignore
         # unlike text models, vision models require a max_tokens (and set it to a very low
         # default, see https://community.openai.com/t/gpt-4-vision-preview-finish-details/475911/10)
@@ -270,15 +270,15 @@
         function=dict(
             name=tool_call.function, arguments=json.dumps(tool_call.arguments)
         ),
         type=tool_call.type,
     )
 
 
-def chat_tools(tools: list[ToolDef]) -> list[ChatCompletionToolParam]:
+def chat_tools(tools: list[ToolInfo]) -> list[ChatCompletionToolParam]:
     chat_tools = [chat_api_tool(tool) for tool in tools]
     return [
         ChatCompletionToolParam(
             type=tool["type"], function=cast(FunctionDefinition, tool["function"])
         )
         for tool in chat_tools
     ]
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_providers/providers.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_providers/providers.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_providers/together.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_providers/together.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_providers/util.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_providers/util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_registry.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_tool.py` & `inspect_ai-0.3.3/src/inspect_ai/solver/_tool/tool_def.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,81 @@
+import inspect
 from dataclasses import dataclass
-from typing import (
-    Any,
-    Callable,
-    Literal,
-    Union,
-)
+from typing import Any, Callable
 
-from inspect_ai._util.error import exception_message
-from inspect_ai._util.json import JSONType
-from inspect_ai._util.registry import registry_info
-
-
-@dataclass
-class ToolParam:
-    name: str
-    """Parameter name."""
-
-    type: JSONType
-    """JSON type of parameter."""
+from docstring_parser import Docstring, DocstringParam
 
-    description: str
-    """Description of parameter."""
+from inspect_ai._util.docstring import parse_docstring
+from inspect_ai._util.json import python_type_to_json_type
+from inspect_ai._util.registry import registry_info
+from inspect_ai.model import ToolParam
 
-    optional: bool
-    """Is the parameter optional"""
+from .tool import TOOL_PARAMS, TOOL_PROMPT, Tool
 
 
 @dataclass
 class ToolDef:
     name: str
     """Tool name."""
 
     description: str
     """Tool description."""
 
-    prompt: str | None
-    """System prommpt text to guide model usage of tool."""
-
     params: list[ToolParam]
     """Tool parameters"""
 
+    prompt: str | None
+    """System prompt text to guide model usage of tool."""
+
     tool: Callable[..., Any]
     """Callable to execute tool."""
 
 
-@dataclass
-class ToolCall:
-    id: str
-    """Unique identifer for tool call."""
-
-    function: str
-    """Function called."""
-
-    arguments: dict[str, Any]
-    """Arguments to function."""
+def tool_defs(tools: list[Tool]) -> list[ToolDef]:
+    return [tool_def(tool) for tool in tools]
 
-    type: Literal["function"]
-    """Type of tool call (currently only 'function')"""
-
-
-@dataclass
-class ToolFunction:
-    name: str
-    """The name of the function to call."""
-
-
-ToolChoice = Union[Literal["none", "auto"], ToolFunction]
-"""Specify which tool to call.
-
-"auto" means the model decides; "none" means never call a tool; and
-ToolFunction instructs the model to call a specific function.
-"""
 
+def tool_def(tool: Tool) -> ToolDef:
+    tool_info = registry_info(tool)
+    name = tool_info.name.split("/")[-1]
+    docstring = tool_docstring(tool)
+
+    # exclude built in tool params (as we will curry these
+    # so the model doesn't need to know about them)
+    metadata_params = list(tool_info.metadata.get(TOOL_PARAMS, {}).keys())
+    params = [
+        tool_param(param)
+        for param in docstring.params
+        if param.arg_name not in metadata_params
+    ]
+    return ToolDef(
+        name=name,
+        description=str(docstring.short_description),
+        prompt=tool_info.metadata.get(TOOL_PROMPT, None),
+        params=params,
+        tool=tool,
+    )
 
-async def call_tool(
-    tools: list[ToolDef], call: ToolCall, metadata: dict[str, Any]
-) -> Any:
-    # find the tool
-    tool_def = next((tool for tool in tools if tool.name == call.function), None)
-    if tool_def is None:
-        return f"Tool {call.function} not found"
 
-    # resolve metadata params and prepend to arguments
-    tool_params: dict[str, str] = registry_info(tool_def.tool).metadata.get(
-        TOOL_PARAMS, {}
+def tool_param(param: DocstringParam) -> ToolParam:
+    return ToolParam(
+        name=param.arg_name,
+        type=python_type_to_json_type(param.type_name),
+        description=str(param.description),
+        optional=param.is_optional is True,
     )
-    resolved_params: dict[str, Any] = {}
-    for name, value in tool_params.items():
-        key = value.removeprefix("metadata.")
-        resolved = metadata.get(key, None)
-        if resolved is None:
-            raise ValueError(f"Metadata value '{key}' not found for tool parameter")
-        resolved_params[name] = resolved
-    arguments = resolved_params | call.arguments
-
-    # call the tool
-    try:
-        return await tool_def.tool(**arguments)
-    except Exception as e:
-        return f"Error: {exception_message(e)}"
 
 
-TOOL_PROMPT = "prompt"
-TOOL_PARAMS = "params"
+def tool_docstring(tool: Tool) -> Docstring:
+    docstring = parse_docstring(inspect.getdoc(tool))
+    # We need tool and parameter descriptions to pass to the agent
+    assert (
+        docstring.short_description is not None
+    ), "Tool must have a short description in the docstring"
+    for param in list(inspect.signature(tool).parameters.keys()):
+        assert param in [
+            docstring_param.arg_name for docstring_param in docstring.params
+        ], f"Parameter {param} must be documented in the docstring"
+    assert [
+        docstring_param.description != "" for docstring_param in docstring.params
+    ], "All tool parameters must have a description"
+    return docstring
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/model/_util.py` & `inspect_ai-0.3.3/src/inspect_ai/model/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from inspect_ai._util.constants import DEFAULT_MAX_RETRIES
 from inspect_ai._util.retry import httpx_should_retry, log_retry_attempt
 
 from ._model import (
     ChatMessage,
     GenerateConfig,
 )
-from ._tool import ToolDef
+from ._tool import ToolInfo
 
 
 async def chat_api_request(
     client: httpx.AsyncClient,
     model_name: str,
     url: str,
     headers: dict[str, Any],
@@ -101,22 +101,22 @@
     type: Literal["function"]
     """Tool type (currently only function is supported)"""
 
     function: ChatApiFunction
     """Type information for function to be called"""
 
 
-def chat_api_tool(tool: ToolDef) -> ChatApiTool:
+def chat_api_tool(tool: ToolInfo) -> ChatApiTool:
     """JSON schema definition for a tool to be called by the model.
 
     Both OpenAI and Mistral use JSON schema for their tool definition
     (others will likely follow suit).
 
     Args:
-       tool (ToolDef): Tool definition
+       tool (ToolInfo): Tool definition
 
     Returns:
        Name and JSON schema for tool parameters and return value.
     """
     # build params
     properties: dict[str, Any] = {}
     required: list[str] = []
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/scorer/_answer.py` & `inspect_ai-0.3.3/src/inspect_ai/scorer/_answer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/scorer/_match.py` & `inspect_ai-0.3.3/src/inspect_ai/scorer/_match.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
           equal to the target (module whitespace, etc.)
        ignore_case (bool): Do case insenstive comparison.
        numeric (bool): Is this a numeric match? (in this
           case different punctuation removal rules are
           used and numbers are normalized before comparisoin).
     """
 
-    def check(value: str, target: str) -> bool:
+    def check(value: str, target: str) -> tuple[str, bool]:
         return match_str(
             value=value,
             target=target,
             location=location,
             ignore_case=ignore_case,
             numeric=numeric,
         )
@@ -42,15 +42,15 @@
     """Check whether the specified text is included in the model output.
 
     Args:
        ignore_case (bool): Use a case insensitive comparison.
 
     """
 
-    def check(value: str, target: str) -> bool:
+    def check(value: str, target: str) -> tuple[str, bool]:
         if ignore_case:
             idx = value.lower().rfind(target.lower())
         else:
             idx = value.rfind(target)
-        return idx != -1
+        return value, idx != -1
 
     return str_match_scorer(check)
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/scorer/_metric.py` & `inspect_ai-0.3.3/src/inspect_ai/scorer/_metric.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from logging import getLogger
 from typing import (
     Any,
     Callable,
     Protocol,
     TypeVar,
     Union,
     cast,
@@ -15,23 +16,28 @@
     RegistryInfo,
     registry_add,
     registry_create,
     registry_name,
     registry_tag,
 )
 
+logger = getLogger(__name__)
+
 CORRECT = "C"
 """Value to assign for correct answers."""
 
 INCORRECT = "I"
 """Value to assing for incorrect answers."""
 
 PARTIAL = "P"
 """Value to assign for partial credit."""
 
+NOANSWER = "N"
+"""Value to assign for no answer or refusal to answer."""
+
 
 Value = Union[
     str | int | float | bool,
     list[str | int | float | bool],
     dict[str, str | int | float | bool],
 ]
 """Value provided by a score.
@@ -42,23 +48,27 @@
 
 
 class Score(BaseModel):
     """Score generated by a scorer.
 
     Args:
        value (Value): Score value.
-       explanation (str | None): Optional explanation of score.
-       metadata (dict[str,Any]): Additional metadata related to the score
+       answer (str | None): Answer extracted from model output (optional).
+       explanation (str | None): Explanation of score (optional).
+       metadata (dict[str,Any]): Additional metadata related to the score.
     """
 
     value: Value
     """Score value."""
 
-    explanation: str | None = None
-    """Optional explanation of score."""
+    answer: str | None = Field(default=None)
+    """Answer extracted from model output (optional)"""
+
+    explanation: str | None = Field(default=None)
+    """Explanation of score (optional)."""
 
     metadata: dict[str, Any] | None = Field(default=None)
     """Additional metadata related to the score"""
 
     @property
     def text(self) -> str:
         """Read the score as text."""
@@ -88,14 +98,59 @@
             or isinstance(self.value, bool)
         ):
             return self.value
         else:
             raise ValueError("This score is not a scalar")
 
 
+ValueToFloat = Callable[[Value], float]
+"""Function used by metrics to translate from a Score value to a float value."""
+
+
+def value_to_float(
+    correct: Value = CORRECT,
+    incorrect: Value = INCORRECT,
+    partial: Value = PARTIAL,
+    noanswer: Value = NOANSWER,
+) -> ValueToFloat:
+    """Create a ValueToFloat function.
+
+    Create a ValueToFloat function that maps string values of
+    the form "C", "I", "P", and "N" to 1, 0, 0.5, and 0
+    (respectively). Note that those are the default literal
+    values, but they can be customized. Numeric values are
+    cast to float. Arrays and dictionaries give a warning
+    and return 0.
+
+    Args:
+       correct (Value): Value that represents a correct answer (1)
+       incorrect (Value): Value that represents an incorrect answer (0)
+       partial (Value): Value to assign partial credit for (0.5)
+       noanswer (Value): Value for refusals to answer (0)
+
+    Returns:
+        ValueToFloat function.
+    """
+
+    def to_float(value: Value) -> float:
+        if isinstance(value, (int, float, bool)):
+            return float(value)
+        elif value == correct:
+            return 1.0
+        elif value == partial:
+            return 0.5
+        elif value == incorrect or value == noanswer:
+            return 0
+        else:
+            logger.warning(f"Unable to convert value to float: {value}")
+            return 0
+
+    return to_float
+
+
 @runtime_checkable
 class Metric(Protocol):
     r"""Evaluate scores using a metric.
 
     Args:
         scores (list[dict]): List of scores.
 
@@ -168,33 +223,14 @@
     r"""Decorator for registering metrics.
 
     Args:
         name: (str | MetricType):
             Optional name for metric. If the decorator has no name
             argument then the name of the underlying MetricType
             will be used to automatically assign a name.
-
-    Returns:
-        Metric with registry attributes.
-
-    Exmaples:
-
-        @metric
-        def accuracy(correct: str = "C") -> Metric:
-            def metric(scores: list[dict]) -> int | float:
-                ...
-            return metric
-
-        @metric
-        class Accuracy(Metric):
-            def __init__(self, correct: str = "C") -> None:
-                self.correct = correct
-
-            def __call__(self, scores: list[dict]) -> int | float:
-                ...
     """
 
     # create_metric_wrapper:
     #  (a) Add the MetricType to the registry using the appropriately
     #      package-namespaced name
     #  (b) Ensure that instances of Metric created by MetricType also
     #      carry registry info.
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/scorer/_metrics/accuracy.py` & `inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/accuracy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 from logging import getLogger
 
-from .._metric import CORRECT, INCORRECT, PARTIAL, Metric, Score, Value, metric
+from .._metric import (
+    Metric,
+    Score,
+    ValueToFloat,
+    metric,
+    value_to_float,
+)
 
 logger = getLogger(__name__)
 
 
 @metric
-def accuracy(
-    correct: Value = CORRECT,
-    incorrect: Value = INCORRECT,
-    partial: Value | None = PARTIAL,
-) -> Metric:
+def accuracy(to_float: ValueToFloat = value_to_float()) -> Metric:
     r"""Compute proportion of total answers which are correct.
 
     Args:
-        correct (Value): Value that represents a correct answer.
-        incorrect (Value): Value that represents an incorrect answer.
-        partial (Value): Value to assign partial credit for
+      to_float (ValueToFloat): Function for mapping
+        Value to float for computing metrics. The default
+        `value_to_float()` maps CORRECT ("C") to 1.0,
+        INCORRECT ("I") to 0, PARTIAL ("P") to 0.5, and
+        NOANSWER ("N") to 0, casts numeric values to
+        float directly, and prints a warning and returns
+        0 if the Value is a complex object (list or dict).
 
     Returns:
        Accuracy metric
     """
 
     def metric(scores: list[Score]) -> float:
-        total_correct = 0.0
-        total = float(len(scores))
+        total = 0.0
         for item in scores:
-            if item.value == correct:
-                total_correct += 1
-            elif item.value == partial:
-                total_correct += 0.5
-            elif item.value != incorrect:
-                logger.warning(
-                    "Unexpected item value for accuracy metric: {item.value}"
-                )
-        return total_correct / total
+            total += to_float(item.value)
+        return total / float(len(scores))
 
     return metric
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/scorer/_metrics/mean.py` & `inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/mean.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/scorer/_metrics/std.py` & `inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/std.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,45 @@
 from logging import getLogger
 from typing import cast
 
 import numpy as np
 
-from .._metric import CORRECT, INCORRECT, PARTIAL, Metric, Score, Value, metric
+from .._metric import (
+    Metric,
+    Score,
+    ValueToFloat,
+    metric,
+    value_to_float,
+)
 
 logger = getLogger(__name__)
 
 
 @metric
 def bootstrap_std(
-    num_samples: int = 1000,
-    correct: Value = CORRECT,
-    incorrect: Value = INCORRECT,
-    partial: Value | None = PARTIAL,
+    num_samples: int = 1000, to_float: ValueToFloat = value_to_float()
 ) -> Metric:
     """Standard deviation of a bootstrapped estimate of the mean.
 
     Args:
        num_samples (int): Number of bootstrap samples to take.
-       correct (Value): Value to compare against.
-       incorrect (Value): Value that represents an incorrect answer.
-       partial (Value): Value to assign partial credit for.
+       to_float (ValueToFloat): Function for mapping
+         Value to float for computing metrics. The default
+         `value_to_float()` maps CORRECT ("C") to 1.0,
+         INCORRECT ("I") to 0, PARTIAL ("P") to 0.5, and
+         NOANSWER ("N") to 0, casts numeric values to
+         float directly, and prints a warning and returns
+         0 if the Value is a complex object (list or dict).
 
     Returns:
        bootstrap_std metric
     """
 
-    def as_float(score: Score) -> float:
-        if isinstance(score.value, (int, float, bool)):
-            return float(score.value)
-        elif score.value == correct:
-            return 1.0
-        elif score.value == partial:
-            return 0.5
-        elif score.value == incorrect:
-            return 0
-        else:
-            logger.warning(
-                "Unexpected item value for bootstrap_std metric: {item.value}"
-            )
-            return 0
-
     def metric(scores: list[Score]) -> float:
-        values = [as_float(score) for score in scores]
+        values = [to_float(score.value) for score in scores]
         std = np.std(
             [
                 np.mean(np.random.choice(values, len(values), replace=True))
                 for _ in range(num_samples)
             ]
         )
         return cast(float, std.item())
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/scorer/_pattern.py` & `inspect_ai-0.3.3/src/inspect_ai/scorer/_pattern.py`

 * *Files 27% similar despite different names*

```diff
@@ -27,27 +27,29 @@
         # extract the answer
         match = re.search(
             pattern, state.output.completion, re.IGNORECASE if ignore_case else 0
         )
 
         # got a match
         if match:
-            # handle case insentive
-            match.groups
-            input = match.group(1) if len(match.groups()) == 1 else match.group(2)
+            # handle case insentitive
+            answer = match.group(1) if len(match.groups()) == 1 else match.group(2)
+            input = answer
             if ignore_case:
                 input = input.lower()
                 target = Target([t.lower() for t in target])
 
             # return score
             return Score(
                 value=CORRECT if input in target else INCORRECT,
+                answer=answer,
                 explanation=state.output.completion,
             )
         # didn't find the scoring pattern
         else:
             return Score(
                 value=INCORRECT,
-                explanation=f"Scoring pattern not matched in output: {state.output.completion}",
+                explanation="Scoring pattern not matched in output: "
+                + f"{state.output.completion}",
             )
 
     return score
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/scorer/_scorer.py` & `inspect_ai-0.3.3/src/inspect_ai/scorer/_scorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         scorer_name = registry_name(
             scorer_type, name if name else getattr(scorer_type, "__name__")
         )
 
         # wrap instatiations of scorer so they carry registry info and metrics
         def scorer_wrapper(*args: Any, **kwargs: Any) -> Scorer:
             scorer = scorer_type(*args, **kwargs)
+
             registry_tag(
                 scorer_type,
                 scorer,
                 RegistryInfo(
                     type="scorer",
                     name=scorer_name,
                     metadata={SCORER_METRICS: metrics} | metadata,
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/solver/__init__.py` & `inspect_ai-0.3.3/src/inspect_ai/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/solver/_critique.py` & `inspect_ai-0.3.3/src/inspect_ai/solver/_critique.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,41 +65,35 @@
         # regenerate
         return await generate(state)
 
     return solve
 
 
 DEFAULT_CRITIQUE_TEMPLATE = r"""
-Given the following question and answer, please critique the answer. A good answer
-comprehensively answers the question and NEVER refuses to answer. If the answer
-is already correct do not provide critique - simply respond 'The original answer
-is fully correct'.
+Given the following question and answer, please critique the answer. A good answer comprehensively answers the question and NEVER refuses to answer. If the answer is already correct do not provide critique - simply respond 'The original answer is fully correct'.
 
 [BEGIN DATA]
 ***
 [Question]: {question}
 ***
 [Answer]: {completion}
 ***
 [END DATA]
 
 Critique: """
 
 
 DEFAULT_CRITIQUE_COMPLETION_TEMPLATE = r"""
-Given the following question, initial answer and critique please generate
-an improved answer to the question:
+Given the following question, initial answer and critique please generate an improved answer to the question:
 
 [BEGIN DATA]
 ***
 [Question]: {question}
 ***
 [Answer]: {completion}
 ***
 [Critique]: {critique}
 ***
 [END DATA]
 
-If the original answer is already correct, just repeat the original answer exactly.
-You should just provide your answer to the question in exactly this format:
-
-Answer: <your answer> """
+If the original answer is already correct, just repeat the original answer exactly. Provide your answer at the end on its own line in the form "ANSWER: $ANSWER" (without quotes) where $ANSWER is the answer to the question.
+"""
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/solver/_multiple_choice.py` & `inspect_ai-0.3.3/src/inspect_ai/solver/_multiple_choice.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,86 +10,89 @@
 from ._solver import Generate, Solver, TaskState, solver
 
 logger = logging.getLogger(__name__)
 
 # this template is based on the multiple choice template in openai simple evals:
 # https://github.com/openai/simple-evals/blob/main/mmlu_eval.py
 
+
 MULTIPLE_CHOICE_TEMPLATE = r"""
-Answer the following multiple choice question. The entire content of your
-response should be of the following format: 'ANSWER: $LETTER' (without quotes)
-where LETTER is one of {letters}. {instructions}
+Answer the following multiple choice question. The entire content of your response should be of the following format: 'ANSWER: $LETTER' (without quotes) where LETTER is one of {letters}.
 
 {question}
 
 {choices}
 """.strip()
 
-# default cot instructions
-COT_INSTRUCTIONS = "Think step by step before answering."
+
+MULTIPLE_CHOICE_TEMPLATE_COT = r"""
+Answer the following multiple choice question. The last line of your response should be of the following format: 'ANSWER: $LETTER' (without quotes) where LETTER is one of {letters}. Think step by step before answering.
+
+{question}
+
+{choices}
+"""
+
 
 # max tokens for differnet variations
 MULTIPLE_CHOICE_MAX_TOKENS = 32
-MULTIPLE_CHOICE_MAX_TOKENS_COT = 512
+MULTIPLE_CHOICE_MAX_TOKENS_COT = 1024
 
 
 @solver
 def multiple_choice(
     *,
     cot: bool = False,
-    instructions: str | None = None,
     template: str | None = None,
     max_tokens: int | None = None,
     shuffle: bool | Random = False,
     answer_pattern: str | None = None,
 ) -> Solver:
     """Multiple choice question solver.
 
     Formats a multiple choice question prompt, then calls `generate()`
     (so you don't need to call `generate()` separately after this solver runs).
 
     The `template` and `max_tokens` parameters have defaults that vary based
-    tbased on whether `cot` is `True`. When NOT using chain of thought,
-    `max_tokens` is set to 32 (otherwise it is set to 512). If you provide your
+    on whether `cot` is `True`. When NOT using chain of thought,
+    `max_tokens` is set to 32 (otherwise it is set to 1024). If you provide your
     own template, you will also need to determine an appropriate value for
     `max_tokens` (as well as `answer_pattern` if `shuffle` is `True`).
 
     If shuffling is requested, then the choices will be presented in random order,
     and the model output mapped back to the correct choices from the dataset.
     When shuffling is enabled, you must also provide an `answer_pattern` that
     allows this substitution to find the answer in the model output.
 
     Args:
         cot (bool): `True` to use chain of thought prompting (defaults to `False`).
-          Note that using chain of thought will be slower and use many more tokens,
+          Note that using chain of thought will be slower and use more tokens,
           so you should assess carefully whether your eval benefits from it or not.
-        instructions (str | None): Instructions to append to the first part
-          of the mutliple choice prompt (note when `cot=True` this defaults to
-          "Think step by step before answering.")
-        template (str | None): Alternate prompt template for uestions/answers.
-          Templates have 4 variables: `letters`, `instructions`, `question`,
-          and `choices (where letters is e.g. 'ABCD').
+        template (str | None): Alternate prompt template for questions/answers.
+          Templates have 3 variables: `letters`, `question`, and `choices
+          (where letters is e.g. 'ABCD').
         max_tokens (int | None): Maximum number of tokens to output.
         shuffle (Random | None): Present answers in a shuffled order (defaults to
           `False`, pass `True` or an instance of `Random` to shuffle)
         answer_pattern (str | None): Regex used to find the answer letter. This is
           only used when `shuffle` is enabled. The regex should have 3 capture groups
          (before the answer, the answer, and after the answer). If the answer is
          expected at the beginning or end then you can use explicit capture groups
          for beginning or end of string, for example (^.*) or (.*$).
     """
     # resolve parameters
-    instructions = instructions if instructions else COT_INSTRUCTIONS if cot else ""
-    template = template if template else MULTIPLE_CHOICE_TEMPLATE
+    template = (
+        template
+        if template
+        else MULTIPLE_CHOICE_TEMPLATE_COT if cot else MULTIPLE_CHOICE_TEMPLATE
+    )
     max_tokens = (
         max_tokens
         if max_tokens
-        else MULTIPLE_CHOICE_MAX_TOKENS_COT
-        if cot
-        else MULTIPLE_CHOICE_MAX_TOKENS
+        else MULTIPLE_CHOICE_MAX_TOKENS_COT if cot else MULTIPLE_CHOICE_MAX_TOKENS
     )
     answer_pattern = answer_pattern if answer_pattern else ANSWER_PATTERN_LETTER
 
     # resolve template contents
     template = resource(template)
 
     # resolve shuffle
@@ -106,26 +109,24 @@
 
         # build choices str, key, and prompt
 
         # unshuffled version (this is what we'll write into history)
         choices_str, _ = make_choices(choices=state.choices)
         user_prompt_text = template.format(
             letters=letters,
-            instructions=instructions,
             question=state.user_prompt.text,
             choices=choices_str,
         )
 
         # shuffled version (this is what we'll present to the model)
         choices_str_shuffled, choices_key = make_choices(
             choices=state.choices, shuffle=shuffle if shuffle else None
         )
         state.user_prompt.text = template.format(
             letters=letters,
-            instructions=instructions,
             question=state.user_prompt.text,
             choices=choices_str_shuffled,
         )
 
         # generate
         state = await generate(state, max_tokens=max_tokens)
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/solver/_plan.py` & `inspect_ai-0.3.3/src/inspect_ai/solver/_plan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 import inspect
-from typing import Any, Callable, TypeVar, cast
+from typing import Any, Awaitable, Callable, TypeVar, cast
 
 from inspect_ai._util.registry import (
     RegistryInfo,
     is_registry_object,
     registry_add,
     registry_create,
     registry_info,
     registry_name,
     registry_tag,
 )
 
-from ._solver import Solver
+from ._solver import Solver, TaskState
 
 
 class Plan:
     """Task plan: List of solvers with an optional finishing solver.
 
-    The finishing solver is called after executing the steps
-    (including in the case where the steps were exited early
-    due to `TaskState.completed = True` or `max_messages`)
+    The optional `finish` solver is called after executing the steps (including in the case
+    where the steps were exited early due to `TaskState.completed = True` or `max_messages`).
+
+    The optional `cleanup` function is called when the plan is complete (even if the plan
+    is terminated due to an exception).
     """
 
     def __init__(
         self,
         steps: Solver | list[Solver],
         finish: Solver | None = None,
+        cleanup: Callable[[TaskState], Awaitable[None]] | None = None,
         name: str | None = None,
     ) -> None:
         """Create a task plan.
 
         Args:
           steps (list[Solver]): Solvers to run for this plan.
           finish (Solver | None): Finishing solver that is always run even for early exit.
+            Note that this solver is NOT run when exception are thrown (use `cleanup` for this)
+          cleanup (Callable[[TaskState], Awaitable[None]] | None): Optional cleanup handler that
+            is called at the end (even if an exception occurs). Note that this function takes
+            a `TaskState` but does not return one (it is only for cleanup not for transforming
+            the state).
           name (str | None): Optional name for plan (for log files).
         """
         if isinstance(steps, Solver):
             self.steps = [steps]
         else:
             self.steps = steps
 
         self.finish = finish
+        self.cleanup = cleanup
         self._name = name
 
     @property
     def name(self) -> str:
         if self._name is not None:
             return self._name
         elif is_registry_object(self):
@@ -54,14 +63,22 @@
 
     steps: list[Solver]
     """Solvers to run for this plan."""
 
     finish: Solver | None = None
     """Finishing sover that is always run even for early exit."""
 
+    cleanup: Callable[[TaskState], Awaitable[None]] | None = None
+    """Function  called at the end of the plan (even if an exception occurs).
+
+    Note that this function takes a `TaskState` but does not return one
+    (it is only for cleanup not for transforming the state). Note also that
+    this function should be declared `async`.
+    """
+
 
 PlanType = TypeVar("PlanType", bound=Callable[..., Plan])
 
 
 def plan(*plan: PlanType | None, name: str | None = None, **attribs: Any) -> Any:
     r"""Decorator for registering plans.
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/solver/_prompt.py` & `inspect_ai-0.3.3/src/inspect_ai/solver/_prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,26 +56,20 @@
 
     return solve
 
 
 DEFAULT_COT_TEMPLATE = r"""
 {prompt}
 
-Before answering, reason in a step-by-step manner as to get the right answer.
-Then print only the text corresponding to the correct answer (without quotes
-or punctuation) on its own line. At the end, repeat just the value of the
-answer again by itself on a new line.
+Before answering, reason in a step-by-step manner as to get the right answer. Provide your answer at the end on its own line in the form "ANSWER: $ANSWER" (without quotes) where $ANSWER is the answer to the question.
 """
 
 
 @solver
 def chain_of_thought(template: str = DEFAULT_COT_TEMPLATE) -> Solver:
     """Solver which modifies the user prompt to encourage chain of thought.
 
-    Modification is doing using a template. Pass the `template` argument
-    to provide your own template.
-
     Args:
        template (str): String or path to file containing CoT template.
           The template uses a single variable: `prompt`.
     """
     return prompt_template(template)
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/solver/_solver.py` & `inspect_ai-0.3.3/src/inspect_ai/solver/_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,29 @@
 from inspect_ai.model import (
     ChatMessage,
     ChatMessageUser,
     GenerateConfigArgs,
     ModelName,
     ModelOutput,
     ToolChoice,
-    ToolDef,
 )
 
+from ._tool.tool import Tool
+
 
 class TaskState:
     def __init__(
         self,
         model: ModelName,
         sample_id: int | str,
         epoch: int,
         input: str | list[ChatMessage],
         choices: list[str] | None,
         messages: list[ChatMessage],
-        tools: list[ToolDef] = [],
+        tools: list[Tool] = [],
         tool_choice: ToolChoice | None = None,
         output: ModelOutput | None = None,
         completed: bool = False,
         metadata: dict[str, Any] = {},
     ) -> None:
         self._model = model
 
@@ -255,14 +256,15 @@
     ) -> SolverType:
         solver_name = registry_name(
             solver_type, name if name else getattr(solver_type, "__name__")
         )
 
         def solver_wrapper(*args: Any, **kwargs: dict[str, Any]) -> Solver:
             solver = solver_type(*args, **kwargs)
+
             registry_tag(
                 solver_type,
                 solver,
                 RegistryInfo(type="solver", name=solver_name),
                 *args,
                 **kwargs,
             )
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/solver/_tool/tool.py` & `inspect_ai-0.3.3/src/inspect_ai/solver/_tool/tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from typing import (
     Any,
     Callable,
     Protocol,
     Tuple,
     TypeVar,
     cast,
@@ -10,15 +11,14 @@
 
 from inspect_ai._util.registry import (
     RegistryInfo,
     registry_add,
     registry_name,
     registry_tag,
 )
-from inspect_ai.model._tool import TOOL_PARAMS, TOOL_PROMPT
 
 ToolResult = str | int | float | bool | Tuple[str | int | float | bool, dict[str, Any]]
 
 
 @runtime_checkable
 class Tool(Protocol):
     async def __call__(
@@ -98,14 +98,18 @@
                 return execute
 
             ```
 
     Returns:
         Tool with registry attributes.
     """
+    # remove spurous spacing from prompt (can occur if a multline string
+    # is used to specify the prompt)
+    if prompt:
+        prompt = re.sub(r"\s+", " ", prompt)
 
     def wrapper(tool_type: ToolType) -> ToolType:
         # determine the name (explicit or implicit from object)
         tool_name = registry_name(
             tool_type, name if name else getattr(tool_type, "__name__")
         )
 
@@ -125,7 +129,11 @@
             )
             return tool
 
         # register the scorer
         return tool_register(cast(ToolType, tool_wrapper), tool_name)
 
     return wrapper
+
+
+TOOL_PROMPT = "prompt"
+TOOL_PARAMS = "params"
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/solver/_tool/use_tools.py` & `inspect_ai-0.3.3/src/inspect_ai/solver/_tool/use_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     ChatMessageSystem,
     ToolChoice,
 )
 
 from .._solver import Generate, Solver, TaskState, solver
 from .._util import append_system_message
 from .tool import Tool
-from .tool_def import tool_def
+from .tool_def import tool_defs
 
 
 @solver
 def use_tools(
     tools: Tool | list[Tool] | None = None, tool_choice: ToolChoice = "auto"
 ) -> Solver:
     """
@@ -22,24 +22,24 @@
           tools the model should use.
 
     Returns:
         A solver that injects the tools and tool_choice into the task state.
     """
     # create tool defs
     tools = tools if isinstance(tools, list) else [tools] if tools else None
-    tool_defs = [tool_def(tool) for tool in tools] if tools else None
+    tdefs = tool_defs(tools) if tools else None
 
     async def solve(state: TaskState, generate: Generate) -> TaskState:
         # register the tools
-        if tool_defs:
-            state.tools.extend(tool_defs)
+        if tools and tdefs:
+            state.tools.extend(tools)
 
             # append the tools system prompts. mark the 'source' of messages
             # as tool so they can be removed if tool_choice == "none"
-            for tool in tool_defs:
+            for tool in tdefs:
                 if tool.prompt:
                     append_system_message(
                         state.messages,
                         ChatMessageSystem(content=tool.prompt, tool=tool.name),
                     )
 
         # set tool choice (note you can call this function w/o tools
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/solver/_tool/web_search.py` & `inspect_ai-0.3.3/src/inspect_ai/solver/_tool/web_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             for page, link in zip(pages, links):
                 if page and not isinstance(page, Exception):
                     page_contents.append(cast(str, page))
                     urls.append(link.url)
                     snippets.append(link.snippet)
             search_calls += 1
 
-        all_page_contents = "\n".join(page_contents)
+        all_page_contents = "\n\n".join(page_contents)
         if all_page_contents == "":
             response = "I'm sorry, I couldn't find any relevant information on the web."
         else:
             response = (
                 "Here are your web search results. Please read them carefully as they may be useful later! "
                 + all_page_contents
             )
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai/util/_context/concurrency.py` & `inspect_ai-0.3.3/src/inspect_ai/util/_context/concurrency.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/util/_context/logger.py` & `inspect_ai-0.3.3/src/inspect_ai/util/_context/logger.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/util/_context/resource.py` & `inspect_ai-0.3.3/src/inspect_ai/util/_context/resource.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai/util/_context/subprocess.py` & `inspect_ai-0.3.3/src/inspect_ai/util/_context/subprocess.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/src/inspect_ai.egg-info/PKG-INFO` & `inspect_ai-0.3.3/src/inspect_ai.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 Metadata-Version: 2.1
 Name: inspect_ai
-Version: 0.3.2
-Summary: Language model evaluations
+Version: 0.3.3
+Summary: Framework for large language model evaluations
+Author: UK AI Safety Institute
 License: MIT License
+Project-URL: Documentation, https://UKGovernmentBEIS.github.io/inspect_ai/
+Project-URL: Source Code, https://github.com/UKGovernmentBEIS/inspect_ai
+Project-URL: Issue Tracker, https://github.com/UKGovernmentBEIS/inspect_ai/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -20,53 +24,78 @@
 Requires-Dist: debugpy
 Requires-Dist: fsspec
 Requires-Dist: httpx
 Requires-Dist: numpy
 Requires-Dist: platformdirs
 Requires-Dist: python-dotenv
 Requires-Dist: jsonlines
+Requires-Dist: json-stream
 Requires-Dist: nest_asyncio
 Requires-Dist: pydantic>=2
 Requires-Dist: s3fs>=2023
 Requires-Dist: semver
 Requires-Dist: shortuuid
 Requires-Dist: tenacity
 Requires-Dist: beautifulsoup4
 Requires-Dist: docstring-parser
 Requires-Dist: typing_extensions
 Requires-Dist: pyyaml
 Requires-Dist: rich
+Requires-Dist: psutil
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-dotenv; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Requires-Dist: types-botocore; extra == "dev"
 Requires-Dist: types-boto3; extra == "dev"
 Requires-Dist: types-beautifulsoup4; extra == "dev"
 Requires-Dist: types-protobuf; extra == "dev"
+Requires-Dist: types-psutil; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: openai; extra == "dev"
 Requires-Dist: anthropic; extra == "dev"
 Requires-Dist: google-cloud-aiplatform; extra == "dev"
 Requires-Dist: google-generativeai; extra == "dev"
 Requires-Dist: mistralai; extra == "dev"
 Requires-Dist: boto3; extra == "dev"
 Requires-Dist: transformers; extra == "dev"
 Requires-Dist: torch; extra == "dev"
+Requires-Dist: datasets; extra == "dev"
 Requires-Dist: langchain; extra == "dev"
 Requires-Dist: langchainhub; extra == "dev"
+Requires-Dist: wikipedia; extra == "dev"
 Requires-Dist: ipywidgets; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: nbformat; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: quarto-cli; extra == "doc"
 Provides-Extra: dist
 Requires-Dist: twine; extra == "dist"
 Requires-Dist: build; extra == "dist"
 
-Language model evaluations
+[<img width="295" src="https://ukgovernmentbeis.github.io/inspect_ai/images/aisi-logo.png" />](https://www.gov.uk/government/organisations/ai-safety-institute)
+
+Welcome to Inspect, a framework for large language model evaluations created by the [UK AI Safety Institute](https://www.gov.uk/government/organisations/ai-safety-institute).
+
+Inspect provides many built-in components, including facilities for prompt engineering, tool usage, multi-turn dialog, and model graded evaluations. Extensions to Inspect (e.g. to support new elicitation and scoring techniques) can be provided by other Python packages.
+
+To get started with Inspect, please see the documentation at <https://UKGovernmentBEIS.github.io/inspect_ai/>.
+
+***
+
+#### Development
+
+To work on development of Inspect, clone the repository and install with the `-e` flag and `[dev]` optional dependencies:
+
+```         
+$ git clone https://github.com/UKGovernmentBEIS/inspect_ai.git
+$ cd inspect_ai
+$ pip install -e ".[dev]"
+```
+
+If you use VS Code, you should be sure to have installed the recommended extensions (Python, Ruff, and MyPy). Note that you'll be promoted to install these when you open the project in VS Code.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai.egg-info/SOURCES.txt` & `inspect_ai-0.3.3/src/inspect_ai.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
-DESCRIPTION.md
+CHANGELOG.md
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 .github/dependabot.yml
 .github/pull_request_template.md
 .github/workflows/build.yml
@@ -27,53 +27,64 @@
 docs/_variables.yml
 docs/datasets.qmd
 docs/eval-logs.qmd
 docs/eval-suites.qmd
 docs/eval-tuning.qmd
 docs/examples.qmd
 docs/index.qmd
+docs/log-viewer.qmd
 docs/models.qmd
 docs/scorers.qmd
 docs/solvers.qmd
 docs/theme.scss
 docs/tools.qmd
 docs/workflow.qmd
 docs/_examples/arc.qmd
-docs/_examples/bias_detection.qmd
 docs/_examples/biology_qa.qmd
 docs/_examples/footer.qmd
 docs/_examples/gsm8k.qmd
 docs/_examples/hellaswag.qmd
 docs/_examples/index.qmd
 docs/_examples/mathematics.qmd
 docs/_examples/popularity.qmd
 docs/_examples/security_guide.qmd
 docs/_examples/theory_of_mind.qmd
 docs/_examples/tool_use.qmd
-docs/_format/post-render.py
 docs/_format/pre-render.sh
 docs/images/aisi-logo.png
 docs/images/eval-log.png
+docs/images/inspect-view-answers.png
+docs/images/inspect-view-filter.png
+docs/images/inspect-view-history.png
+docs/images/inspect-view-home.png
+docs/images/inspect-view-info.png
+docs/images/inspect-view-logging-console.png
+docs/images/inspect-view-logging.png
+docs/images/inspect-view-main.png
+docs/images/inspect-view-messages.png
+docs/images/inspect-view-metadata.png
+docs/images/inspect-view-scoring.png
+docs/images/inspect-view-sort.png
 docs/images/popularity.png
 docs/images/rate-limit.png
 docs/images/running-theory.png
-examples/bias_detection.py
 examples/biology_qa.py
 examples/popularity.py
 examples/security_guide.py
 examples/theory_of_mind.py
 examples/tool_use.py
 examples/agents/langchain/.env.example
 examples/agents/langchain/.gitignore
 examples/agents/langchain/README.md
 examples/agents/langchain/inspect_langchain.py
 examples/agents/langchain/requirements.txt
 examples/agents/langchain/wikipedia.jsonl
 examples/agents/langchain/wikipedia.py
 src/inspect_ai/__init__.py
+src/inspect_ai/__main__.py
 src/inspect_ai/py.typed
 src/inspect_ai.egg-info/PKG-INFO
 src/inspect_ai.egg-info/SOURCES.txt
 src/inspect_ai.egg-info/dependency_links.txt
 src/inspect_ai.egg-info/entry_points.txt
 src/inspect_ai.egg-info/requires.txt
 src/inspect_ai.egg-info/top_level.txt
@@ -118,37 +129,83 @@
 src/inspect_ai/_util/samples.py
 src/inspect_ai/_util/text.py
 src/inspect_ai/_util/url.py
 src/inspect_ai/_util/version.py
 src/inspect_ai/_view/schema.py
 src/inspect_ai/_view/view.py
 src/inspect_ai/_view/www/.gitignore
-src/inspect_ai/_view/www/App.css
 src/inspect_ai/_view/www/App.mjs
-src/inspect_ai/_view/www/Log.mjs
 src/inspect_ai/_view/www/api.mjs
 src/inspect_ai/_view/www/favicon.svg
 src/inspect_ai/_view/www/index.html
 src/inspect_ai/_view/www/log-schema.json
 src/inspect_ai/_view/www/log.d.ts
 src/inspect_ai/_view/www/package-lock.json
 src/inspect_ai/_view/www/package.json
-src/inspect_ai/_view/www/bootstrap/css/bootstrap-icons.min.css
-src/inspect_ai/_view/www/bootstrap/css/bootstrap.min.css
-src/inspect_ai/_view/www/bootstrap/css/fonts/bootstrap-icons.woff
-src/inspect_ai/_view/www/bootstrap/css/fonts/bootstrap-icons.woff2
-src/inspect_ai/_view/www/bootstrap/js/bootstrap.bundle.min.js
+src/inspect_ai/_view/www/tools.js
+src/inspect_ai/_view/www/libs/clipboard.min.js
+src/inspect_ai/_view/www/libs/json5.min.js
+src/inspect_ai/_view/www/libs/purify.min.js
+src/inspect_ai/_view/www/libs/showdown.min.js
+src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css
+src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css
+src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff
+src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2
+src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js
+src/inspect_ai/_view/www/libs/prism/prism-dark.css
+src/inspect_ai/_view/www/libs/prism/prism.min.css
+src/inspect_ai/_view/www/libs/prism/prism.min.js
 src/inspect_ai/_view/www/preact/hooks.js
 src/inspect_ai/_view/www/preact/preact-hooks.mjs
 src/inspect_ai/_view/www/preact/preact.mjs
 src/inspect_ai/_view/www/preact/htm/htm.mjs
 src/inspect_ai/_view/www/preact/htm/preact.js
 src/inspect_ai/_view/www/preact/htm/preact.mjs
-src/inspect_ai/_view/www/prism/prism.min.css
-src/inspect_ai/_view/www/prism/prism.min.js
+src/inspect_ai/_view/www/src/App.css
+src/inspect_ai/_view/www/src/Constants.mjs
+src/inspect_ai/_view/www/src/Register.mjs
+src/inspect_ai/_view/www/src/components/AnsiDisplay.css
+src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs
+src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs
+src/inspect_ai/_view/www/src/components/Card.mjs
+src/inspect_ai/_view/www/src/components/ChatView.mjs
+src/inspect_ai/_view/www/src/components/Dialog.mjs
+src/inspect_ai/_view/www/src/components/EmptyPanel.mjs
+src/inspect_ai/_view/www/src/components/ErrorPanel.mjs
+src/inspect_ai/_view/www/src/components/LabeledValue.mjs
+src/inspect_ai/_view/www/src/components/LoadingScreen.mjs
+src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs
+src/inspect_ai/_view/www/src/components/MessageContent.mjs
+src/inspect_ai/_view/www/src/components/MetaDataView.mjs
+src/inspect_ai/_view/www/src/components/RenderedContent.mjs
+src/inspect_ai/_view/www/src/components/TabSet.mjs
+src/inspect_ai/_view/www/src/components/ToolButton.mjs
+src/inspect_ai/_view/www/src/components/ansi-output.js
+src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs
+src/inspect_ai/_view/www/src/log-reader/Native-Log-Reader.mjs
+src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs
+src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs
+src/inspect_ai/_view/www/src/plan/PlanCard.mjs
+src/inspect_ai/_view/www/src/samples/SampleGroupSeparator.mjs
+src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs
+src/inspect_ai/_view/www/src/samples/SampleView.mjs
+src/inspect_ai/_view/www/src/samples/SamplesCard.mjs
+src/inspect_ai/_view/www/src/title/TitleBlock.mjs
+src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs
+src/inspect_ai/_view/www/src/usage/UsageCard.mjs
+src/inspect_ai/_view/www/src/utils/Format.mjs
+src/inspect_ai/_view/www/src/utils/Git.mjs
+src/inspect_ai/_view/www/src/utils/Path.mjs
+src/inspect_ai/_view/www/src/utils/Type.mjs
+src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs
+src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs
+src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs
+src/inspect_ai/_view/www/src/workspace/SortFilter.mjs
+src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs
+src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs
 src/inspect_ai/dataset/__init__.py
 src/inspect_ai/dataset/_dataset.py
 src/inspect_ai/dataset/_util.py
 src/inspect_ai/dataset/_examples/bias_detection.jsonl
 src/inspect_ai/dataset/_examples/biology_qa.jsonl
 src/inspect_ai/dataset/_examples/popularity.jsonl
 src/inspect_ai/dataset/_examples/security_guide.jsonl
@@ -227,15 +284,15 @@
 tests/test_tools.py
 tests/utils.py
 tests/test_dataset/samples.csv
 tests/test_dataset/samples.json
 tests/test_dataset/samples.jsonl
 tests/test_images/images.jsonl
 tests/test_task_list/__init__.py
-tests/test_task_list/attribs.py
+tests/test_task_list/attribs.ipynb
 tests/test_task_list/multiple.py
 tests/test_task_list/multiple_dir/_decoy2.py
 tests/test_task_list/multiple_dir/bar.py
 tests/test_task_list/multiple_dir/foo.py
 tests/test_task_list/multiple_dir/_decoy/testit.py
 tests/test_task_list/recurse/.folder3/epsilon.py
 tests/test_task_list/recurse/folder1/_decoy.py
```

### Comparing `inspect_ai-0.3.2/src/inspect_ai.egg-info/requires.txt` & `inspect_ai-0.3.3/src/inspect_ai.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 debugpy
 fsspec
 httpx
 numpy
 platformdirs
 python-dotenv
 jsonlines
+json-stream
 nest_asyncio
 pydantic>=2
 s3fs>=2023
 semver
 shortuuid
 tenacity
 beautifulsoup4
 docstring-parser
 typing_extensions
 pyyaml
 rich
+psutil
 
 [dev]
 ruff
 mypy
 pre-commit
 pytest
 pytest-asyncio
@@ -28,25 +30,28 @@
 pytest-dotenv
 pytest-xdist
 pandas-stubs
 types-botocore
 types-boto3
 types-beautifulsoup4
 types-protobuf
+types-psutil
 types-PyYAML
 openai
 anthropic
 google-cloud-aiplatform
 google-generativeai
 mistralai
 boto3
 transformers
 torch
+datasets
 langchain
 langchainhub
+wikipedia
 ipywidgets
 ipython
 nbformat
 
 [dist]
 twine
 build
```

### Comparing `inspect_ai-0.3.2/tests/test_anthropic.py` & `inspect_ai-0.3.3/tests/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/test_collapse_user_message.py` & `inspect_ai-0.3.3/tests/test_collapse_user_message.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/test_dataset.py` & `inspect_ai-0.3.3/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/test_images/images.jsonl` & `inspect_ai-0.3.3/tests/test_images/images.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/test_images.py` & `inspect_ai-0.3.3/tests/test_images.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 
 from inspect_ai import Task, eval, task
 from inspect_ai.dataset import json_dataset
 from inspect_ai.scorer import match
 from inspect_ai.solver import generate, system_message
 
 SYSTEM_MESSAGE = """
-For the following exercise, it is important that you answer with only a single
-word or numeric value in brackets. For example, [22] or [house]. Do not include
-any discussion, narrative, or rationale, just a single value in brackets.
+For the following exercise, it is important that you answer with only a single word or numeric value in brackets. For example, [22] or [house]. Do not include any discussion, narrative, or rationale, just a single value in brackets.
 """
 
 
 @task
 def images():
     return Task(
         dataset=json_dataset(os.path.join("tests", "test_images", "images.jsonl")),
```

### Comparing `inspect_ai-0.3.2/tests/test_list_task.py` & `inspect_ai-0.3.3/tests/test_list_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def test_task_list_multiple_dir():
     tasks = list_test_tasks_dir(["multiple_dir"])
     assert len(tasks) == 2
 
 
 def test_task_list_attribs():
-    tasks = list_test_tasks_dir(["attribs.py"])
+    tasks = list_test_tasks_dir(["attribs.ipynb"])
     assert tasks[0].attribs.get("light") is True
     assert tasks[0].attribs.get("type") == "bio"
 
 
 def test_task_list_filter():
     tasks = list_test_tasks_dir(["*"], filter=lambda t: t.attribs.get("type") == "bio")
     assert len(tasks) == 1
```

### Comparing `inspect_ai-0.3.2/tests/test_logprobs.py` & `inspect_ai-0.3.3/tests/test_logprobs.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/test_metric.py` & `inspect_ai-0.3.3/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/test_num_choices.py` & `inspect_ai-0.3.3/tests/test_num_choices.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/test_openai.py` & `inspect_ai-0.3.3/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/test_registry.py` & `inspect_ai-0.3.3/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/test_retry.py` & `inspect_ai-0.3.3/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/test_scorer.py` & `inspect_ai-0.3.3/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/test_solver.py` & `inspect_ai-0.3.3/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/test_stop_reason.py` & `inspect_ai-0.3.3/tests/test_stop_reason.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,37 @@
 import pytest
 from utils import (
-    addition,
     skip_if_no_anthropic,
     skip_if_no_mistral,
     skip_if_no_openai,
     skip_if_no_together,
 )
 
 from inspect_ai.model import GenerateConfig, ModelOutput, get_model
-from inspect_ai.solver._tool.tool_def import tool_def
 
 
 async def generate(model_name) -> ModelOutput:
     model = get_model(model_name)
     return await model.generate(input="Hello.")
 
 
-async def generate_tool(model_name) -> ModelOutput:
-    model = get_model(model_name)
-    return await model.generate(input="What is 1 + 1?", tools=[tool_def(addition())])
-
-
 async def generate_token_limit(model_name) -> ModelOutput:
     model = get_model(model_name)
     return await model.generate(
-        input="Tell me a story.", config=GenerateConfig(max_tokens=10)
+        input="Tell me a story.", config=GenerateConfig(max_tokens=2)
     )
 
 
-async def check_stop_reason(model_name, tool_calls: bool = True):
+async def check_stop_reason(model_name):
     response = await generate(model_name)
     assert response.choices[0].stop_reason == "stop"
 
     response = await generate_token_limit(model_name)
     assert response.choices[0].stop_reason == "length"
 
-    if tool_calls:
-        response = await generate_tool(model_name)
-        assert response.choices[0].stop_reason == "tool_calls"
-
 
 @pytest.mark.asyncio
 @skip_if_no_openai
 async def test_openai_stop_reason() -> None:
     await check_stop_reason("openai/gpt-3.5-turbo")
 
 
@@ -51,20 +40,14 @@
 async def test_anthropic_stop_reason() -> None:
     await check_stop_reason("anthropic/claude-3-haiku-20240307")
 
 
 @pytest.mark.asyncio
 @skip_if_no_mistral
 async def test_mistral_stop_reason() -> None:
-    await check_stop_reason("mistral/mistral-medium-latest", tool_calls=False)
+    await check_stop_reason("mistral/mistral-medium-latest")
 
 
 @pytest.mark.asyncio
 @skip_if_no_together
 async def test_together_stop_reason() -> None:
-    await check_stop_reason("together/google/gemma-2b-it", tool_calls=False)
-
-
-# @pytest.mark.asyncio
-# @skip_if_no_azureai
-# async def test_azureai_stop_reason() -> None:
-#     await check_stop_reason(None, tool_calls=False)
+    await check_stop_reason("together/google/gemma-2b-it")
```

### Comparing `inspect_ai-0.3.2/tests/test_subprocess.py` & `inspect_ai-0.3.3/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/test_tools.py` & `inspect_ai-0.3.3/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.2/tests/utils.py` & `inspect_ai-0.3.3/tests/utils.py`

 * *Files identical despite different names*

