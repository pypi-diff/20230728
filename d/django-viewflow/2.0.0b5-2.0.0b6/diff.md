# Comparing `tmp/django-viewflow-2.0.0b5.tar.gz` & `tmp/django-viewflow-2.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-viewflow-2.0.0b5.tar", last modified: Mon Jul 10 10:45:02 2023, max compression
+gzip compressed data, was "django-viewflow-2.0.0b6.tar", last modified: Fri Jul 28 07:56:12 2023, max compression
```

## Comparing `django-viewflow-2.0.0b5.tar` & `django-viewflow-2.0.0b6.tar`

### file list

```diff
@@ -1,328 +1,329 @@
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.895388 django-viewflow-2.0.0b5/
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    34520 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/LICENSE
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1340 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/LICENSE_EXCEPTION
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      193 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/MANIFEST.in
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1029 2023-07-10 10:45:02.895388 django-viewflow-2.0.0b5/PKG-INFO
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6963 2023-07-10 10:26:43.000000 django-viewflow-2.0.0b5/README.md
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.847388 django-viewflow-2.0.0b5/django_viewflow.egg-info/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1029 2023-07-10 10:45:02.000000 django-viewflow-2.0.0b5/django_viewflow.egg-info/PKG-INFO
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11669 2023-07-10 10:45:02.000000 django-viewflow-2.0.0b5/django_viewflow.egg-info/SOURCES.txt
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        1 2023-07-10 10:45:02.000000 django-viewflow-2.0.0b5/django_viewflow.egg-info/dependency_links.txt
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        1 2023-01-10 07:03:38.000000 django-viewflow-2.0.0b5/django_viewflow.egg-info/not-zip-safe
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       33 2023-07-10 10:45:02.000000 django-viewflow-2.0.0b5/django_viewflow.egg-info/requires.txt
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        9 2023-07-10 10:45:02.000000 django-viewflow-2.0.0b5/django_viewflow.egg-info/top_level.txt
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      228 2023-07-10 10:45:02.895388 django-viewflow-2.0.0b5/setup.cfg
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1405 2023-07-10 10:27:45.000000 django-viewflow-2.0.0b5/setup.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.847388 django-viewflow-2.0.0b5/viewflow/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1200 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      482 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/apps.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1737 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/conf.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.847388 django-viewflow-2.0.0b5/viewflow/contrib/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/__init__.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.847388 django-viewflow-2.0.0b5/viewflow/contrib/admin/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1263 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/admin/__init__.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      444 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/admin/apps.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    10383 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/auth.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/contrib/plotly/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      138 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/plotly/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2170 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/plotly/material.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2494 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/plotly/views.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2257 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/plotly/viewset.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4611 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fields.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/forms/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      753 2023-01-12 07:46:01.000000 django-viewflow-2.0.0b5/viewflow/forms/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    27485 2023-01-12 07:46:01.000000 django-viewflow-2.0.0b5/viewflow/forms/renderers.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/fsm/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      751 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     7886 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/admin.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    15456 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/base.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3001 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/chart.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      725 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/typing.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1568 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/views.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5438 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/viewset.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6787 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/jsonstore.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/de/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/de/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6147 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    19568 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/es/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/es/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9136 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    20862 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/fr/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9296 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    21031 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/it/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/it/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9466 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    21002 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/ja/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    10300 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/ja/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    21914 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/kk/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/kk/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      378 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/kk/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17712 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/kk/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/ko/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      373 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/ko/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17707 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/ko/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/pt/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      380 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17714 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/ru/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11819 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    23228 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/zh_Hans/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      373 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17707 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/zh_Hans/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/management/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2742 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/management/__init__.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.855388 django-viewflow-2.0.0b5/viewflow/management/commands/
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/management/commands/__init__.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2082 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/management/commands/flowexport.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2471 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/middleware.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/static/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/static/viewflow/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.855388 django-viewflow-2.0.0b5/viewflow/static/viewflow/css/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2598 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/css/perfect-scrollbar.css
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    19972 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/css/trix.css
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   460203 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/css/viewflow.min.css
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   220163 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/css/vis-network.min.css
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.859388 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   182028 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   155276 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   206260 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   173620 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   156236 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   135984 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   339600 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   215704 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3314 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons.css
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   164912 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   128352 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons.woff2
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.863388 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    86508 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64960 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    94048 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    72088 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    86184 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64740 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    91968 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    70360 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    85692 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64320 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    92864 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    70760 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    86444 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    65484 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    93228 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    71284 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    85876 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64632 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    91728 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    70280 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    84224 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    63048 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    90784 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    68328 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4173 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/roboto-fontface.css
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.867388 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1077522 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.eot
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1077336 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.otf
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1077336 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.ttf
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   718180 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   603192 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   213035 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/simple-icons.css
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   184911 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/simple-icons.min.css
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.867388 django-viewflow-2.0.0b5/viewflow/static/viewflow/img/
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1311 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/img/favicon.png
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2200 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/img/user.png
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.875388 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    19549 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/perfect-scrollbar.min.js
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    77830 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/perfect-scrollbar.min.js.map
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17674 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/smartcrop.js
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   229927 2023-01-27 12:19:41.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/trix.js
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   156812 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/turbo.es2017-umd.js
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   564585 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/viewflow.min.js
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1658508 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/viewflow.min.js.map
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   490205 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/vis-network.min.js
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  2010720 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/vis-network.min.js.map
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.875388 django-viewflow-2.0.0b5/viewflow/templates/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      672 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/400.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1183 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/403.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      695 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/404.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      832 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/500.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.875388 django-viewflow-2.0.0b5/viewflow/templates/admin/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      151 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_change_form.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      637 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_change_form_object_tools.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1206 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_change_list.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2998 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_transition_form.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/templates/formtools/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.875388 django-viewflow-2.0.0b5/viewflow/templates/formtools/wizard/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      794 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/formtools/wizard/wizard_form.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.875388 django-viewflow-2.0.0b5/viewflow/templates/registration/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      757 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/logged_out.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1638 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/login.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1653 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/password_change_done.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2097 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/password_change_form.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      586 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_complete.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      941 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      795 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_done.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      975 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_form.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3737 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/profile.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      926 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/provider_list.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.879388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1776 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/base.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1211 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/base_lockscreen.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5946 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/base_page.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.879388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.879388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/import_export/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2571 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/import_export/export_action.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/import_export/import_action.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1061 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/plotly.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      831 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/swagger.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.879388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1938 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/app_menu.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2467 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/list_bulk_actions.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      703 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/list_filter.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1401 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/list_pagination.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1860 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/object_detail_card.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1535 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/site_menu.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      261 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/snackbar.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      851 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/view_action_menu.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      358 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/viewflow_css.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      326 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/viewflow_js.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.879388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/material/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1864 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/material/circular_progress.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.879388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2787 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/confirm_delete.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3167 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/delete_action.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      523 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/detail.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3137 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/form.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6184 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/list.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1210 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/transition.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.883388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2768 2023-01-12 07:46:01.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/assign.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       40 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/base_page.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      339 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/celery_task_detail.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1738 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/flow_menu.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2509 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/graph.bpmn
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4224 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/graph.svg
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4340 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_cancel.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8037 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_dashboard.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1288 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_data.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3696 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_detail.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      633 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_list.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       41 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_tasks_list.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2716 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/start.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3339 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1104 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_assign.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2899 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_base.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      736 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_cancel.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2777 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_detail.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      633 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_list.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      736 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_revive.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      740 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_unassign.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      732 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_undo.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2847 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/tasks_assign.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2851 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/tasks_unassign.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1371 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/workflow_menu.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1987 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/workflow_tasks_list.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.883388 django-viewflow-2.0.0b5/viewflow/templatetags/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templatetags/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      429 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templatetags/fsm.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8866 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templatetags/viewflow.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1470 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templatetags/workflow.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1811 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/this_object.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.883388 django-viewflow-2.0.0b5/viewflow/urls/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1800 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/urls/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11582 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/urls/base.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11203 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/urls/model.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5347 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/urls/sites.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     7314 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/utils.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.883388 django-viewflow-2.0.0b5/viewflow/views/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      707 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3991 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/actions.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1916 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/base.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3935 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/create.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3417 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/delete.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3465 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/detail.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1853 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/filters.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    15971 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/list.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3844 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/search.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4714 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/update.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.887388 django-viewflow-2.0.0b5/viewflow/workflow/
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      438 2022-07-13 10:36:23.000000 django-viewflow-2.0.0b5/viewflow/workflow/__init__.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6067 2023-04-27 11:52:17.000000 django-viewflow-2.0.0b5/viewflow/workflow/activation.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2417 2023-03-17 09:25:31.000000 django-viewflow-2.0.0b5/viewflow/workflow/admin.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      344 2023-04-24 08:09:15.000000 django-viewflow-2.0.0b5/viewflow/workflow/apps.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    13505 2023-02-24 12:01:50.000000 django-viewflow-2.0.0b5/viewflow/workflow/base.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    20092 2022-01-31 10:53:07.000000 django-viewflow-2.0.0b5/viewflow/workflow/chart.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1540 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b5/viewflow/workflow/context.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      142 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b5/viewflow/workflow/exceptions.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4431 2023-07-04 09:48:28.000000 django-viewflow-2.0.0b5/viewflow/workflow/fields.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.887388 django-viewflow-2.0.0b5/viewflow/workflow/flow/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      738 2023-04-17 08:01:45.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3994 2022-12-08 11:16:57.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/mixins.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6309 2023-04-17 08:01:26.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/nodes.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3307 2023-02-09 10:21:20.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/utils.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.887388 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1676 2022-12-08 09:41:38.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6320 2022-12-08 09:41:24.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/actions.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      903 2022-08-08 11:14:26.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/chart.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1254 2022-05-18 09:25:12.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/create.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5113 2023-07-10 06:38:27.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/dashboard.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3697 2022-12-27 05:50:40.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/detail.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2958 2021-12-14 11:27:01.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/filters.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6179 2023-05-24 07:46:01.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/list.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3642 2023-05-24 07:43:27.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/mixins.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1469 2022-07-11 07:29:24.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/update.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    13545 2023-07-07 09:40:27.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/viewset.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2912 2021-12-13 03:06:49.000000 django-viewflow-2.0.0b5/viewflow/workflow/lock.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9876 2023-07-07 10:21:50.000000 django-viewflow-2.0.0b5/viewflow/workflow/managers.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.891388 django-viewflow-2.0.0b5/viewflow/workflow/migrations/
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2444 2020-05-21 12:16:30.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0001_initial.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      956 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0002_fsmchange.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      426 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0003_task_owner_permission_change.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      658 2020-05-21 12:15:16.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0004_extend_fields_length.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      260 2020-05-21 12:27:44.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0004_subprocess.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      293 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0005_merge.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      397 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0005_rename_flowcls.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4169 2020-05-21 12:17:10.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0006_i18n.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      282 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0006_merge.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      724 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0007_owner_permission_obj.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      409 2019-10-28 09:00:22.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0007_task_assigned.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1534 2020-05-21 12:16:55.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0008_jsonfield_and_artifact.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      287 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0008_merge.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      266 2019-10-28 12:09:38.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0009_merge.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2683 2023-04-24 08:20:10.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0010_viewflow20.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      747 2023-07-05 11:28:45.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0011_alter_task_created_and_more.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8481 2023-07-06 09:15:24.000000 django-viewflow-2.0.0b5/viewflow/workflow/models.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.895388 django-viewflow-2.0.0b5/viewflow/workflow/nodes/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1119 2023-04-28 05:08:57.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2253 2023-04-27 11:59:45.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/end.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1816 2023-04-25 06:37:06.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/func.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2808 2023-04-27 10:58:01.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/handle.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1972 2023-07-04 09:24:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/if_gate.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2534 2023-05-09 06:58:04.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/job.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5061 2023-04-03 08:08:46.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/join.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3931 2023-04-03 09:48:31.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/mixins.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      933 2022-12-08 08:46:15.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/obsolete.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5657 2023-04-27 11:59:12.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/split.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5519 2023-04-27 10:05:03.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/start.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4543 2023-07-04 11:54:12.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/subprocess.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2548 2022-12-08 08:49:59.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/switch.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8082 2023-04-25 06:27:17.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/view.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      372 2023-04-18 09:17:56.000000 django-viewflow-2.0.0b5/viewflow/workflow/signals.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      843 2020-06-13 08:59:51.000000 django-viewflow-2.0.0b5/viewflow/workflow/status.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1752 2020-05-18 11:34:55.000000 django-viewflow-2.0.0b5/viewflow/workflow/token.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1226 2023-07-07 09:48:41.000000 django-viewflow-2.0.0b5/viewflow/workflow/utils.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.439328 django-viewflow-2.0.0b6/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    34520 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/LICENSE
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1340 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/LICENSE_EXCEPTION
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      193 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/MANIFEST.in
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1029 2023-07-28 07:56:12.439328 django-viewflow-2.0.0b6/PKG-INFO
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     7023 2023-07-28 07:38:32.000000 django-viewflow-2.0.0b6/README.md
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.367324 django-viewflow-2.0.0b6/django_viewflow.egg-info/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1029 2023-07-28 07:56:12.000000 django-viewflow-2.0.0b6/django_viewflow.egg-info/PKG-INFO
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11721 2023-07-28 07:56:12.000000 django-viewflow-2.0.0b6/django_viewflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        1 2023-07-28 07:56:12.000000 django-viewflow-2.0.0b6/django_viewflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        1 2023-01-10 07:03:38.000000 django-viewflow-2.0.0b6/django_viewflow.egg-info/not-zip-safe
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       33 2023-07-28 07:56:12.000000 django-viewflow-2.0.0b6/django_viewflow.egg-info/requires.txt
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        9 2023-07-28 07:56:12.000000 django-viewflow-2.0.0b6/django_viewflow.egg-info/top_level.txt
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      228 2023-07-28 07:56:12.439328 django-viewflow-2.0.0b6/setup.cfg
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1405 2023-07-28 07:38:46.000000 django-viewflow-2.0.0b6/setup.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.371324 django-viewflow-2.0.0b6/viewflow/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1200 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      482 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/apps.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1737 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/conf.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.371324 django-viewflow-2.0.0b6/viewflow/contrib/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/contrib/__init__.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.371324 django-viewflow-2.0.0b6/viewflow/contrib/admin/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1263 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/contrib/admin/__init__.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      444 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/contrib/admin/apps.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    10383 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/contrib/auth.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.371324 django-viewflow-2.0.0b6/viewflow/contrib/plotly/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      138 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/contrib/plotly/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2170 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/contrib/plotly/material.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2494 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/contrib/plotly/views.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2257 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/contrib/plotly/viewset.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4611 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/fields.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.371324 django-viewflow-2.0.0b6/viewflow/forms/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      753 2023-01-12 07:46:01.000000 django-viewflow-2.0.0b6/viewflow/forms/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    27485 2023-01-12 07:46:01.000000 django-viewflow-2.0.0b6/viewflow/forms/renderers.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.375324 django-viewflow-2.0.0b6/viewflow/fsm/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      751 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/fsm/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     7886 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/fsm/admin.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    15456 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/fsm/base.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3001 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/fsm/chart.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      725 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/fsm/typing.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1568 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/fsm/views.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5438 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/fsm/viewset.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6787 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/jsonstore.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.359323 django-viewflow-2.0.0b6/viewflow/locale/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.355323 django-viewflow-2.0.0b6/viewflow/locale/de/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.375324 django-viewflow-2.0.0b6/viewflow/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6147 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    19568 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.355323 django-viewflow-2.0.0b6/viewflow/locale/es/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.375324 django-viewflow-2.0.0b6/viewflow/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9136 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    20862 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.355323 django-viewflow-2.0.0b6/viewflow/locale/fr/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.379325 django-viewflow-2.0.0b6/viewflow/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9296 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    21031 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.355323 django-viewflow-2.0.0b6/viewflow/locale/it/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.379325 django-viewflow-2.0.0b6/viewflow/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9466 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    21002 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.355323 django-viewflow-2.0.0b6/viewflow/locale/ja/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.379325 django-viewflow-2.0.0b6/viewflow/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    10300 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    21914 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.359323 django-viewflow-2.0.0b6/viewflow/locale/kk/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.379325 django-viewflow-2.0.0b6/viewflow/locale/kk/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      378 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/kk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17712 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/kk/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.359323 django-viewflow-2.0.0b6/viewflow/locale/ko/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.379325 django-viewflow-2.0.0b6/viewflow/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      373 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17707 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.359323 django-viewflow-2.0.0b6/viewflow/locale/pt/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.383325 django-viewflow-2.0.0b6/viewflow/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      380 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17714 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.359323 django-viewflow-2.0.0b6/viewflow/locale/ru/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.383325 django-viewflow-2.0.0b6/viewflow/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11819 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    23228 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.359323 django-viewflow-2.0.0b6/viewflow/locale/zh_Hans/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.383325 django-viewflow-2.0.0b6/viewflow/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      373 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17707 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/locale/zh_Hans/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.383325 django-viewflow-2.0.0b6/viewflow/management/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2742 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/management/__init__.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.383325 django-viewflow-2.0.0b6/viewflow/management/commands/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/management/commands/__init__.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2082 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/management/commands/flowexport.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2471 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/middleware.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.359323 django-viewflow-2.0.0b6/viewflow/static/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.359323 django-viewflow-2.0.0b6/viewflow/static/viewflow/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.383325 django-viewflow-2.0.0b6/viewflow/static/viewflow/css/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2598 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/css/perfect-scrollbar.css
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    19972 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/css/trix.css
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   460203 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/css/viewflow.min.css
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   220163 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/css/vis-network.min.css
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.359323 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.391325 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   182028 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   155276 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   206260 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   173620 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   156236 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   135984 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   339600 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   215704 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3314 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons.css
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   164912 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   128352 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons.woff2
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.399325 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    86508 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64960 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    94048 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    72088 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    86184 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64740 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    91968 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    70360 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    85692 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64320 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    92864 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    70760 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    86444 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    65484 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    93228 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    71284 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    85876 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64632 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    91728 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    70280 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    84224 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    63048 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    90784 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    68328 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4173 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/roboto-fontface.css
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.407326 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1077522 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.eot
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1077336 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.otf
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1077336 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.ttf
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   718180 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   603192 2023-07-28 07:51:10.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   213035 2023-07-28 07:51:10.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/simple-icons.css
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   184911 2023-07-28 07:51:10.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/simple-icons.min.css
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.407326 django-viewflow-2.0.0b6/viewflow/static/viewflow/img/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1311 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/img/favicon.png
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2200 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/img/user.png
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.411326 django-viewflow-2.0.0b6/viewflow/static/viewflow/js/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    19549 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/js/perfect-scrollbar.min.js
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    77830 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/js/perfect-scrollbar.min.js.map
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17674 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/js/smartcrop.js
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   229927 2023-01-27 12:19:41.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/js/trix.js
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   156812 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/js/turbo.es2017-umd.js
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   564585 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/js/viewflow.min.js
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1658508 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/js/viewflow.min.js.map
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   490205 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/js/vis-network.min.js
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  2010720 2023-07-28 07:51:09.000000 django-viewflow-2.0.0b6/viewflow/static/viewflow/js/vis-network.min.js.map
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.415326 django-viewflow-2.0.0b6/viewflow/templates/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      672 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/400.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1183 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/403.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      695 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/404.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      832 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/500.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.415326 django-viewflow-2.0.0b6/viewflow/templates/admin/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      151 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/admin/fsm_change_form.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      637 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/admin/fsm_change_form_object_tools.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1206 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/admin/fsm_change_list.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2998 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/admin/fsm_transition_form.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.359323 django-viewflow-2.0.0b6/viewflow/templates/formtools/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.415326 django-viewflow-2.0.0b6/viewflow/templates/formtools/wizard/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      794 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/formtools/wizard/wizard_form.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.419327 django-viewflow-2.0.0b6/viewflow/templates/registration/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      757 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/registration/logged_out.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1638 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/registration/login.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1653 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/registration/password_change_done.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2165 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/registration/password_change_form.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      586 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1009 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      795 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/registration/password_reset_done.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1043 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/registration/password_reset_form.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3805 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/registration/profile.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      926 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/registration/provider_list.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.419327 django-viewflow-2.0.0b6/viewflow/templates/viewflow/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1776 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/base.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1211 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/base_lockscreen.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5946 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/base_page.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.419327 django-viewflow-2.0.0b6/viewflow/templates/viewflow/contrib/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.419327 django-viewflow-2.0.0b6/viewflow/templates/viewflow/contrib/import_export/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2639 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/contrib/import_export/export_action.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/contrib/import_export/import_action.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1061 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/contrib/plotly.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      831 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/contrib/swagger.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.423327 django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1938 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/app_menu.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2535 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/list_bulk_actions.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      771 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/list_filter.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1401 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/list_pagination.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1860 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/object_detail_card.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1535 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/site_menu.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      261 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/snackbar.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      851 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/view_action_menu.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      358 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/viewflow_css.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      326 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/viewflow_js.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.423327 django-viewflow-2.0.0b6/viewflow/templates/viewflow/material/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1864 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/material/circular_progress.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.423327 django-viewflow-2.0.0b6/viewflow/templates/viewflow/views/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2855 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/views/confirm_delete.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3235 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/views/delete_action.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      523 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/views/detail.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3137 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/views/form.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6314 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/views/list.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1210 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/views/transition.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.427327 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2768 2023-01-12 07:46:01.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/assign.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       40 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/base_page.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      339 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/celery_task_detail.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1738 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/flow_menu.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2509 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/graph.bpmn
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4224 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/graph.svg
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4408 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/process_cancel.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8037 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/process_dashboard.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1288 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/process_data.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3716 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/process_detail.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      633 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/process_list.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       41 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/process_tasks_list.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2716 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/start.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3359 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1104 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_assign.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3265 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_base.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      736 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_cancel.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      681 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_data.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2777 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_detail.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      633 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_list.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      736 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_revive.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      740 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_unassign.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      732 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_undo.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2915 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/tasks_assign.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2919 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/tasks_unassign.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1371 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/workflow_menu.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1987 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/workflow_tasks_list.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.427327 django-viewflow-2.0.0b6/viewflow/templatetags/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templatetags/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      429 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templatetags/fsm.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8866 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templatetags/viewflow.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2407 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/templatetags/workflow.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1811 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/this_object.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.427327 django-viewflow-2.0.0b6/viewflow/urls/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1800 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/urls/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11582 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/urls/base.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11203 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/urls/model.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5347 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/urls/sites.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     7314 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/utils.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.431327 django-viewflow-2.0.0b6/viewflow/views/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      707 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/views/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3991 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/views/actions.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1916 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/views/base.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3935 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/views/create.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3417 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/views/delete.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3465 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/views/detail.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1853 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/views/filters.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    15971 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/views/list.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3844 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/views/search.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4714 2023-07-28 07:50:46.000000 django-viewflow-2.0.0b6/viewflow/views/update.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.431327 django-viewflow-2.0.0b6/viewflow/workflow/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      438 2022-07-13 10:36:23.000000 django-viewflow-2.0.0b6/viewflow/workflow/__init__.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6067 2023-04-27 11:52:17.000000 django-viewflow-2.0.0b6/viewflow/workflow/activation.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2417 2023-03-17 09:25:31.000000 django-viewflow-2.0.0b6/viewflow/workflow/admin.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      344 2023-04-24 08:09:15.000000 django-viewflow-2.0.0b6/viewflow/workflow/apps.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    13505 2023-02-24 12:01:50.000000 django-viewflow-2.0.0b6/viewflow/workflow/base.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    20092 2022-01-31 10:53:07.000000 django-viewflow-2.0.0b6/viewflow/workflow/chart.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1540 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b6/viewflow/workflow/context.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      142 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b6/viewflow/workflow/exceptions.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4431 2023-07-04 09:48:28.000000 django-viewflow-2.0.0b6/viewflow/workflow/fields.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.431327 django-viewflow-2.0.0b6/viewflow/workflow/flow/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      738 2023-04-17 08:01:45.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3994 2022-12-08 11:16:57.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/mixins.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6309 2023-04-17 08:01:26.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/nodes.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3307 2023-02-09 10:21:20.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/utils.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.435328 django-viewflow-2.0.0b6/viewflow/workflow/flow/views/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1676 2022-12-08 09:41:38.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/views/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6320 2022-12-08 09:41:24.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/views/actions.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      903 2022-08-08 11:14:26.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/views/chart.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1254 2022-05-18 09:25:12.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/views/create.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5113 2023-07-10 06:38:27.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/views/dashboard.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3697 2022-12-27 05:50:40.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/views/detail.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2958 2021-12-14 11:27:01.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/views/filters.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6321 2023-07-11 05:09:38.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/views/list.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3642 2023-05-24 07:43:27.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/views/mixins.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1469 2022-07-11 07:29:24.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/views/update.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    13545 2023-07-07 09:40:27.000000 django-viewflow-2.0.0b6/viewflow/workflow/flow/viewset.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2912 2021-12-13 03:06:49.000000 django-viewflow-2.0.0b6/viewflow/workflow/lock.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9876 2023-07-07 10:21:50.000000 django-viewflow-2.0.0b6/viewflow/workflow/managers.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.439328 django-viewflow-2.0.0b6/viewflow/workflow/migrations/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2444 2020-05-21 12:16:30.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0001_initial.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      956 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0002_fsmchange.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      426 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0003_task_owner_permission_change.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      658 2020-05-21 12:15:16.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0004_extend_fields_length.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      260 2020-05-21 12:27:44.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0004_subprocess.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      293 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0005_merge.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      397 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0005_rename_flowcls.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4169 2020-05-21 12:17:10.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0006_i18n.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      282 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0006_merge.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      724 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0007_owner_permission_obj.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      409 2019-10-28 09:00:22.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0007_task_assigned.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1534 2020-05-21 12:16:55.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0008_jsonfield_and_artifact.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      287 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0008_merge.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      266 2019-10-28 12:09:38.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0009_merge.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2683 2023-04-24 08:20:10.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0010_viewflow20.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      747 2023-07-05 11:28:45.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/0011_alter_task_created_and_more.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b6/viewflow/workflow/migrations/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8481 2023-07-06 09:15:24.000000 django-viewflow-2.0.0b6/viewflow/workflow/models.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-28 07:56:12.439328 django-viewflow-2.0.0b6/viewflow/workflow/nodes/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1119 2023-04-28 05:08:57.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2253 2023-04-27 11:59:45.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/end.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1816 2023-04-25 06:37:06.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/func.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2808 2023-04-27 10:58:01.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/handle.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1972 2023-07-04 09:24:08.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/if_gate.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2534 2023-05-09 06:58:04.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/job.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5061 2023-04-03 08:08:46.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/join.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3931 2023-04-03 09:48:31.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/mixins.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      933 2022-12-08 08:46:15.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/obsolete.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5657 2023-04-27 11:59:12.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/split.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5519 2023-04-27 10:05:03.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/start.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4543 2023-07-04 11:54:12.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/subprocess.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2548 2022-12-08 08:49:59.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/switch.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8082 2023-04-25 06:27:17.000000 django-viewflow-2.0.0b6/viewflow/workflow/nodes/view.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      372 2023-04-18 09:17:56.000000 django-viewflow-2.0.0b6/viewflow/workflow/signals.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      843 2020-06-13 08:59:51.000000 django-viewflow-2.0.0b6/viewflow/workflow/status.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1752 2020-05-18 11:34:55.000000 django-viewflow-2.0.0b6/viewflow/workflow/token.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1226 2023-07-07 09:48:41.000000 django-viewflow-2.0.0b6/viewflow/workflow/utils.py
```

### Comparing `django-viewflow-2.0.0b5/LICENSE` & `django-viewflow-2.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/LICENSE_EXCEPTION` & `django-viewflow-2.0.0b6/LICENSE_EXCEPTION`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/PKG-INFO` & `django-viewflow-2.0.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-viewflow
-Version: 2.0.0b5
+Version: 2.0.0b6
 Summary: Reusable library to build business applications fast
 Home-page: UNKNOWN
 Author: Mikhail Podgurskiy
 Author-email: kmmbvnr@gmail.com
 License: AGPL
 Description: UNKNOWN
 Keywords: django,admin,workflow,fsm,bpm,bpmn
```

### Comparing `django-viewflow-2.0.0b5/README.md` & `django-viewflow-2.0.0b6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,16 @@
     from viewflow import jsonstore
     from viewflow.workflow.models import Process
 
     class PizzaOrder(Process):
         customer_name = jsonstore.CharField(max_length=250)
         address = jsonstore.TextField()
         toppings = jsonstore.TextField()
-        tips_received = json_Store.IntegerField(default=0)
+        tips_received = jsonstore.IntegerField(default=0)
+        baking_time = jsonstore.IntegerField(default=10)
 
         class Meta:
             proxy = True
 ```
 
 2. Create a new flow definition file flows.py
 
@@ -83,14 +84,15 @@
 data from PizzaOrder:
 
 ```python
 
     from viewflow import this
     from viewflow.workflow import flow
     from viewflow.workflow.flow.views import CreateProcessView, UpdateProcessView
+    from .models import PizzaOrder
 
     class PizzaFlow(flow.Flow):
         process_class = PizzaOrder
 
         start = flow.Start(
             CreateProcessView.as_view(
                 fields=["customer_name", "address", "toppings"]
@@ -111,16 +113,18 @@
 3. Add the flow to your URL configuration:
 
 Finally, add the PizzaFlow to your URL configuration. You can use the Site and
 FlowAppViewset classes to register your workflow with the pre-built frontend.
 
 ```python
 
+    from django.urls import path
     from viewflow.contrib.auth import AuthViewset
     from viewflow.urls import Application, Site
+    from viewflow.workflow.flow import FlowAppViewset
     from my_pizza.flows import PizzaFlow
 
     site = Site(
         title="Pizza Flow Demo",
         viewsets=[
             FlowAppViewset(PizzaFlow, icon="local_pizza"),
         ]
@@ -129,17 +133,17 @@
     urlpatterns = [
         path("accounts/", AuthViewset().urls),
         path("", site.urls),
     ]
 
 ```
 
-4. Run migrations and access the workflow through the pre-built frontend.
+4. Make and run migrations and access the workflow through the pre-built frontend.
 
-Run migrations to create the necessary database tables, then start your Django
+Make and run migrations to create the necessary database tables, then start your Django
 server and access the workflow through the pre-built frontend. You should be
 able to create and track pizza orders with the workflow.
 
 ## Documentation
 
 Viewflow's documentation for the latest version is available at
 http://docs.viewflow.io/
@@ -175,22 +179,18 @@
 
 Viewflow PRO has a commercial-friendly license allowing private forks and
 modifications of Viewflow. You can find the commercial license terms in
 [COMM-LICENSE](./COMM-LICENSE).
 
 ## Changelog
 
-2.0.0.b5 2023-07-10
+2.0.0.b6 2023-07-28
 -------------------
 
-- Alow attach layout to forms in default form rendering template
-- Fix subprocess node activation
-- Added db indexes for workflow models
-- Improve workflow REST API support
-
+- Fix label for File and Image fields
 
 
 [build]: https://img.shields.io/github/actions/workflow/status/viewflow/viewflow/django.yml?branch=main
 [coverage]: https://img.shields.io/coveralls/github/viewflow/viewflow/v2
 [travis-svg]: https://travis-ci.org/viewflow/viewflow.svg
 [travis]: https://travis-ci.org/viewflow/viewflow
 [pypi]: https://pypi.org/project/django-viewflow/
```

### Comparing `django-viewflow-2.0.0b5/django_viewflow.egg-info/PKG-INFO` & `django-viewflow-2.0.0b6/django_viewflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-viewflow
-Version: 2.0.0b5
+Version: 2.0.0b6
 Summary: Reusable library to build business applications fast
 Home-page: UNKNOWN
 Author: Mikhail Podgurskiy
 Author-email: kmmbvnr@gmail.com
 License: AGPL
 Description: UNKNOWN
 Keywords: django,admin,workflow,fsm,bpm,bpmn
```

### Comparing `django-viewflow-2.0.0b5/django_viewflow.egg-info/SOURCES.txt` & `django-viewflow-2.0.0b6/django_viewflow.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,15 @@
 viewflow/templates/viewflow/workflow/process_list.html
 viewflow/templates/viewflow/workflow/process_tasks_list.html
 viewflow/templates/viewflow/workflow/start.html
 viewflow/templates/viewflow/workflow/task.html
 viewflow/templates/viewflow/workflow/task_assign.html
 viewflow/templates/viewflow/workflow/task_base.html
 viewflow/templates/viewflow/workflow/task_cancel.html
+viewflow/templates/viewflow/workflow/task_data.html
 viewflow/templates/viewflow/workflow/task_detail.html
 viewflow/templates/viewflow/workflow/task_list.html
 viewflow/templates/viewflow/workflow/task_revive.html
 viewflow/templates/viewflow/workflow/task_unassign.html
 viewflow/templates/viewflow/workflow/task_undo.html
 viewflow/templates/viewflow/workflow/tasks_assign.html
 viewflow/templates/viewflow/workflow/tasks_unassign.html
```

### Comparing `django-viewflow-2.0.0b5/setup.py` & `django-viewflow-2.0.0b6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 README = open("README.md", "r", encoding="utf-8").read()
 
 setuptools.setup(
     name="django-viewflow",
-    version="2.0.0b5",
+    version="2.0.0b6",
     author_email="kmmbvnr@gmail.com",
     author="Mikhail Podgurskiy",
     description="Reusable library to build business applications fast",
     include_package_data=True,
     keywords=["django", "admin", "workflow", "fsm", "bpm", "bpmn"],
     license="AGPL",
     # long_description_content_type="text/markdown",
```

### Comparing `django-viewflow-2.0.0b5/viewflow/__init__.py` & `django-viewflow-2.0.0b6/viewflow/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/conf.py` & `django-viewflow-2.0.0b6/viewflow/conf.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/contrib/admin/__init__.py` & `django-viewflow-2.0.0b6/viewflow/contrib/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/contrib/auth.py` & `django-viewflow-2.0.0b6/viewflow/contrib/auth.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/contrib/plotly/material.py` & `django-viewflow-2.0.0b6/viewflow/contrib/plotly/material.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/contrib/plotly/views.py` & `django-viewflow-2.0.0b6/viewflow/contrib/plotly/views.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/contrib/plotly/viewset.py` & `django-viewflow-2.0.0b6/viewflow/contrib/plotly/viewset.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/fields.py` & `django-viewflow-2.0.0b6/viewflow/fields.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/forms/__init__.py` & `django-viewflow-2.0.0b6/viewflow/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/forms/renderers.py` & `django-viewflow-2.0.0b6/viewflow/forms/renderers.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/fsm/__init__.py` & `django-viewflow-2.0.0b6/viewflow/fsm/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/fsm/admin.py` & `django-viewflow-2.0.0b6/viewflow/fsm/admin.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/fsm/base.py` & `django-viewflow-2.0.0b6/viewflow/fsm/base.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/fsm/chart.py` & `django-viewflow-2.0.0b6/viewflow/fsm/chart.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/fsm/typing.py` & `django-viewflow-2.0.0b6/viewflow/fsm/typing.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/fsm/views.py` & `django-viewflow-2.0.0b6/viewflow/fsm/views.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/fsm/viewset.py` & `django-viewflow-2.0.0b6/viewflow/fsm/viewset.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/jsonstore.py` & `django-viewflow-2.0.0b6/viewflow/jsonstore.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/de/LC_MESSAGES/django.mo` & `django-viewflow-2.0.0b6/viewflow/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/de/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b6/viewflow/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/es/LC_MESSAGES/django.mo` & `django-viewflow-2.0.0b6/viewflow/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/es/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b6/viewflow/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/fr/LC_MESSAGES/django.mo` & `django-viewflow-2.0.0b6/viewflow/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/fr/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b6/viewflow/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/it/LC_MESSAGES/django.mo` & `django-viewflow-2.0.0b6/viewflow/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/it/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b6/viewflow/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/ja/LC_MESSAGES/django.mo` & `django-viewflow-2.0.0b6/viewflow/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/ja/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b6/viewflow/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/kk/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b6/viewflow/locale/kk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/ko/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b6/viewflow/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/pt/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b6/viewflow/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/ru/LC_MESSAGES/django.mo` & `django-viewflow-2.0.0b6/viewflow/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/ru/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b6/viewflow/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/locale/zh_Hans/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b6/viewflow/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/management/__init__.py` & `django-viewflow-2.0.0b6/viewflow/management/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/management/commands/flowexport.py` & `django-viewflow-2.0.0b6/viewflow/management/commands/flowexport.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/middleware.py` & `django-viewflow-2.0.0b6/viewflow/middleware.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/css/perfect-scrollbar.css` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/css/perfect-scrollbar.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/css/trix.css` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/css/trix.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/css/viewflow.min.css` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/css/viewflow.min.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/css/vis-network.min.css` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/css/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons.css` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/material-icons/material-icons.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/roboto-fontface.css` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/roboto/roboto-fontface.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.eot` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.eot`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.otf` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.otf`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.ttf` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.ttf`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff2` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/simple-icons.css` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/simple-icons.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/simple-icons.min.css` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/fonts/simple-icons/simple-icons.min.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/img/favicon.png` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/img/favicon.png`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/img/user.png` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/img/user.png`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/perfect-scrollbar.min.js` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/js/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/perfect-scrollbar.min.js.map` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/js/perfect-scrollbar.min.js.map`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/smartcrop.js` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/js/smartcrop.js`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/trix.js` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/js/trix.js`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/turbo.es2017-umd.js` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/js/turbo.es2017-umd.js`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/viewflow.min.js` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/js/viewflow.min.js`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/viewflow.min.js.map` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/js/viewflow.min.js.map`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/vis-network.min.js` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/js/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/vis-network.min.js.map` & `django-viewflow-2.0.0b6/viewflow/static/viewflow/js/vis-network.min.js.map`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/400.html` & `django-viewflow-2.0.0b6/viewflow/templates/400.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/403.html` & `django-viewflow-2.0.0b6/viewflow/templates/403.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/404.html` & `django-viewflow-2.0.0b6/viewflow/templates/404.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/500.html` & `django-viewflow-2.0.0b6/viewflow/templates/500.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_change_form_object_tools.html` & `django-viewflow-2.0.0b6/viewflow/templates/admin/fsm_change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_change_list.html` & `django-viewflow-2.0.0b6/viewflow/templates/admin/fsm_change_list.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_transition_form.html` & `django-viewflow-2.0.0b6/viewflow/templates/admin/fsm_transition_form.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/formtools/wizard/wizard_form.html` & `django-viewflow-2.0.0b6/viewflow/templates/formtools/wizard/wizard_form.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/registration/logged_out.html` & `django-viewflow-2.0.0b6/viewflow/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/registration/login.html` & `django-viewflow-2.0.0b6/viewflow/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/registration/password_change_done.html` & `django-viewflow-2.0.0b6/viewflow/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/registration/password_change_form.html` & `django-viewflow-2.0.0b6/viewflow/templates/registration/password_change_form.html`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     <div class="mdc-layout-grid__inner vf-page__grid-inner">
       <div class="mdc-layout-grid__cell mdc-layout-grid__cell--span-10-desktop mdc-layout-grid__cell--span-8-tablet mdc-layout-grid__cell--span-4-phone">
         <div class="mdc-card vf-card">
           <section class="vf-card__header">
             <h1 class="vf-card__title">{{ title }}</h1>
           </section>
           <vf-form>
-            <form class="vf-form" method="POST">
+            <form class="vf-form" method="POST" {% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>
               {% csrf_token %}
               <section class="vf-card__form">
                 {% render form view.layout %}
               </section>
               <section class="mdc-card__actions vf-card__actions">
                 <button class="mdc-button mdc-card__action mdc-card__action--button mdc-button--raised" type="submit">{% trans "Change" %}</button>
               </section>
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_complete.html` & `django-viewflow-2.0.0b6/viewflow/templates/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_confirm.html` & `django-viewflow-2.0.0b6/viewflow/templates/registration/password_reset_confirm.html`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {% block lockscreen-sidebar-content %}
 
   {% if validlink %}
 
     <p>{% trans "Please enter your new password twice so we can verify you typed it in correctly." %}</p>
 
     <vf-form>
-      <form class="vf-form" method="POST">
+      <form class="vf-form" method="POST" {% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>
         {% csrf_token %}
         {% form form view.layout %}
         <div class="vf-page-lockscreen__sidebar-action-row">
           <button class="mdc-button mdc-card__action mdc-card__action--button mdc-button--raised" type="submit">{% trans 'Change my password' %}</button>
         </div>
       </form>
     </vf-form>
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_done.html` & `django-viewflow-2.0.0b6/viewflow/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_form.html` & `django-viewflow-2.0.0b6/viewflow/templates/registration/password_reset_form.html`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 {% block lockscreen-sidebar-header-title %}{{ title }}{% endblock %}
 
 
 {% block lockscreen-sidebar-content %}
   <p>{% trans 'Forgotten your password? Enter your email address below, and we’ll email instructions for setting a new one.' %}</p>
 
   <vf-form>
-    <form class="vf-form" method="POST">
+    <form class="vf-form" method="POST" {% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>
       {% csrf_token %}
       {% render form view.layout %}
       <div class="vf-page-lockscreen__sidebar-action-row">
         <a href="{% url 'login' %}" class="mdc-button mdc-card__action mdc-card__action--button" type="submit">{% trans 'Cancel' %}</a>
         <button class="mdc-button mdc-card__action mdc-card__action--button mdc-button--raised" type="submit">{% trans 'Reset' %}</button>
       </div>
     </form>
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
 {% extends 'viewflow/base_lockscreen.html' %} {% load i18n viewflow %} {% block
 title %}{{ title }} - {{ block.super }}{% endblock %} {% block lockscreen-
 sidebar-header-title %}{{ title }}{% endblock %} {% block lockscreen-sidebar-
 content %}
 {% trans 'Forgotten your password? Enter your email address below, and weâll
 email instructions for setting a new one.' %}
-{% csrf_token %} {% render form view.layout %}
+
+% if form.is_multipart %} enctype="multipart/form-data"{% endif %}> {%
+csrf_token %} {% render form view.layout %}
 {%_trans_'Cancel'_%} {% trans 'Reset' %}
  {% endblock %} {% block lockscreen-content-icon %}lock{% endblock %}
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/registration/profile.html` & `django-viewflow-2.0.0b6/viewflow/templates/registration/profile.html`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
           <section class="mdc-card__actions vf-page-profile__avatar-actions">
             <div class="mdc-button mdc-button--raised mdc-card__action vf-page-profile__avatar-change">
               {% trans "Change" %}
               <input type="file">
 
             </div>
           </section>
-          <form method="POST" enctype="multipart/form-data">
+          <form method="POST" enctype="multipart/form-data" {% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>
             {% csrf_token %}
             <input type="file" name="avatar" style="display:none">
             <button type="submit" style="display:none">{% trans "Submit" %}</button>
           </form>
         </vf-page-profile-avatar>
       </div>
     </div>
```

#### html2text {}

```diff
@@ -13,9 +13,11 @@
   {% url 'password_change' as password_change_url %} {% if password_change_url
 %} {%_trans_"Change_password"_%} {% endif %} {% url 'profile_edit' as
 profile_edit_url %} {% if profile_edit_url %} {%_trans_"Edit"_%} {% endif %}
 
 [{{ request.user|user_avatar_url }}]
 
 {% trans "Change" %} [File]
-{% csrf_token %} [File] {% trans "Submit" %}
+
+% if form.is_multipart %} enctype="multipart/form-data"{% endif %}> {%
+csrf_token %} [File] {% trans "Submit" %}
 {% endblock content %}
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/registration/provider_list.html` & `django-viewflow-2.0.0b6/viewflow/templates/registration/provider_list.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/base.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/base.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/base_lockscreen.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/base_lockscreen.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/base_page.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/base_page.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/import_export/export_action.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/contrib/import_export/export_action.html`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
               <h1 class="vf-card__title">{{ view.model|verbose_name_plural|title }}</h1>
               <h2 class="vf-card__breadcrumbs">
                 <a href="{% current_viewset_reverse viewset 'list' %}">{{ view.model|verbose_name_plural|title }}</a>
                 <a>{% trans 'Export' %}</a>
               </h2>
             </section>
             <vf-form>
-              <form class="vf-form" method="POST" data-turbo="false">
+              <form class="vf-form" method="POST" data-turbo="false" {% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>
                 {% csrf_token %}
                 <section class="vf-card__form">
                   <h3 class="vf-card__alert">
                     {% if view.objects_count %}
                       {% blocktrans with name=view.model|verbose_name plural_name=view.model|verbose_name_plural count objects_count=view.objects_count %}
                         Export the {{ name }}
                       {% plural %}
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 {% extends request.resolver_match.app.base_template_name|default:'viewflow/
 base_page.html' %} {% load i18n viewflow %} {% block content %}
 {% block confirm-cell %}
 ****** {{ view.model|verbose_name_plural|title }} ******
 ***** {{_view.model|verbose_name_plural|title_}} {% trans 'Export' %} *****
 
-{% csrf_token %}
+% if form.is_multipart %} enctype="multipart/form-data"{% endif %}> {%
+csrf_token %}
 **** {% if view.objects_count %} {% blocktrans with
 name=view.model|verbose_name plural_name=view.model|verbose_name_plural count
 objects_count=view.objects_count %} Export the {{ name }} {% plural %} Export
 the {{ objects_count }} {{ plural_name }} {% endblocktrans %} {% else %} {%
 blocktrans with plural_name=view.model|verbose_name_plural %} Export all {
 { plural_name }} {% endblocktrans %} {% endif %} ****
   {% render form %}   arrow_back{% trans "Back" %}
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/plotly.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/contrib/plotly.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/swagger.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/contrib/swagger.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/app_menu.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/app_menu.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/list_bulk_actions.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/list_bulk_actions.html`

 * *Files 3% similar despite different names*

```diff
@@ -50,13 +50,13 @@
           {% endfor %}
         </ul>
       </div>
     </div>
   </div>
 </div>
 <vf-form>
-  <form action="." method="post" class="vf-list__action-form">
+  <form action="." method="post" class="vf-list__action-form" {% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>
     {% csrf_token %}
     <button type="submit" class="vf-list__action-button mdc-button mdc-button--dense mdc-button--raised">GO</button>
   </form>
 </vf-form>
 </div>
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/list_filter.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/list_filter.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% load i18n viewflow %}
 <vf-list-filter id="id_filter_drawer" class="mdc-drawer mdc-drawer--dismissible vf-list__filter{% if view.filterset.form.has_changed %} mdc-drawer--open{% endif %}">
   <nav class="mdc-drawer__content">
     <h4 class="vf-list__filter-title">{% trans "Filter" %}</h4>
     <vf-form>
-      <form method="GET" class="vf-list__filter-form">
+      <form method="GET" class="vf-list__filter-form" {% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>
         {% render view.filterset.form %}
         <input type="hidden" name="{{ view.ordering_kwarg }}" value="{{ request.GET|list_order:view }}">
         <div class="v_list__filter-actions">
           <button class="mdc-button" type="submit">{% trans "Filter" %}</button>
         </div>
       </form>
     </vf-form>
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/list_pagination.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/list_pagination.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/object_detail_card.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/object_detail_card.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/site_menu.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/site_menu.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/view_action_menu.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/includes/view_action_menu.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/material/circular_progress.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/material/circular_progress.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/confirm_delete.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/views/confirm_delete.html`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                     {% endif %}
                   {% endif %}
                   <a>{% trans 'Delete' %}</a>
                 </h2>
               {% endblock %}
             </section>
             <vf-form>
-              <form class="vf-form" method="POST">
+              <form class="vf-form" method="POST" {% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>
                 {% csrf_token %}
                 <section class="vf-card__form">
                   <h3 class="vf-card__alert">
                     {% blocktrans with escaped_object=object %}"{{ escaped_object }}" and all of the following related items will be deleted{% endblocktrans %}
                   </h3>
 
                   {% for model, objects in view.get_deleted_objects %}
```

#### html2text {}

```diff
@@ -4,15 +4,16 @@
 ****** {{ view.object }} ******
 {% block confirm-header-subtitle %}
 ***** {{_view.model|verbose_name_plural|title_}} {% if view.object.pk %} {%
 current_viewset_reverse viewset 'detail' view.object.pk as detail_url %} {% if
 detail_url %} {{_view.object_}} {% else %} {{_view.object_}} {% endif %} {%
 endif %} {% trans 'Delete' %} *****
 {% endblock %}
-{% csrf_token %}
+% if form.is_multipart %} enctype="multipart/form-data"{% endif %}> {%
+csrf_token %}
 **** {% blocktrans with escaped_object=object %}"{{ escaped_object }}" and all
 of the following related items will be deleted{% endblocktrans %} ****
 {% for model, objects in view.get_deleted_objects %}
 **** {{ model|verbose_name_plural|title }} ****
 {% for object in objects %} {% get_absolute_url site object as object_url %} {%
 if object_url %}{{_object_}}{% else %}{{ object }}{% endif %}{% if not
 forloop.last %}, {% endif %} {% endfor %} {% endfor %}   Delete
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/delete_action.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/views/delete_action.html`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
               <h1 class="vf-card__title">{{ view.model|verbose_name_plural|title }}</h1>
               <h2 class="vf-card__breadcrumbs">
                 <a href="{% current_viewset_reverse viewset 'list' %}">{{ view.model|verbose_name_plural|title }}</a>
                 <a>{% trans 'Delete' %}</a>
               </h2>
             </section>
             <vf-form>
-              <form class="vf-form" method="POST">
+              <form class="vf-form" method="POST" {% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>
                 {% csrf_token %}
                 {{ form }}
                 <section class="vf-card__form">
                   <h3 class="vf-card__alert">
                     {% if view.objects_count  %}
                       {% blocktrans with name=view.model|verbose_name plural_name=view.model|verbose_name_plural count objects_count=view.objects_count %}
                         Are you sure you want to delete the {{ name }} and related items?
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 {% extends request.resolver_match.app.base_template_name|default:'viewflow/
 base_page.html' %} {% load i18n viewflow %} {% block content %}
 {% block confirm-cell %}
 ****** {{ view.model|verbose_name_plural|title }} ******
 ***** {{_view.model|verbose_name_plural|title_}} {% trans 'Delete' %} *****
 
-{% csrf_token %} {{ form }}
+% if form.is_multipart %} enctype="multipart/form-data"{% endif %}> {%
+csrf_token %} {{ form }}
 **** {% if view.objects_count %} {% blocktrans with
 name=view.model|verbose_name plural_name=view.model|verbose_name_plural count
 objects_count=view.objects_count %} Are you sure you want to delete the {{ name
 }} and related items? {% plural %} Are you sure you want to delete the {
 { objects_count }} {{ plural_name }} and related items? {% endblocktrans %} {%
 else %} {% blocktrans with plural_name=view.model|verbose_name_plural %} Are
 you sure you want to delete all {{ plural_name }} and related items? {%
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/detail.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/views/detail.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/form.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/views/form.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/list.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/views/list.html`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,19 @@
   <div class="mdc-layout-grid vf-page__grid mdc-drawer-app-content">
     <div class="mdc-layout-grid__inner vf-page__grid-inner">
       {% block list-cell %}
         <div class="mdc-layout-grid__cell {% block list-cell-span %}mdc-layout-grid__cell--span-12{% endblock %}">
           <div class="mdc-card vf-card">
             {% block list-header %}
               <section class="vf-card__header">
-                {% block list-header-title %}<h1 class="vf-card__title">{{ view.model|verbose_name_plural|title }}</h1>{% endblock %}
+                {% block list-header-title %}<h1 class="vf-card__title">
+                  {% if view.title %}{{ view.title }}
+                  {% else %}{{ view.model|verbose_name_plural|title }}
+                  {% endif %}
+                </h1>{% endblock %}
                 {% block list-header-subtitle %}{% endblock %}
                 {% block list-header-menu %}
                   <div class="vf-card__menu">
                     {% if view.filterset %}
                       <vf-list-filter-trigger class="mdc-button vf-list__filter-trigger{% if view.filterset.form.has_changed %} vf-list__filter-trigger--active{% endif %}" data-toggle-filter-id="id_filter_drawer">
                         <i class="material-icons">filter_list</i>
                       </vf-list-filter-trigger>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
 {% extends request.resolver_match.app.base_template_name|default:'viewflow/
 base_page.html' %} {% load viewflow %} {% block page-toolbar-actions %} {% if
 view.search_enabled %}{% endif %} {{ block.super }} {% endblock %} {% block
 content %} {% block list-filter %}{% if view.filterset %}{% include 'viewflow/
 includes/list_filter.html' %}{% endif %}{% endblock list-filter %}
 {% block list-cell %}
 {% block list-header %}  {% block list-header-title %}
-****** {{ view.model|verbose_name_plural|title }} ******
+****** {% if view.title %}{{ view.title }} {% else %}{
+{ view.model|verbose_name_plural|title }} {% endif %} ******
 {% endblock %} {% block list-header-subtitle %}{% endblock %} {% block list-
 header-menu %}
 {% if view.filterset %}  filter_list  {% endif %} {% include 'viewflow/
 includes/view_action_menu.html' with view=view only %}
 {% endblock %}  {% endblock list-header %} {% block list-content %} {% with
 bulk_actions=view.get_bulk_actions %}   {% if bulk_actions %}{% endif %}
 % if paginator and paginator.count %} data-total-items-count="{
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/transition.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/views/transition.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/assign.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/assign.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/flow_menu.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/flow_menu.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/graph.bpmn` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/graph.bpmn`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/graph.svg` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/graph.svg`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_cancel.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/process_cancel.html`

 * *Files 10% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                   </div>
                 </div>
               {% endfor %}
             </div>
           </div>
 
           <div class="mdc-card__actions vf-card__actions">
-            <form method="POST">{% csrf_token %}
+            <form method="POST" {% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>{% csrf_token %}
               <button type="submit" name="_cancel_process" value="1" class="mdc-button mdc-button--raised mdc-card__action mdc-card__action--button">
                 <div class="mdc-button__ripple"></div>
                 <span class="mdc-button__label">{% trans "Cancel" %}</span> <!- todo perms -->
               </button>
             </form>
           </div>
         </div>
```

#### html2text {}

```diff
@@ -13,14 +13,15 @@
 activation.task.flow_task.task_type == 'JOIN' %} merge_type {% else %}
 newspaper {% endif %}
 {{_activation.task.flow_task_}} {% if activation.task.flow_task.task_type ==
 'HUMAN' %}
 {{ activation.task.owner|default:"No owner assigned" }}
 {% endif %}
 {% endfor %}
-{% csrf_token %}
+% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>{%
+csrf_token %}
 {% trans "Cancel" %}
 todo perms -->
 {% block panel-cell %}
 {% include_process_data process %}
 {% endblock panel-cell %}
 {% endblock %}
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_dashboard.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/process_dashboard.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_data.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/process_data.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_detail.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/process_detail.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends request.resolver_match.app.base_template_name|default:'viewflow/workflow/base_page.html' %}
 {% load i18n viewflow workflow  %}
 
 
 {% block content %}
   <div class="mdc-layout-grid vf-page__grid">
-    <div class="mdc-layout-grid__inner">
+    <div class="mdc-layout-grid__inner vf-page__grid-inner">
       <div class="mdc-layout-grid__cell mdc-layout-grid__cell--span-8-desktop mdc-layout-grid__cell--span-8-tablet mdc-layout-grid__cell--span-4-phone">
         <div class="mdc-card vf-card">
           <section class="vf-card__header">
             <h1 class="vf-card__title">
               {{ process.brief }}
             </h1>
             <h2 class="vf-card__breadcrumbs">
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_list.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/process_list.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/start.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/start.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends request.resolver_match.app.base_template_name|default:'viewflow/workflow/base_page.html' %}
 {% load i18n viewflow workflow %}
 
 
 {% block content %}{% with process=request.activation.process task=request.activation.task %}
   <div class="mdc-layout-grid vf-page__grid">
-    <div class="mdc-layout-grid__inner">
+    <div class="mdc-layout-grid__inner vf-page__grid-inner">
       {% block form-cell %}
         <div class="mdc-layout-grid__cell {% block form-cell-span %}mdc-layout-grid__cell--span-8-desktop mdc-layout-grid__cell--span-8-tablet mdc-layout-grid__cell--span-4-phone{% endblock %}">
           <div class="mdc-card vf-card">
             <section class="vf-card__header">
               {% block form-header-title %}
                 <h1 class="vf-card__title">
                   {{ request.activation.task.flow_task }}
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_assign.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_assign.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_base.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_base.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% extends request.resolver_match.app.base_template_name|default:'viewflow/workflow/base_page.html' %}
 {% load i18n viewflow workflow %}
 
 {% block content %}{% with process=request.activation.process task=request.activation.task %}
   <div class="mdc-layout-grid vf-page__grid">
-    <div class="mdc-layout-grid__inner">
+    <div class="mdc-layout-grid__inner vf-page__grid-inner">
       <div class="mdc-layout-grid__cell mdc-layout-grid__cell--span-8-desktop mdc-layout-grid__cell--span-8-tablet mdc-layout-grid__cell--span-4-phone">
         <div class="mdc-card vf-card">
           <section class="vf-card__header">
             <h1 class="vf-card__title">
               {{ task.flow_task.task_description|default:task.flow_task.task_title }}
             </h1>
             <h2 class="vf-card__breadcrumbs">
@@ -38,13 +38,20 @@
           <section class="mdc-card__actions vf-card__actions">
             {% block task_actions %}{% endblock %}
           </section>
         </div>
       </div>
       {% block panel-cell %}
         <div class="mdc-layout-grid__cell {% block panel-cell-span %}mdc-layout-grid__cell--span-4-desktop mdc-layout-grid__cell--span-8-tablet mdc-layout-grid__cell--span-4-phone{% endblock %}">
-          {% include_process_data request.activation.process %}
+          <div class="mdc-layout-grid__inner vf-page__grid-inner">
+            <div class="mdc-layout-grid__cell mdc-layout-grid__cell--span-12">
+              {% include_process_data request.activation.process %}
+            </div>
+            <div class="mdc-layout-grid__cell mdc-layout-grid__cell--span-12">
+              {% include_task_data request.activation.task %}
+            </div>
+          </div>
         </div>
       {% endblock panel-cell %}
     </div>
   </div>
 {% endwith %}{% endblock %}
```

#### html2text {}

```diff
@@ -9,9 +9,10 @@
 
  }}" style="width:100%">
  }}" style="width:100%">
 {% block task_content %}{% endblock %}
   {% block task_actions %}{% endblock %}
 {% block panel-cell %}
 {% include_process_data request.activation.process %}
+{% include_task_data request.activation.task %}
 {% endblock panel-cell %}
 {% endwith %}{% endblock %}
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_cancel.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_cancel.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_detail.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_detail.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_list.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_list.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_revive.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_revive.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_unassign.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_unassign.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_undo.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/task_undo.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/tasks_assign.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/tasks_assign.html`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             <h1 class="vf-card__title">{% trans "Assign selected tasks" %}</h1>
             <h2 class="vf-card__breadcrumbs">
               <a href="{% reverse viewset 'queue' %}">{% trans 'Queue' %}</a>
               <a>{% trans 'Assign' %}</a>
             </h2>
           </section>
           <vf-form>
-            <form class="vf-form" method="POST">
+            <form class="vf-form" method="POST" {% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>
               {% csrf_token %}
               {{ form }}
               <section class="vf-card__form">
                 <table class="vf-list__table">
                   <thead>
                     <tr>
                       <th class="vf-list__table-header vf-list__table-header-text">#</th>
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends request.resolver_match.app.base_template_name|default:'viewflow/
 base_page.html' %} {% load i18n viewflow %} {% block content %}
 ****** {% trans "Assign selected tasks" %} ******
 ***** {%_trans_'Queue'_%} {% trans 'Assign' %} *****
 
-{% csrf_token %} {{ form }}
+% if form.is_multipart %} enctype="multipart/form-data"{% endif %}> {%
+csrf_token %} {{ form }}
 #               {% trans       {% trans   {% trans "Process  {% trans "Created" %}
                 "Task" %}      "Brief" %} brief" %}
 #{              {              {          {                  {
 {               {              {          {                  {
 task.process_id task.flow_task task.brief task.process.brief task.created|timesince
 }}/{{ task.id   }}             }}         }}                 }}
 }}
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/tasks_unassign.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/tasks_unassign.html`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             <h1 class="vf-card__title">{% trans "Unassign selected tasks" %}</h1>
             <h2 class="vf-card__breadcrumbs">
               <a href="{% reverse viewset 'inbox' %}">{% trans 'Inbox' %}</a>
               <a>{% trans 'Unassign' %}</a>
             </h2>
           </section>
           <vf-form>
-            <form class="vf-form" method="POST">
+            <form class="vf-form" method="POST" {% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>
               {% csrf_token %}
               {{ form }}
               <section class="vf-card__form">
                 <table class="vf-list__table">
                   <thead>
                     <tr>
                       <th class="vf-list__table-header vf-list__table-header-text">#</th>
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends request.resolver_match.app.base_template_name|default:'viewflow/
 base_page.html' %} {% load i18n viewflow %} {% block content %}
 ****** {% trans "Unassign selected tasks" %} ******
 ***** {%_trans_'Inbox'_%} {% trans 'Unassign' %} *****
 
-{% csrf_token %} {{ form }}
+% if form.is_multipart %} enctype="multipart/form-data"{% endif %}> {%
+csrf_token %} {{ form }}
 #               {% trans       {% trans   {% trans "Process  {% trans "Created" %}
                 "Task" %}      "Brief" %} brief" %}
 #{              {              {          {                  {
 {               {              {          {                  {
 task.process_id task.flow_task task.brief task.process.brief task.created|timesince
 }}/{{ task.id   }}             }}         }}                 }}
 }}
```

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/workflow_menu.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/workflow_menu.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/workflow_tasks_list.html` & `django-viewflow-2.0.0b6/viewflow/templates/viewflow/workflow/workflow_tasks_list.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/templatetags/viewflow.py` & `django-viewflow-2.0.0b6/viewflow/templatetags/viewflow.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/this_object.py` & `django-viewflow-2.0.0b6/viewflow/this_object.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/urls/__init__.py` & `django-viewflow-2.0.0b6/viewflow/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/urls/base.py` & `django-viewflow-2.0.0b6/viewflow/urls/base.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/urls/model.py` & `django-viewflow-2.0.0b6/viewflow/urls/model.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/urls/sites.py` & `django-viewflow-2.0.0b6/viewflow/urls/sites.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/utils.py` & `django-viewflow-2.0.0b6/viewflow/utils.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/views/__init__.py` & `django-viewflow-2.0.0b6/viewflow/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/views/actions.py` & `django-viewflow-2.0.0b6/viewflow/views/actions.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/views/base.py` & `django-viewflow-2.0.0b6/viewflow/views/base.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/views/create.py` & `django-viewflow-2.0.0b6/viewflow/views/create.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/views/delete.py` & `django-viewflow-2.0.0b6/viewflow/views/delete.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/views/detail.py` & `django-viewflow-2.0.0b6/viewflow/views/detail.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/views/filters.py` & `django-viewflow-2.0.0b6/viewflow/views/filters.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/views/list.py` & `django-viewflow-2.0.0b6/viewflow/views/list.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/views/search.py` & `django-viewflow-2.0.0b6/viewflow/views/search.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/views/update.py` & `django-viewflow-2.0.0b6/viewflow/views/update.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/activation.py` & `django-viewflow-2.0.0b6/viewflow/workflow/activation.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/admin.py` & `django-viewflow-2.0.0b6/viewflow/workflow/admin.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/base.py` & `django-viewflow-2.0.0b6/viewflow/workflow/base.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/chart.py` & `django-viewflow-2.0.0b6/viewflow/workflow/chart.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/context.py` & `django-viewflow-2.0.0b6/viewflow/workflow/context.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/fields.py` & `django-viewflow-2.0.0b6/viewflow/workflow/fields.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/__init__.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/mixins.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/mixins.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/nodes.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/nodes.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/utils.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/utils.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/__init__.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/actions.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/views/actions.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/chart.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/views/chart.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/create.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/views/create.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/dashboard.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/detail.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/views/detail.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/filters.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/views/filters.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/list.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/views/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     mixins.ProcessViewTemplateNames,
     ListModelView,
 ):
     """List of current user assigned tasks of a flow"""
 
     flow_class = None
     template_filename = "process_tasks_list.html"
+    title = _('Inbox')
 
     columns = ("task_id", "flow_task", "brief", "created")
     filterset_class = filters.FlowUserTaskListFilter
 
     def task_id(self, task):
         task_url = task.flow_task.reverse("index", args=[task.process_id, task.pk])
         return mark_safe(f'<a href="{task_url}">#{task.process_id}/{task.pk}</a>')
@@ -52,14 +53,15 @@
 ):
     """List of current user available tasks of a flow"""
 
     columns = ("task_id", "flow_task", "brief", "created")
     filterset_class = filters.FlowUserTaskListFilter
     flow_class = None
     template_filename = "process_tasks_list.html"
+    title = _('Queue')
 
     def task_id(self, task):
         task_url = task.flow_task.reverse("index", args=[task.process_id, task.pk])
         return mark_safe(f'<a href="{task_url}">#{task.process_id}/{task.pk}</a>')
 
     task_id.short_description = _("#")
 
@@ -86,14 +88,15 @@
 ):
     """List of current user completed tasks of a flow."""
 
     columns = ("task_id", "brief", "created", "finished", "process_summary")
     filterset_class = filters.FlowArchiveListFilter
     flow_class = None
     template_filename = "process_tasks_list.html"
+    title = _('Archive')
 
     def task_id(self, task):
         task_url = task.flow_task.reverse("index", args=[task.process_id, task.pk])
         return mark_safe(f'<a href="{task_url}">#{task.process_id}/{task.pk}</a>')
 
     task_id.short_description = _("#")
 
@@ -149,14 +152,15 @@
 class WorkflowInboxListView(WorkflowTaskListView):
     """List of current user assigned tasks from all viewset registered flows."""
 
     columns = ("task_id", "flow_task", "brief", "process_brief", "created")
     bulk_actions = (
         Action(name=_("Unassign selected tasks"), viewname="tasks_unassign"),
     )
+    title = _('Inbox')
 
     filterset_class = filters.FlowUserTaskListFilter
 
     @viewprop
     def queryset(self):
         """List of tasks assigned to the current user."""
         return self.model._default_manager.inbox(self.flow_classes, self.request.user)
@@ -167,22 +171,24 @@
 
 class WorkflowQueueListView(WorkflowTaskListView):
     """List of current user available tasks from all viewset registered flows."""
 
     columns = ("task_id", "process_brief", "flow_task", "brief", "created")
     filterset_class = filters.FlowUserTaskListFilter
     bulk_actions = (Action(name=_("Assign selected tasks"), viewname="tasks_assign"),)
+    title = _('Queue')
 
     @viewprop
     def queryset(self):
         return self.model._default_manager.queue(self.flow_classes, self.request.user)
 
 
 class WorkflowArchiveListView(WorkflowTaskListView):
     """List of current user participated tasks from all viewset registered flows."""
 
     columns = ("task_id", "flow_task", "brief", "process_brief", "created", "finished")
     filterset_class = filters.FlowArchiveListFilter
+    title = _('Archive')
 
     @viewprop
     def queryset(self):
         return self.model._default_manager.archive(self.flow_classes, self.request.user)
```

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/mixins.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/update.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/views/update.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/flow/viewset.py` & `django-viewflow-2.0.0b6/viewflow/workflow/flow/viewset.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/lock.py` & `django-viewflow-2.0.0b6/viewflow/workflow/lock.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/managers.py` & `django-viewflow-2.0.0b6/viewflow/workflow/managers.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0001_initial.py` & `django-viewflow-2.0.0b6/viewflow/workflow/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0002_fsmchange.py` & `django-viewflow-2.0.0b6/viewflow/workflow/migrations/0002_fsmchange.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0004_extend_fields_length.py` & `django-viewflow-2.0.0b6/viewflow/workflow/migrations/0004_extend_fields_length.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0006_i18n.py` & `django-viewflow-2.0.0b6/viewflow/workflow/migrations/0006_i18n.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0007_owner_permission_obj.py` & `django-viewflow-2.0.0b6/viewflow/workflow/migrations/0007_owner_permission_obj.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0008_jsonfield_and_artifact.py` & `django-viewflow-2.0.0b6/viewflow/workflow/migrations/0008_jsonfield_and_artifact.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0010_viewflow20.py` & `django-viewflow-2.0.0b6/viewflow/workflow/migrations/0010_viewflow20.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0011_alter_task_created_and_more.py` & `django-viewflow-2.0.0b6/viewflow/workflow/migrations/0011_alter_task_created_and_more.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/models.py` & `django-viewflow-2.0.0b6/viewflow/workflow/models.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/__init__.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/end.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/end.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/func.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/func.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/handle.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/handle.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/if_gate.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/if_gate.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/job.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/job.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/join.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/join.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/mixins.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/mixins.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/obsolete.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/obsolete.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/split.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/split.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/start.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/start.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/subprocess.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/subprocess.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/switch.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/switch.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/nodes/view.py` & `django-viewflow-2.0.0b6/viewflow/workflow/nodes/view.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/status.py` & `django-viewflow-2.0.0b6/viewflow/workflow/status.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/token.py` & `django-viewflow-2.0.0b6/viewflow/workflow/token.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b5/viewflow/workflow/utils.py` & `django-viewflow-2.0.0b6/viewflow/workflow/utils.py`

 * *Files identical despite different names*

