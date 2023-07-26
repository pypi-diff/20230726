# Comparing `tmp/ytdl-sub-2023.7.26.post1.tar.gz` & `tmp/ytdl-sub-2023.7.26.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.7.26.post1.tar", last modified: Wed Jul 26 03:27:19 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.7.26.post2.tar", last modified: Wed Jul 26 16:01:24 2023, max compression
```

## Comparing `ytdl-sub-2023.7.26.post1.tar` & `ytdl-sub-2023.7.26.post2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.954542 ytdl-sub-2023.7.26.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-26 03:27:19.954542 ytdl-sub-2023.7.26.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-26 03:27:19.954542 ytdl-sub-2023.7.26.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.942542 ytdl-sub-2023.7.26.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.942542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 03:27:00.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.946542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.946542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.946542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.946542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/source_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.946542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19945 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.946542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.946542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.950542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/embed_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.950542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.950542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.950542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.950542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.950542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20104 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.950542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    15182 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.950542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.954542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.954542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.954542 ytdl-sub-2023.7.26.post1/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-26 03:26:59.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:27:19.946542 ytdl-sub-2023.7.26.post1/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-26 03:27:19.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-26 03:27:19.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 03:27:19.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 03:27:19.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 03:27:19.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 03:27:19.000000 ytdl-sub-2023.7.26.post1/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.916410 ytdl-sub-2023.7.26.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-26 16:01:24.916410 ytdl-sub-2023.7.26.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-26 16:01:24.916410 ytdl-sub-2023.7.26.post2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.872409 ytdl-sub-2023.7.26.post2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.880409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.884409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.888409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.888409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.888409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/source_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.892409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19945 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.892409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.892409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.900410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.900410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.900410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.900410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.900410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.904410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.904410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15182 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.904410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.912410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.916410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.916410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.884409 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-26 16:01:24.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-26 16:01:24.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:01:24.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 16:01:24.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 16:01:24.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 16:01:24.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.7.26.post1/LICENSE` & `ytdl-sub-2023.7.26.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/PKG-INFO` & `ytdl-sub-2023.7.26.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.26.post1
+Version: 2023.7.26.post2
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.26.post1/README.md` & `ytdl-sub-2023.7.26.post2/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/pyproject.toml` & `ytdl-sub-2023.7.26.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/setup.cfg` & `ytdl-sub-2023.7.26.post2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/defaults.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/plugin.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/source_plugin.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/source_plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,16 +142,35 @@
         """
         Optional. Whether to download entries in the reverse order of the metadata downloaded.
         Defaults to True.
         """
         return self._download_reverse.value
 
 
-class UrlListValidator(ListValidator[UrlValidator]):
-    _inner_list_type = UrlValidator
+class UrlStringOrDictValidator(UrlValidator):
+    """
+    URL validator that supports a single string like:
+
+    download:
+      - "https://"
+
+    or
+
+    download:
+      - url: "https://"
+    """
+
+    _expected_value_type = (dict, str)
+
+    def __init__(self, name, value):
+        super().__init__(name, {"url": value} if isinstance(value, str) else value)
+
+
+class UrlListValidator(ListValidator[UrlStringOrDictValidator]):
+    _inner_list_type = UrlStringOrDictValidator
     _expected_value_type_name = "collection url list"
 
     def __init__(self, name, value):
         super().__init__(name, value)
 
         added_variables: Dict[str, str] = self.list[0].variables.dict_with_format_strings
 
@@ -193,25 +212,19 @@
 
         # Copy since we're popping things
         value_copy = copy.deepcopy(value)
         if isinstance(value, dict):
             # Pop old required field in case it's still there
             value_copy.pop("download_strategy", None)
 
-            if "urls" in value_copy:
-                self._urls = UrlListValidator(name=name, value=value_copy["urls"])
-            else:
-                # Validate using a single URL validator first
-                _ = UrlValidator(name=name, value=value_copy)
-                self._urls = UrlListValidator(name=name, value=[value_copy])
+        # Deal with old multi-url download strategy
+        if isinstance(value, dict) and "urls" in value_copy:
+            self._urls = UrlListValidator(name=name, value=value_copy["urls"])
         else:
-            # Should error here. TODO: Add simplifications download here (string, list)
-            self._urls = UrlListValidator(
-                name=name, value=UrlValidator(name=name, value=value_copy)
-            )
+            self._urls = UrlListValidator(name=name, value=value_copy)
 
     @property
     def urls(self) -> UrlListValidator:
         """
         Required. A list of :ref:`url` with the addition of the ``variables`` attribute.
         Multiple URLs should be listed in the order of priority, with the lowest priority being the
         top-most, and highest priority being the bottom-most. If a download exists in more than
```

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/main.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/embed_thumbnail.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/embed_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -30,40 +30,39 @@
       - "_jellyfin_tv_show"
 
 ####################################################################################################
 
   # TV show from one or more sources. Uses {url}'s avatar and banner as poster and fanart
   _tv_show_by_date:
     download:
-      urls:
-        - url: "{url}"
-          playlist_thumbnails:
-            - name: "{tv_show_poster_file_name}"
-              uid: "avatar_uncropped"
-            - name: "{tv_show_fanart_file_name}"
-              uid: "banner_uncropped"
-        - url: "{url2}"
-        - url: "{url3}"
-        - url: "{url4}"
-        - url: "{url5}"
-        - url: "{url6}"
-        - url: "{url7}"
-        - url: "{url8}"
-        - url: "{url9}"
-        - url: "{url10}"
-        - url: "{url11}"
-        - url: "{url12}"
-        - url: "{url13}"
-        - url: "{url14}"
-        - url: "{url15}"
-        - url: "{url16}"
-        - url: "{url17}"
-        - url: "{url18}"
-        - url: "{url19}"
-        - url: "{url20}"
+      - url: "{url}"
+        playlist_thumbnails:
+          - name: "{tv_show_poster_file_name}"
+            uid: "avatar_uncropped"
+          - name: "{tv_show_fanart_file_name}"
+            uid: "banner_uncropped"
+      - url: "{url2}"
+      - url: "{url3}"
+      - url: "{url4}"
+      - url: "{url5}"
+      - url: "{url6}"
+      - url: "{url7}"
+      - url: "{url8}"
+      - url: "{url9}"
+      - url: "{url10}"
+      - url: "{url11}"
+      - url: "{url12}"
+      - url: "{url13}"
+      - url: "{url14}"
+      - url: "{url15}"
+      - url: "{url16}"
+      - url: "{url17}"
+      - url: "{url18}"
+      - url: "{url19}"
+      - url: "{url20}"
     overrides:
       url2: ""
       url3: ""
       url4: ""
       url5: ""
       url6: ""
       url7: ""
```

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -17,730 +17,690 @@
       - "_tv_show_collection"
 
 ####################################################################################################
 # SEASON PRESETS
 
   collection_season_1:
     download:
-      urls:
-        - url: "{collection_season_1_url}"
-          variables:
-            collection_season_number: "1"
-            collection_season_number_padded: "01"
-          playlist_thumbnails:
-            # Use latest_entry first, then see if YT channel artwork exists
-            # ONLY FOR SEASON 1! The channel artwork will be the show's artwork.
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
-            - name: "{tv_show_poster_file_name}"
-              uid: "avatar_uncropped"
-            - name: "{tv_show_fanart_file_name}"
-              uid: "banner_uncropped"
+      - url: "{collection_season_1_url}"
+        variables:
+          collection_season_number: "1"
+          collection_season_number_padded: "01"
+        playlist_thumbnails:
+          # Use latest_entry first, then see if YT channel artwork exists
+          # ONLY FOR SEASON 1! The channel artwork will be the show's artwork.
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
+          - name: "{tv_show_poster_file_name}"
+            uid: "avatar_uncropped"
+          - name: "{tv_show_fanart_file_name}"
+            uid: "banner_uncropped"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_1_name}"
             attributes:
               number: "1"
 
   collection_season_2:
     download:
-      urls:
-        - url: "{collection_season_2_url}"
-          variables:
-            collection_season_number: "2"
-            collection_season_number_padded: "02"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_2_url}"
+        variables:
+          collection_season_number: "2"
+          collection_season_number_padded: "02"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_2_name}"
             attributes:
               number: "2"
 
   collection_season_3:
     download:
-      urls:
-        - url: "{collection_season_3_url}"
-          variables:
-            collection_season_number: "3"
-            collection_season_number_padded: "03"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_3_url}"
+        variables:
+          collection_season_number: "3"
+          collection_season_number_padded: "03"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_3_name}"
             attributes:
               number: "3"
 
   collection_season_4:
     download:
-      urls:
-        - url: "{collection_season_4_url}"
-          variables:
-            collection_season_number: "4"
-            collection_season_number_padded: "04"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_4_url}"
+        variables:
+          collection_season_number: "4"
+          collection_season_number_padded: "04"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_4_name}"
             attributes:
               number: "4"
 
   collection_season_5:
     download:
-      urls:
-        - url: "{collection_season_5_url}"
-          variables:
-            collection_season_number: "5"
-            collection_season_number_padded: "05"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_5_url}"
+        variables:
+          collection_season_number: "5"
+          collection_season_number_padded: "05"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_5_name}"
             attributes:
               number: "5"
 
   collection_season_6:
     download:
-      urls:
-        - url: "{collection_season_6_url}"
-          variables:
-            collection_season_number: "6"
-            collection_season_number_padded: "06"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_6_url}"
+        variables:
+          collection_season_number: "6"
+          collection_season_number_padded: "06"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_6_name}"
             attributes:
               number: "6"
 
   collection_season_7:
     download:
-      urls:
-        - url: "{collection_season_7_url}"
-          variables:
-            collection_season_number: "7"
-            collection_season_number_padded: "07"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_7_url}"
+        variables:
+          collection_season_number: "7"
+          collection_season_number_padded: "07"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_7_name}"
             attributes:
               number: "7"
 
   collection_season_8:
     download:
-      urls:
-        - url: "{collection_season_8_url}"
-          variables:
-            collection_season_number: "8"
-            collection_season_number_padded: "08"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_8_url}"
+        variables:
+          collection_season_number: "8"
+          collection_season_number_padded: "08"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_8_name}"
             attributes:
               number: "8"
 
   collection_season_9:
     download:
-      urls:
-        - url: "{collection_season_9_url}"
-          variables:
-            collection_season_number: "9"
-            collection_season_number_padded: "09"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_9_url}"
+        variables:
+          collection_season_number: "9"
+          collection_season_number_padded: "09"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_9_name}"
             attributes:
               number: "9"
 
   collection_season_10:
     download:
-      urls:
-        - url: "{collection_season_10_url}"
-          variables:
-            collection_season_number: "10"
-            collection_season_number_padded: "10"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_10_url}"
+        variables:
+          collection_season_number: "10"
+          collection_season_number_padded: "10"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_10_name}"
             attributes:
               number: "10"
 
   collection_season_11:
     download:
-      urls:
-        - url: "{collection_season_11_url}"
-          variables:
-            collection_season_number: "11"
-            collection_season_number_padded: "11"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_11_url}"
+        variables:
+          collection_season_number: "11"
+          collection_season_number_padded: "11"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_11_name}"
             attributes:
               number: "11"
 
   collection_season_12:
     download:
-      urls:
-        - url: "{collection_season_12_url}"
-          variables:
-            collection_season_number: "12"
-            collection_season_number_padded: "12"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_12_url}"
+        variables:
+          collection_season_number: "12"
+          collection_season_number_padded: "12"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_12_name}"
             attributes:
               number: "12"
 
   collection_season_13:
     download:
-      urls:
-        - url: "{collection_season_13_url}"
-          variables:
-            collection_season_number: "13"
-            collection_season_number_padded: "13"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_13_url}"
+        variables:
+          collection_season_number: "13"
+          collection_season_number_padded: "13"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_13_name}"
             attributes:
               number: "13"
 
   collection_season_14:
     download:
-      urls:
-        - url: "{collection_season_14_url}"
-          variables:
-            collection_season_number: "14"
-            collection_season_number_padded: "14"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_14_url}"
+        variables:
+          collection_season_number: "14"
+          collection_season_number_padded: "14"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_14_name}"
             attributes:
               number: "14"
 
   collection_season_15:
     download:
-      urls:
-        - url: "{collection_season_15_url}"
-          variables:
-            collection_season_number: "15"
-            collection_season_number_padded: "15"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_15_url}"
+        variables:
+          collection_season_number: "15"
+          collection_season_number_padded: "15"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_15_name}"
             attributes:
               number: "15"
 
   collection_season_16:
     download:
-      urls:
-        - url: "{collection_season_16_url}"
-          variables:
-            collection_season_number: "16"
-            collection_season_number_padded: "16"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_16_url}"
+        variables:
+          collection_season_number: "16"
+          collection_season_number_padded: "16"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_16_name}"
             attributes:
               number: "16"
 
   collection_season_17:
     download:
-      urls:
-        - url: "{collection_season_17_url}"
-          variables:
-            collection_season_number: "17"
-            collection_season_number_padded: "17"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_17_url}"
+        variables:
+          collection_season_number: "17"
+          collection_season_number_padded: "17"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_17_name}"
             attributes:
               number: "17"
 
   collection_season_18:
     download:
-      urls:
-        - url: "{collection_season_18_url}"
-          variables:
-            collection_season_number: "18"
-            collection_season_number_padded: "18"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_18_url}"
+        variables:
+          collection_season_number: "18"
+          collection_season_number_padded: "18"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_18_name}"
             attributes:
               number: "18"
 
   collection_season_19:
     download:
-      urls:
-        - url: "{collection_season_19_url}"
-          variables:
-            collection_season_number: "19"
-            collection_season_number_padded: "19"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_19_url}"
+        variables:
+          collection_season_number: "19"
+          collection_season_number_padded: "19"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_19_name}"
             attributes:
               number: "19"
 
   collection_season_20:
     download:
-      urls:
-        - url: "{collection_season_20_url}"
-          variables:
-            collection_season_number: "20"
-            collection_season_number_padded: "20"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_20_url}"
+        variables:
+          collection_season_number: "20"
+          collection_season_number_padded: "20"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_20_name}"
             attributes:
               number: "20"
 
   collection_season_21:
     download:
-      urls:
-        - url: "{collection_season_21_url}"
-          variables:
-            collection_season_number: "21"
-            collection_season_number_padded: "21"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_21_url}"
+        variables:
+          collection_season_number: "21"
+          collection_season_number_padded: "21"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_21_name}"
             attributes:
               number: "21"
 
   collection_season_22:
     download:
-      urls:
-        - url: "{collection_season_22_url}"
-          variables:
-            collection_season_number: "22"
-            collection_season_number_padded: "22"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_22_url}"
+        variables:
+          collection_season_number: "22"
+          collection_season_number_padded: "22"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_22_name}"
             attributes:
               number: "22"
 
   collection_season_23:
     download:
-      urls:
-        - url: "{collection_season_23_url}"
-          variables:
-            collection_season_number: "23"
-            collection_season_number_padded: "23"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_23_url}"
+        variables:
+          collection_season_number: "23"
+          collection_season_number_padded: "23"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_23_name}"
             attributes:
               number: "23"
 
   collection_season_24:
     download:
-      urls:
-        - url: "{collection_season_24_url}"
-          variables:
-            collection_season_number: "24"
-            collection_season_number_padded: "24"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_24_url}"
+        variables:
+          collection_season_number: "24"
+          collection_season_number_padded: "24"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_24_name}"
             attributes:
               number: "24"
 
   collection_season_25:
     download:
-      urls:
-        - url: "{collection_season_25_url}"
-          variables:
-            collection_season_number: "25"
-            collection_season_number_padded: "25"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_25_url}"
+        variables:
+          collection_season_number: "25"
+          collection_season_number_padded: "25"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_25_name}"
             attributes:
               number: "25"
 
   collection_season_26:
     download:
-      urls:
-        - url: "{collection_season_26_url}"
-          variables:
-            collection_season_number: "26"
-            collection_season_number_padded: "26"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_26_url}"
+        variables:
+          collection_season_number: "26"
+          collection_season_number_padded: "26"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_26_name}"
             attributes:
               number: "26"
 
   collection_season_27:
     download:
-      urls:
-        - url: "{collection_season_27_url}"
-          variables:
-            collection_season_number: "27"
-            collection_season_number_padded: "27"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_27_url}"
+        variables:
+          collection_season_number: "27"
+          collection_season_number_padded: "27"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_27_name}"
             attributes:
               number: "27"
 
   collection_season_28:
     download:
-      urls:
-        - url: "{collection_season_28_url}"
-          variables:
-            collection_season_number: "28"
-            collection_season_number_padded: "28"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_28_url}"
+        variables:
+          collection_season_number: "28"
+          collection_season_number_padded: "28"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_28_name}"
             attributes:
               number: "28"
 
   collection_season_29:
     download:
-      urls:
-        - url: "{collection_season_29_url}"
-          variables:
-            collection_season_number: "29"
-            collection_season_number_padded: "29"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_29_url}"
+        variables:
+          collection_season_number: "29"
+          collection_season_number_padded: "29"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_29_name}"
             attributes:
               number: "29"
 
   collection_season_30:
     download:
-      urls:
-        - url: "{collection_season_30_url}"
-          variables:
-            collection_season_number: "30"
-            collection_season_number_padded: "30"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_30_url}"
+        variables:
+          collection_season_number: "30"
+          collection_season_number_padded: "30"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_30_name}"
             attributes:
               number: "30"
 
   collection_season_31:
     download:
-      urls:
-        - url: "{collection_season_31_url}"
-          variables:
-            collection_season_number: "31"
-            collection_season_number_padded: "31"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_31_url}"
+        variables:
+          collection_season_number: "31"
+          collection_season_number_padded: "31"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_31_name}"
             attributes:
               number: "31"
 
   collection_season_32:
     download:
-      urls:
-        - url: "{collection_season_32_url}"
-          variables:
-            collection_season_number: "32"
-            collection_season_number_padded: "32"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_32_url}"
+        variables:
+          collection_season_number: "32"
+          collection_season_number_padded: "32"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_32_name}"
             attributes:
               number: "32"
 
   collection_season_33:
     download:
-      urls:
-        - url: "{collection_season_33_url}"
-          variables:
-            collection_season_number: "33"
-            collection_season_number_padded: "33"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_33_url}"
+        variables:
+          collection_season_number: "33"
+          collection_season_number_padded: "33"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_33_name}"
             attributes:
               number: "33"
 
   collection_season_34:
     download:
-      urls:
-        - url: "{collection_season_34_url}"
-          variables:
-            collection_season_number: "34"
-            collection_season_number_padded: "34"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_34_url}"
+        variables:
+          collection_season_number: "34"
+          collection_season_number_padded: "34"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_34_name}"
             attributes:
               number: "34"
 
   collection_season_35:
     download:
-      urls:
-        - url: "{collection_season_35_url}"
-          variables:
-            collection_season_number: "35"
-            collection_season_number_padded: "35"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_35_url}"
+        variables:
+          collection_season_number: "35"
+          collection_season_number_padded: "35"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_35_name}"
             attributes:
               number: "35"
 
   collection_season_36:
     download:
-      urls:
-        - url: "{collection_season_36_url}"
-          variables:
-            collection_season_number: "36"
-            collection_season_number_padded: "36"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_36_url}"
+        variables:
+          collection_season_number: "36"
+          collection_season_number_padded: "36"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_36_name}"
             attributes:
               number: "36"
 
   collection_season_37:
     download:
-      urls:
-        - url: "{collection_season_37_url}"
-          variables:
-            collection_season_number: "37"
-            collection_season_number_padded: "37"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_37_url}"
+        variables:
+          collection_season_number: "37"
+          collection_season_number_padded: "37"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_37_name}"
             attributes:
               number: "37"
 
   collection_season_38:
     download:
-      urls:
-        - url: "{collection_season_38_url}"
-          variables:
-            collection_season_number: "38"
-            collection_season_number_padded: "38"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_38_url}"
+        variables:
+          collection_season_number: "38"
+          collection_season_number_padded: "38"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_38_name}"
             attributes:
               number: "38"
 
   collection_season_39:
     download:
-      urls:
-        - url: "{collection_season_39_url}"
-          variables:
-            collection_season_number: "39"
-            collection_season_number_padded: "39"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_39_url}"
+        variables:
+          collection_season_number: "39"
+          collection_season_number_padded: "39"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_39_name}"
             attributes:
               number: "39"
 
   collection_season_40:
     download:
-      urls:
-        - url: "{collection_season_40_url}"
-          variables:
-            collection_season_number: "40"
-            collection_season_number_padded: "40"
-          playlist_thumbnails:
-            - name: "{season_poster_file_name}"
-              uid: "latest_entry"
+      - url: "{collection_season_40_url}"
+        variables:
+          collection_season_number: "40"
+          collection_season_number_padded: "40"
+        playlist_thumbnails:
+          - name: "{season_poster_file_name}"
+            uid: "latest_entry"
 
     output_directory_nfo_tags:
       tags:
         namedseason:
           - tag: "{collection_season_40_name}"
             attributes:
               number: "40"
```

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.26.post1
+Version: 2023.7.26.post2
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.26.post1/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

