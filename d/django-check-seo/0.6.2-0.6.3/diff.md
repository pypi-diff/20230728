# Comparing `tmp/django-check-seo-0.6.2.tar.gz` & `tmp/django-check-seo-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-check-seo-0.6.2.tar", last modified: Wed Apr 19 13:25:48 2023, max compression
+gzip compressed data, was "django-check-seo-0.6.3.tar", last modified: Fri Jul 28 14:00:07 2023, max compression
```

## Comparing `django-check-seo-0.6.2.tar` & `django-check-seo-0.6.3.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.803523 django-check-seo-0.6.2/
--rw-r--r--   0 kapt      (1000) kapt      (1000)       93 2023-04-19 13:25:26.000000 django-check-seo-0.6.2/.bumpversion.cfg
--rw-r--r--   0 kapt      (1000) kapt      (1000)      365 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/.coveragerc
--rw-r--r--   0 kapt      (1000) kapt      (1000)       74 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/.flake8
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.791523 django-check-seo-0.6.2/.github/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.795523 django-check-seo-0.6.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 kapt      (1000) kapt      (1000)      834 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)      595 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)      130 2021-09-09 16:31:58.000000 django-check-seo-0.6.2/.gitignore
--rw-r--r--   0 kapt      (1000) kapt      (1000)      113 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/.isort.cfg
--rw-r--r--   0 kapt      (1000) kapt      (1000)      797 2022-06-14 09:16:04.000000 django-check-seo-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0 kapt      (1000) kapt      (1000)       78 2021-09-09 16:31:58.000000 django-check-seo-0.6.2/AUTHORS.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)    16871 2023-04-19 13:25:29.000000 django-check-seo-0.6.2/CHANGELOG.rst
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1554 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/CONTRIBUTING.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)    35149 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/LICENSE
--rw-r--r--   0 kapt      (1000) kapt      (1000)      220 2022-06-14 08:10:41.000000 django-check-seo-0.6.2/MANIFEST.in
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6745 2023-04-19 13:25:48.803523 django-check-seo-0.6.2/PKG-INFO
--rw-r--r--   0 kapt      (1000) kapt      (1000)     5661 2023-04-18 13:48:27.000000 django-check-seo-0.6.2/README.md
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.799523 django-check-seo-0.6.2/django_check_seo/
--rw-r--r--   0 kapt      (1000) kapt      (1000)       66 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      181 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/apps.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.799523 django-check-seo-0.6.2/django_check_seo/checks/
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/checks/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      320 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/checks/custom_list.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1778 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/checks/site.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.799523 django-check-seo-0.6.2/django_check_seo/checks_list/
--rw-r--r--   0 kapt      (1000) kapt      (1000)      418 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/checks_list/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     7826 2023-03-03 15:45:59.000000 django-check-seo-0.6.2/django_check_seo/checks_list/check_description.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4001 2022-06-14 09:17:55.000000 django-check-seo-0.6.2/django_check_seo/checks_list/check_h1.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3793 2022-06-14 09:17:55.000000 django-check-seo-0.6.2/django_check_seo/checks_list/check_h2.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2914 2022-06-14 09:27:26.000000 django-check-seo-0.6.2/django_check_seo/checks_list/check_images.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3931 2022-06-14 09:17:55.000000 django-check-seo-0.6.2/django_check_seo/checks_list/check_keyword_url.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1928 2023-04-19 13:25:13.000000 django-check-seo-0.6.2/django_check_seo/checks_list/check_keywords.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4092 2022-06-14 09:17:55.000000 django-check-seo-0.6.2/django_check_seo/checks_list/check_links.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     5709 2022-06-14 09:17:55.000000 django-check-seo-0.6.2/django_check_seo/checks_list/check_title.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3367 2022-06-14 09:17:55.000000 django-check-seo-0.6.2/django_check_seo/checks_list/check_url.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2018 2022-06-14 09:17:55.000000 django-check-seo-0.6.2/django_check_seo/checks_list/content_words_number.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2453 2022-06-14 09:17:55.000000 django-check-seo-0.6.2/django_check_seo/checks_list/keyword_present_first_paragraph.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2052 2022-09-21 15:03:12.000000 django-check-seo-0.6.2/django_check_seo/checks_list/launch_checks.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      668 2023-03-03 15:45:59.000000 django-check-seo-0.6.2/django_check_seo/cms_toolbars.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.799523 django-check-seo-0.6.2/django_check_seo/conf/
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/conf/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      815 2022-06-14 08:53:12.000000 django-check-seo-0.6.2/django_check_seo/conf/settings.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.795523 django-check-seo-0.6.2/django_check_seo/locale/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.795523 django-check-seo-0.6.2/django_check_seo/locale/fr/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.799523 django-check-seo-0.6.2/django_check_seo/locale/fr/LC_MESSAGES/
--rw-r--r--   0 kapt      (1000) kapt      (1000)    16533 2022-06-14 09:38:51.000000 django-check-seo-0.6.2/django_check_seo/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 kapt      (1000) kapt      (1000)    24514 2022-06-14 09:38:24.000000 django-check-seo-0.6.2/django_check_seo/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.799523 django-check-seo-0.6.2/django_check_seo/migrations/
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/migrations/__init__.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.795523 django-check-seo-0.6.2/django_check_seo/static/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.799523 django-check-seo-0.6.2/django_check_seo/static/django-check-seo/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4734 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/static/django-check-seo/design.css
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.803523 django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/
--rw-r--r--   0 kapt      (1000) kapt      (1000)    11358 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/LICENCE
--rw-r--r--   0 kapt      (1000) kapt      (1000)      139 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/NOTICE
--rw-r--r--   0 kapt      (1000) kapt      (1000)   164936 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/Roboto-Black.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)   163448 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/Roboto-Bold.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)   162636 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/Roboto-Light.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)   158604 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/Roboto-Regular.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)   122512 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/Roboto-Thin.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)    15388 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/static/django-check-seo/logo-small.png
--rw-r--r--   0 kapt      (1000) kapt      (1000)   137074 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/static/django-check-seo/logo.png
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.803523 django-check-seo-0.6.2/django_check_seo/templates/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3231 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/templates/default.html
--rw-r--r--   0 kapt      (1000) kapt      (1000)      665 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/django_check_seo/templates/element.html
--rw-r--r--   0 kapt      (1000) kapt      (1000)      603 2022-06-20 09:56:51.000000 django-check-seo-0.6.2/django_check_seo/urls.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2939 2023-04-18 13:32:21.000000 django-check-seo-0.6.2/django_check_seo/views.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.799523 django-check-seo-0.6.2/django_check_seo.egg-info/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6745 2023-04-19 13:25:48.000000 django-check-seo-0.6.2/django_check_seo.egg-info/PKG-INFO
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2490 2023-04-19 13:25:48.000000 django-check-seo-0.6.2/django_check_seo.egg-info/SOURCES.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)        1 2023-04-19 13:25:48.000000 django-check-seo-0.6.2/django_check_seo.egg-info/dependency_links.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)       49 2023-04-19 13:25:48.000000 django-check-seo-0.6.2/django_check_seo.egg-info/requires.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)       17 2023-04-19 13:25:48.000000 django-check-seo-0.6.2/django_check_seo.egg-info/top_level.txt
--rwxr-xr-x   0 kapt      (1000) kapt      (1000)     4701 2022-09-21 15:17:31.000000 django-check-seo-0.6.2/launch_tests.sh
--rw-r--r--   0 kapt      (1000) kapt      (1000)       94 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/pytest.ini
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1088 2023-04-19 13:25:48.803523 django-check-seo-0.6.2/setup.cfg
--rw-r--r--   0 kapt      (1000) kapt      (1000)       52 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/setup.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-19 13:25:48.803523 django-check-seo-0.6.2/tests/
--rw-r--r--   0 kapt      (1000) kapt      (1000)    16223 2021-09-09 16:31:52.000000 django-check-seo-0.6.2/tests/test_content_words_number.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     9522 2021-09-09 16:31:52.000000 django-check-seo-0.6.2/tests/test_description.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6045 2021-09-09 16:31:52.000000 django-check-seo-0.6.2/tests/test_h1.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6469 2021-09-09 16:31:52.000000 django-check-seo-0.6.2/tests/test_h2.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4439 2021-09-09 16:31:52.000000 django-check-seo-0.6.2/tests/test_images.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     5135 2021-09-09 16:31:52.000000 django-check-seo-0.6.2/tests/test_keyword_present_first_paragraph.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     5989 2021-09-09 16:31:58.000000 django-check-seo-0.6.2/tests/test_keyword_url.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2476 2021-09-09 16:31:52.000000 django-check-seo-0.6.2/tests/test_keywords.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6480 2021-09-09 16:31:52.000000 django-check-seo-0.6.2/tests/test_links.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     7288 2021-09-09 16:31:52.000000 django-check-seo-0.6.2/tests/test_title.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3672 2021-09-09 16:31:52.000000 django-check-seo-0.6.2/tests/test_url.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      618 2021-09-08 08:29:05.000000 django-check-seo-0.6.2/tests_settings.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.467699 django-check-seo-0.6.3/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       93 2023-07-28 13:59:47.000000 django-check-seo-0.6.3/.bumpversion.cfg
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      365 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/.coveragerc
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       74 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/.flake8
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.455699 django-check-seo-0.6.3/.github/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.459699 django-check-seo-0.6.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      834 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      595 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      130 2021-09-09 16:31:58.000000 django-check-seo-0.6.3/.gitignore
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      113 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/.isort.cfg
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      797 2022-06-14 09:16:04.000000 django-check-seo-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       78 2021-09-09 16:31:58.000000 django-check-seo-0.6.3/AUTHORS.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    17060 2023-07-28 13:59:50.000000 django-check-seo-0.6.3/CHANGELOG.rst
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1554 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/CONTRIBUTING.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    35149 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/LICENSE
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      220 2022-06-14 08:10:41.000000 django-check-seo-0.6.3/MANIFEST.in
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6759 2023-07-28 14:00:07.467699 django-check-seo-0.6.3/PKG-INFO
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     5675 2023-07-28 13:57:31.000000 django-check-seo-0.6.3/README.md
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.459699 django-check-seo-0.6.3/django_check_seo/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       66 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      181 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/apps.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.459699 django-check-seo-0.6.3/django_check_seo/checks/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/checks/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      320 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/checks/custom_list.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1778 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/checks/site.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.459699 django-check-seo-0.6.3/django_check_seo/checks_list/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      418 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/checks_list/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     7826 2023-03-03 15:45:59.000000 django-check-seo-0.6.3/django_check_seo/checks_list/check_description.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4001 2022-06-14 09:17:55.000000 django-check-seo-0.6.3/django_check_seo/checks_list/check_h1.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3793 2022-06-14 09:17:55.000000 django-check-seo-0.6.3/django_check_seo/checks_list/check_h2.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2914 2022-06-14 09:27:26.000000 django-check-seo-0.6.3/django_check_seo/checks_list/check_images.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3931 2022-06-14 09:17:55.000000 django-check-seo-0.6.3/django_check_seo/checks_list/check_keyword_url.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1928 2023-04-19 13:25:13.000000 django-check-seo-0.6.3/django_check_seo/checks_list/check_keywords.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4092 2022-06-14 09:17:55.000000 django-check-seo-0.6.3/django_check_seo/checks_list/check_links.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     5709 2022-06-14 09:17:55.000000 django-check-seo-0.6.3/django_check_seo/checks_list/check_title.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3367 2022-06-14 09:17:55.000000 django-check-seo-0.6.3/django_check_seo/checks_list/check_url.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2018 2022-06-14 09:17:55.000000 django-check-seo-0.6.3/django_check_seo/checks_list/content_words_number.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2453 2022-06-14 09:17:55.000000 django-check-seo-0.6.3/django_check_seo/checks_list/keyword_present_first_paragraph.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2052 2022-09-21 15:03:12.000000 django-check-seo-0.6.3/django_check_seo/checks_list/launch_checks.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      668 2023-03-03 15:45:59.000000 django-check-seo-0.6.3/django_check_seo/cms_toolbars.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.459699 django-check-seo-0.6.3/django_check_seo/conf/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/conf/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      815 2022-06-14 08:53:12.000000 django-check-seo-0.6.3/django_check_seo/conf/settings.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.455699 django-check-seo-0.6.3/django_check_seo/locale/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.455699 django-check-seo-0.6.3/django_check_seo/locale/fr/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.459699 django-check-seo-0.6.3/django_check_seo/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    16533 2022-06-14 09:38:51.000000 django-check-seo-0.6.3/django_check_seo/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    24514 2022-06-14 09:38:24.000000 django-check-seo-0.6.3/django_check_seo/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.459699 django-check-seo-0.6.3/django_check_seo/migrations/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/migrations/__init__.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.455699 django-check-seo-0.6.3/django_check_seo/static/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.463699 django-check-seo-0.6.3/django_check_seo/static/django-check-seo/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4734 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/static/django-check-seo/design.css
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.463699 django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    11358 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/LICENCE
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      139 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/NOTICE
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   164936 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/Roboto-Black.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   163448 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/Roboto-Bold.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   162636 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/Roboto-Light.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   158604 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/Roboto-Regular.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   122512 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/Roboto-Thin.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    15388 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/static/django-check-seo/logo-small.png
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   137074 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/static/django-check-seo/logo.png
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.463699 django-check-seo-0.6.3/django_check_seo/templates/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3246 2023-07-28 13:59:08.000000 django-check-seo-0.6.3/django_check_seo/templates/default.html
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      665 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/django_check_seo/templates/element.html
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      603 2022-06-20 09:56:51.000000 django-check-seo-0.6.3/django_check_seo/urls.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2939 2023-04-18 13:32:21.000000 django-check-seo-0.6.3/django_check_seo/views.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.459699 django-check-seo-0.6.3/django_check_seo.egg-info/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6759 2023-07-28 14:00:07.000000 django-check-seo-0.6.3/django_check_seo.egg-info/PKG-INFO
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2490 2023-07-28 14:00:07.000000 django-check-seo-0.6.3/django_check_seo.egg-info/SOURCES.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        1 2023-07-28 14:00:07.000000 django-check-seo-0.6.3/django_check_seo.egg-info/dependency_links.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       49 2023-07-28 14:00:07.000000 django-check-seo-0.6.3/django_check_seo.egg-info/requires.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       17 2023-07-28 14:00:07.000000 django-check-seo-0.6.3/django_check_seo.egg-info/top_level.txt
+-rwxr-xr-x   0 kapt      (1000) kapt      (1000)     4701 2022-09-21 15:17:31.000000 django-check-seo-0.6.3/launch_tests.sh
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       94 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/pytest.ini
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1088 2023-07-28 14:00:07.467699 django-check-seo-0.6.3/setup.cfg
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       52 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/setup.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-07-28 14:00:07.467699 django-check-seo-0.6.3/tests/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    16223 2021-09-09 16:31:52.000000 django-check-seo-0.6.3/tests/test_content_words_number.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     9522 2021-09-09 16:31:52.000000 django-check-seo-0.6.3/tests/test_description.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6045 2021-09-09 16:31:52.000000 django-check-seo-0.6.3/tests/test_h1.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6469 2021-09-09 16:31:52.000000 django-check-seo-0.6.3/tests/test_h2.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4439 2021-09-09 16:31:52.000000 django-check-seo-0.6.3/tests/test_images.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     5135 2021-09-09 16:31:52.000000 django-check-seo-0.6.3/tests/test_keyword_present_first_paragraph.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     5989 2021-09-09 16:31:58.000000 django-check-seo-0.6.3/tests/test_keyword_url.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2476 2021-09-09 16:31:52.000000 django-check-seo-0.6.3/tests/test_keywords.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6480 2021-09-09 16:31:52.000000 django-check-seo-0.6.3/tests/test_links.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     7288 2021-09-09 16:31:52.000000 django-check-seo-0.6.3/tests/test_title.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3672 2021-09-09 16:31:52.000000 django-check-seo-0.6.3/tests/test_url.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      618 2021-09-08 08:29:05.000000 django-check-seo-0.6.3/tests_settings.py
```

### Comparing `django-check-seo-0.6.2/.github/ISSUE_TEMPLATE/bug_report.md` & `django-check-seo-0.6.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/.github/ISSUE_TEMPLATE/feature_request.md` & `django-check-seo-0.6.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/.pre-commit-config.yaml` & `django-check-seo-0.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/CHANGELOG.rst` & `django-check-seo-0.6.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 Changelog
 =========
 
 
+v0.6.3 (2023-07-28)
+-------------------
+
+Bug fixes
+~~~~~~~~~
+- Fix #58 - remove unused load cms_tags [Corentin Bettiol]
+
+Documentation
+~~~~~~~~~~~~~
+- Update changelog [Corentin Bettiol]
+
+
 v0.6.2 (2023-04-19)
 -------------------
 
 Documentation
 ~~~~~~~~~~~~~
 - Update changelog [Corentin Bettiol]
```

### Comparing `django-check-seo-0.6.2/CONTRIBUTING.md` & `django-check-seo-0.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/LICENSE` & `django-check-seo-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/PKG-INFO` & `django-check-seo-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-check-seo
-Version: 0.6.2
+Version: 0.6.3
 Summary: Django Check SEO will check the SEO aspects of your site for you, and will provide advice in case of problems.
 Home-page: https://github.com/kapt-labs/django-check-seo
 Author: Dev Kapt
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.8
@@ -69,15 +69,15 @@
 
 ----
 
 # Misc
 
 This application needs `beautifulsoup4` (>=4.7.0) and `djangocms_page_meta` *(==0.8.5 if using django < 1.11)*. It may be used with or without `django-cms` (a django-check-seo button will appear in the topbar if you're using django-cms).
 
-If you're not using Django CMS, here's the link format to access your pages reports:
+If you're not using Django CMS (only Django), here's the link format to access your pages reports:
 
 ```
 https://example.com/django-check-seo/?page=/example-page/
   -> will check https://example.com/example-page/
 
 https://example.com/fr/django-check-seo/?page=/example-page/
   -> will check https://example.com/example-page/
```

### Comparing `django-check-seo-0.6.2/README.md` & `django-check-seo-0.6.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 ----
 
 # Misc
 
 This application needs `beautifulsoup4` (>=4.7.0) and `djangocms_page_meta` *(==0.8.5 if using django < 1.11)*. It may be used with or without `django-cms` (a django-check-seo button will appear in the topbar if you're using django-cms).
 
-If you're not using Django CMS, here's the link format to access your pages reports:
+If you're not using Django CMS (only Django), here's the link format to access your pages reports:
 
 ```
 https://example.com/django-check-seo/?page=/example-page/
   -> will check https://example.com/example-page/
 
 https://example.com/fr/django-check-seo/?page=/example-page/
   -> will check https://example.com/example-page/
```

### Comparing `django-check-seo-0.6.2/django_check_seo/checks/site.py` & `django-check-seo-0.6.3/django_check_seo/checks/site.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/checks_list/check_description.py` & `django-check-seo-0.6.3/django_check_seo/checks_list/check_description.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/checks_list/check_h1.py` & `django-check-seo-0.6.3/django_check_seo/checks_list/check_h1.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/checks_list/check_h2.py` & `django-check-seo-0.6.3/django_check_seo/checks_list/check_h2.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/checks_list/check_images.py` & `django-check-seo-0.6.3/django_check_seo/checks_list/check_images.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/checks_list/check_keyword_url.py` & `django-check-seo-0.6.3/django_check_seo/checks_list/check_keyword_url.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/checks_list/check_keywords.py` & `django-check-seo-0.6.3/django_check_seo/checks_list/check_keywords.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/checks_list/check_links.py` & `django-check-seo-0.6.3/django_check_seo/checks_list/check_links.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/checks_list/check_title.py` & `django-check-seo-0.6.3/django_check_seo/checks_list/check_title.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/checks_list/check_url.py` & `django-check-seo-0.6.3/django_check_seo/checks_list/check_url.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/checks_list/content_words_number.py` & `django-check-seo-0.6.3/django_check_seo/checks_list/content_words_number.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/checks_list/keyword_present_first_paragraph.py` & `django-check-seo-0.6.3/django_check_seo/checks_list/keyword_present_first_paragraph.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/checks_list/launch_checks.py` & `django-check-seo-0.6.3/django_check_seo/checks_list/launch_checks.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/cms_toolbars.py` & `django-check-seo-0.6.3/django_check_seo/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/conf/settings.py` & `django-check-seo-0.6.3/django_check_seo/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/locale/fr/LC_MESSAGES/django.mo` & `django-check-seo-0.6.3/django_check_seo/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/locale/fr/LC_MESSAGES/django.po` & `django-check-seo-0.6.3/django_check_seo/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/static/django-check-seo/design.css` & `django-check-seo-0.6.3/django_check_seo/static/django-check-seo/design.css`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/LICENCE` & `django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/LICENCE`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/Roboto-Black.ttf` & `django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/Roboto-Bold.ttf` & `django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/Roboto-Light.ttf` & `django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/Roboto-Regular.ttf` & `django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/static/django-check-seo/fonts/Roboto-Thin.ttf` & `django-check-seo-0.6.3/django_check_seo/static/django-check-seo/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/static/django-check-seo/logo-small.png` & `django-check-seo-0.6.3/django_check_seo/static/django-check-seo/logo-small.png`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/static/django-check-seo/logo.png` & `django-check-seo-0.6.3/django_check_seo/static/django-check-seo/logo.png`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/templates/default.html` & `django-check-seo-0.6.3/django_check_seo/templates/default.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% load cms_tags i18n static %}
+{% load i18n static %}
 <!DOCTYPE html>
 <html>
   <head>
     <meta charset="utf-8" />
     <title>Django check SEO</title>
     <link rel="stylesheet" type="text/css" href="{% static "django-check-seo/design.css" %}" />
   </head>
@@ -26,21 +26,21 @@
             {% autoescape off %}{{ nb_problems_warnings }}{% endautoescape %}
           </h2>
 
           <h3>{% trans "on the public page" %}</h3>
 
           <ul class="red-list list">
             {% for problem in problems %}
-                {% include "element.html" with element=problem %}
+              {% include "element.html" with element=problem %}
             {% endfor %}
           </ul>
 
           <ul class="yellow-list list">
             {% for warning in warnings %}
-                {% include "element.html" with element=warning %}
+              {% include "element.html" with element=warning %}
             {% endfor %}
           </ul>
 
           {% if success|length > 0 %}
             <hr />
             <ul class="green-list list">
               <h2>{%trans "Successful checks" %}</h2>
@@ -66,15 +66,17 @@
 
         <hr />
 
         <article>
           <h2>{% trans "Documentation" %}</h2>
 
           <p>
-            {% blocktrans %}The documentation is available via the <a href="https://github.com/kapt-labs/django-check-seo/wiki" target="_blank">project wiki</a>.{% endblocktrans %}
+            {% blocktrans %}
+              The documentation is available via the <a href="https://github.com/kapt-labs/django-check-seo/wiki" target="_blank">project wiki</a>.
+            {% endblocktrans %}
           </p>
         </article>
 
         <hr />
 
         <article class="not-important grey-list">
           <h2>Raw data</h2>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% load cms_tags i18n static %}
+{% load i18n static %}
 esign.css" %}" />
 ****** ogo-small.png" %}" alt="Django Check SEO" /> ******
     * {% trans "Keywords:" %}
     * {% if keywords|length > 0 %} {{ keywords|unordered_list }} {% else %}
     * {% trans "no keywords!" %}
     * {% endif %}
 ***** {% autoescape off %}{{ nb_problems_warnings }}{% endautoescape %} *****
@@ -20,15 +20,15 @@
 ***** {% trans "About" %} *****
 {% trans "The main objective of this application is to check the aspects of the
 web pages involved in SEO, to ensure that the page content will be correctly
 crawled by search engines." %}
 
 ===============================================================================
 ***** {% trans "Documentation" %} *****
-{% blocktrans %}The documentation is available via the project_wiki.{%
+{% blocktrans %} The documentation is available via the project_wiki. {%
 endblocktrans %}
 
 ===============================================================================
 ***** Raw data *****
 {% blocktrans %}Raw data are here for debug purposes. Join at least your
 settings if you're submitting a_new_issue.{% endblocktrans %}
   {% trans "See extracted html" %}
```

### Comparing `django-check-seo-0.6.2/django_check_seo/templates/element.html` & `django-check-seo-0.6.3/django_check_seo/templates/element.html`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/urls.py` & `django-check-seo-0.6.3/django_check_seo/urls.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo/views.py` & `django-check-seo-0.6.3/django_check_seo/views.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/django_check_seo.egg-info/PKG-INFO` & `django-check-seo-0.6.3/django_check_seo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-check-seo
-Version: 0.6.2
+Version: 0.6.3
 Summary: Django Check SEO will check the SEO aspects of your site for you, and will provide advice in case of problems.
 Home-page: https://github.com/kapt-labs/django-check-seo
 Author: Dev Kapt
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.8
@@ -69,15 +69,15 @@
 
 ----
 
 # Misc
 
 This application needs `beautifulsoup4` (>=4.7.0) and `djangocms_page_meta` *(==0.8.5 if using django < 1.11)*. It may be used with or without `django-cms` (a django-check-seo button will appear in the topbar if you're using django-cms).
 
-If you're not using Django CMS, here's the link format to access your pages reports:
+If you're not using Django CMS (only Django), here's the link format to access your pages reports:
 
 ```
 https://example.com/django-check-seo/?page=/example-page/
   -> will check https://example.com/example-page/
 
 https://example.com/fr/django-check-seo/?page=/example-page/
   -> will check https://example.com/example-page/
```

### Comparing `django-check-seo-0.6.2/django_check_seo.egg-info/SOURCES.txt` & `django-check-seo-0.6.3/django_check_seo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/launch_tests.sh` & `django-check-seo-0.6.3/launch_tests.sh`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/setup.cfg` & `django-check-seo-0.6.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-check-seo
-version = 0.6.2
+version = 0.6.3
 description = Django Check SEO will check the SEO aspects of your site for you, and will provide advice in case of problems.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kapt-labs/django-check-seo
 author = Dev Kapt
 author_email = dev@kapt.mobi
 classifiers =
```

### Comparing `django-check-seo-0.6.2/tests/test_content_words_number.py` & `django-check-seo-0.6.3/tests/test_content_words_number.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/tests/test_description.py` & `django-check-seo-0.6.3/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/tests/test_h1.py` & `django-check-seo-0.6.3/tests/test_h1.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/tests/test_h2.py` & `django-check-seo-0.6.3/tests/test_h2.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/tests/test_images.py` & `django-check-seo-0.6.3/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/tests/test_keyword_present_first_paragraph.py` & `django-check-seo-0.6.3/tests/test_keyword_present_first_paragraph.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/tests/test_keyword_url.py` & `django-check-seo-0.6.3/tests/test_keyword_url.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/tests/test_keywords.py` & `django-check-seo-0.6.3/tests/test_keywords.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/tests/test_links.py` & `django-check-seo-0.6.3/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/tests/test_title.py` & `django-check-seo-0.6.3/tests/test_title.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/tests/test_url.py` & `django-check-seo-0.6.3/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.2/tests_settings.py` & `django-check-seo-0.6.3/tests_settings.py`

 * *Files identical despite different names*

