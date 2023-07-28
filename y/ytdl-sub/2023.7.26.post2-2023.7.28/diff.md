# Comparing `tmp/ytdl-sub-2023.7.26.post2.tar.gz` & `tmp/ytdl-sub-2023.7.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.7.26.post2.tar", last modified: Wed Jul 26 16:01:24 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.7.28.tar", last modified: Fri Jul 28 20:14:04 2023, max compression
```

## Comparing `ytdl-sub-2023.7.26.post2.tar` & `ytdl-sub-2023.7.28.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.916410 ytdl-sub-2023.7.26.post2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-26 16:01:24.916410 ytdl-sub-2023.7.26.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-26 16:01:24.916410 ytdl-sub-2023.7.26.post2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.872409 ytdl-sub-2023.7.26.post2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.880409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.884409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.888409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.888409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.888409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/source_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.892409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19945 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.892409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.892409 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.900410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/embed_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.900410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.900410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.900410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.900410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.904410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.904410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    15182 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.904410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.912410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.916410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.916410 ytdl-sub-2023.7.26.post2/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-26 16:01:04.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:01:24.884409 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-26 16:01:24.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-26 16:01:24.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:01:24.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 16:01:24.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 16:01:24.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 16:01:24.000000 ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.468413 ytdl-sub-2023.7.28/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-07-28 20:14:04.468413 ytdl-sub-2023.7.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-28 20:14:04.472413 ytdl-sub-2023.7.28/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.456413 ytdl-sub-2023.7.28/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.456413 ytdl-sub-2023.7.28/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 20:13:44.000000 ytdl-sub-2023.7.28/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.460413 ytdl-sub-2023.7.28/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.460413 ytdl-sub-2023.7.28/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/config/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.460413 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.460413 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/source_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.460413 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20124 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.460413 ytdl-sub-2023.7.28/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.460413 ytdl-sub-2023.7.28/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.464413 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.464413 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.464413 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.464413 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.464413 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.464413 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.464413 ytdl-sub-2023.7.28/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.468413 ytdl-sub-2023.7.28/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.468413 ytdl-sub-2023.7.28/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.468413 ytdl-sub-2023.7.28/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.468413 ytdl-sub-2023.7.28/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-28 20:13:43.000000 ytdl-sub-2023.7.28/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:14:04.456413 ytdl-sub-2023.7.28/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-07-28 20:14:04.000000 ytdl-sub-2023.7.28/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-28 20:14:04.000000 ytdl-sub-2023.7.28/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:14:04.000000 ytdl-sub-2023.7.28/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-28 20:14:04.000000 ytdl-sub-2023.7.28/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-28 20:14:04.000000 ytdl-sub-2023.7.28/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 20:14:04.000000 ytdl-sub-2023.7.28/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.7.26.post2/LICENSE` & `ytdl-sub-2023.7.28/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/PKG-INFO` & `ytdl-sub-2023.7.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.26.post2
+Version: 2023.7.28
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.26.post2/README.md` & `ytdl-sub-2023.7.28/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/pyproject.toml` & `ytdl-sub-2023.7.28/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/setup.cfg` & `ytdl-sub-2023.7.28/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/defaults.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/plugin.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/config/plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/config/preset_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
            output_options:
              # required
              output_directory: "/path/to/videos_or_music"
              file_name: "{title_sanitized}.{ext}"
              # optional
              thumbnail_name: "{title_sanitized}.{thumbnail_ext}"
              info_json_name: "{title_sanitized}.{info_json_ext}"
-             download_archive_name: ".ytdl-sub-{subscription_name}-download-archive.txt"
+             download_archive_name: ".ytdl-sub-{subscription_name}-download-archive.json"
              maintain_download_archive: True
              keep_files_before: now
              keep_files_after: 19000101
     """
 
     _required_keys = {"output_directory", "file_name"}
     _optional_keys = {
@@ -350,15 +350,15 @@
         """
         return self._info_json_name
 
     @property
     def download_archive_name(self) -> Optional[OverridesStringFormatterValidator]:
         """
         Optional. The file name to store a subscriptions download archive placed relative to
-        the output directory. Defaults to ``.ytdl-sub-{subscription_name}-download-archive.txt``
+        the output directory. Defaults to ``.ytdl-sub-{subscription_name}-download-archive.json``
         """
         return self._download_archive_name
 
     @property
     def maintain_download_archive(self) -> bool:
         """
         Optional. Maintains a download archive file in the output directory for a subscription.
```

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/source_plugin.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/source_plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 from ytdl_sub.entries.variables.kwargs import SOURCE_ENTRY
 from ytdl_sub.entries.variables.kwargs import SPONSORBLOCK_CHAPTERS
 from ytdl_sub.entries.variables.kwargs import UPLOAD_DATE_INDEX
 from ytdl_sub.entries.variables.kwargs import YTDL_SUB_MATCH_FILTER_REJECT
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.utils.thumbnail import ThumbnailTypes
-from ytdl_sub.utils.thumbnail import convert_download_thumbnail
 from ytdl_sub.utils.thumbnail import download_and_convert_url_thumbnail
+from ytdl_sub.utils.thumbnail import try_convert_download_thumbnail
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 download_logger = Logger.get(name="downloader")
 
 
 class URLDownloadState:
     def __init__(self, entries_total: int):
@@ -78,19 +78,17 @@
         """
         for thumbnail_info in thumbnail_list_info.list:
             thumbnail_name = self.overrides.apply_formatter(thumbnail_info.name, entry=entry)
             thumbnail_id = self.overrides.apply_formatter(thumbnail_info.uid)
 
             # If latest entry, always update the thumbnail on each entry
             if thumbnail_id == ThumbnailTypes.LATEST_ENTRY:
-                # Make sure the entry's thumbnail is converted to jpg
-                convert_download_thumbnail(entry, error_if_not_found=False)
 
                 # always save in dry-run even if it doesn't exist...
-                if self.is_dry_run or os.path.isfile(entry.get_download_thumbnail_path()):
+                if self.is_dry_run or entry.is_thumbnail_downloaded():
                     self.save_file(
                         file_name=entry.get_download_thumbnail_name(),
                         output_file_name=thumbnail_name,
                         copy_file=True,
                     )
                     self._thumbnails_downloaded.add(thumbnail_name)
                 continue
@@ -134,16 +132,22 @@
                 parent=EntryParent(
                     entry.kwargs(SOURCE_ENTRY), working_directory=self.working_directory
                 ),
             )
 
     def modify_entry(self, entry: Entry) -> Optional[Entry]:
         """
-        Use the entry to download thumbnails (or move if LATEST_ENTRY)
+        Use the entry to download thumbnails (or move if LATEST_ENTRY).
+        In addition, convert the entry thumbnail to jpg
         """
+        # We always convert entry thumbnails to jpgs, and is performed here to be done
+        # as early as possible in the plugin pipeline (downstream plugins depend on it being jpg)
+        if not self.is_dry_run:
+            try_convert_download_thumbnail(entry=entry)
+
         if entry.kwargs_get(COLLECTION_URL) in self._collection_url_mapping:
             self._download_url_thumbnails(
                 collection_url=self._collection_url_mapping[entry.kwargs(COLLECTION_URL)],
                 entry=entry,
             )
         return entry
 
@@ -342,15 +346,15 @@
 
     def _extract_entry_info_with_retry(self, entry: Entry) -> Entry:
         download_entry_dict = YTDLP.extract_info_with_retry(
             ytdl_options_overrides=self.download_ytdl_options,
             is_downloaded_fn=None if self.is_dry_run else entry.is_downloaded,
             is_thumbnail_downloaded_fn=None
             if (self.is_dry_run or not self.is_entry_thumbnails_enabled)
-            else entry.is_thumbnail_downloaded,
+            else entry.is_thumbnail_downloaded_via_ytdlp,
             url=entry.webpage_url,
         )
         return Entry(download_entry_dict, working_directory=self.working_directory)
 
     def _iterate_child_entries(
         self, url_validator: UrlValidator, entries: List[Entry]
     ) -> Iterator[Entry]:
```

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/url/url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,18 +82,20 @@
 
         Raises
         ------
         FileNotDownloadedException
             If the entry fails to download
         """
         num_tries = 0
-        entry_files_exist = False
         copied_ytdl_options_overrides = copy.deepcopy(ytdl_options_overrides)
 
-        while not entry_files_exist and num_tries < cls._EXTRACT_ENTRY_NUM_RETRIES:
+        is_downloaded = False
+        entry_dict: Optional[Dict] = None
+
+        while num_tries < cls._EXTRACT_ENTRY_NUM_RETRIES:
             entry_dict = cls.extract_info(
                 ytdl_options_overrides=copied_ytdl_options_overrides, **kwargs
             )
 
             is_downloaded = is_downloaded_fn is None or is_downloaded_fn()
             is_thumbnail_downloaded = (
                 is_thumbnail_downloaded_fn is None or is_thumbnail_downloaded_fn()
@@ -111,26 +113,30 @@
             if is_downloaded and not is_thumbnail_downloaded:
                 copied_ytdl_options_overrides["skip_download"] = True
                 copied_ytdl_options_overrides["writethumbnail"] = True
 
             time.sleep(cls._EXTRACT_ENTRY_RETRY_WAIT_SEC)
             num_tries += 1
 
-            # Remove the download archive so it can retry without thinking its already downloaded,
+            # Remove the download archive to retry without thinking its already downloaded,
             # even though it is not
             if "download_archive" in copied_ytdl_options_overrides:
                 del copied_ytdl_options_overrides["download_archive"]
 
             if num_tries < cls._EXTRACT_ENTRY_NUM_RETRIES:
                 cls.logger.debug(
                     "Failed to download entry. Retrying %d / %d",
                     num_tries,
                     cls._EXTRACT_ENTRY_NUM_RETRIES,
                 )
 
+        # Still return if the media file downloaded (thumbnail could be missing)
+        if is_downloaded and entry_dict is not None:
+            return entry_dict
+
         error_dict = {"ytdl_options": ytdl_options_overrides, "kwargs": kwargs}
         raise FileNotDownloadedException(
             f"yt-dlp failed to download an entry with these arguments: {error_dict}"
         )
 
     @classmethod
     def _get_entry_dicts_from_info_json_files(cls, working_directory: str) -> List[Dict]:
```

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/entries/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         """
         return f"{self.uid}.{self.thumbnail_ext}"
 
     def get_download_thumbnail_path(self) -> str:
         """Returns the entry's thumbnail's file path to where it was downloaded"""
         return str(Path(self.working_directory()) / self.get_download_thumbnail_name())
 
-    def get_ytdlp_download_thumbnail_path(self) -> Optional[str]:
+    def try_get_ytdlp_download_thumbnail_path(self) -> Optional[str]:
         """
         The source `thumbnail` value and the actual downloaded thumbnail extension sometimes do
         not match. Return the actual downloaded thumbnail path.
         """
         thumbnails = self.kwargs_get("thumbnails", [])
         possible_thumbnail_exts = {"jpg", "webp"}  # Always check for jpg and webp thumbs
 
@@ -80,21 +80,30 @@
         kwargs_dict["ytdl_sub_entry_variables"] = self.to_dict()
         kwargs_json = json.dumps(kwargs_dict, ensure_ascii=False, sort_keys=True, indent=2)
 
         with open(self.get_download_info_json_path(), "w", encoding="utf-8") as file:
             file.write(kwargs_json)
 
     @final
+    def is_thumbnail_downloaded_via_ytdlp(self) -> bool:
+        """
+        Returns
+        -------
+        True if ANY thumbnail file exist locally. False otherwise.
+        """
+        return self.try_get_ytdlp_download_thumbnail_path() is not None
+
+    @final
     def is_thumbnail_downloaded(self) -> bool:
         """
         Returns
         -------
-        True if the thumbnail file exist locally. False otherwise.
+        True if the thumbnail file exists and is its proper format. False otherwise.
         """
-        return self.get_ytdlp_download_thumbnail_path() is not None
+        return os.path.isfile(self.get_download_thumbnail_path())
 
     @final
     def is_downloaded(self) -> bool:
         """
         Returns
         -------
         True if the file exist locally. False otherwise.
```

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/main.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/embed_thumbnail.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/embed_thumbnail.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from ytdl_sub.config.plugin import PluginPriority
 from ytdl_sub.config.preset_options import OptionsValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.utils.ffmpeg import FFMPEG
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.logger import Logger
-from ytdl_sub.utils.thumbnail import convert_download_thumbnail
 from ytdl_sub.validators.audo_codec_validator import AUDIO_CODEC_EXTS
 from ytdl_sub.validators.validators import BoolValidator
 
 logger = Logger.get("embed_thumbnail")
 
 
 class EmbedThumbnailOptions(BoolValidator, OptionsValidator):
@@ -87,16 +86,19 @@
             return None
 
         if entry.ext == "webm":
             logger.warning("webm does not support embedded thumbnails, skipping")
             return None
 
         if not self.is_dry_run:
-            # convert the entry thumbnail so it is embedded as jpg
-            convert_download_thumbnail(entry=entry)
+            if not entry.is_thumbnail_downloaded():
+                logger.warning(
+                    "Cannot embed thumbnail for '%s' because it is not available", entry.title
+                )
+                return None
 
             if entry.ext in AUDIO_CODEC_EXTS:
                 self._embed_audio_file(entry)
             else:
                 self._embed_video_thumbnail(entry)
 
         return FileMetadata("Embedded thumbnail")
```

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/music_tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import mediafile
 
 from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.logger import Logger
-from ytdl_sub.utils.thumbnail import convert_download_thumbnail
 from ytdl_sub.validators.audo_codec_validator import AUDIO_CODEC_EXTS
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
 from ytdl_sub.validators.string_formatter_validators import ListFormatterValidator
 from ytdl_sub.validators.string_formatter_validators import StringFormatterValidator
 from ytdl_sub.validators.validators import BoolValidator
 
 logger = Logger.get("music_tags")
@@ -158,19 +157,15 @@
                         logger.warning(
                             "Music tag '%s' does not support lists. "
                             "Only setting the first element",
                             tag_name,
                         )
                     setattr(audio_file, tag_name, tag_value[0])
 
-            if self.plugin_options.embed_thumbnail:
-
-                # convert the entry thumbnail so it is embedded as jpg
-                convert_download_thumbnail(entry=entry)
-
+            if self.plugin_options.embed_thumbnail and entry.is_thumbnail_downloaded():
                 with open(entry.get_download_thumbnail_path(), "rb") as thumb:
                     mediafile_img = mediafile.Image(
                         data=thumb.read(), desc="cover", type=mediafile.ImageType.front
                     )
 
                 audio_file.images = [mediafile_img]
```

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import copy
-import os.path
 from pathlib import Path
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from yt_dlp.utils import sanitize_filename
@@ -17,15 +16,14 @@
 from ytdl_sub.entries.variables.kwargs import UID
 from ytdl_sub.utils.chapters import Chapters
 from ytdl_sub.utils.chapters import Timestamp
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.ffmpeg import FFMPEG
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileMetadata
-from ytdl_sub.utils.thumbnail import convert_download_thumbnail
 from ytdl_sub.validators.string_select_validator import StringSelectValidator
 
 
 def _split_video_ffmpeg_cmd(
     input_file: str, output_file: str, timestamps: List[Timestamp], idx: int
 ) -> List[str]:
     timestamp_begin = timestamps[idx].standardized_str
@@ -180,19 +178,14 @@
             if self.plugin_options.when_no_chapters == "drop":
                 return []
 
             raise ValidationException(
                 f"Tried to split '{entry.title}' by chapters but it has no chapters"
             )
 
-        # convert the entry thumbnail early so we do not have to guess the thumbnail extension
-        # when copying it. Do not error if it's not found, in case thumbnail_name is not set
-        if not self.is_dry_run:
-            convert_download_thumbnail(entry=entry, error_if_not_found=False)
-
         for idx, title in enumerate(chapters.titles):
             new_uid = _split_video_uid(source_uid=entry.uid, idx=idx)
 
             if not self.is_dry_run:
                 # Get the input/output file paths
                 input_file = entry.get_download_file_path()
                 output_file = str(Path(self.working_directory) / f"{new_uid}.{entry.ext}")
@@ -205,15 +198,15 @@
                         timestamps=chapters.timestamps,
                         idx=idx,
                     )
                 )
 
                 # Copy the original vid thumbnail to the working directory with the new uid. This so
                 # downstream logic thinks this split video has its own thumbnail
-                if os.path.isfile(entry.get_download_thumbnail_path()):
+                if entry.is_thumbnail_downloaded():
                     FileHandler.copy(
                         src_file_path=entry.get_download_thumbnail_path(),
                         dst_file_path=Path(self.working_directory)
                         / f"{new_uid}.{entry.thumbnail_ext}",
                     )
 
             # Format the split video
```

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.7.28/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import contextlib
+import logging
 import os
 import shutil
 from abc import ABC
 from pathlib import Path
 from typing import List
 from typing import Optional
 
@@ -17,15 +18,17 @@
 from ytdl_sub.subscriptions.base_subscription import BaseSubscription
 from ytdl_sub.subscriptions.subscription_ytdl_options import SubscriptionYTDLOptions
 from ytdl_sub.utils.datetime import to_date_range
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileHandlerTransactionLog
 from ytdl_sub.utils.file_handler import FileMetadata
-from ytdl_sub.utils.thumbnail import convert_download_thumbnail
+from ytdl_sub.utils.logger import Logger
+
+logger: logging.Logger = Logger.get()
 
 
 def _get_split_plugin(plugins: List[Plugin]) -> Optional[SplitPlugin]:
     split_plugins = [plugin for plugin in plugins if isinstance(plugin, SplitPlugin)]
 
     if len(split_plugins) == 1:
         return split_plugins[0]
@@ -65,31 +68,31 @@
         self._enhanced_download_archive.save_file_to_output_directory(
             file_name=entry.get_download_file_name(),
             file_metadata=entry_metadata,
             output_file_name=output_file_name,
             entry=entry,
         )
 
-        # TODO: see if entry even has a thumbnail
-        if self.output_options.thumbnail_name:
+        # Always pretend to include the thumbnail in a dry-run
+        if self.output_options.thumbnail_name and (dry_run or entry.is_thumbnail_downloaded()):
             output_thumbnail_name = self.overrides.apply_formatter(
                 formatter=self.output_options.thumbnail_name, entry=entry
             )
 
-            # We always convert entry thumbnails to jpgs, and is performed here
-            if not dry_run:
-                convert_download_thumbnail(entry=entry)
-
             # Copy the thumbnails since they could be used later for other things
             self._enhanced_download_archive.save_file_to_output_directory(
                 file_name=entry.get_download_thumbnail_name(),
                 output_file_name=output_thumbnail_name,
                 entry=entry,
                 copy_file=True,
             )
+        elif not entry.is_thumbnail_downloaded():
+            logger.warning(
+                "Cannot save thumbnail for '%s' because it is not available", entry.title
+            )
 
         if self.output_options.info_json_name:
             output_info_json_name = self.overrides.apply_formatter(
                 formatter=self.output_options.info_json_name, entry=entry
             )
 
             # if not dry-run, write the info json
```

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.7.28/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.7.28/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.26.post2
+Version: 2023.7.28
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.26.post2/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.7.28/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

