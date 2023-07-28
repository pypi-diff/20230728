# Comparing `tmp/django-photologue-3.8.1.tar.gz` & `tmp/django-photologue-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-photologue-3.8.1.tar", last modified: Sun Dec  3 15:42:16 2017, max compression
+gzip compressed data, was "dist/django-photologue-3.9.tar", last modified: Sun Apr 21 16:55:04 2019, max compression
```

## Comparing `django-photologue-3.8.1.tar` & `django-photologue-3.9.tar`

### file list

```diff
@@ -1,215 +1,188 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/django_photologue.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      934 2017-12-03 15:42:16.000000 django-photologue-3.8.1/django_photologue.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2017-12-03 15:42:16.000000 django-photologue-3.8.1/django_photologue.egg-info/not-zip-safe
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       19 2017-12-03 15:42:16.000000 django-photologue-3.8.1/django_photologue.egg-info/top_level.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6406 2017-12-03 15:42:16.000000 django-photologue-3.8.1/django_photologue.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       67 2017-12-03 15:42:16.000000 django-photologue-3.8.1/django_photologue.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2017-12-03 15:42:16.000000 django-photologue-3.8.1/django_photologue.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      712 2017-12-03 15:42:15.000000 django-photologue-3.8.1/CONTRIBUTORS.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      934 2017-12-03 15:42:16.000000 django-photologue-3.8.1/PKG-INFO
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/scripts/
--rwxrwxr-x   0 vagrant   (1000) vagrant   (1000)     3229 2017-12-03 15:42:15.000000 django-photologue-3.8.1/scripts/releaser_hooks.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:15.000000 django-photologue-3.8.1/scripts/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1583 2017-12-03 15:42:15.000000 django-photologue-3.8.1/LICENSE.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1890 2017-12-03 15:42:15.000000 django-photologue-3.8.1/README.rst
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/uk/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    27437 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/uk/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    20767 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/uk/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/sk/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/sk/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    22551 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/sk/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15036 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/sk/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/pl/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    18782 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/pl/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7097 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/pl/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/eu/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/eu/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    19614 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/eu/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10135 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/eu/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/cs/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    19868 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/cs/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     9764 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/cs/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/hu/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/hu/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    22959 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/hu/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16370 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/hu/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/en_US/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/en_US/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    19517 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/en_US/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8171 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/en_US/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/es_ES/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/es_ES/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    22199 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/es_ES/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    14896 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/es_ES/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/pt/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    19005 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/pt/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7876 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/pt/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/da_DK/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/da_DK/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15954 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/da_DK/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      510 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/da_DK/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/fr/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    23185 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16527 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/fr/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/no/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/no/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    18189 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/no/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6716 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/no/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/en/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/en/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15939 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/en/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      495 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/en/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/ru/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    25369 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/ru/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16893 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/ru/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/tr/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    19995 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/tr/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    11136 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/tr/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/it/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/it/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    19100 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/it/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8006 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/it/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/de/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/de/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    22650 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15916 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/de/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/es/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/es/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15938 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/es/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      494 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/es/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/nl/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    21936 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/nl/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    14567 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/nl/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/da/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/da/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    21516 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/da/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    14158 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/da/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/pt_BR/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    19019 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/pt_BR/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7890 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/pt_BR/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/ca/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/locale/ca/LC_MESSAGES/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15939 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/ca/LC_MESSAGES/django.po
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      495 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/locale/ca/LC_MESSAGES/django.mo
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/utils/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3798 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/utils/reflection.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2029 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/utils/watermark.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/utils/__init__.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/res/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    14453 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/res/sample.jpg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      659 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/res/test_photologue_portrait.jpg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      573 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/res/test_photologue_square.jpg
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/res/zips/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7815 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/res/zips/not_image.zip
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15784 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/res/zips/ignored_files.zip
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7652 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/res/zips/sample.zip
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      659 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/res/test_photologue_landscape.jpg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       58 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/res/test_nonsense.jpg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      659 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/res/test_photologue_&quoting.jpg
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/templates/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/templates/photologue/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1275 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/photo_archive_year.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1134 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/gallery_archive_year.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      903 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/gallery_archive_day.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      700 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/photo_list.html
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/templates/photologue/tags/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      187 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/tags/prev_in_gallery.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      187 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/tags/next_in_gallery.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       26 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/root.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      930 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/photo_archive_day.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      780 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/gallery_detail.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1435 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/photo_archive_month.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      941 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/photo_archive.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      824 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/gallery_archive.html
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/templates/photologue/includes/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      805 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/includes/paginator.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      570 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/includes/gallery_sample.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1165 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/gallery_list.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1321 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/photo_detail.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1330 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/photologue/gallery_archive_month.html
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/templates/admin/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/templates/admin/photologue/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/templates/admin/photologue/photo/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      260 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/admin/photologue/photo/change_list.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2100 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templates/admin/photologue/photo/upload_zip.html
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/templatetags/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4377 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templatetags/photologue_tags.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/templatetags/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    36245 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/models.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7964 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/forms.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/management/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/management/commands/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1026 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/management/commands/plflush.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      550 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/management/commands/plcreatesize.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1412 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/management/commands/plcache.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1479 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/management/commands/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/management/__init__.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/migrations/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      440 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/migrations/0006_auto_20141028_2005.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      473 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/migrations/0005_auto_20141027_1552.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1375 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/migrations/0004_auto_20140915_1259.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      925 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/migrations/0007_auto_20150404_1737.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1387 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/migrations/0002_photosize_data.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      566 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/migrations/0009_auto_20160102_0904.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      454 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/migrations/0008_auto_20150509_1557.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    12280 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/migrations/0001_initial.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1188 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/migrations/0010_auto_20160105_1307.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      552 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/migrations/0003_auto_20140822_1716.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/migrations/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4058 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/urls.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/contrib/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      299 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/photo_archive_year.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      410 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/gallery_archive_year.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      757 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/gallery_archive_day.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      927 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/photo_list.html
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/tags/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      183 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/tags/prev_in_gallery.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      183 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/tags/next_in_gallery.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       25 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/root.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      579 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/photo_archive_day.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      723 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/gallery_detail.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      595 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/photo_archive_month.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      545 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/photo_archive.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      834 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/gallery_archive.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1239 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/gallery_list.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      791 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/photo_detail.html
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      776 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/contrib/old_style_templates/templates/photologue/gallery_archive_month.html
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:16.000000 django-photologue-3.8.1/photologue/tests/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      458 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/test_effect.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5056 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/test_resize.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1915 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/test_views_photo.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2219 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/test_gallery.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2146 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/test_views_gallery.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      431 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/test_urls.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1084 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/test_photosize.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1447 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/test_sitemap.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     9650 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/test_photo.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      784 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/helpers.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5773 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/test_sites.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8571 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/test_zipupload.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4022 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/tests/factories.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      582 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/managers.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10398 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/admin.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       98 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1809 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/sitemaps.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5789 2017-12-03 15:42:15.000000 django-photologue-3.8.1/photologue/views.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      377 2017-12-03 15:42:15.000000 django-photologue-3.8.1/MANIFEST.in
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      382 2017-12-03 15:42:16.000000 django-photologue-3.8.1/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      122 2017-12-03 15:42:15.000000 django-photologue-3.8.1/requirements.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1839 2017-12-03 15:42:15.000000 django-photologue-3.8.1/setup.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      246 2019-04-21 16:55:04.000000 django-photologue-3.9/requirements.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1723 2019-04-21 16:55:04.000000 django-photologue-3.9/README.rst
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2923 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/urls.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/res/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      659 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/res/test_photologue_portrait.jpg
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      659 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/res/test_photologue_&quoting.jpg
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      573 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/res/test_photologue_square.jpg
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/res/zips/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15784 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/res/zips/ignored_files.zip
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7815 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/res/zips/not_image.zip
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7652 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/res/zips/sample.zip
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      659 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/res/test_photologue_landscape.jpg
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    14453 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/res/sample.jpg
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       58 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/res/test_nonsense.jpg
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    36757 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/models.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/it/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7965 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    19101 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/de/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15912 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    22706 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/ru/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16852 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    25370 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/no/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/no/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6675 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/no/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    18190 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/no/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/pl/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7056 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    18783 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/cs/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     9776 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    20016 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/en_US/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/en_US/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8130 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/en_US/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    19518 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/en_US/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/nl/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    14526 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    21937 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/eu/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/eu/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10240 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/eu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    19658 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/eu/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/fr/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16487 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    23187 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/hu/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/hu/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16361 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    22992 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/hu/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/pt/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7835 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    19006 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/uk/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    21607 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    28415 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/pt_BR/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7849 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    19020 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/es_ES/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/es_ES/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    14861 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/es_ES/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    22206 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/es_ES/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/ca/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/ca/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15942 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/ca/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    22580 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/ca/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/sk/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/sk/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15443 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/sk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    23100 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/sk/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/tr/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    11095 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    19996 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/tr/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/en/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      454 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    15940 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/da/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/da/LC_MESSAGES/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    14117 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/da/LC_MESSAGES/django.mo
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    21517 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/locale/da/LC_MESSAGES/django.po
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/utils/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3798 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/utils/reflection.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/utils/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2030 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/utils/watermark.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7909 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/forms.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     9626 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/test_photo.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4022 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/factories.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1084 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/test_photosize.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      784 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/helpers.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1447 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/test_sitemap.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5773 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/test_sites.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      458 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/test_effect.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8571 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/test_zipupload.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5056 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/test_resize.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1915 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/test_views_photo.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2219 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/test_gallery.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      431 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/test_urls.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2146 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/tests/test_views_gallery.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1330 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/gallery_archive_month.html
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/tags/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      187 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/tags/prev_in_gallery.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      187 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/tags/next_in_gallery.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      903 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/gallery_archive_day.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      941 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/photo_archive.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      700 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/photo_list.html
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/includes/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      805 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/includes/paginator.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      570 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/includes/gallery_sample.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1275 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/photo_archive_year.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      780 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/gallery_detail.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       26 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/root.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1321 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/photo_detail.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1435 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/photo_archive_month.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1134 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/gallery_archive_year.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1165 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/gallery_list.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      824 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/gallery_archive.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      930 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/photologue/photo_archive_day.html
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/admin/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/admin/photologue/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/admin/photologue/photo/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2094 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/admin/photologue/photo/upload_zip.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      260 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templates/admin/photologue/photo/change_list.html
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10280 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/admin.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      582 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/managers.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/migrations/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1404 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/migrations/0002_photosize_data.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      454 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/migrations/0008_auto_20150509_1557.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1188 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/migrations/0010_auto_20160105_1307.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      473 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/migrations/0005_auto_20141027_1552.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      440 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/migrations/0006_auto_20141028_2005.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      566 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/migrations/0009_auto_20160102_0904.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      552 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/migrations/0003_auto_20140822_1716.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1375 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/migrations/0004_auto_20140915_1259.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      925 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/migrations/0007_auto_20150404_1737.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/migrations/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    12280 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/migrations/0001_initial.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      727 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/migrations/0011_auto_20190223_2138.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1734 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/views.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       96 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/__init__.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/management/
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/management/commands/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1026 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/management/commands/plflush.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      550 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/management/commands/plcreatesize.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1412 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/management/commands/plcache.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1479 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/management/commands/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/management/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1809 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/sitemaps.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templatetags/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4377 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templatetags/photologue_tags.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/photologue/templatetags/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      986 2019-04-21 16:55:04.000000 django-photologue-3.9/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      377 2019-04-21 16:55:04.000000 django-photologue-3.9/MANIFEST.in
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/django_photologue.egg-info/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-04-21 16:55:04.000000 django-photologue-3.9/django_photologue.egg-info/not-zip-safe
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      986 2019-04-21 16:55:04.000000 django-photologue-3.9/django_photologue.egg-info/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5053 2019-04-21 16:55:04.000000 django-photologue-3.9/django_photologue.egg-info/SOURCES.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-04-21 16:55:04.000000 django-photologue-3.9/django_photologue.egg-info/dependency_links.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       54 2019-04-21 16:55:04.000000 django-photologue-3.9/django_photologue.egg-info/requires.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       19 2019-04-21 16:55:04.000000 django-photologue-3.9/django_photologue.egg-info/top_level.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      708 2019-04-21 16:55:04.000000 django-photologue-3.9/CONTRIBUTORS.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      380 2019-04-21 16:55:04.000000 django-photologue-3.9/setup.cfg
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/scripts/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-04-21 16:55:04.000000 django-photologue-3.9/scripts/__init__.py
+-rwxrwxr-x   0 vagrant   (1000) vagrant   (1000)     3265 2019-04-21 16:55:04.000000 django-photologue-3.9/scripts/releaser_hooks.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1773 2019-04-21 16:55:04.000000 django-photologue-3.9/setup.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1583 2019-04-21 16:55:04.000000 django-photologue-3.9/LICENSE.txt
```

### Comparing `django-photologue-3.8.1/django_photologue.egg-info/PKG-INFO` & `django-photologue-3.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: django-photologue
-Version: 3.8.1
+Version: 3.9
 Summary: Powerful image management for the Django web framework.
-Home-page: https://github.com/jdriscoll/django-photologue
+Home-page: https://github.com/richardbarran/django-photologue
 Author: Justin Driscoll, Marcos Daniel Petry, Richard Barran
 Author-email: justin@driscolldev.com, marcospetry@gmail.com, richard@arbee-design.co.uk
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -15,8 +15,9 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
```

### Comparing `django-photologue-3.8.1/django_photologue.egg-info/SOURCES.txt` & `django-photologue-3.9/django_photologue.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -15,45 +15,26 @@
 photologue/admin.py
 photologue/forms.py
 photologue/managers.py
 photologue/models.py
 photologue/sitemaps.py
 photologue/urls.py
 photologue/views.py
-photologue/contrib/old_style_templates/templates/photologue/gallery_archive.html
-photologue/contrib/old_style_templates/templates/photologue/gallery_archive_day.html
-photologue/contrib/old_style_templates/templates/photologue/gallery_archive_month.html
-photologue/contrib/old_style_templates/templates/photologue/gallery_archive_year.html
-photologue/contrib/old_style_templates/templates/photologue/gallery_detail.html
-photologue/contrib/old_style_templates/templates/photologue/gallery_list.html
-photologue/contrib/old_style_templates/templates/photologue/photo_archive.html
-photologue/contrib/old_style_templates/templates/photologue/photo_archive_day.html
-photologue/contrib/old_style_templates/templates/photologue/photo_archive_month.html
-photologue/contrib/old_style_templates/templates/photologue/photo_archive_year.html
-photologue/contrib/old_style_templates/templates/photologue/photo_detail.html
-photologue/contrib/old_style_templates/templates/photologue/photo_list.html
-photologue/contrib/old_style_templates/templates/photologue/root.html
-photologue/contrib/old_style_templates/templates/photologue/tags/next_in_gallery.html
-photologue/contrib/old_style_templates/templates/photologue/tags/prev_in_gallery.html
 photologue/locale/ca/LC_MESSAGES/django.mo
 photologue/locale/ca/LC_MESSAGES/django.po
 photologue/locale/cs/LC_MESSAGES/django.mo
 photologue/locale/cs/LC_MESSAGES/django.po
 photologue/locale/da/LC_MESSAGES/django.mo
 photologue/locale/da/LC_MESSAGES/django.po
-photologue/locale/da_DK/LC_MESSAGES/django.mo
-photologue/locale/da_DK/LC_MESSAGES/django.po
 photologue/locale/de/LC_MESSAGES/django.mo
 photologue/locale/de/LC_MESSAGES/django.po
 photologue/locale/en/LC_MESSAGES/django.mo
 photologue/locale/en/LC_MESSAGES/django.po
 photologue/locale/en_US/LC_MESSAGES/django.mo
 photologue/locale/en_US/LC_MESSAGES/django.po
-photologue/locale/es/LC_MESSAGES/django.mo
-photologue/locale/es/LC_MESSAGES/django.po
 photologue/locale/es_ES/LC_MESSAGES/django.mo
 photologue/locale/es_ES/LC_MESSAGES/django.po
 photologue/locale/eu/LC_MESSAGES/django.mo
 photologue/locale/eu/LC_MESSAGES/django.po
 photologue/locale/fr/LC_MESSAGES/django.mo
 photologue/locale/fr/LC_MESSAGES/django.po
 photologue/locale/hu/LC_MESSAGES/django.mo
@@ -89,14 +70,15 @@
 photologue/migrations/0004_auto_20140915_1259.py
 photologue/migrations/0005_auto_20141027_1552.py
 photologue/migrations/0006_auto_20141028_2005.py
 photologue/migrations/0007_auto_20150404_1737.py
 photologue/migrations/0008_auto_20150509_1557.py
 photologue/migrations/0009_auto_20160102_0904.py
 photologue/migrations/0010_auto_20160105_1307.py
+photologue/migrations/0011_auto_20190223_2138.py
 photologue/migrations/__init__.py
 photologue/res/sample.jpg
 photologue/res/test_nonsense.jpg
 photologue/res/test_photologue_&quoting.jpg
 photologue/res/test_photologue_landscape.jpg
 photologue/res/test_photologue_portrait.jpg
 photologue/res/test_photologue_square.jpg
```

### Comparing `django-photologue-3.8.1/PKG-INFO` & `django-photologue-3.9/django_photologue.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: django-photologue
-Version: 3.8.1
+Version: 3.9
 Summary: Powerful image management for the Django web framework.
-Home-page: https://github.com/jdriscoll/django-photologue
+Home-page: https://github.com/richardbarran/django-photologue
 Author: Justin Driscoll, Marcos Daniel Petry, Richard Barran
 Author-email: justin@driscolldev.com, marcospetry@gmail.com, richard@arbee-design.co.uk
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -15,8 +15,9 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
```

### Comparing `django-photologue-3.8.1/scripts/releaser_hooks.py` & `django-photologue-3.9/scripts/releaser_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import subprocess
 import os
 try:
     import polib
 except ImportError:
-    print('Prerelease hooks will not work as you have not installed polib.')
+    print('Msg to the package releaser: prerelease hooks will not work as you have not installed polib.')
     raise
 import copy
 import codecs
 
 
 def prereleaser_before(data):
     """
@@ -19,15 +19,15 @@
 
     """
     print('Running unit tests.')
     subprocess.check_output(["python", "example_project/manage.py", "test", "photologue"])
 
     print('Running PEP8 check.')
     # See setup.cfg for configuration options.
-    subprocess.check_output(["pep8"])
+    subprocess.check_output(["pycodestyle"])
 
     print('Checking that we have no outstanding DB migrations.')
     output = subprocess.check_output(["python", "example_project/manage.py", "makemigrations", "--dry-run",
                                       "photologue"])
     if not output == b"No changes detected in app 'photologue'\n":
         raise Exception('There are outstanding migrations for Photologue.')
```

### Comparing `django-photologue-3.8.1/LICENSE.txt` & `django-photologue-3.9/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2007-2017, Justin C. Driscoll and all the people named in CONTRIBUTORS.txt.
+Copyright (c) 2007-2018, Justin C. Driscoll and all the people named in CONTRIBUTORS.txt.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
     1. Redistributions of source code must retain the above copyright notice,
        this list of conditions and the following disclaimer.
```

### Comparing `django-photologue-3.8.1/README.rst` & `django-photologue-3.9/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Django-photologue
 =================
 .. image:: https://img.shields.io/pypi/v/django-photologue.svg
     :target: https://pypi.python.org/pypi/django-photologue/
     :alt: Latest PyPI version
 
-.. image:: https://img.shields.io/pypi/wheel/django-photologue.svg
-    :target: https://pypi.python.org/pypi/django-photologue/
-    :alt: Wheel Status
-    
-.. image:: https://travis-ci.org/jdriscoll/django-photologue.svg?branch=master
-    :target: https://travis-ci.org/jdriscoll/django-photologue
+.. image:: https://travis-ci.org/richardbarran/django-photologue.svg?branch=master
+    :target: https://travis-ci.org/richardbarran/django-photologue
+
+.. image:: https://coveralls.io/repos/github/richardbarran/django-photologue/badge.svg?branch=master
+    :target: https://coveralls.io/github/richardbarran/django-photologue?branch=master
 
-.. image:: https://coveralls.io/repos/jdriscoll/django-photologue/badge.png
-  :target: https://coveralls.io/r/jdriscoll/django-photologue
 
 A powerful image management and gallery application for the Django web framework. Upload photos, group them into
 galleries, apply effects such as watermarks.
 
 Take a closer look
 ------------------
 - We have a `demo website <http://www.django-photologue.net/>`_.
-- We also have some `examples of sites using Photologue 
-  <https://github.com/jdriscoll/django-photologue/wiki/Examples-and-forks>`_ on the wiki.
+- We also have some `examples of sites using Photologue
+  <https://github.com/richardbarran/django-photologue/wiki/Examples-and-forks>`_ on the wiki.
 
 Documentation
 -------------
-Please head over to our `online documentation at ReadTheDocs <https://django-photologue.readthedocs.io/en/stable/>`_ 
+Please head over to our `online documentation at ReadTheDocs <https://django-photologue.readthedocs.io/en/stable/>`_
 for instructions on installing and configuring this application.
 
 Python 3? Amazon S3?
 --------------------
 Yes! Photologue is CI tested against both Python 2 and Python 3.
 
-For S3, you'll have to install Boto, which for now is not compatible with Python 3 so you're stuck with Python 2.7...
+S3 also works with the standard BOTO package.
 
 Support
 -------
 If you have any questions or need help with any aspect of Photologue then please `join our mailing list
 <http://groups.google.com/group/django-photologue>`_.
 
 Travis CI status
```

### Comparing `django-photologue-3.8.1/photologue/locale/uk/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/uk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 # Translators:
 # Translators:
 # Dmytro Litvinov <litvinov.dmytro.it@gmail.com>, 2017
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
-"PO-Revision-Date: 2017-09-23 17:33+0000\n"
-"Last-Translator: Dmytro Litvinov <litvinov.dmytro.it@gmail.com>\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
+"Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Ukrainian (http://www.transifex.com/richardbarran/django-"
 "photologue/language/uk/)\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
+"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
+"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
+"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: admin.py:62
 #, python-format
 msgid ""
 "The following photo does not belong to the same site(s) as the gallery, so "
 "will never be displayed: %(photo_list)s."
 msgid_plural ""
@@ -34,35 +36,40 @@
 "ж вона не буде відображена %(photo_list)s"
 msgstr[1] ""
 "Наступні фотографії не відносяться до того ж сайту(сайтам), що і галерея, то "
 "ж вони не будуть відображені %(photo_list)s."
 msgstr[2] ""
 "Наступні фотографії не відносяться до того ж сайту(сайтам), що і галерея, то "
 "ж вони не будуть відображені %(photo_list)s"
+msgstr[3] ""
+"Наступні фотографії не відносяться до того ж сайту(сайтам), що і галерея, то "
+"ж вони не будуть відображені %(photo_list)s"
 
 #: admin.py:74
 #, python-format
 msgid "The gallery has been successfully added to %(site)s"
 msgid_plural "The galleries have been successfully added to %(site)s"
 msgstr[0] "Галерея була успішно додана до %(site)s"
 msgstr[1] "Галереї були успішно додані до%(site)s"
 msgstr[2] "Галереї були успішно додані до %(site)s"
+msgstr[3] "Галереї були успішно додані до %(site)s"
 
 #: admin.py:81
 msgid "Add selected galleries to the current site"
 msgstr "Додати вибрані галереї до поточного сайту"
 
 #: admin.py:87
 #, python-format
 msgid "The gallery has been successfully removed from %(site)s"
 msgid_plural ""
 "The selected galleries have been successfully removed from %(site)s"
 msgstr[0] "Галерея була успішно видалена з %(site)s"
 msgstr[1] "Вибрані галереї були успішно видалені з %(site)s"
 msgstr[2] "Вибрані галереї були успішно видалені з %(site)s"
+msgstr[3] "Вибрані галереї були успішно видалені з %(site)s"
 
 #: admin.py:94
 msgid "Remove selected galleries from the current site"
 msgstr "Видалити вибрані галереї з поточного сайту"
 
 #: admin.py:101
 #, python-format
@@ -70,14 +77,15 @@
 "All photos in gallery %(galleries)s have been successfully added to %(site)s"
 msgid_plural ""
 "All photos in galleries %(galleries)s have been successfully added to "
 "%(site)s"
 msgstr[0] "Всі фото в галереї %(galleries)s були успішно додані до %(site)s"
 msgstr[1] "Всі фото в галереях %(galleries)sбули успішно додані до %(site)s"
 msgstr[2] "Всі фото в галереях %(galleries)s були успішно додані до %(site)s"
+msgstr[3] "Всі фото в галереях %(galleries)s були успішно додані до %(site)s"
 
 #: admin.py:112
 msgid "Add all photos of selected galleries to the current site"
 msgstr "Додати всі фото з вибраних галерей до поточного сайту"
 
 #: admin.py:119
 #, python-format
@@ -86,531 +94,534 @@
 "%(site)s"
 msgid_plural ""
 "All photos in galleries %(galleries)s have been successfully removed from "
 "%(site)s"
 msgstr[0] "Усі фото з галереї %(galleries)s були упішно видели з%(site)s"
 msgstr[1] "Усі фото в галереях %(galleries)s були успішно видалені з %(site)s"
 msgstr[2] "Усі фото в галереях %(galleries)s були успішно видалені з %(site)s"
+msgstr[3] "Усі фото в галереях %(galleries)s були успішно видалені з %(site)s"
 
 #: admin.py:130
 msgid "Remove all photos in selected galleries from the current site"
 msgstr "Видалити всі фото у вибраних галереях з поточного сайту"
 
 #: admin.py:171
 #, python-format
 msgid "The photo has been successfully added to %(site)s"
 msgid_plural "The selected photos have been successfully added to %(site)s"
 msgstr[0] "Вибрані фото були успішно додані до сайту %(site)s"
 msgstr[1] "Вибрані фото були успішно додані до сайтів %(site)s"
 msgstr[2] "Вибрані фото були успішно додані до сайтів %(site)s"
+msgstr[3] "Вибрані фото були успішно додані до сайтів %(site)s"
 
 #: admin.py:178
 msgid "Add selected photos to the current site"
 msgstr "Додати вибрані фото до поточного сайту"
 
 #: admin.py:184
 #, python-format
 msgid "The photo has been successfully removed from %(site)s"
 msgid_plural "The selected photos have been successfully removed from %(site)s"
 msgstr[0] "Фото було успішно видалено з %(site)s"
 msgstr[1] "Вибрані фотографії було успішно видалено з %(site)s"
 msgstr[2] "Вибрані фотографії було успішно видалено з %(site)s"
+msgstr[3] "Вибрані фотографії було успішно видалено з %(site)s"
 
 #: admin.py:191
 msgid "Remove selected photos from the current site"
 msgstr "Видатили вибрані фото з поточного сайту"
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr "Завантажити Zip архів з фотографіями"
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr "Назва"
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 "Всім завантаженим фото отримають назву, яка складається з цієї назви + "
 "послідовний номер.  Це поле необхідне для створення нової галереї, але воно "
 "необов'язкове, коли додаєшь до існуючої галереї - якщо назва не вказана, "
 "назва фотографій буде складана з існюючого ім'я галереї."
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr "Галерея"
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Виберіть галерею для завантаження фотографій. Залиште поле пустим, щоб "
 "створити нову галерею з відповідною назвою."
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr "Підпис"
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "Підпис був додав до всіх фотографій."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr "Опис"
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr "Опис цієї Галереї. Необхідно тільки для нових галерей."
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr "Чи є загальнодоступним"
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 "Зніміть цю галку, щоб зробити завантажену галерею і всі фото в ній "
 "приватними."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr "Вже є така галерея з такою назвою."
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr "Виберіть існуюючу галерею чи введіть назву для нової галереї."
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 "Файл \"{filename}\" був пропущений, так як знаходиться в піддиректорії; всі "
 "фото повинні бути в кореневій директорії архіву."
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr "Не вдалось опрацювати файл \"{0}\" в .zip архіві."
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "Фото були додані до галереї \"{0}\"."
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Дуже низьке"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Низьке"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Чуть гірше за середнє"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Середнє"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Чуть краще середнього"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Високе"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Дуже високе"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Верхня сторона"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Права сторона"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Нижня сторона"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Ліва сторона"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Центр (за замовчуванням)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Зеркально відобразити зліва направо"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Зеркально відобразити зверху вниз"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Повернути на 90 градусів проти годинникової стрілки"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Повернути на 90 градусів за годинниковою стрілкою"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Повернути на 180 градусів"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Розмістити мозайкою"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Масштабувати"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 "Ланцюг з багатьма фільтрами використовує наступний шаблон \"FILTER_ONE-"
 ">FILTER_TWO->FILTER_THREE\". Фільтри для зображень будуть прийматись у "
 "порядку черги. Наступні фільтри доступні: %s"
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "дата публікації"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "назва"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "слаг назви"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "\"слаг\" - унікальна читабельна назва для об'єкта в адресній стрічці."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "опис"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "публічно"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Публічні галереї будуть відображенні на сторінках по замовчуванням."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "фотографії"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr "сайти"
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "галерея"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "галереї"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "кількість"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "зображення"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "вибрана дата"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 "Дані зображення були використані; воно утриється із зображення EXIF даних."
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr "кількість просмотрів"
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "обрізаний з"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "ефект"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "Розмір \"admin_thumbnal\" не визначен."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Мініатюра"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "слаг"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "підпис"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "дата завантаження"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr ""
 "Публічні фотографії будуть відображатись у використовуваємих уявленнях по "
 "замовчуванню."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "фото"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "ім'я"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "повернути чи зеркально відобразити"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "колір"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 "Значення 0.0 дає чорно-біле відображення, а 1.0 віддає оригінальне "
 "зображення."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "яскравість"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr "Значення 0.0 дає чорне зображення, а 1.0 - оригінальне зображення."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "контраст"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Значення 0.0 дає суцільно сіре відображення, а 1.0 віддає оригінальне "
 "зображення."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "різкість"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Значення 0.0 дає розмите відображення, а 1.0 віддає оригінальне зображення."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "фільтри"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "розмір"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "Висота відбиття у відсотках від оригінального зображення. Коефіцієнт 0.0 не "
 "додає відбиття, коефіціент 1.0 додає відбиття рівний висоті оригінального "
 "зображення.  "
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "сила"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr "Початкова непрозорість градієнта відблиска."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 "Колір фона градієнта відображення. Відмітьте це для відповідності кольора "
 "фона вашої сторінки."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "фото-ефект"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "фото-ефекти"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "стиль"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "непрозорість"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "Непрозорість накладення."
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "водяний знак"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "водяні знаки"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "Название размера фотографии должно содержать только буквы, числа и символы "
 "подчеркивания. Примеры: \\\"thumbnail\\\", \\\"display\\\", \\\"small\\\", \\"
 "\"main_page_widget\\\n"
 "\n"
 "Назва розміра фотографії повинно мати тільки букви, числа та символи "
 "підкреслення. Наприклад: \"thumbnail\", \"display\", \"small\", "
 "\"main_page_widget\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "ширина"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Якщо ширина виставлено в \"0\", то зображення буде масштабоване по висоті."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "висота"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Якщо висота виставлено в \"0\", то зображення буде масштабоване по ширині"
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "якість"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "якість JPEG зображення"
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "збільшити фото?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "Якщо вибрано, то зображення буде масштабоване у випадку необхідності, щоб "
 "відповідати розмірам.  Обрізані розміри будуть масшабовані незалежно від "
 "цієї настройки."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "обрізати?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr "Якщо вибрано, то зображення буде замаштабоване та обрізано по розміру."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "кешувати?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr "Якщо вибрано, то розмір фото буде закешован при додаванні фото."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "збільшити лічильник просмотрів?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Якщо вибрано, то \"view_count\" зображення  буде збільшено, коли показується "
 "цей розмір фотографії"
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "Водяний знак"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "розмір фотографії"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "Розміри фотографій"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr "Можна обрізати фотографії, якщо встановлені ширина на висота."
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr "Завантажити zip архів"
```

### Comparing `django-photologue-3.8.1/photologue/locale/uk/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/uk/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
-"PO-Revision-Date: 2017-09-23 17:33+0000\n"
-"Last-Translator: Dmytro Litvinov <litvinov.dmytro.it@gmail.com>\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
+"Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Ukrainian (http://www.transifex.com/richardbarran/django-"
 "photologue/language/uk/)\n"
+"Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: uk\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
+"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
+"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
+"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 msgid ""
 "\n"
 "\t\t\t\t    page %(page_number)s of %(total_pages)s\n"
 "\t\t\t\t"
 msgstr ""
 "\n"
@@ -94,24 +95,26 @@
 "All photos in gallery %(galleries)s have been successfully added to %(site)s"
 msgid_plural ""
 "All photos in galleries %(galleries)s have been successfully added to "
 "%(site)s"
 msgstr[0] "Всі фото в галереї %(galleries)s були успішно додані до %(site)s"
 msgstr[1] "Всі фото в галереях %(galleries)sбули успішно додані до %(site)s"
 msgstr[2] "Всі фото в галереях %(galleries)s були успішно додані до %(site)s"
+msgstr[3] "Всі фото в галереях %(galleries)s були успішно додані до %(site)s"
 
 msgid ""
 "All photos in gallery %(galleries)s have been successfully removed from "
 "%(site)s"
 msgid_plural ""
 "All photos in galleries %(galleries)s have been successfully removed from "
 "%(site)s"
 msgstr[0] "Усі фото з галереї %(galleries)s були упішно видели з%(site)s"
 msgstr[1] "Усі фото в галереях %(galleries)s були успішно видалені з %(site)s"
 msgstr[2] "Усі фото в галереях %(galleries)s були успішно видалені з %(site)s"
+msgstr[3] "Усі фото в галереях %(galleries)s були успішно видалені з %(site)s"
 
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
@@ -362,27 +365,32 @@
 "ж вона не буде відображена %(photo_list)s"
 msgstr[1] ""
 "Наступні фотографії не відносяться до того ж сайту(сайтам), що і галерея, то "
 "ж вони не будуть відображені %(photo_list)s."
 msgstr[2] ""
 "Наступні фотографії не відносяться до того ж сайту(сайтам), що і галерея, то "
 "ж вони не будуть відображені %(photo_list)s"
+msgstr[3] ""
+"Наступні фотографії не відносяться до того ж сайту(сайтам), що і галерея, то "
+"ж вони не будуть відображені %(photo_list)s"
 
 msgid "The gallery has been successfully added to %(site)s"
 msgid_plural "The galleries have been successfully added to %(site)s"
 msgstr[0] "Галерея була успішно додана до %(site)s"
 msgstr[1] "Галереї були успішно додані до%(site)s"
 msgstr[2] "Галереї були успішно додані до %(site)s"
+msgstr[3] "Галереї були успішно додані до %(site)s"
 
 msgid "The gallery has been successfully removed from %(site)s"
 msgid_plural ""
 "The selected galleries have been successfully removed from %(site)s"
 msgstr[0] "Галерея була успішно видалена з %(site)s"
 msgstr[1] "Вибрані галереї були успішно видалені з %(site)s"
 msgstr[2] "Вибрані галереї були успішно видалені з %(site)s"
+msgstr[3] "Вибрані галереї були успішно видалені з %(site)s"
 
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "Висота відбиття у відсотках від оригінального зображення. Коефіцієнт 0.0 не "
@@ -396,20 +404,22 @@
 msgstr "Непрозорість накладення."
 
 msgid "The photo has been successfully added to %(site)s"
 msgid_plural "The selected photos have been successfully added to %(site)s"
 msgstr[0] "Вибрані фото були успішно додані до сайту %(site)s"
 msgstr[1] "Вибрані фото були успішно додані до сайтів %(site)s"
 msgstr[2] "Вибрані фото були успішно додані до сайтів %(site)s"
+msgstr[3] "Вибрані фото були успішно додані до сайтів %(site)s"
 
 msgid "The photo has been successfully removed from %(site)s"
 msgid_plural "The selected photos have been successfully removed from %(site)s"
 msgstr[0] "Фото було успішно видалено з %(site)s"
 msgstr[1] "Вибрані фотографії було успішно видалено з %(site)s"
 msgstr[2] "Вибрані фотографії було успішно видалено з %(site)s"
+msgstr[3] "Вибрані фотографії було успішно видалено з %(site)s"
 
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "Фото були додані до галереї \"{0}\"."
 
 msgid "This photo is found in the following galleries"
 msgstr "Це фото знайдено у наступних галереях"
```

### Comparing `django-photologue-3.8.1/photologue/locale/sk/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/sk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,57 +8,61 @@
 # saboter <translations@pymutan.com>, 2014
 # saboter <translations@pymutan.com>, 2014
 # saboter <translations@pymutan.com>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
-"PO-Revision-Date: 2017-09-23 18:41+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Slovak (http://www.transifex.com/richardbarran/django-"
 "photologue/language/sk/)\n"
 "Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 #: admin.py:62
 #, python-format
 msgid ""
 "The following photo does not belong to the same site(s) as the gallery, so "
 "will never be displayed: %(photo_list)s."
 msgid_plural ""
 "The following photos do not belong to the same site(s) as the gallery, so "
 "will never be displayed: %(photo_list)s."
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
+msgstr[3] ""
 
 #: admin.py:74
 #, python-format
 msgid "The gallery has been successfully added to %(site)s"
 msgid_plural "The galleries have been successfully added to %(site)s"
 msgstr[0] "Galéria bola úspešne pridaná na %(site)s"
 msgstr[1] "Galérie boli úspešne pridané na %(site)s"
 msgstr[2] "Galérie boli úspešne pridané na %(site)s"
+msgstr[3] "Galérie boli úspešne pridané na %(site)s"
 
 #: admin.py:81
 msgid "Add selected galleries to the current site"
 msgstr "Pridať vybrané galérie na aktuálnu stránku"
 
 #: admin.py:87
 #, python-format
 msgid "The gallery has been successfully removed from %(site)s"
 msgid_plural ""
 "The selected galleries have been successfully removed from %(site)s"
 msgstr[0] "Galéria bola úspešne odobratá zo %(site)s"
 msgstr[1] "Označené galérie boli úspešne odobrané zo %(site)s"
 msgstr[2] "Označené galérie boli úspešne odobrané zo %(site)s"
+msgstr[3] "Označené galérie boli úspešne odobrané zo %(site)s"
 
 #: admin.py:94
 msgid "Remove selected galleries from the current site"
 msgstr "Odobrať označené galérie z aktuálnej stránky"
 
 #: admin.py:101
 #, python-format
@@ -72,14 +76,17 @@
 "%(site)s"
 msgstr[1] ""
 "Všetky fotografie z galérií %(galleries)s boli úspešne pridané na stránku "
 "%(site)s"
 msgstr[2] ""
 "Všetky fotografie z galérií %(galleries)s boli úspešne pridané na stránku "
 "%(site)s"
+msgstr[3] ""
+"Všetky fotografie z galérií %(galleries)s boli úspešne pridané na stránku "
+"%(site)s"
 
 #: admin.py:112
 msgid "Add all photos of selected galleries to the current site"
 msgstr "Pridať všetky fotografie z označených galérií do aktuálnej stránky"
 
 #: admin.py:119
 #, python-format
@@ -94,516 +101,521 @@
 "%(site)s"
 msgstr[1] ""
 "Všetky fotografie z galérií %(galleries)s boli úspešne odobraté zo stránky "
 "%(site)s"
 msgstr[2] ""
 "Všetky fotografie z galérií %(galleries)s boli úspešne odobraté zo stránky "
 "%(site)s"
+msgstr[3] ""
+"Všetky fotografie z galérií %(galleries)s boli úspešne odobraté zo stránky "
+"%(site)s"
 
 #: admin.py:130
 msgid "Remove all photos in selected galleries from the current site"
 msgstr "Odobrať všetky fotografie z vybraných galérií z aktuálnej stránky"
 
 #: admin.py:171
 #, python-format
 msgid "The photo has been successfully added to %(site)s"
 msgid_plural "The selected photos have been successfully added to %(site)s"
 msgstr[0] "Fotografia bola úspešne pridaná na %(site)s"
 msgstr[1] "Označené fotografie boli úspešne pridané na %(site)s"
 msgstr[2] "Označené fotografie boli úspešne pridané na %(site)s"
+msgstr[3] "Označené fotografie boli úspešne pridané na %(site)s"
 
 #: admin.py:178
 msgid "Add selected photos to the current site"
 msgstr "Pridať označené fotografie na aktuálnu stránku"
 
 #: admin.py:184
 #, python-format
 msgid "The photo has been successfully removed from %(site)s"
 msgid_plural "The selected photos have been successfully removed from %(site)s"
 msgstr[0] "Fotografia bola úspešne odobratá zo %(site)s"
 msgstr[1] "Označené fotografie boli úspešne odobraté zo %(site)s"
 msgstr[2] "Označené fotografie boli úspešne odobraté zo %(site)s"
+msgstr[3] "Označené fotografie boli úspešne odobraté zo %(site)s"
 
 #: admin.py:191
 msgid "Remove selected photos from the current site"
 msgstr " Odobrať označené fotografie z aktuálnej stránky"
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr "Nahrať ZIP archív s fotkami"
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr "Titulok"
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr "Galéria"
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Vyberte galériu do ktorej chcete pridať tieto obrázky. Pre vytvorenie novej "
 "galérie so zadaným názvom ponechajte toto pole prázdne."
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr "Titulok"
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "Titulok bude pridaný do všetkých fotografií."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr "Popis"
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr "Je verejná"
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr "Odškrtnite, aby odovzdané galérie a zahrnuté fotografie boli súkromné."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr "Galéria s týmto názvom už existuje."
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr "Vyberte existujúcu galériu, alebo vyplnte názov pre novú."
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 "Ignorujem súbor \"{filename}\" nakoľko je v podadresári, všetky obrázky by "
 "mali byť priamo v zip archíve bez vnorenej adresárovej štruktúry."
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr "Nepodarilo sa spracovať súbor \"{0}\" v .zip archíve."
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "Fotografie boli pridané do galérie \"{0}\". "
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Veľmi Nízka"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Nízka"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Stredne-Nízka"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Stredná"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Stredne-Vysoká"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Vysoká"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Veľmi Vysoká"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Hore"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Vpravo"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Dole"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Vľavo"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Stred (Štandardne)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Prevrátiť zľava doprava"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Prevrátiť zhora nadol"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Otočiť o 90 stupňov proti smeru hodinových ručičiek"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Otočiť o 90 stupňov v smere hodinových ručičiek"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Otočiť o 180 stupňov"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Dláždiť"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Dodržať mierku"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 "Zreťazte viac filtrov pomocou nasledovného vzoru \"FILTER_JEDNA->FILTER_DVA-"
 ">FILTER_TRI\". Obrázkové filtre budú použité v poradí. Nasledujúce filtre sú "
 "k dispozícii: %s."
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "dátum zverejnenia"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "názov"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "identifikátor názvu"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "\"Identifikátor\" je unikátny názov objektu vhodný pre použitie v URL."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "popis"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "je verejný"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Verejné galérie budú zobrazené v štandardných zobrazeniach."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "fotografie"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr "stránky"
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "galéria"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "galérie"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "počet"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "obrázok"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "dátum odfotenia"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr "počet zobrazení"
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "orezať od"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "efekt"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "Veľkosť fotografie \"admin_thumbnail\" nebola definovaná."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Náhľad"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "identifikátor"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "titulok"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "dátum pridania"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr "Verejné fotografie budú zobrazené v štandardných zobrazeniach."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "fotografia"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "meno"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "otočiť alebo prevrátiť"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "farba"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr "Faktor 0.0 dáva čiernobiely obrázok, faktor 1.0 dáva pôvodný obrázok."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "jas"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr "Faktor 0.0 dáva čierny obrázok, faktor 1.0 dáva pôvodný obrázok."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "kontrast"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr "Faktor 0.0 dáva šedý obrázok, faktor 1.0 dáva pôvodný obrázok."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "ostrosť"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr "Faktor 0.0 dáva rozmazaný obrázok, faktor 1.0 dáva pôvodný obrázok."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "filtre"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "veľkosť"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "Výška odrazu v percentách pôvodného obrázku. Faktor 0.0 nepridáva žiadny "
 "odraz, faktor 1.0 pridáva odraz rovný výśke pôvodného obrázku."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "intenzita"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr "Počiatočná presvitnosť odrazového gradientu."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 "Farba pozadia odrazového gradientu. Túto položku nastavte tak, aby sa "
 "zhodovala s farbou pozadia vašej stránky."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "efekt fotografie"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "efekty fotografie"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "štýl"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "priesvitnosť"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "Priesvitnosť prekrytia."
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "vodoznak"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "vodoznaky"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "Názov veľkosti fotografie by mal obsahovať len písmená, čísla a podčiarky. "
 "Príklady:  \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "šírka"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Ak je šírka nastavená na \"0\" obrázok bude podľa mierky upravený na zadanú "
 "výšku."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "výška"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Ak je výška nastavená na \"0\" obrázok bude podľa mierky upravený na zadanú "
 "šírku"
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "kvalita"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "JPEG kvalita obrázku."
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "prispôsobiť obzázky?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "Ak je táto položka vybratá a je to potrebné, obrázok bude prispôsobený tak, "
 "aby sa zmestil do zadaných rozmerov."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "orezať ak je to potrebné ?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "Ak je táto položka vybratá, obrázok bude upravený a orezaný, aby sa zmestil "
 "do zadaných rozmerov."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "pred-generovať ?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 "Ak je táto položka vybratá, veľkosť fotografie bude pred-generovaná počas "
 "pridávania fotografií."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "zvýšiť počet zobrazení?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Ak je táto položka vybratá, \"view_count\" obrázku bude zvýšený, keď sa "
 "zobrazí veľkosť tohto obrázku."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "použiť vodoznak na obrázok"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "veľkosť fotografie"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "veľkosti fotografie"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr "Fotky môžete orezať len vtedy, ak je nastavená šírka a výška."
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr "Nahrať ZIP archív"
```

### Comparing `django-photologue-3.8.1/photologue/locale/sk/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/sk/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
-"PO-Revision-Date: 2017-09-23 18:41+0000\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Slovak (http://www.transifex.com/richardbarran/django-"
 "photologue/language/sk/)\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: sk\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 msgid ""
 "\n"
 "\t\t\t\t    page %(page_number)s of %(total_pages)s\n"
 "\t\t\t\t"
 msgstr ""
 "\n"
@@ -92,14 +92,17 @@
 "%(site)s"
 msgstr[1] ""
 "Všetky fotografie z galérií %(galleries)s boli úspešne pridané na stránku "
 "%(site)s"
 msgstr[2] ""
 "Všetky fotografie z galérií %(galleries)s boli úspešne pridané na stránku "
 "%(site)s"
+msgstr[3] ""
+"Všetky fotografie z galérií %(galleries)s boli úspešne pridané na stránku "
+"%(site)s"
 
 msgid ""
 "All photos in gallery %(galleries)s have been successfully removed from "
 "%(site)s"
 msgid_plural ""
 "All photos in galleries %(galleries)s have been successfully removed from "
 "%(site)s"
@@ -108,14 +111,17 @@
 "%(site)s"
 msgstr[1] ""
 "Všetky fotografie z galérií %(galleries)s boli úspešne odobraté zo stránky "
 "%(site)s"
 msgstr[2] ""
 "Všetky fotografie z galérií %(galleries)s boli úspešne odobraté zo stránky "
 "%(site)s"
+msgstr[3] ""
+"Všetky fotografie z galérií %(galleries)s boli úspešne odobraté zo stránky "
+"%(site)s"
 
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "Veľkosť fotografie \"admin_thumbnail\" nebola definovaná."
 
 msgid "Bottom"
 msgstr "Dole"
 
@@ -339,21 +345,23 @@
 "zhodovala s farbou pozadia vašej stránky."
 
 msgid "The gallery has been successfully added to %(site)s"
 msgid_plural "The galleries have been successfully added to %(site)s"
 msgstr[0] "Galéria bola úspešne pridaná na %(site)s"
 msgstr[1] "Galérie boli úspešne pridané na %(site)s"
 msgstr[2] "Galérie boli úspešne pridané na %(site)s"
+msgstr[3] "Galérie boli úspešne pridané na %(site)s"
 
 msgid "The gallery has been successfully removed from %(site)s"
 msgid_plural ""
 "The selected galleries have been successfully removed from %(site)s"
 msgstr[0] "Galéria bola úspešne odobratá zo %(site)s"
 msgstr[1] "Označené galérie boli úspešne odobrané zo %(site)s"
 msgstr[2] "Označené galérie boli úspešne odobrané zo %(site)s"
+msgstr[3] "Označené galérie boli úspešne odobrané zo %(site)s"
 
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "Výška odrazu v percentách pôvodného obrázku. Faktor 0.0 nepridáva žiadny "
@@ -366,20 +374,22 @@
 msgstr "Priesvitnosť prekrytia."
 
 msgid "The photo has been successfully added to %(site)s"
 msgid_plural "The selected photos have been successfully added to %(site)s"
 msgstr[0] "Fotografia bola úspešne pridaná na %(site)s"
 msgstr[1] "Označené fotografie boli úspešne pridané na %(site)s"
 msgstr[2] "Označené fotografie boli úspešne pridané na %(site)s"
+msgstr[3] "Označené fotografie boli úspešne pridané na %(site)s"
 
 msgid "The photo has been successfully removed from %(site)s"
 msgid_plural "The selected photos have been successfully removed from %(site)s"
 msgstr[0] "Fotografia bola úspešne odobratá zo %(site)s"
 msgstr[1] "Označené fotografie boli úspešne odobraté zo %(site)s"
 msgstr[2] "Označené fotografie boli úspešne odobraté zo %(site)s"
+msgstr[3] "Označené fotografie boli úspešne odobraté zo %(site)s"
 
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "Fotografie boli pridané do galérie \"{0}\". "
 
 msgid "This photo is found in the following galleries"
 msgstr "Táto fotka sa nachádza v nasledujúcich galériách"
```

### Comparing `django-photologue-3.8.1/photologue/locale/pl/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/pl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
 "PO-Revision-Date: 2017-09-19 14:01+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Polish (http://www.transifex.com/richardbarran/django-"
 "photologue/language/pl/)\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -120,484 +120,484 @@
 msgid "Remove selected photos from the current site"
 msgstr ""
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr ""
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr ""
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr ""
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "Podpis będzie dodany do wszystkich zdjęć."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr ""
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr ""
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 "Odznacz aby uczynić wrzucaną galerię oraz zawarte w niej zdjęcia prywatnymi."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr ""
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr ""
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr ""
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr ""
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Bardzo niska"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Niska"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Niższa średnia"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Średnia"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Wyższa średnia"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Wysoka"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Bardzo wysoka"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Góra"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Prawo"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Dół"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Lewo"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Środek (Domyślnie)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Odbij w poziomie"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Odbij w pionie"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Odwróć 90 stopni w lewo"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Odwróć 90 stopni w prawo"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Obróć o 180 stopni"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Kafelki"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Skaluj"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "data publikacji"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "tytuł"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "tytuł - slug "
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "\"Slug\" jest unikalnym, zgodnym z formatem dla URL-i tytułem obiektu."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "opis"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "jest publiczna"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Galerie publiczne będą wyświetlana w domyślnych widokach."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "zdjęcia"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr ""
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "galeria"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "galerie"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "ilość"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "obraz"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "data wykonania"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr ""
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "obetnij z"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "efekt"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "Rozmiar zdjęcia \"admin_thumbnail\" nie został zdefiniowany."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Miniaturka"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "slug"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "podpis"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "data dodania"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr "Publiczne zdjęcia będą wyświetlane w domyślnych widokach."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "zdjęcie"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "nazwa"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "obróć lub odbij"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "kolor"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 "Współczynnik 0.0 daje czarno-biały obraz, współczynnik 1.0 daje obraz "
 "oryginalny."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "jasność"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Współczynnik 0.0 daje czarny obraz, współczynnik 1.0 daje obraz oryginalny."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "kontrast"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Współczynnik 0.0 daje jednolity szary obraz, współczynnik 1.0 daje obraz "
 "oryginalny."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "ostrość"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Współczynnik 0.0 daje rozmazany obraz, współczynnik 1.0 daje obraz "
 "oryginalny."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "filtry"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "rozmiar"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "Wysokość odbicia jako procent oryginalnego obrazu. Współczynnik 0.0 nie "
 "dodaje odbicia, współczynnik 1.0 dodaje odbicie równe wysokości oryginalnego "
 "obrazu."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "intensywność"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr ""
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "efekt zdjęcia"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "efekty zdjęć"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "styl"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "przeźroczystość"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "Poziom przezroczystości"
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "znak wodny"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "znaki wodne"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "Nazwa rozmiaru zdjęcia powinna zawierać tylko litery, cyfry i podkreślenia. "
 "Przykłady: \"miniatura\", \"wystawa\", \"male\", \"widget_strony_glownej\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "szerokość"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Jeśli szerokość jest ustawiona na \"0\" to obraz będzie skalowany do podanej "
 "wysokości."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "wysokość"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Jeśli wysokość jest ustawiona na \"0\" to obraz będzie skalowany do podanej "
 "szerokości."
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "jakość"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "Jakość obrazu JPEG"
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "skalować obrazy w górę?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "Jeśli zaznaczone to obraz będzie skalowany w górę tak aby pasował do "
 "podanych wymiarów. Obcinane rozmiary będą skalowane niezależnie od tego "
 "ustawienia."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "przyciąć aby pasował?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "Jeśli zaznaczone to obraz będzie skalowany i przycinany tak aby pasował do "
 "podanych wymiarów."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "wstępnie cachować?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 "Jesli zaznaczone to ten rozmiar zdjęć będzie wstępnie cachowany przy "
 "dodawaniu zdjęć."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "zwiększyć licznik odsłon?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Jeśli zaznaczone to \"licznik_odslon\" będzie zwiększany gdy ten rozmiar "
 "zdjęcia będzie wyświetlany."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "oznacz kluczem wodnym"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "rozmiar zdjęcia"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "rozmiary zdjęć"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr ""
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/pl/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/pl/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
 "PO-Revision-Date: 2017-09-19 14:01+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Polish (http://www.transifex.com/richardbarran/django-"
 "photologue/language/pl/)\n"
+"Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "\"Slug\" jest unikalnym, zgodnym z formatem dla URL-i tytułem obiektu."
```

### Comparing `django-photologue-3.8.1/photologue/locale/eu/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/eu/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 # Translators:
-# Urtzi Odriozola <urtzi.odriozola@gmail.com>, 2016
+# Urtzi Odriozola <urtzi.odriozola@gmail.com>, 2016,2018
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
-"PO-Revision-Date: 2017-09-19 18:58+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
+"PO-Revision-Date: 2018-03-15 09:14+0000\n"
 "Last-Translator: Urtzi Odriozola <urtzi.odriozola@gmail.com>\n"
 "Language-Team: Basque (http://www.transifex.com/richardbarran/django-"
 "photologue/language/eu/)\n"
 "Language: eu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -112,471 +112,471 @@
 msgid "Remove selected photos from the current site"
 msgstr "Ezabatu aukeratutako argazkiak uneko webgunetik."
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr "Igo argazkien zip artxiboa"
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr "Izenburua"
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr "Galeria"
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Aukeratu irudi hau gehitzeko galeria. Utzi hau hutsik emandako izenburutik "
 "galeria berri bat sortzeko."
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr "Irudi testua"
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "Irudi testua argazki guztiei gehituko zaie."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr "Deskribapena"
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 "Galeria honen deskribapena. Galeria berrientzat bakarrik da beharrezkoa."
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr "Publikoa da"
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 "Ez markatu hau igotako galeria eta bertako argazkiak pribatu izatea nahi "
 "baduzu."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr "Izenburu hori duen galeria existitzen da."
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr ""
 "Aukeratu existitzen den galeria edo sartu galeria berri baten izenburua."
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr "Ezin izan da .zip artxiboko \"{0}\" fitxategia prozesatu."
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "Argazkiak \"{0}\" galeriara gehitu dira."
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Oso baxua"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Baxua"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Ertaina-Baxua"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Ertaina"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Ertaina-Altua"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Altua"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Oso altua"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Goia"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Eskuina"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Behea"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Ezkerra"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Erdia (Lehenetsia)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Itzuli eskerretik eskuinera"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Itzuli goitik behera"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Biratu 90 gradu erlojuaren kontrako norantzan"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Biratu 90 gradu erloju norantzan"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Biratu 180 gradu"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
-msgstr ""
+msgstr "Lauza"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
-msgstr ""
+msgstr "Tamaina"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "argitaratze data"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "izenburua"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "izenburuaren sluga"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr ""
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "deskribapena"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "publikoa da"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr ""
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "argazkiak"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr "webguneak"
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "galeria"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "galeriak"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "zenbatu"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "irudia"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr ""
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr "Irudia atera zeneko data; irudiaren EXIF datutik hartzen da."
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr ""
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "moztu hemendik"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "efektua"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr ""
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr ""
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "slug"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "irudi testua"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr ""
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr ""
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "argazkia"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "izena"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "biratu edo itzuli"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "kolorea"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "dizdira"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "kontrastea"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "zorroztasuna"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "filtroak"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "tamaina"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "indarra"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr ""
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "argazki efektua"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "argazki efektuak"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "estiloa"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "opakutasun"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "Estalkiaren opakutasuna."
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "ur marka"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "ur markak"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "Irudiaren tamaina izenak hizkiak, zenbakiak eta beheko marrak bakarrik izan "
 "ditzake. Adibidez: \"thumbnail\", \"display\", \"small\", \"main_page_widget"
 "\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "zabalera"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Zabaleran \"0\" jarriz gero, irudiaren tamaina altueraren arabera ezarriko "
 "da."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "altuera"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Altueran \"0\" jarriz gero, irudiaren tamaina zabaleraren arabera ezarriko "
 "da."
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "kalitatea"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "JPEG irudi kalitatea."
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "irudiak handitu?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "neurrira moztu?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "aurrez katxeatu?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
-msgstr ""
+msgstr "ikustaldi kopurua zenbatu?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "jarri ur marka irudiari"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "argazki tamaina"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "argazki tamainak"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr ""
 "Zabalera eta altuera definituta badaude bakarrik moztu daitezke irudiak."
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr "Igo zip fitxategia"
```

### Comparing `django-photologue-3.8.1/photologue/locale/eu/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/eu/LC_MESSAGES/django.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
-"PO-Revision-Date: 2017-09-19 18:58+0000\n"
+"PO-Revision-Date: 2018-03-15 09:14+0000\n"
 "Last-Translator: Urtzi Odriozola <urtzi.odriozola@gmail.com>\n"
 "Language-Team: Basque (http://www.transifex.com/richardbarran/django-"
 "photologue/language/eu/)\n"
+"Language: eu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: eu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "\n"
 "\t\t\t\t    page %(page_number)s of %(total_pages)s\n"
 "\t\t\t\t"
 msgstr ""
@@ -223,14 +222,17 @@
 
 msgid "Rotate 90 degrees clockwise"
 msgstr "Biratu 90 gradu erloju norantzan"
 
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Biratu 90 gradu erlojuaren kontrako norantzan"
 
+msgid "Scale"
+msgstr "Tamaina"
+
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Aukeratu irudi hau gehitzeko galeria. Utzi hau hutsik emandako izenburutik "
 "galeria berri bat sortzeko."
 
@@ -264,14 +266,17 @@
 
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "Argazkiak \"{0}\" galeriara gehitu dira."
 
 msgid "This photo is found in the following galleries"
 msgstr "Argazki hau ondorengo galerietan aurkitu da"
 
+msgid "Tile"
+msgstr "Lauza"
+
 msgid "Title"
 msgstr "Izenburua"
 
 msgid "Top"
 msgstr "Goia"
 
 msgid ""
@@ -354,14 +359,17 @@
 
 msgid "height"
 msgstr "altuera"
 
 msgid "image"
 msgstr "irudia"
 
+msgid "increment view count?"
+msgstr "ikustaldi kopurua zenbatu?"
+
 msgid "is public"
 msgstr "publikoa da"
 
 msgid "name"
 msgstr "izena"
 
 msgid "opacity"
```

### Comparing `django-photologue-3.8.1/photologue/locale/cs/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/cs/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -8,57 +8,61 @@
 # Jakub Dorňák <jakub.dornak@misli.cz>, 2013
 # Jakub Dorňák <jakub.dornak@misli.cz>, 2013
 # Viktor Matys <v.matys@seznam.cz>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
 "PO-Revision-Date: 2017-09-23 19:18+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Czech (http://www.transifex.com/richardbarran/django-"
 "photologue/language/cs/)\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
 #: admin.py:62
 #, python-format
 msgid ""
 "The following photo does not belong to the same site(s) as the gallery, so "
 "will never be displayed: %(photo_list)s."
 msgid_plural ""
 "The following photos do not belong to the same site(s) as the gallery, so "
 "will never be displayed: %(photo_list)s."
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
+msgstr[3] ""
 
 #: admin.py:74
 #, python-format
 msgid "The gallery has been successfully added to %(site)s"
 msgid_plural "The galleries have been successfully added to %(site)s"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
+msgstr[3] ""
 
 #: admin.py:81
 msgid "Add selected galleries to the current site"
 msgstr ""
 
 #: admin.py:87
 #, python-format
 msgid "The gallery has been successfully removed from %(site)s"
 msgid_plural ""
 "The selected galleries have been successfully removed from %(site)s"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
+msgstr[3] ""
 
 #: admin.py:94
 msgid "Remove selected galleries from the current site"
 msgstr ""
 
 #: admin.py:101
 #, python-format
@@ -66,14 +70,15 @@
 "All photos in gallery %(galleries)s have been successfully added to %(site)s"
 msgid_plural ""
 "All photos in galleries %(galleries)s have been successfully added to "
 "%(site)s"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
+msgstr[3] ""
 
 #: admin.py:112
 msgid "Add all photos of selected galleries to the current site"
 msgstr ""
 
 #: admin.py:119
 #, python-format
@@ -82,515 +87,518 @@
 "%(site)s"
 msgid_plural ""
 "All photos in galleries %(galleries)s have been successfully removed from "
 "%(site)s"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
+msgstr[3] ""
 
 #: admin.py:130
 msgid "Remove all photos in selected galleries from the current site"
 msgstr ""
 
 #: admin.py:171
 #, python-format
 msgid "The photo has been successfully added to %(site)s"
 msgid_plural "The selected photos have been successfully added to %(site)s"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
+msgstr[3] ""
 
 #: admin.py:178
 msgid "Add selected photos to the current site"
 msgstr ""
 
 #: admin.py:184
 #, python-format
 msgid "The photo has been successfully removed from %(site)s"
 msgid_plural "The selected photos have been successfully removed from %(site)s"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
+msgstr[3] ""
 
 #: admin.py:191
 msgid "Remove selected photos from the current site"
 msgstr ""
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr ""
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr ""
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Vyberte fotogalerii, do které se mají tyto obrázky přidat. Ponechte prázdné "
 "pro vytvoření nové fotogalerie s daným názvem."
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr ""
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "Titulek bude přidán ke všem fotografiím."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr "Popis"
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr "Je veřejné"
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 "Zrušte zaškrtnutí, pokud chcete, aby byla nově nahraná fotogalerie neveřejná."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr "Již existuje galerie s tímto titulkem."
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr "Vyberte existující galerii, nebo zadejte titulek pro novou galerii."
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr "Nešlo zpracovat soubor \"{0}\" v zip archivu."
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "Fotografie byly přidány do galerie  \"{0}\"."
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Velmi nízká"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Nízká"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Nížší střední"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Střední"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Vyšší střední"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Vysoká"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Velmi vysoká"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Nahoře"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Vpravo"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Dole"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Vlevo"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Uprostřed (výchozí)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Obrátit vodorovně"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Obrátit svisle"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Otočit o 90 stupňů vlevo"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Otočit o 90 stupňů vpravo"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Otočit o 180 stupňů"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Dláždit"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Přizpůsobit velikost"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 "Zřetězte více filtrů použitím vzoru „PRVNI_FILTR->DRUHY_FILTR-"
 ">TRETI_FILTR“.\n"
 "Filtry budou aplikovány v daném pořadí. K dispozici jsou tyto filtry: %s."
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "datum zveřejnění"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "název"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "identifikátor"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "Unikátní název, který bude použit v URL adrese (bez diakritiky)."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "popis"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "veřejné"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Veřejné fotogalerie budou zobrazeny ve výchozích pohledech."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "fotografie"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr ""
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "fotogalerie"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "fotogalerie"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "počet"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "obrázek"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "datum pořízení"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr "počet zobrazení"
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "oříznout"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "efekt"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "Velikost „admin_thumbnail“ není definovaná."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Náhled"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "identifikátor"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "titulek"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "datum přidání"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr "Veřejné fotografie budou zobrazeny ve výchozích pohledech."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "fotografie"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "název"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "obrátit nebo otočit"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "barva"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 "Hodnota 0,0 udělá černobílý obrázek, hodnota 1,0 zachová původní barvy."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "jas"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr "Hodnota 0,0 udělá černý obrázek, hodnota 1,0 zachová původní jas."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "kontrast"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr "Hodnota 0,0 udělá šedý obrázek, hodnota 1,0 zachová původní kontrast."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "ostrost"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Hodnota 0,0 udělá rozmazaný obrázek, hodnota 1,0 zachová původní ostrost."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "filtry"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "velikost"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "Výška odrazu jako podíl výšky původního obrázku. Hodnota 0.0 nepřidá žádný "
 "odraz, hodnota 1.0 přidá odraz stejně vysoký, jako původní obrázek."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "intenzita"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr "Počáteční intenzita postupně slábnoucího odrazu."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr "Barva pozadí odrazu. Nastavte na barvu pozadí stránky."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "efekt"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "efekty"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "styl"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "krytí"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "Neprůhlednost překrývajícího obrázku."
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "vodotisk"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "vodotisky"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "Název velikosti by měl obsahovat pouze písmena, číslice a podtržítka. "
 "Například: „nahled“, „male_zobrazeni“, „velke_zobrazeni“."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "šířka"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Pokud je šířka nastavena na 0, velikost obrázku bude upravena podle zadané "
 "výšky."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "výška"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Pokud je výška nastavena na 0, velikost obrázku bude upravena podle zadané "
 "šířky."
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "kvalita"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "Kvalita JPEG."
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "zvětšit obrázky?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "Pokud je vybráno, obrázek bude podle potřeby zvětšen, aby odpovídal "
 "požadovaným rozměrům. Pokud má být obrázek oříznutý, bude podle potřeby "
 "zvětšen bez ohledu na toto nastavení."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "oříznout?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "Pokud je vybráno, obrázek bude oříznutý, aby odpovídal požadovaným proporcím."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "vytvářet předem?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 "Pokud je vybráno, bude pro každý obrázek vytvořena varianta v této velikosti "
 "předem, místo až v době zobrazení."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "navyšovat počet zobrazení?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Pokud je vybráno, bude hodnota „view_count“ obrázku navyšována s každým "
 "zobrazením obrázku této velikosti."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "obrázek s vodotiskem"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "velikost obrázku"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "velikosti obrázků"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr "Ořezávat fotografie je možné, pouze pokud je zadána výška i šířka."
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/cs/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/cs/LC_MESSAGES/django.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
 "PO-Revision-Date: 2017-09-23 19:18+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Czech (http://www.transifex.com/richardbarran/django-"
 "photologue/language/cs/)\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: cs\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "Unikátní název, který bude použit v URL adrese (bez diakritiky)."
 
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
```

### Comparing `django-photologue-3.8.1/photologue/locale/hu/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/hu/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # Translators:
 # David Smith, 2015
 # David Smith, 2015-2016
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
-"Last-Translator: David Smith\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
+"Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Hungarian (http://www.transifex.com/richardbarran/django-"
 "photologue/language/hu/)\n"
 "Language: hu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -118,504 +118,504 @@
 msgid "Remove selected photos from the current site"
 msgstr "Kiválasztott fotók eltávolítása jelen webhelyről"
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr "Fotókat tartalmazó zip fájl feltöltése"
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr "Cím"
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 "Az összes feltöltött fotó címe ebből a címből + egy sorszámból fog állni."
 "<br>Új album létrehozása esetén ezt a mezőt kötelező kitölteni, meglévő "
 "album esetén elhagyható - utóbbi esetben a fotók címe a meglévő album "
 "nevéből fog képződni."
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr "Album"
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Válasszon ki egy albumot, amelyhez a fotók hozzáadásra kerüljenek! Hagyja "
 "üresen, ha új albumot akar létrehozni a megadott címmel!"
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr "Képaláírás"
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "A képaláírás minden új fotóra érvényes lesz."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr "Leírás"
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr "Album leírása. Csak új albumok esetén kötelező."
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr "Nyilvános"
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 "Vegye ki a pipát, ha a feltöltött albumot és a benne lévő fotókat priváttá "
 "akarja tenni."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr "Ezzel a címmel már létezik album."
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr ""
 "Válasszon egy meglévő albumot, vagy írjon be egy címet új album "
 "létrehozásához."
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 "„{filename}” fájl mellőzve lett, mivel valamely mappában van. A fotóknak "
 "közvetlenül kell a zip fájlban lenniük."
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr "zip fájlban lévő „{0}” fájl feldolgozása sikertelen."
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "Fotók hozzáadva a(z) „{0}” albumhoz."
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Nagyon alacsony"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Alacsony"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Közepesen alacsony"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Közepes"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Közepesen magas"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Magas"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Nagyon magas"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Teteje"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Jobb oldala"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Alja"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Bal oldala"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Közepe (Alapértelmezett)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Függőleges tengely mentén tükrözés"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Vízszintes tengely mentén tükrözés"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Óramutató járásával ellenkező irányba 90 fok forgatása"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Óramutató járásával megegyező irányba 90 fok forgatás"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "180 fokos forgtás"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Cím"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Méretezés"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 "Több szűrőt is alkalmazhat egymás után a következő mintára: „SZŰRŐ_EGY-"
 ">SZŰRŐ_KETTŐ->SZŰRŐ_HÁROM”. A szűrők a megadott sorrendben, egymás után "
 "lesznek a képre alkalmazva. A következő szűrők állnak  rendelkezésére: %s"
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "publikálás dátuma"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "cím"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "cím slug"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "A \"slug\" egy objektum egyedi, URL-be ágyazható leírása."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "leírás"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "nyilvános"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Nyilvános albumok láthatóak lesznek az alapértelmezett nézetekben."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "fotók"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr "webhelyek"
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "album"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "albumok"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "számláló"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "kép"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "készítés dátuma"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr "Fotó készítésének dátuma (kép EXIF adataiból kinyerve)."
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr "nézettségi számláló"
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "kivágás"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "szűrő"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "Nincs definiálva \"admin_thumbnail\" fotóméret."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Kicsinyített kép"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "slug"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "képaláírás"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "hozzáadva"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr "Nyilvános fotók láthatóak lesznek az alapértelmezett nézetekben."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "fotó"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "név"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "forgatás vagy türközés"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "szín"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 "A 0.0-ás érték fekete-fehér képet, az 1.0-ás pedig az eredeti, színes képet "
 "eredményezi"
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "fényerő"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "A 0.0-ás érték egy fekete képet, az 1.0-ás pedig az eredeti képet "
 "eredményezi."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "kontraszt"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "A 0.0-ás érték egy egyszínű, szürke képet, az 1.0-ás érték pedig az eredeti "
 "képet eredményezi."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "élesség"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "A 0.0-ás érték egy elmosott képet, az 1.0-ás érték pedig az eredeti képet "
 "eredményezi."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "szűrők"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "méret"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "A tükröződés magasságát az eredeti kép magasságának százalékában kell "
 "megadni. A 0.0-ás érték egy tükröződés nélküli képet, az 1.0-ás érték pedig "
 "egy, Az eredeti kép magasságával megegyező magasságú tükröződést tartalmazó "
 "képet eremdényez."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "erősség"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr "A tükröződés elhalványodásának kezdő átlátszósága."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 "A tükröződés színátmenetének háttérszíne. Állítsa be olyan színűre, amilyen "
 "színű háttérre kerül a kép!"
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "fotó effekt"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "fotó effektek"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "stílus"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "átlátszóság"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "A felső réteg átlátszósága."
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "vízjel"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "vízjelek"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "A fotóméretek neve csak kis betűket, számokat és aláhúzásjeleket "
 "tartalmazhat. Pl.: \"thumbnail\", \"display\", \"small\", \"main_page_widget"
 "\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "szélesség"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Ha a szélességet 0-ra állítja, a kép a megadott magasság alapján arányosan "
 "fog méreteződni."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "magasság"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Ha a magasságot 0-ra állítja, a kép a megadott magasság alapján arányosan "
 "fog méreteződni."
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "minőség"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "JPEG minőség"
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "képek felméretezése?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "Ha be van állítva, akkor a megadott méretnél kisebb képek fel lesznek "
 "nagyítva, hogy kitöltsék a rendelkezésre álló helyet. Képkivágás esetén "
 "ettől az opciótól függetlenül mindenképpen fel lesznek nagyítva a képek "
 "szükség esetén."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "képkivágás?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "Ha be van állítva, akkor a képek úgy lesznek átméretezve a megadott "
 "képarárnyra, hogy egy részük le lesz vágva."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "előre generálás?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 "Ha be van állítva, akkor a hozzáadáskor előre le lesz generálva a fotó erre "
 "a méretre."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "nézettségi számláló növelése?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Ha be van állítva, akkor a kép „nézettségi számláló” mezőjében lévő érték "
 "minden megjelenítés után egyel növekedni fog."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "vízjelhez felhasznált kép"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "fotóméret"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "fotóméretek"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr "Képkivágás csak szélesség és magasság megadása után lehetséges."
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr "Zip fájl feltöltése"
```

### Comparing `django-photologue-3.8.1/photologue/locale/hu/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/hu/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
-"Last-Translator: David Smith\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
+"Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Hungarian (http://www.transifex.com/richardbarran/django-"
 "photologue/language/hu/)\n"
+"Language: hu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "\n"
 "\t\t\t\t    page %(page_number)s of %(total_pages)s\n"
 "\t\t\t\t"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/en_US/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/en_US/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
 "PO-Revision-Date: 2013-11-20 11:06+0000\n"
 "Last-Translator: richardbarran <richard@arbee-design.co.uk>\n"
 "Language-Team: English (United States) (http://www.transifex.com/projects/p/"
 "django-photologue/language/en_US/)\n"
 "Language: en_US\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -103,501 +103,501 @@
 msgid "Remove selected photos from the current site"
 msgstr ""
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr ""
 
-#: forms.py:34
+#: forms.py:31
 #, fuzzy
 #| msgid "title"
 msgid "Title"
 msgstr "title"
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 #, fuzzy
 #| msgid "gallery"
 msgid "Gallery"
 msgstr "gallery"
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 
-#: forms.py:47
+#: forms.py:44
 #, fuzzy
 #| msgid "caption"
 msgid "Caption"
 msgstr "caption"
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "Caption will be added to all photos."
 
-#: forms.py:50
+#: forms.py:47
 #, fuzzy
 #| msgid "description"
 msgid "Description"
 msgstr "description"
 
-#: forms.py:52
+#: forms.py:49
 #, fuzzy
 #| msgid "A description of this Gallery."
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr "A description of this Gallery."
 
-#: forms.py:53
+#: forms.py:50
 #, fuzzy
 #| msgid "is public"
 msgid "Is public"
 msgstr "is public"
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr ""
 
-#: forms.py:89
+#: forms.py:86
 #, fuzzy
 #| msgid "Select a .zip file of images to upload into a new Gallery."
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr "Select a .zip file of images to upload into a new Gallery."
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr ""
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr ""
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Very Low"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Low"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Medium-Low"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Medium"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Medium-High"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "High"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Very High"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Top"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Right"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Bottom"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Left"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Center (Default)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Flip left to right"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Flip top to bottom"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Rotate 90 degrees counter-clockwise"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Rotate 90 degrees clockwise"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Rotate 180 degrees"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Tile"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Scale"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "date published"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "title"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "title slug"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "A \"slug\" is a unique URL-friendly title for an object."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "description"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "is public"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Public galleries will be displayed in the default views."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "photos"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr ""
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "gallery"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "galleries"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "count"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "image"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "date taken"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr "view count"
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "crop from"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "effect"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "An \"admin_thumbnail\" photo size has not been defined."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Thumbnail"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "slug"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "caption"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "date added"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr "Public photographs will be displayed in the default views."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "photo"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "name"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "rotate or flip"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "color"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "brightness"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "contrast"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "sharpness"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "filters"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "size"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "strength"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr "The initial opacity of the reflection gradient."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "photo effect"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "photo effects"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "style"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "opacity"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "The opacity of the overlay."
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "watermark"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "watermarks"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "width"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "height"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "quality"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "JPEG image quality."
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "upscale images?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "crop to fit?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "pre-cache?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr "If selected this photo size will be pre-cached as photos are added."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "increment view count?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "watermark image"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "photo size"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "photo sizes"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr "Can only crop photos if both width and height dimensions are set."
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/en_US/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/en_US/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
 "PO-Revision-Date: 2013-11-20 11:06+0000\n"
 "Last-Translator: richardbarran <richard@arbee-design.co.uk>\n"
 "Language-Team: English (United States) (http://www.transifex.com/projects/p/"
 "django-photologue/language/en_US/)\n"
 "Language: en_US\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
```

### Comparing `django-photologue-3.8.1/photologue/locale/es_ES/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/es_ES/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 # dmalisani <dmalisani@gmail.com>, 2014
 # Rafa Muñoz Cárdenas <bymenda@gmail.com>, 2009
 # salvador ortiz <chava.door@gmail.com>, 2017
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
-"Last-Translator: salvador ortiz <chava.door@gmail.com>\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
+"PO-Revision-Date: 2017-12-03 14:46+0000\n"
+"Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Spanish (Spain) (http://www.transifex.com/richardbarran/"
 "django-photologue/language/es_ES/)\n"
 "Language: es_ES\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -117,497 +117,497 @@
 msgid "Remove selected photos from the current site"
 msgstr "Eliminar la foto seleccionada del sitio actual"
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr "Subir un archivo ZIP de fotos"
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr "Titulo"
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr "Galería"
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Seleccione una galería para agregarle estas imágenes. Déjelo vacío para "
 "crear una nueva galería a partir de este título."
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr "Pie de foto"
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "El pie de foto se añadirá a todas las fotos."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr "Descripción"
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 "Una descripción para esta galería. Solo es requerido para nuevas galerías."
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr "Es público"
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 "Desactive esto para hacer que la galería subida y fotos incluidas sean "
 "privadas."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr "Ya existe una galería con ese título."
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr ""
 "Seleccione una galería existente o ingrese un nuevo nombre para la galería."
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 "Ignorando archivos \"{filename}\" por estar en subcarpetas, todas las "
 "imágenes deben estar en la carpeta de primer nivel del zip."
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr "No se pudo procesar el archivo \"{0}\" en el archivo zip."
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "La foto a sido agregada correctamente a \"{0}\"."
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Muy bajo"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Bajo"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Medio-bajo"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Medio"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Medio-alto"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Alto"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Muy alto"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Arriba"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Derecha"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Abajo"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Izquierda"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Centro (por defecto)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Voltear de izquerda a derecha"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Voltear de arriba a abajo"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Rotar 90 grados en sentido horario"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Rotar 90 grados en sentido antihorario"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Rotar 180 grados"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Mosaico"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Escalar"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 "Encadene múltiples filtros usando el siguiente patrón \"FILTRO_UNO-"
 ">FILTRO_DOS->FILTRO_TRES\". Los filtros de imagen se aplicarán en orden. Los "
 "siguientes filtros están disponibles: %s."
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "fecha de publicación"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "título"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "título slug"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "Un \"slug\" es un único título URL-amigable para un objeto."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "descripción"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "es público"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Las galerías públicas serán mostradas en las vistas por defecto."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "fotos"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr "sitios"
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "galería"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "galerías"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "contar"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "imagen"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "fecha en la que se tomó"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr "La fecha de la imagen fue obtenida por información EXIF de la imagen."
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr "Contador de visitas"
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "Recortar desde"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "efecto"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "El tamaño de foto de \"miniatura de admin\" no ha sido definido."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Miniatura"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "slug"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "pie de foto"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "fecha añadida"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr "Las fotos públicas serán mostradas en las vistas por defecto."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "foto"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "nombre"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "rotar o voltear"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "color"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 "Un factor de 0.0 proporciona una imagen blanca y negra. Un factor de 1.0 "
 "proporciona la imagen original."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "iluminación"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Un factor de 0.0 proporciona una imagen negra. Un factor de 1.0 proporciona "
 "la imagen original."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "contraste"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Un factor de 0.0 proporciona una imagen sólida gris. Un factor de 1.0 "
 "proporciona la imagen original."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "Resaltado"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Un factor de 0.0 proporciona una imagen desenfocada, un factor de 1.0 "
 "proporciona la imagen original."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "filtros"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "tamaño"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "La altura de la reflexión como porcentaje de la imagen original. Un factor "
 "de 0.0 no da ninguna reflexión, un factor de 1.0 añade una reflexión igual a "
 "la altura de la imagen original."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "fortaleza"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr "La opacidad inicial del gradiente de reflexión."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 "El color de fondo del gradiente de reflexión. Establezca esto para hacer "
 "coincidir el color de fondo con el color de tu página."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "efecto de foto"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "efectos de foto"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "estilo"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "opacidad"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "La opacidad de la superposición"
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "marca de agua"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "marcas de agua"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "El nombre del tamaño solo puede contener letras, números y subrayados. Por "
 "ejemplo:\"miniaturas\", \"muestra\", \"muestra_principal\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "anchura"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Si la anchura se establece a \"0\" la imagen será escalada hasta la altura "
 "proporcionada"
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "altura"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Si la altura se establece a \"0\" la imagen será escalada hasta la anchura "
 "proporcionada"
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "calidad"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "Calidad de imagen JPEG."
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "¿Aumentar imágenes?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "Si se selecciona la imagen será aumentada si es necesario para ajustarse a "
 "las dimensiones proporcionadas. Los tamaños recortados serán aumentados de "
 "acuerdo a esta opción."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "¿Recortar hasta ajustar?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "Si se selecciona la imagen será escalada y recortada para ajustarse a las "
 "dimensiones proporcionadas."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "¿pre-cachear?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 "Si se selecciona, este tamaño de foto será pre-cacheado cuando se añadan "
 "nuevas fotos."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "¿incrementar contador de visualizaciones?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Si se selecciona el \"contador de visualizaciones\" se incrementará cuando "
 "esta foto sea visualizada."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "marca de agua"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "tamaño de foto"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "tamaños de foto"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr "Solo puede recortar las fotos si ancho y alto están establecidos."
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr "Subir archivo ZIP"
```

### Comparing `django-photologue-3.8.1/photologue/locale/es_ES/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/es_ES/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
-"Last-Translator: salvador ortiz <chava.door@gmail.com>\n"
+"PO-Revision-Date: 2017-12-03 14:46+0000\n"
+"Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Spanish (Spain) (http://www.transifex.com/richardbarran/"
 "django-photologue/language/es_ES/)\n"
+"Language: es_ES\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: es_ES\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "\n"
 "\t\t\t\t    page %(page_number)s of %(total_pages)s\n"
 "\t\t\t\t"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/pt/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/pt/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Translators:
 # Translators:
 # David Kwast <david.kwast@gmail.com>, 2009
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
 "PO-Revision-Date: 2017-09-19 14:01+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Portuguese (http://www.transifex.com/richardbarran/django-"
 "photologue/language/pt/)\n"
 "Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -105,489 +105,489 @@
 msgid "Remove selected photos from the current site"
 msgstr ""
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr ""
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr ""
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr ""
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "A legenda será adicionada para todas as fotos"
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr ""
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr ""
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 "Desmarque esta opção para tornar a galeria, incluindo suas fotos, não "
 "pública."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr ""
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr ""
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr ""
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr ""
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Muito Baixa"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Baixa"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Média-Baixa"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Média"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Média-Alta"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Alta"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Muito Alta"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Cima"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Direita"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Baixo"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Esquerda"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Centro (Padrão)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Inverter da direita para a esquerda"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Inverter de cima para baixo"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Rotacionar 90 graus no sentido anti-horário"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Rotacionar 90 graus no sentido horário"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Rotacionar 180 graus"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Título"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Escala"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 "Encadeie multiplos filtros usando o seguinte padrão \"FILTRO_UM->FILTRO_DOIS-"
 ">FILTRO_TRÊS\". Os filtors serão aplicados na ordem em que foram encadeados. "
 "Os seguintes filtros estão disponíveis: %s."
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "data de publicação"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "título"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "slug do título"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "Um \"slug\" é um título único compatível com uma URL."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "descrição"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "é publico"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Galerias públicas serão mostradas nas views padrões."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "fotos"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr ""
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "Galeria"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "Galerias"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "contagem"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "imagem"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "data em que a foto foi tirada"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr ""
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "cortar"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "efeito"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "Um tamanho para a foto do \"admin_thumbnail\" ainda não foi definido."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Thumbnail"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "slug"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "legenda"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "data que foi adicionado(a)"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr "Fotos públicas serão mostradas nas views padrões."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "foto"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "nome"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "rotacionar ou inverter"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "cor"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 "O valor 0.0 deixará a imagem em preto e branco, o fator 1.0 não alterará a "
 "mesma.A factor of 0.0 gives a black and white image, a factor of 1.0 gives "
 "the original image."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "brilho"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "O valor 0.0 deixará a imagem totalmente preta, o valor 1.0 não alterará a "
 "mesma."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "contraste"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "O valor 0.0 deixará a imagem totalmente cinza, o valor 1.0 não alterará a "
 "mesma."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "nitidez"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "O valor 0.0 deixará a imagem embaçada, o valor 1.0 não alterará a mesma."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "filtros"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "tamanho"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "Valor entre 0 e 1. O reflexo será proporcional a altura da imagem. O valor "
 "0.0 não produzirá um reflexo e o valor 1.0 produzirá um reflexo com a mesma "
 "altura da imagem original."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "força"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr "O valor inicial da opacidade do gradiente de reflexão."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 "A cor de fundo do gradiente de reflexão. Ajuste de acordo com a cor de fundo "
 "de sua página."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "efeito de foto"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "efeitos de foto"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "estilo"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "opacidade"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "A opacidade da sobre-imagem (overlay)"
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "marca d'água"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "marcas d'água"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "O nome do tamanho da foto somente poderá conter letras, números e "
 "underscores. Exemplos: \"thumbnail\", \"tela\", \"pequeno\", \"grande\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "largura"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Se o valor da largura for \"0\", a imagem será redimensionada de acordo com "
 "a altura informada"
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "altura"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Se o valor da altura for \"0\", a imagem será redimensionada de acordo com a "
 "largura informada"
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "qualidade"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "qualidade da imagem JPEG"
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "Aumentar a dimensão das imagens?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "Se selecionado, a imagem terá sua dimensão aumentada. Imagens cortadas serão "
 "redimensionadas independentemente desta configuração."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "cortar para conformar?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "Se selecionado, a imagem será redimensionada e cortada para se conformar de "
 "acordo com as dimensões fornecidas."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "pré-cachear?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 "Se selecionado, o tamanho da foto será pré-cacheado logo após sua inclusão."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "Incrementar o contador de visualizações?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Se selecionado, o \"view_count\" desta imagem será incrementado quando o "
 "tamanho da mesma for mostrado."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "imagem para marca d'água"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "tamanho da foto"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "tamanhos das fotos"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr ""
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/pt/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
 "PO-Revision-Date: 2017-09-19 14:01+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
-"Language-Team: Portuguese (http://www.transifex.com/richardbarran/django-"
-"photologue/language/pt/)\n"
+"Language-Team: Portuguese (Brazil) (http://www.transifex.com/richardbarran/"
+"django-photologue/language/pt_BR/)\n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pt\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "Um \"slug\" é um título único compatível com uma URL."
 
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
```

### Comparing `django-photologue-3.8.1/photologue/locale/da_DK/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/en/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 #
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
 "PO-Revision-Date: 2015-12-23 14:50+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
-"Language-Team: Danish (Denmark) (http://www.transifex.com/richardbarran/"
-"django-photologue/language/da_DK/)\n"
-"Language: da_DK\n"
+"Language-Team: English (http://www.transifex.com/richardbarran/django-"
+"photologue/language/en/)\n"
+"Language: en\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin.py:62
 #, python-format
@@ -104,458 +104,458 @@
 msgid "Remove selected photos from the current site"
 msgstr ""
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr ""
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr ""
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr ""
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr ""
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr ""
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr ""
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr ""
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr ""
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr ""
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr ""
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr ""
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr ""
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr ""
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr ""
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr ""
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr ""
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr ""
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr ""
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr ""
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr ""
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr ""
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr ""
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr ""
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr ""
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr ""
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr ""
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr ""
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr ""
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr ""
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr ""
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr ""
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr ""
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr ""
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr ""
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr ""
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr ""
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr ""
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr ""
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr ""
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr ""
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr ""
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr ""
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr ""
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr ""
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr ""
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr ""
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr ""
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr ""
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr ""
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr ""
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr ""
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr ""
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr ""
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr ""
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr ""
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr ""
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr ""
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr ""
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr ""
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr ""
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr ""
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr ""
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr ""
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr ""
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr ""
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr ""
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr ""
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr ""
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr ""
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr ""
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr ""
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr ""
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr ""
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr ""
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr ""
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr ""
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr ""
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr ""
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr ""
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr ""
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr ""
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr ""
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/fr/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/fr/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # Translators:
 # Matthieu Payet <matthieu.payet4@gmail.com>, 2017
 # Théophane Hufschmitt <huf31@gmx.fr>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
-"Last-Translator: Matthieu Payet <matthieu.payet4@gmail.com>\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
+"Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: French (http://www.transifex.com/richardbarran/django-"
 "photologue/language/fr/)\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -119,508 +119,508 @@
 msgid "Remove selected photos from the current site"
 msgstr "Supprimer les photos séléctionnées du site courant"
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr "Télécharger une archive de photos au format *.zip"
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr "Titre"
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 "Ce titre + <un nombre> sera donné à toutes les photos téléchargées.<br/> Ce "
 "champ est requis lors de la création d'une nouvelle galerie mais est "
 "facultative lors d'un ajout à une galerie existante. S'il n'est pas fourni, "
 "les titres des photos seront créés à partir du nom de la galerie existante."
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr "Galerie"
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Sélectionner une galerie à laquelle ajouter ces images. Laisser ce champ "
 "vide pour créer une nouvelle galerie à partir du titre indiqué."
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr "Légende"
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "La légende sera ajoutée a toutes les photos."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr "Description"
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 "Une description de cette galerie. Requise seulement pour les nouvelles "
 "galeries."
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr "Est publique"
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 "Décochez cette case pour rendre la galerie des photos envoyées sur le "
 "serveur et son contenu privés."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr "Une galerie portant ce nom existe déjà."
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr ""
 "Sélectionner une galerie existante ou entrer un titre pour une nouvelle "
 "galerie."
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 "Fichier \"{filename}\" ignoré car il apparaît dans un sous-dossier. Toutes "
 "les images doivent être à la racine du fichier zip."
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr "Impossible de traîter le fichier \"{0}\" dans l'archive zip."
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "Les photos ont été ajoutés à la galerie \"{0}\"."
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Très Bas"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Bas"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Moyen-Bas"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Moyen"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Moyen-Haut"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Haut"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Très Haut"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Sommet"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Droite"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Bas"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Gauche"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Centré (par défaut)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Inversion de gauche à droite"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Inversion de haut en bas"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Rotation de 90 degrés dans le sens anti-horloger"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Rotation de 90 degrés dans le sens horloger"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Rotation de 180 degrés"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Mosaïque"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Redimensionner"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 "Faite suivre de multiple filtres en utilisant la forme suivante \"FILTRE_UN-"
 ">FILTRE_DEUX->FILTRE_TROIS\". Les filtres d'image seront appliqués dans "
 "l'ordre. Les filtres suivants sont disponibles: %s."
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "date de publication"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "titre"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "version abrégée du titre"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr ""
 "Un \"slug\" est un titre abrégé et unique, compatible avec les URL, pour un "
 "objet."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "description"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "est public"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Les galeries publiques seront affichée dans les vues par défaut."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "photos"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr "sites"
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "galerie"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "galleries"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "nombre"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "image"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "date de prise de vue"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 "La date à laquelle l'image a été prise ; obtenue à partir des données EXIF "
 "de l'image."
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr "nombre"
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "découper à partir de"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "effet"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "Une taille de photo \"admin_thumbnail\" n'a pas encore été définie."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Miniature"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "libellé court"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "légende"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "date d'ajout"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr "Les photographies publique seront affichées dans les vues par défaut."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "photo"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "nom"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "rotation ou inversion"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "couleur"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 "Un facteur de 0.0 donne une image en noir et blanc, un facteur de 1.0 donne "
 "l'image originale."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "brillance"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Un facteur de 0.0 donne une image noire, un facteur de 1.0 donne l'image "
 "originale."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "contraste"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Un facteur de 0.0 donne une image grise, un facteur de 1.0 donne l'image "
 "originale."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "netteté"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Une facteur de 0.0 donne une image floue, un facteur de 1.0 donne l'image "
 "d'origine."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "filtres"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "taille"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "La hauteur de la réflection sous la forme d'un pourcentage de l'image "
 "d'origine. Un facteur de 0.0 n'ajoute aucune réflection, un facteur de 1.0 "
 "ajoute une réflection égale à la hauteur de l'image d'origine."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "force"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr "L'opacité initial du gradient de reflet."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 "La couleur de fond du gradient de reflet. Faites correspondre ce paramètre "
 "avec la couleur de fond de votre page."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "effet photo"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "effets photo"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "style"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "opacité"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "L'opacité de la surcouche."
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "filigrane"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "filigranes"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "Le nom de la taille de la photo ne doit contenir que des lettres, des "
 "chiffres et des caractères de soulignement. Exemples: \"miniature\", "
 "\"affichage\", \"petit\", \"widget_page_principale\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "largeur"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Si la largeur est réglée à \"0\" l l'image sera redimensionnée par rapport à "
 "la hauteur fournie."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "hauteur"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Si la hauteur est réglée à \"0\" l l'image sera redimensionnée par rapport à "
 "la largeur fournie."
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "qualité"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "Qualité JPEG de l'image."
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "agrandir les images ?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "Si sélectionné l'image sera agrandie si nécessaire pour coïncider avec les "
 "dimensions fournies. Les dimensions ajustées seront agrandies sans prendre "
 "en compte ce paramètre."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "découper pour adapter à la taille ?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "Si sélectionné l'image sera redimensionnée et recadrée pour coïncider avec "
 "les dimensions fournies."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "mise en cache ?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 "Si sélectionné cette taille de photo sera mise en cache au moment au les "
 "photos sont ajoutées."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "incrémenter le nombre d'affichages ?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Si sélectionné le \"view_count\" (nombre d'affichage) de l'image sera "
 "incrémenté quand cette taille de photo sera affichée."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "placer un filigrane sur l'image"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "taille de la photo"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "tailles des photos"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr ""
 "La hauteur et la largeur doivent être toutes les deux définies pour "
 "retailler des photos."
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
```

### Comparing `django-photologue-3.8.1/photologue/locale/fr/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/fr/LC_MESSAGES/django.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
-"Last-Translator: Matthieu Payet <matthieu.payet4@gmail.com>\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
+"Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: French (http://www.transifex.com/richardbarran/django-"
 "photologue/language/fr/)\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: fr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid ""
 "\n"
 "\t\t\t\t    page %(page_number)s of %(total_pages)s\n"
 "\t\t\t\t"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/no/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/no/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
 "PO-Revision-Date: 2017-09-19 14:01+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Norwegian (http://www.transifex.com/richardbarran/django-"
 "photologue/language/no/)\n"
 "Language: no\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -104,476 +104,476 @@
 msgid "Remove selected photos from the current site"
 msgstr ""
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr ""
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr ""
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr ""
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "Undertitler blir lagt til på alle bilder."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr ""
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr ""
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr "Avmarker dette for å gjøre galleriet og dets bilder private."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr ""
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr ""
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr ""
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr ""
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Veldig lav"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Lav"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Middels-lav"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Middels"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Middels-høy"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Høy"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Veldig høy"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Topp"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Høyre"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Bunn"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Venstre"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Senter (forhåndsvalgt)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Snu venstre mot høyre"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Snu topp mot bunn"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Rotér 90 grader mot klokka"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Rotér 90 grader med klokka"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Rotér 180 grader"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Flislegg"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Skalér"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "publiseringsdato"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "tittel"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "tittel (slug)"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "En \"slug\" er en unik URL-vennlig tittel for et objekt."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "beskrivelse"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "publisert"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Publiserte gallerier vil bli vist på vanlig vis."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "bilder"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr ""
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "galleri"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "gallerier"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "visninger"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "bilde"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "dato tatt"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr ""
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "kutt fra"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "effekt"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "En \"admin_thumbnail\"-bildestørrelse har ikke blitt opprettet."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Miniatyrbilde"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "slug"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "undertittel"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "opplastingsdato"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr "Publiserte bilder vil bli vist på vanlig måte."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "bilde"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "navn"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "rotér og snu"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "farge"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 "En verdi på 0.0 gir et sort/hvitt-bilde, en verdi på 1.0 gir originalbildet."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "lyshet"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr "En verdi på 0.0 gir et sort bilde, en verdi på 1.0 gir originalbildet."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "kontrast"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "En verdi på 0.0 gir et grått bilde, en verdi på 1.0 gir originalbildet."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "skarphet"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "En verdi på 0.0 gir et utydlig bilde, en verdi på 1.0 gir originalbildet."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "filter"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "størrelse"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "Høyden av refleksjonen som prosent av originalbildet. En verdi på 0.0 gir "
 "ingen refleksjon, en verdi på 1.0 gir en refleksjon tilsvarende høyden på "
 "originalbildet."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "styrke"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr ""
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "bildeeffekt"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "bildeeffekter"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "stil"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "gjennomsiktighet"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "Gjennomsiktigheten av overlegget."
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "vannmerke"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "vannmerker"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "Navn på bildestørrelse kan kun inneholde bokstaver, tall og understreker. "
 "Eksempler: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "bredde"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Hvis bredden er satt til \"0\" blir bildet skalert til den oppgitte høyden."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "høyde"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Hvis høyden er satt til \"0\" blir bildet skalert til den oppgitte bredden."
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "kvalitet"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "JPEG bildekvalitet"
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "oppskalér bilder?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "Hvis valgt, blir bildet vil bli skalert opp om det er nødvendig. Kuttede "
 "størrelser vil bli oppskalert uansett innstilling."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "kutt for tilpasning?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "Hvis valgt blir bildet skalert og kuttet for å passe med den oppgitte "
 "størrelsen."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "mellomlagre på forhånd?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 "Hvis valgt blir denne bildestørrelsen mellomlagret på forhånd når nye bilder "
 "blir lagt til."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "øke visningstelleren?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Hvis valgt vil \"visningstelleren\" øke hver gang denne bildestørrelsen "
 "vises."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "vannmerke på bilde"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "bildestørrelse"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "bildestørrelser"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr ""
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/no/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/no/LC_MESSAGES/django.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
 "PO-Revision-Date: 2017-09-19 14:01+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Norwegian (http://www.transifex.com/richardbarran/django-"
 "photologue/language/no/)\n"
+"Language: no\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: no\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "En \"slug\" er en unik URL-vennlig tittel for et objekt."
 
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
```

### Comparing `django-photologue-3.8.1/photologue/locale/en/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/it/LC_MESSAGES/django.po`

 * *Files 21% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 #
 # Translators:
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
-"PO-Revision-Date: 2015-12-23 14:50+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
+"PO-Revision-Date: 2017-09-19 14:01+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
-"Language-Team: English (http://www.transifex.com/richardbarran/django-"
-"photologue/language/en/)\n"
-"Language: en\n"
+"Language-Team: Italian (http://www.transifex.com/richardbarran/django-"
+"photologue/language/it/)\n"
+"Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin.py:62
 #, python-format
@@ -104,458 +104,492 @@
 msgid "Remove selected photos from the current site"
 msgstr ""
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr ""
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr ""
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr ""
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
-msgstr ""
+msgstr "La didascalia verrà aggiunta a tutte le foto"
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr ""
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr ""
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
+"Deseleziona l'opzione per rendere private le immagini e la galleria una "
+"volta caricata."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr ""
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr ""
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr ""
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr ""
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
-msgstr ""
+msgstr "Molto Bassa"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
-msgstr ""
+msgstr "Bassa"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
-msgstr ""
+msgstr "Medio-Bassa"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
-msgstr ""
+msgstr "Media"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
-msgstr ""
+msgstr "Medio-Alta"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
-msgstr ""
+msgstr "Alta"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
-msgstr ""
+msgstr "Molto Alta"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
-msgstr ""
+msgstr "In alto"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
-msgstr ""
+msgstr "A destra"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
-msgstr ""
+msgstr "In basso"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
-msgstr ""
+msgstr "A sinistra"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
-msgstr ""
+msgstr "Al centro (Default)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
-msgstr ""
+msgstr "Inverti destra con sinistra"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
-msgstr ""
+msgstr "Inverti alto con basso"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
-msgstr ""
+msgstr "Ruota di 90 gradi in senso anti-orario"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
-msgstr ""
+msgstr "Ruota di 90 gradi in senso orario"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
-msgstr ""
+msgstr "Ruota di 180 gradi"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
-msgstr ""
+msgstr "Affianca"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
-msgstr ""
+msgstr "Ridimensiona"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
+"Collega filtri multipli in cascata con il seguente schema \"FILTRO_UNO-"
+">FILTRO_DUE->FILTER_TRE\". I filtri saranno applicati in ordine alle "
+"immagini. I seguenti filtri sono disponibili: %s."
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
-msgstr ""
+msgstr "data di pubblicazione"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
-msgstr ""
+msgstr "titolo"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
-msgstr ""
+msgstr "slug"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
-msgstr ""
+msgstr "Uno \"Slug\" è un titolo univoco per un oggetto, usabile come URL."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
-msgstr ""
+msgstr "descrizione"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
-msgstr ""
+msgstr "è pubblica"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
-msgstr ""
+msgstr "Le gallerie pubbliche verranno visualizzate nelle viste di default."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
-msgstr ""
+msgstr "foto"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr ""
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
-msgstr ""
+msgstr "galleria"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
-msgstr ""
+msgstr "gallerie"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
-msgstr ""
+msgstr "numero"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
-msgstr ""
+msgstr "immagine"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
-msgstr ""
+msgstr "data dello scatto"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr ""
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
-msgstr ""
+msgstr "ritagliata da"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
-msgstr ""
+msgstr "effetto"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
-msgstr ""
+msgstr "La dimensione \"admin_thumbnail\" non è ancora stata creata."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
-msgstr ""
+msgstr "Miniatura"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
-msgstr ""
+msgstr "slug"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
-msgstr ""
+msgstr "didascalia"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
-msgstr ""
+msgstr "data di inserimento"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
-msgstr ""
+msgstr "Le fotografie pubbliche verranno visualizzate nelle viste di default."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
-msgstr ""
+msgstr "fotografia"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
-msgstr ""
+msgstr "nome"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
-msgstr ""
+msgstr "ruota o inverti"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
-msgstr ""
+msgstr "colore"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
+"Un fattore di 0.0 restituisce un'immagine in bianco e nero, un fattore di "
+"1.0 restituisce l'immagine originale."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
-msgstr ""
+msgstr "luminosità"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
+"Un fattore di 0.0 restituisce un'immagine nera, un fattore di 1.0 "
+"restituisce l'immagine originale."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
-msgstr ""
+msgstr "contrasto"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
+"Un fattore di 0.0 restituisce un'immagine grigia, un fattore di 1.0 "
+"restituisce l'immagine originale."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
-msgstr ""
+msgstr "nitidezza"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
+"Un fattore di 0.0 restituisce un'immagine sfuocata, un fattore di 1.0 "
+"restituisce l'immagine originale."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
-msgstr ""
+msgstr "filtri"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
-msgstr ""
+msgstr "dimensione"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
+"L'altezza del riflesso come percentuale dell'immagine originale. Un fattore "
+"di 0.0 non aggiunge nessun riflesso, un fattore di 1.0 aggiunge un riflesso "
+"della stessa altezza dell'immagine originale."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
-msgstr ""
+msgstr "intensità"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
-msgstr ""
+msgstr "Opacità iniziale del gradiente del riflesso."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
+"Il colore di sfondo del gradiente di riflesso. Sceglilo in modo che "
+"corrisponda al colore dello sfondo della tua immagine."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
-msgstr ""
+msgstr "effetto fotografico"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
-msgstr ""
+msgstr "effetti fotografici"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
-msgstr ""
+msgstr "stile"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
-msgstr ""
+msgstr "opacità"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
-msgstr ""
+msgstr "Opacità della copertura"
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
-msgstr ""
+msgstr "watermark"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
-msgstr ""
+msgstr "watermark"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
+"Le dimensioni fotografiche devono contenere solo lettere, numeri o caratteri "
+"di sottolineatura. Per esempio: : \"thumbnail\", \"display\", \"small\", "
+"\"main_page_widget\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
-msgstr ""
+msgstr "larghezza"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
+"Se la dimensione è \"0\", l'immagine verrà ridimensionata all'altezza "
+"specificata."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
-msgstr ""
+msgstr "altezza"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
+"Se l'altezza è \"0\", l'immagine verrà ridimensionata alla larghezza "
+"specificata."
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
-msgstr ""
+msgstr "qualità"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
-msgstr ""
+msgstr "qualità dell'immagine JPEG"
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
-msgstr ""
+msgstr "ingrandisco le immagini?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
+"Se selezionato, l'immagine verrà ingrandita (se necessario) per "
+"corrispondere alle dimensioni specificate. Dimensioni ritagliate verranno "
+"ridimensionate senza tenere conto di questa configurazione."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
-msgstr ""
+msgstr "Ritaglio per stare nelle dimensioni?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
+"Se selezionato, l'immagine verrà ridimensionata e ritagliata per rientrare "
+"nelle dimensioni specificate."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
-msgstr ""
+msgstr "pre-cache?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
+"Se selezionato, questa dimensione di foto verrà pre-salvata mentre le foto "
+"sono inserite."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
-msgstr ""
+msgstr "incrementa il contatore di visualizzazioni?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
+"Se selezionato, il \"contatore di visualizzazioni\" dell'immagine sarà "
+"incrementato ad ogni visualizzazione dell'immagine."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
-msgstr ""
+msgstr "immagine di watermark"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
-msgstr ""
+msgstr "dimensione della foto"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
-msgstr ""
+msgstr "dimensioni delle foto"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr ""
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-photologue-3.8.1/photologue/locale/ru/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Translators:
 # Translators:
 # AduchiMergen <aduchimergen@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
 "PO-Revision-Date: 2017-09-19 14:01+0000\n"
 "Last-Translator: AduchiMergen <aduchimergen@gmail.com>\n"
 "Language-Team: Russian (http://www.transifex.com/richardbarran/django-"
 "photologue/language/ru/)\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -121,503 +121,503 @@
 msgid "Remove selected photos from the current site"
 msgstr ""
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr "Загрузка Zip архива с фотографиями"
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr "Название"
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 "Всем загруженным фотографиям будет присвоено название составленное из этого "
 "названия и порядкового номера изображения.<br> Это поле является "
 "обязательным, для создания новой галереи, но не является обязательным при "
 "добавлении к существующей галерее - если не указано, названия фото будут "
 "созданы из имени галереи."
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr "Галерея"
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Выберете галерею для загрузки фотографий. Оставьте поле пустым для создания "
 "новой галереи с соответствующим названием."
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr "Описание"
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "Описание будет добавлено ко всем фотографиям."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr "Описание галереи"
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr "Описание для этой галереи. Необходимо только для новой галереи."
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr "Опубликовать"
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 "Снимите эту галку, чтобы сделать загруженную галерею и включенные в нее "
 "фотографии приватными."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr "Уже существует галерея с таким названием"
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr "Выберете существующую галерею, или введите название новой галереи"
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 "Файл \"{filename}\" пропущен, так как находится в поддиректории; все "
 "изображения должны находиться в корневой директории архива."
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr "Не удалось обработать файл  \"{0}\" в .zip архиве."
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "Фотографии были добавлены в галерею \"{0}\"."
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Очень низкое"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Низкое"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Чуть хуже среднего"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Среднее"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Чуть лучше среднего"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Высокое"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Очень высокое"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Верхняя сторона"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Правая сторона"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Нижняя сторона"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Левая сторона"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Центр (По-умолчанию)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Зеркально отобразить слева направо"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Зеркально отобразить сверху вниз"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Повернуть на 90 градусов против часовой стрелке"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Повернуть на 90 градусов по часовой стрелке"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Повернуть на 180 градусов"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Разместить мозайкой"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Масштабировать"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 "Цепочка фильтров для изображений (\"ФИЛЬТР_1->ФИЛЬТР_2->ФИЛЬТР_3\"). Фильтры "
 "будут применены по порядку. Доступны следующие фильтры: %s."
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "дата публикации"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "название"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "слаг название"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr ""
 "\"слаг\" - это уникальное читаемое название для объекта в адресной строке."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "описание"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "публично"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Публичные галереи будут отображены в представлениях по-умолчанию."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "фотографии"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr ""
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "галерея"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "галереи"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "количество"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "изображение"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "дата наложения"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr "кол-во просмотров"
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "обрезанный из"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "эффект"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "Размер миниатюры \"admin_thumbnail\" не определен."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Миниатюра"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "слаг"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "Описание"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "дата добавления"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr ""
 "Публичные фотографии будут отображены в используемых представлениях по "
 "умолчанию."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "фотография"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "имя"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "повернуть или зеркально отобразить"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "цвет"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 "Значение коэффициента 0.0 дает черно-белое изображение, а значение  "
 "коэффициента 1.0 дает оригинальное изображение."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "яркость"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Значение коэффициента 0.0 дает черное изображение, а значение  коэффициента "
 "1.0 дает оригинальное изображение."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "контраст"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Значение коэффициента 0.0 дает сплошное серое изображение, а значение  "
 "коэффициента 1.0 дает оригинальное изображение."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "резкость"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Значение коэффициента 0.0 дает расплывчатое изображение, а значение  "
 "коэффициента 1.0 дает оригинальное изображение."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "фильтры"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "размер"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "Высота отражения как процент от оригинального изображения. Значение "
 "коэффициента 0.0 не добавляет отображения, а значение коэффициента 1.0 "
 "добавляет отражение равное высоте оригинального изображения."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "сила"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr "Начальная непрозрачность градиента отражения."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 "Цвет фона градиента отражения. Отметьте это для соответствия цвету фона "
 "Вашей страницы."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "фотоэффект"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "фотоэффекты"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "стиль"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "непрозрачность"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "Непрозрачность подложки."
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "водяной знак"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "водяные знаки"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "Название размера фотографии должно содержать только буквы, числа и символы "
 "подчеркивания. Примеры: \"thumbnail\", \"display\", \"small\", "
 "\"main_page_widget\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "ширина"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Если ширина выставлена в \"0\", то изображение будет мастштабировано по "
 "высоте."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "высота"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Если высота выставлена в \"0\", то изображение будет мастштабировано по "
 "ширине"
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "качество"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "качество JPEG изображения."
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "увеличивать изображения?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "Если выбранно, то изображение будет масштабировано в случае необходимости, "
 "чтобы соответствовать габаритам. Обрезанные размеры будут увеличены в "
 "масштабе независимо от этой настройки."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "обрезать?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "Если выбранно, то изображение будет масштабировано и обрезано, чтобы "
 "подходить по габаритам."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "кэшировать?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 "Если выбранно, то размер фотографии будет закэширован при добавлении "
 "фотографий"
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "увеличивать счетчик просмотров?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Если выбрано, то \"view_count\" изображения будет увеличено когда "
 "показывается этот размер фотографии."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "изображение водяного знака"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "размер фотографии"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "размеры фотографий"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr "Можно обрезать фото только если установленны длинна и ширина."
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr "Загрузить zip архив"
```

### Comparing `django-photologue-3.8.1/photologue/locale/ru/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/ru/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
 "PO-Revision-Date: 2017-09-19 14:01+0000\n"
 "Last-Translator: AduchiMergen <aduchimergen@gmail.com>\n"
 "Language-Team: Russian (http://www.transifex.com/richardbarran/django-"
 "photologue/language/ru/)\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 msgid ""
 "\n"
 "\t\t\t\t    page %(page_number)s of %(total_pages)s\n"
```

### Comparing `django-photologue-3.8.1/photologue/locale/tr/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/tr/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 # ali rıza keleş <ali.r.keles@gmail.com>, 2009
 # ali rıza keleş <ali.r.keles@gmail.com>, 2009,2014
 # ali rıza keleş <ali.r.keles@gmail.com>, 2009
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Turkish (http://www.transifex.com/richardbarran/django-"
 "photologue/language/tr/)\n"
 "Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -107,475 +107,475 @@
 msgid "Remove selected photos from the current site"
 msgstr "Seçili fotoları siteden kaldır"
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr ""
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr ""
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Bu resimleri eklemek için bir galeri seçin. Verilen başlıktan yeni bir "
 "galeri oluşturmak için boş bırakın."
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr ""
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "Altyazı tüm fotolara eklenecektir."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr ""
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr ""
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 "Yüklenen bu galeriyi ve içerisindeki tüm fotoları özel yapmak için "
 "işaretlemeyin."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr "Bu başlıkta bir galeri zaten var."
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr ""
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 "\"{filename}\" alt bir klasör içinde olduğu için gözardı edilecek; zip "
 "içindeki tüm fotolar en üst klasörde yer almalı. "
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr "Zip arşivindeki \"{0}\" dosyası işlenemedi."
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr ""
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Çok düşük"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Düşük"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Orta-Düşük"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Orta"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Orta-Yüksek"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Yüksek"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Çok Yüksek"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Üst"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Sağ"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Alt"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Sol"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Merkez (Varsayılan)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Soldan sağa ayna aksi"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Yukardan aşağıya ayna aksi"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "90 derece saat yönü tersine döndür"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "90 derece saat yönüne döndür"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "180 derece döndür"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Kutu-kutu, kiremit tarzı"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Ölçekle"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 "Birden çok filtreyi şu şekilde uygulayabilirsin: \"ILK_FILTRE->IKINCI_FILTRE-"
 ">UCUNCU_FILTRE\". Filtreler sırayla uygulanacaktır. Etkin filtreler: %s"
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "yayınlama tarihi"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "başlık"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "başlık slug"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "\"Slug\" bir nesne için url dostu eşsiz bir başlıktır."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "tanım"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "Görünür mü?"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Görülebilir galeriler varsayılan görünümlerde sergilenirler."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "fotolar"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr "siteler"
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "galeri"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "galeriler"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "sayaç"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "imaj"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "çekilme tarihi"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr "görüntüleme sayısı"
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "şuradan kes"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "efekt"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "Bir \"admin_thumbnail\" foto ölçüleri tanımlanmamış."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Minyatür"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "slug"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "alt yazı"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "eklenme tarihi"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr "Görülebilir fotolar varsayılan görünümlerde sergilenirler."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "foto"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "isim"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "döndür ya da ayna aksi"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "renk"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr "0.0 siyah beyaz bir imaj, 1.0 orjinal imajı verir."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "parlaklık"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr "0.0 siyah bir imaj, 1.0 orjinal imajı verir."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "kontrast"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr "0.0 katı gri bir imaj, 1.0 orjinal imajı verir."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "keskinlik"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr "0.0 blanık bir imaj, 1.0 orjinal imajı verir."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "filtreler"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "boyutlar"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "Yansımanın yüksekliği, orjinal imajın yüzdelik oranıdır. 0.0 hiç yansıma "
 "vermezken, 1.0 orjinal imaj yüksekliği kadar bir yansıma sağlar."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "gerilim"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr "Yansıma gradyantının başlangıç opaklığı."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 "Yansıma gradyantının arkaplan rengi. Bu ayarı sayfanızın arka plan rengine "
 "eş seçin."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "foto efekti"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "foto efektleri"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "tarz"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "opaklık"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "Katmanın opaklığı."
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "su damga"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "su damgaları"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "Foto ebat isimleri sadece hafler, rakamlar ve alt tireler içerebilir. "
 "Örnekler: \"minyaturler\", \"sergi\", \"kucuk\", \"ana_sayfa_vinyeti\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "genişlik"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr "Eğer genişlik 0 verilirse, verilen yüksekliğe göre ölçeklenecek."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "yükseklik"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr "Eğer yükseklik 0 verilirse, verilen genişliğe göre ölçeklenecek. "
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "kalite"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "JPEG kalitesi"
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "imajı büyüt?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr "Eğer seçilirse, imaj verilen ölçülere göre gerekli ise büyütülecek."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "sığdırmak için kes?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "Eğer seçilirse imaj ölçeklenecek ve verilen ebatlara sığdırmak için "
 "ölçeklenecek."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "wstępnie cachować?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr "Eğer seçilirse, fotolar eklenirken, ön belleklenecek."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "görüntüleme sayısını arttır?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Eğer seçilirse, imajın \"görüntülenme sayısı\", foto görüntülendikçe artacak."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "su damgası imajı"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "photo ebadı"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "photo ebadları"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr "Eğer hem yükseklik hem de genişlik belirtilirse fotoğraf kırpılır."
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/tr/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/tr/LC_MESSAGES/django.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Turkish (http://www.transifex.com/richardbarran/django-"
 "photologue/language/tr/)\n"
+"Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid ""
 "\n"
 "\t\t\t\t    page %(page_number)s of %(total_pages)s\n"
 "\t\t\t\t"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/it/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 # Translators:
+# David Kwast <david.kwast@gmail.com>, 2009
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
 "PO-Revision-Date: 2017-09-19 14:01+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
-"Language-Team: Italian (http://www.transifex.com/richardbarran/django-"
-"photologue/language/it/)\n"
-"Language: it\n"
+"Language-Team: Portuguese (Brazil) (http://www.transifex.com/richardbarran/"
+"django-photologue/language/pt_BR/)\n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: admin.py:62
 #, python-format
 msgid ""
 "The following photo does not belong to the same site(s) as the gallery, so "
 "will never be displayed: %(photo_list)s."
 msgid_plural ""
@@ -104,492 +105,489 @@
 msgid "Remove selected photos from the current site"
 msgstr ""
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr ""
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr ""
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr ""
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr ""
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
-msgstr "La didascalia verrà aggiunta a tutte le foto"
+msgstr "A legenda será adicionada para todas as fotos"
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr ""
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr ""
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
-"Deseleziona l'opzione per rendere private le immagini e la galleria una "
-"volta caricata."
+"Desmarque esta opção para tornar a galeria, incluindo suas fotos, não "
+"pública."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr ""
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr ""
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr ""
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr ""
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
-msgstr "Molto Bassa"
+msgstr "Muito Baixa"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
-msgstr "Bassa"
+msgstr "Baixa"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
-msgstr "Medio-Bassa"
+msgstr "Média-Baixa"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
-msgstr "Media"
+msgstr "Média"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
-msgstr "Medio-Alta"
+msgstr "Média-Alta"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Alta"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
-msgstr "Molto Alta"
+msgstr "Muito Alta"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
-msgstr "In alto"
+msgstr "Cima"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
-msgstr "A destra"
+msgstr "Direita"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
-msgstr "In basso"
+msgstr "Baixo"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
-msgstr "A sinistra"
+msgstr "Esquerda"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
-msgstr "Al centro (Default)"
+msgstr "Centro (Padrão)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
-msgstr "Inverti destra con sinistra"
+msgstr "Inverter da direita para a esquerda"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
-msgstr "Inverti alto con basso"
+msgstr "Inverter de cima para baixo"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
-msgstr "Ruota di 90 gradi in senso anti-orario"
+msgstr "Rotacionar 90 graus no sentido anti-horário"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
-msgstr "Ruota di 90 gradi in senso orario"
+msgstr "Rotacionar 90 graus no sentido horário"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
-msgstr "Ruota di 180 gradi"
+msgstr "Rotacionar 180 graus"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
-msgstr "Affianca"
+msgstr "Título"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
-msgstr "Ridimensiona"
+msgstr "Escala"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
-"Collega filtri multipli in cascata con il seguente schema \"FILTRO_UNO-"
-">FILTRO_DUE->FILTER_TRE\". I filtri saranno applicati in ordine alle "
-"immagini. I seguenti filtri sono disponibili: %s."
+"Encadeie multiplos filtros usando o seguinte padrão \"FILTRO_UM->FILTRO_DOIS-"
+">FILTRO_TRÊS\". Os filtors serão aplicados na ordem em que foram encadeados. "
+"Os seguintes filtros estão disponíveis: %s."
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
-msgstr "data di pubblicazione"
+msgstr "data de publicação"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
-msgstr "titolo"
+msgstr "título"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
-msgstr "slug"
+msgstr "slug do título"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
-msgstr "Uno \"Slug\" è un titolo univoco per un oggetto, usabile come URL."
+msgstr "Um \"slug\" é um título único compatível com uma URL."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
-msgstr "descrizione"
+msgstr "descrição"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
-msgstr "è pubblica"
+msgstr "é publico"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
-msgstr "Le gallerie pubbliche verranno visualizzate nelle viste di default."
+msgstr "Galerias públicas serão mostradas nas views padrões."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
-msgstr "foto"
+msgstr "fotos"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr ""
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
-msgstr "galleria"
+msgstr "Galeria"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
-msgstr "gallerie"
+msgstr "Galerias"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
-msgstr "numero"
+msgstr "contagem"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
-msgstr "immagine"
+msgstr "imagem"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
-msgstr "data dello scatto"
+msgstr "data em que a foto foi tirada"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr ""
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
-msgstr "ritagliata da"
+msgstr "cortar"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
-msgstr "effetto"
+msgstr "efeito"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
-msgstr "La dimensione \"admin_thumbnail\" non è ancora stata creata."
+msgstr "Um tamanho para a foto do \"admin_thumbnail\" ainda não foi definido."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
-msgstr "Miniatura"
+msgstr "Thumbnail"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "slug"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
-msgstr "didascalia"
+msgstr "legenda"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
-msgstr "data di inserimento"
+msgstr "data que foi adicionado(a)"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
-msgstr "Le fotografie pubbliche verranno visualizzate nelle viste di default."
+msgstr "Fotos públicas serão mostradas nas views padrões."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
-msgstr "fotografia"
+msgstr "foto"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "nome"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
-msgstr "ruota o inverti"
+msgstr "rotacionar ou inverter"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
-msgstr "colore"
+msgstr "cor"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
-"Un fattore di 0.0 restituisce un'immagine in bianco e nero, un fattore di "
-"1.0 restituisce l'immagine originale."
+"O valor 0.0 deixará a imagem em preto e branco, o fator 1.0 não alterará a "
+"mesma.A factor of 0.0 gives a black and white image, a factor of 1.0 gives "
+"the original image."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
-msgstr "luminosità"
+msgstr "brilho"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
-"Un fattore di 0.0 restituisce un'immagine nera, un fattore di 1.0 "
-"restituisce l'immagine originale."
+"O valor 0.0 deixará a imagem totalmente preta, o valor 1.0 não alterará a "
+"mesma."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
-msgstr "contrasto"
+msgstr "contraste"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
-"Un fattore di 0.0 restituisce un'immagine grigia, un fattore di 1.0 "
-"restituisce l'immagine originale."
+"O valor 0.0 deixará a imagem totalmente cinza, o valor 1.0 não alterará a "
+"mesma."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
-msgstr "nitidezza"
+msgstr "nitidez"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
-"Un fattore di 0.0 restituisce un'immagine sfuocata, un fattore di 1.0 "
-"restituisce l'immagine originale."
+"O valor 0.0 deixará a imagem embaçada, o valor 1.0 não alterará a mesma."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
-msgstr "filtri"
+msgstr "filtros"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
-msgstr "dimensione"
+msgstr "tamanho"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
-"L'altezza del riflesso come percentuale dell'immagine originale. Un fattore "
-"di 0.0 non aggiunge nessun riflesso, un fattore di 1.0 aggiunge un riflesso "
-"della stessa altezza dell'immagine originale."
+"Valor entre 0 e 1. O reflexo será proporcional a altura da imagem. O valor "
+"0.0 não produzirá um reflexo e o valor 1.0 produzirá um reflexo com a mesma "
+"altura da imagem original."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
-msgstr "intensità"
+msgstr "força"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
-msgstr "Opacità iniziale del gradiente del riflesso."
+msgstr "O valor inicial da opacidade do gradiente de reflexão."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
-"Il colore di sfondo del gradiente di riflesso. Sceglilo in modo che "
-"corrisponda al colore dello sfondo della tua immagine."
+"A cor de fundo do gradiente de reflexão. Ajuste de acordo com a cor de fundo "
+"de sua página."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
-msgstr "effetto fotografico"
+msgstr "efeito de foto"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
-msgstr "effetti fotografici"
+msgstr "efeitos de foto"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
-msgstr "stile"
+msgstr "estilo"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
-msgstr "opacità"
+msgstr "opacidade"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
-msgstr "Opacità della copertura"
+msgstr "A opacidade da sobre-imagem (overlay)"
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
-msgstr "watermark"
+msgstr "marca d'água"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
-msgstr "watermark"
+msgstr "marcas d'água"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
-"Le dimensioni fotografiche devono contenere solo lettere, numeri o caratteri "
-"di sottolineatura. Per esempio: : \"thumbnail\", \"display\", \"small\", "
-"\"main_page_widget\"."
+"O nome do tamanho da foto somente poderá conter letras, números e "
+"underscores. Exemplos: \"thumbnail\", \"tela\", \"pequeno\", \"grande\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
-msgstr "larghezza"
+msgstr "largura"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
-"Se la dimensione è \"0\", l'immagine verrà ridimensionata all'altezza "
-"specificata."
+"Se o valor da largura for \"0\", a imagem será redimensionada de acordo com "
+"a altura informada"
 
-#: models.py:774
+#: models.py:782
 msgid "height"
-msgstr "altezza"
+msgstr "altura"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
-"Se l'altezza è \"0\", l'immagine verrà ridimensionata alla larghezza "
-"specificata."
+"Se o valor da altura for \"0\", a imagem será redimensionada de acordo com a "
+"largura informada"
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
-msgstr "qualità"
+msgstr "qualidade"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
-msgstr "qualità dell'immagine JPEG"
+msgstr "qualidade da imagem JPEG"
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
-msgstr "ingrandisco le immagini?"
+msgstr "Aumentar a dimensão das imagens?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
-"Se selezionato, l'immagine verrà ingrandita (se necessario) per "
-"corrispondere alle dimensioni specificate. Dimensioni ritagliate verranno "
-"ridimensionate senza tenere conto di questa configurazione."
+"Se selecionado, a imagem terá sua dimensão aumentada. Imagens cortadas serão "
+"redimensionadas independentemente desta configuração."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
-msgstr "Ritaglio per stare nelle dimensioni?"
+msgstr "cortar para conformar?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
-"Se selezionato, l'immagine verrà ridimensionata e ritagliata per rientrare "
-"nelle dimensioni specificate."
+"Se selecionado, a imagem será redimensionada e cortada para se conformar de "
+"acordo com as dimensões fornecidas."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
-msgstr "pre-cache?"
+msgstr "pré-cachear?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
-"Se selezionato, questa dimensione di foto verrà pre-salvata mentre le foto "
-"sono inserite."
+"Se selecionado, o tamanho da foto será pré-cacheado logo após sua inclusão."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
-msgstr "incrementa il contatore di visualizzazioni?"
+msgstr "Incrementar o contador de visualizações?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
-"Se selezionato, il \"contatore di visualizzazioni\" dell'immagine sarà "
-"incrementato ad ogni visualizzazione dell'immagine."
+"Se selecionado, o \"view_count\" desta imagem será incrementado quando o "
+"tamanho da mesma for mostrado."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
-msgstr "immagine di watermark"
+msgstr "imagem para marca d'água"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
-msgstr "dimensione della foto"
+msgstr "tamanho da foto"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
-msgstr "dimensioni delle foto"
+msgstr "tamanhos das fotos"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr ""
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/it/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/it/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
 "PO-Revision-Date: 2017-09-19 14:01+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Italian (http://www.transifex.com/richardbarran/django-"
 "photologue/language/it/)\n"
+"Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: it\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "Uno \"Slug\" è un titolo univoco per un oggetto, usabile come URL."
 
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
```

### Comparing `django-photologue-3.8.1/photologue/locale/de/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/de/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 # Translators:
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2009
 # Jannis, 2012
 # Jannis , 2012
-# Jannis, 2012-2013
-# Jannis, 2012
+# Jannis Vajen, 2012-2013
+# Jannis Vajen, 2012
 # Jannis Vajen, 2012,2015
-# Jannis, 2015-2016
+# Jannis Vajen, 2015-2016
 # Martin Darmüntzel <martin@trivialanalog.de>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
-"Last-Translator: Jannis\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
+"Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: German (http://www.transifex.com/richardbarran/django-"
 "photologue/language/de/)\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -122,506 +122,506 @@
 msgid "Remove selected photos from the current site"
 msgstr "Entferne ausgewählte Fotos von der aktuellen Seite"
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr "Lade ein Zip-Archiv an Fotos hoch"
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr "Titel"
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 "Für alle hochgeladenen Fotos wird ein Titel aus diesem Titel und einer "
 "fortlaufenden Nummer generiert.<br>Dieses Feld muss nur ausgefüllt werden, "
 "wenn eine neue Galerie angelegt wird, andernfalls ist es optional – wenn "
 "keine Angabe getätigt wird der Name der Galerie als Titel für die "
 "Einzelbilder herangezogen."
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr "Galerie"
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Wähle eine Galerie aus, zu der diese Bilder hinzugefügt werden sollen. Lasse "
 "dieses Feld leer, um eine neue Galerie mit dem angegeben Titel zu erzeugen."
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr "Bildunterschrift"
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "Die Bildunterschrift wird allen Fotos hinzugefügt."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr "Beschreibung"
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr "Eine Beschreibung dieser Galerie. Nur erforderlich bei neuen Galerien."
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr "Ist öffentlich"
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 "Schalte dies aus, um die hochgeladene Galerie und alle enthaltenen Bilder "
 "privat zu machen."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr "Es existiert bereits eine Gallerie mit diesem Titel."
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr ""
 "Wähle eine existierende Galerie aus oder gib einen Titel für eine neue "
 "Galerie ein."
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 "Ignoriere die Datei \"{filename}\", da sie sich in einem Unterordner "
 "befindet; alle Bilder sollten sich im Wurzelverzeichnis der Zip-Datei "
 "befinden."
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr "Konnte die Datei \"{0}\" aus dem Zip-Archiv nicht verarbeiten."
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "Die Fotos wurden zur Galerie \"{0}\" hinzugefügt."
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Sehr niedrig"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Niedrig"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Mittel-niedrig"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Mittel"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Mittel-hoch"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Hoch"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Sehr hoch"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Oben"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Rechts"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Unten"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Links"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Mitte (Standard)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Horizontal spiegeln"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Vertikal spiegeln"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Um 90° nach links drehen"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Um 90° nach rechts drehen"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Um 180° drehen"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Kacheln"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Skalieren"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 "Verkette mehrere Filter in der Art \"FILTER_EINS->FILTER_ZWEI->FILTER_DREI"
 "\". Bildfilter werden nach der Reihe angewendet. Folgende Filter sind "
 "verfügbar: %s."
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "Veröffentlichungsdatum"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "Titel"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "Kurztitel"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr ""
 "Ein Kurztitel (\"slug\") ist ein eindeutiger, URL-geeigneter Titel für ein "
 "Objekt."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "Beschreibung"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "ist öffentlich"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Öffentliche Galerien werden in den Standard-Views angezeigt."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "Fotos"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr "Seiten"
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "Galerie"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "Galerien"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "Anzahl"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "Bild"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "Aufnahmedatum"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 "Datum, an dem das Foto geschossen wurde; ausgelesen aus den EXIF-Daten."
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr "Anzahl an Aufrufen"
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "Beschneiden von"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "Effekt"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "Es ist keine Fotogröße \"admin_thumbnail\" definiert."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Vorschaubild"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "Kurztitel"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "Bildunterschrift"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "Datum des Eintrags"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr "Öffentliche Fotos werden in den Standard-Views angezeigt."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "Foto"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "Name"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "drehen oder spiegeln"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "Farbe"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 "Ein Faktor von 0.0 erzeugt ein Schwarzweißbild, ein Faktor von 1.0 erhält "
 "das Originalbild."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "Helligkeit"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Ein Faktor von 0.0 erzeugt ein schwarzes Bild, ein Faktor von 1.0 erhält das "
 "Originalbild."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "Kontrast"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Ein Faktor von 0.0 erzeugt ein opak graues Bild, ein Faktor von 1.0 erhält "
 "das Originalbild."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "Schärfe"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Ein Faktor von 0.0 erzeugt ein sehr unscharfes Bild, ein Faktor von 1.0 "
 "erhält das Originalbild."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "Filter"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "Größe"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "Die Höhe der Reflexion als Prozentwert des Originalbildes. Ein Faktor von "
 "0.0 erzeugt keine Reflexion, ein Faktor von 1.0 ergibt eine Reflexion von "
 "der Höhe des Originalbildes."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "Stärke"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr "Die Anfangs-Deckung des Reflexions-Verlaufs."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 "Die Hintergrundfarbe des Reflexions-Verlaufs. Setze dies auf die "
 "Hintergrundfarbe deiner Seite."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "Foto-Effekt"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "Foto-Effekte"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "Stil"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "Deckung"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "Deckung (Opazität) der Überlagerung"
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "Wasserzeichen"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "Wasserzeichen"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "Der Name der Fotogröße darf nur Buchstaben, Zahlen und Unterstriche "
 "enthalten. Beispiele: \"thumbnail\", \"display\", \"small\", "
 "\"main_page_widget\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "Breite"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Wenn die Breite auf \"0\" gesetzt ist, wird das Bild proportional auf die "
 "angebene Höhe skaliert."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "Höhe"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Wenn die Höhe auf \"0\" gesetzt ist, wird das Bild proportional auf die "
 "angebene Breite skaliert."
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "Qualität"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "JPEG-Bildqualität"
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "Bilder hochskalieren?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "Soll das Bild hochskaliert werden, um das angegebene Format zu erreichen? "
 "Beschnittene Größen werden unabhängig von dieser Einstellung bei Bedarf "
 "hochskaliert."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "Zuschneiden?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "Soll das Bild auf das angegebene Format skaliert und beschnitten werden?"
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "Vorausspeichern?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 "Soll diese Bildgröße im Voraus gespeichert (pre-cached) werden, wenn Fotos "
 "hinzugefügt werden?"
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "Bildzähler?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Soll der Ansichts-Zähler (view-count) hochgezählt werden, wenn ein Foto "
 "dieser Größe angezeigt wird?"
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "Wasserzeichen-Bild"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "Foto-Größe"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "Foto-Größen"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr ""
 "Fotos können nur zugeschnitten werden, wenn Breite und Höhe angegeben sind."
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr "Lade ein Zip-Archiv hoch"
```

### Comparing `django-photologue-3.8.1/photologue/locale/de/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/de/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
-"Last-Translator: Jannis\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
+"Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: German (http://www.transifex.com/richardbarran/django-"
 "photologue/language/de/)\n"
+"Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "\n"
 "\t\t\t\t    page %(page_number)s of %(total_pages)s\n"
 "\t\t\t\t"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/nl/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/nl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 # Translators:
 # Peter-Paul van Gemerden <info@ppvg.nl>, 2009
 # Reint T. Kamp <reint@fastmail.com>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Dutch (http://www.transifex.com/richardbarran/django-"
 "photologue/language/nl/)\n"
 "Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -113,495 +113,495 @@
 msgid "Remove selected photos from the current site"
 msgstr "Verwijder geselecteerde foto van de huidige pagina"
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr "Upload een zip-archief met foto's"
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr "Titel"
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr "Gallerij"
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Selecteer een gallerij om deze foto's aan toe te voegen. Laat dit leeg om "
 "een nieuwe gallerij aan te maken met de gegeven titel. "
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr "Onderschrift"
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "Onderschrift wordt toegevoegd aan alle foto's."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr "Omschrijving"
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr "Is publiek toegankelijk"
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr "Haal dit vinkje weg om de geüploade galerij en foto's privé te maken."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr "Een gallerij met deze titel bestaat al"
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr ""
 "Selecteer een bestaande gallerij of vul de titel in van een nieuwe gallerij"
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 "Bestand \"{filename}\" ligt in een onderliggende map. Alleen afbeeldingen in "
 "de bovenste folder van de zip worden gebruikt. "
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr "Kon bestand \"{0}\" in het zip-archief niet verwerken."
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "De foto's zijn toegevoegd aan gallerij \"{0}\"."
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Zeer laag"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Laag"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Middel-laag"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Gemiddeld"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Middel-hoog"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Hoog"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Zeer hoog"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Boven"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Rechts"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Onder"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Links"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Midden (standaard)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Spiegel horizontaal"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Spiegel verticaal"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Roteer 90 graden linksom"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Roteer 90 graden rechtsom"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Roteer 180 graden"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Tegelen"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Schalen"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 "Keten meerdere filters aan elkaar met het patroon: \"FILTER_EEN->FILTER_TWEE-"
 ">FILTER_DRIE\". Afbeeldingsfilters worden in volgorde toegepast. De volgende "
 "filters zijn beschikbaar: %s."
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "datum gepubliceerd"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "titel"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "titel 'zetsel'"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "Een \"zetsel\" is een unieke URL-vriendelijke titel voor een object."
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "beschrijving"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "is openbaar"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Openbare galerijen worden weergegeven in de standaardviews."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "foto's"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr "pagina's"
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "galerij"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "galerijen"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "aantal"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "afbeelding"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "datum genomen"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr "weergave teller"
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "afknippen vanaf"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "effect"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "Er is geen \"admin_thumbnail\" foto-maat vastgelegd."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Miniatuur"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "zetsel"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "onderschrift"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "datum toegevoegd"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr "Openbare foto's worden weergegeven in de standaardviews."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "foto"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "naam"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "roteer of spiegel"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "kleur"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 "Een factor van 0.0 geeft een zwart-wit afbeelding, een factor van 1.0 geeft "
 "de originele afbeelding."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "helderheid"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Een factor van 0.0 geeft een zwarte afbeelding, een factor van 1.0 geeft de "
 "originele afbeelding."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "contrast"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Een factor van 0.0 geeft een egaal grijze afbeelding, een factor van 1.0 "
 "geeft de originele afbeelding."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "scherpte"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "Een factor van 0.0 geeft een vervaagde afbeelding, een factor van 1.0 geeft "
 "de originele afbeelding."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "filters"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "afmeting"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "De hoogte van de reflectie als precentage van de originele afbeelding. Een "
 "factor van 0.0 voegt geen reflectie toe, een factor van 1.0 voegt een "
 "reflectie toe met een gelijke hoogte als de originele afbeelding."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "sterkte"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr "De initiële doorzichtigheid van de reflectie-gradatie."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 "De achtergrondkleur van de reflectie-gradatie. Stel dit in als hetzelfde als "
 "de achtergrondkleur van je pagina."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "foto-effect"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "foto-effecten"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "stijl"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "doorzichtigheid"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "De doorzichtigheid van overliggende afbeelding."
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "watermerk"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "watermerken"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "De naam van de foto-maat mag alleen letters, nummers en underscores "
 "bevatten. Voorbeelden: \"miniatuur\", \"weergave\", \"klein\", "
 "\"hoofdpagina_zijbalk_miniatuur\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "breedte"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Als de breedte op \"0\" wordt gezet zal de afbeelding geschaald worden naar "
 "de opgegeven hoogte."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "hoogte"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Als de hoogte op \"0\" wordt gezet zal de afbeelding geschaald worden naar "
 "de opgegeven breedte."
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "kwaliteit"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "JPEG afbeeldingskwaliteit"
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "afbeeldingen opschalen?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "Als dit is gekozen zal de afbeelding, indien nodig, opgeschaald worden naar "
 "opgegeven afmetingen. Afgeknipte maten worden altijd opgeschaald, ongeacht "
 "deze instelling."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "gepast afknippen?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "Als dit is gekozen zal de afbeelding geschaald en afgeknipt worden naar de "
 "opgegeven afmetingen."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "vooraf cachen?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 "Als dit is gekozen zullen foto's met deze foto-maat van te voren worden "
 "gecached wanneer ze worden toegevoegd."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "aantal vertoningen ophogen?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Als dit is gekozen zal het aantal vertoningen van de afbeelding worden "
 "opgehoogd wanneer deze foto-maat wordt weergegeven."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "watermerk-afbeelding"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "foto-maat"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "foto-maten"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr ""
 "Kan alleen foto's uitsnijden als zowel de waarde van de breedte en de hoogte "
 "zijn ingesteld."
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
```

### Comparing `django-photologue-3.8.1/photologue/locale/nl/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/nl/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
+"PO-Revision-Date: 2017-12-03 14:47+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Dutch (http://www.transifex.com/richardbarran/django-"
 "photologue/language/nl/)\n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: nl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "\n"
 "\t\t\t\t    page %(page_number)s of %(total_pages)s\n"
 "\t\t\t\t"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/da/LC_MESSAGES/django.po` & `django-photologue-3.9/photologue/locale/da/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 # Translators:
 # Michael Lind Mortensen <illio@cs.au.dk>, 2009
 # Rasmus Mortensen <Rasmus.klett@gmail.com>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2017-12-03 14:46+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
+"POT-Creation-Date: 2019-04-20 16:51+0200\n"
+"PO-Revision-Date: 2017-12-03 14:46+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Danish (http://www.transifex.com/richardbarran/django-"
 "photologue/language/da/)\n"
 "Language: da\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -110,493 +110,493 @@
 msgid "Remove selected photos from the current site"
 msgstr "Fjern valgte billeder fra den nuværende webside"
 
 #: admin.py:205 templates/admin/photologue/photo/upload_zip.html:27
 msgid "Upload a zip archive of photos"
 msgstr "Upload et zip-arkiv af billeder"
 
-#: forms.py:34
+#: forms.py:31
 msgid "Title"
 msgstr "Titel"
 
-#: forms.py:37
+#: forms.py:34
 msgid ""
 "All uploaded photos will be given a title made up of this title + a "
 "sequential number.<br>This field is required if creating a new gallery, but "
 "is optional when adding to an existing gallery - if not supplied, the photo "
 "titles will be creating from the existing gallery name."
 msgstr ""
 
-#: forms.py:43
+#: forms.py:40
 msgid "Gallery"
 msgstr "Galleri"
 
-#: forms.py:45
+#: forms.py:42
 msgid ""
 "Select a gallery to add these images to. Leave this empty to create a new "
 "gallery from the supplied title."
 msgstr ""
 "Vælg et galleri at tilføje disse billeder til. Lad feltet være tomt for at "
 "oprette et nyt galleri med den valgte title"
 
-#: forms.py:47
+#: forms.py:44
 msgid "Caption"
 msgstr "Billedtekst"
 
-#: forms.py:49
+#: forms.py:46
 msgid "Caption will be added to all photos."
 msgstr "Billedeteksten vil blive tilføjet til alle billeder."
 
-#: forms.py:50
+#: forms.py:47
 msgid "Description"
 msgstr "Beskrivelse"
 
-#: forms.py:52
+#: forms.py:49
 msgid "A description of this Gallery. Only required for new galleries."
 msgstr ""
 
-#: forms.py:53
+#: forms.py:50
 msgid "Is public"
 msgstr "Er offentlig"
 
-#: forms.py:56
+#: forms.py:53
 msgid ""
 "Uncheck this to make the uploaded gallery and included photographs private."
 msgstr ""
 "Fjern afkrydsningen her for at gøre det uploadede galleri og alle "
 "inkluderede billeder private."
 
-#: forms.py:79
+#: forms.py:76
 msgid "A gallery with that title already exists."
 msgstr "Et galleri med den titel eksisterer allerede"
 
-#: forms.py:89
+#: forms.py:86
 msgid "Select an existing gallery, or enter a title for a new gallery."
 msgstr "Vælg et eksisterende galleri, eller skriv en titel til et nyt galleri"
 
-#: forms.py:122
+#: forms.py:119
 #, python-brace-format
 msgid ""
 "Ignoring file \"{filename}\" as it is in a subfolder; all images should be "
 "in the top folder of the zip."
 msgstr ""
 "Ignorerer fil \"{filename}\", da det er en undermappe; alle billeder bør "
 "være i topmappen af zip-filen"
 
-#: forms.py:163
+#: forms.py:160
 #, python-brace-format
 msgid "Could not process file \"{0}\" in the .zip archive."
 msgstr "Kunne ikke behandle fil \"{0}\" i zip-arkivet."
 
-#: forms.py:179
+#: forms.py:176
 #, python-brace-format
 msgid "The photos have been added to gallery \"{0}\"."
 msgstr "Billederne er blevet tilføjet til galleri \"{0}\""
 
-#: models.py:99
+#: models.py:100
 msgid "Very Low"
 msgstr "Meget Lav"
 
-#: models.py:100
+#: models.py:101
 msgid "Low"
 msgstr "Lav"
 
-#: models.py:101
+#: models.py:102
 msgid "Medium-Low"
 msgstr "Medium Lav"
 
-#: models.py:102
+#: models.py:103
 msgid "Medium"
 msgstr "Medium"
 
-#: models.py:103
+#: models.py:104
 msgid "Medium-High"
 msgstr "Medium Høj"
 
-#: models.py:104
+#: models.py:105
 msgid "High"
 msgstr "Høj"
 
-#: models.py:105
+#: models.py:106
 msgid "Very High"
 msgstr "Meget Høj"
 
-#: models.py:110
+#: models.py:111
 msgid "Top"
 msgstr "Top"
 
-#: models.py:111
+#: models.py:112
 msgid "Right"
 msgstr "Højre"
 
-#: models.py:112
+#: models.py:113
 msgid "Bottom"
 msgstr "Bund"
 
-#: models.py:113
+#: models.py:114
 msgid "Left"
 msgstr "Venstre"
 
-#: models.py:114
+#: models.py:115
 msgid "Center (Default)"
 msgstr "Center (Standard)"
 
-#: models.py:118
+#: models.py:119
 msgid "Flip left to right"
 msgstr "Flip venstre til højre"
 
-#: models.py:119
+#: models.py:120
 msgid "Flip top to bottom"
 msgstr "Flip top til bund"
 
-#: models.py:120
+#: models.py:121
 msgid "Rotate 90 degrees counter-clockwise"
 msgstr "Roter 90 grader mod uret"
 
-#: models.py:121
+#: models.py:122
 msgid "Rotate 90 degrees clockwise"
 msgstr "Roter 90 grader med uret"
 
-#: models.py:122
+#: models.py:123
 msgid "Rotate 180 degrees"
 msgstr "Roter 180 grader"
 
-#: models.py:126
+#: models.py:127
 msgid "Tile"
 msgstr "Tile"
 
-#: models.py:127
+#: models.py:128
 msgid "Scale"
 msgstr "Skala"
 
-#: models.py:137
+#: models.py:138
 #, python-format
 msgid ""
 "Chain multiple filters using the following pattern \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Image filters will be applied in order. The following "
 "filters are available: %s."
 msgstr ""
 "Sæt adskillige filtre i kæde vha. følgende mønster \"FILTER_ONE->FILTER_TWO-"
 ">FILTER_THREE\". Billedefiltre vil blive påført i den anførte rækkefølge. De "
 "følgende filtre er tilgænglige: %s."
 
-#: models.py:161
+#: models.py:162
 msgid "date published"
 msgstr "dato offentliggjort"
 
-#: models.py:163 models.py:508
+#: models.py:164 models.py:513
 msgid "title"
 msgstr "titel"
 
-#: models.py:166
+#: models.py:167
 msgid "title slug"
 msgstr "titel slug"
 
-#: models.py:169 models.py:514
+#: models.py:170 models.py:519
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "En \"slug\" er en unik URL-venlig titel for et objekt"
 
-#: models.py:170 models.py:586
+#: models.py:171 models.py:591
 msgid "description"
 msgstr "beskrivelse"
 
-#: models.py:172 models.py:519
+#: models.py:173 models.py:524
 msgid "is public"
 msgstr "er offentlig"
 
-#: models.py:174
+#: models.py:175
 msgid "Public galleries will be displayed in the default views."
 msgstr "Offentlige gallerier vil blive vist i standard views."
 
-#: models.py:178 models.py:531
+#: models.py:179 models.py:536
 msgid "photos"
 msgstr "billeder"
 
-#: models.py:180 models.py:522
+#: models.py:181 models.py:527
 msgid "sites"
 msgstr "websider"
 
-#: models.py:188
+#: models.py:189
 msgid "gallery"
 msgstr "galleri"
 
-#: models.py:189
+#: models.py:190
 msgid "galleries"
 msgstr "gallerier"
 
-#: models.py:226
+#: models.py:227
 msgid "count"
 msgstr "tæller"
 
-#: models.py:242 models.py:727
+#: models.py:243 models.py:735
 msgid "image"
 msgstr "billede"
 
-#: models.py:245
+#: models.py:246
 msgid "date taken"
 msgstr "dato taget"
 
-#: models.py:248
+#: models.py:249
 msgid "Date image was taken; is obtained from the image EXIF data."
 msgstr ""
 
-#: models.py:249
+#: models.py:250
 msgid "view count"
 msgstr "set tæller"
 
-#: models.py:252
+#: models.py:253
 msgid "crop from"
 msgstr "beskær fra"
 
-#: models.py:261
+#: models.py:262
 msgid "effect"
 msgstr "effekt"
 
-#: models.py:281
+#: models.py:282
 msgid "An \"admin_thumbnail\" photo size has not been defined."
 msgstr "En \"admin_thumbnail\" billedestørrelse er ikke blevet defineret."
 
-#: models.py:289
+#: models.py:288
 msgid "Thumbnail"
 msgstr "Thumbnail"
 
-#: models.py:511
+#: models.py:516
 msgid "slug"
 msgstr "slug"
 
-#: models.py:515
+#: models.py:520
 msgid "caption"
 msgstr "billedetekst"
 
-#: models.py:517
+#: models.py:522
 msgid "date added"
 msgstr "dato tilføjet"
 
-#: models.py:521
+#: models.py:526
 msgid "Public photographs will be displayed in the default views."
 msgstr "Offentlige billeder vil blive vist i standard views."
 
-#: models.py:530
+#: models.py:535
 msgid "photo"
 msgstr "billede"
 
-#: models.py:583 models.py:759
+#: models.py:588 models.py:767
 msgid "name"
 msgstr "navn"
 
-#: models.py:658
+#: models.py:666
 msgid "rotate or flip"
 msgstr "roter eller flip"
 
-#: models.py:662 models.py:690
+#: models.py:670 models.py:698
 msgid "color"
 msgstr "farve"
 
-#: models.py:664
+#: models.py:672
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
 msgstr ""
 "En faktor af 0.0 giver et sort og hvidt billede, en faktor af 1.0 giver det "
 "originale billede."
 
-#: models.py:666
+#: models.py:674
 msgid "brightness"
 msgstr "lysstyrke"
 
-#: models.py:668
+#: models.py:676
 msgid ""
 "A factor of 0.0 gives a black image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "En faktor af 0.0 giver et sort billede, en faktor af 1.0 giver det originale "
 "billede."
 
-#: models.py:670
+#: models.py:678
 msgid "contrast"
 msgstr "kontrast"
 
-#: models.py:672
+#: models.py:680
 msgid ""
 "A factor of 0.0 gives a solid grey image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "En faktor af 0.0 giver et solidt gråt billede, en faktor af 1.0 giver det "
 "originale billede."
 
-#: models.py:674
+#: models.py:682
 msgid "sharpness"
 msgstr "skarphed"
 
-#: models.py:676
+#: models.py:684
 msgid ""
 "A factor of 0.0 gives a blurred image, a factor of 1.0 gives the original "
 "image."
 msgstr ""
 "En faktor af 0.0 giver et sløret billede, en faktor af 1.0 giver det "
 "originale billede."
 
-#: models.py:678
+#: models.py:686
 msgid "filters"
 msgstr "filtre"
 
-#: models.py:682
+#: models.py:690
 msgid "size"
 msgstr "størrelse"
 
-#: models.py:684
+#: models.py:692
 msgid ""
 "The height of the reflection as a percentage of the orignal image. A factor "
 "of 0.0 adds no reflection, a factor of 1.0 adds a reflection equal to the "
 "height of the orignal image."
 msgstr ""
 "Højden af reflektionen som en procentdel af det originale billede. En faktor "
 "af 0.0 tilføjer ingen reflektion, en faktor af 1.0 tilføjer en reflektion "
 "lig med højden af det oprindelige billede."
 
-#: models.py:687
+#: models.py:695
 msgid "strength"
 msgstr "styrke"
 
-#: models.py:689
+#: models.py:697
 msgid "The initial opacity of the reflection gradient."
 msgstr "Den initielle uigennemsigtighed af den reflektive gradient."
 
-#: models.py:693
+#: models.py:701
 msgid ""
 "The background color of the reflection gradient. Set this to match the "
 "background color of your page."
 msgstr ""
 "Baggrundsfarven af den reflektive gradient. Sæt dette til at passe med "
 "baggrundsfarven af din side."
 
-#: models.py:697 models.py:803
+#: models.py:705 models.py:811
 msgid "photo effect"
 msgstr "billedeeffekt"
 
-#: models.py:698
+#: models.py:706
 msgid "photo effects"
 msgstr "billedeeffekter"
 
-#: models.py:729
+#: models.py:737
 msgid "style"
 msgstr "stil"
 
-#: models.py:733
+#: models.py:741
 msgid "opacity"
 msgstr "uigennemsigtighed"
 
-#: models.py:735
+#: models.py:743
 msgid "The opacity of the overlay."
 msgstr "Uigennemsigtigheden af overlaget."
 
-#: models.py:738
+#: models.py:746
 msgid "watermark"
 msgstr "vandmærke"
 
-#: models.py:739
+#: models.py:747
 msgid "watermarks"
 msgstr "vandmærker"
 
-#: models.py:763
+#: models.py:771
 msgid ""
 "Photo size name should contain only letters, numbers and underscores. "
 "Examples: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 msgstr ""
 "Billede størrelse navn må kun indeholde bogstaver, numre og underscores. "
 "Eksempler: \"thumbnail\", \"display\", \"small\", \"main_page_widget\"."
 
-#: models.py:770
+#: models.py:778
 msgid "width"
 msgstr "bredde"
 
-#: models.py:773
+#: models.py:781
 msgid ""
 "If width is set to \"0\" the image will be scaled to the supplied height."
 msgstr ""
 "Hvis bredden er sat til \"0\" vil billede blive skaleret til den givne højde."
 
-#: models.py:774
+#: models.py:782
 msgid "height"
 msgstr "højde"
 
-#: models.py:777
+#: models.py:785
 msgid ""
 "If height is set to \"0\" the image will be scaled to the supplied width"
 msgstr ""
 "Hvis højden er sat til \"0\" vil billede blive skaleret til den givne bredde."
 
-#: models.py:778
+#: models.py:786
 msgid "quality"
 msgstr "kvalitet"
 
-#: models.py:781
+#: models.py:789
 msgid "JPEG image quality."
 msgstr "JPEG billedekvalitet"
 
-#: models.py:782
+#: models.py:790
 msgid "upscale images?"
 msgstr "opskaler billeder?"
 
-#: models.py:784
+#: models.py:792
 msgid ""
 "If selected the image will be scaled up if necessary to fit the supplied "
 "dimensions. Cropped sizes will be upscaled regardless of this setting."
 msgstr ""
 "Hvis valgt, vil billedet blive skaleret op såfremt det er nødvendigt for at "
 "passe til de givne dimensioner. Beskårede størrelser vil blive opskaleret "
 "uanset denne indstilling."
 
-#: models.py:788
+#: models.py:796
 msgid "crop to fit?"
 msgstr "beskær til at passe?"
 
-#: models.py:790
+#: models.py:798
 msgid ""
 "If selected the image will be scaled and cropped to fit the supplied "
 "dimensions."
 msgstr ""
 "Hvis valgt, vil billedet blive skaleret og beskåret for at passe til de "
 "givne dimensioner."
 
-#: models.py:792
+#: models.py:800
 msgid "pre-cache?"
 msgstr "pre-cache?"
 
-#: models.py:794
+#: models.py:802
 msgid "If selected this photo size will be pre-cached as photos are added."
 msgstr ""
 "Hvis valgt, vil dette billedes størrelse blive pre-cached som billeder "
 "bliver tilføjet."
 
-#: models.py:795
+#: models.py:803
 msgid "increment view count?"
 msgstr "inkrementer set tæller?"
 
-#: models.py:797
+#: models.py:805
 msgid ""
 "If selected the image's \"view_count\" will be incremented when this photo "
 "size is displayed."
 msgstr ""
 "Hvis valgt, vil billedets \"view_count\" blive inkrementeret når billedets "
 "størrelse vises."
 
-#: models.py:809
+#: models.py:817
 msgid "watermark image"
 msgstr "vandmærkebillede"
 
-#: models.py:814
+#: models.py:822
 msgid "photo size"
 msgstr "billedestørrelse"
 
-#: models.py:815
+#: models.py:823
 msgid "photo sizes"
 msgstr "billedestørrelser"
 
-#: models.py:832
+#: models.py:840
 msgid "Can only crop photos if both width and height dimensions are set."
 msgstr "Kan kun beskære billeder hvis både bedde og højde er specificeret."
 
 #: templates/admin/photologue/photo/change_list.html:9
 msgid "Upload a zip archive"
 msgstr "Upload et zip-arkiv"
```

### Comparing `django-photologue-3.8.1/photologue/locale/da/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/da/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
-"PO-Revision-Date: 2017-09-19 14:01+0000\n"
+"PO-Revision-Date: 2017-12-03 14:46+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
 "Language-Team: Danish (http://www.transifex.com/richardbarran/django-"
 "photologue/language/da/)\n"
+"Language: da\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "\n"
 "\t\t\t\t    page %(page_number)s of %(total_pages)s\n"
 "\t\t\t\t"
 msgstr ""
```

### Comparing `django-photologue-3.8.1/photologue/locale/pt_BR/LC_MESSAGES/django.mo` & `django-photologue-3.9/photologue/locale/pt/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Photologue\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-05 20:42+0000\n"
 "PO-Revision-Date: 2017-09-19 14:01+0000\n"
 "Last-Translator: Richard Barran <richard@arbee-design.co.uk>\n"
-"Language-Team: Portuguese (Brazil) (http://www.transifex.com/richardbarran/"
-"django-photologue/language/pt_BR/)\n"
+"Language-Team: Portuguese (http://www.transifex.com/richardbarran/django-"
+"photologue/language/pt/)\n"
+"Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pt_BR\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "A \"slug\" is a unique URL-friendly title for an object."
 msgstr "Um \"slug\" é um título único compatível com uma URL."
 
 msgid ""
 "A factor of 0.0 gives a black and white image, a factor of 1.0 gives the "
 "original image."
```

### Comparing `django-photologue-3.8.1/photologue/utils/reflection.py` & `django-photologue-3.9/photologue/utils/reflection.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/utils/watermark.py` & `django-photologue-3.9/photologue/utils/watermark.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,9 +59,10 @@
 def test():
     im = Image.open('test.png')
     mark = Image.open('overlay.png')
     watermark(im, mark, 'tile', 0.5).show()
     watermark(im, mark, 'scale', 1.0).show()
     watermark(im, mark, (100, 100), 0.5).show()
 
+
 if __name__ == '__main__':
     test()
```

### Comparing `django-photologue-3.8.1/photologue/res/sample.jpg` & `django-photologue-3.9/photologue/res/sample.jpg`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/res/test_photologue_portrait.jpg` & `django-photologue-3.9/photologue/res/test_photologue_portrait.jpg`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/res/test_photologue_square.jpg` & `django-photologue-3.9/photologue/res/test_photologue_square.jpg`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/res/zips/not_image.zip` & `django-photologue-3.9/photologue/res/zips/not_image.zip`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/res/zips/ignored_files.zip` & `django-photologue-3.9/photologue/res/zips/ignored_files.zip`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/res/zips/sample.zip` & `django-photologue-3.9/photologue/res/zips/sample.zip`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/res/test_photologue_landscape.jpg` & `django-photologue-3.9/photologue/res/test_photologue_&quoting.jpg`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/res/test_photologue_&quoting.jpg` & `django-photologue-3.9/photologue/res/test_photologue_landscape.jpg`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/photo_archive_year.html` & `django-photologue-3.9/photologue/templates/photologue/photo_archive_year.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/gallery_archive_year.html` & `django-photologue-3.9/photologue/templates/photologue/gallery_archive_year.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/gallery_archive_day.html` & `django-photologue-3.9/photologue/templates/photologue/gallery_archive_day.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/photo_list.html` & `django-photologue-3.9/photologue/templates/photologue/photo_list.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/photo_archive_day.html` & `django-photologue-3.9/photologue/templates/photologue/photo_archive_day.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/gallery_detail.html` & `django-photologue-3.9/photologue/templates/photologue/gallery_detail.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/photo_archive_month.html` & `django-photologue-3.9/photologue/templates/photologue/photo_archive_month.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/photo_archive.html` & `django-photologue-3.9/photologue/templates/photologue/photo_archive.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/gallery_archive.html` & `django-photologue-3.9/photologue/templates/photologue/gallery_archive.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/includes/paginator.html` & `django-photologue-3.9/photologue/templates/photologue/includes/paginator.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/includes/gallery_sample.html` & `django-photologue-3.9/photologue/templates/photologue/includes/gallery_sample.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/gallery_list.html` & `django-photologue-3.9/photologue/templates/photologue/gallery_list.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/photo_detail.html` & `django-photologue-3.9/photologue/templates/photologue/photo_detail.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/photologue/gallery_archive_month.html` & `django-photologue-3.9/photologue/templates/photologue/gallery_archive_month.html`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/templates/admin/photologue/photo/upload_zip.html` & `django-photologue-3.9/photologue/templates/admin/photologue/photo/upload_zip.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends "admin/base_site.html" %}
-{% load i18n admin_urls admin_static %}
+{% load i18n admin_urls static %}
 
 {# Admin styling code largely taken from http://www.dmertl.com/blog/?p=116 #}
 
 {% block extrastyle %}
 	{{ block.super }}
     <link rel="stylesheet" type="text/css" href="{% static "admin/css/forms.css" %}"/>
 {% endblock %}
@@ -19,15 +19,15 @@
         &rsaquo; {% trans 'Upload' %}
     </div>
 {% endblock %}
 
 {% block content_title %}{% endblock %}
 
 {% block content %}
-	
+
 	<h1>{% trans "Upload a zip archive of photos" %}</h1>
 	{% blocktrans %}
 		<p>On this page you can upload many photos at once, as long as you have
 		put them all in a zip archive. The photos can be either:</p>
 		<ul>
 			<li>Added to an existing gallery.</li>
 			<li>Otherwise, a new gallery is created with the supplied title.</li>
@@ -50,8 +50,8 @@
             {% endfor %}
         </div>
         <div class="submit-row">
             <input type="submit" value="{% trans 'Upload' %}" class="default"/>
         </div>
     </form>
 
-{% endblock %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{% extends "admin/base_site.html" %} {% load i18n admin_urls admin_static %} {#
-Admin styling code largely taken from http://www.dmertl.com/blog/?p=116 #} {%
-block extrastyle %} {{ block.super }}
+{% extends "admin/base_site.html" %} {% load i18n admin_urls static %} {# Admin
+styling code largely taken from http://www.dmertl.com/blog/?p=116 #} {% block
+extrastyle %} {{ block.super }}
 ss/forms.css" %}"/> {% endblock %} {% block bodyclass %}{{ opts.app_label }}-{
 { opts.object_name.lower }} change-form{% endblock %} {% block breadcrumbs %}
 {%_trans_'Home'_%} › {{_app_label|capfirst|escape_}} › {% if
 has_change_permission %}{{_opts.verbose_name_plural|capfirst_}}{% else %}{
 { opts.verbose_name_plural|capfirst }}{% endif %} › {% trans 'Upload' %}
 {% endblock %} {% block content_title %}{% endblock %} {% block content %}
 ****** {% trans "Upload a zip archive of photos" %} ******
```

### Comparing `django-photologue-3.8.1/photologue/templatetags/photologue_tags.py` & `django-photologue-3.9/photologue/templatetags/photologue_tags.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/models.py` & `django-photologue-3.9/photologue/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-import os
-import random
-from datetime import datetime
-from inspect import isclass
 import logging
-from io import BytesIO
+import unicodedata
 from importlib import import_module
+from inspect import isclass
+
 import exifread
-import unicodedata
+import os
+import random
 from PIL import Image, ImageFile, ImageFilter, ImageEnhance
-
-from django.utils.timezone import now
-from django.db import models
-from django.db.models.signals import post_save
+from datetime import datetime
 from django.conf import settings
+from django.contrib.sites.models import Site
+from django.core.exceptions import ValidationError
 from django.core.files.base import ContentFile
 from django.core.files.storage import default_storage
-from django.urls import reverse
-from django.core.exceptions import ValidationError
+from django.core.validators import RegexValidator
+from django.db import models
+from django.db.models.signals import post_save
 from django.template.defaultfilters import slugify
+from django.urls import reverse
 from django.utils.encoding import force_text, smart_str, filepath_to_uri
+from django.utils.encoding import python_2_unicode_compatible
 from django.utils.functional import curry
 from django.utils.safestring import mark_safe
+from django.utils.timezone import now
 from django.utils.translation import ugettext_lazy as _
-from django.utils.encoding import python_2_unicode_compatible
-from django.core.validators import RegexValidator
-from django.contrib.sites.models import Site
-
+from io import BytesIO
 from sortedm2m.fields import SortedManyToManyField
 
+from .managers import GalleryQuerySet, PhotoQuerySet
 from .utils.reflection import add_reflection
 from .utils.watermark import apply_watermark
-from .managers import GalleryQuerySet, PhotoQuerySet
 
 logger = logging.getLogger('photologue.models')
 
 # Default limit for gallery.latest
 LATEST_LIMIT = getattr(settings, 'PHOTOLOGUE_GALLERY_LATEST_LIMIT', None)
 
 # Number of random images from the gallery to display.
@@ -139,15 +138,14 @@
                             '. Image filters will be applied in order. The following filters are available: %s.'
                             % (', '.join(filter_names)))
 
 size_method_map = {}
 
 
 class TagField(models.CharField):
-
     """Tags have been removed from Photologue, but the migrations still refer to them so this
     Tagfield definition is left here.
     """
 
     def __init__(self, **kwargs):
         default_kwargs = {'max_length': 255, 'blank': True}
         default_kwargs.update(kwargs)
@@ -220,27 +218,28 @@
 
     def photo_count(self, public=True):
         """Return a count of all the photos in this gallery."""
         if public:
             return self.public().count()
         else:
             return self.photos.filter(sites__id=settings.SITE_ID).count()
+
     photo_count.short_description = _('count')
 
     def public(self):
         """Return a queryset of all the public photos in this gallery."""
         return self.photos.is_public().filter(sites__id=settings.SITE_ID)
 
     def orphaned_photos(self):
         """
         Return all photos that belong to this gallery but don't share the
         gallery's site.
         """
-        return self.photos.filter(is_public=True)\
-                          .exclude(sites__id__in=self.sites.all())
+        return self.photos.filter(is_public=True) \
+            .exclude(sites__id__in=self.sites.all())
 
 
 class ImageModel(models.Model):
     image = models.ImageField(_('image'),
                               max_length=IMAGE_FIELD_MAX_LENGTH,
                               upload_to=get_storage_path)
     date_taken = models.DateTimeField(_('date taken'),
@@ -281,14 +280,15 @@
         if func is None:
             return _('An "admin_thumbnail" photo size has not been defined.')
         else:
             if hasattr(self, 'get_absolute_url'):
                 return mark_safe(u'<a href="{}"><img src="{}"></a>'.format(self.get_absolute_url(), func()))
             else:
                 return mark_safe(u'<a href="{}"><img src="{}"></a>'.format(self.image.url, func()))
+
     admin_thumbnail.short_description = _('Thumbnail')
     admin_thumbnail.allow_tags = True
 
     def cache_path(self):
         return os.path.join(os.path.dirname(self.image.name), "cache")
 
     def cache_url(self):
@@ -305,16 +305,19 @@
     def _get_SIZE_photosize(self, size):
         return PhotoSizeCache().sizes.get(size)
 
     def _get_SIZE_size(self, size):
         photosize = PhotoSizeCache().sizes.get(size)
         if not self.size_exists(photosize):
             self.create_size(photosize)
-        return Image.open(self.image.storage.open(
-            self._get_SIZE_filename(size))).size
+        try:
+            return Image.open(self.image.storage.open(
+                self._get_SIZE_filename(size))).size
+        except:
+            return None
 
     def _get_SIZE_url(self, size):
         photosize = PhotoSizeCache().sizes.get(size)
         if not self.size_exists(photosize):
             self.create_size(photosize)
         if photosize.increment_count:
             self.increment_count()
@@ -382,15 +385,15 @@
                 if new_width == 0:
                     ratio = float(new_height) / cur_height
                 else:
                     ratio = float(new_width) / cur_width
             new_dimensions = (int(round(cur_width * ratio)),
                               int(round(cur_height * ratio)))
             if new_dimensions[0] > cur_width or \
-               new_dimensions[1] > cur_height:
+                    new_dimensions[1] > cur_height:
                 if not photosize.upscale:
                     return im
             im = im.resize(new_dimensions, Image.ANTIALIAS)
         return im
 
     def create_size(self, photosize):
         if self.size_exists(photosize):
@@ -422,14 +425,17 @@
             im = self.effect.post_process(im)
         elif photosize.effect is not None:
             im = photosize.effect.post_process(im)
         # Save file
         im_filename = getattr(self, "get_%s_filename" % photosize.name)()
         try:
             buffer = BytesIO()
+            # Issue #182 - test fix from https://github.com/bashu/django-watermark/issues/31
+            if im.mode.endswith('A'):
+                im = im.convert(im.mode[:-1])
             if im_format != 'JPEG':
                 im.save(buffer, im_format)
             else:
                 im.save(buffer, 'JPEG', quality=int(photosize.quality),
                         optimize=True)
             buffer_contents = ContentFile(buffer.getvalue())
             self.image.storage.save(im_filename, buffer_contents)
@@ -601,20 +607,24 @@
         try:
             im = Image.open(SAMPLE_IMAGE_PATH)
         except IOError:
             raise IOError(
                 'Photologue was unable to open the sample image: %s.' % SAMPLE_IMAGE_PATH)
         im = self.process(im)
         buffer = BytesIO()
+        # Issue #182 - test fix from https://github.com/bashu/django-watermark/issues/31
+        if im.mode.endswith('A'):
+            im = im.convert(im.mode[:-1])
         im.save(buffer, 'JPEG', quality=90, optimize=True)
         buffer_contents = ContentFile(buffer.getvalue())
         default_storage.save(self.sample_filename(), buffer_contents)
 
     def admin_sample(self):
         return u'<img src="%s">' % self.sample_url()
+
     admin_sample.short_description = 'Sample'
     admin_sample.allow_tags = True
 
     def pre_process(self, im):
         return im
 
     def post_process(self, im):
@@ -648,15 +658,14 @@
             default_storage.delete(self.sample_filename())
         except:
             pass
         models.Model.delete(self)
 
 
 class PhotoEffect(BaseEffect):
-
     """ A pre-defined effect to apply to photos """
     transpose_method = models.CharField(_('rotate or flip'),
                                         max_length=15,
                                         blank=True,
                                         choices=IMAGE_TRANSPOSE_CHOICES)
     color = models.FloatField(_('color'),
                               default=1.0,
@@ -735,49 +744,48 @@
 
     class Meta:
         verbose_name = _('watermark')
         verbose_name_plural = _('watermarks')
 
     def delete(self):
         assert self._get_pk_val() is not None, "%s object can't be deleted because its %s attribute is set to None." \
-            % (self._meta.object_name, self._meta.pk.attname)
+                                               % (self._meta.object_name, self._meta.pk.attname)
         super(Watermark, self).delete()
         self.image.storage.delete(self.image.name)
 
     def post_process(self, im):
         mark = Image.open(self.image.storage.open(self.image.name))
         return apply_watermark(im, mark, self.style, self.opacity)
 
 
 @python_2_unicode_compatible
 class PhotoSize(models.Model):
-
     """About the Photosize name: it's used to create get_PHOTOSIZE_url() methods,
     so the name has to follow the same restrictions as any Python method name,
     e.g. no spaces or non-ascii characters."""
 
     name = models.CharField(_('name'),
                             max_length=40,
                             unique=True,
                             help_text=_(
                                 'Photo size name should contain only letters, numbers and underscores. Examples: '
                                 '"thumbnail", "display", "small", "main_page_widget".'),
                             validators=[RegexValidator(regex='^[a-z0-9_]+$',
                                                        message='Use only plain lowercase letters (ASCII), numbers and '
-                                                       'underscores.'
+                                                               'underscores.'
                                                        )]
                             )
     width = models.PositiveIntegerField(_('width'),
                                         default=0,
                                         help_text=_(
                                             'If width is set to "0" the image will be scaled to the supplied height.'))
     height = models.PositiveIntegerField(_('height'),
                                          default=0,
                                          help_text=_(
-        'If height is set to "0" the image will be scaled to the supplied width'))
+                                             'If height is set to "0" the image will be scaled to the supplied width'))
     quality = models.PositiveIntegerField(_('quality'),
                                           choices=JPEG_QUALITY_CHOICES,
                                           default=70,
                                           help_text=_('JPEG image quality.'))
     upscale = models.BooleanField(_('upscale images?'),
                                   default=False,
                                   help_text=_('If selected the image will be scaled up if necessary to fit the '
@@ -833,23 +841,24 @@
     def save(self, *args, **kwargs):
         super(PhotoSize, self).save(*args, **kwargs)
         PhotoSizeCache().reset()
         self.clear_cache()
 
     def delete(self):
         assert self._get_pk_val() is not None, "%s object can't be deleted because its %s attribute is set to None." \
-            % (self._meta.object_name, self._meta.pk.attname)
+                                               % (self._meta.object_name, self._meta.pk.attname)
         self.clear_cache()
         super(PhotoSize, self).delete()
 
     def _get_size(self):
         return (self.width, self.height)
 
     def _set_size(self, value):
         self.width, self.height = value
+
     size = property(_get_size, _set_size)
 
 
 class PhotoSizeCache(object):
     __state = {"sizes": {}}
 
     def __init__(self):
@@ -888,9 +897,11 @@
     if not created:
         return
     if getattr(settings, 'PHOTOLOGUE_MULTISITE', False):
         return
     if instance.sites.exists():
         return
     instance.sites.add(Site.objects.get_current())
+
+
 post_save.connect(add_default_site, sender=Gallery)
 post_save.connect(add_default_site, sender=Photo)
```

### Comparing `django-photologue-3.8.1/photologue/forms.py` & `django-photologue-3.9/photologue/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 except ImportError:
     # Python 2.
     from zipfile import BadZipfile as BadZipFile
 import logging
 import os
 from io import BytesIO
 
-try:
-    import Image
-except ImportError:
-    from PIL import Image
+from PIL import Image
 
 
 from django import forms
 from django.utils.translation import ugettext_lazy as _
 from django.contrib import messages
 from django.contrib.sites.models import Site
 from django.conf import settings
@@ -149,15 +146,15 @@
 
             # Basic check that we have a valid image.
             try:
                 file = BytesIO(data)
                 opened = Image.open(file)
                 opened.verify()
             except Exception:
-                # Pillow (or PIL) doesn't recognize it as an image.
+                # Pillow doesn't recognize it as an image.
                 # If a "bad" file is found we just skip it.
                 # But we do flag this both in the logs and to the user.
                 logger.error('Could not process file "{0}" in the .zip archive.'.format(
                     filename))
                 if request:
                     messages.warning(request,
                                      _('Could not process file "{0}" in the .zip archive.').format(
```

### Comparing `django-photologue-3.8.1/photologue/management/commands/plflush.py` & `django-photologue-3.9/photologue/management/commands/plflush.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/management/commands/plcreatesize.py` & `django-photologue-3.9/photologue/management/commands/plcreatesize.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/management/commands/plcache.py` & `django-photologue-3.9/photologue/management/commands/plcache.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/management/commands/__init__.py` & `django-photologue-3.9/photologue/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/migrations/0004_auto_20140915_1259.py` & `django-photologue-3.9/photologue/migrations/0004_auto_20140915_1259.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/migrations/0007_auto_20150404_1737.py` & `django-photologue-3.9/photologue/migrations/0007_auto_20150404_1737.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/migrations/0002_photosize_data.py` & `django-photologue-3.9/photologue/migrations/0002_photosize_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,13 +31,13 @@
                              increment_count=True)
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('photologue', '0001_initial'),
-        ('contenttypes', '0001_initial'),
+        ('contenttypes', '0002_remove_content_type_name'),
     ]
 
     operations = [
         migrations.RunPython(initial_photosizes),
     ]
```

### Comparing `django-photologue-3.8.1/photologue/migrations/0009_auto_20160102_0904.py` & `django-photologue-3.9/photologue/migrations/0009_auto_20160102_0904.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/migrations/0001_initial.py` & `django-photologue-3.9/photologue/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/migrations/0010_auto_20160105_1307.py` & `django-photologue-3.9/photologue/migrations/0010_auto_20160105_1307.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/migrations/0003_auto_20140822_1716.py` & `django-photologue-3.9/photologue/migrations/0003_auto_20140822_1716.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/urls.py` & `django-photologue-3.9/photologue/urls.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from django.conf.urls import url
 from django.views.generic import RedirectView
 from django.urls import reverse_lazy
 
 from .views import PhotoListView, PhotoDetailView, GalleryListView, \
     GalleryDetailView, PhotoArchiveIndexView, PhotoDateDetailView, PhotoDayArchiveView, \
     PhotoYearArchiveView, PhotoMonthArchiveView, GalleryArchiveIndexView, GalleryYearArchiveView, \
-    GalleryDateDetailView, GalleryDayArchiveView, GalleryMonthArchiveView, GalleryDateDetailOldView, \
-    GalleryDayArchiveOldView, GalleryMonthArchiveOldView, PhotoDateDetailOldView, \
-    PhotoDayArchiveOldView, PhotoMonthArchiveOldView
+    GalleryDateDetailView, GalleryDayArchiveView, GalleryMonthArchiveView
 
 """NOTE: the url names are changing. In the long term, I want to remove the 'pl-'
 prefix on all urls, and instead rely on an application namespace 'photologue'.
 
 At the same time, I want to change some URL patterns, e.g. for pagination. Changing the urls
 twice within a few releases, could be confusing, so instead I am updating URLs bit by bit.
 
@@ -65,28 +63,8 @@
 
     url(r'^photo/(?P<slug>[\-\d\w]+)/$',
         PhotoDetailView.as_view(),
         name='pl-photo'),
     url(r'^photolist/$',
         PhotoListView.as_view(),
         name='photo-list'),
-
-    # Deprecated URLs.
-    url(r'^gallery/(?P<year>\d{4})/(?P<month>[a-z]{3})/(?P<day>\w{1,2})/(?P<slug>[\-\d\w]+)/$',
-        GalleryDateDetailOldView.as_view(),
-        name='pl-gallery-detail'),
-    url(r'^gallery/(?P<year>\d{4})/(?P<month>[a-z]{3})/(?P<day>\w{1,2})/$',
-        GalleryDayArchiveOldView.as_view(),
-        name='pl-gallery-archive-day'),
-    url(r'^gallery/(?P<year>\d{4})/(?P<month>[a-z]{3})/$',
-        GalleryMonthArchiveOldView.as_view(),
-        name='pl-gallery-archive-month'),
-    url(r'^photo/(?P<year>\d{4})/(?P<month>[a-z]{3})/(?P<day>\w{1,2})/(?P<slug>[\-\d\w]+)/$',
-        PhotoDateDetailOldView.as_view(),
-        name='pl-photo-detail'),
-    url(r'^photo/(?P<year>\d{4})/(?P<month>[a-z]{3})/(?P<day>\w{1,2})/$',
-        PhotoDayArchiveOldView.as_view(),
-        name='pl-photo-archive-day'),
-    url(r'^photo/(?P<year>\d{4})/(?P<month>[a-z]{3})/$',
-        PhotoMonthArchiveOldView.as_view(),
-        name='pl-photo-archive-month')
 ]
```

### Comparing `django-photologue-3.8.1/photologue/tests/test_resize.py` & `django-photologue-3.9/photologue/tests/test_resize.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/tests/test_views_photo.py` & `django-photologue-3.9/photologue/tests/test_views_photo.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/tests/test_gallery.py` & `django-photologue-3.9/photologue/tests/test_gallery.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/tests/test_views_gallery.py` & `django-photologue-3.9/photologue/tests/test_views_gallery.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/tests/test_photosize.py` & `django-photologue-3.9/photologue/tests/test_photosize.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/tests/test_sitemap.py` & `django-photologue-3.9/photologue/tests/test_sitemap.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/tests/test_photo.py` & `django-photologue-3.9/photologue/tests/test_photo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 
-import os
 import unittest
 
+import os
 from django import VERSION
 from django.conf import settings
-from django.core.files.storage import default_storage
 from django.core.files.base import ContentFile
-from ..models import Image, Photo, PHOTOLOGUE_DIR, PHOTOLOGUE_CACHEDIRTAG
+from django.core.files.storage import default_storage
+
 from .factories import LANDSCAPE_IMAGE_PATH, QUOTING_IMAGE_PATH, \
     UNICODE_IMAGE_PATH, NONSENSE_IMAGE_PATH, GalleryFactory, PhotoFactory
 from .helpers import PhotologueBaseTest
+from ..models import Image, Photo, PHOTOLOGUE_DIR, PHOTOLOGUE_CACHEDIRTAG
 
 
 class PhotoTest(PhotologueBaseTest):
 
     def tearDown(self):
         """Delete any extra test files (if created)."""
         super(PhotoTest, self).tearDown()
@@ -72,16 +73,15 @@
 
     def test_accessor_methods(self):
         self.assertEqual(self.pl.get_testPhotoSize_photosize(), self.s)
         self.assertEqual(self.pl.get_testPhotoSize_size(),
                          Image.open(self.pl.image.storage.open(
                              self.pl.get_testPhotoSize_filename())).size)
         self.assertEqual(self.pl.get_testPhotoSize_url(),
-                         self.pl.cache_url() + '/' +
-                         self.pl._get_filename_for_size(self.s))
+                         self.pl.cache_url() + '/' + self.pl._get_filename_for_size(self.s))
         self.assertEqual(self.pl.get_testPhotoSize_filename(),
                          os.path.join(self.pl.cache_path(),
                                       self.pl._get_filename_for_size(self.s)))
 
     def test_quoted_url(self):
         """Test for issue #29 - filenames of photos are incorrectly quoted when
         building a URL."""
@@ -102,15 +102,14 @@
         """Trivial check that unicode titles work.
         (I was trying to track down an elusive unicode issue elsewhere)"""
         self.pl2 = PhotoFactory(title='É',
                                 slug='é')
 
 
 class PhotoManagerTest(PhotologueBaseTest):
-
     """Some tests for the methods on the Photo manager class."""
 
     def setUp(self):
         """Create 2 photos."""
         super(PhotoManagerTest, self).setUp()
         self.pl2 = PhotoFactory()
 
@@ -123,15 +122,14 @@
         self.assertEqual(Photo.objects.is_public().count(), 2)
         self.pl.is_public = False
         self.pl.save()
         self.assertEqual(Photo.objects.is_public().count(), 1)
 
 
 class PreviousNextTest(PhotologueBaseTest):
-
     """Tests for the methods that provide the previous/next photos in a gallery."""
 
     def setUp(self):
         """Create a test gallery with 2 photos."""
         super(PreviousNextTest, self).setUp()
         self.test_gallery = GalleryFactory()
         self.pl1 = PhotoFactory()
@@ -218,21 +216,21 @@
 
 class ImageModelTest(PhotologueBaseTest):
 
     def setUp(self):
         super(ImageModelTest, self).setUp()
 
         # Unicode image has unicode in the path
-        #self.pu = TestPhoto(name='portrait')
+        # self.pu = TestPhoto(name='portrait')
         self.pu = PhotoFactory()
         self.pu.image.save(os.path.basename(UNICODE_IMAGE_PATH),
                            ContentFile(open(UNICODE_IMAGE_PATH, 'rb').read()))
 
         # Nonsense image contains nonsense
-        #self.pn = TestPhoto(name='portrait')
+        # self.pn = TestPhoto(name='portrait')
         self.pn = PhotoFactory()
         self.pn.image.save(os.path.basename(NONSENSE_IMAGE_PATH),
                            ContentFile(open(NONSENSE_IMAGE_PATH, 'rb').read()))
 
     def tearDown(self):
         super(ImageModelTest, self).tearDown()
         self.pu.delete()
```

### Comparing `django-photologue-3.8.1/photologue/tests/helpers.py` & `django-photologue-3.9/photologue/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/tests/test_sites.py` & `django-photologue-3.9/photologue/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/tests/test_zipupload.py` & `django-photologue-3.9/photologue/tests/test_zipupload.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/tests/factories.py` & `django-photologue-3.9/photologue/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/managers.py` & `django-photologue-3.9/photologue/managers.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/photologue/admin.py` & `django-photologue-3.9/photologue/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from django import forms
 from django.conf import settings
 from django.conf.urls import url
 from django.contrib import admin
-from django.contrib.sites.models import Site
 from django.contrib import messages
-from django.utils.translation import ungettext, ugettext_lazy as _
-from django.shortcuts import render
 from django.contrib.admin import helpers
+from django.contrib.sites.models import Site
 from django.http import HttpResponseRedirect
+from django.shortcuts import render
+from django.utils.translation import ungettext, ugettext_lazy as _
 
+from .forms import UploadZipForm
 from .models import Gallery, Photo, PhotoEffect, PhotoSize, \
     Watermark
-from .forms import UploadZipForm
 
 MULTISITE = getattr(settings, 'PHOTOLOGUE_MULTISITE', False)
 
 
 class GalleryAdminForm(forms.ModelForm):
-
     class Meta:
         model = Gallery
         if MULTISITE:
             exclude = []
         else:
             exclude = ['sites']
 
@@ -97,47 +96,41 @@
         photos = Photo.objects.filter(galleries__in=queryset)
         current_site = Site.objects.get_current()
         current_site.photo_set.add(*photos)
         msg = ungettext(
             'All photos in gallery %(galleries)s have been successfully added to %(site)s',
             'All photos in galleries %(galleries)s have been successfully added to %(site)s',
             len(queryset)
-        ) % {
-            'site': current_site.name,
-            'galleries': ", ".join(["'{0}'".format(gallery.title)
-                                    for gallery in queryset])
-        }
+        ) % {'site': current_site.name,
+             'galleries': ", ".join(["'{0}'".format(gallery.title) for gallery in queryset])}
         messages.success(request, msg)
 
     add_photos_to_current_site.short_description = \
         _("Add all photos of selected galleries to the current site")
 
     def remove_photos_from_current_site(modeladmin, request, queryset):
         photos = Photo.objects.filter(galleries__in=queryset)
         current_site = Site.objects.get_current()
         current_site.photo_set.remove(*photos)
         msg = ungettext(
             'All photos in gallery %(galleries)s have been successfully removed from %(site)s',
             'All photos in galleries %(galleries)s have been successfully removed from %(site)s',
             len(queryset)
-        ) % {
-            'site': current_site.name,
-            'galleries': ", ".join(["'{0}'".format(gallery.title)
-                                    for gallery in queryset])
-        }
+        ) % {'site': current_site.name,
+             'galleries': ", ".join(["'{0}'".format(gallery.title) for gallery in queryset])}
         messages.success(request, msg)
 
     remove_photos_from_current_site.short_description = \
         _("Remove all photos in selected galleries from the current site")
 
+
 admin.site.register(Gallery, GalleryAdmin)
 
 
 class PhotoAdminForm(forms.ModelForm):
-
     class Meta:
         model = Photo
         if MULTISITE:
             exclude = []
         else:
             exclude = ['sites']
 
@@ -243,14 +236,15 @@
             'fields': ('reflection_size', 'reflection_strength', 'background_color')
         }),
         ('Transpose', {
             'fields': ('transpose_method',)
         }),
     )
 
+
 admin.site.register(PhotoEffect, PhotoEffectAdmin)
 
 
 class PhotoSizeAdmin(admin.ModelAdmin):
     list_display = ('name', 'width', 'height', 'crop', 'pre_cache', 'effect', 'increment_count')
     fieldsets = (
         (None, {
@@ -260,14 +254,15 @@
             'fields': ('upscale', 'crop', 'pre_cache', 'increment_count')
         }),
         ('Enhancements', {
             'fields': ('effect', 'watermark',)
         }),
     )
 
+
 admin.site.register(PhotoSize, PhotoSizeAdmin)
 
 
 class WatermarkAdmin(admin.ModelAdmin):
     list_display = ('name', 'opacity', 'style')
```

### Comparing `django-photologue-3.8.1/photologue/sitemaps.py` & `django-photologue-3.9/photologue/sitemaps.py`

 * *Files identical despite different names*

### Comparing `django-photologue-3.8.1/setup.py` & `django-photologue-3.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-#/usr/bin/env python
+# /usr/bin/env python
 import uuid
-import os
 from setuptools import setup, find_packages
-from pip.req import parse_requirements
 
+try:  # for pip >= 10
+    from pip._internal.req import parse_requirements
+except ImportError:  # for pip <= 9.0.3
+    from pip.req import parse_requirements
 import photologue
 
 
 def get_requirements(source):
-
     try:
         install_reqs = parse_requirements(source, session=uuid.uuid1())
     except TypeError:
         # Older version of pip.
         install_reqs = parse_requirements(source)
-    required = list(set([str(ir.req) for ir in install_reqs]))
+    required = sorted(set([str(ir.req) for ir in install_reqs]))
 
-    # Temp situation: transition from PIL to Pillow, add a hook so people can
-    # skip installing Pillow.
-    if os.path.exists('/tmp/PHOTOLOGUE_NO_PILLOW'):
-        required = [item for item in required if not item.startswith('Pillow')]
     return required
 
+
 setup(
     name="django-photologue",
     version=photologue.__version__,
     description="Powerful image management for the Django web framework.",
     author="Justin Driscoll, Marcos Daniel Petry, Richard Barran",
     author_email="justin@driscolldev.com, marcospetry@gmail.com, richard@arbee-design.co.uk",
-    url="https://github.com/jdriscoll/django-photologue",
+    url="https://github.com/richardbarran/django-photologue",
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     classifiers=['Development Status :: 5 - Production/Stable',
                  'Environment :: Web Environment',
                  'Framework :: Django',
                  'Intended Audience :: Developers',
                  'License :: OSI Approved :: BSD License',
                  'Operating System :: OS Independent',
                  'Programming Language :: Python',
                  'Programming Language :: Python :: 2.7',
                  'Programming Language :: Python :: 3',
                  'Programming Language :: Python :: 3.4',
                  'Programming Language :: Python :: 3.5',
+                 'Programming Language :: Python :: 3.6',
                  'Topic :: Utilities'],
     install_requires=get_requirements('requirements.txt'),
 )
```

