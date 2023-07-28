# Comparing `tmp/auto_archiver-0.6.1.tar.gz` & `tmp/auto_archiver-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_archiver-0.6.1.tar", last modified: Fri Jul 28 11:54:59 2023, max compression
+gzip compressed data, was "auto_archiver-0.6.2.tar", last modified: Fri Jul 28 12:13:39 2023, max compression
```

## Comparing `auto_archiver-0.6.1.tar` & `auto_archiver-0.6.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.501509 auto_archiver-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.501509 auto_archiver-0.6.1/src/auto_archiver/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.505509 auto_archiver-0.6.1/src/auto_archiver/archivers/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/instagram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/instagram_tbot_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/telegram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/telethon_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/tiktok_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/twitter_api_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/twitter_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/vk_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/archivers/youtubedl_archiver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.505509 auto_archiver-0.6.1/src/auto_archiver/core/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.505509 auto_archiver-0.6.1/src/auto_archiver/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/databases/api_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/databases/console_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/databases/csv_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/databases/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/databases/gsheet_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.505509 auto_archiver-0.6.1/src/auto_archiver/enrichers/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/hash_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/metadata_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/pdq_hash_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/screenshot_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/thumbnail_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/wacz_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/wayback_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/enrichers/whisper_enricher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/src/auto_archiver/feeders/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/feeders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/feeders/cli_feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/feeders/feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/feeders/gsheet_feeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/src/auto_archiver/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/html_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/mute_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/src/auto_archiver/formatters/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/templates/html_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/formatters/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/src/auto_archiver/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/storages/gd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/storages/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/storages/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/storages/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.509509 auto_archiver-0.6.1/src/auto_archiver/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/utils/gsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/utils/gworksheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/utils/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-28 11:52:25.000000 auto_archiver-0.6.1/src/auto_archiver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:54:59.501509 auto_archiver-0.6.1/src/auto_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 11:54:59.000000 auto_archiver-0.6.1/src/auto_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.356216 auto_archiver-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.356216 auto_archiver-0.6.2/src/auto_archiver/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.360216 auto_archiver-0.6.2/src/auto_archiver/archivers/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/instagram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/instagram_tbot_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/telegram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/telethon_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/tiktok_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/twitter_api_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/twitter_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/vk_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/archivers/youtubedl_archiver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.360216 auto_archiver-0.6.2/src/auto_archiver/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.360216 auto_archiver-0.6.2/src/auto_archiver/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/databases/api_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/databases/console_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/databases/csv_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/databases/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/databases/gsheet_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.360216 auto_archiver-0.6.2/src/auto_archiver/enrichers/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/hash_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/metadata_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/pdq_hash_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/screenshot_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/thumbnail_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/wacz_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/wayback_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/enrichers/whisper_enricher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/src/auto_archiver/feeders/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/feeders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/feeders/cli_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/feeders/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/feeders/gsheet_feeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/src/auto_archiver/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/html_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/mute_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/src/auto_archiver/formatters/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/templates/html_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/formatters/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/src/auto_archiver/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/storages/gd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/storages/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/storages/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/storages/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.364216 auto_archiver-0.6.2/src/auto_archiver/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/utils/gsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/utils/gworksheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/utils/webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-28 12:11:02.000000 auto_archiver-0.6.2/src/auto_archiver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:13:39.356216 auto_archiver-0.6.2/src/auto_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 12:13:39.000000 auto_archiver-0.6.2/src/auto_archiver.egg-info/top_level.txt
```

### Comparing `auto_archiver-0.6.1/LICENSE` & `auto_archiver-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/PKG-INFO` & `auto_archiver-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_archiver
-Version: 0.6.1
+Version: 0.6.2
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.6.1/README.md` & `auto_archiver-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/setup.cfg` & `auto_archiver-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/archivers/archiver.py` & `auto_archiver-0.6.2/src/auto_archiver/archivers/archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/archivers/instagram_archiver.py` & `auto_archiver-0.6.2/src/auto_archiver/archivers/instagram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/archivers/instagram_tbot_archiver.py` & `auto_archiver-0.6.2/src/auto_archiver/archivers/instagram_tbot_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/archivers/telegram_archiver.py` & `auto_archiver-0.6.2/src/auto_archiver/archivers/telegram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/archivers/telethon_archiver.py` & `auto_archiver-0.6.2/src/auto_archiver/archivers/telethon_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/archivers/tiktok_archiver.py` & `auto_archiver-0.6.2/src/auto_archiver/archivers/tiktok_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/archivers/twitter_api_archiver.py` & `auto_archiver-0.6.2/src/auto_archiver/archivers/twitter_api_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/archivers/twitter_archiver.py` & `auto_archiver-0.6.2/src/auto_archiver/archivers/twitter_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/archivers/vk_archiver.py` & `auto_archiver-0.6.2/src/auto_archiver/archivers/vk_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/archivers/youtubedl_archiver.py` & `auto_archiver-0.6.2/src/auto_archiver/archivers/youtubedl_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/core/config.py` & `auto_archiver-0.6.2/src/auto_archiver/core/config.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/core/context.py` & `auto_archiver-0.6.2/src/auto_archiver/core/context.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/core/media.py` & `auto_archiver-0.6.2/src/auto_archiver/core/media.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/core/metadata.py` & `auto_archiver-0.6.2/src/auto_archiver/core/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
                     hash_algo.update(buf)
             return hash_algo.hexdigest()
 
         media_hashes = set()
         new_media = []
         for m in self.media:
             h = m.get("hash")
-            if not h: h = calculate_hash_in_chunks(hashlib.sha256(), 1.6e7, m.filename)
+            if not h: h = calculate_hash_in_chunks(hashlib.sha256(), int(1.6e7), m.filename)
             if len(h) and h in media_hashes: continue
             media_hashes.add(h)
             new_media.append(m)
         self.media = new_media
 
     def get_first_image(self, default=None) -> Media:
         for m in self.media:
```

### Comparing `auto_archiver-0.6.1/src/auto_archiver/core/orchestrator.py` & `auto_archiver-0.6.2/src/auto_archiver/core/orchestrator.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/core/step.py` & `auto_archiver-0.6.2/src/auto_archiver/core/step.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/databases/api_db.py` & `auto_archiver-0.6.2/src/auto_archiver/databases/api_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/databases/console_db.py` & `auto_archiver-0.6.2/src/auto_archiver/databases/console_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/databases/csv_db.py` & `auto_archiver-0.6.2/src/auto_archiver/databases/csv_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/databases/database.py` & `auto_archiver-0.6.2/src/auto_archiver/databases/database.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/databases/gsheet_db.py` & `auto_archiver-0.6.2/src/auto_archiver/databases/gsheet_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/enrichers/enricher.py` & `auto_archiver-0.6.2/src/auto_archiver/enrichers/enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/enrichers/hash_enricher.py` & `auto_archiver-0.6.2/src/auto_archiver/enrichers/hash_enricher.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.chunksize = int(self.chunksize)
         ArchivingContext.set("hash_enricher.algorithm", self.algorithm, keep_on_reset=True)
 
     @staticmethod
     def configs() -> dict:
         return {
             "algorithm": {"default": "SHA-256", "help": "hash algorithm to use", "choices": ["SHA-256", "SHA3-512"]},
-            "chunksize": {"default": 1.6e7, "help": "number of bytes to use when reading files in chunks (if this value is too large you will run out of RAM), default is 16MB"},
+            "chunksize": {"default": int(1.6e7), "help": "number of bytes to use when reading files in chunks (if this value is too large you will run out of RAM), default is 16MB"},
         }
 
     def enrich(self, to_enrich: Metadata) -> None:
         url = to_enrich.get_url()
         logger.debug(f"calculating media hashes for {url=} (using {self.algorithm})")
 
         for i, m in enumerate(to_enrich.media):
```

### Comparing `auto_archiver-0.6.1/src/auto_archiver/enrichers/metadata_enricher.py` & `auto_archiver-0.6.2/src/auto_archiver/enrichers/metadata_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/enrichers/pdq_hash_enricher.py` & `auto_archiver-0.6.2/src/auto_archiver/enrichers/pdq_hash_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/enrichers/screenshot_enricher.py` & `auto_archiver-0.6.2/src/auto_archiver/enrichers/screenshot_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/enrichers/thumbnail_enricher.py` & `auto_archiver-0.6.2/src/auto_archiver/enrichers/thumbnail_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/enrichers/wacz_enricher.py` & `auto_archiver-0.6.2/src/auto_archiver/enrichers/wacz_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/enrichers/wayback_enricher.py` & `auto_archiver-0.6.2/src/auto_archiver/enrichers/wayback_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/enrichers/whisper_enricher.py` & `auto_archiver-0.6.2/src/auto_archiver/enrichers/whisper_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/feeders/cli_feeder.py` & `auto_archiver-0.6.2/src/auto_archiver/feeders/cli_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/feeders/feeder.py` & `auto_archiver-0.6.2/src/auto_archiver/feeders/feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/feeders/gsheet_feeder.py` & `auto_archiver-0.6.2/src/auto_archiver/feeders/gsheet_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/formatters/formatter.py` & `auto_archiver-0.6.2/src/auto_archiver/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/formatters/html_formatter.py` & `auto_archiver-0.6.2/src/auto_archiver/formatters/html_formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/formatters/templates/html_template.html` & `auto_archiver-0.6.2/src/auto_archiver/formatters/templates/html_template.html`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/formatters/templates/macros.html` & `auto_archiver-0.6.2/src/auto_archiver/formatters/templates/macros.html`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/storages/gd.py` & `auto_archiver-0.6.2/src/auto_archiver/storages/gd.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/storages/local.py` & `auto_archiver-0.6.2/src/auto_archiver/storages/local.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/storages/s3.py` & `auto_archiver-0.6.2/src/auto_archiver/storages/s3.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/storages/storage.py` & `auto_archiver-0.6.2/src/auto_archiver/storages/storage.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/utils/gsheet.py` & `auto_archiver-0.6.2/src/auto_archiver/utils/gsheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/utils/gworksheet.py` & `auto_archiver-0.6.2/src/auto_archiver/utils/gworksheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/utils/misc.py` & `auto_archiver-0.6.2/src/auto_archiver/utils/misc.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver/utils/url.py` & `auto_archiver-0.6.2/src/auto_archiver/utils/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,17 @@
         if "twimg.com" in url and "/default_profile_images" in url: return False
 
         # instagram profile pictures
         if "https://scontent.cdninstagram.com/" in url and "150x150" in url: return False
         # instagram recurring images
         if "https://static.cdninstagram.com/rsrc.php/" in url: return False
 
+        # telegram
+        if "https://telegram.org/img/emoji/" in url: return False
+
         return True
 
     @staticmethod
     def twitter_best_quality_url(url: str) -> str:
         """
         some twitter image URLs point to a less-than best quality
         this returns the URL pointing to the highest (original) quality
```

### Comparing `auto_archiver-0.6.1/src/auto_archiver/utils/webdriver.py` & `auto_archiver-0.6.2/src/auto_archiver/utils/webdriver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.6.1/src/auto_archiver.egg-info/PKG-INFO` & `auto_archiver-0.6.2/src/auto_archiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-archiver
-Version: 0.6.1
+Version: 0.6.2
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.6.1/src/auto_archiver.egg-info/SOURCES.txt` & `auto_archiver-0.6.2/src/auto_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

