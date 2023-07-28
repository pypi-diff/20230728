# Comparing `tmp/il-supermarket-scraper-0.2.9.tar.gz` & `tmp/il-supermarket-scraper-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "il-supermarket-scraper-0.2.9.tar", last modified: Mon May 15 11:54:38 2023, max compression
+gzip compressed data, was "il-supermarket-scraper-0.3.tar", last modified: Fri Jul 28 07:10:17 2023, max compression
```

## Comparing `il-supermarket-scraper-0.2.9.tar` & `il-supermarket-scraper-0.3.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:54:38.737460 il-supermarket-scraper-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-15 11:54:38.737460 il-supermarket-scraper-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:54:38.729460 il-supermarket-scraper-0.2.9/il_supermarket_scarper/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:54:38.729460 il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/apsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/bina.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/cerberus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/multipage_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/publishprice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrapper_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:54:38.733460 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/bareket.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/bitan.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/cofix.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/doralon.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/good_pharm.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/hazihinam.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/keshet.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/king_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/maayan2000.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/machsani_ashuk.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/mega.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/mega_market.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/nativ_hashed.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/osherad.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/polizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/ramilevy.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/salachdabach.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/shefa_barcart_ashem.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/shufersal.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/shuk_ahir.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/stop_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/super_pharm.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/super_yuda.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/superdosh.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/tivtaam.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/victory.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/yellow.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/yohananof.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/zolvebegadol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:54:38.733460 il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/file_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/gzip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/retrey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:54:38.733460 il-supermarket-scraper-0.2.9/il_supermarket_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-15 11:54:38.000000 il-supermarket-scraper-0.2.9/il_supermarket_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-15 11:54:38.000000 il-supermarket-scraper-0.2.9/il_supermarket_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:54:38.000000 il-supermarket-scraper-0.2.9/il_supermarket_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-15 11:54:38.000000 il-supermarket-scraper-0.2.9/il_supermarket_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 11:54:38.000000 il-supermarket-scraper-0.2.9/il_supermarket_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 11:54:38.737460 il-supermarket-scraper-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:54:38.737460 il-supermarket-scraper-0.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-15 11:54:27.000000 il-supermarket-scraper-0.2.9/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:10:17.395575 il-supermarket-scraper-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-28 07:10:17.395575 il-supermarket-scraper-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:10:17.391575 il-supermarket-scraper-0.3/il_supermarket_scarper/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:10:17.391575 il-supermarket-scraper-0.3/il_supermarket_scarper/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/engines/apsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/engines/bina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/engines/cerberus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/engines/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/engines/multipage_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/engines/publishprice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/engines/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrapper_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:10:17.395575 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/bareket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/bitan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/cofix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/doralon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/good_pharm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/hazihinam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/keshet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/king_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/maayan2000.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/machsani_ashuk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/mega.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/mega_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/nativ_hashed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/osherad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/polizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/ramilevy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/salachdabach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/shefa_barcart_ashem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/shufersal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/shuk_ahir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/stop_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/super_pharm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/super_yuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/superdosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/tivtaam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/victory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/yellow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/yohananof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/zolvebegadol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:10:17.395575 il-supermarket-scraper-0.3/il_supermarket_scarper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/utils/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/utils/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/utils/gzip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/utils/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/utils/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/utils/retrey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/il_supermarket_scarper/utils/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:10:17.395575 il-supermarket-scraper-0.3/il_supermarket_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-28 07:10:17.000000 il-supermarket-scraper-0.3/il_supermarket_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-28 07:10:17.000000 il-supermarket-scraper-0.3/il_supermarket_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 07:10:17.000000 il-supermarket-scraper-0.3/il_supermarket_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-28 07:10:17.000000 il-supermarket-scraper-0.3/il_supermarket_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 07:10:17.000000 il-supermarket-scraper-0.3/il_supermarket_scraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 07:10:17.395575 il-supermarket-scraper-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:10:17.395575 il-supermarket-scraper-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-28 07:10:08.000000 il-supermarket-scraper-0.3/tests/test_main.py
```

### Comparing `il-supermarket-scraper-0.2.9/LICENSE.txt` & `il-supermarket-scraper-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/PKG-INFO` & `il-supermarket-scraper-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: il-supermarket-scraper
-Version: 0.2.9
+Version: 0.3
 Summary: python package that implement a scraping for israeli supermarket data
 Home-page: https://github.com/jladan/package_demo
 Author: Sefi Erlich
 Author-email: erlichsefi@gmail.com
 License: MIT
 Keywords: israel,israeli,scraper,supermarket
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `il-supermarket-scraper-0.2.9/README.md` & `il-supermarket-scraper-0.3/README.md`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/apsx.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/engines/apsx.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/bina.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/engines/bina.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/cerberus.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/engines/cerberus.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from il_supermarket_scarper.utils import (
     extract_xml_file_from_gz_file,
     Logger,
     execute_in_event_loop,
     collect_from_ftp,
     fetch_temporary_gz_file_from_ftp,
+    retry_files,
 )
 from .engine import Engine
 
 
 class Cerberus(Engine):
     """scraper for all Cerberus base site. (seems like can't support historical data)"""
 
@@ -29,45 +30,56 @@
         super().__init__(chain, chain_id, folder_name)
         self.ftp_host = ftp_host
         self.ftp_path = ftp_path
         self.ftp_username = ftp_username
         self.ftp_password = ftp_password
         self.ftp_session = False
 
-    def scrape(self, limit=None, files_types=None, store_id=None, only_latest=False):
+    @retry_files(num_of_retrys=2)
+    def scrape(
+        self,
+        limit=None,
+        files_types=None,
+        store_id=None,
+        only_latest=False,
+        files_names_to_scrape=None,
+    ):
         super().scrape(
             limit=limit,
             files_types=files_types,
             store_id=store_id,
             only_latest=only_latest,
         )
         files = self.collect_files_details_from_site(
             limit=limit,
             files_types=files_types,
             filter_null=True,
             filter_zero=True,
             store_id=store_id,
             only_latest=only_latest,
+            files_names_to_scrape=files_names_to_scrape,
         )
         self.on_collected_details(files)
 
         results = execute_in_event_loop(
             self.persist_from_ftp, files, max_workers=self.max_workers
         )
         self.on_download_completed(results=results)
         self.on_scrape_completed(self.get_storage_path())
+        return results
 
     def collect_files_details_from_site(
         self,
         limit=None,
         files_types=None,
         filter_null=False,
         filter_zero=False,
         store_id=None,
         only_latest=False,
+        files_names_to_scrape=None,
     ):
         """collect all files to download from the site"""
         files = collect_from_ftp(
             self.ftp_host, self.ftp_username, self.ftp_password, self.ftp_path
         )
 
         Logger.info(f"Found {len(files)} files")
@@ -94,24 +106,26 @@
         # apply noraml filter
         files = self.apply_limit(
             files,
             limit=limit,
             files_types=files_types,
             store_id=store_id,
             only_latest=only_latest,
+            files_names_to_scrape=files_names_to_scrape,
         )
         Logger.info(f"After applying limit: Found {len(files)} files")
 
         return files
 
     def persist_from_ftp(self, file_name):
         """download file to hard drive and extract it."""
         downloaded = False
         extract_succefully = False
-        additionl_info = {}
+        restart_and_retry = False
+        error = None
         try:
             ext = os.path.splitext(file_name)[1]
             if ext not in [".gz", ".xml"]:
                 raise ValueError(f"File {file_name} extension is not .gz or .xml")
 
             Logger.info(f"Start persisting file {file_name}")
             temporary_gz_file_path = os.path.join(self.storage_path, file_name)
@@ -132,19 +146,20 @@
             extract_succefully = True
         except Exception as exception:  # pylint: disable=broad-except
             Logger.error(
                 f"Error downloading {file_name},extract_succefully={extract_succefully}"
                 f",downloaded={downloaded}"
             )
             Logger.error_execption(exception)
-            additionl_info = {"error": str(exception)}
-
+            error = str(exception)
+            restart_and_retry = True
         finally:
             if ext == ".gz" and os.path.exists(temporary_gz_file_path):
                 os.remove(temporary_gz_file_path)
 
         return {
             "file_name": file_name,
             "downloaded": downloaded,
             "extract_succefully": extract_succefully,
-            **additionl_info,
+            "restart_and_retry": restart_and_retry,
+            "error": error,
         }
```

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/engine.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/engines/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     Logger,
     ScraperStatus,
     extract_xml_file_from_gz_file,
     url_connection_retry,
     session_with_cookies,
     url_retrieve,
     wget_file,
+    RestartSessionError,
 )
 
 
 class Engine(ScraperStatus, ABC):
     """base engine for scraping"""
 
     def __init__(
@@ -85,23 +86,24 @@
         self,
         intreable,
         limit=None,
         files_types=None,
         by_function=lambda x: x,
         store_id=None,
         only_latest=False,
+        files_names_to_scrape=None,
     ):
         """filter the list according to condition"""
         assert (
             not only_latest or limit is None
         ), "only_latest flag can't be applied with limit."
 
         # filter files already downloaded
         intreable_ = self.filter_already_downloaded(
-            self.storage_path, intreable, by_function=by_function
+            self.storage_path, files_names_to_scrape, intreable, by_function=by_function
         )
         files_was_filtered_since_already_download = (
             len(list(intreable)) != 0 and len(list(intreable_)) == 0
         )
 
         # filter unique links
         intreable_ = self.unique(intreable_, by_function=by_function)
@@ -195,21 +197,29 @@
 
     def post_scraping(self):
         """job to do post scraping"""
         cookie_file = f"{self.chain}_cookies.txt"
         if os.path.exists(cookie_file):
             os.remove(cookie_file)
 
-    def scrape(self, limit=None, files_types=None, store_id=None, only_latest=False):
+    def scrape(
+        self,
+        limit=None,
+        files_types=None,
+        store_id=None,
+        only_latest=False,
+        files_names_to_scrape=None,
+    ):
         """run the scraping logic"""
         self.post_scraping()
         self.on_scraping_start(
             limit=limit,
             files_types=files_types,
             store_id=store_id,
+            files_names_to_scrape=files_names_to_scrape,
             only_latest=only_latest,
         )
         Logger.info(f"Starting scraping for {self.chain}")
         self.make_storage_path_dir()
 
     def make_storage_path_dir(self):
         """create the storage path"""
@@ -237,46 +247,58 @@
 
     def save_and_extract(self, arg):
         """download file and extract it"""
 
         file_link, file_name = arg
         file_save_path = os.path.join(self.storage_path, file_name)
         Logger.info(f"Downloading {file_link} to {file_save_path}")
-        downloaded, extract_succefully, error = self._save_and_extract(
-            file_link, file_save_path
-        )
+        (
+            downloaded,
+            extract_succefully,
+            error,
+            restart_and_retry,
+        ) = self._save_and_extract(file_link, file_save_path)
 
         return {
             "file_name": file_name,
             "downloaded": downloaded,
             "extract_succefully": extract_succefully,
             "error": error,
+            "restart_and_retry": restart_and_retry,
         }
 
     def _save_and_extract(self, file_link, file_save_path):
         downloaded = False
         extract_succefully = False
         error = None
+        restart_and_retry = False
         try:
             try:
                 file_save_path_with_ext = self.retrieve_file(file_link, file_save_path)
             except Exception:  # pylint: disable=broad-except
                 file_save_path_with_ext = wget_file(file_link, file_save_path)
             downloaded = True
 
             if file_save_path_with_ext.endswith("gz"):
                 extract_xml_file_from_gz_file(file_save_path_with_ext)
 
                 os.remove(file_save_path_with_ext)
             extract_succefully = True
 
             Logger.info(f"Done downloading {file_link}")
-
+        except RestartSessionError as exception:
+            Logger.error(
+                f"Error downloading {file_link},extract_succefully={extract_succefully}"
+                f",downloaded={downloaded}"
+            )
+            Logger.error_execption(exception)
+            error = str(exception)
+            restart_and_retry = True
         except Exception as exception:  # pylint: disable=broad-except
             Logger.error(
                 f"Error downloading {file_link},extract_succefully={extract_succefully}"
                 f",downloaded={downloaded}"
             )
             Logger.error_execption(exception)
             error = str(exception)
 
-        return downloaded, extract_succefully, error
+        return downloaded, extract_succefully, error, restart_and_retry
```

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/matrix.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/engines/matrix.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/multipage_web.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/engines/multipage_web.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,15 +56,20 @@
             raise ConnectionError(
                 f"Didn't find the element contains number"
                 f" of pages. found={elements}, in {html}."
             )
         return int(elements[0])
 
     def collect_files_details_from_site(
-        self, limit=None, files_types=None, store_id=None, only_latest=False
+        self,
+        limit=None,
+        files_types=None,
+        store_id=None,
+        only_latest=False,
+        files_names_to_scrape=None,
     ):
         self.post_scraping()
         url = self.get_request_url()
 
         total_pages = self.get_number_of_pages(url[0])
         Logger.info(f"Found {total_pages} pages")
 
@@ -84,14 +89,15 @@
         file_names, download_urls = self.apply_limit_zip(
             file_names,
             download_urls,
             limit=limit,
             files_types=files_types,
             store_id=store_id,
             only_latest=only_latest,
+            files_names_to_scrape=files_names_to_scrape
         )
 
         return download_urls, file_names
 
     def collect_files_details_from_page(self, html):
         """collect the details deom one page"""
         links = []
```

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/publishprice.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/engines/publishprice.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from bs4 import BeautifulSoup
 
 from il_supermarket_scarper.utils import (
     Logger,
     session_and_check_status,
     _is_weekend_in_israel,
     _is_holiday_in_israel,
+    _now,
 )
 from .web import WebBase
 
 
 class PublishPrice(WebBase):
     """
     scrape the file of PublishPrice
@@ -24,16 +25,22 @@
             folder_name=folder_name,
         )
         self.folder = None
 
     def get_data_from_page(self, req_res):
         soup = BeautifulSoup(req_res.text, features="lxml")
 
-        self.folder = soup.find_all("tr")[3].a.attrs["href"]
-        Logger.info(f"Last folder is {self.folder}")
+        target_date = _now().strftime("%Y%m%d")
+        current_date_page = list(
+            filter(lambda x: target_date in str(x.a), soup.find_all("tr"))
+        )
+        assert len(current_date_page) == 1, f"can't find {target_date}"
+
+        self.folder = current_date_page[0].a.attrs["href"]
+        Logger.info(f"Looking at folder = {self.folder}")
 
         req_res = session_and_check_status(self.url + self.folder)
         soup = BeautifulSoup(req_res.text, features="lxml")
         return soup.find_all("tr")[3:]
 
     def extract_task_from_entry(self, all_trs):
         # filter empty files
@@ -52,15 +59,22 @@
 
     def get_store_name_format(self, store_id):
         return f"-{store_id:04d}-"
 
     def _is_validate_scraper_found_no_files(
         self, limit=None, files_types=None, store_id=None, only_latest=False
     ):
-        return super()._is_validate_scraper_found_no_files(  # what fails the rest
-            limit=limit,
-            files_types=files_types,
-            store_id=store_id,
-            only_latest=only_latest,
-        ) or (
-            store_id and (_is_weekend_in_israel() or _is_holiday_in_israel())
-        )  # if we are looking for one store file in a weekend or holiday
+        return (
+            super()._is_validate_scraper_found_no_files(  # what fails the rest
+                limit=limit,
+                files_types=files_types,
+                store_id=store_id,
+                only_latest=only_latest,
+            )
+            or (  # if we are looking for one store file in a weekend or holiday
+                store_id and (_is_weekend_in_israel() or _is_holiday_in_israel())
+            )
+            or (  # if we are looking a specific number of file in a weekend or holiday
+                limit is not None
+                and (_is_weekend_in_israel() or _is_holiday_in_israel())
+            )
+        )
```

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/engines/web.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/engines/web.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from bs4 import BeautifulSoup
 from il_supermarket_scarper.utils import (
     Logger,
     execute_in_event_loop,
     session_and_check_status,
+    retry_files,
 )
 
 from .engine import Engine
 
 
 class WebBase(Engine):
     """scrape the file of websites that the only why to download them is via web"""
 
     def __init__(self, chain, chain_id, url, folder_name=None):
         super().__init__(chain, chain_id, folder_name)
         self.url = url
+        self.max_retry = 2
 
     def get_data_from_page(self, req_res):
         """get the file list from a page"""
         soup = BeautifulSoup(req_res.text, features="lxml")
         return soup.find_all("tr")[1:]
 
     def get_request_url(self):
@@ -38,31 +40,38 @@
         file_names,
         download_urls,
         limit=None,
         files_types=None,
         by_function=lambda x: x[0],
         store_id=None,
         only_latest=False,
+        files_names_to_scrape=None,
     ):
         """apply limit to zip"""
         ziped = self.apply_limit(
             list(zip(file_names, download_urls)),
             limit=limit,
             files_types=files_types,
             by_function=by_function,
             store_id=store_id,
             only_latest=only_latest,
+            files_names_to_scrape=files_names_to_scrape,
         )
         if len(ziped) == 0:
             return [], []
         return list(zip(*ziped))
 
     # @cache()
     def collect_files_details_from_site(
-        self, limit=None, files_types=None, store_id=None, only_latest=False
+        self,
+        limit=None,
+        files_types=None,
+        store_id=None,
+        only_latest=False,
+        files_names_to_scrape=None,
     ):
         """collect all enteris to download from site"""
         urls_to_collect_link_from = self.get_request_url()
 
         all_trs = []
         for url in urls_to_collect_link_from:
             req_res = session_and_check_status(url)
@@ -78,41 +87,56 @@
             file_names, download_urls = self.apply_limit_zip(
                 file_names,
                 download_urls,
                 limit=limit,
                 files_types=files_types,
                 store_id=store_id,
                 only_latest=only_latest,
+                files_names_to_scrape=files_names_to_scrape,
             )
 
             Logger.info(f"After applying limit: Found {len(all_trs)} entries")
 
         return download_urls, file_names
 
-    # solution: add files_names_to_scrape as in input to func scrape
-    # filter 'results' to faillers and retrey.
-    def scrape(self, limit=None, files_types=None, store_id=None, only_latest=False):
+    @retry_files(num_of_retrys=2)
+    def scrape(
+        self,
+        limit=None,
+        files_types=None,
+        store_id=None,
+        only_latest=False,
+        files_names_to_scrape=None,
+    ):
         """scarpe the files from multipage sites"""
         super().scrape(
-            limit, files_types=files_types, store_id=store_id, only_latest=only_latest
+            limit,
+            files_types=files_types,
+            store_id=store_id,
+            only_latest=only_latest,
         )
 
         download_urls, file_names = self.collect_files_details_from_site(
             limit=limit,
             files_types=files_types,
             store_id=store_id,
             only_latest=only_latest,
+            files_names_to_scrape=files_names_to_scrape,
         )
+
         self.on_collected_details(file_names, download_urls)
 
         Logger.info(f"collected {len(download_urls)} to download.")
         if len(download_urls) > 0:
             results = execute_in_event_loop(
                 self.save_and_extract,
                 zip(download_urls, file_names),
                 max_workers=self.max_workers,
             )
         else:
             results = {}
+
         self.on_download_completed(results=results)
+
         self.on_scrape_completed(self.get_storage_path())
         self.post_scraping()
+        return results
```

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/main.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/main.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrapper_runner.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/scrapper_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         if self.lookup_in_db:
             scraper.enable_collection_status()
         scraper.scrape(
             limit=limit,
             files_types=files_types,
             store_id=store_id,
             only_latest=only_latest,
+            files_names_to_scrape=None,
         )
         Logger.info(f"done scraping {chain_name}")
 
         folder_with_files = scraper.get_storage_path()
         if self.size_estimation_mode:
             Logger.info(f"Summrize test data for {chain_name}")
             summerize_dump_folder_contant(folder_with_files)
```

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/__init__.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/bareket.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/bareket.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/cofix.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/cofix.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/nativ_hashed.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/nativ_hashed.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/polizer.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/polizer.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/super_pharm.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/super_pharm.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers/tivtaam.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers/tivtaam.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/scrappers_factory.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/scrappers_factory.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/__init__.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .status import (
     get_output_folder,
     clean_dump_folder,
     summerize_dump_folder_contant,
     _is_saturday_in_israel,
     _is_holiday_in_israel,
     _is_weekend_in_israel,
+    _now,
 )
 from .mongo import ScraperStatus
 from .file_types import FileTypesFilters
 from .connection import (
     download_connection_retry,
     url_connection_retry,
     disable_when_outside_israel,
@@ -19,7 +20,9 @@
     cache,
     url_retrieve,
     collect_from_ftp,
     fetch_temporary_gz_file_from_ftp,
     wget_file,
 )
 from .loop import execute_in_event_loop, multiple_page_aggregtion
+from .exceptions import RestartSessionError
+from .retrey import retry_files
```

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/connection.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/utils/connection.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/file_types.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/utils/file_types.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/gzip_utils.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/utils/gzip_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import gzip
 import shutil
 import os
 import io
 import zipfile
+from .exceptions import RestartSessionError
 
 
 def extract_xml_file_from_gz_file(file_save_path):
     """extract xml from gz"""
     try:
         with gzip.open(file_save_path, "rb") as infile:
             with open(os.path.splitext(file_save_path)[0] + ".xml", "wb") as outfile:
@@ -32,12 +33,16 @@
 def report_failed_zip(exception, file_save_path):
     """report a file wasn't able to extracted"""
     file_contant = ""
     with open(file_save_path, "r", encoding="utf-8") as file:
         file_contant = file.readlines()
     file_size = os.path.getsize(file_save_path)
     os.remove(file_save_path)
+
+    if "link expired" in str(file_contant):
+        raise RestartSessionError()
+
     raise ValueError(
         f"Error decoding file:{ file_save_path } with "
         f"error: {str(exception)} file size {str(file_size) } ,"
         f"file_contant {str(file_contant)}"
     )
```

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/logger.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/loop.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/utils/loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         # use multi-thread
         futures = []
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             for arg in iterable:
                 futures.append(loop.run_in_executor(executor, function_to_execute, arg))
 
         if len(futures) == 0:
-            return [], []
+            return []
         all_done, not_done = await asyncio.wait(futures)
         assert len(not_done) == 0, "Not all tasks are done, should be blocking."
     else:
         # or just itreate over all
         all_done = []
         for arg in iterable:
             all_done.append(function_to_execute(arg))
```

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/mongo.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/utils/mongo.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     def on_download_completed(self, **additional_info):
         """report file downloaded"""
         self._insert_an_update(ScraperStatus.DOWNLOADED, **additional_info)
         self._add_downloaded_files_to_list(**additional_info)
 
     def filter_already_downloaded(
-        self, storage_path, filelist, by_function=lambda x: x
+        self, storage_path, files_names_to_scrape, filelist, by_function=lambda x: x
     ):
         """filter files already exists in long term memory or was downloaded before"""
         if self.collection_status:
             # filter according to database
             store_db = self.myclient[self.database]
 
             new_filelist = []
@@ -95,15 +95,25 @@
                         f"filtered file {file} since it already "
                         "was downloaded and extracted"
                     )
             return new_filelist
 
         # filter according to disk
         exits_on_disk = os.listdir(storage_path)
-        return list(filter(lambda x: x not in exits_on_disk, filelist))
+
+        if files_names_to_scrape:
+            # delete what ever to retry
+            for file in exits_on_disk:
+                if file.split(".")[0] in files_names_to_scrape:
+                    os.remove(os.path.join(storage_path,file))
+
+            # find only the files we would like to download
+            filelist = list(filter(lambda x: by_function(x) in files_names_to_scrape, filelist))
+
+        return list(filter(lambda x: by_function(x) not in exits_on_disk, filelist))
 
     def _add_downloaded_files_to_list(self, results, **_):
         if self.collection_status:
             when = datetime.datetime.now()
             store_db = self.myclient[self.database]
             for res in results:
                 if res["downloaded"] and res["extract_succefully"]:
```

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/retrey.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/utils/retrey.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import random
 import time
+import inspect
 
 from datetime import datetime
 from functools import partial
 
 import functools
 
 
@@ -187,7 +188,77 @@
         tries,
         delay,
         max_delay,
         backoff,
         jitter,
         logger,
     )
+
+
+def retry_files(num_of_retrys=2, arg_name="files_names_to_scrape"):
+    """retry only ceritin files"""
+
+    @decorator
+    def retry_files_decorator(func, *fargs, **fkwargs):
+        args = fargs if fargs else []
+        kwargs = fkwargs if fkwargs else {}
+        return __retry_files(func, args, kwargs, arg_name, num_of_retrys=num_of_retrys)
+
+    return retry_files_decorator
+
+
+def __retry_files(
+    func,
+    args,
+    kwargs,
+    arg_name,
+    num_of_retrys=1,
+    logger=logging_logger,
+):
+    retry_list = []
+    all_results = []
+    for i in range(num_of_retrys):
+        logger.info(f"Itreation #{i},retry_list={retry_list}")
+
+        if retry_list:
+            # replace the value of 'files_names_to_scrape'
+            args_names = inspect.getfullargspec(func).args
+            assert arg_name in args_names, f"{arg_name} wasn't found in {args_names}."
+
+            arg_list = list(args)
+            arg_list[args_names.index(arg_name)] = retry_list
+            args = tuple(arg_list)
+
+        results = func(*args, **kwargs)
+
+        # next iteration
+        retry_list, other_results = compute_retry(results)
+
+        all_results.append(other_results)
+        # if there is not files in the retry list, break
+        if len(retry_list) == 0:
+            break
+
+    return all_results
+
+
+def compute_retry(results):
+    """find the files to retry"""
+    files_to_retry = []
+    other_results = []
+    for result in results:
+        if result["restart_and_retry"]:
+            files_to_retry.append(result["file_name"])
+        else:
+            other_results.append(result)
+    return files_to_retry, other_results
+
+
+# def filter_spesific_files(download_urls, file_names, retry_list):
+#     """filter the files to retry"""
+#     _download_urls = []
+#     _file_names = []
+#     for download_url, file_name in zip(download_urls, file_names):
+#         if file_name in retry_list:
+#             _download_urls.append(download_url)
+#             _file_names.append(file_name)
+#     return _download_urls, _file_names
```

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scarper/utils/status.py` & `il-supermarket-scraper-0.3/il_supermarket_scarper/utils/status.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scraper.egg-info/PKG-INFO` & `il-supermarket-scraper-0.3/il_supermarket_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: il-supermarket-scraper
-Version: 0.2.9
+Version: 0.3
 Summary: python package that implement a scraping for israeli supermarket data
 Home-page: https://github.com/jladan/package_demo
 Author: Sefi Erlich
 Author-email: erlichsefi@gmail.com
 License: MIT
 Keywords: israel,israeli,scraper,supermarket
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `il-supermarket-scraper-0.2.9/il_supermarket_scraper.egg-info/SOURCES.txt` & `il-supermarket-scraper-0.3/il_supermarket_scraper.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 il_supermarket_scarper/scrappers/tivtaam.py
 il_supermarket_scarper/scrappers/victory.py
 il_supermarket_scarper/scrappers/yellow.py
 il_supermarket_scarper/scrappers/yohananof.py
 il_supermarket_scarper/scrappers/zolvebegadol.py
 il_supermarket_scarper/utils/__init__.py
 il_supermarket_scarper/utils/connection.py
+il_supermarket_scarper/utils/exceptions.py
 il_supermarket_scarper/utils/file_types.py
 il_supermarket_scarper/utils/gzip_utils.py
 il_supermarket_scarper/utils/logger.py
 il_supermarket_scarper/utils/loop.py
 il_supermarket_scarper/utils/mongo.py
 il_supermarket_scarper/utils/retrey.py
 il_supermarket_scarper/utils/status.py
```

### Comparing `il-supermarket-scraper-0.2.9/setup.py` & `il-supermarket-scraper-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,26 @@
         "il_supermarket_scarper.scrappers",
         "il_supermarket_scarper.utils",
     ],
     # Needed for dependencies
     install_requires=[
         "retry==0.9.2",
         "mock==4.0.3",
-        "requests==2.28.2",
+        "requests==2.31.0",
         "lxml==4.9.1",
         "beautifulsoup4==4.10.0",
         "pymongo==4.2.0",
         "pytz==2022.4",
         "holidays==0.16",
         "cachetools==5.2.0",
     ],
     tests_require=["pytest==7.1"],
     extras_require={"test": ["pytest"]},
     # *strongly* suggested for sharing
-    version="0.2.9",
+    version="0.3",
     # The license can be anything you like
     license="MIT",
     description="python package that implement a scraping for israeli supermarket data",
     # We will also need a readme eventually (there will be a warning)
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["israel", "israeli", "scraper", "supermarket"],
```

### Comparing `il-supermarket-scraper-0.2.9/tests/test_integration.py` & `il-supermarket-scraper-0.3/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from il_supermarket_scarper.utils.status import get_status
 from il_supermarket_scarper.scrappers_factory import ScraperFactory
 from il_supermarket_scarper.utils.connection import disable_when_outside_israel
 
 
 @disable_when_outside_israel
 def test_scrapers_are_updated():
-    """test the number of scrapers are the same as listed at the gov.il sirte"""
+    """test the number of scrapers are the same as listed at the gov.il site"""
     num_of_scarper_listed = len(ScraperFactory.all_scrapers_name())
     num_of_scarper_on_gov_site = get_status()
 
     assert num_of_scarper_listed == num_of_scarper_on_gov_site
 
 
 def test_all_chain_id_unqiue():
```

### Comparing `il-supermarket-scraper-0.2.9/tests/test_main.py` & `il-supermarket-scraper-0.3/tests/test_main.py`

 * *Files identical despite different names*

