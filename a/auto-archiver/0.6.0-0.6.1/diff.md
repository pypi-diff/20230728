# Comparing `tmp/auto_archiver-0.6.0.tar.gz` & `tmp/auto_archiver-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_archiver-0.6.0.tar", last modified: Thu Jul 27 14:46:00 2023, max compression
+gzip compressed data, was "auto_archiver-0.6.1.tar", last modified: Fri Jul 28 11:54:59 2023, max compression
```

## Comparing `auto_archiver-0.6.0.tar` & `auto_archiver-0.6.1.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.840499 auto_archiver-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-27 14:46:00.840499 auto_archiver-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-27 14:46:00.840499 auto_archiver-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.820499 auto_archiver-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.828498 auto_archiver-0.6.0/src/auto_archiver/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.832499 auto_archiver-0.6.0/src/auto_archiver/archivers/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/instagram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/instagram_tbot_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/telegram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/telethon_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/tiktok_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/twitter_api_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/twitter_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/vk_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/archivers/youtubedl_archiver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.832499 auto_archiver-0.6.0/src/auto_archiver/core/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.832499 auto_archiver-0.6.0/src/auto_archiver/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/databases/api_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/databases/console_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/databases/csv_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/databases/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/databases/gsheet_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.836499 auto_archiver-0.6.0/src/auto_archiver/enrichers/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/hash_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/pdq_hash_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/screenshot_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/thumbnail_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/wacz_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/wayback_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/enrichers/whisper_enricher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.836499 auto_archiver-0.6.0/src/auto_archiver/feeders/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/feeders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/feeders/cli_feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/feeders/feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/feeders/gsheet_feeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.836499 auto_archiver-0.6.0/src/auto_archiver/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/html_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/mute_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.836499 auto_archiver-0.6.0/src/auto_archiver/formatters/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/templates/html_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/formatters/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.840499 auto_archiver-0.6.0/src/auto_archiver/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/storages/gd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/storages/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/storages/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/storages/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.840499 auto_archiver-0.6.0/src/auto_archiver/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/utils/gsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/utils/gworksheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/utils/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-27 14:43:17.000000 auto_archiver-0.6.0/src/auto_archiver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:46:00.832499 auto_archiver-0.6.0/src/auto_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 14:46:00.000000 auto_archiver-0.6.0/src/auto_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.501509 auto_archiver-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.501509 auto_archiver-0.6.1/src/auto_archiver/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.505509 auto_archiver-0.6.1/src/auto_archiver/archivers/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/instagram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/instagram_tbot_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/telegram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/telethon_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/tiktok_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/twitter_api_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/twitter_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/vk_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/youtubedl_archiver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.505509 auto_archiver-0.6.1/src/auto_archiver/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.505509 auto_archiver-0.6.1/src/auto_archiver/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/databases/api_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/databases/console_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/databases/csv_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/databases/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/databases/gsheet_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.505509 auto_archiver-0.6.1/src/auto_archiver/enrichers/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/hash_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/metadata_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/pdq_hash_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/screenshot_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/thumbnail_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/wacz_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/wayback_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/whisper_enricher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/src/auto_archiver/feeders/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/feeders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/feeders/cli_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/feeders/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/feeders/gsheet_feeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/src/auto_archiver/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/html_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/mute_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/src/auto_archiver/formatters/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/templates/html_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/src/auto_archiver/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/storages/gd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/storages/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/storages/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/storages/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/src/auto_archiver/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/utils/gsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/utils/gworksheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/utils/webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.501509 auto_archiver-0.6.1/src/auto_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/top_level.txt
```

### Comparing `auto_archiver-0.6.0/LICENSE` & `auto_archiver-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/PKG-INFO` & `auto_archiver-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_archiver
-Version: 0.6.0
+Version: 0.6.1
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.6.0/README.md` & `auto_archiver-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/setup.cfg` & `auto_archiver-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/archivers/archiver.py` & `auto_archiver-0.6.1/src/auto_archiver/archivers/archiver.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,19 +23,14 @@
         # used when archivers need to login or do other one-time setup
         pass
 
     def sanitize_url(self, url: str) -> str:
         # used to clean unnecessary URL parameters OR unfurl redirect links
         return url
 
-    def is_rearchivable(self, url: str) -> bool:
-        # archivers can signal if it does not make sense to rearchive a piece of content
-        # default is rearchiving
-        return True
-
     def _guess_file_type(self, path: str) -> str:
         """
         Receives a URL or filename and returns global mimetype like 'image' or 'video'
         see https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types/Common_types
         """
         mime = mimetypes.guess_type(path)[0]
         if mime is not None:
@@ -52,13 +47,14 @@
                 to_filename = to_filename[-64:]
         if item:
             to_filename = os.path.join(ArchivingContext.get_tmp_dir(), to_filename)
         headers = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.138 Safari/537.36'
         }
         d = requests.get(url, headers=headers)
+        assert d.status_code == 200, f"got response code {d.status_code} for {url=}"
         with open(to_filename, 'wb') as f:
             f.write(d.content)
         return to_filename
 
     @abstractmethod
     def download(self, item: Metadata) -> Metadata: pass
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/archivers/instagram_archiver.py` & `auto_archiver-0.6.1/src/auto_archiver/archivers/instagram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/archivers/instagram_tbot_archiver.py` & `auto_archiver-0.6.1/src/auto_archiver/archivers/instagram_tbot_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/archivers/telegram_archiver.py` & `auto_archiver-0.6.1/src/auto_archiver/archivers/telegram_archiver.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,14 @@
     def __init__(self, config: dict) -> None:
         super().__init__(config)
 
     @staticmethod
     def configs() -> dict:
         return {}
 
-    def is_rearchivable(self, url: str) -> bool:
-        # telegram posts are static
-        return False
-
     def download(self, item: Metadata) -> Metadata:
         url = item.get_url()
         # detect URLs that we definitely cannot handle
         if 't.me' != item.netloc:
             return False
 
         headers = {
@@ -53,18 +49,18 @@
             image_urls = []
             for im in image_tags:
                 urls = [u.replace("'", "") for u in re.findall(r'url\((.*?)\)', im['style'])]
                 image_urls += urls
 
             if not len(image_urls): return False
             for img_url in image_urls:
-                result.add_media(Media(self.download_from_url(img_url)))
+                result.add_media(Media(self.download_from_url(img_url, item=item)))
         else:
             video_url = video.get('src')
-            m_video = Media(self.download_from_url(video_url))
+            m_video = Media(self.download_from_url(video_url, item=item))
             # extract duration from HTML
             try:
                 duration = s.find_all('time')[0].contents[0]
                 if ':' in duration:
                     duration = float(duration.split(
                         ':')[0]) * 60 + float(duration.split(':')[1])
                 else:
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/archivers/telethon_archiver.py` & `auto_archiver-0.6.1/src/auto_archiver/archivers/telethon_archiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,14 @@
             "channel_invites": {
                 "default": {},
                 "help": "(JSON string) private channel invite links (format: t.me/joinchat/HASH OR t.me/+HASH) and (optional but important to avoid hanging for minutes on startup) channel id (format: CHANNEL_ID taken from a post url like https://t.me/c/CHANNEL_ID/1), the telegram account will join any new channels on setup",
                 "cli_set": lambda cli_val, cur_val: dict(cur_val, **json.loads(cli_val))
             }
         }
 
-    def is_rearchivable(self, url: str) -> bool:
-        # telegram posts are static
-        return False
-
     def setup(self) -> None:
         """
         1. trigger login process for telegram or proceed if already saved in a session file
         2. joins channel_invites where needed
         """
         logger.info(f"SETUP {self.name} checking login...")
         with self.client.start():
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/archivers/tiktok_archiver.py` & `auto_archiver-0.6.1/src/auto_archiver/archivers/tiktok_archiver.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,14 @@
     def __init__(self, config: dict) -> None:
         super().__init__(config)
 
     @staticmethod
     def configs() -> dict:
         return {}
 
-    def is_rearchivable(self, url: str) -> bool:
-        # TikTok posts are static
-        return False
-
     def download(self, item: Metadata) -> Metadata:
         url = item.get_url()
         if 'tiktok.com' not in url:
             return False
 
         result = Metadata()
         try:
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/archivers/twitter_api_archiver.py` & `auto_archiver-0.6.1/src/auto_archiver/archivers/twitter_api_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/archivers/twitter_archiver.py` & `auto_archiver-0.6.1/src/auto_archiver/archivers/twitter_archiver.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,18 +33,14 @@
                 logger.debug(f'Expanded url {url} to {r.url}')
                 url = r.url
             except:
                 logger.error(f'Failed to expand url {url}')
         # https://twitter.com/MeCookieMonster/status/1617921633456640001?s=20&t=3d0g4ZQis7dCbSDg-mE7-w
         return self.link_clean_pattern.sub("\\1", url)
 
-    def is_rearchivable(self, url: str) -> bool:
-        # Twitter posts are static (for now)
-        return False
-
     def download(self, item: Metadata) -> Metadata:
         """
         if this url is archivable will download post info and look for other posts from the same group with media.
         can handle private/public channels
         """
         url = item.get_url()
         # detect URLs that we definitely cannot handle
@@ -74,15 +70,15 @@
                 media.set("src", variant.url).set("duration", tweet_media.duration)
                 mimetype = variant.contentType
             elif type(tweet_media) == Gif:
                 variant = tweet_media.variants[0]
                 media.set("src", variant.url)
                 mimetype = variant.contentType
             elif type(tweet_media) == Photo:
-                media.set("src", tweet_media.fullUrl.replace('name=large', 'name=orig').replace('name=small', 'name=orig'))
+                media.set("src", UrlUtil.twitter_best_quality_url(tweet_media.fullUrl))
                 mimetype = "image/jpeg"
             else:
                 logger.warning(f"Could not get media URL of {tweet_media}")
                 continue
             ext = mimetypes.guess_extension(mimetype)
             media.filename = self.download_from_url(media.get("src"), f'{slugify(url)}_{i}{ext}', item)
             result.add_media(media)
@@ -114,14 +110,15 @@
             v = tweet["video"]
             urls.append(self.choose_variant(v.get("variants", [])))
 
         logger.debug(f"Twitter hack got {urls=}")
 
         for i, u in enumerate(urls):
             media = Media(filename="")
+            u = UrlUtil.twitter_best_quality_url(u)
             media.set("src", u)
             ext = ""
             if (mtype := mimetypes.guess_type(UrlUtil.remove_get_parameters(u))[0]):
                 ext = mimetypes.guess_extension(mtype)
 
             media.filename = self.download_from_url(u, f'{slugify(url)}_{i}{ext}', item)
             result.add_media(media)
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/archivers/vk_archiver.py` & `auto_archiver-0.6.1/src/auto_archiver/archivers/vk_archiver.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,18 +23,14 @@
     def configs() -> dict:
         return {
             "username": {"default": None, "help": "valid VKontakte username"},
             "password": {"default": None, "help": "valid VKontakte password"},
             "session_file": {"default": "secrets/vk_config.v2.json", "help": "valid VKontakte password"},
         }
 
-    def is_rearchivable(self, url: str) -> bool:
-        # VK content is static
-        return False
-
     def download(self, item: Metadata) -> Metadata:
         url = item.get_url()
 
         if "vk.com" not in item.netloc: return False
 
         # some urls can contain multiple wall/photo/... parts and all will be fetched
         vk_scrapes = self.vks.scrape(url)
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/archivers/youtubedl_archiver.py` & `auto_archiver-0.6.1/src/auto_archiver/archivers/youtubedl_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/core/config.py` & `auto_archiver-0.6.1/src/auto_archiver/core/config.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/core/context.py` & `auto_archiver-0.6.1/src/auto_archiver/core/context.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/core/media.py` & `auto_archiver-0.6.1/src/auto_archiver/core/media.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 
 from __future__ import annotations
+import os
+import traceback
 from typing import Any, List
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 import mimetypes
 
+import ffmpeg
+from ffmpeg._run import Error
+
 from .context import ArchivingContext
 
 from loguru import logger
 
 
 @dataclass_json  # annotation order matters
 @dataclass
@@ -70,10 +75,27 @@
         self._mimetype = v
 
     def is_video(self) -> bool:
         return self.mimetype.startswith("video")
 
     def is_audio(self) -> bool:
         return self.mimetype.startswith("audio")
-    
+
     def is_image(self) -> bool:
         return self.mimetype.startswith("image")
+
+    def is_valid_video(self) -> bool:
+        # checks for video streams with ffmpeg, or min file size for a video
+        # self.is_video() should be used together with this method
+        try:
+            streams = ffmpeg.probe(self.filename, select_streams='v')['streams']
+            logger.warning(f"STREAMS FOR {self.filename} {streams}")
+            return any(s.get("duration_ts") > 0 for s in streams)
+        except Error: return False # ffmpeg errors when reading bad files
+        except Exception as e:
+            logger.error(e)
+            logger.error(traceback.format_exc())
+            try:
+                fsize = os.path.getsize(self.filename)
+                return fsize > 20_000
+            except: pass
+        return True
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/core/metadata.py` & `auto_archiver-0.6.1/src/auto_archiver/core/metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 from __future__ import annotations
+import hashlib
 from typing import Any, List, Union, Dict
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 import datetime
 from urllib.parse import urlparse
 from dateutil.parser import parse as parse_dt
 from .media import Media
@@ -12,42 +13,41 @@
 
 @dataclass_json  # annotation order matters
 @dataclass
 class Metadata:
     status: str = "no archiver"
     metadata: Dict[str, Any] = field(default_factory=dict)
     media: List[Media] = field(default_factory=list)
-    rearchivable: bool = True  # defaults to true, archivers can overwrite
 
     def __post_init__(self):
         self.set("_processed_at", datetime.datetime.utcnow())
 
     def merge(self: Metadata, right: Metadata, overwrite_left=True) -> Metadata:
         """
         merges two Metadata instances, will overwrite according to overwrite_left flag
         """
         if not right: return self
         if overwrite_left:
             if right.status and len(right.status):
                 self.status = right.status
-            self.rearchivable |= right.rearchivable
             for k, v in right.metadata.items():
                 assert k not in self.metadata or type(v) == type(self.get(k))
                 if type(v) not in [dict, list, set] or k not in self.metadata:
                     self.set(k, v)
                 else:  # key conflict
                     if type(v) in [dict, set]: self.set(k, self.get(k) | v)
                     elif type(v) == list: self.set(k, self.get(k) + v)
             self.media.extend(right.media)
         else:  # invert and do same logic
             return right.merge(self)
         return self
 
     def store(self: Metadata, override_storages: List = None):
         # calls .store for all contained media. storages [Storage]
+        self.remove_duplicate_media_by_hash()
         storages = override_storages or ArchivingContext.get("storages")
         for media in self.media:
             media.store(override_storages=storages, url=self.get_url())
 
     def set(self, key: str, val: Any) -> Metadata:
         self.metadata[key] = val
         return self
@@ -120,26 +120,47 @@
         return media
 
     def get_media_by_id(self, id: str, default=None) -> Media:
         for m in self.media:
             if m.get("id") == id: return m
         return default
 
+    def remove_duplicate_media_by_hash(self) -> None:
+        # iterates all media, calculates a hash if it's missing and deletes duplicates
+        def calculate_hash_in_chunks(hash_algo, chunksize, filename) -> str:
+            # taken from hash_enricher, cannot be isolated to misc due to circular imports
+            with open(filename, "rb") as f:
+                while True:
+                    buf = f.read(chunksize)
+                    if not buf: break
+                    hash_algo.update(buf)
+            return hash_algo.hexdigest()
+
+        media_hashes = set()
+        new_media = []
+        for m in self.media:
+            h = m.get("hash")
+            if not h: h = calculate_hash_in_chunks(hashlib.sha256(), 1.6e7, m.filename)
+            if len(h) and h in media_hashes: continue
+            media_hashes.add(h)
+            new_media.append(m)
+        self.media = new_media
+
     def get_first_image(self, default=None) -> Media:
         for m in self.media:
             if "image" in m.mimetype: return m
         return default
 
     def set_final_media(self, final: Media) -> Metadata:
         """final media is a special type of media: if you can show only 1 this is it, it's useful for some DBs like GsheetDb"""
         self.add_media(final, "_final_media")
 
     def get_final_media(self) -> Media:
         _default = self.media[0] if len(self.media) else None
         return self.get_media_by_id("_final_media", _default)
-    
+
     def get_all_media(self) -> List[Media]:
         # returns a list with all the media and inner media
         return [inner for m in self.media for inner in m.all_inner_media(True)]
 
     def __str__(self) -> str:
         return self.__repr__()
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/core/orchestrator.py` & `auto_archiver-0.6.1/src/auto_archiver/core/orchestrator.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,31 +58,27 @@
         # 1 - cleanup
         # each archiver is responsible for cleaning/expanding its own URLs
         url = original_url
         for a in self.archivers: url = a.sanitize_url(url)
         result.set_url(url)
         if original_url != url: result.set("original_url", original_url)
 
-        # 2 - rearchiving logic + notify start to DB
-        # archivers can signal whether the content is rearchivable: eg: tweet vs webpage
-        for a in self.archivers: result.rearchivable |= a.is_rearchivable(url)
-        logger.debug(f"{result.rearchivable=} for {url=}")
-
+        # 2 - notify start to DB
         # signal to DB that archiving has started
         # and propagate already archived if it exists
         cached_result = None
         for d in self.databases:
             # are the databases to decide whether to archive?
             # they can simply return True by default, otherwise they can avoid duplicates. should this logic be more granular, for example on the archiver level: a tweet will not need be scraped twice, whereas an instagram profile might. the archiver could not decide from the link which parts to archive,
             # instagram profile example: it would always re-archive everything
             # maybe the database/storage could use a hash/key to decide if there's a need to re-archive
             d.started(result)
             if (local_result := d.fetch(result)):
                 cached_result = (cached_result or Metadata()).merge(local_result)
-        if cached_result and not cached_result.rearchivable:
+        if cached_result:
             logger.debug("Found previously archived entry")
             for d in self.databases:
                 d.done(cached_result)
             return cached_result
 
         # 3 - call archivers until one succeeds
         for a in self.archivers:
@@ -105,15 +101,14 @@
             try: e.enrich(result)
             except Exception as exc: logger.error(f"Unexpected error with enricher {e.name}: {exc}: {traceback.format_exc()}")
 
         # 5 - store media
         # looks for Media in result.media and also result.media[x].properties (as list or dict values)
         result.store()
 
-        #TODO: remove any duplicate media, if hash is available
 
         # 6 - format and store formatted if needed
         # enrichers typically need access to already stored URLs etc
         if (final_media := self.formatter.format(result)):
             final_media.store(url=url)
             result.set_final_media(final_media)
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/core/step.py` & `auto_archiver-0.6.1/src/auto_archiver/core/step.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from inspect import ClassFoundException
 from typing import Type
 from abc import ABC
-# from collections.abc import Iterable
 
 
 @dataclass
 class Step(ABC):
     name: str = None
 
     def __init__(self, config: dict) -> None:
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/databases/api_db.py` & `auto_archiver-0.6.1/src/auto_archiver/databases/api_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/databases/console_db.py` & `auto_archiver-0.6.1/src/auto_archiver/databases/console_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/databases/csv_db.py` & `auto_archiver-0.6.1/src/auto_archiver/databases/csv_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/databases/database.py` & `auto_archiver-0.6.1/src/auto_archiver/databases/database.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/databases/gsheet_db.py` & `auto_archiver-0.6.1/src/auto_archiver/databases/gsheet_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/enrichers/enricher.py` & `auto_archiver-0.6.1/src/auto_archiver/enrichers/enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/enrichers/hash_enricher.py` & `auto_archiver-0.6.1/src/auto_archiver/enrichers/hash_enricher.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         url = to_enrich.get_url()
         logger.debug(f"calculating media hashes for {url=} (using {self.algorithm})")
 
         for i, m in enumerate(to_enrich.media):
             if len(hd := self.calculate_hash(m.filename)):
                 to_enrich.media[i].set("hash", f"{self.algorithm}:{hd}")
 
-    def calculate_hash(self, filename):
+    def calculate_hash(self, filename) -> str:
         hash = None
         if self.algorithm == "SHA-256":
             hash = hashlib.sha256()
         elif self.algorithm == "SHA3-512":
             hash = hashlib.sha3_512()
         else: return ""
         with open(filename, "rb") as f:
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/enrichers/pdq_hash_enricher.py` & `auto_archiver-0.6.1/src/auto_archiver/enrichers/pdq_hash_enricher.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 
     def enrich(self, to_enrich: Metadata) -> None:
         url = to_enrich.get_url()
         logger.debug(f"calculating perceptual hashes for {url=}")
 
         for m in to_enrich.media:
             for media in m.all_inner_media(True):
-                if media.is_image() and media.get("id") != "screenshot" and len(hd := self.calculate_pdq_hash(media.filename)):
-                        media.set("pdq_hash", hd)    
+                if media.is_image() and "screenshot" not in media.get("id") and "warc-file-" not in media.get("id") and len(hd := self.calculate_pdq_hash(media.filename)):
+                    media.set("pdq_hash", hd)
 
     def calculate_pdq_hash(self, filename):
         # returns a hexadecimal string with the perceptual hash for the given filename
         try:
             with Image.open(filename) as img:
                 # convert the image to RGB
                 image_rgb = np.array(img.convert("RGB"))
                 # compute the 256-bit PDQ hash (we do not store the quality score)
                 hash_array, _ = pdqhash.compute(image_rgb)
                 hash = "".join(str(b) for b in hash_array)
                 return hex(int(hash, 2))[2:]
         except UnidentifiedImageError as e:
             logger.error(f"Image {filename=} is likely corrupted or in unsupported format {e}: {traceback.format_exc()}")
-        return ""
+        return ""
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/enrichers/screenshot_enricher.py` & `auto_archiver-0.6.1/src/auto_archiver/enrichers/screenshot_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/enrichers/thumbnail_enricher.py` & `auto_archiver-0.6.1/src/auto_archiver/enrichers/thumbnail_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/enrichers/wacz_enricher.py` & `auto_archiver-0.6.1/src/auto_archiver/enrichers/wacz_enricher.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,28 +40,28 @@
 
     def enrich(self, to_enrich: Metadata) -> bool:
         if to_enrich.get_media_by_id("browsertrix"):
             logger.info(f"WACZ enricher had already been executed: {to_enrich.get_media_by_id('browsertrix')}")
             return True
 
         url = to_enrich.get_url()
-        logger.warning(f"ENRICHING WACZ for {url=}")
 
         collection = str(uuid.uuid4())[0:8]
         browsertrix_home = os.path.abspath(ArchivingContext.get_tmp_dir())
 
         if os.getenv('RUNNING_IN_DOCKER'):
             logger.debug(f"generating WACZ without Docker for {url=}")
 
             cmd = [
                 "crawl",
                 "--url", url,
                 "--scopeType", "page",
                 "--generateWACZ",
                 "--text",
+                "--screenshot", "fullPage",
                 "--collection", collection,
                 "--id", collection,
                 "--saveState", "never",
                 "--behaviors", "autoscroll,autoplay,autofetch,siteSpecific",
                 "--behaviorTimeout", str(self.timeout),
                 "--timeout", str(self.timeout)]
 
@@ -76,14 +76,15 @@
                 "-v", f"{browsertrix_home}:/crawls/",
                 # "-it", # this leads to "the input device is not a TTY"
                 "webrecorder/browsertrix-crawler", "crawl",
                 "--url", url,
                 "--scopeType", "page",
                 "--generateWACZ",
                 "--text",
+                "--screenshot", "fullPage",
                 "--collection", collection,
                 "--behaviors", "autoscroll,autoplay,autofetch,siteSpecific",
                 "--behaviorTimeout", str(self.timeout),
                 "--timeout", str(self.timeout)
             ]
 
             if self.profile:
@@ -132,31 +133,57 @@
                 if filename.endswith('.gz'):
                     chunk_file = os.path.join(warc_dir, filename)
                     with open(chunk_file, 'rb') as infile:
                         shutil.copyfileobj(infile, outfile)
 
         # get media out of .warc
         counter = 0
+        seen_urls = set()
         with open(warc_filename, 'rb') as warc_stream:
             for record in ArchiveIterator(warc_stream):
                 # only include fetched resources
+                if record.rec_type == "resource":  # screenshots
+                    fn = os.path.join(tmp_dir, f"warc-file-{counter}.png")
+                    with open(fn, "wb") as outf: outf.write(record.raw_stream.read())
+                    m = Media(filename=fn)
+                    to_enrich.add_media(m, "browsertrix-screenshot")
+                    counter += 1
+
                 if record.rec_type != 'response': continue
                 record_url = record.rec_headers.get_header('WARC-Target-URI')
                 if not UrlUtil.is_relevant_url(record_url):
                     logger.debug(f"Skipping irrelevant URL {record_url} but it's still present in the WACZ.")
                     continue
+                if record_url in seen_urls:
+                    logger.debug(f"Skipping already seen URL {record_url}.")
+                    continue
 
                 # filter by media mimetypes
                 content_type = record.http_headers.get("Content-Type")
                 if not content_type: continue
                 if not any(x in content_type for x in ["video", "image", "audio"]): continue
 
                 # create local file and add media
                 ext = mimetypes.guess_extension(content_type)
-                fn = os.path.join(tmp_dir, f"warc-file-{counter}{ext}")
+                warc_fn = f"warc-file-{counter}{ext}"
+                fn = os.path.join(tmp_dir, warc_fn)
+
+                record_url_best_qual = UrlUtil.twitter_best_quality_url(record_url)
                 with open(fn, "wb") as outf: outf.write(record.raw_stream.read())
+
                 m = Media(filename=fn)
                 m.set("src", record_url)
-                # TODO URLUTIL to ignore known-recurring media like favicons, profile pictures, etc.
-                to_enrich.add_media(m, f"browsertrix-media-{counter}")
+                # if a link with better quality exists, try to download that
+                if record_url_best_qual != record_url:
+                    try:
+                        m.filename = self.download_from_url(record_url_best_qual, warc_fn, to_enrich)
+                        m.set("src", record_url_best_qual)
+                        m.set("src_alternative", record_url)
+                    except Exception as e: logger.warning(f"Unable to download best quality URL for {record_url=} got error {e}, using original in WARC.")
+
+                # remove bad videos
+                if m.is_video() and not m.is_valid_video(): continue
+                
+                to_enrich.add_media(m, warc_fn)
                 counter += 1
+                seen_urls.add(record_url)
         logger.info(f"WACZ extract_media finished, found {counter} relevant media file(s)")
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/enrichers/wayback_enricher.py` & `auto_archiver-0.6.1/src/auto_archiver/enrichers/wayback_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/enrichers/whisper_enricher.py` & `auto_archiver-0.6.1/src/auto_archiver/enrichers/whisper_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/feeders/cli_feeder.py` & `auto_archiver-0.6.1/src/auto_archiver/feeders/cli_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/feeders/feeder.py` & `auto_archiver-0.6.1/src/auto_archiver/feeders/feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/feeders/gsheet_feeder.py` & `auto_archiver-0.6.1/src/auto_archiver/feeders/gsheet_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/formatters/formatter.py` & `auto_archiver-0.6.1/src/auto_archiver/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/formatters/html_formatter.py` & `auto_archiver-0.6.1/src/auto_archiver/formatters/html_formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/formatters/templates/html_template.html` & `auto_archiver-0.6.1/src/auto_archiver/formatters/templates/html_template.html`

 * *Files 26% similar despite different names*

```diff
@@ -61,19 +61,20 @@
         video {
             filter: gray;
             -webkit-filter: grayscale(1);
             filter: grayscale(1);
         }
 
         /* Disable grayscale on hover */
-        img:hover,
+        /* img:hover,
         video:hover {
             -webkit-filter: grayscale(0);
             filter: none;
-        }
+        } */
+
 
         .collapsible {
             background-color: #777;
             color: white;
             cursor: pointer;
             padding: 5px;
             margin: 10px;
@@ -97,65 +98,76 @@
         }
     </style>
 </head>
 
 <body>
     <div id="notification"></div>
     <h2>Archived media for <a href="{{ url }}">{{ url }}</a></h2>
+    {% if title | string | length > 0 %}
     <p><b>title:</b> '<span class="copy">{{ title }}</span>'</p>
+    {% endif %}
     <h2 class="center">content {{ media | length }} item(s)</h2>
+    <form class="center">
+        <label>
+            <input type="checkbox" id="safe-media-view" checked>
+            Safe Media View
+        </label>
+    </form>
     <table class="content">
         <tr>
             <th>about</th>
             <th>preview(s)</th>
         </tr>
-        {% for m in media %}
-        <tr>
-            <td>
-                <ul>
-                    <li><b>key:</b> <span class="copy">{{ m.key }}</span></li>
-                    <li><b>type:</b> <span class="copy">{{ m.mimetype }}</span></li>
-
-                    {% for prop in m.properties %}
-
-                    {% if m.properties[prop] | is_list %}
-                    <p></p>
-                    <div>
-                        <b class="collapsible" title="expand">{{ prop }}:</b>
+        <tbody>
+            {% for m in media %}
+            <tr>
+                <td>
+                    <ul>
+                        <li><b>key:</b> <span class="copy">{{ m.key }}</span></li>
+                        <li><b>type:</b> <span class="copy">{{ m.mimetype }}</span></li>
+
+                        {% for prop in m.properties %}
+
+                        {% if m.properties[prop] | is_list %}
                         <p></p>
-                        <div class="collapsible-content">
-                            {% for subprop in m.properties[prop] %}
-                            {% if subprop | is_media %}
-                            {{ macros.display_media(subprop, true, url) }}
-
-                            <ul>
-                                {% for subprop_prop in subprop.properties %}
-                                <li><b>{{ subprop_prop }}:</b> {{ macros.copy_urlize(subprop.properties[subprop_prop]) }}</li>
+                        <div>
+                            <b class="collapsible" title="expand">{{ prop }}:</b>
+                            <p></p>
+                            <div class="collapsible-content">
+                                {% for subprop in m.properties[prop] %}
+                                {% if subprop | is_media %}
+                                {{ macros.display_media(subprop, true, url) }}
+
+                                <ul>
+                                    {% for subprop_prop in subprop.properties %}
+                                    <li><b>{{ subprop_prop }}:</b>
+                                        {{ macros.copy_urlize(subprop.properties[subprop_prop]) }}</li>
+                                    {% endfor %}
+                                </ul>
+
+                                {% else %}
+                                {{ subprop }}
+                                {% endif %}
                                 {% endfor %}
-                            </ul>
-
-                            {% else %}
-                            {{ subprop }}
-                            {% endif %}
-                            {% endfor %}
+                            </div>
                         </div>
-                    </div>
-                    <p></p>
-                    {% elif m.properties[prop] | string | length > 1 %}
-                    <li><b>{{ prop }}:</b> {{ macros.copy_urlize(m.properties[prop]) }}</li>
-                    {% endif %}
-
-                    {% endfor %}
-                </ul>
-            </td>
-            <td>
-                {{ macros.display_media(m, true, url) }}
-            </td>
-        </tr>
-        {% endfor %}
+                        <p></p>
+                        {% elif m.properties[prop] | string | length > 1 %}
+                        <li><b>{{ prop }}:</b> {{ macros.copy_urlize(m.properties[prop]) }}</li>
+                        {% endif %}
+
+                        {% endfor %}
+                    </ul>
+                </td>
+                <td>
+                    {{ macros.display_media(m, true, url) }}
+                </td>
+            </tr>
+            {% endfor %}
+        </tbody>
     </table>
     <h2 class="center">metadata</h2>
     <table class="metadata">
         <tr>
             <th>key</th>
             <th>value</th>
         </tr>
@@ -216,10 +228,53 @@
             if (content.style.display === "block") {
                 content.style.display = "none";
             } else {
                 content.style.display = "block";
             }
         });
     }
+
+    // logic for enabled/disabled greyscale
+    // Get references to the checkboxes and images/videos
+    const safeImageViewCheckbox = document.getElementById('safe-media-view');
+    const imagesVideos = document.querySelectorAll('img, video');
+
+    // Function to toggle grayscale effect
+    function toggleGrayscale() {
+        imagesVideos.forEach(element => {
+            if (safeImageViewCheckbox.checked) {
+                // Enable grayscale effect
+                element.style.filter = 'grayscale(1)';
+                element.style.webkitFilter = 'grayscale(1)';
+            } else {
+                // Disable grayscale effect
+                element.style.filter = 'none';
+                element.style.webkitFilter = 'none';
+            }
+        });
+    }
+
+    // Add event listener to the checkbox to trigger the toggleGrayscale function
+    safeImageViewCheckbox.addEventListener('change', toggleGrayscale);
+
+    // Handle the hover effect using JavaScript
+    imagesVideos.forEach(element => {
+        element.addEventListener('mouseenter', () => {
+            // Disable grayscale effect on hover
+            element.style.filter = 'none';
+            element.style.webkitFilter = 'none';
+        });
+
+        element.addEventListener('mouseleave', () => {
+            // Re-enable grayscale effect if checkbox is checked
+            if (safeImageViewCheckbox.checked) {
+                element.style.filter = 'grayscale(1)';
+                element.style.webkitFilter = 'grayscale(1)';
+            }
+        });
+    });
+
+    // Call the function on page load to apply the initial state
+    toggleGrayscale();
 </script>
 
 </html>
```

#### html2text {}

```diff
@@ -1,12 +1,15 @@
 {# templates/results.html #} {% import 'macros.html' as macros %}
 
 ***** Archived media for {{_url_}} *****
+{% if title | string | length > 0 %}
 title: '{{ title }}'
+{% endif %}
 ***** content {{ media | length }} item(s) *****
+ * Safe Media View
 about                                   preview(s)
     * key: {{ m.key }}
     * type: {{ m.mimetype }}
     * {% for prop in m.properties %} {%
       if m.properties[prop] | is_list
       %}
       {{ prop }}:
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/formatters/templates/macros.html` & `auto_archiver-0.6.1/src/auto_archiver/formatters/templates/macros.html`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,14 @@
     <div>
         Reverse Image Search:&nbsp;
         <a href="https://www.google.com/searchbyimage?sbisrc=4chanx&image_url={{ url | quote }}&safe=off">Google</a>,&nbsp;
         <a href="https://lens.google.com/uploadbyurl?url={{ url | quote }}">Google Lens</a>,&nbsp;
         <a href="https://yandex.ru/images/touch/search?rpt=imageview&url={{ url | quote }}">Yandex</a>,&nbsp;
         <a href="https://www.bing.com/images/search?view=detailv2&iss=sbi&form=SBIVSP&sbisrc=UrlPaste&q=imgurl:{{ url | quote }}">Bing</a>,&nbsp;
         <a href="https://www.tineye.com/search/?url={{ url | quote }}">Tineye</a>,&nbsp;
-        <a href="https://iqdb.org/?url={{ url | quote }}">IQDB</a>,&nbsp;
-        <a href="https://saucenao.com/search.php?db=999&url={{ url | quote }}">SauceNAO</a>,&nbsp;
-        <a href="https://imgops.com/{{ url | quote }}">IMGOPS</a>
     </div>
     <p></p>
 </div>
 {% elif 'video' in m.mimetype %}
 <div>
     <video src="{{ url }}" controls style="max-height:400px;max-width:600px;">
         Your browser does not support the video element.
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
 {% macro display_media(m, links, main_url) -%} {% for url in m.urls %} {% if
 url | length == 0 %} No URL available for {{ m.key }}. {% elif 'http' in url %}
 {% if 'image' in m.mimetype %}
 [{{_url_}}]
-Reverse Image Search:  Google,  Google_Lens,  Yandex,  Bing,  Tineye,  IQDB, 
-SauceNAO,  IMGOPS
+Reverse Image Search:  Google,  Google_Lens,  Yandex,  Bing,  Tineye, 
 {% elif 'video' in m.mimetype %}
  Your browser does not support the video element.
 {% elif 'audio' in m.mimetype %}
   Your browser does not support the audio element.
 {% elif m.filename | get_extension == ".wacz" %} replayweb {% else %} No
 preview available for {{ m.key }}. {% endif %} {% else %} {{ m.url | urlize }}
 {% endif %} {% if links %} open or download or {{ copy_urlize(url, "copy") }}
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/storages/gd.py` & `auto_archiver-0.6.1/src/auto_archiver/storages/gd.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/storages/local.py` & `auto_archiver-0.6.1/src/auto_archiver/storages/local.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/storages/s3.py` & `auto_archiver-0.6.1/src/auto_archiver/storages/s3.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/storages/storage.py` & `auto_archiver-0.6.1/src/auto_archiver/storages/storage.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/utils/gsheet.py` & `auto_archiver-0.6.1/src/auto_archiver/utils/gsheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/utils/gworksheet.py` & `auto_archiver-0.6.1/src/auto_archiver/utils/gworksheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver/utils/misc.py` & `auto_archiver-0.6.1/src/auto_archiver/utils/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
             r = requests.get(url)
             logger.debug(f'Expanded url {url} to {r.url}')
             return r.url
         except:
             logger.error(f'Failed to expand url {url}')
     return url
 
+
 def getattr_or(o: object, prop: str, default=None):
     try:
         res = getattr(o, prop)
         if res is None: raise
         return res
     except:
         return default
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/utils/url.py` & `auto_archiver-0.6.1/src/auto_archiver/utils/url.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 from urllib.parse import urlparse, urlunparse
 
-
 class UrlUtil:
     telegram_private = re.compile(r"https:\/\/t\.me(\/c)\/(.+)\/(\d+)")
     is_istagram = re.compile(r"https:\/\/www\.instagram\.com")
 
     @staticmethod
     def clean(url: str) -> str: return url
 
@@ -39,8 +38,23 @@
         # ifnore icons
         if clean_url.endswith(".ico"): return False
         # ignore SVGs
         if UrlUtil.remove_get_parameters(url).endswith(".svg"): return False
 
         # twitter profile pictures
         if "twimg.com/profile_images" in url: return False
+        if "twimg.com" in url and "/default_profile_images" in url: return False
+
+        # instagram profile pictures
+        if "https://scontent.cdninstagram.com/" in url and "150x150" in url: return False
+        # instagram recurring images
+        if "https://static.cdninstagram.com/rsrc.php/" in url: return False
+
         return True
+
+    @staticmethod
+    def twitter_best_quality_url(url: str) -> str:
+        """
+        some twitter image URLs point to a less-than best quality
+        this returns the URL pointing to the highest (original) quality
+        """
+        return re.sub(r"name=(\w+)", "name=orig", url, 1)
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver/utils/webdriver.py` & `auto_archiver-0.6.1/src/auto_archiver/utils/webdriver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.0/src/auto_archiver.egg-info/PKG-INFO` & `auto_archiver-0.6.1/src/auto_archiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-archiver
-Version: 0.6.0
+Version: 0.6.1
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.6.0/src/auto_archiver.egg-info/SOURCES.txt` & `auto_archiver-0.6.1/src/auto_archiver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 src/auto_archiver/databases/console_db.py
 src/auto_archiver/databases/csv_db.py
 src/auto_archiver/databases/database.py
 src/auto_archiver/databases/gsheet_db.py
 src/auto_archiver/enrichers/__init__.py
 src/auto_archiver/enrichers/enricher.py
 src/auto_archiver/enrichers/hash_enricher.py
+src/auto_archiver/enrichers/metadata_enricher.py
 src/auto_archiver/enrichers/pdq_hash_enricher.py
 src/auto_archiver/enrichers/screenshot_enricher.py
 src/auto_archiver/enrichers/thumbnail_enricher.py
 src/auto_archiver/enrichers/wacz_enricher.py
 src/auto_archiver/enrichers/wayback_enricher.py
 src/auto_archiver/enrichers/whisper_enricher.py
 src/auto_archiver/feeders/__init__.py
```

