# Comparing `tmp/ytdl-sub-2023.7.25.post7.tar.gz` & `tmp/ytdl-sub-2023.7.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.7.25.post7.tar", last modified: Tue Jul 25 21:42:56 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.7.26.tar", last modified: Wed Jul 26 02:53:51 2023, max compression
```

## Comparing `ytdl-sub-2023.7.25.post7.tar` & `ytdl-sub-2023.7.26.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.752361 ytdl-sub-2023.7.25.post7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 21:42:56.752361 ytdl-sub-2023.7.25.post7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 21:42:56.752361 ytdl-sub-2023.7.25.post7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.720361 ytdl-sub-2023.7.25.post7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.724361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.728361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.728361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    20664 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.732361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.732361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/source_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.732361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.732361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.736361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.740361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/embed_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.740361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.740361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.740361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.740361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.744361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.744361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    15121 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.744361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.748361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.752361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.752361 ytdl-sub-2023.7.25.post7/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-25 21:42:33.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:42:56.724361 ytdl-sub-2023.7.25.post7/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 21:42:56.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-25 21:42:56.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:42:56.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 21:42:56.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 21:42:56.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 21:42:56.000000 ytdl-sub-2023.7.25.post7/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.041715 ytdl-sub-2023.7.26/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-07-26 02:53:51.041715 ytdl-sub-2023.7.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-26 02:53:51.045715 ytdl-sub-2023.7.26/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.009715 ytdl-sub-2023.7.26/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.013715 ytdl-sub-2023.7.26/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.017715 ytdl-sub-2023.7.26/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.021715 ytdl-sub-2023.7.26/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/config/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.021715 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.021715 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/source_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.025715 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19945 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.025715 ytdl-sub-2023.7.26/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.025715 ytdl-sub-2023.7.26/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.029715 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.029715 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.029715 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.029715 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.029715 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.033715 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.033715 ytdl-sub-2023.7.26/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15182 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.033715 ytdl-sub-2023.7.26/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.037715 ytdl-sub-2023.7.26/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.041715 ytdl-sub-2023.7.26/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.041715 ytdl-sub-2023.7.26/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-26 02:53:13.000000 ytdl-sub-2023.7.26/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:53:51.017715 ytdl-sub-2023.7.26/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-07-26 02:53:50.000000 ytdl-sub-2023.7.26/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-26 02:53:51.000000 ytdl-sub-2023.7.26/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 02:53:50.000000 ytdl-sub-2023.7.26/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 02:53:50.000000 ytdl-sub-2023.7.26/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 02:53:50.000000 ytdl-sub-2023.7.26/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 02:53:50.000000 ytdl-sub-2023.7.26/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.7.25.post7/LICENSE` & `ytdl-sub-2023.7.26/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/PKG-INFO` & `ytdl-sub-2023.7.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.25.post7
+Version: 2023.7.26
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.25.post7/README.md` & `ytdl-sub-2023.7.26/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/pyproject.toml` & `ytdl-sub-2023.7.26/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/setup.cfg` & `ytdl-sub-2023.7.26/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/defaults.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/plugin.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/config/plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/regex.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,530 +1,445 @@
-import copy
 from typing import Any
 from typing import Dict
-from typing import Iterable
 from typing import List
 from typing import Optional
-from typing import Tuple
-from typing import Type
-from typing import Union
 
-from mergedeep import mergedeep
+from yt_dlp.utils import sanitize_filename
 
-from ytdl_sub.config.config_validator import ConfigValidator
 from ytdl_sub.config.plugin import Plugin
-from ytdl_sub.config.preset_class_mappings import DownloadStrategyMapping
-from ytdl_sub.config.preset_class_mappings import PluginMapping
-from ytdl_sub.config.preset_options import OptionsValidator
-from ytdl_sub.config.preset_options import OutputOptions
-from ytdl_sub.config.preset_options import Overrides
-from ytdl_sub.config.preset_options import TOptionsValidator
-from ytdl_sub.config.preset_options import YTDLOptions
-from ytdl_sub.downloaders.source_plugin import SourcePlugin
+from ytdl_sub.config.plugin import PluginPriority
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
-from ytdl_sub.prebuilt_presets import PREBUILT_PRESET_NAMES
-from ytdl_sub.prebuilt_presets import PUBLISHED_PRESET_NAMES
-from ytdl_sub.utils.exceptions import ValidationException
+from ytdl_sub.entries.variables.kwargs import YTDL_SUB_REGEX_SOURCE_VARS
+from ytdl_sub.utils.exceptions import RegexNoMatchException
+from ytdl_sub.utils.exceptions import StringFormattingVariableNotFoundException
 from ytdl_sub.utils.logger import Logger
-from ytdl_sub.utils.yaml import dump_yaml
+from ytdl_sub.validators.regex_validator import RegexListValidator
+from ytdl_sub.validators.source_variable_validator import SourceVariableNameListValidator
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
-from ytdl_sub.validators.string_formatter_validators import DictFormatterValidator
-from ytdl_sub.validators.string_formatter_validators import OverridesDictFormatterValidator
-from ytdl_sub.validators.string_formatter_validators import OverridesStringFormatterValidator
+from ytdl_sub.validators.string_formatter_validators import ListFormatterValidator
 from ytdl_sub.validators.string_formatter_validators import StringFormatterValidator
-from ytdl_sub.validators.validators import DictValidator
-from ytdl_sub.validators.validators import ListValidator
-from ytdl_sub.validators.validators import StringListValidator
-from ytdl_sub.validators.validators import StringValidator
-from ytdl_sub.validators.validators import Validator
-from ytdl_sub.validators.validators import validation_exception
-
-PRESET_KEYS = {
-    "preset",
-    "output_options",
-    "ytdl_options",
-    "overrides",
-    *DownloadStrategyMapping.sources(),
-    *PluginMapping.plugins(),
-}
-
-logger = Logger.get()
-
-
-def _parent_preset_error_message(
-    current_preset_name: str, parent_preset_name: str, presets: List[str]
-) -> ValidationException:
-    user_defined_presets = set(presets) - PREBUILT_PRESET_NAMES - {current_preset_name}
-
-    return validation_exception(
-        name=current_preset_name,
-        error_message=f"preset '{parent_preset_name}' does not exist in the provided config.\n"
-        f"Available prebuilt presets: {', '.join(sorted(PUBLISHED_PRESET_NAMES))}\n"
-        f"Your presets: {', '.join(sorted(user_defined_presets))}",
-    )
+from ytdl_sub.validators.validators import BoolValidator
+
+logger = Logger.get(name="regex")
+
+
+class VariableRegex(StrictDictValidator):
+
+    _optional_keys = {"match", "exclude", "capture_group_defaults", "capture_group_names"}
 
+    def __init__(self, name, value):
+        super().__init__(name, value)
+        self._match = self._validate_key_if_present(key="match", validator=RegexListValidator)
+        self._exclude = self._validate_key_if_present(key="exclude", validator=RegexListValidator)
+        self._capture_group_defaults = self._validate_key_if_present(
+            key="capture_group_defaults", validator=ListFormatterValidator
+        )
+        self._capture_group_names = self._validate_key_if_present(
+            key="capture_group_names", validator=SourceVariableNameListValidator, default=[]
+        )
+
+        if self._match is None and self._exclude is None:
+            raise self._validation_exception("must specify either `match` or `exclude`")
 
-class PresetPlugins:
-    def __init__(self):
-        self.plugin_types: List[Type[Plugin]] = []
-        self.plugin_options: List[OptionsValidator] = []
+        if self._match is None and (self._capture_group_defaults or self._capture_group_names.list):
+            raise self._validation_exception(
+                "capture group parameters requires at least one `match` to be specified"
+            )
+
+        # If defaults are to be used, ensure there are the same number of defaults as there are
+        # capture groups
+        if self._capture_group_defaults is not None and self._match.num_capture_groups != len(
+            self._capture_group_defaults.list
+        ):
+            raise self._validation_exception(
+                f"number of defaults must match number of capture groups, "
+                f"{len(self._capture_group_defaults.list)} != {self._match.num_capture_groups}"
+            )
+
+        # If there are capture groups, ensure there are capture group names
+        if self._match and (len(self._capture_group_names.list) != self._match.num_capture_groups):
+            raise self._validation_exception(
+                f"number of capture group names must match number of capture groups, "
+                f"{len(self._capture_group_names.list)} != {self._match.num_capture_groups}"
+            )
+
+    @property
+    def match(self) -> Optional[RegexListValidator]:
+        """
+        List of regex strings to try to match against a source or override variable. Each regex
+        string must have the same number of capture groups.
+        """
+        return self._match
 
-    def add(self, plugin_type: Type[Plugin], plugin_options: OptionsValidator) -> "PresetPlugins":
+    @property
+    def exclude(self) -> Optional[RegexListValidator]:
         """
-        Add a pair of plugin type and options to the list
+        List of regex strings to try to match against a source or override variable. If one of the
+        regex strings match, then the entry will be skipped. If both ``exclude`` and ``match`` are
+        specified, entries will get skipped if the regex matches against both ``exclude`` and
+        ``match``.
         """
-        self.plugin_types.append(plugin_type)
-        self.plugin_options.append(plugin_options)
-        return self
+        return self._exclude
 
-    def zipped(self) -> Iterable[Tuple[Type[Plugin], OptionsValidator]]:
+    @property
+    def capture_group_names(self) -> Optional[List[str]]:
         """
-        Returns
-        -------
-        Plugin and PluginOptions zipped
+        Optional (only when no capture groups are in the regex string). List of names to store the
+        capture group values to. These and ``_sanitized`` versions will be available to use as
+        source variables. The list's length must be equal to the number of match capture groups.
         """
-        return zip(self.plugin_types, self.plugin_options)
+        return [validator.value for validator in self._capture_group_names.list]
 
-    def get(self, plugin_type: Type[TOptionsValidator]) -> Optional[TOptionsValidator]:
+    @property
+    def capture_group_defaults(self) -> Optional[List[StringFormatterValidator]]:
         """
-        Parameters
-        ----------
-        plugin_type
-            Fetch the plugin options for this type
+        Optional. List of string format validators to use for capture group defaults if a
+        source variable cannot be matched. The list's length must be equal to the number of match
+        capture groups.
+        """
+        return self._capture_group_defaults.list if self.has_defaults else None
 
+    @property
+    def has_defaults(self) -> bool:
+        """
         Returns
         -------
-        Options of this plugin if they exit. Otherwise, return None.
+        True if a validation exception should be raised if not captured. False otherwise.
         """
-        plugin_option_types = [type(plugin_options) for plugin_options in self.plugin_options]
-        if plugin_type in plugin_option_types:
-            return self.plugin_options[plugin_option_types.index(plugin_type)]
-        return None
-
+        return self._capture_group_defaults is not None
 
-class DownloadStrategyValidator(StrictDictValidator):
-    """
-    Ensures a download strategy exists for a source. Does not validate any more than that.
-    The respective Downloader's option validator will do that.
-    """
 
-    # All media sources must define a download strategy
-    _required_keys = {"download_strategy"}
+class FromSourceVariablesRegex(StrictDictValidator):
 
-    # Extra fields will be strict-validated using other StictDictValidators
+    _optional_keys = Entry.source_variables()
     _allow_extra_keys = True
 
-    def __init__(self, name: str, value: Any):
-        super().__init__(name=name, value=value)
-        self.download_strategy_name = self._validate_key(
-            key="download_strategy",
-            validator=StringValidator,
+    def __init__(self, name, value):
+        super().__init__(name, value)
+        self.variable_capture_dict: Dict[str, VariableRegex] = {
+            key: self._validate_key(key=key, validator=VariableRegex) for key in self._keys
+        }
+
+
+class RegexOptions(OptionsDictValidator):
+    r"""
+    Performs regex matching on an entry's source or override variables. Regex can be used to filter
+    entries from proceeding with download or capture groups to create new source variables. NOTE to
+    use backslashes anywhere in your regex, i.e. ``\d``, you must add another backslash escape. This
+    means ``\d`` should be written as ``\\d``. This is because YAML requires an escape for any
+    backslash usage.
+
+    If you want to regex-search multiple source variables to create a logical OR effect, you can
+    create an override variable that contains the concatenation of them, and search that with regex.
+    For example, creating the override variable ``"title_and_description": "{title} {description}"``
+    and using ``title_and_description`` can regex match/exclude from either ``title`` or
+    ``description``.
+
+    Usage:
+
+    .. code-block:: yaml
+
+       presets:
+         my_example_preset:
+           regex:
+             # By default, if any match fails and has no defaults, the entry will
+             # be skipped. If False, ytdl-sub will error and stop all downloads
+             # from proceeding.
+             skip_if_match_fails: True
+
+             from:
+               # For each entry's `title` value...
+               title:
+                 # Perform this regex match on it to act as a filter.
+                 # This will only download videos with "[Official Video]" in it. Note that we
+                 # double backslash to make YAML happy
+                 match:
+                   - '\\[Official Video\\]'
+
+               # For each entry's `description` value...
+               description:
+                 # Match with capture groups and defaults.
+                 # This tries to scrape a date from the description and produce new
+                 # source variables
+                 match:
+                   - "([0-9]{4})-([0-9]{2})-([0-9]{2})"
+                 # Exclude any entry where the description contains #short
+                 exclude:
+                   - "#short"
+
+                 # Each capture group creates these new source variables, respectively,
+                 # as well a sanitized version, i.e. `captured_upload_year_sanitized`
+                 capture_group_names:
+                   - "captured_upload_year"
+                   - "captured_upload_month"
+                   - "captured_upload_day"
+
+                 # And if the string does not match, use these as respective default
+                 # values for the new source variables.
+                 capture_group_defaults:
+                   - "{upload_year}"
+                   - "{upload_month}"
+                   - "{upload_day}"
+    """
+
+    _required_keys = {"from"}
+    _optional_keys = {"skip_if_match_fails"}
+
+    @classmethod
+    def partial_validate(cls, name: str, value: Any) -> None:
+        """
+        Partially validate regex
+        """
+        if isinstance(value, dict):
+            value["from"] = value.get("from", {})
+        _ = cls(name, value)
+
+    def __init__(self, name, value):
+        super().__init__(name, value)
+        self._from = self._validate_key(key="from", validator=FromSourceVariablesRegex)
+        self._skip_if_match_fails: bool = self._validate_key_if_present(
+            key="skip_if_match_fails", validator=BoolValidator, default=True
         ).value
 
-    def get(self, downloader_source: str) -> Type[SourcePlugin]:
+    @property
+    def skip_if_match_fails(self) -> Optional[bool]:
+        """
+        Defaults to True. If True, when any match fails and has no defaults, the entry will be
+        skipped. If False, ytdl-sub will error and all downloads will not proceed.
+        """
+        return self._skip_if_match_fails
+
+    def validate_with_variables(
+        self, source_variables: List[str], override_variables: Dict[str, str]
+    ) -> None:
         """
+        Ensures each source variable capture group is valid
+
         Parameters
         ----------
-        downloader_source:
-            Name of the download source
+        source_variables
+            Available source variables when running the plugin
+        override_variables
+            Available override variables when running the plugin
+        """
+        for key, regex_options in self.source_variable_capture_dict.items():
+            # Ensure each variable getting captured is a source variable
+            if key not in source_variables and key not in override_variables:
+                raise self._validation_exception(
+                    f"cannot regex capture '{key}' because it is not a source or override variable"
+                )
 
+            # Ensure the capture group names are not existing source/override variables
+            for capture_group_name in regex_options.capture_group_names:
+                if capture_group_name in source_variables:
+                    raise self._validation_exception(
+                        f"'{capture_group_name}' cannot be used as a capture group name because it "
+                        f"is a source variable"
+                    )
+                if capture_group_name in override_variables:
+                    raise self._validation_exception(
+                        f"'{capture_group_name}' cannot be used as a capture group name because it "
+                        f"is an override variable"
+                    )
+
+    @property
+    def source_variable_capture_dict(self) -> Dict[str, VariableRegex]:
+        """
         Returns
         -------
-        The downloader class
+        Dict of { source variable: capture options }
+        """
+        return self._from.variable_capture_dict
 
-        Raises
-        ------
-        ValidationException
-            If the download strategy is invalid
+    def added_source_variables(self) -> List[str]:
         """
-        try:
-            return DownloadStrategyMapping.get(
-                source=downloader_source, download_strategy=self.download_strategy_name
+        Returns
+        -------
+        List of new source variables created via regex capture
+        """
+        added_source_vars: List[str] = []
+        for regex_options in self.source_variable_capture_dict.values():
+            added_source_vars.extend(regex_options.capture_group_names)
+            added_source_vars.extend(
+                f"{capture_group_name}_sanitized"
+                for capture_group_name in regex_options.capture_group_names
             )
-        except ValueError as value_exc:
-            raise self._validation_exception(error_message=value_exc)
 
+        return added_source_vars
 
-class _PresetShell(StrictDictValidator):
-    # Have all present keys optional since parent presets could not have all the
-    # required keys. They will get validated in the init after the mergedeep of dicts
-    # and ensure required keys are present.
-    _optional_keys = PRESET_KEYS
 
+class RegexPlugin(Plugin[RegexOptions]):
+    plugin_options_type = RegexOptions
+    priority = PluginPriority(
+        modify_entry=PluginPriority.MODIFY_ENTRY_AFTER_SPLIT + 0,
+    )
 
-class Preset(_PresetShell):
     @classmethod
-    def _validate_download_strategy(
-        cls, config: ConfigValidator, name: str, value: Dict, parent_presets: StringListValidator
-    ) -> None:
-        sources: List[str] = []
-        for source_name in DownloadStrategyMapping.sources():
-            if source_name in value:
-                sources.append(source_name)
-
-        if len(sources) > 1:
-            raise validation_exception(
-                name=name,
-                error_message=f"Contains the sources {', '.join(sources)} but can only have one",
-            )
-
-        # If no sources, nothing more to validate
-        if not sources:
-            return
-
-        # Ensure all parent/child presets use the same download strategy
-        preset_strs = [preset.value for preset in parent_presets.list] + [name]
-        download_strategy: Optional[str] = None
-        download_strategy_preset: Optional[str] = None
-        for parent_preset in preset_strs:
-            # See if the parent has a download strategy
-            parent_download_strategy = (
-                config.presets.dict.get(parent_preset, {})
-                .get("download", {})
-                .get("download_strategy")
-            )
-
-            # If the parent download strategy is None, do nothing
-            if parent_download_strategy is None:
-                continue
+    def _add_processed_regex_variable_name(cls, entry: Entry, source_var: str) -> None:
+        if not entry.kwargs_contains(YTDL_SUB_REGEX_SOURCE_VARS):
+            entry.add_kwargs({YTDL_SUB_REGEX_SOURCE_VARS: []})
 
-            # If download strategy is not set, then set it to parent download strategy
-            if download_strategy is None:
-                download_strategy = parent_download_strategy
-                download_strategy_preset = parent_preset
-
-            # If it's set and does not match the parent download strategy, error
-            if download_strategy is not None and download_strategy != parent_download_strategy:
-                raise ValidationException(
-                    f"Preset {download_strategy_preset} uses download strategy {download_strategy}"
-                    f", but is inherited by preset {parent_preset} which uses download strategy "
-                    f"{parent_download_strategy}."
-                )
+        entry.kwargs(YTDL_SUB_REGEX_SOURCE_VARS).append(source_var)
 
-        source_name = sources[0]
-        source_dict = copy.deepcopy(value[source_name])
+    @classmethod
+    def _contains_processed_regex_variable(cls, entry: Entry, variable_name: str) -> bool:
+        return variable_name in entry.kwargs_get(YTDL_SUB_REGEX_SOURCE_VARS, [])
 
-        # Set the parent download strategy if present
-        if download_strategy:
-            source_dict["download_strategy"] = download_strategy
+    def _try_skip_entry(self, entry: Entry, variable_name: str) -> None:
+        # Skip the entry if toggled
+        if self.plugin_options.skip_if_match_fails:
+            logger.info(
+                "Regex failed to match '%s' from '%s', skipping.",
+                variable_name,
+                entry.title,
+            )
+            return None
 
-        downloader = DownloadStrategyValidator(name=f"{name}.{source_name}", value=source_dict).get(
-            downloader_source=source_name
-        )
-        del source_dict["download_strategy"]
+        # Otherwise, error
+        raise RegexNoMatchException(f"Regex failed to match '{variable_name}' from '{entry.title}'")
 
-        downloader.plugin_options_type.partial_validate(
-            name=f"{name}.{source_name}", value=source_dict
-        )
+    def _can_process_at_metadata_stage(self, entry: Entry, variable_name: str) -> bool:
+        # If the variable is an override...
+        if variable_name in self.overrides.dict:
+            # Try to see if it can resolve
+            try:
+                self.overrides.apply_formatter(
+                    formatter=self.overrides.dict[variable_name],
+                    entry=entry,
+                )
+            # If it can not from missing variables (from post-metadata stage), return False
+            except StringFormattingVariableNotFoundException:
+                return False
+        # If it is a source variable and not present, return false
+        elif variable_name not in entry.to_dict():
+            return False
+
+        return True
+
+    def _get_regex_input_string(self, entry: Entry, variable_name: str) -> str:
+        # Apply override formatter if it's an override
+        if variable_name in self.overrides.dict:
+            return self.overrides.apply_formatter(
+                formatter=self.overrides.dict[variable_name],
+                entry=entry,
+            )
+        # Otherwise pluck from the entry's source variable
+        return entry.to_dict()[variable_name]
 
-    @classmethod
-    def preset_partial_validate(cls, config: ConfigValidator, name: str, value: Any) -> None:
+    def _modify_entry_metadata(self, entry: Entry, is_metadata_stage: bool) -> Optional[Entry]:
         """
-        Partially validates a preset. Used to ensure every preset in a ConfigFile looks sane.
-        Cannot fully validate each preset using the Preset init because required fields could
-        be missing, which become filled in a child preset.
-
         Parameters
         ----------
-        config
-            Config that this preset belongs to
-        name
-            Preset name
-        value
-            Preset value
+        entry
+            Entry to add source variables to
+        is_metadata_stage
+            Whether this is called at the metadata stage or modify stage
+
+        Returns
+        -------
+        Entry with regex capture variables added to its source variables
 
         Raises
         ------
         ValidationException
-            If validation fails
+            If no capture and no defaults
         """
-        # Ensure value is a dict
-        _ = _PresetShell(name=name, value=value)
-        assert isinstance(value, dict)
-
-        parent_presets = StringListValidator(name=f"{name}.preset", value=value.get("preset", []))
-        for parent_preset_name in parent_presets.list:
-            if parent_preset_name.value not in config.presets.keys:
-                raise _parent_preset_error_message(
-                    current_preset_name=name,
-                    parent_preset_name=parent_preset_name.value,
-                    presets=config.presets.keys,
-                )
-
-        cls._validate_download_strategy(
-            config=config, name=name, value=value, parent_presets=parent_presets
-        )
-        cls._partial_validate_key(name, value, "output_options", OutputOptions)
-        cls._partial_validate_key(name, value, "ytdl_options", YTDLOptions)
-        cls._partial_validate_key(name, value, "overrides", Overrides)
-
-        for plugin_name in PluginMapping.plugins():
-            cls._partial_validate_key(
-                name,
-                value,
-                key=plugin_name,
-                validator=PluginMapping.get(plugin_name).plugin_options_type,
-            )
-
-    @property
-    def _source_variables(self) -> List[str]:
-        return Entry.source_variables()
-
-    def __validate_and_get_downloader(self, downloader_source: str) -> Type[SourcePlugin]:
-        return self._validate_key(key=downloader_source, validator=DownloadStrategyValidator).get(
-            downloader_source=downloader_source
-        )
-
-    def __validate_and_get_downloader_options(
-        self, downloader_source: str, downloader: Type[SourcePlugin]
-    ) -> OptionsValidator:
-        # Remove the download_strategy key before validating it against the downloader options
-        # TODO: make this cleaner
-        del self._dict[downloader_source]["download_strategy"]
-        return self._validate_key(key=downloader_source, validator=downloader.plugin_options_type)
-
-    def __validate_and_get_downloader_and_options(
-        self,
-    ) -> Tuple[Type[SourcePlugin], OptionsValidator]:
-        downloader: Optional[Type[SourcePlugin]] = None
-        download_options: Optional[OptionsValidator] = None
-        downloader_sources = DownloadStrategyMapping.sources()
-
-        for key in self._keys:
-            # skip if the key is not a download source
-            if key not in downloader_sources:
+        # Iterate each source var to capture and add to the entry
+        for (
+            variable_name,
+            regex_options,
+        ) in self.plugin_options.source_variable_capture_dict.items():
+
+            # Record which regex source variables are processed, to
+            # process as many variables as possible in the metadata stage, then the rest
+            # after the media file has been downloaded.
+            if self._contains_processed_regex_variable(entry, variable_name):
                 continue
 
-            # Ensure there are not multiple sources, i.e. youtube and soundcloud
-            if downloader:
-                raise self._validation_exception(
-                    f"'{self._name}' can only have one of the following sources: "
-                    f"{', '.join(downloader_sources)}"
-                )
-
-            downloader = self.__validate_and_get_downloader(downloader_source=key)
-            download_options = self.__validate_and_get_downloader_options(
-                downloader_source=key, downloader=downloader
-            )
-
-        # If downloader was not set, error since it is required
-        if not downloader:
-
-            raise self._validation_exception(
-                f"'{self._name} must have one of the following sources: "
-                f"{', '.join(downloader_sources)}"
-            )
-
-        return downloader, download_options
-
-    def __validate_and_get_plugins(self) -> PresetPlugins:
-        preset_plugins = PresetPlugins()
-
-        for key in self._keys:
-            if key not in PluginMapping.plugins():
+            # If it's the metadata stage, and it can't be processed, skip until post-metadata
+            if is_metadata_stage and not self._can_process_at_metadata_stage(
+                entry=entry, variable_name=variable_name
+            ):
                 continue
 
-            plugin = PluginMapping.get(plugin=key)
-            plugin_options = self._validate_key(key=key, validator=plugin.plugin_options_type)
-
-            preset_plugins.add(plugin_type=plugin, plugin_options=plugin_options)
-
-        return preset_plugins
-
-    def __validate_added_variables(self):
-        source_variables = copy.deepcopy(self._source_variables)
-
-        # Validate added download option variables here since plugins could subsequently use them
-        self.downloader_options.validate_with_variables(
-            source_variables=source_variables,
-            override_variables=self.overrides.dict_with_format_strings,
-        )
-        source_variables.extend(self.downloader_options.added_source_variables())
+            self._add_processed_regex_variable_name(entry, variable_name)
 
-        for _, plugin_options in sorted(
-            self.plugins.zipped(), key=lambda pl: pl[0].priority.modify_entry
-        ):
-            # Validate current plugin using source + added plugin variables
-            plugin_options.validate_with_variables(
-                source_variables=source_variables,
-                override_variables=self.overrides.dict_with_format_strings,
+            regex_input_str = self._get_regex_input_string(
+                entry=entry,
+                variable_name=variable_name,
             )
 
-            # Extend existing source variables with ones created from this plugin
-            source_variables.extend(plugin_options.added_source_variables())
-
-    def __validate_override_string_formatter_validator(
-        self,
-        formatter_validator: Union[StringFormatterValidator, OverridesStringFormatterValidator],
-    ):
-        # Set the formatter variables to be the overrides
-        variable_dict = copy.deepcopy(self.overrides.dict_with_format_strings)
-
-        # If the formatter supports source variables, set the formatter variables to include
-        # both source and override variables
-        if not isinstance(formatter_validator, OverridesStringFormatterValidator):
-            source_variables = {
-                source_var: "dummy_string"
-                for source_var in self._source_variables
-                + self.downloader_options.added_source_variables()
-            }
-            variable_dict = dict(source_variables, **variable_dict)
-
-            # For all plugins, add in any extra added source variables
-            for plugin_options in self.plugins.plugin_options:
-                added_plugin_variables = {
-                    source_var: "dummy_string"
-                    for source_var in plugin_options.added_source_variables()
-                }
-                # sanity check plugin variables do not override source variables
-                expected_len = len(variable_dict) + len(added_plugin_variables)
-                variable_dict = dict(variable_dict, **added_plugin_variables)
-
-                assert (
-                    len(variable_dict) == expected_len
-                ), "plugin variables overwrote source variables"
-
-        _ = formatter_validator.apply_formatter(variable_dict=variable_dict)
-
-    def __recursive_preset_validate(
-        self,
-        validator: Optional[Validator] = None,
-    ) -> None:
-        """
-        Ensure all OverridesStringFormatterValidator's only contain variables from the overrides
-        and resolve.
-        """
-        if validator is None:
-            validator = self
-
-        if isinstance(validator, DictValidator):
-            # pylint: disable=protected-access
-            # Usage of protected variables in other validators is fine. The reason to keep
-            # them protected is for readability when using them in subscriptions.
-            for validator_value in validator._validator_dict.values():
-                self.__recursive_preset_validate(validator_value)
-            # pylint: enable=protected-access
-        elif isinstance(validator, ListValidator):
-            for list_value in validator.list:
-                self.__recursive_preset_validate(list_value)
-        elif isinstance(validator, (StringFormatterValidator, OverridesStringFormatterValidator)):
-            self.__validate_override_string_formatter_validator(validator)
-        elif isinstance(validator, (DictFormatterValidator, OverridesDictFormatterValidator)):
-            for validator_value in validator.dict.values():
-                self.__validate_override_string_formatter_validator(validator_value)
-
-    def _get_presets_to_merge(
-        self, parent_presets: str | List[str], seen_presets: List[str], config: ConfigValidator
-    ) -> List[Dict]:
-        presets_to_merge: List[Dict] = []
-
-        if isinstance(parent_presets, str):
-            parent_presets = [parent_presets]
-
-        for parent_preset in reversed(parent_presets):
-            # Make sure we do not hit an infinite loop
-            if parent_preset in seen_presets:
-                raise self._validation_exception(
-                    f"preset loop detected with the preset '{parent_preset}'"
-                )
-
-            # Make sure the parent preset actually exists
-            if parent_preset not in config.presets.keys:
-                raise _parent_preset_error_message(
-                    current_preset_name=self._name,
-                    parent_preset_name=parent_preset,
-                    presets=config.presets.keys,
-                )
-
-            parent_preset_dict = copy.deepcopy(config.presets.dict[parent_preset])
-            presets_to_merge.append(parent_preset_dict)
-
-            if "preset" in parent_preset_dict:
-                presets_to_merge.extend(
-                    self._get_presets_to_merge(
-                        parent_presets=parent_preset_dict["preset"],
-                        seen_presets=seen_presets + [parent_preset],
-                        config=config,
+            if (
+                regex_options.exclude is not None
+                and regex_options.exclude.match_any(input_str=regex_input_str) is not None
+            ):
+                return self._try_skip_entry(entry=entry, variable_name=variable_name)
+
+            # If match is present
+            if regex_options.match is not None:
+                maybe_capture = regex_options.match.match_any(input_str=regex_input_str)
+
+                # And nothing matched
+                if maybe_capture is None:
+                    # and no defaults
+                    if not regex_options.has_defaults:
+                        return self._try_skip_entry(entry=entry, variable_name=variable_name)
+
+                    # otherwise, use defaults (apply them using the original entry source dict)
+                    source_variables_and_overrides_dict = dict(
+                        entry.to_dict(), **self.overrides.dict_with_format_strings
                     )
-                )
-
-        return presets_to_merge
-
-    def __merge_parent_preset_dicts_if_present(self, config: ConfigValidator):
-        parent_preset_validator = self._validate_key_if_present(
-            key="preset", validator=StringListValidator
-        )
-        if parent_preset_validator is None:
-            return
-
-        # Get list of all parent presets in depth-first search order, beginning with this preset
-        presets_to_merge: List[Dict] = [copy.deepcopy(self._value)] + self._get_presets_to_merge(
-            parent_presets=[preset.value for preset in parent_preset_validator.list],
-            seen_presets=[],
-            config=config,
-        )
-
-        # Merge all presets
-        self._value = dict(
-            mergedeep.merge({}, *reversed(presets_to_merge), strategy=mergedeep.Strategy.ADDITIVE)
-        )
-
-    def __init__(self, config: ConfigValidator, name: str, value: Any):
-        super().__init__(name=name, value=value)
-
-        # Perform the merge of parent presets before validating any keys
-        self.__merge_parent_preset_dicts_if_present(config=config)
-
-        self.downloader, self.downloader_options = self.__validate_and_get_downloader_and_options()
-
-        self.output_options = self._validate_key(
-            key="output_options",
-            validator=OutputOptions,
-        )
-
-        self.ytdl_options = self._validate_key(
-            key="ytdl_options", validator=YTDLOptions, default={}
-        )
 
-        self.overrides = self._validate_key(key="overrides", validator=Overrides, default={})
-        self.plugins: PresetPlugins = self.__validate_and_get_plugins()
-        self.__validate_added_variables()
-
-        # After all options are initialized, perform a recursive post-validate that requires
-        # values from multiple validators
-        self.__recursive_preset_validate()
+                    # add both the default...
+                    entry.add_variables(
+                        variables_to_add={
+                            regex_options.capture_group_names[i]: default.apply_formatter(
+                                variable_dict=source_variables_and_overrides_dict
+                            )
+                            for i, default in enumerate(regex_options.capture_group_defaults)
+                        },
+                    )
+                    # and sanitized default
+                    entry.add_variables(
+                        variables_to_add={
+                            f"{regex_options.capture_group_names[i]}_sanitized": sanitize_filename(
+                                default.apply_formatter(
+                                    variable_dict=source_variables_and_overrides_dict
+                                )
+                            )
+                            for i, default in enumerate(regex_options.capture_group_defaults)
+                        },
+                    )
+                # There is a capture, add the source variables to the entry as
+                # {source_var}_capture_1, {source_var}_capture_2, ...
+                else:
+                    # Add the value...
+                    entry.add_variables(
+                        variables_to_add={
+                            regex_options.capture_group_names[i]: capture
+                            for i, capture in enumerate(maybe_capture)
+                        },
+                    )
+                    # And the sanitized value
+                    entry.add_variables(
+                        variables_to_add={
+                            f"{regex_options.capture_group_names[i]}_sanitized": sanitize_filename(
+                                capture
+                            )
+                            for i, capture in enumerate(maybe_capture)
+                        },
+                    )
 
-    @property
-    def name(self) -> str:
-        """
-        Returns
-        -------
-        Name of the preset
-        """
-        return self._name
+        return entry
 
-    @classmethod
-    def from_dict(cls, config: ConfigValidator, preset_name: str, preset_dict: Dict) -> "Preset":
+    def modify_entry_metadata(self, entry: Entry) -> Optional[Entry]:
         """
-        Parameters
-        ----------
-        config:
-            Validated instance of the config
-        preset_name:
-            Name of the preset
-        preset_dict:
-            The preset config in dict format
-
-        Returns
-        -------
-        The Subscription validator
+        Perform regex at the metadata stage
         """
-        return cls(config=config, name=preset_name, value=preset_dict)
+        return self._modify_entry_metadata(entry, is_metadata_stage=True)
 
-    @property
-    def yaml(self) -> str:
+    def modify_entry(self, entry: Entry) -> Optional[Entry]:
         """
-        Returns
-        -------
-        Preset in YAML format
+        Perform regex at the metadata stage
         """
-        return dump_yaml({"presets": {self._name: self._value}})
+        return self._modify_entry_metadata(entry, is_metadata_stage=False)
```

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/source_plugin.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/source_plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import contextlib
 import os
-from abc import ABC
 from pathlib import Path
 from typing import Dict
 from typing import Iterable
 from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Set
@@ -184,15 +183,15 @@
         )
 
         entry.add_variables(variables_to_add=collection_url.variables.dict_with_format_strings)
 
         return entry
 
 
-class MultiUrlDownloader(SourcePlugin[MultiUrlValidator], ABC):
+class MultiUrlDownloader(SourcePlugin[MultiUrlValidator]):
     """
     Class that interacts with ytdl to perform the download of metadata and content,
     and should translate that to list of Entry objects.
     """
 
     plugin_options_type = MultiUrlValidator
     plugin_extensions = [UrlDownloaderThumbnailPlugin, UrlDownloaderCollectionVariablePlugin]
```

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/url/url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/main.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/embed_thumbnail.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/embed_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.7.26/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from abc import ABC
 from pathlib import Path
-from typing import Type
 
 from ytdl_sub.config.config_validator import ConfigOptions
 from ytdl_sub.config.preset import Preset
 from ytdl_sub.config.preset import PresetPlugins
-from ytdl_sub.config.preset_options import OptionsValidator
 from ytdl_sub.config.preset_options import OutputOptions
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.config.preset_options import YTDLOptions
-from ytdl_sub.downloaders.source_plugin import SourcePlugin
+from ytdl_sub.downloaders.url.validators import MultiUrlValidator
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 
 class BaseSubscription(ABC):
     """
     Subscription classes are the 'controllers' that perform...
 
@@ -48,24 +46,15 @@
         self._enhanced_download_archive = EnhancedDownloadArchive(
             file_name=self.overrides.apply_formatter(self.output_options.download_archive_name),
             working_directory=self.working_directory,
             output_directory=self.output_directory,
         )
 
     @property
-    def downloader_class(self) -> Type[SourcePlugin]:
-        """
-        Returns
-        -------
-        This subscription's downloader class
-        """
-        return self._preset_options.downloader
-
-    @property
-    def downloader_options(self) -> OptionsValidator:
+    def downloader_options(self) -> MultiUrlValidator:
         """
         Returns
         -------
         The download options for this subscription's downloader
         """
         return self._preset_options.downloader_options
```

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Optional
 
 from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.plugin import SplitPlugin
 from ytdl_sub.downloaders.info_json.info_json_downloader import InfoJsonDownloader
 from ytdl_sub.downloaders.info_json.info_json_downloader import InfoJsonDownloaderOptions
 from ytdl_sub.downloaders.source_plugin import SourcePlugin
+from ytdl_sub.downloaders.url.downloader import MultiUrlDownloader
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.subscriptions.base_subscription import BaseSubscription
 from ytdl_sub.subscriptions.subscription_ytdl_options import SubscriptionYTDLOptions
 from ytdl_sub.utils.datetime import to_date_range
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.file_handler import FileHandler
@@ -326,15 +327,15 @@
             preset=self._preset_options,
             plugins=plugins,
             enhanced_download_archive=self._enhanced_download_archive,
             working_directory=self.working_directory,
             dry_run=dry_run,
         )
 
-        downloader = self.downloader_class(
+        downloader = MultiUrlDownloader(
             options=self.downloader_options,
             enhanced_download_archive=self._enhanced_download_archive,
             download_ytdl_options=subscription_ytdl_options.download_builder(),
             metadata_ytdl_options=subscription_ytdl_options.metadata_builder(),
             overrides=self.overrides,
         )
 
@@ -364,15 +365,15 @@
             enhanced_download_archive=self._enhanced_download_archive,
             working_directory=self.working_directory,
             dry_run=dry_run,
         )
 
         # Re-add the original downloader class' plugins
         plugins.extend(
-            self.downloader_class(
+            MultiUrlDownloader(
                 options=self.downloader_options,
                 enhanced_download_archive=self._enhanced_download_archive,
                 download_ytdl_options=subscription_ytdl_options.download_builder(),
                 metadata_ytdl_options=subscription_ytdl_options.metadata_builder(),
                 overrides=self.overrides,
             ).added_plugins()
         )
```

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 
 from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset import Preset
-from ytdl_sub.downloaders.source_plugin import SourcePlugin
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.plugins.audio_extract import AudioExtractPlugin
 from ytdl_sub.plugins.chapters import ChaptersPlugin
 from ytdl_sub.plugins.date_range import DateRangePlugin
 from ytdl_sub.plugins.file_convert import FileConvertPlugin
 from ytdl_sub.plugins.match_filters import MatchFiltersPlugin
 from ytdl_sub.plugins.subtitles import SubtitlesPlugin
@@ -39,18 +38,14 @@
     def _get_plugin(self, plugin_type: Type[PluginT]) -> Optional[PluginT]:
         for plugin in self._plugins:
             if isinstance(plugin, plugin_type):
                 return plugin
         return None
 
     @property
-    def _downloader(self) -> Type[SourcePlugin]:
-        return self._preset.downloader
-
-    @property
     def _global_options(self) -> Dict:
         """
         Returns
         -------
         ytdl-options to apply to every run no matter what
         """
         ytdl_options = {
```

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.7.26/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.7.26/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.25.post7
+Version: 2023.7.26
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.25.post7/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.7.26/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

