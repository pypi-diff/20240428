# Comparing `tmp/querent-3.0.5.tar.gz` & `tmp/querent-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querent-3.0.5.tar", last modified: Sat Apr 27 22:03:50 2024, max compression
+gzip compressed data, was "querent-3.0.6.tar", last modified: Sun Apr 28 00:02:07 2024, max compression
```

## Comparing `querent-3.0.5.tar` & `querent-3.0.6.tar`

### file list

```diff
@@ -1,260 +1,260 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.617422 querent-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-27 21:57:45.000000 querent-3.0.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-27 22:03:50.617422 querent-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-27 21:57:45.000000 querent-3.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.541422 querent-3.0.5/querent/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-27 21:57:45.000000 querent-3.0.5/querent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.541422 querent-3.0.5/querent/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-27 21:57:45.000000 querent-3.0.5/querent/callback/event_callback_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-27 21:57:45.000000 querent-3.0.5/querent/callback/event_callback_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.545421 querent-3.0.5/querent/channel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-27 21:57:45.000000 querent-3.0.5/querent/channel/channel_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.545421 querent-3.0.5/querent/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.545421 querent-3.0.5/querent/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.549422 querent-3.0.5/querent/collectors/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/aws/aws_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.549422 querent-3.0.5/querent/collectors/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/azure/azure_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/collector_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/collector_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/collector_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/collector_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.549422 querent-3.0.5/querent/collectors/drive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/drive/google_drive_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.549422 querent-3.0.5/querent/collectors/dropbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/dropbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/dropbox/dropbox_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.549422 querent-3.0.5/querent/collectors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/email/email_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/email/imap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.549422 querent-3.0.5/querent/collectors/fs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/fs/fs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.553422 querent-3.0.5/querent/collectors/gcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/gcs/gcs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.553422 querent-3.0.5/querent/collectors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/github/github_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.553422 querent-3.0.5/querent/collectors/jira/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/jira/jira_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.553422 querent-3.0.5/querent/collectors/news/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/news/news_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.553422 querent-3.0.5/querent/collectors/slack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/slack/slack_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.557422 querent-3.0.5/querent/collectors/webscaper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/webscaper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-27 21:57:45.000000 querent-3.0.5/querent/collectors/webscaper/web_scraper_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.557422 querent-3.0.5/querent/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/common_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.557422 querent-3.0.5/querent/common/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/errors/metric_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.565422 querent-3.0.5/querent/common/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/collected_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/collector_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/engine_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/file_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/ingested_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/ingested_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/ingested_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/ingested_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/querent_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/querent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/resource_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/types/workflow_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-27 21:57:45.000000 querent-3.0.5/querent/common/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.565422 querent-3.0.5/querent/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.565422 querent-3.0.5/querent/config/collector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/collector/collector_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.569422 querent-3.0.5/querent/config/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/core/gpt_llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/core/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/core/opensource_llm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.569422 querent-3.0.5/querent/config/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/engine/engine_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/graph_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.569422 querent-3.0.5/querent/config/ingestor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/ingestor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/ingestor/ingestor_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.573422 querent-3.0.5/querent/config/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/logger/logger_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.573422 querent-3.0.5/querent/config/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/metric/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.573422 querent-3.0.5/querent/config/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/resource/resource_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.573422 querent-3.0.5/querent/config/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-27 21:57:45.000000 querent-3.0.5/querent/config/workflow/workflow_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.573422 querent-3.0.5/querent/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.573422 querent-3.0.5/querent/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-27 21:57:45.000000 querent-3.0.5/querent/core/base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.577422 querent-3.0.5/querent/core/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/core/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-04-27 21:57:45.000000 querent-3.0.5/querent/core/transformers/bert_ner_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-27 21:57:45.000000 querent-3.0.5/querent/core/transformers/fixed_entities_set_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-04-27 21:57:45.000000 querent-3.0.5/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13002 2024-04-27 21:57:45.000000 querent-3.0.5/querent/core/transformers/gpt_llm_gpt_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-04-27 21:57:45.000000 querent-3.0.5/querent/core/transformers/relationship_extraction_llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.577422 querent-3.0.5/querent/dal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/dal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.577422 querent-3.0.5/querent/gnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/gnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.581422 querent-3.0.5/querent/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-27 21:57:45.000000 querent-3.0.5/querent/graph/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-27 21:57:45.000000 querent-3.0.5/querent/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-27 21:57:45.000000 querent-3.0.5/querent/graph/graph_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-27 21:57:45.000000 querent-3.0.5/querent/graph/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-27 21:57:45.000000 querent-3.0.5/querent/graph/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-27 21:57:45.000000 querent-3.0.5/querent/graph/shacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-27 21:57:45.000000 querent-3.0.5/querent/graph/subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-27 21:57:45.000000 querent-3.0.5/querent/graph/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.585422 querent-3.0.5/querent/ingestors/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.585422 querent-3.0.5/querent/ingestors/audio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/audio/audio_ingestors.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/base_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.585422 querent-3.0.5/querent/ingestors/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/code/code_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.585422 querent-3.0.5/querent/ingestors/csv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/csv/csv_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.585422 querent-3.0.5/querent/ingestors/doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/doc/doc_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.589422 querent-3.0.5/querent/ingestors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/email/email_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/email/email_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.589422 querent-3.0.5/querent/ingestors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/github/github_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.589422 querent-3.0.5/querent/ingestors/html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/html/html_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.589422 querent-3.0.5/querent/ingestors/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/images/image_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/ingestor_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/ingestor_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.589422 querent-3.0.5/querent/ingestors/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/json/json_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.593422 querent-3.0.5/querent/ingestors/pdfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/pdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/pdfs/pdf_ingestor_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.593422 querent-3.0.5/querent/ingestors/ppt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/ppt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/ppt/ppt_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.593422 querent-3.0.5/querent/ingestors/texts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/texts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/texts/text_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.593422 querent-3.0.5/querent/ingestors/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/video/video_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.593422 querent-3.0.5/querent/ingestors/xlsx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/xlsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/xlsx/xlsx_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.597422 querent-3.0.5/querent/ingestors/xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-27 21:57:45.000000 querent-3.0.5/querent/ingestors/xml/xml_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.597422 querent-3.0.5/querent/kg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.601422 querent-3.0.5/querent/kg/ner_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/ner_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/ner_helperfunctions/attn_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/ner_helperfunctions/contextual_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/ner_helperfunctions/dependency_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/ner_helperfunctions/filter_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/ner_helperfunctions/fixed_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/ner_helperfunctions/fixed_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/ner_helperfunctions/ner_llm_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/querent_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.605422 querent-3.0.5/querent/kg/rel_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/rel_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/rel_helperfunctions/contextual_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/rel_helperfunctions/embedding_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/rel_helperfunctions/fixed_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/rel_helperfunctions/openai_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/rel_helperfunctions/openllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/rel_helperfunctions/questionanswer_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/rel_helperfunctions/rel_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-27 21:57:45.000000 querent-3.0.5/querent/kg/rel_helperfunctions/triple_to_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.605422 querent-3.0.5/querent/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-27 21:57:45.000000 querent-3.0.5/querent/logging/custom_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-27 21:57:45.000000 querent-3.0.5/querent/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-27 21:57:45.000000 querent-3.0.5/querent/logging/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-27 21:57:45.000000 querent-3.0.5/querent/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.609422 querent-3.0.5/querent/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.609422 querent-3.0.5/querent/metric/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/metric/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-27 21:57:45.000000 querent-3.0.5/querent/metric/adapters/promethus_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-27 21:57:45.000000 querent-3.0.5/querent/metric/base_metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-27 21:57:45.000000 querent-3.0.5/querent/metric/metric_logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-27 21:57:45.000000 querent-3.0.5/querent/metric/metric_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.609422 querent-3.0.5/querent/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-27 21:57:45.000000 querent-3.0.5/querent/processors/async_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-27 21:57:45.000000 querent-3.0.5/querent/processors/text_cleanup_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-27 21:57:45.000000 querent-3.0.5/querent/processors/text_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.613422 querent-3.0.5/querent/querent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/querent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-27 21:57:45.000000 querent-3.0.5/querent/querent/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-27 21:57:45.000000 querent-3.0.5/querent/querent/querent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-27 21:57:45.000000 querent-3.0.5/querent/querent/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/querent/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.613422 querent-3.0.5/querent/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-27 21:57:45.000000 querent-3.0.5/querent/storage/gcs_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-27 21:57:45.000000 querent-3.0.5/querent/storage/milvus_vectorevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-27 21:57:45.000000 querent-3.0.5/querent/storage/neo4j_graphevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-27 21:57:45.000000 querent-3.0.5/querent/storage/postgres_graphevent_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.613422 querent-3.0.5/querent/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-04-27 21:57:45.000000 querent-3.0.5/querent/tools/web_page_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.617422 querent-3.0.5/querent/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:57:45.000000 querent-3.0.5/querent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-27 21:57:45.000000 querent-3.0.5/querent/utils/webpage_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.617422 querent-3.0.5/querent/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-27 21:57:45.000000 querent-3.0.5/querent/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-04-27 21:57:45.000000 querent-3.0.5/querent/workflow/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-27 21:57:45.000000 querent-3.0.5/querent/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:03:50.617422 querent-3.0.5/querent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-27 22:03:50.000000 querent-3.0.5/querent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-27 22:03:50.000000 querent-3.0.5/querent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-27 22:03:50.000000 querent-3.0.5/querent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-27 22:03:50.000000 querent-3.0.5/querent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 22:03:50.000000 querent-3.0.5/querent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:03:50.617422 querent-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-27 21:57:45.000000 querent-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.047162 querent-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-27 23:57:32.000000 querent-3.0.6/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-04-28 00:02:07.047162 querent-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-27 23:57:32.000000 querent-3.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.979163 querent-3.0.6/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-27 23:57:32.000000 querent-3.0.6/querent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.979163 querent-3.0.6/querent/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-27 23:57:32.000000 querent-3.0.6/querent/callback/event_callback_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-27 23:57:32.000000 querent-3.0.6/querent/callback/event_callback_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.983162 querent-3.0.6/querent/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-27 23:57:32.000000 querent-3.0.6/querent/channel/channel_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.983162 querent-3.0.6/querent/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.983162 querent-3.0.6/querent/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.983162 querent-3.0.6/querent/collectors/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/aws/aws_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.983162 querent-3.0.6/querent/collectors/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/azure/azure_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/collector_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/collector_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/collector_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/collector_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.987162 querent-3.0.6/querent/collectors/drive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/drive/google_drive_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.987162 querent-3.0.6/querent/collectors/dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/dropbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/dropbox/dropbox_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.987162 querent-3.0.6/querent/collectors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/email/email_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/email/imap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.987162 querent-3.0.6/querent/collectors/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/fs/fs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.987162 querent-3.0.6/querent/collectors/gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/gcs/gcs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.987162 querent-3.0.6/querent/collectors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/github/github_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.991162 querent-3.0.6/querent/collectors/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/jira/jira_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.991162 querent-3.0.6/querent/collectors/news/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/news/news_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.991162 querent-3.0.6/querent/collectors/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/slack/slack_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.991162 querent-3.0.6/querent/collectors/webscaper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/webscaper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-27 23:57:32.000000 querent-3.0.6/querent/collectors/webscaper/web_scraper_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.991162 querent-3.0.6/querent/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/common_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.991162 querent-3.0.6/querent/common/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/errors/metric_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.999162 querent-3.0.6/querent/common/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/collected_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/collector_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/engine_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/file_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/ingested_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/ingested_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/ingested_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/ingested_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/querent_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/querent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/resource_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/types/workflow_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-27 23:57:32.000000 querent-3.0.6/querent/common/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.999162 querent-3.0.6/querent/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.999162 querent-3.0.6/querent/config/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/collector/collector_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:06.999162 querent-3.0.6/querent/config/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/core/gpt_llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/core/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/core/opensource_llm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.003162 querent-3.0.6/querent/config/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/engine/engine_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/graph_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.003162 querent-3.0.6/querent/config/ingestor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/ingestor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/ingestor/ingestor_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.003162 querent-3.0.6/querent/config/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/logger/logger_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.003162 querent-3.0.6/querent/config/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/metric/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.003162 querent-3.0.6/querent/config/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/resource/resource_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.003162 querent-3.0.6/querent/config/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-27 23:57:32.000000 querent-3.0.6/querent/config/workflow/workflow_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.003162 querent-3.0.6/querent/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.007162 querent-3.0.6/querent/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-27 23:57:32.000000 querent-3.0.6/querent/core/base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.007162 querent-3.0.6/querent/core/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/core/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-04-27 23:57:32.000000 querent-3.0.6/querent/core/transformers/bert_ner_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-27 23:57:32.000000 querent-3.0.6/querent/core/transformers/fixed_entities_set_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-04-27 23:57:32.000000 querent-3.0.6/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13002 2024-04-27 23:57:32.000000 querent-3.0.6/querent/core/transformers/gpt_llm_gpt_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-04-27 23:57:32.000000 querent-3.0.6/querent/core/transformers/relationship_extraction_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.007162 querent-3.0.6/querent/dal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/dal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.007162 querent-3.0.6/querent/gnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/gnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.011162 querent-3.0.6/querent/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-27 23:57:32.000000 querent-3.0.6/querent/graph/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-27 23:57:32.000000 querent-3.0.6/querent/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-27 23:57:32.000000 querent-3.0.6/querent/graph/graph_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-27 23:57:32.000000 querent-3.0.6/querent/graph/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-27 23:57:32.000000 querent-3.0.6/querent/graph/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-27 23:57:32.000000 querent-3.0.6/querent/graph/shacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-27 23:57:32.000000 querent-3.0.6/querent/graph/subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-27 23:57:32.000000 querent-3.0.6/querent/graph/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.011162 querent-3.0.6/querent/ingestors/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.015162 querent-3.0.6/querent/ingestors/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/audio/audio_ingestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/base_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.015162 querent-3.0.6/querent/ingestors/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/code/code_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.015162 querent-3.0.6/querent/ingestors/csv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/csv/csv_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.015162 querent-3.0.6/querent/ingestors/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/doc/doc_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.015162 querent-3.0.6/querent/ingestors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/email/email_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/email/email_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.019162 querent-3.0.6/querent/ingestors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/github/github_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.019162 querent-3.0.6/querent/ingestors/html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/html/html_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.019162 querent-3.0.6/querent/ingestors/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/images/image_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/ingestor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/ingestor_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.019162 querent-3.0.6/querent/ingestors/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/json/json_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.023162 querent-3.0.6/querent/ingestors/pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/pdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/pdfs/pdf_ingestor_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.023162 querent-3.0.6/querent/ingestors/ppt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/ppt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/ppt/ppt_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.023162 querent-3.0.6/querent/ingestors/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/texts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/texts/text_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.023162 querent-3.0.6/querent/ingestors/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/video/video_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.023162 querent-3.0.6/querent/ingestors/xlsx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/xlsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/xlsx/xlsx_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.023162 querent-3.0.6/querent/ingestors/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-27 23:57:32.000000 querent-3.0.6/querent/ingestors/xml/xml_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.027162 querent-3.0.6/querent/kg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.027162 querent-3.0.6/querent/kg/ner_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/ner_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/ner_helperfunctions/attn_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/ner_helperfunctions/contextual_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/ner_helperfunctions/dependency_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/ner_helperfunctions/filter_triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/ner_helperfunctions/fixed_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/ner_helperfunctions/fixed_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/ner_helperfunctions/ner_llm_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/querent_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.031162 querent-3.0.6/querent/kg/rel_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/rel_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/rel_helperfunctions/contextual_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/rel_helperfunctions/embedding_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/rel_helperfunctions/fixed_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/rel_helperfunctions/openai_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/rel_helperfunctions/openllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/rel_helperfunctions/questionanswer_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/rel_helperfunctions/rel_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-27 23:57:32.000000 querent-3.0.6/querent/kg/rel_helperfunctions/triple_to_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.035162 querent-3.0.6/querent/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-27 23:57:32.000000 querent-3.0.6/querent/logging/custom_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-27 23:57:32.000000 querent-3.0.6/querent/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-27 23:57:32.000000 querent-3.0.6/querent/logging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-27 23:57:32.000000 querent-3.0.6/querent/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.035162 querent-3.0.6/querent/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.035162 querent-3.0.6/querent/metric/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/metric/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-27 23:57:32.000000 querent-3.0.6/querent/metric/adapters/promethus_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-27 23:57:32.000000 querent-3.0.6/querent/metric/base_metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-27 23:57:32.000000 querent-3.0.6/querent/metric/metric_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-27 23:57:32.000000 querent-3.0.6/querent/metric/metric_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.039162 querent-3.0.6/querent/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-27 23:57:32.000000 querent-3.0.6/querent/processors/async_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-27 23:57:32.000000 querent-3.0.6/querent/processors/text_cleanup_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-27 23:57:32.000000 querent-3.0.6/querent/processors/text_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.039162 querent-3.0.6/querent/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/querent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-27 23:57:32.000000 querent-3.0.6/querent/querent/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-27 23:57:32.000000 querent-3.0.6/querent/querent/querent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-27 23:57:32.000000 querent-3.0.6/querent/querent/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/querent/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.043162 querent-3.0.6/querent/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-27 23:57:32.000000 querent-3.0.6/querent/storage/gcs_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-27 23:57:32.000000 querent-3.0.6/querent/storage/milvus_vectorevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-27 23:57:32.000000 querent-3.0.6/querent/storage/neo4j_graphevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-27 23:57:32.000000 querent-3.0.6/querent/storage/postgres_graphevent_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.043162 querent-3.0.6/querent/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-04-27 23:57:32.000000 querent-3.0.6/querent/tools/web_page_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.043162 querent-3.0.6/querent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 23:57:32.000000 querent-3.0.6/querent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-27 23:57:32.000000 querent-3.0.6/querent/utils/webpage_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.043162 querent-3.0.6/querent/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-27 23:57:32.000000 querent-3.0.6/querent/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-04-27 23:57:32.000000 querent-3.0.6/querent/workflow/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-27 23:57:32.000000 querent-3.0.6/querent/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:02:07.043162 querent-3.0.6/querent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-04-28 00:02:06.000000 querent-3.0.6/querent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-28 00:02:06.000000 querent-3.0.6/querent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-28 00:02:06.000000 querent-3.0.6/querent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-28 00:02:06.000000 querent-3.0.6/querent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 00:02:06.000000 querent-3.0.6/querent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 00:02:07.047162 querent-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-27 23:57:32.000000 querent-3.0.6/setup.py
```

### Comparing `querent-3.0.5/LICENCE` & `querent-3.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/PKG-INFO` & `querent-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.5
+Version: 3.0.6
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
@@ -32,15 +32,15 @@
 Classifier: Topic :: Utilities
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
-Requires-Python: >=3.9, <=3.10
+Requires-Python: ==3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.4
 Requires-Dist: attrs==23.1.0
 Requires-Dist: azure-storage-blob==12.19.0
 Requires-Dist: beautifulsoup4==4.12.3
@@ -100,14 +100,16 @@
 Requires-Dist: slack-sdk==3.26.1
 Requires-Dist: spacy==3.7.2
 Requires-Dist: speechrecognition==3.10.1
 Requires-Dist: tika==2.6.0
 Requires-Dist: tensorflow==2.14.0
 Requires-Dist: transformers==4.36.0
 Requires-Dist: unidecode==1.3.7
+Provides-Extra: torch
+Requires-Dist: torch; extra == "torch"
 
 # Querent
 
 The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 
 ![image](https://github.com/Querent-ai/querent-ai/assets/61435908/39124a0c-3d9e-434f-9b54-9aa51dcefbd7)
```

### Comparing `querent-3.0.5/README.md` & `querent-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/__init__.py` & `querent-3.0.6/querent/__init__.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/callback/event_callback_dispatcher.py` & `querent-3.0.6/querent/callback/event_callback_dispatcher.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/callback/event_callback_interface.py` & `querent-3.0.6/querent/callback/event_callback_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/channel/channel_interface.py` & `querent-3.0.6/querent/channel/channel_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/aws/aws_collector.py` & `querent-3.0.6/querent/collectors/aws/aws_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/azure/azure_collector.py` & `querent-3.0.6/querent/collectors/azure/azure_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/collector_errors.py` & `querent-3.0.6/querent/collectors/collector_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/collector_factory.py` & `querent-3.0.6/querent/collectors/collector_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/collector_resolver.py` & `querent-3.0.6/querent/collectors/collector_resolver.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/drive/google_drive_collector.py` & `querent-3.0.6/querent/collectors/drive/google_drive_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/dropbox/dropbox_collector.py` & `querent-3.0.6/querent/collectors/dropbox/dropbox_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/email/email_collector.py` & `querent-3.0.6/querent/collectors/email/email_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/email/imap.py` & `querent-3.0.6/querent/collectors/email/imap.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/fs/fs_collector.py` & `querent-3.0.6/querent/collectors/fs/fs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/gcs/gcs_collector.py` & `querent-3.0.6/querent/collectors/gcs/gcs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/github/github_collector.py` & `querent-3.0.6/querent/collectors/github/github_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/jira/jira_collector.py` & `querent-3.0.6/querent/collectors/jira/jira_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/news/news_collector.py` & `querent-3.0.6/querent/collectors/news/news_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/slack/slack_collector.py` & `querent-3.0.6/querent/collectors/slack/slack_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/collectors/webscaper/web_scraper_collector.py` & `querent-3.0.6/querent/collectors/webscaper/web_scraper_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/common/common_errors.py` & `querent-3.0.6/querent/common/common_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/common/errors/metric_errors.py` & `querent-3.0.6/querent/common/errors/metric_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/common/types/collected_bytes.py` & `querent-3.0.6/querent/common/types/collected_bytes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/common/types/file_buffer.py` & `querent-3.0.6/querent/common/types/file_buffer.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/common/types/ingested_code.py` & `querent-3.0.6/querent/common/types/ingested_code.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/common/types/ingested_images.py` & `querent-3.0.6/querent/common/types/ingested_images.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/common/types/ingested_messages.py` & `querent-3.0.6/querent/common/types/ingested_messages.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/common/types/ingested_tokens.py` & `querent-3.0.6/querent/common/types/ingested_tokens.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/common/types/querent_queue.py` & `querent-3.0.6/querent/common/types/querent_queue.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/common/uri.py` & `querent-3.0.6/querent/common/uri.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/config/collector/collector_config.py` & `querent-3.0.6/querent/config/collector/collector_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/config/config.py` & `querent-3.0.6/querent/config/config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/config/core/gpt_llm_config.py` & `querent-3.0.6/querent/config/core/gpt_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/config/core/llm_config.py` & `querent-3.0.6/querent/config/core/llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/config/core/opensource_llm_config.py` & `querent-3.0.6/querent/config/core/opensource_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/config/engine/engine_config.py` & `querent-3.0.6/querent/config/engine/engine_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/config/graph_config.py` & `querent-3.0.6/querent/config/graph_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/config/ingestor/ingestor_config.py` & `querent-3.0.6/querent/config/ingestor/ingestor_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/config/metric/prometheus.py` & `querent-3.0.6/querent/config/metric/prometheus.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/config/resource/resource_config.py` & `querent-3.0.6/querent/config/resource/resource_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/config/workflow/workflow_config.py` & `querent-3.0.6/querent/config/workflow/workflow_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/core/base_engine.py` & `querent-3.0.6/querent/core/base_engine.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/core/transformers/bert_ner_opensourcellm.py` & `querent-3.0.6/querent/core/transformers/bert_ner_opensourcellm.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/core/transformers/fixed_entities_set_opensourcellm.py` & `querent-3.0.6/querent/core/transformers/fixed_entities_set_opensourcellm.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py` & `querent-3.0.6/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/core/transformers/gpt_llm_gpt_ner.py` & `querent-3.0.6/querent/core/transformers/gpt_llm_gpt_ner.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/core/transformers/relationship_extraction_llm.py` & `querent-3.0.6/querent/core/transformers/relationship_extraction_llm.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/graph/errors.py` & `querent-3.0.6/querent/graph/errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/graph/graph.py` & `querent-3.0.6/querent/graph/graph.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/graph/graph_namespace.py` & `querent-3.0.6/querent/graph/graph_namespace.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/graph/ontology.py` & `querent-3.0.6/querent/graph/ontology.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/graph/schema.py` & `querent-3.0.6/querent/graph/schema.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/graph/shacl.py` & `querent-3.0.6/querent/graph/shacl.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/graph/subject.py` & `querent-3.0.6/querent/graph/subject.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/graph/utils.py` & `querent-3.0.6/querent/graph/utils.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/audio/audio_ingestors.py` & `querent-3.0.6/querent/ingestors/audio/audio_ingestors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/base_ingestor.py` & `querent-3.0.6/querent/ingestors/base_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/code/code_ingestor.py` & `querent-3.0.6/querent/ingestors/code/code_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/csv/csv_ingestor.py` & `querent-3.0.6/querent/ingestors/csv/csv_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/doc/doc_ingestor.py` & `querent-3.0.6/querent/ingestors/doc/doc_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/email/email_ingestor.py` & `querent-3.0.6/querent/ingestors/email/email_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/email/email_reader.py` & `querent-3.0.6/querent/ingestors/email/email_reader.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/github/github_ingestor.py` & `querent-3.0.6/querent/ingestors/github/github_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/html/html_ingestor.py` & `querent-3.0.6/querent/ingestors/html/html_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/images/image_ingestor.py` & `querent-3.0.6/querent/ingestors/images/image_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/ingestor_factory.py` & `querent-3.0.6/querent/ingestors/ingestor_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/ingestor_manager.py` & `querent-3.0.6/querent/ingestors/ingestor_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/json/json_ingestor.py` & `querent-3.0.6/querent/ingestors/json/json_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/pdfs/pdf_ingestor_v1.py` & `querent-3.0.6/querent/ingestors/pdfs/pdf_ingestor_v1.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/ppt/ppt_ingestor.py` & `querent-3.0.6/querent/ingestors/ppt/ppt_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/texts/text_ingestor.py` & `querent-3.0.6/querent/ingestors/texts/text_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/video/video_ingestor.py` & `querent-3.0.6/querent/ingestors/video/video_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/xlsx/xlsx_ingestor.py` & `querent-3.0.6/querent/ingestors/xlsx/xlsx_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/ingestors/xml/xml_ingestor.py` & `querent-3.0.6/querent/ingestors/xml/xml_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/ner_helperfunctions/attn_scores.py` & `querent-3.0.6/querent/kg/ner_helperfunctions/attn_scores.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/ner_helperfunctions/contextual_embeddings.py` & `querent-3.0.6/querent/kg/ner_helperfunctions/contextual_embeddings.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/ner_helperfunctions/dependency_parsing.py` & `querent-3.0.6/querent/kg/ner_helperfunctions/dependency_parsing.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/ner_helperfunctions/filter_triples.py` & `querent-3.0.6/querent/kg/ner_helperfunctions/filter_triples.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/ner_helperfunctions/fixed_entities.py` & `querent-3.0.6/querent/kg/ner_helperfunctions/fixed_entities.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/ner_helperfunctions/fixed_predicate.py` & `querent-3.0.6/querent/kg/ner_helperfunctions/fixed_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/ner_helperfunctions/ner_llm_transformer.py` & `querent-3.0.6/querent/kg/ner_helperfunctions/ner_llm_transformer.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/querent_kg.py` & `querent-3.0.6/querent/kg/querent_kg.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/rel_helperfunctions/contextual_predicate.py` & `querent-3.0.6/querent/kg/rel_helperfunctions/contextual_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/rel_helperfunctions/embedding_store.py` & `querent-3.0.6/querent/kg/rel_helperfunctions/embedding_store.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/rel_helperfunctions/fixed_relationships.py` & `querent-3.0.6/querent/kg/rel_helperfunctions/fixed_relationships.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py` & `querent-3.0.6/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/rel_helperfunctions/openai_functions.py` & `querent-3.0.6/querent/kg/rel_helperfunctions/openai_functions.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/rel_helperfunctions/questionanswer_llama2.py` & `querent-3.0.6/querent/kg/rel_helperfunctions/questionanswer_llama2.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/rel_helperfunctions/rel_normalize.py` & `querent-3.0.6/querent/kg/rel_helperfunctions/rel_normalize.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/kg/rel_helperfunctions/triple_to_json.py` & `querent-3.0.6/querent/kg/rel_helperfunctions/triple_to_json.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/logging/filters.py` & `querent-3.0.6/querent/logging/filters.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/logging/handlers.py` & `querent-3.0.6/querent/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/logging/logger.py` & `querent-3.0.6/querent/logging/logger.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/metric/adapters/promethus_adapter.py` & `querent-3.0.6/querent/metric/adapters/promethus_adapter.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/metric/metric_logging_handler.py` & `querent-3.0.6/querent/metric/metric_logging_handler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/metric/metric_registry.py` & `querent-3.0.6/querent/metric/metric_registry.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/processors/text_cleanup_processor.py` & `querent-3.0.6/querent/processors/text_cleanup_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/processors/text_processor.py` & `querent-3.0.6/querent/processors/text_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/querent/auto_scaler.py` & `querent-3.0.6/querent/querent/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/querent/querent.py` & `querent-3.0.6/querent/querent/querent.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/querent/resource_manager.py` & `querent-3.0.6/querent/querent/resource_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/storage/gcs_query.py` & `querent-3.0.6/querent/storage/gcs_query.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/storage/milvus_vectorevent_storage.py` & `querent-3.0.6/querent/storage/milvus_vectorevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/storage/neo4j_graphevent_storage.py` & `querent-3.0.6/querent/storage/neo4j_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/storage/postgres_graphevent_storage.py` & `querent-3.0.6/querent/storage/postgres_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/tools/web_page_extractor.py` & `querent-3.0.6/querent/tools/web_page_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/utils/webpage_extractor.py` & `querent-3.0.6/querent/utils/webpage_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/workflow/_helpers.py` & `querent-3.0.6/querent/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent/workflow/workflow.py` & `querent-3.0.6/querent/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent.egg-info/PKG-INFO` & `querent-3.0.6/querent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.5
+Version: 3.0.6
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
@@ -32,15 +32,15 @@
 Classifier: Topic :: Utilities
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
-Requires-Python: >=3.9, <=3.10
+Requires-Python: ==3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.4
 Requires-Dist: attrs==23.1.0
 Requires-Dist: azure-storage-blob==12.19.0
 Requires-Dist: beautifulsoup4==4.12.3
@@ -100,14 +100,16 @@
 Requires-Dist: slack-sdk==3.26.1
 Requires-Dist: spacy==3.7.2
 Requires-Dist: speechrecognition==3.10.1
 Requires-Dist: tika==2.6.0
 Requires-Dist: tensorflow==2.14.0
 Requires-Dist: transformers==4.36.0
 Requires-Dist: unidecode==1.3.7
+Provides-Extra: torch
+Requires-Dist: torch; extra == "torch"
 
 # Querent
 
 The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 
 ![image](https://github.com/Querent-ai/querent-ai/assets/61435908/39124a0c-3d9e-434f-9b54-9aa51dcefbd7)
```

### Comparing `querent-3.0.5/querent.egg-info/SOURCES.txt` & `querent-3.0.6/querent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `querent-3.0.5/querent.egg-info/requires.txt` & `querent-3.0.6/querent.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -59,7 +59,10 @@
 slack-sdk==3.26.1
 spacy==3.7.2
 speechrecognition==3.10.1
 tika==2.6.0
 tensorflow==2.14.0
 transformers==4.36.0
 unidecode==1.3.7
+
+[torch]
+torch
```

### Comparing `querent-3.0.5/setup.py` & `querent-3.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 torch_index_url = "https://download.pytorch.org/whl/cpu"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="querent",
-    version="3.0.5",
+    version="3.0.6",
     author="Querent AI",
     description="The Asynchronous Data Dynamo and Graph Neural Network Catalyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Querent-ai/querent-ai",
     project_urls={
         "Documentation": "https://github.com/Querent-ai/querent-ai/docs",
@@ -162,15 +162,18 @@
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Typing :: Typed",
     ],
-    python_requires=">=3.9, <=3.10",
-    dependency_links=[
-        f"{torch_index_url}/torch-2.0.1%2Bcpu-cp39-cp39-win_amd64.whl"  # Adjust this accordingly
-    ],
+    python_requires="==3.10",
     packages=find_packages(exclude=("tests", "tests.*")),
     install_requires=requirements,
+    extras_require={
+        "torch": ["torch"],
+    },
+    dependency_links=[
+        f"{torch_index_url}/torch-2.0.1%2Bcpu-cp310-cp310-linux_x86_64.whl",
+    ],
     license="Business Source License 1.1",
 )
```

