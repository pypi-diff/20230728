# Comparing `tmp/pymediawiki-0.7.2.tar.gz` & `tmp/pymediawiki-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymediawiki-0.7.2.tar", last modified: Mon Sep  5 15:55:01 2022, max compression
+gzip compressed data, was "pymediawiki-0.7.3.tar", last modified: Fri Jul 28 17:33:46 2023, max compression
```

## Comparing `pymediawiki-0.7.2.tar` & `pymediawiki-0.7.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.160260 pymediawiki-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.144260 pymediawiki-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.148260 pymediawiki-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1531 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    12395 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     6320 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     7044 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5615 2022-09-05 15:55:01.160260 pymediawiki-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4355 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.148260 pymediawiki-0.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     8085 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.148260 pymediawiki-0.7.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.148260 pymediawiki-0.7.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.144260 pymediawiki-0.7.2/docs/source/_themes/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.148260 pymediawiki-0.7.2/docs/source/_themes/custom_theme/
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3873 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (121)     1977 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)     7535 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/search.html
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.144260 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.148260 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3358 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/css/badge_only.css
--rw-r--r--   0 runner    (1001) docker     (121)   116310 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/css/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.148260 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)   134808 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (121)   165742 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (121)   444379 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (121)   165548 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    98024 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (121)    77160 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.148260 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)    15414 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/js/modernizr.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     4400 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/_themes/custom_theme/versions.html
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/code.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9857 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4970 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.152260 pymediawiki-0.7.2/mediawiki/
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/mediawiki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7672 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/mediawiki/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    35044 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/mediawiki/mediawiki.py
--rw-r--r--   0 runner    (1001) docker     (121)    31534 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/mediawiki/mediawikipage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2645 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/mediawiki/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.152260 pymediawiki-0.7.2/pymediawiki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5615 2022-09-05 15:55:01.000000 pymediawiki-0.7.2/pymediawiki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-09-05 15:55:01.000000 pymediawiki-0.7.2/pymediawiki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 15:55:01.000000 pymediawiki-0.7.2/pymediawiki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 15:55:00.000000 pymediawiki-0.7.2/pymediawiki.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 15:55:01.000000 pymediawiki-0.7.2/pymediawiki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-05 15:55:01.000000 pymediawiki-0.7.2/pymediawiki.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.152260 pymediawiki-0.7.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)    19940 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/scripts/generate_test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-09-05 15:55:01.164260 pymediawiki-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:55:01.160260 pymediawiki-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    69040 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/tests/mediawiki_test.py
--rw-r--r--   0 runner    (1001) docker     (121)  1553032 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/tests/mock_categorytree.json
--rw-r--r--   0 runner    (1001) docker     (121)  9398407 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/tests/mock_requests.json
--rw-r--r--   0 runner    (1001) docker     (121)   830140 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/tests/mock_responses.json
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-09-05 15:54:45.000000 pymediawiki-0.7.2/tests/utilities.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.848982 pymediawiki-0.7.3/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.780982 pymediawiki-0.7.3/.github/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.788982 pymediawiki-0.7.3/.github/workflows/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      873 2022-11-23 01:48:52.000000 pymediawiki-0.7.3/.github/workflows/publish.yml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1532 2023-07-28 16:46:38.000000 pymediawiki-0.7.3/.github/workflows/python-package.yml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1089 2023-07-28 16:46:38.000000 pymediawiki-0.7.3/.gitignore
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    20216 2022-09-27 17:16:18.000000 pymediawiki-0.7.3/.pylintrc
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6675 2023-07-28 17:26:09.000000 pymediawiki-0.7.3/CHANGELOG.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7044 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/CONTRIBUTING.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1069 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     5615 2023-07-28 17:33:46.848982 pymediawiki-0.7.3/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4355 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/README.rst
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      547 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/codecov.yml
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.788982 pymediawiki-0.7.3/docs/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     8085 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/Makefile
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.788982 pymediawiki-0.7.3/docs/source/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.788982 pymediawiki-0.7.3/docs/source/_static/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_static/.gitkeep
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.780982 pymediawiki-0.7.3/docs/source/_themes/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.792982 pymediawiki-0.7.3/docs/source/_themes/custom_theme/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      520 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3873 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/breadcrumbs.html
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1977 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/footer.html
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7535 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/layout.html
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1530 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/search.html
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      365 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/searchbox.html
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.784982 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.792982 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/css/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3358 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/css/badge_only.css
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)   116310 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/css/theme.css
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.800982 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/fonts/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)   134808 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/fonts/FontAwesome.otf
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)   165742 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)   444379 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)   165548 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    98024 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.woff
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    77160 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.woff2
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.800982 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/js/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    15414 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/js/modernizr.min.js
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4400 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/js/theme.js
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      327 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/theme.conf
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1299 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/_themes/custom_theme/versions.html
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1649 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/code.rst
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     9857 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/conf.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      196 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/index.rst
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4970 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/docs/source/quickstart.rst
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.804982 pymediawiki-0.7.3/mediawiki/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      960 2022-12-15 23:59:37.000000 pymediawiki-0.7.3/mediawiki/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7922 2023-07-28 16:46:38.000000 pymediawiki-0.7.3/mediawiki/exceptions.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    35652 2023-07-28 17:26:09.000000 pymediawiki-0.7.3/mediawiki/mediawiki.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    31534 2022-12-15 23:59:37.000000 pymediawiki-0.7.3/mediawiki/mediawikipage.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2645 2022-12-15 23:59:37.000000 pymediawiki-0.7.3/mediawiki/utilities.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.804982 pymediawiki-0.7.3/pymediawiki.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     5615 2023-07-28 17:33:46.000000 pymediawiki-0.7.3/pymediawiki.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1821 2023-07-28 17:33:46.000000 pymediawiki-0.7.3/pymediawiki.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-07-28 17:33:46.000000 pymediawiki-0.7.3/pymediawiki.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2022-08-06 19:44:49.000000 pymediawiki-0.7.3/pymediawiki.egg-info/not-zip-safe
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       38 2023-07-28 17:33:46.000000 pymediawiki-0.7.3/pymediawiki.egg-info/requires.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       10 2023-07-28 17:33:46.000000 pymediawiki-0.7.3/pymediawiki.egg-info/top_level.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      293 2022-10-30 03:11:33.000000 pymediawiki-0.7.3/pyproject.toml
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.804982 pymediawiki-0.7.3/scripts/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    19940 2022-12-16 12:39:47.000000 pymediawiki-0.7.3/scripts/generate_test_data.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1555 2023-07-28 17:33:46.848982 pymediawiki-0.7.3/setup.cfg
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       38 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/setup.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-28 17:33:46.848982 pymediawiki-0.7.3/tests/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       23 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/tests/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    69040 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/tests/mediawiki_test.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)  1553032 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/tests/mock_categorytree.json
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)  9398407 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/tests/mock_requests.json
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)   830140 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/tests/mock_responses.json
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1248 2022-05-11 16:25:17.000000 pymediawiki-0.7.3/tests/utilities.py
```

### Comparing `pymediawiki-0.7.2/.github/workflows/publish.yml` & `pymediawiki-0.7.3/.github/workflows/publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install --upgrade twine build
     - name: Build and publish
```

### Comparing `pymediawiki-0.7.2/.github/workflows/python-package.yml` & `pymediawiki-0.7.3/.github/workflows/python-package.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.6', '3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install flake8 pytest pytest-cov
         python -m pip install -e .
```

### Comparing `pymediawiki-0.7.2/.gitignore` & `pymediawiki-0.7.3/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -88,7 +88,10 @@
 .spyderproject
 
 # Rope project settings
 .ropeproject
 
 # PyPi
 .pypirc
+
+# vscode
+.vscode/
```

### Comparing `pymediawiki-0.7.2/CHANGELOG.md` & `pymediawiki-0.7.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # MediaWiki Changelog
 
+## Version 0.7.3
+
+* Add `unordered_options` to the `DisambiguationError` to attempt to get options in the order presented on the page; [issue #124](https://github.com/barrust/mediawiki/issues/124)
+* Add [verify SSL support](https://requests.readthedocs.io/en/latest/user/advanced/#ssl-cert-verification) by passing info directly to the requests library.
+
 ## Version 0.7.2
 
 * Add `page_preview` property to simulate the page preview hover [PR #114](https://github.com/barrust/mediawiki/pull/114)
 * Add `available_languages` property [PR #116](https://github.com/barrust/mediawiki/pull/116)
 
 ## Version 0.7.1
```

### Comparing `pymediawiki-0.7.2/CONTRIBUTING.md` & `pymediawiki-0.7.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/LICENSE` & `pymediawiki-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/PKG-INFO` & `pymediawiki-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymediawiki
-Version: 0.7.2
+Version: 0.7.3
 Summary: Wikipedia and MediaWiki API wrapper for Python
 Home-page: https://github.com/barrust/mediawiki
 Author: Tyler Barrus
 Author-email: barrust@gmail.com
 License: MIT
 Keywords: python,mediawiki,wikipedia,API,wiki,parser,natural language processing,nlp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymediawiki-0.7.2/README.rst` & `pymediawiki-0.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/codecov.yml` & `pymediawiki-0.7.3/codecov.yml`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/Makefile` & `pymediawiki-0.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/__init__.py` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/breadcrumbs.html` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/footer.html` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/footer.html`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/layout.html` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/layout.html`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/search.html` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/search.html`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/css/badge_only.css` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/css/theme.css` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/fonts/FontAwesome.otf` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.eot` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.svg` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.ttf` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.woff` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.woff2` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/js/modernizr.min.js` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/js/modernizr.min.js`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/static/js/theme.js` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/_themes/custom_theme/versions.html` & `pymediawiki-0.7.3/docs/source/_themes/custom_theme/versions.html`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/code.rst` & `pymediawiki-0.7.3/docs/source/code.rst`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/conf.py` & `pymediawiki-0.7.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/docs/source/quickstart.rst` & `pymediawiki-0.7.3/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/mediawiki/__init__.py` & `pymediawiki-0.7.3/mediawiki/__init__.py`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/mediawiki/exceptions.py` & `pymediawiki-0.7.3/mediawiki/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 MediaWiki Exceptions
 """
 from .utilities import str_or_unicode
 
-
 ODD_ERROR_MESSAGE = (
     "This should not happen. If the MediaWiki site you are "
     "querying is available, then please report this issue on "
     "GitHub: github.com/barrust/mediawiki"
 )
 
 
@@ -124,14 +123,15 @@
                             possible results
         Note:
             `options` only includes titles that link to valid \
             MediaWiki pages """
 
     def __init__(self, title, may_refer_to, url, details=None):
         self._title = title
+        self._unordered_options = may_refer_to
         self._options = sorted(may_refer_to)
         self._details = details
         self._url = url
         msg = ('\n"{0}" may refer to: \n  ' "{1}").format(
             self.title, "\n  ".join(self.options)
         )
         super(DisambiguationError, self).__init__(msg)
@@ -148,14 +148,19 @@
 
     @property
     def options(self):
         """ list: The list of possible page titles """
         return self._options
 
     @property
+    def unordered_options(self):
+        """list: The list of possible page titles, un-sorted in an attempt to get them as they showup on the page"""
+        return self._unordered_options
+
+    @property
     def details(self):
         """ list: The details of the proposed non-disambigous pages """
         return self._details
 
 
 class HTTPTimeoutError(MediaWikiBaseException):
     """ Exception raised when a request to the Mediawiki site times out.
```

### Comparing `pymediawiki-0.7.2/mediawiki/mediawiki.py` & `pymediawiki-0.7.3/mediawiki/mediawiki.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     MediaWikiLoginError,
     PageError,
 )
 from .mediawikipage import MediaWikiPage
 from .utilities import memoize
 
 URL = "https://github.com/barrust/mediawiki"
-VERSION = "0.7.2"
+VERSION = "0.7.3"
 
 
 class MediaWiki(object):
     """ MediaWiki API Wrapper Instance
 
         Args:
             url (str): API URL of the MediaWiki site; defaults to Wikipedia
@@ -63,41 +63,45 @@
         "__supported_languages",
         "__available_languages",
         "_cache",
         "_refresh_interval",
         "_use_cache",
         "_is_logged_in",
         "_proxies",
+        "_verify_ssl",
     ]
 
     def __init__(
         self,
         url="https://{lang}.wikipedia.org/w/api.php",
         lang="en",
         timeout=15.0,
         rate_limit=False,
         rate_limit_wait=timedelta(milliseconds=50),
         cat_prefix="Category",
         user_agent=None,
         username=None,
         password=None,
         proxies=None,
+        verify_ssl=True,
     ):
         """ Init Function """
         self._version = VERSION
         self._lang = lang.lower()
         self._api_url = url.format(lang=self._lang)
         self._cat_prefix = None
         self.category_prefix = cat_prefix
         self._timeout = None
         self.timeout = timeout
         # requests library parameters
         self._session = None
         self._user_agent = ("python-mediawiki/VERSION-{0}" "/({1})/BOT").format(VERSION, URL)
         self._proxies = None
+        self._verify_ssl = None
+        self.verify_ssl = verify_ssl
         # set libary parameters
         if user_agent is not None:
             self.user_agent = user_agent
         self.proxies = proxies  # this will call self._reset_session()
 
         self._rate_limit = None
         self.rate_limit = bool(rate_limit)
@@ -224,14 +228,27 @@
 
         if timeout is None:
             self._timeout = None  # no timeout
             return
         self._timeout = float(timeout)  # allow the exception to be raised
 
     @property
+    def verify_ssl(self):
+        """ bool | str: Verify SSL when using requests or path to cert file """
+        return self._verify_ssl
+
+    @verify_ssl.setter
+    def verify_ssl(self, verify_ssl):
+        """ Set request verify SSL parameter; defaults to True if issue """
+        self._verify_ssl = True
+        if isinstance(verify_ssl, (bool, str)):
+            self._verify_ssl = verify_ssl
+        self._reset_session()
+
+    @property
     def language(self):
         """ str: The API URL language, if possible this will update the API \
                  URL
 
             Note:
                 Use correct language titles with the updated API URL
             Note:
@@ -399,14 +416,15 @@
             self._session.close()
 
         headers = {"User-Agent": self._user_agent}
         self._session = requests.Session()
         self._session.headers.update(headers)
         if self._proxies is not None:
             self._session.proxies.update(self._proxies)
+        self._session.verify = self._verify_ssl
         self._is_logged_in = False
 
     def clear_memoized(self):
         """ Clear memoized (cached) values """
         if hasattr(self, "_cache"):
             self._cache.clear()
```

### Comparing `pymediawiki-0.7.2/mediawiki/mediawikipage.py` & `pymediawiki-0.7.3/mediawiki/mediawikipage.py`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/mediawiki/utilities.py` & `pymediawiki-0.7.3/mediawiki/utilities.py`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/pymediawiki.egg-info/PKG-INFO` & `pymediawiki-0.7.3/pymediawiki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymediawiki
-Version: 0.7.2
+Version: 0.7.3
 Summary: Wikipedia and MediaWiki API wrapper for Python
 Home-page: https://github.com/barrust/mediawiki
 Author: Tyler Barrus
 Author-email: barrust@gmail.com
 License: MIT
 Keywords: python,mediawiki,wikipedia,API,wiki,parser,natural language processing,nlp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymediawiki-0.7.2/pymediawiki.egg-info/SOURCES.txt` & `pymediawiki-0.7.3/pymediawiki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/scripts/generate_test_data.py` & `pymediawiki-0.7.3/scripts/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/setup.cfg` & `pymediawiki-0.7.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pymediawiki
-version = 0.7.2
+version = attr: mediawiki.__version__
 author = Tyler Barrus
 author_email = barrust@gmail.com
 url = https://github.com/barrust/mediawiki
 description = Wikipedia and MediaWiki API wrapper for Python
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = python, mediawiki, wikipedia, API, wiki, parser, natural language processing, nlp
```

### Comparing `pymediawiki-0.7.2/tests/mediawiki_test.py` & `pymediawiki-0.7.3/tests/mediawiki_test.py`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/tests/mock_categorytree.json` & `pymediawiki-0.7.3/tests/mock_categorytree.json`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/tests/mock_requests.json` & `pymediawiki-0.7.3/tests/mock_requests.json`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/tests/mock_responses.json` & `pymediawiki-0.7.3/tests/mock_responses.json`

 * *Files identical despite different names*

### Comparing `pymediawiki-0.7.2/tests/utilities.py` & `pymediawiki-0.7.3/tests/utilities.py`

 * *Files identical despite different names*

