# Comparing `tmp/ytdl_sub-2024.4.28.tar.gz` & `tmp/ytdl-sub-2024.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl_sub-2024.4.28.tar", last modified: Sun Apr 28 05:48:21 2024, max compression
+gzip compressed data, was "ytdl-sub-2024.4.3.tar", last modified: Wed Apr  3 00:34:23 2024, max compression
```

## Comparing `ytdl_sub-2024.4.28.tar` & `ytdl-sub-2024.4.3.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.676217 ytdl_sub-2024.4.28/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    51273 2024-04-28 05:48:21.676217 ytdl_sub-2024.4.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 05:48:21.676217 ytdl_sub-2024.4.28/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.644217 ytdl_sub-2024.4.28/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.648217 ytdl_sub-2024.4.28/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.648217 ytdl_sub-2024.4.28/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/cli/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/cli/output_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/cli/output_transaction_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.652217 ytdl_sub-2024.4.28/src/ytdl_sub/cli/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/cli/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/cli/parsers/dl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/cli/parsers/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.652217 ytdl_sub-2024.4.28/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.652217 ytdl_sub-2024.4.28/src/ytdl_sub/config/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/plugin/plugin_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/plugin/plugin_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/plugin/preset_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.652217 ytdl_sub-2024.4.28/src/ytdl_sub/config/validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/validators/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/config/validators/variable_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.652217 ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.652217 ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/source_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.656217 ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20766 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.656217 ytdl_sub-2024.4.28/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.656217 ytdl_sub-2024.4.28/src/ytdl_sub/entries/script/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/entries/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/entries/script/custom_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/entries/script/function_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    42267 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/entries/script/variable_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/entries/script/variable_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.656217 ytdl_sub-2024.4.28/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/entries/variables/override_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.660217 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    14569 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/embed_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/file_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/filter_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/filter_include.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.660217 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/throttle_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.660217 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.660217 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    23681 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/helpers/url.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.660217 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.664217 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music/singles.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.664217 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music_videos/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music_videos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.664217 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34839 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.664217 ytdl_sub-2024.4.28/src/ytdl_sub/script/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.668217 ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/array_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/boolean_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/conditional_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/date_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/json_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/map_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/numeric_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/regex_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/string_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21712 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22535 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/script_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.668217 ytdl_sub-2024.4.28/src/ytdl_sub/script/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/types/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/types/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/types/resolvable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/types/syntax_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/types/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/types/variable_dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.668217 ytdl_sub-2024.4.28/src/ytdl_sub/script/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/utils/exception_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/utils/name_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/script/utils/type_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.668217 ytdl_sub-2024.4.28/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    16254 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/subscriptions/subscription_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.672217 ytdl_sub-2024.4.28/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.672217 ytdl_sub-2024.4.28/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/scriptable.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.676217 ytdl_sub-2024.4.28/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.676217 ytdl_sub-2024.4.28/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-04-28 05:48:10.000000 ytdl_sub-2024.4.28/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:48:21.676217 ytdl_sub-2024.4.28/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    51273 2024-04-28 05:48:21.000000 ytdl_sub-2024.4.28/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-04-28 05:48:21.000000 ytdl_sub-2024.4.28/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 05:48:21.000000 ytdl_sub-2024.4.28/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-28 05:48:21.000000 ytdl_sub-2024.4.28/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-28 05:48:21.000000 ytdl_sub-2024.4.28/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 05:48:21.000000 ytdl_sub-2024.4.28/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.359598 ytdl-sub-2024.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-04-03 00:34:23.359598 ytdl-sub-2024.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-03 00:34:23.359598 ytdl-sub-2024.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.327597 ytdl-sub-2024.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.331597 ytdl-sub-2024.4.3/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.331597 ytdl-sub-2024.4.3/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/output_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/output_transaction_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.331597 ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/dl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/preset_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/variable_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/source_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.339598 ytdl-sub-2024.4.3/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.339598 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/custom_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/function_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42267 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/variable_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/variable_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.339598 ytdl-sub-2024.4.3/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/variables/override_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/file_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/filter_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/filter_include.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/throttle_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    23681 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/url.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/singles.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.347598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34839 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.347598 ytdl-sub-2024.4.3/src/ytdl_sub/script/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.347598 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/boolean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/conditional_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/json_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/numeric_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/regex_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/string_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21712 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22535 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/script_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.347598 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/resolvable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/syntax_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/variable_dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.351598 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/exception_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/name_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/type_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.351598 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16254 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.351598 ytdl-sub-2024.4.3/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.355598 ytdl-sub-2024.4.3/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/scriptable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.355598 ytdl-sub-2024.4.3/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.355598 ytdl-sub-2024.4.3/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.355598 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl_sub-2024.4.28/LICENSE` & `ytdl-sub-2024.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/README.md` & `ytdl-sub-2024.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/cli/entrypoint.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/cli/output_summary.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/cli/output_summary.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/cli/output_transaction_log.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/cli/output_transaction_log.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/cli/parsers/dl.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/dl.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/cli/parsers/main.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,16 +146,14 @@
 parser = argparse.ArgumentParser(
     description="ytdl-sub: Automate download and adding metadata with YoutubeDL",
 )
 parser.add_argument("-v", "--version", action="version", version="%(prog)s " + __local_version__)
 _add_shared_arguments(parser, suppress_defaults=False)
 
 subparsers = parser.add_subparsers(dest="subparser")
-
-
 ###################################################################################################
 # SUBSCRIPTION PARSER
 class SubArguments:
     UPDATE_WITH_INFO_JSON = CLIArgument(
         short="-u",
         long="--update-with-info-json",
     )
```

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/config/defaults.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/config/overrides.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/overrides.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/config/plugin/plugin.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/config/plugin/plugin_mapping.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin_mapping.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/config/plugin/preset_plugins.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/config/preset.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/config/validators/options.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/options.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/config/validators/variable_validation.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/variable_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from ytdl_sub.validators.string_formatter_validators import validate_formatters
 
 # Entry variables to mock during validation
 _DUMMY_ENTRY_VARIABLES: Dict[str, str] = {
     name: to_variable_dependency_format_string(
         # pylint: disable=protected-access
         script=BASE_SCRIPT,
-        parsed_format_string=BASE_SCRIPT._variables[name],
+        parsed_format_string=BASE_SCRIPT._variables[name]
         # pylint: enable=protected-access
     )
     for name in BASE_SCRIPT.variable_names
 }
 
 
 def _add_dummy_variables(variables: Iterable[str]) -> Dict[str, str]:
```

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/source_plugin.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/source_plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,19 +244,17 @@
         -------
         YTLD options dict for downloading
         """
         return (
             self._download_ytdl_options_builder.clone()
             .add(self.ytdl_option_defaults(), before=True)
             .add(
-                (
-                    self.plugin_options.urls.list[url_idx].ytdl_options.dict
-                    if url_idx is not None
-                    else None
-                ),
+                self.plugin_options.urls.list[url_idx].ytdl_options.dict
+                if url_idx is not None
+                else None,
                 before=True,
             )
             .to_dict()
         )
 
     def metadata_ytdl_options(self, ytdl_option_overrides: Dict) -> Dict:
         """
@@ -350,19 +348,17 @@
 
     def _extract_entry_info_with_retry(self, entry: Entry) -> Entry:
         download_entry_dict = YTDLP.extract_info_with_retry(
             ytdl_options_overrides=self.download_ytdl_options(
                 url_idx=entry.get(v.ytdl_sub_input_url_index, int)
             ),
             is_downloaded_fn=None if self.is_dry_run else entry.is_downloaded,
-            is_thumbnail_downloaded_fn=(
-                None
-                if (self.is_dry_run or not self.is_entry_thumbnails_enabled)
-                else entry.is_thumbnail_downloaded_via_ytdlp
-            ),
+            is_thumbnail_downloaded_fn=None
+            if (self.is_dry_run or not self.is_entry_thumbnails_enabled)
+            else entry.is_thumbnail_downloaded_via_ytdlp,
             url=entry.webpage_url,
         )
         return Entry(
             download_entry_dict,
             working_directory=self.working_directory,
         )
```

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/entries/script/custom_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/custom_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/entries/script/function_scripts.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/function_scripts.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/entries/script/variable_definitions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/variable_definitions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/entries/script/variable_types.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/variable_types.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/entries/variables/override_variables.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/variables/override_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/main.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/chapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,21 +259,21 @@
 
         if self._is_removing_chapters:
             remove_chapters_post_processor = {
                 "key": "ModifyChapters",
                 "force_keyframes": self.plugin_options.force_key_frames,
             }
             if self.plugin_options.remove_sponsorblock_categories is not None:
-                remove_chapters_post_processor["remove_sponsor_segments"] = (
-                    self.plugin_options.remove_sponsorblock_categories
-                )
+                remove_chapters_post_processor[
+                    "remove_sponsor_segments"
+                ] = self.plugin_options.remove_sponsorblock_categories
             if self.plugin_options.remove_chapters_regex is not None:
-                remove_chapters_post_processor["remove_chapters_patterns"] = (
-                    self.plugin_options.remove_chapters_regex
-                )
+                remove_chapters_post_processor[
+                    "remove_chapters_patterns"
+                ] = self.plugin_options.remove_chapters_regex
 
             if self.plugin_options.embed_chapters:
                 builder.add(
                     {
                         # re-add chapters
                         "postprocessors": [
                             remove_chapters_post_processor,
```

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/embed_thumbnail.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/embed_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/filter_exclude.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/filter_exclude.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/filter_include.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/filter_include.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/format.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/format.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,17 +155,17 @@
         timestamp_begin = chapters.timestamps[idx].readable_str
         timestamp_end = Timestamp(new_entry.get(v.duration, int)).readable_str
         if idx + 1 < len(chapters.timestamps):
             timestamp_end = chapters.timestamps[idx + 1].readable_str
 
         metadata_value_dict = {}
         if self.is_dry_run:
-            metadata_value_dict["Warning"] = (
-                "Dry-run assumes embedded chapters with no modifications"
-            )
+            metadata_value_dict[
+                "Warning"
+            ] = "Dry-run assumes embedded chapters with no modifications"
 
         metadata_value_dict["Source Title"] = new_entry.title
         metadata_value_dict["Segment"] = f"{timestamp_begin} - {timestamp_end}"
 
         metadata = FileMetadata.from_dict(
             value_dict=metadata_value_dict,
             title="From Chapter Split",
```

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/throttle_protection.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/throttle_protection.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/helpers/players.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/players.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/helpers/url.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/url.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music/singles.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/singles.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/__init__.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/array_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/array_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/boolean_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/boolean_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/conditional_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/conditional_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/error_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/error_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/json_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/json_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/map_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/map_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/numeric_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/numeric_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/regex_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/regex_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,17 +48,7 @@
     @staticmethod
     def regex_capture_groups(regex: String) -> Integer:
         """
         :description:
           Returns number of capture groups in regex
         """
         return Integer(re.compile(regex.value).groups)
-
-    @staticmethod
-    def regex_sub(regex: String, replacement: String, string: String) -> String:
-        """
-        :description:
-          Returns the string obtained by replacing the leftmost non-overlapping occurrences of the
-          pattern in string by the replacement string. The replacement string can reference the
-          match groups via backslash escapes. Callables as replacement argument are not supported.
-        """
-        return String(re.sub(regex.value, replacement.value, string.value))
```

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/functions/string_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/string_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/parser.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/parser.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/script.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/script.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/script_output.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/script_output.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/types/array.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/array.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/types/function.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/function.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/types/map.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/map.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/types/resolvable.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/resolvable.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/types/syntax_tree.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/syntax_tree.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/types/variable.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/variable.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/types/variable_dependency.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/variable_dependency.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/utils/exception_formatters.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/exception_formatters.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/utils/exceptions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/utils/name_validation.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/name_validation.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/script/utils/type_checking.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/type_checking.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,21 +70,21 @@
         # Add overrides pre-archive
         self.overrides.add(
             {
                 SubscriptionVariables.subscription_name(): self.name,
             }
         )
 
-        self._enhanced_download_archive: Optional[EnhancedDownloadArchive] = (
-            _initialize_download_archive(
-                output_options=self.output_options,
-                overrides=self.overrides,
-                working_directory=self.working_directory,
-                output_directory=self.output_directory,
-            )
+        self._enhanced_download_archive: Optional[
+            EnhancedDownloadArchive
+        ] = _initialize_download_archive(
+            output_options=self.output_options,
+            overrides=self.overrides,
+            working_directory=self.working_directory,
+            output_directory=self.output_directory,
         )
 
         # Add post-archive variables
         self.overrides.add(
             {
                 SubscriptionVariables.subscription_has_download_archive(): f"""{{
                         %bool({self.download_archive.num_entries > 0})
```

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/subscriptions/subscription_validators.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,17 +139,17 @@
             name=name,
             value=value,
             subscription_name=subscription_name,
             config=config,
             presets=presets,
             indent_overrides=indent_overrides,
         )
-        self._overrides_to_add[SubscriptionVariables.subscription_value().variable_name] = (
-            self.value
-        )
+        self._overrides_to_add[
+            SubscriptionVariables.subscription_value().variable_name
+        ] = self.value
 
 
 class SubscriptionListValuesValidator(SubscriptionLeafValidator, StringListValidator):
     def __init__(
         self,
         name,
         value,
@@ -166,17 +166,17 @@
             presets=presets,
             indent_overrides=indent_overrides,
         )
 
         for idx, list_value in enumerate(self.list):
             # Write the first list value into subscription_value as well
             if idx == 0:
-                self._overrides_to_add[SubscriptionVariables.subscription_value().variable_name] = (
-                    list_value.value
-                )
+                self._overrides_to_add[
+                    SubscriptionVariables.subscription_value().variable_name
+                ] = list_value.value
 
             self._overrides_to_add[
                 SubscriptionVariables.subscription_value_i(index=idx).variable_name
             ] = list_value.value
 
 
 class SubscriptionWithOverridesValidator(SubscriptionLeafValidator, DictFormatterValidator):
@@ -215,17 +215,17 @@
             name=name,
             value=value,
             subscription_name=subscription_name,
             config=config,
             presets=presets,
             indent_overrides=indent_overrides,
         )
-        self._overrides_to_add[SubscriptionVariables.subscription_map().variable_name] = (
-            ScriptUtils.to_script(self.dict)
-        )
+        self._overrides_to_add[
+            SubscriptionVariables.subscription_map().variable_name
+        ] = ScriptUtils.to_script(self.dict)
 
 
 class SubscriptionValidator(SubscriptionOutput):
     """
     Top-level subscription validator
     """
```

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/file_path.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_path.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,18 +209,17 @@
                         yield
             finally:
                 redirect_stream.flush()
 
     @classmethod
     def _append_to_error_log(cls):
         # Any time an exception occurs, dump all debug logs into the error log
-        with (
-            open(cls.debug_log_filename(), mode="r", encoding="utf-8") as debug_logs,
-            open(cls.error_log_filename(), mode="a", encoding="utf-8") as error_logs,
-        ):
+        with open(cls.debug_log_filename(), mode="r", encoding="utf-8") as debug_logs, open(
+            cls.error_log_filename(), mode="a", encoding="utf-8"
+        ) as error_logs:
             error_logs.writelines(debug_logs.readlines())
 
     @classmethod
     def log_exception(cls, exception: Exception, log_filepath: Optional[Path] = None):
         """
         Logs an exception based on the exception type. Will transfer all
         debug logs into the error log file. This allows for subscriptions to only write to the
```

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/script.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/script.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/scriptable.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/scriptable.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.4.28/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+setup.cfg
 src/ytdl_sub/__init__.py
 src/ytdl_sub/main.py
 src/ytdl_sub.egg-info/PKG-INFO
 src/ytdl_sub.egg-info/SOURCES.txt
 src/ytdl_sub.egg-info/dependency_links.txt
 src/ytdl_sub.egg-info/entry_points.txt
 src/ytdl_sub.egg-info/requires.txt
```

