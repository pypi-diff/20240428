# Comparing `tmp/talisman-tools-0.6.4.tar.gz` & `tmp/talisman-tools-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talisman-tools-0.6.4.tar", last modified: Wed Apr 24 13:53:25 2024, max compression
+gzip compressed data, was "talisman-tools-0.6.5.tar", last modified: Sat Apr 27 14:11:02 2024, max compression
```

## Comparing `talisman-tools-0.6.4.tar` & `talisman-tools-0.6.5.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.550465 talisman-tools-0.6.4/
--rw-r--r--   0 root         (0) root         (0)      713 2024-04-24 13:53:25.550465 talisman-tools-0.6.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 13:52:40.000000 talisman-tools-0.6.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-04-24 13:50:59.000000 talisman-tools-0.6.4/VERSION
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 13:53:25.550465 talisman-tools-0.6.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1665 2024-04-24 13:50:59.000000 talisman-tools-0.6.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.526465 talisman-tools-0.6.4/talisman_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 13:52:40.000000 talisman-tools-0.6.4/talisman_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.530465 talisman-tools-0.6.4/talisman_tools/arguments/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 13:52:40.000000 talisman-tools-0.6.4/talisman_tools/arguments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      676 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/arguments/domain.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/arguments/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/arguments/processor.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/arguments/reader.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/arguments/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.530465 talisman-tools-0.6.4/talisman_tools/commands/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.530465 talisman-tools-0.6.4/talisman_tools/commands/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/dataset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.530465 talisman-tools-0.6.4/talisman_tools/commands/dataset/commands/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/dataset/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.530465 talisman-tools-0.6.4/talisman_tools/commands/dataset/commands/convert/
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/dataset/commands/convert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/dataset/commands/convert/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/dataset/commands/subparsers.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/dataset/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.530465 talisman-tools-0.6.4/talisman_tools/commands/model/
--rw-rw-rw-   0 root         (0) root         (0)       82 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.530465 talisman-tools-0.6.4/talisman_tools/commands/model/commands/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.534465 talisman-tools-0.6.4/talisman_tools/commands/model/commands/check_performance/
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/check_performance/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2893 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/check_performance/action.py
--rw-rw-rw-   0 root         (0) root         (0)     1038 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/check_performance/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.534465 talisman-tools-0.6.4/talisman_tools/commands/model/commands/configure/
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/configure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/configure/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.534465 talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3605 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/action.py
--rw-rw-rw-   0 root         (0) root         (0)     4892 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/evaluation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.538465 talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/evaluators/
--rw-rw-rw-   0 root         (0) root         (0)      708 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/evaluators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/evaluators/disambiguation_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1821 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/evaluators/nerc.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/evaluators/relext.py
--rw-rw-rw-   0 root         (0) root         (0)     5278 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    15234 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1322 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.538465 talisman-tools-0.6.4/talisman_tools/commands/model/commands/process/
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/process/action.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/process/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/commands/subparsers.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/model/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.538465 talisman-tools-0.6.4/talisman_tools/commands/servers/
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.538465 talisman-tools-0.6.4/talisman_tools/commands/servers/arguments/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 13:52:40.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/arguments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/arguments/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.538465 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.542465 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/converter/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/converter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/converter/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.542465 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/converter/methods/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 13:52:40.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/converter/methods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2857 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/converter/methods/convert.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/converter/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.542465 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/loader/
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/loader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/loader/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.542465 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/loader/methods/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 13:52:40.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/loader/methods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/loader/methods/load.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/loader/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.542465 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/processor/
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/processor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1698 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/processor/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.542465 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/processor/methods/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 13:52:40.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/processor/methods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2571 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/processor/methods/process.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/processor/methods/update.py
--rw-rw-rw-   0 root         (0) root         (0)      927 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/processor/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/commands/subparsers.py
--rw-rw-rw-   0 root         (0) root         (0)      779 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     3064 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/servers/server_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/subparsers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.546465 talisman-tools-0.6.4/talisman_tools/commands/train/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 13:52:40.000000 talisman-tools-0.6.4/talisman_tools/commands/train/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/train/action.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/commands/train/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.546465 talisman-tools-0.6.4/talisman_tools/configure/
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/configure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5626 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/configure/configure.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/configure/wrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.546465 talisman-tools-0.6.4/talisman_tools/configure/wrapper/
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/configure/wrapper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1377 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/configure/wrapper/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.546465 talisman-tools-0.6.4/talisman_tools/helper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 13:52:40.000000 talisman-tools-0.6.4/talisman_tools/helper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/helper/concurrency.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/helper/env.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/helper/log_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/helper/multiprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/parser_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.550465 talisman-tools-0.6.4/talisman_tools/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     1159 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1840 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/plugin/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/plugin/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/plugin/domain.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/plugin/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/plugin/kb.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/plugin/processor.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/plugin/reader.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/plugin/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/plugin/trainer.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/plugin/wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)      942 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/plugin/wrapper_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      796 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/talisman.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2024-04-23 13:03:07.000000 talisman-tools-0.6.4/talisman_tools/talisman_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:25.526465 talisman-tools-0.6.4/talisman_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      713 2024-04-24 13:53:25.000000 talisman-tools-0.6.4/talisman_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4615 2024-04-24 13:53:25.000000 talisman-tools-0.6.4/talisman_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 13:53:25.000000 talisman-tools-0.6.4/talisman_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-24 13:53:25.000000 talisman-tools-0.6.4/talisman_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      312 2024-04-24 13:53:25.000000 talisman-tools-0.6.4/talisman_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-24 13:53:25.000000 talisman-tools-0.6.4/talisman_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.760741 talisman-tools-0.6.5/
+-rw-r--r--   0 root         (0) root         (0)      713 2024-04-27 14:11:02.760741 talisman-tools-0.6.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:45.000000 talisman-tools-0.6.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-04-27 14:10:37.000000 talisman-tools-0.6.5/VERSION
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 14:11:02.760741 talisman-tools-0.6.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2024-04-27 14:10:37.000000 talisman-tools-0.6.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.732740 talisman-tools-0.6.5/talisman_tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:45.000000 talisman-tools-0.6.5/talisman_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.736740 talisman-tools-0.6.5/talisman_tools/arguments/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:45.000000 talisman-tools-0.6.5/talisman_tools/arguments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      676 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/arguments/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/arguments/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/arguments/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/arguments/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/arguments/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.736740 talisman-tools-0.6.5/talisman_tools/commands/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.736740 talisman-tools-0.6.5/talisman_tools/commands/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/dataset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.740741 talisman-tools-0.6.5/talisman_tools/commands/dataset/commands/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/dataset/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.740741 talisman-tools-0.6.5/talisman_tools/commands/dataset/commands/convert/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/dataset/commands/convert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/dataset/commands/convert/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/dataset/commands/subparsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/dataset/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.740741 talisman-tools-0.6.5/talisman_tools/commands/model/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.740741 talisman-tools-0.6.5/talisman_tools/commands/model/commands/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.740741 talisman-tools-0.6.5/talisman_tools/commands/model/commands/check_performance/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/check_performance/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2893 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/check_performance/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/check_performance/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.740741 talisman-tools-0.6.5/talisman_tools/commands/model/commands/configure/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/configure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/configure/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.744741 talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3605 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     4892 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/evaluation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.744741 talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/evaluators/
+-rw-rw-rw-   0 root         (0) root         (0)      708 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/evaluators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/evaluators/disambiguation_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/evaluators/nerc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/evaluators/relext.py
+-rw-rw-rw-   0 root         (0) root         (0)     5278 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    15234 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.748741 talisman-tools-0.6.5/talisman_tools/commands/model/commands/process/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/process/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/process/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/commands/subparsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/model/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.748741 talisman-tools-0.6.5/talisman_tools/commands/servers/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.748741 talisman-tools-0.6.5/talisman_tools/commands/servers/arguments/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:45.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/arguments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/arguments/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.748741 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.748741 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/converter/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/converter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/converter/action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.752741 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/converter/methods/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:45.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/converter/methods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2857 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/converter/methods/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/converter/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.752741 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/loader/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/loader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/loader/action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.752741 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/loader/methods/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:45.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/loader/methods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/loader/methods/load.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/loader/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.752741 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/processor/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/processor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/processor/action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.752741 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/processor/methods/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:45.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/processor/methods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2881 2024-04-27 14:10:37.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/processor/methods/process.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/processor/methods/update.py
+-rw-rw-rw-   0 root         (0) root         (0)      927 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/processor/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/commands/subparsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      779 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2024-04-27 14:10:37.000000 talisman-tools-0.6.5/talisman_tools/commands/servers/server_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/subparsers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.756741 talisman-tools-0.6.5/talisman_tools/commands/train/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:45.000000 talisman-tools-0.6.5/talisman_tools/commands/train/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/train/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/commands/train/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.756741 talisman-tools-0.6.5/talisman_tools/configure/
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/configure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5626 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/configure/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/configure/wrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.756741 talisman-tools-0.6.5/talisman_tools/configure/wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/configure/wrapper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/configure/wrapper/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.756741 talisman-tools-0.6.5/talisman_tools/helper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-27 14:10:45.000000 talisman-tools-0.6.5/talisman_tools/helper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/helper/concurrency.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/helper/env.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/helper/log_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/helper/multiprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/parser_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.760741 talisman-tools-0.6.5/talisman_tools/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/plugin/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/plugin/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/plugin/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/plugin/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/plugin/kb.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/plugin/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/plugin/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/plugin/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/plugin/trainer.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/plugin/wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/plugin/wrapper_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      796 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/talisman.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-04-24 13:52:33.000000 talisman-tools-0.6.5/talisman_tools/talisman_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:11:02.736740 talisman-tools-0.6.5/talisman_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      713 2024-04-27 14:11:02.000000 talisman-tools-0.6.5/talisman_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4615 2024-04-27 14:11:02.000000 talisman-tools-0.6.5/talisman_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 14:11:02.000000 talisman-tools-0.6.5/talisman_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-27 14:11:02.000000 talisman-tools-0.6.5/talisman_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      312 2024-04-27 14:11:02.000000 talisman-tools-0.6.5/talisman_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-27 14:11:02.000000 talisman-tools-0.6.5/talisman_tools.egg-info/top_level.txt
```

### Comparing `talisman-tools-0.6.4/PKG-INFO` & `talisman-tools-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-tools
-Version: 0.6.4
+Version: 0.6.5
 Summary: Talisman applications
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-tools-0.6.4/setup.py` & `talisman-tools-0.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description_content_type="text/markdown",
     author='ISPRAS Talisman NLP team',
     author_email='modis@ispras.ru',
     maintainer='Vladimir Mayorov',
     maintainer_email='vmayorov@ispras.ru',
     packages=find_packages(include=['talisman_tools', 'talisman_tools.*']),
     install_requires=[
-        'talisman-interfaces~=0.5.3', 'talisman-dm~=1.0.0a37',
+        'talisman-interfaces~=0.5.4', 'talisman-dm~=1.0.0a37',
         'fastapi>=0.73.0', 'pydantic~=1.10.4', 'uvicorn>=0.13.3', 'requests~=2.31.0', 'urllib3~=2.2.0',
         'jsonformatter>=0.3.0',
         'starlette', 'anyio',
         'pyyaml'
     ],
     extras_require={
         'logstash': ['python3-logstash>=0.4.80'],
```

### Comparing `talisman-tools-0.6.4/talisman_tools/arguments/domain.py` & `talisman-tools-0.6.5/talisman_tools/arguments/domain.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/arguments/loader.py` & `talisman-tools-0.6.5/talisman_tools/arguments/loader.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/arguments/processor.py` & `talisman-tools-0.6.5/talisman_tools/arguments/processor.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/arguments/reader.py` & `talisman-tools-0.6.5/talisman_tools/arguments/reader.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/arguments/serializer.py` & `talisman-tools-0.6.5/talisman_tools/arguments/serializer.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/dataset/commands/convert/parser.py` & `talisman-tools-0.6.5/talisman_tools/commands/dataset/commands/convert/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/dataset/parser.py` & `talisman-tools-0.6.5/talisman_tools/commands/dataset/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/check_performance/action.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/check_performance/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/check_performance/parser.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/check_performance/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/configure/parser.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/configure/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/action.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/evaluation.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/evaluation.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/evaluators/__init__.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/evaluators/disambiguation_quality.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/evaluators/disambiguation_quality.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/evaluators/nerc.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/evaluators/nerc.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/evaluators/relext.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/evaluators/relext.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/helpers.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/helpers.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/metrics.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/evaluate/parser.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/evaluate/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/process/action.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/process/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/process/parser.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/process/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/commands/subparsers.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/commands/subparsers.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/model/parser.py` & `talisman-tools-0.6.5/talisman_tools/commands/model/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/arguments/server.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/arguments/server.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/commands/converter/action.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/commands/converter/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/commands/converter/methods/convert.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/commands/converter/methods/convert.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/commands/converter/parser.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/commands/converter/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/commands/loader/action.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/commands/loader/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/commands/loader/methods/load.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/commands/loader/methods/load.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/commands/loader/parser.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/commands/loader/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/commands/processor/action.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/commands/processor/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/commands/processor/methods/process.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/commands/processor/methods/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any, List, Optional, Sequence, Tuple, Union
 
 from fastapi import FastAPI, HTTPException, Request
 from tdm import TalismanDocumentModel
 
 from talisman_tools.commands.servers.server_helper import log_debug_data
 from tp_interfaces.abstract import AbstractDocumentProcessor, ImmutableBaseModel
+from tp_interfaces.abstract.exception import WrongRequest
 from tp_interfaces.helpers.batch import AbstractModelInput, async_batch_process_inputs
 from tp_interfaces.logging.context import update_log_extras
 
 _logger = logging.getLogger(__name__)
 
 
 def register_process_docs(
@@ -48,13 +49,16 @@
             response_post_processor = itemgetter(0)
 
         with update_log_extras(id=[message.message.id for message in messages]):
             log_debug_data(logger, f"got {len(messages)} documents for processing", request)
             task = partial(async_batch_process_inputs, inputs=messages, processor=process_with_config)
             try:
                 response = await task()
+            except WrongRequest as e:
+                logger.error("WrongRequest exception while processing request", exc_info=e)
+                raise HTTPException(status_code=422, detail=str(e) if len(str(e)) else "Internal error: " + e.__repr__())
             except Exception as e:
                 logger.error("Exception while processing request", exc_info=e)
                 raise HTTPException(status_code=500)
             log_debug_data(logger, f"processed {len(response)} documents", request)
 
             return response_post_processor(response)
```

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/commands/processor/methods/update.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/commands/processor/methods/update.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/commands/processor/parser.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/commands/processor/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/commands/subparsers.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/commands/subparsers.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/parser.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/servers/server_helper.py` & `talisman-tools-0.6.5/talisman_tools/commands/servers/server_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-import logging
 import logging.config
 from contextlib import AbstractContextManager
-from typing import Any, AsyncContextManager, Dict, Generator, Sequence, Tuple
+from typing import AsyncContextManager
 
 from fastapi import FastAPI, Request
 from fastapi.encoders import jsonable_encoder
 from fastapi.exceptions import RequestValidationError
-from pydantic import PydanticTypeError
-from pydantic.error_wrappers import ErrorWrapper, ValidationError
 from starlette import status
 from starlette.responses import JSONResponse
 
 _logger = logging.getLogger(__name__)
 
 
 def register_context_manager(app: FastAPI, context_manager: AbstractContextManager):
@@ -33,47 +30,21 @@
     async def exit_manager():
         await context_manager.__aexit__(None, None, None)
 
 
 def register_exception_handlers(app: FastAPI, logger: logging.Logger = _logger):
     @app.exception_handler(RequestValidationError)
     async def validation_exception_handler(request, exc: RequestValidationError):
-        error_content = jsonable_encoder({"detail": list(unwrap(exc.raw_errors))})
+        error_content = jsonable_encoder({"detail": exc.args})
         logger.error("Pydantic validation error", extra=error_content)
         return JSONResponse(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             content=error_content,
         )
 
-    def unwrap(errors: Sequence[Any]) -> Generator[Dict[str, Any], None, None]:
-        for error in errors:
-            if isinstance(error, ErrorWrapper):
-                yield wrap_description(error)
-            elif isinstance(error, list):
-                yield from unwrap(error)
-            else:
-                logging.error(f'Unknown error object: {error}')
-                raise RuntimeError(f'Unknown error object: {error}')
-
-    def wrap_description(wrap: ErrorWrapper) -> Dict[str, Any]:
-        loc = wrap.loc_tuple()  # validated parameter
-        if isinstance(wrap.exc, ValidationError):
-            model, errors = validation_error(wrap.exc)
-        elif isinstance(wrap.exc, PydanticTypeError):
-            model, errors = type_error(wrap.exc)
-        else:
-            model, errors = type(wrap.exc).__name__, []
-        return {'model': model, 'loc': loc, 'errors': errors}
-
-    def validation_error(exc: ValidationError) -> Tuple[str, list]:
-        return exc.model.__name__, exc.errors()
-
-    def type_error(exc: PydanticTypeError) -> Tuple[str, str]:
-        return type(exc).__name__, exc.msg_template
-
 
 def log_debug_data(logger: logging.Logger, msg: str, request: Request = None, **kwargs) -> None:
     extras = {}
     if request is not None:
         extras['client'] = request.client
     extras.update({key: jsonable_encoder(value) for key, value in kwargs.items()})
     logger.debug(msg, extra=extras)
```

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/subparsers.py` & `talisman-tools-0.6.5/talisman_tools/commands/subparsers.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/train/action.py` & `talisman-tools-0.6.5/talisman_tools/commands/train/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/commands/train/parser.py` & `talisman-tools-0.6.5/talisman_tools/commands/train/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/configure/configure.py` & `talisman-tools-0.6.5/talisman_tools/configure/configure.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/configure/wrapper/actions.py` & `talisman-tools-0.6.5/talisman_tools/configure/wrapper/actions.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/helper/concurrency.py` & `talisman-tools-0.6.5/talisman_tools/helper/concurrency.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/helper/multiprocessing.py` & `talisman-tools-0.6.5/talisman_tools/helper/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/parser_helper.py` & `talisman-tools-0.6.5/talisman_tools/parser_helper.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/plugin/__init__.py` & `talisman-tools-0.6.5/talisman_tools/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/plugin/abstract.py` & `talisman-tools-0.6.5/talisman_tools/plugin/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/plugin/cli.py` & `talisman-tools-0.6.5/talisman_tools/plugin/cli.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/plugin/domain.py` & `talisman-tools-0.6.5/talisman_tools/plugin/domain.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/plugin/endpoint.py` & `talisman-tools-0.6.5/talisman_tools/plugin/endpoint.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/plugin/reader.py` & `talisman-tools-0.6.5/talisman_tools/plugin/reader.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/plugin/serializer.py` & `talisman-tools-0.6.5/talisman_tools/plugin/serializer.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/plugin/wrapper_actions.py` & `talisman-tools-0.6.5/talisman_tools/plugin/wrapper_actions.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/talisman.py` & `talisman-tools-0.6.5/talisman_tools/talisman.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools/talisman_logging.py` & `talisman-tools-0.6.5/talisman_tools/talisman_logging.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.4/talisman_tools.egg-info/PKG-INFO` & `talisman-tools-0.6.5/talisman_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-tools
-Version: 0.6.4
+Version: 0.6.5
 Summary: Talisman applications
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-tools-0.6.4/talisman_tools.egg-info/SOURCES.txt` & `talisman-tools-0.6.5/talisman_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

