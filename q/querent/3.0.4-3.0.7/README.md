# Comparing `tmp/querent-3.0.4.tar.gz` & `tmp/querent-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querent-3.0.4.tar", last modified: Thu Apr 25 04:36:46 2024, max compression
+gzip compressed data, was "querent-3.0.7.tar", last modified: Sun Apr 28 01:12:11 2024, max compression
```

## Comparing `querent-3.0.4.tar` & `querent-3.0.7.tar`

### file list

```diff
@@ -1,262 +1,260 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.280917 querent-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-25 04:30:56.000000 querent-3.0.4/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)    16983 2024-04-25 04:36:46.276917 querent-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-25 04:30:56.000000 querent-3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.204917 querent-3.0.4/querent/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-25 04:30:56.000000 querent-3.0.4/querent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.208917 querent-3.0.4/querent/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-25 04:30:56.000000 querent-3.0.4/querent/callback/event_callback_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-25 04:30:56.000000 querent-3.0.4/querent/callback/event_callback_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.208917 querent-3.0.4/querent/channel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-25 04:30:56.000000 querent-3.0.4/querent/channel/channel_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.208917 querent-3.0.4/querent/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.212917 querent-3.0.4/querent/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.212917 querent-3.0.4/querent/collectors/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/aws/aws_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.216917 querent-3.0.4/querent/collectors/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/azure/azure_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/collector_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/collector_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/collector_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/collector_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.216917 querent-3.0.4/querent/collectors/drive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/drive/google_drive_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.216917 querent-3.0.4/querent/collectors/dropbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/dropbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/dropbox/dropbox_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.216917 querent-3.0.4/querent/collectors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/email/email_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/email/imap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.216917 querent-3.0.4/querent/collectors/fs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/fs/fs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.220917 querent-3.0.4/querent/collectors/gcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/gcs/gcs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.220917 querent-3.0.4/querent/collectors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/github/github_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.220917 querent-3.0.4/querent/collectors/jira/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/jira/jira_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.220917 querent-3.0.4/querent/collectors/news/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/news/news_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.220917 querent-3.0.4/querent/collectors/slack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/slack/slack_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.224917 querent-3.0.4/querent/collectors/webscaper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/webscaper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-25 04:30:56.000000 querent-3.0.4/querent/collectors/webscaper/web_scraper_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.224917 querent-3.0.4/querent/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/common_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.224917 querent-3.0.4/querent/common/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/errors/metric_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.228917 querent-3.0.4/querent/common/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/collected_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/collector_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/engine_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/file_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/ingested_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/ingested_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/ingested_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/ingested_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/querent_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/querent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/resource_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/types/workflow_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-25 04:30:56.000000 querent-3.0.4/querent/common/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.232917 querent-3.0.4/querent/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.232917 querent-3.0.4/querent/config/collector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/collector/collector_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.232917 querent-3.0.4/querent/config/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/core/gpt_llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/core/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/core/opensource_llm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.236917 querent-3.0.4/querent/config/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/engine/engine_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/graph_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.236917 querent-3.0.4/querent/config/ingestor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/ingestor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/ingestor/ingestor_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.236917 querent-3.0.4/querent/config/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/logger/logger_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.236917 querent-3.0.4/querent/config/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/metric/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.236917 querent-3.0.4/querent/config/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/resource/resource_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.236917 querent-3.0.4/querent/config/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-25 04:30:56.000000 querent-3.0.4/querent/config/workflow/workflow_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.240917 querent-3.0.4/querent/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.240917 querent-3.0.4/querent/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.240917 querent-3.0.4/querent/core/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13817 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/transformers/bert_ner_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/transformers/fixed_entities_set_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16897 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/transformers/gpt_llm_gpt_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-04-25 04:30:56.000000 querent-3.0.4/querent/core/transformers/relationship_extraction_llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.244917 querent-3.0.4/querent/dal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/dal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.244917 querent-3.0.4/querent/gnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/gnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.248917 querent-3.0.4/querent/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/graph_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/shacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-25 04:30:56.000000 querent-3.0.4/querent/graph/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.248917 querent-3.0.4/querent/ingestors/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.248917 querent-3.0.4/querent/ingestors/audio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/audio/audio_ingestors.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/base_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.248917 querent-3.0.4/querent/ingestors/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/code/code_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.248917 querent-3.0.4/querent/ingestors/csv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/csv/csv_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.252917 querent-3.0.4/querent/ingestors/doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/doc/doc_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.252917 querent-3.0.4/querent/ingestors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/email/email_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/email/email_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.252917 querent-3.0.4/querent/ingestors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/github/github_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.252917 querent-3.0.4/querent/ingestors/html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/html/html_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.252917 querent-3.0.4/querent/ingestors/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/images/image_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/ingestor_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/ingestor_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/json/json_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/pdfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/pdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/pdfs/pdf_ingestor_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/ppt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/ppt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/ppt/ppt_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/texts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/texts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/texts/text_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/video/video_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/xlsx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/xlsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/xlsx/xlsx_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.256917 querent-3.0.4/querent/ingestors/xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-25 04:30:56.000000 querent-3.0.4/querent/ingestors/xml/xml_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.260917 querent-3.0.4/querent/kg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.260917 querent-3.0.4/querent/kg/ner_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/attn_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/contextual_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/dependency_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/filter_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/fixed_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/fixed_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/ner_helperfunctions/ner_llm_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/querent_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.268917 querent-3.0.4/querent/kg/rel_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/contextual_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/embedding_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/filter_semantic_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/fixed_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/openai_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/openllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/questionanswer_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/rag_retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/rel_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-25 04:30:56.000000 querent-3.0.4/querent/kg/rel_helperfunctions/triple_to_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.268917 querent-3.0.4/querent/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 04:30:56.000000 querent-3.0.4/querent/logging/custom_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-25 04:30:56.000000 querent-3.0.4/querent/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-25 04:30:56.000000 querent-3.0.4/querent/logging/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-25 04:30:56.000000 querent-3.0.4/querent/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.268917 querent-3.0.4/querent/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.272917 querent-3.0.4/querent/metric/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/metric/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-25 04:30:56.000000 querent-3.0.4/querent/metric/adapters/promethus_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-25 04:30:56.000000 querent-3.0.4/querent/metric/base_metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-25 04:30:56.000000 querent-3.0.4/querent/metric/metric_logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-25 04:30:56.000000 querent-3.0.4/querent/metric/metric_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.272917 querent-3.0.4/querent/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 04:30:56.000000 querent-3.0.4/querent/processors/async_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-25 04:30:56.000000 querent-3.0.4/querent/processors/text_cleanup_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-25 04:30:56.000000 querent-3.0.4/querent/processors/text_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.272917 querent-3.0.4/querent/querent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/querent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-25 04:30:56.000000 querent-3.0.4/querent/querent/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-25 04:30:56.000000 querent-3.0.4/querent/querent/querent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-25 04:30:56.000000 querent-3.0.4/querent/querent/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/querent/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.276917 querent-3.0.4/querent/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-25 04:30:56.000000 querent-3.0.4/querent/storage/gcs_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-25 04:30:56.000000 querent-3.0.4/querent/storage/milvus_vectorevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-25 04:30:56.000000 querent-3.0.4/querent/storage/neo4j_graphevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-25 04:30:56.000000 querent-3.0.4/querent/storage/postgres_graphevent_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.276917 querent-3.0.4/querent/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-04-25 04:30:56.000000 querent-3.0.4/querent/tools/web_page_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.276917 querent-3.0.4/querent/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:30:56.000000 querent-3.0.4/querent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-25 04:30:56.000000 querent-3.0.4/querent/utils/webpage_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.276917 querent-3.0.4/querent/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 04:30:56.000000 querent-3.0.4/querent/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-04-25 04:30:56.000000 querent-3.0.4/querent/workflow/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-25 04:30:56.000000 querent-3.0.4/querent/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:36:46.276917 querent-3.0.4/querent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16983 2024-04-25 04:36:46.000000 querent-3.0.4/querent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-25 04:36:46.000000 querent-3.0.4/querent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:36:46.000000 querent-3.0.4/querent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 04:36:46.000000 querent-3.0.4/querent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 04:36:46.000000 querent-3.0.4/querent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 04:36:46.280917 querent-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-25 04:30:56.000000 querent-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.410132 querent-3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-28 01:07:38.000000 querent-3.0.7/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    16950 2024-04-28 01:12:11.410132 querent-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-28 01:07:38.000000 querent-3.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.334132 querent-3.0.7/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-28 01:07:38.000000 querent-3.0.7/querent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.338132 querent-3.0.7/querent/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-28 01:07:38.000000 querent-3.0.7/querent/callback/event_callback_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-28 01:07:38.000000 querent-3.0.7/querent/callback/event_callback_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.338132 querent-3.0.7/querent/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-28 01:07:38.000000 querent-3.0.7/querent/channel/channel_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.338132 querent-3.0.7/querent/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.342132 querent-3.0.7/querent/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.342132 querent-3.0.7/querent/collectors/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/aws/aws_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.342132 querent-3.0.7/querent/collectors/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/azure/azure_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/collector_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/collector_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/collector_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/collector_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.346132 querent-3.0.7/querent/collectors/drive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/drive/google_drive_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.346132 querent-3.0.7/querent/collectors/dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/dropbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/dropbox/dropbox_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.346132 querent-3.0.7/querent/collectors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/email/email_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/email/imap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.346132 querent-3.0.7/querent/collectors/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/fs/fs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.346132 querent-3.0.7/querent/collectors/gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/gcs/gcs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.350132 querent-3.0.7/querent/collectors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/github/github_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.350132 querent-3.0.7/querent/collectors/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/jira/jira_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.350132 querent-3.0.7/querent/collectors/news/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/news/news_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.350132 querent-3.0.7/querent/collectors/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/slack/slack_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.350132 querent-3.0.7/querent/collectors/webscaper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/webscaper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-28 01:07:38.000000 querent-3.0.7/querent/collectors/webscaper/web_scraper_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.354132 querent-3.0.7/querent/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/common_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.354132 querent-3.0.7/querent/common/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/errors/metric_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.358132 querent-3.0.7/querent/common/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/collected_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/collector_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/engine_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/file_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/ingested_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/ingested_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/ingested_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/ingested_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/querent_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/querent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/resource_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/types/workflow_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-28 01:07:38.000000 querent-3.0.7/querent/common/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.362132 querent-3.0.7/querent/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.362132 querent-3.0.7/querent/config/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/collector/collector_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.362132 querent-3.0.7/querent/config/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/core/gpt_llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/core/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/core/opensource_llm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.362132 querent-3.0.7/querent/config/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/engine/engine_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/graph_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.362132 querent-3.0.7/querent/config/ingestor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/ingestor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/ingestor/ingestor_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.366132 querent-3.0.7/querent/config/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/logger/logger_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.366132 querent-3.0.7/querent/config/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/metric/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.366132 querent-3.0.7/querent/config/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/resource/resource_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.366132 querent-3.0.7/querent/config/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-28 01:07:38.000000 querent-3.0.7/querent/config/workflow/workflow_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.366132 querent-3.0.7/querent/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.366132 querent-3.0.7/querent/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-28 01:07:38.000000 querent-3.0.7/querent/core/base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.370132 querent-3.0.7/querent/core/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/core/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-04-28 01:07:38.000000 querent-3.0.7/querent/core/transformers/bert_ner_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-28 01:07:38.000000 querent-3.0.7/querent/core/transformers/fixed_entities_set_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-04-28 01:07:38.000000 querent-3.0.7/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13002 2024-04-28 01:07:38.000000 querent-3.0.7/querent/core/transformers/gpt_llm_gpt_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-04-28 01:07:38.000000 querent-3.0.7/querent/core/transformers/relationship_extraction_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.370132 querent-3.0.7/querent/dal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/dal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.370132 querent-3.0.7/querent/gnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/gnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.374132 querent-3.0.7/querent/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-28 01:07:38.000000 querent-3.0.7/querent/graph/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-28 01:07:38.000000 querent-3.0.7/querent/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-28 01:07:38.000000 querent-3.0.7/querent/graph/graph_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-28 01:07:38.000000 querent-3.0.7/querent/graph/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-28 01:07:38.000000 querent-3.0.7/querent/graph/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-28 01:07:38.000000 querent-3.0.7/querent/graph/shacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-28 01:07:38.000000 querent-3.0.7/querent/graph/subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-28 01:07:38.000000 querent-3.0.7/querent/graph/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.374132 querent-3.0.7/querent/ingestors/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.374132 querent-3.0.7/querent/ingestors/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/audio/audio_ingestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/base_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.378132 querent-3.0.7/querent/ingestors/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/code/code_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.378132 querent-3.0.7/querent/ingestors/csv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/csv/csv_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.378132 querent-3.0.7/querent/ingestors/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/doc/doc_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.378132 querent-3.0.7/querent/ingestors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/email/email_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/email/email_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.378132 querent-3.0.7/querent/ingestors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/github/github_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.378132 querent-3.0.7/querent/ingestors/html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/html/html_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.386132 querent-3.0.7/querent/ingestors/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/images/image_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/ingestor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/ingestor_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.386132 querent-3.0.7/querent/ingestors/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/json/json_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.390132 querent-3.0.7/querent/ingestors/pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/pdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/pdfs/pdf_ingestor_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.390132 querent-3.0.7/querent/ingestors/ppt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/ppt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/ppt/ppt_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.390132 querent-3.0.7/querent/ingestors/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/texts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/texts/text_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.390132 querent-3.0.7/querent/ingestors/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/video/video_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.390132 querent-3.0.7/querent/ingestors/xlsx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/xlsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/xlsx/xlsx_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.390132 querent-3.0.7/querent/ingestors/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-28 01:07:38.000000 querent-3.0.7/querent/ingestors/xml/xml_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.390132 querent-3.0.7/querent/kg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.394132 querent-3.0.7/querent/kg/ner_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/ner_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/ner_helperfunctions/attn_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/ner_helperfunctions/contextual_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/ner_helperfunctions/dependency_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/ner_helperfunctions/filter_triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/ner_helperfunctions/fixed_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/ner_helperfunctions/fixed_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/ner_helperfunctions/ner_llm_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/querent_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.398132 querent-3.0.7/querent/kg/rel_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/rel_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/rel_helperfunctions/contextual_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/rel_helperfunctions/embedding_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/rel_helperfunctions/fixed_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/rel_helperfunctions/openai_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/rel_helperfunctions/openllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/rel_helperfunctions/questionanswer_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/rel_helperfunctions/rel_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-28 01:07:38.000000 querent-3.0.7/querent/kg/rel_helperfunctions/triple_to_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.402132 querent-3.0.7/querent/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-28 01:07:38.000000 querent-3.0.7/querent/logging/custom_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-28 01:07:38.000000 querent-3.0.7/querent/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-28 01:07:38.000000 querent-3.0.7/querent/logging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-28 01:07:38.000000 querent-3.0.7/querent/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.402132 querent-3.0.7/querent/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.402132 querent-3.0.7/querent/metric/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/metric/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-28 01:07:38.000000 querent-3.0.7/querent/metric/adapters/promethus_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-28 01:07:38.000000 querent-3.0.7/querent/metric/base_metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-28 01:07:38.000000 querent-3.0.7/querent/metric/metric_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-28 01:07:38.000000 querent-3.0.7/querent/metric/metric_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.402132 querent-3.0.7/querent/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-28 01:07:38.000000 querent-3.0.7/querent/processors/async_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-28 01:07:38.000000 querent-3.0.7/querent/processors/text_cleanup_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-28 01:07:38.000000 querent-3.0.7/querent/processors/text_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.406132 querent-3.0.7/querent/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/querent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-28 01:07:38.000000 querent-3.0.7/querent/querent/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-28 01:07:38.000000 querent-3.0.7/querent/querent/querent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-28 01:07:38.000000 querent-3.0.7/querent/querent/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/querent/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.406132 querent-3.0.7/querent/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-28 01:07:38.000000 querent-3.0.7/querent/storage/gcs_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-28 01:07:38.000000 querent-3.0.7/querent/storage/milvus_vectorevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-28 01:07:38.000000 querent-3.0.7/querent/storage/neo4j_graphevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-28 01:07:38.000000 querent-3.0.7/querent/storage/postgres_graphevent_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.406132 querent-3.0.7/querent/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-04-28 01:07:38.000000 querent-3.0.7/querent/tools/web_page_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.410132 querent-3.0.7/querent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 01:07:38.000000 querent-3.0.7/querent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-28 01:07:38.000000 querent-3.0.7/querent/utils/webpage_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.410132 querent-3.0.7/querent/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 01:07:38.000000 querent-3.0.7/querent/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-04-28 01:07:38.000000 querent-3.0.7/querent/workflow/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-28 01:07:38.000000 querent-3.0.7/querent/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 01:12:11.410132 querent-3.0.7/querent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16950 2024-04-28 01:12:11.000000 querent-3.0.7/querent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-28 01:12:11.000000 querent-3.0.7/querent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-28 01:12:11.000000 querent-3.0.7/querent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-28 01:12:11.000000 querent-3.0.7/querent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 01:12:11.000000 querent-3.0.7/querent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 01:12:11.410132 querent-3.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-28 01:07:38.000000 querent-3.0.7/setup.py
```

### Comparing `querent-3.0.4/LICENCE` & `querent-3.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/PKG-INFO` & `querent-3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.4
+Version: 3.0.7
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
@@ -32,35 +32,33 @@
 Classifier: Topic :: Utilities
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.10, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: aiofiles==23.2.1
-Requires-Dist: aiohttp==3.9.3
+Requires-Dist: aiohttp==3.9.4
 Requires-Dist: attrs==23.1.0
 Requires-Dist: azure-storage-blob==12.19.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: boto3==1.26.146
 Requires-Dist: botocore==1.29.146
 Requires-Dist: bs4==0.0.1
 Requires-Dist: cachetools==5.3.3
 Requires-Dist: coverage==7.3.3
 Requires-Dist: dropbox==11.36.2
-Requires-Dist: faiss-cpu==1.7.4
+Requires-Dist: fastembed==0.2.6
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: gensim==4.3.2
 Requires-Dist: google-api-python-client==2.105.0
 Requires-Dist: google-cloud-storage==2.14.0
-Requires-Dist: google-cloud-storage==2.14.0
-Requires-Dist: google-cloud-storage==2.14.0
 Requires-Dist: hdbscan==0.8.33
 Requires-Dist: jira==3.6.0
 Requires-Dist: jmespath==1.0.1
 Requires-Dist: joblib==1.2.0
 Requires-Dist: json5==0.9.24
 Requires-Dist: jsonmerge==1.9.0
 Requires-Dist: jsonschema==4.17.3
@@ -99,17 +97,19 @@
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests_html==0.10.0
 Requires-Dist: slack-sdk==3.26.1
 Requires-Dist: slack-sdk==3.26.1
 Requires-Dist: spacy==3.7.2
 Requires-Dist: speechrecognition==3.10.1
 Requires-Dist: tika==2.6.0
+Requires-Dist: tensorflow==2.14.0
 Requires-Dist: transformers==4.36.0
 Requires-Dist: unidecode==1.3.7
-Requires-Dist: sentence-transformers==2.2.2
+Provides-Extra: torch
+Requires-Dist: torch; extra == "torch"
 
 # Querent
 
 The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 
 ![image](https://github.com/Querent-ai/querent-ai/assets/61435908/39124a0c-3d9e-434f-9b54-9aa51dcefbd7)
```

### Comparing `querent-3.0.4/README.md` & `querent-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/__init__.py` & `querent-3.0.7/querent/__init__.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/callback/event_callback_dispatcher.py` & `querent-3.0.7/querent/callback/event_callback_dispatcher.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/callback/event_callback_interface.py` & `querent-3.0.7/querent/callback/event_callback_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/channel/channel_interface.py` & `querent-3.0.7/querent/channel/channel_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/aws/aws_collector.py` & `querent-3.0.7/querent/collectors/aws/aws_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/azure/azure_collector.py` & `querent-3.0.7/querent/collectors/azure/azure_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/collector_errors.py` & `querent-3.0.7/querent/collectors/collector_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/collector_factory.py` & `querent-3.0.7/querent/collectors/collector_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/collector_resolver.py` & `querent-3.0.7/querent/collectors/collector_resolver.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/drive/google_drive_collector.py` & `querent-3.0.7/querent/collectors/drive/google_drive_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/dropbox/dropbox_collector.py` & `querent-3.0.7/querent/collectors/dropbox/dropbox_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/email/email_collector.py` & `querent-3.0.7/querent/collectors/email/email_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/email/imap.py` & `querent-3.0.7/querent/collectors/email/imap.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/fs/fs_collector.py` & `querent-3.0.7/querent/collectors/fs/fs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/gcs/gcs_collector.py` & `querent-3.0.7/querent/collectors/gcs/gcs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/github/github_collector.py` & `querent-3.0.7/querent/collectors/github/github_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/jira/jira_collector.py` & `querent-3.0.7/querent/collectors/jira/jira_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/news/news_collector.py` & `querent-3.0.7/querent/collectors/news/news_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/slack/slack_collector.py` & `querent-3.0.7/querent/collectors/slack/slack_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/collectors/webscaper/web_scraper_collector.py` & `querent-3.0.7/querent/collectors/webscaper/web_scraper_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/common/common_errors.py` & `querent-3.0.7/querent/common/common_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/common/errors/metric_errors.py` & `querent-3.0.7/querent/common/errors/metric_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/common/types/collected_bytes.py` & `querent-3.0.7/querent/common/types/collected_bytes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/common/types/file_buffer.py` & `querent-3.0.7/querent/common/types/file_buffer.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/common/types/ingested_code.py` & `querent-3.0.7/querent/common/types/ingested_code.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/common/types/ingested_images.py` & `querent-3.0.7/querent/common/types/ingested_images.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/common/types/ingested_messages.py` & `querent-3.0.7/querent/common/types/ingested_messages.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/common/types/ingested_tokens.py` & `querent-3.0.7/querent/common/types/ingested_tokens.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/common/types/querent_queue.py` & `querent-3.0.7/querent/common/types/querent_queue.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/common/uri.py` & `querent-3.0.7/querent/common/uri.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/config/collector/collector_config.py` & `querent-3.0.7/querent/config/collector/collector_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/config/config.py` & `querent-3.0.7/querent/config/config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/config/core/gpt_llm_config.py` & `querent-3.0.7/querent/config/core/gpt_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/config/core/llm_config.py` & `querent-3.0.7/querent/config/core/llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/config/core/opensource_llm_config.py` & `querent-3.0.7/querent/config/core/opensource_llm_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,15 @@
     description: str = "An engine for extracting relationships"
     version: str = "0.0.1"
     logger: str = "RelationshipExtractor.engine_config"
     model_type: str = 'llama'
     model_path: str = './tests/llama-2-7b-chat.Q5_K_M.gguf' 
     grammar_file_path: str = './querent/kg/rel_helperfunctions/json.gbnf'
     qa_template: str = Field(default=None)
-    vector_store_path: str = "./querent/kg/rel_helperfunctions/vectorstores/"
     emb_model_name: str = 'sentence-transformers/all-MiniLM-L6-v2'
-    rag_approach: bool = False
     is_confined_search: bool = False
     spacy_model_path: str = 'en_core_web_lg'
     nltk_path: str = '/model/nltk_data'
 
     def __init__(self, config_source=None, **kwargs):
         config_data = {}
         config_data.update(kwargs)
```

### Comparing `querent-3.0.4/querent/config/engine/engine_config.py` & `querent-3.0.7/querent/config/engine/engine_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/config/graph_config.py` & `querent-3.0.7/querent/config/graph_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/config/ingestor/ingestor_config.py` & `querent-3.0.7/querent/config/ingestor/ingestor_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/config/metric/prometheus.py` & `querent-3.0.7/querent/config/metric/prometheus.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/config/resource/resource_config.py` & `querent-3.0.7/querent/config/resource/resource_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/config/workflow/workflow_config.py` & `querent-3.0.7/querent/config/workflow/workflow_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/core/base_engine.py` & `querent-3.0.7/querent/core/base_engine.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/core/transformers/bert_ner_opensourcellm.py` & `querent-3.0.7/querent/core/transformers/bert_ner_opensourcellm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from unidecode import unidecode
 from transformers import AutoTokenizer
 from querent.kg.ner_helperfunctions.fixed_predicate import FixedPredicateExtractor
 from querent.common.types.ingested_images import IngestedImages
 from querent.config.core.opensource_llm_config import Opensource_LLM_Config
 from querent.core.transformers.relationship_extraction_llm import RelationExtractor
 from querent.kg.rel_helperfunctions.contextual_predicate import process_data
 from querent.kg.ner_helperfunctions.contextual_embeddings import EntityEmbeddingExtractor
@@ -20,15 +19,14 @@
 from querent.kg.querent_kg import QuerentKG
 from querent.config.graph_config import GraphConfig
 from querent.kg.ner_helperfunctions.attn_scores import EntityAttentionExtractor
 from querent.kg.ner_helperfunctions.filter_triples import TripleFilter
 from querent.config.core.llm_config import LLM_Config
 from querent.kg.rel_helperfunctions.triple_to_json import TripleToJsonConverter
 from querent.kg.rel_helperfunctions.embedding_store import EmbeddingStore
-from querent.kg.rel_helperfunctions.filter_semantic_triples import SemanticTripleFilter
 
 """
     BERTLLM is a class derived from BaseEngine designed for processing language models, particularly focusing on named entity recognition and relationship extraction in text. It integrates various components for handling different types of input data (messages, images, code, tokens), extracting entities, filtering relevant information, and constructing knowledge graphs.
 
     Key functionalities include:
     - Initializing with a specific configuration for named entity recognition (NER) and language model processing.
     - Validating the presence of NER models and tokenizers.
@@ -41,40 +39,44 @@
     """
 
 
 class BERTLLM(BaseEngine):
     def __init__(
         self,
         input_queue:QuerentQueue,
-        config: LLM_Config
+        config: LLM_Config,
+        Embedding=None
     ):  
         self.logger = setup_logger(__name__, "BERTLLM")
         super().__init__(input_queue)
         self.skip_inferences=config.skip_inferences
         try:
-            if not self.skip_inferences:
-                mock_config = Opensource_LLM_Config(qa_template=config.user_context,
-                                                    model_type = config.rel_model_type,
-                                                    model_path = config.rel_model_path,
-                                                    grammar_file_path = config.grammar_file_path,
-                                                    emb_model_name = config.emb_model_name,
-                                                    spacy_model_path = config.spacy_model_path,
-                                                    nltk_path = config.nltk_path
-                                                    )
-                self.semantic_extractor = RelationExtractor(mock_config)
             self.graph_config = GraphConfig(identifier=config.name)
             self.contextual_graph = QuerentKG(self.graph_config)
             self.semantic_graph = QuerentKG(self.graph_config)
             self.file_buffer = FileBuffer()
             self.ner_tokenizer = AutoTokenizer.from_pretrained(config.ner_model_name)
             self.ner_model = NER_LLM.load_model(config.ner_model_name, "NER")
             self.ner_llm_instance = NER_LLM(provided_tokenizer=self.ner_tokenizer, provided_model=self.ner_model)
             self.nlp_model = NER_LLM.set_nlp_model(config.spacy_model_path)
             self.nlp_model = NER_LLM.get_class_variable()
-            self.create_emb = EmbeddingStore(inference_api_key=config.huggingface_token)
+            if not Embedding:
+                self.create_emb = EmbeddingStore()
+            else:
+                self.create_emb = Embedding
+            if not self.skip_inferences:
+                mock_config = Opensource_LLM_Config(qa_template=config.user_context,
+                                                    model_type = config.rel_model_type,
+                                                    model_path = config.rel_model_path,
+                                                    grammar_file_path = config.grammar_file_path,
+                                                    emb_model_name = config.emb_model_name,
+                                                    spacy_model_path = config.spacy_model_path,
+                                                    nltk_path = config.nltk_path
+                                                    )
+                self.semantic_extractor = RelationExtractor(mock_config,self.create_emb)
             self.attn_scores_instance = EntityAttentionExtractor(model=self.ner_model, tokenizer=self.ner_tokenizer)
             self.enable_filtering = config.enable_filtering
             self.filter_params = config.filter_params or {}
             self.triple_filter = None
             if self.enable_filtering:
                 self.triple_filter = TripleFilter(**self.filter_params)
             self.sample_entities = config.sample_entities
@@ -95,15 +97,14 @@
                 self.predicate_context_extractor = FixedPredicateExtractor(fixed_predicates=self.fixed_relationships, predicate_types=self.sample_relationships,model = self.nlp_model)
             elif self.sample_relationships:
                 self.predicate_context_extractor = FixedPredicateExtractor(predicate_types=self.sample_relationships,model = self.nlp_model)
             else:
                 self.predicate_context_extractor = None
             self.user_context = config.user_context
             self.isConfinedSearch = config.is_confined_search
-            self.semantictriplefilter = SemanticTripleFilter()
         except Exception as e:
             self.logger.error("Error initializing BERT LLM Class", e)
             raise e
         
  
 
     def validate(self) -> bool:
@@ -199,15 +200,14 @@
                         filtered_triples = pairs_with_predicates
                 else:
                     filtered_triples = pairs_with_predicates
                 if not filtered_triples:
                     return
                 elif not self.skip_inferences:
                     relationships = self.semantic_extractor.process_tokens(filtered_triples)
-                    relationships = self.semantictriplefilter.filter_triples(relationships)
                     if len(relationships) > 0:
                         embedding_triples = self.create_emb.generate_embeddings(relationships)
                         if self.sample_relationships:
                             embedding_triples = self.predicate_context_extractor.process_predicate_types(embedding_triples)
                         for triple in embedding_triples:
                             if not self.termination_event.is_set():
                                 graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
```

### Comparing `querent-3.0.4/querent/core/transformers/fixed_entities_set_opensourcellm.py` & `querent-3.0.7/querent/core/transformers/fixed_entities_set_opensourcellm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from unidecode import unidecode
 from transformers import AutoTokenizer
 from querent.kg.ner_helperfunctions.fixed_predicate import FixedPredicateExtractor
 from querent.common.types.ingested_images import IngestedImages
 from querent.config.core.opensource_llm_config import Opensource_LLM_Config
 from querent.core.transformers.relationship_extraction_llm import RelationExtractor
 from querent.kg.rel_helperfunctions.contextual_predicate import process_data
 from querent.kg.ner_helperfunctions.fixed_entities import FixedEntityExtractor
@@ -11,31 +10,29 @@
 from querent.common.types.querent_event import EventState, EventType
 from querent.core.base_engine import BaseEngine
 from querent.common.types.ingested_tokens import IngestedTokens
 from querent.common.types.ingested_messages import IngestedMessages
 from querent.common.types.ingested_code import IngestedCode
 from querent.common.types.querent_queue import QuerentQueue
 from querent.common.types.file_buffer import FileBuffer
-from querent.kg.rel_helperfunctions.filter_semantic_triples import SemanticTripleFilter
 from querent.logging.logger import setup_logger
 from querent.kg.querent_kg import QuerentKG
 from querent.config.graph_config import GraphConfig
 from querent.kg.ner_helperfunctions.filter_triples import TripleFilter
 from querent.config.core.llm_config import LLM_Config
 from querent.kg.rel_helperfunctions.triple_to_json import TripleToJsonConverter
 from querent.kg.rel_helperfunctions.embedding_store import EmbeddingStore
-import time
-
 
 
 class Fixed_Entities_LLM(BaseEngine):
     def __init__(
         self,
         input_queue:QuerentQueue,
-        config: LLM_Config
+        config: LLM_Config,
+        Embedding=None
     ):  
         self.logger = setup_logger(__name__, "Fixed_Entities_LLM")
         super().__init__(input_queue)
         self.skip_inferences=config.skip_inferences
         if not self.skip_inferences:
             mock_config = Opensource_LLM_Config(qa_template=config.user_context,
                                                 model_type = config.rel_model_type,
@@ -52,15 +49,18 @@
         self.semantic_graph = QuerentKG(self.graph_config)
         self.file_buffer = FileBuffer()
         self.ner_tokenizer = AutoTokenizer.from_pretrained(config.ner_model_name)
         self.ner_llm_instance = NER_LLM(provided_tokenizer=self.ner_tokenizer, provided_model= "dummy")
         self.nlp_model = NER_LLM.set_nlp_model(config.spacy_model_path)
         self.nlp_model = NER_LLM.get_class_variable()
         huggingface_token = config.huggingface_token
-        self.create_emb = EmbeddingStore(inference_api_key=huggingface_token)
+        if Embedding is None:
+            self.create_emb = EmbeddingStore()
+        else:
+            self.create_emb = Embedding
         self.enable_filtering = config.enable_filtering
         self.filter_params = config.filter_params or {}
         self.triple_filter = None
         if self.enable_filtering:
             self.triple_filter = TripleFilter(**self.filter_params)
         self.sample_entities = config.sample_entities
         self.fixed_entities = config.fixed_entities
@@ -80,15 +80,14 @@
             self.predicate_context_extractor = FixedPredicateExtractor(fixed_predicates=self.fixed_relationships, predicate_types=self.sample_relationships,model = self.nlp_model)
         elif self.sample_relationships:
             self.predicate_context_extractor = FixedPredicateExtractor(predicate_types=self.sample_relationships,model = self.nlp_model)
         else:
             self.predicate_context_extractor = None
         self.user_context = config.user_context
         self.isConfinedSearch = config.is_confined_search
-        self.semantictriplefilter = SemanticTripleFilter()
         
  
 
     def validate(self) -> bool:
         return self.ner_tokenizer is not None
 
     def process_messages(self, data: IngestedMessages):
@@ -163,15 +162,14 @@
                 filtered_triples = process_data(doc_entity_pairs, file)
                 if not filtered_triples:
                     self.logger.debug("No entity pairs")
                     return
                 elif not self.skip_inferences:
                     relationships = self.semantic_extractor.process_tokens(filtered_triples)
                     self.logger.debug(f"length of relationships {len(relationships)}")
-                    relationships = self.semantictriplefilter.filter_triples(relationships)
                     if len(relationships) > 0:
                         embedding_triples = self.create_emb.generate_embeddings(relationships)
                         if self.sample_relationships:
                             embedding_triples = self.predicate_context_extractor.process_predicate_types(embedding_triples)
                         for triple in embedding_triples:
                             if not self.termination_event.is_set():
                                 graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
```

### Comparing `querent-3.0.4/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py` & `querent-3.0.7/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import asyncio
 import json
-import re
 from querent.core.transformers.fixed_entities_set_opensourcellm import Fixed_Entities_LLM
 from querent.kg.ner_helperfunctions.fixed_predicate import FixedPredicateExtractor
 from querent.config.core.gpt_llm_config import GPTConfig
 from querent.core.transformers.bert_ner_opensourcellm import BERTLLM
 from querent.common.types.ingested_images import IngestedImages
 from querent.kg.ner_helperfunctions.ner_llm_transformer import NER_LLM
 from querent.kg.rel_helperfunctions.openai_functions import FunctionRegistry
@@ -70,19 +68,19 @@
                 raise ValueError("If specific predicates are provided, their types should also be provided.")
             if self.fixed_relationships and self.sample_relationships:
                 self.predicate_context_extractor = FixedPredicateExtractor(fixed_predicates=self.fixed_relationships, predicate_types=self.sample_relationships,  model = self.nlp_model)
             elif self.sample_relationships:
                 self.predicate_context_extractor = FixedPredicateExtractor(predicate_types=self.sample_relationships,  model = self.nlp_model)
             else:
                 self.predicate_context_extractor = None
-            self.create_emb = EmbeddingStore(inference_api_key=config.huggingface_token)
+            self.create_emb = EmbeddingStore()
             if config.is_confined_search:
-                self.llm_instance = Fixed_Entities_LLM(input_queue, llm_config)
+                self.llm_instance = Fixed_Entities_LLM(input_queue, llm_config, self.create_emb)
             else :
-                self.llm_instance = BERTLLM(input_queue, llm_config)
+                self.llm_instance = BERTLLM(input_queue, llm_config, self.create_emb)
             self.rel_model_name = config.rel_model_name
             if config.openai_api_key:
                 self.gpt_llm = OpenAI(api_key=config.openai_api_key)
             else:
                 self.gpt_llm = OpenAI()
             self.function_registry = FunctionRegistry()
```

### Comparing `querent-3.0.4/querent/core/transformers/relationship_extraction_llm.py` & `querent-3.0.7/querent/core/transformers/relationship_extraction_llm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 from typing import Any, List, Tuple
 from querent.kg.rel_helperfunctions.embedding_store import EmbeddingStore
 from querent.kg.rel_helperfunctions.questionanswer_llama2 import QASystem
-from querent.kg.rel_helperfunctions.rag_retriever import RAGRetriever
 from querent.kg.rel_helperfunctions.rel_normalize import TextNormalizer
 from querent.logging.logger import setup_logger
 from querent.config.core.opensource_llm_config import Opensource_LLM_Config
 from llama_cpp import LlamaGrammar
 
 import ast
 
@@ -40,32 +39,28 @@
         extract_relationships(triples):
             Extracts relationships from the given triples.
         trim_triples(data):
             Trims the given data to a more concise format.
     """
 
 class RelationExtractor():
-    def __init__(self, config: Opensource_LLM_Config):  
+    def __init__(self, config: Opensource_LLM_Config, Embedding=None):  
         self.logger = setup_logger(config.logger, "RelationshipExtractor")
         try:
             super().__init__()
             self.config = config
-            self.create_emb = EmbeddingStore(vector_store_path=config.vector_store_path)
+            if Embedding is None:
+                self.create_emb = EmbeddingStore()
+            else:
+                self.create_emb = Embedding
             self.qa_system = QASystem(
                 rel_model_path=config.model_path,
                 rel_model_type=config.model_type,
                 )
             self.grammar = LlamaGrammar.from_file(file = config.grammar_file_path)
-            self.rag_approach = config.rag_approach
-            if  self.rag_approach == True:
-                self.rag_retriever = RAGRetriever(
-                faiss_index_path=config.get_faiss_index_path(),
-                emb_model_name=config.emb_model_name,
-                embedding_store=self.create_emb,
-                logger=self.logger)
             self.is_confined_search = config.is_confined_search
         except Exception as e:
             self.logger.error(f"Initialization failed: {e}")
             raise Exception(f"Initialization failed: {e}")
         
     def validate(self, data) -> bool:
         try:
@@ -103,16 +98,14 @@
             self.logger.error(f"Error in validation: {e}")
             return False
     
     def process_tokens(self, payload):
         try:
             triples = payload
             trimmed_triples = self.normalizetriples_buildindex(triples)
-            if self.rag_approach == True:
-                self.rag_retriever.build_faiss_index(trimmed_triples)
             relationships = self.extract_relationships(triples)
         
             return relationships
         
         except Exception as e:
             self.logger.error(f"Error in processing event: {e}")
             raise Exception(f"Invalid in processing event: {e}")
@@ -145,41 +138,14 @@
                     "context": input2_data.get("context", ""),
                     "file_path": input2_data.get("file_path", ""),
                     "subject_type": input1.get("subject_type","Unlabeled"),
                     "object_type": input1.get("object_type","Unlabeled")
                 }),
                 input1.get("object","")
             )
-            # else:
-            #         if input1.get("subject","").lower() in input2_data.get("entity1_nn_chunk","").lower or input2_data.get("entity1_nn_chunk","").lower in input1.get("subject","").lower() or input2_data.get("entity1_nn_chunk","").lower == input1.get("subject","").lower():
-            #             triple = (
-            #             input1.get("subject",""),
-            #             json.dumps({
-            #                 "predicate": input1.get("predicate",""),
-            #                 "predicate_type": input1.get("predicate_type","Unlabeled"),
-            #                 "context": input2_data.get("context", ""),
-            #                 "file_path": input2_data.get("file_path", ""),
-            #                 "subject_type": input2_data.get("entity1_label","Unlabeled"),
-            #                 "object_type": input2_data.get("entity2_label","Unlabeled")
-            #             }),
-            #             input1.get("object","")
-            #         )
-            #         else:
-            #             triple = (
-            #             input1.get("subject",""),
-            #             json.dumps({
-            #                 "predicate": input1.get("predicate",""),
-            #                 "predicate_type": input1.get("predicate_type","Unlabeled"),
-            #                 "context": input2_data.get("context", ""),
-            #                 "file_path": input2_data.get("file_path", ""),
-            #                 "subject_type": input2.get("entity2_label","Unlabeled"),
-            #                 "object_type": input1.get("entity1_label","Unlabeled")
-            #             }),
-            #             input1.get("object","")
-                    # )
             return triple
         except Exception as e:
             self.logger.error(f"Error in creating semantic triple: {e}")
             raise Exception(f"Error in creating semantic triple: {e}")
         
     def replace_entities(self, text, entity1, entity2):
         data = json.loads(text)
@@ -196,43 +162,36 @@
         return data
 
     def extract_relationships(self, triples):
         try:
             self.logger.debug(f"Length of identified triples {len(triples)}")
             updated_triples = []
             for _, predicate_str, _ in triples:
-                documents=[]
                 data = json.loads(predicate_str)
                 context = data['context']
                 predicate = predicate_str if isinstance(predicate_str, dict) else json.loads(predicate_str)
-                if self.rag_approach == True:
-                    db = self.rag_retriever.load_faiss_index()
-                    prompt=("What is the relationship between {entity1} and the Object is {entity2}.").format(entity1=predicate.get('entity1_nn_chunk', ''), entity2=predicate.get('entity2_nn_chunk', ''))
-                    top_docs = self.rag_retriever.retrieve_documents(db, prompt=prompt)
-                    documents = top_docs
-                else:
-                    query = """Please analyze the provided context and two entities. Use this information to answer the users query below.
+                query = """Please analyze the provided context and two entities. Use this information to answer the users query below.
 Context: {context}
 Entity 1: {entity1} and Entity 2: {entity2}
 Query:{question}
 Answer:"""
-                    if not self.config.qa_template:
-                        question = "In the context of reservoir studies, identify the subject, predicate, and object in a semantic triple framework, focusing on reservoir attributes (e.g., porosity, permeability), processes (e.g., influences, determines), and outcomes (e.g., recovery efficiency). Specify the types for the subject (attribute), predicate (process), and object (outcome)."
-                        query = query.format(question = question, context = context, entity1=predicate.get('entity1_nn_chunk', ''), entity2=predicate.get('entity2_nn_chunk', ''))   
-                    else:
-                        question = self.config.qa_template
-                        query = query.format(question = question, context = context, entity1=predicate.get('entity1_nn_chunk', ''), entity2=predicate.get('entity2_nn_chunk', ''))    
-                    answer_relation = self.qa_system.ask_question(prompt=query, llm=self.qa_system.llm, grammar=self.grammar)
-                    try:
-                        choices_text = answer_relation['choices'][0]['text']
-                        answer_relation = self.replace_entities(choices_text,entity1=predicate.get('entity1_nn_chunk', ''), entity2=predicate.get('entity2_nn_chunk'))
-                        updated_triple= self.create_semantic_triple(answer_relation, predicate_str)
-                        updated_triples.append(updated_triple)
-                    except Exception as e:
-                        continue
+                if not self.config.qa_template:
+                    question = "In the context of reservoir studies, identify the subject, predicate, and object in a semantic triple framework, focusing on reservoir attributes (e.g., porosity, permeability), processes (e.g., influences, determines), and outcomes (e.g., recovery efficiency). Specify the types for the subject (attribute), predicate (process), and object (outcome)."
+                    query = query.format(question = question, context = context, entity1=predicate.get('entity1_nn_chunk', ''), entity2=predicate.get('entity2_nn_chunk', ''))   
+                else:
+                    question = self.config.qa_template
+                    query = query.format(question = question, context = context, entity1=predicate.get('entity1_nn_chunk', ''), entity2=predicate.get('entity2_nn_chunk', ''))    
+                answer_relation = self.qa_system.ask_question(prompt=query, llm=self.qa_system.llm, grammar=self.grammar)
+                try:
+                    choices_text = answer_relation['choices'][0]['text']
+                    answer_relation = self.replace_entities(choices_text,entity1=predicate.get('entity1_nn_chunk', ''), entity2=predicate.get('entity2_nn_chunk'))
+                    updated_triple= self.create_semantic_triple(answer_relation, predicate_str)
+                    updated_triples.append(updated_triple)
+                except Exception as e:
+                    continue
             return updated_triples
         except Exception as e:
             self.logger.error(f"Error in extracting relationships: {e}")
 
     def trim_triples(self, data):
         try:
             trimmed_data = []
```

### Comparing `querent-3.0.4/querent/graph/errors.py` & `querent-3.0.7/querent/graph/errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/graph/graph.py` & `querent-3.0.7/querent/graph/graph.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/graph/graph_namespace.py` & `querent-3.0.7/querent/graph/graph_namespace.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/graph/ontology.py` & `querent-3.0.7/querent/graph/ontology.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/graph/schema.py` & `querent-3.0.7/querent/graph/schema.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/graph/shacl.py` & `querent-3.0.7/querent/graph/shacl.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/graph/subject.py` & `querent-3.0.7/querent/graph/subject.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/graph/utils.py` & `querent-3.0.7/querent/graph/utils.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/audio/audio_ingestors.py` & `querent-3.0.7/querent/ingestors/audio/audio_ingestors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/base_ingestor.py` & `querent-3.0.7/querent/ingestors/base_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/code/code_ingestor.py` & `querent-3.0.7/querent/ingestors/code/code_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/csv/csv_ingestor.py` & `querent-3.0.7/querent/ingestors/csv/csv_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/doc/doc_ingestor.py` & `querent-3.0.7/querent/ingestors/doc/doc_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/email/email_ingestor.py` & `querent-3.0.7/querent/ingestors/email/email_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/email/email_reader.py` & `querent-3.0.7/querent/ingestors/email/email_reader.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/github/github_ingestor.py` & `querent-3.0.7/querent/ingestors/github/github_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/html/html_ingestor.py` & `querent-3.0.7/querent/ingestors/html/html_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/images/image_ingestor.py` & `querent-3.0.7/querent/ingestors/images/image_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/ingestor_factory.py` & `querent-3.0.7/querent/ingestors/ingestor_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/ingestor_manager.py` & `querent-3.0.7/querent/ingestors/ingestor_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/json/json_ingestor.py` & `querent-3.0.7/querent/ingestors/json/json_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/pdfs/pdf_ingestor_v1.py` & `querent-3.0.7/querent/ingestors/pdfs/pdf_ingestor_v1.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/ppt/ppt_ingestor.py` & `querent-3.0.7/querent/ingestors/ppt/ppt_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/texts/text_ingestor.py` & `querent-3.0.7/querent/ingestors/texts/text_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/video/video_ingestor.py` & `querent-3.0.7/querent/ingestors/video/video_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/xlsx/xlsx_ingestor.py` & `querent-3.0.7/querent/ingestors/xlsx/xlsx_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/ingestors/xml/xml_ingestor.py` & `querent-3.0.7/querent/ingestors/xml/xml_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/ner_helperfunctions/attn_scores.py` & `querent-3.0.7/querent/kg/ner_helperfunctions/attn_scores.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/ner_helperfunctions/contextual_embeddings.py` & `querent-3.0.7/querent/kg/ner_helperfunctions/contextual_embeddings.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/ner_helperfunctions/dependency_parsing.py` & `querent-3.0.7/querent/kg/ner_helperfunctions/dependency_parsing.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/ner_helperfunctions/filter_triples.py` & `querent-3.0.7/querent/kg/ner_helperfunctions/filter_triples.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/ner_helperfunctions/fixed_entities.py` & `querent-3.0.7/querent/kg/ner_helperfunctions/fixed_entities.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/ner_helperfunctions/fixed_predicate.py` & `querent-3.0.7/querent/kg/ner_helperfunctions/fixed_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/ner_helperfunctions/ner_llm_transformer.py` & `querent-3.0.7/querent/kg/ner_helperfunctions/ner_llm_transformer.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/querent_kg.py` & `querent-3.0.7/querent/kg/querent_kg.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/rel_helperfunctions/contextual_predicate.py` & `querent-3.0.7/querent/kg/rel_helperfunctions/contextual_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/rel_helperfunctions/fixed_relationships.py` & `querent-3.0.7/querent/kg/rel_helperfunctions/fixed_relationships.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py` & `querent-3.0.7/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/rel_helperfunctions/openai_functions.py` & `querent-3.0.7/querent/kg/rel_helperfunctions/openai_functions.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/rel_helperfunctions/questionanswer_llama2.py` & `querent-3.0.7/querent/kg/rel_helperfunctions/questionanswer_llama2.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/rel_helperfunctions/rel_normalize.py` & `querent-3.0.7/querent/kg/rel_helperfunctions/rel_normalize.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/kg/rel_helperfunctions/triple_to_json.py` & `querent-3.0.7/querent/kg/rel_helperfunctions/triple_to_json.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/logging/filters.py` & `querent-3.0.7/querent/logging/filters.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/logging/handlers.py` & `querent-3.0.7/querent/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/logging/logger.py` & `querent-3.0.7/querent/logging/logger.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/metric/adapters/promethus_adapter.py` & `querent-3.0.7/querent/metric/adapters/promethus_adapter.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/metric/metric_logging_handler.py` & `querent-3.0.7/querent/metric/metric_logging_handler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/metric/metric_registry.py` & `querent-3.0.7/querent/metric/metric_registry.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/processors/text_cleanup_processor.py` & `querent-3.0.7/querent/processors/text_cleanup_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/processors/text_processor.py` & `querent-3.0.7/querent/processors/text_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/querent/auto_scaler.py` & `querent-3.0.7/querent/querent/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/querent/querent.py` & `querent-3.0.7/querent/querent/querent.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/querent/resource_manager.py` & `querent-3.0.7/querent/querent/resource_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/storage/gcs_query.py` & `querent-3.0.7/querent/storage/gcs_query.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/storage/milvus_vectorevent_storage.py` & `querent-3.0.7/querent/storage/milvus_vectorevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/storage/neo4j_graphevent_storage.py` & `querent-3.0.7/querent/storage/neo4j_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/storage/postgres_graphevent_storage.py` & `querent-3.0.7/querent/storage/postgres_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/tools/web_page_extractor.py` & `querent-3.0.7/querent/tools/web_page_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/utils/webpage_extractor.py` & `querent-3.0.7/querent/utils/webpage_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/workflow/_helpers.py` & `querent-3.0.7/querent/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent/workflow/workflow.py` & `querent-3.0.7/querent/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.4/querent.egg-info/PKG-INFO` & `querent-3.0.7/querent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.4
+Version: 3.0.7
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
@@ -32,35 +32,33 @@
 Classifier: Topic :: Utilities
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.10, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: aiofiles==23.2.1
-Requires-Dist: aiohttp==3.9.3
+Requires-Dist: aiohttp==3.9.4
 Requires-Dist: attrs==23.1.0
 Requires-Dist: azure-storage-blob==12.19.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: boto3==1.26.146
 Requires-Dist: botocore==1.29.146
 Requires-Dist: bs4==0.0.1
 Requires-Dist: cachetools==5.3.3
 Requires-Dist: coverage==7.3.3
 Requires-Dist: dropbox==11.36.2
-Requires-Dist: faiss-cpu==1.7.4
+Requires-Dist: fastembed==0.2.6
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: gensim==4.3.2
 Requires-Dist: google-api-python-client==2.105.0
 Requires-Dist: google-cloud-storage==2.14.0
-Requires-Dist: google-cloud-storage==2.14.0
-Requires-Dist: google-cloud-storage==2.14.0
 Requires-Dist: hdbscan==0.8.33
 Requires-Dist: jira==3.6.0
 Requires-Dist: jmespath==1.0.1
 Requires-Dist: joblib==1.2.0
 Requires-Dist: json5==0.9.24
 Requires-Dist: jsonmerge==1.9.0
 Requires-Dist: jsonschema==4.17.3
@@ -99,17 +97,19 @@
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests_html==0.10.0
 Requires-Dist: slack-sdk==3.26.1
 Requires-Dist: slack-sdk==3.26.1
 Requires-Dist: spacy==3.7.2
 Requires-Dist: speechrecognition==3.10.1
 Requires-Dist: tika==2.6.0
+Requires-Dist: tensorflow==2.14.0
 Requires-Dist: transformers==4.36.0
 Requires-Dist: unidecode==1.3.7
-Requires-Dist: sentence-transformers==2.2.2
+Provides-Extra: torch
+Requires-Dist: torch; extra == "torch"
 
 # Querent
 
 The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 
 ![image](https://github.com/Querent-ai/querent-ai/assets/61435908/39124a0c-3d9e-434f-9b54-9aa51dcefbd7)
```

### Comparing `querent-3.0.4/querent.egg-info/SOURCES.txt` & `querent-3.0.7/querent.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -147,22 +147,20 @@
 querent/kg/ner_helperfunctions/filter_triples.py
 querent/kg/ner_helperfunctions/fixed_entities.py
 querent/kg/ner_helperfunctions/fixed_predicate.py
 querent/kg/ner_helperfunctions/ner_llm_transformer.py
 querent/kg/rel_helperfunctions/__init__.py
 querent/kg/rel_helperfunctions/contextual_predicate.py
 querent/kg/rel_helperfunctions/embedding_store.py
-querent/kg/rel_helperfunctions/filter_semantic_triples.py
 querent/kg/rel_helperfunctions/fixed_relationships.py
 querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
 querent/kg/rel_helperfunctions/opeai_ratelimiter.py
 querent/kg/rel_helperfunctions/openai_functions.py
 querent/kg/rel_helperfunctions/openllm.py
 querent/kg/rel_helperfunctions/questionanswer_llama2.py
-querent/kg/rel_helperfunctions/rag_retriever.py
 querent/kg/rel_helperfunctions/rel_normalize.py
 querent/kg/rel_helperfunctions/triple_to_json.py
 querent/logging/__init__.py
 querent/logging/custom_formatter.py
 querent/logging/filters.py
 querent/logging/handlers.py
 querent/logging/logger.py
```

### Comparing `querent-3.0.4/querent.egg-info/requires.txt` & `querent-3.0.7/querent.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 aiofiles==23.2.1
-aiohttp==3.9.3
+aiohttp==3.9.4
 attrs==23.1.0
 azure-storage-blob==12.19.0
 beautifulsoup4==4.12.3
 boto3==1.26.146
 botocore==1.29.146
 bs4==0.0.1
 cachetools==5.3.3
 coverage==7.3.3
 dropbox==11.36.2
-faiss-cpu==1.7.4
+fastembed==0.2.6
 ffmpeg-python==0.2.0
 gensim==4.3.2
 google-api-python-client==2.105.0
 google-cloud-storage==2.14.0
-google-cloud-storage==2.14.0
-google-cloud-storage==2.14.0
 hdbscan==0.8.33
 jira==3.6.0
 jmespath==1.0.1
 joblib==1.2.0
 json5==0.9.24
 jsonmerge==1.9.0
 jsonschema==4.17.3
@@ -58,10 +56,13 @@
 requests==2.31.0
 requests_html==0.10.0
 slack-sdk==3.26.1
 slack-sdk==3.26.1
 spacy==3.7.2
 speechrecognition==3.10.1
 tika==2.6.0
+tensorflow==2.14.0
 transformers==4.36.0
 unidecode==1.3.7
-sentence-transformers==2.2.2
+
+[torch]
+torch
```

### Comparing `querent-3.0.4/setup.py` & `querent-3.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """
     Querent AI: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 """
 
 from setuptools import setup, find_packages
 
+# List of required packages
 requirements = [
     "aiofiles==23.2.1",
-    "aiohttp==3.9.3",
+    "aiohttp==3.9.4",
     "attrs==23.1.0",
     "azure-storage-blob==12.19.0",
     "beautifulsoup4==4.12.3",
     "boto3==1.26.146",
     "botocore==1.29.146",
     "bs4==0.0.1",
     "cachetools==5.3.3",
     "coverage==7.3.3",
     "dropbox==11.36.2",
-    "faiss-cpu==1.7.4",
+    "fastembed==0.2.6",
     "ffmpeg-python==0.2.0",
     "gensim==4.3.2",
     "google-api-python-client==2.105.0",
     "google-cloud-storage==2.14.0",
-    "google-cloud-storage==2.14.0",
-    "google-cloud-storage==2.14.0",
     "hdbscan==0.8.33",
     "jira==3.6.0",
     "jmespath==1.0.1",
     "joblib==1.2.0",
     "json5==0.9.24",
     "jsonmerge==1.9.0",
     "jsonschema==4.17.3",
@@ -65,26 +64,28 @@
     "requests==2.31.0",
     "requests_html==0.10.0",
     "slack-sdk==3.26.1",
     "slack-sdk==3.26.1",
     "spacy==3.7.2",
     "speechrecognition==3.10.1",
     "tika==2.6.0",
+    "tensorflow==2.14.0",
     "transformers==4.36.0",
     "unidecode==1.3.7",
-    "sentence-transformers==2.2.2",
 ]
 
+# PyTorch index URL for dependency link
+torch_index_url = "https://download.pytorch.org/whl/cpu"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="querent",
-    version="3.0.4",
+    version="3.0.7",
     author="Querent AI",
     description="The Asynchronous Data Dynamo and Graph Neural Network Catalyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Querent-ai/querent-ai",
     project_urls={
         "Documentation": "https://github.com/Querent-ai/querent-ai/docs",
@@ -161,12 +162,18 @@
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Typing :: Typed",
     ],
-    python_requires=">=3.9, <4",
+    python_requires=">=3.10, <3.11",
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

