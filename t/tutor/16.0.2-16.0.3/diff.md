# Comparing `tmp/tutor-16.0.2.tar.gz` & `tmp/tutor-16.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-16.0.2.tar", last modified: Thu Jun 22 11:16:18 2023, max compression
+gzip compressed data, was "tutor-16.0.3.tar", last modified: Fri Jul 28 20:07:15 2023, max compression
```

## Comparing `tutor-16.0.2.tar` & `tutor-16.0.3.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.793367 tutor-16.0.2/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-22 11:15:38.000000 tutor-16.0.2/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)      121 2023-06-22 11:15:38.000000 tutor-16.0.2/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     6665 2023-06-22 11:16:18.793367 tutor-16.0.2/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     4745 2023-06-22 11:15:38.000000 tutor-16.0.2/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-22 11:15:38.000000 tutor-16.0.2/pyproject.toml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.760034 tutor-16.0.2/requirements/
--rw-r--r--   0 ci        (1000) ci        (1000)       98 2023-06-22 11:15:38.000000 tutor-16.0.2/requirements/base.in
--rw-r--r--   0 ci        (1000) ci        (1000)      340 2023-06-22 11:15:38.000000 tutor-16.0.2/requirements/plugins.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-22 11:16:18.793367 tutor-16.0.2/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     2506 2023-06-22 11:15:38.000000 tutor-16.0.2/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.766701 tutor-16.0.2/tests/
--rw-r--r--   0 ci        (1000) ci        (1000)     2491 2023-06-22 11:15:38.000000 tutor-16.0.2/tests/test_bindmount.py
--rw-r--r--   0 ci        (1000) ci        (1000)     4172 2023-06-22 11:15:38.000000 tutor-16.0.2/tests/test_config.py
--rw-r--r--   0 ci        (1000) ci        (1000)    15898 2023-06-22 11:15:38.000000 tutor-16.0.2/tests/test_env.py
--rw-r--r--   0 ci        (1000) ci        (1000)     3063 2023-06-22 11:15:38.000000 tutor-16.0.2/tests/test_plugin_indexes.py
--rw-r--r--   0 ci        (1000) ci        (1000)     8279 2023-06-22 11:15:38.000000 tutor-16.0.2/tests/test_plugins_v0.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2432 2023-06-22 11:15:38.000000 tutor-16.0.2/tests/test_serialize.py
--rw-r--r--   0 ci        (1000) ci        (1000)    10669 2023-06-22 11:15:38.000000 tutor-16.0.2/tests/test_utils.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.770034 tutor-16.0.2/tutor/
--rw-r--r--   0 ci        (1000) ci        (1000)     1159 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2546 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/bindmount.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.773368 tutor-16.0.2/tutor/commands/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/__init__.py
--rwxr-xr-x   0 ci        (1000) ci        (1000)     4485 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/cli.py
--rw-r--r--   0 ci        (1000) ci        (1000)    16737 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/compose.py
--rw-r--r--   0 ci        (1000) ci        (1000)     7317 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/config.py
--rw-r--r--   0 ci        (1000) ci        (1000)      794 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/context.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2240 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/dev.py
--rw-r--r--   0 ci        (1000) ci        (1000)    11658 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/images.py
--rw-r--r--   0 ci        (1000) ci        (1000)    10722 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/jobs.py
--rw-r--r--   0 ci        (1000) ci        (1000)    21075 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/k8s.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1772 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/local.py
--rw-r--r--   0 ci        (1000) ci        (1000)     4446 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/mounts.py
--rw-r--r--   0 ci        (1000) ci        (1000)      741 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/params.py
--rw-r--r--   0 ci        (1000) ci        (1000)    13436 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/plugins.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.773368 tutor-16.0.2/tutor/commands/upgrade/
--rw-r--r--   0 ci        (1000) ci        (1000)      185 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/upgrade/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2082 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/upgrade/common.py
--rw-r--r--   0 ci        (1000) ci        (1000)     6047 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/upgrade/compose.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5685 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/commands/upgrade/k8s.py
--rw-r--r--   0 ci        (1000) ci        (1000)     9685 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.773368 tutor-16.0.2/tutor/core/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/core/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.776701 tutor-16.0.2/tutor/core/hooks/
--rw-r--r--   0 ci        (1000) ci        (1000)      292 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/core/hooks/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5707 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/core/hooks/actions.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2929 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/core/hooks/contexts.py
--rw-r--r--   0 ci        (1000) ci        (1000)     9006 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/core/hooks/filters.py
--rw-r--r--   0 ci        (1000) ci        (1000)      638 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/core/hooks/priorities.py
--rw-r--r--   0 ci        (1000) ci        (1000)    17753 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/env.py
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/exceptions.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1213 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/fmt.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.776701 tutor-16.0.2/tutor/hooks/
--rw-r--r--   0 ci        (1000) ci        (1000)      273 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/hooks/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)    24524 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/hooks/catalog.py
--rw-r--r--   0 ci        (1000) ci        (1000)      571 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/images.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5076 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/interactive.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.776701 tutor-16.0.2/tutor/plugins/
--rw-r--r--   0 ci        (1000) ci        (1000)     3802 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/plugins/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      548 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/plugins/base.py
--rw-r--r--   0 ci        (1000) ci        (1000)     6989 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/plugins/indexes.py
--rw-r--r--   0 ci        (1000) ci        (1000)    15218 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/plugins/v0.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2376 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/plugins/v1.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/py.typed
--rw-r--r--   0 ci        (1000) ci        (1000)     1947 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/serialize.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1385 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/tasks.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.776701 tutor-16.0.2/tutor/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.753367 tutor-16.0.2/tutor/templates/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.776701 tutor-16.0.2/tutor/templates/apps/caddy/
--rw-r--r--   0 ci        (1000) ci        (1000)     1989 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/caddy/Caddyfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.776701 tutor-16.0.2/tutor/templates/apps/openedx/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.780034 tutor-16.0.2/tutor/templates/apps/openedx/config/
--rw-r--r--   0 ci        (1000) ci        (1000)     1542 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/config/cms.env.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1787 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/config/lms.env.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.780034 tutor-16.0.2/tutor/templates/apps/openedx/config/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)      673 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/config/partials/auth.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.753367 tutor-16.0.2/tutor/templates/apps/openedx/settings/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.780034 tutor-16.0.2/tutor/templates/apps/openedx/settings/cms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/settings/cms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      591 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/settings/cms/development.py
--rw-r--r--   0 ci        (1000) ci        (1000)      529 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/settings/cms/production.py
--rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/settings/cms/test.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.780034 tutor-16.0.2/tutor/templates/apps/openedx/settings/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/settings/lms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1132 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/settings/lms/development.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1039 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/settings/lms/production.py
--rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/settings/lms/test.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.780034 tutor-16.0.2/tutor/templates/apps/openedx/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)    10001 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/settings/partials/common_all.py
--rw-r--r--   0 ci        (1000) ci        (1000)      924 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/settings/partials/common_cms.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1450 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/settings/partials/common_lms.py
--rw-r--r--   0 ci        (1000) ci        (1000)      105 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/settings/partials/common_test.py
--rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/openedx/uwsgi.ini
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.783367 tutor-16.0.2/tutor/templates/apps/permissions/
--rw-r--r--   0 ci        (1000) ci        (1000)      380 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/permissions/setowners.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.783367 tutor-16.0.2/tutor/templates/apps/redis/
--rw-r--r--   0 ci        (1000) ci        (1000)      854 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/apps/redis/redis.conf
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.756701 tutor-16.0.2/tutor/templates/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.783367 tutor-16.0.2/tutor/templates/build/openedx/
--rw-r--r--   0 ci        (1000) ci        (1000)    12605 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.783367 tutor-16.0.2/tutor/templates/build/openedx/bin/
--rwxr-xr-x   0 ci        (1000) ci        (1000)     7042 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/bin/openedx-assets
--rwxr-xr-x   0 ci        (1000) ci        (1000)      116 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/bin/reload-uwsgi
--rw-r--r--   0 ci        (1000) ci        (1000)     2329 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/bin/site-configuration
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.783367 tutor-16.0.2/tutor/templates/build/openedx/locale/
--rw-r--r--   0 ci        (1000) ci        (1000)      438 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/locale/customlocales.md
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.783367 tutor-16.0.2/tutor/templates/build/openedx/requirements/
--rw-r--r--   0 ci        (1000) ci        (1000)      305 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/requirements/private-sample.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/revisions.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.783367 tutor-16.0.2/tutor/templates/build/openedx/settings/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.783367 tutor-16.0.2/tutor/templates/build/openedx/settings/cms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/settings/cms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      317 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/settings/cms/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/settings/cms/i18n.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.786701 tutor-16.0.2/tutor/templates/build/openedx/settings/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/settings/lms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      306 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/settings/lms/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/settings/lms/i18n.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.786701 tutor-16.0.2/tutor/templates/build/openedx/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)      441 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/settings/partials/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)      420 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/settings/partials/i18n.py
--rw-r--r--   0 ci        (1000) ci        (1000)      262 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/settings/uwsgi.ini
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.786701 tutor-16.0.2/tutor/templates/build/openedx/themes/
--rw-r--r--   0 ci        (1000) ci        (1000)       75 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/openedx/themes/README
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.786701 tutor-16.0.2/tutor/templates/build/permissions/
--rw-r--r--   0 ci        (1000) ci        (1000)      189 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/permissions/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      302 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/build/permissions/setowner.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.786701 tutor-16.0.2/tutor/templates/config/
--rw-r--r--   0 ci        (1000) ci        (1000)      515 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/config/base.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2610 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/config/defaults.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.786701 tutor-16.0.2/tutor/templates/dev/
--rw-r--r--   0 ci        (1000) ci        (1000)      885 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/dev/docker-compose.jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1395 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/dev/docker-compose.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.756701 tutor-16.0.2/tutor/templates/jobs/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.790034 tutor-16.0.2/tutor/templates/jobs/init/
--rw-r--r--   0 ci        (1000) ci        (1000)      418 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/jobs/init/cms.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1807 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/jobs/init/lms.sh
--rw-r--r--   0 ci        (1000) ci        (1000)      756 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/jobs/init/mounted-edx-platform.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1455 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/jobs/init/mysql.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.790034 tutor-16.0.2/tutor/templates/k8s/
--rw-r--r--   0 ci        (1000) ci        (1000)    12952 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/k8s/deployments.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2090 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/k8s/jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)      125 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/k8s/namespace.yml
--rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/k8s/override.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2358 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/k8s/services.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1428 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/k8s/volumes.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2142 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/kustomization.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.793367 tutor-16.0.2/tutor/templates/local/
--rw-r--r--   0 ci        (1000) ci        (1000)     2185 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/local/docker-compose.jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)      950 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/local/docker-compose.prod.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     6496 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/local/docker-compose.yml
--rw-r--r--   0 ci        (1000) ci        (1000)       19 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/templates/version
--rw-r--r--   0 ci        (1000) ci        (1000)     1327 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/types.py
--rw-r--r--   0 ci        (1000) ci        (1000)    10935 2023-06-22 11:15:38.000000 tutor-16.0.2/tutor/utils.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-22 11:16:18.770034 tutor-16.0.2/tutor.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     6665 2023-06-22 11:16:18.000000 tutor-16.0.2/tutor.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     4098 2023-06-22 11:16:18.000000 tutor-16.0.2/tutor.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-22 11:16:18.000000 tutor-16.0.2/tutor.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-06-22 11:16:18.000000 tutor-16.0.2/tutor.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)      397 2023-06-22 11:16:18.000000 tutor-16.0.2/tutor.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        6 2023-06-22 11:16:18.000000 tutor-16.0.2/tutor.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.232971 tutor-16.0.3/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-07-28 20:06:28.000000 tutor-16.0.3/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)      121 2023-07-28 20:06:28.000000 tutor-16.0.3/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     6665 2023-07-28 20:07:15.232971 tutor-16.0.3/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     4745 2023-07-28 20:06:28.000000 tutor-16.0.3/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-07-28 20:06:28.000000 tutor-16.0.3/pyproject.toml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.192971 tutor-16.0.3/requirements/
+-rw-r--r--   0 ci        (1000) ci        (1000)       98 2023-07-28 20:06:28.000000 tutor-16.0.3/requirements/base.in
+-rw-r--r--   0 ci        (1000) ci        (1000)      340 2023-07-28 20:06:28.000000 tutor-16.0.3/requirements/plugins.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-07-28 20:07:15.232971 tutor-16.0.3/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     2506 2023-07-28 20:06:28.000000 tutor-16.0.3/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.199637 tutor-16.0.3/tests/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2491 2023-07-28 20:06:28.000000 tutor-16.0.3/tests/test_bindmount.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     4172 2023-07-28 20:06:28.000000 tutor-16.0.3/tests/test_config.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15898 2023-07-28 20:06:28.000000 tutor-16.0.3/tests/test_env.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     3063 2023-07-28 20:06:28.000000 tutor-16.0.3/tests/test_plugin_indexes.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     8279 2023-07-28 20:06:28.000000 tutor-16.0.3/tests/test_plugins_v0.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2432 2023-07-28 20:06:28.000000 tutor-16.0.3/tests/test_serialize.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    10669 2023-07-28 20:06:28.000000 tutor-16.0.3/tests/test_utils.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.202971 tutor-16.0.3/tutor/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1159 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2546 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/bindmount.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.209637 tutor-16.0.3/tutor/commands/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/__init__.py
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     4485 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/cli.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    16737 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/compose.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     7317 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/config.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      794 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/context.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2240 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/dev.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    11658 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/images.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    10752 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/jobs.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    21075 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/k8s.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1772 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/local.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     4446 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/mounts.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      741 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/params.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    13436 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/plugins.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.212971 tutor-16.0.3/tutor/commands/upgrade/
+-rw-r--r--   0 ci        (1000) ci        (1000)      185 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/upgrade/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2082 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/upgrade/common.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     6047 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/upgrade/compose.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5685 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/commands/upgrade/k8s.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     9685 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.212971 tutor-16.0.3/tutor/core/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/core/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.216304 tutor-16.0.3/tutor/core/hooks/
+-rw-r--r--   0 ci        (1000) ci        (1000)      292 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/core/hooks/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5707 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/core/hooks/actions.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2929 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/core/hooks/contexts.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     9006 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/core/hooks/filters.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      638 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/core/hooks/priorities.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    17753 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/env.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/exceptions.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1213 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/fmt.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.216304 tutor-16.0.3/tutor/hooks/
+-rw-r--r--   0 ci        (1000) ci        (1000)      273 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/hooks/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    24524 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/hooks/catalog.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      571 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/images.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5076 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/interactive.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.219637 tutor-16.0.3/tutor/plugins/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3802 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/plugins/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      548 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/plugins/base.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     6989 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/plugins/indexes.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15218 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/plugins/v0.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2376 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/plugins/v1.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/py.typed
+-rw-r--r--   0 ci        (1000) ci        (1000)     1947 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/serialize.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1385 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/tasks.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.219637 tutor-16.0.3/tutor/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.189637 tutor-16.0.3/tutor/templates/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.219637 tutor-16.0.3/tutor/templates/apps/caddy/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1989 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/caddy/Caddyfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.219637 tutor-16.0.3/tutor/templates/apps/openedx/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.219637 tutor-16.0.3/tutor/templates/apps/openedx/config/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1542 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/config/cms.env.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1787 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/config/lms.env.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.219637 tutor-16.0.3/tutor/templates/apps/openedx/config/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)      673 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/config/partials/auth.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.189637 tutor-16.0.3/tutor/templates/apps/openedx/settings/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.219637 tutor-16.0.3/tutor/templates/apps/openedx/settings/cms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/settings/cms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      591 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/settings/cms/development.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      529 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/settings/cms/production.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/settings/cms/test.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.222971 tutor-16.0.3/tutor/templates/apps/openedx/settings/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/settings/lms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1132 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/settings/lms/development.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1039 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/settings/lms/production.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/settings/lms/test.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.222971 tutor-16.0.3/tutor/templates/apps/openedx/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)    10001 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/settings/partials/common_all.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      924 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/settings/partials/common_cms.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1450 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/settings/partials/common_lms.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      105 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/settings/partials/common_test.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/openedx/uwsgi.ini
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.222971 tutor-16.0.3/tutor/templates/apps/permissions/
+-rw-r--r--   0 ci        (1000) ci        (1000)      380 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/permissions/setowners.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.222971 tutor-16.0.3/tutor/templates/apps/redis/
+-rw-r--r--   0 ci        (1000) ci        (1000)      854 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/apps/redis/redis.conf
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.189637 tutor-16.0.3/tutor/templates/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.222971 tutor-16.0.3/tutor/templates/build/openedx/
+-rw-r--r--   0 ci        (1000) ci        (1000)    12877 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.226304 tutor-16.0.3/tutor/templates/build/openedx/bin/
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     7042 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/bin/openedx-assets
+-rwxr-xr-x   0 ci        (1000) ci        (1000)      116 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/bin/reload-uwsgi
+-rw-r--r--   0 ci        (1000) ci        (1000)     2329 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/bin/site-configuration
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.226304 tutor-16.0.3/tutor/templates/build/openedx/locale/
+-rw-r--r--   0 ci        (1000) ci        (1000)      438 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/locale/customlocales.md
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.226304 tutor-16.0.3/tutor/templates/build/openedx/requirements/
+-rw-r--r--   0 ci        (1000) ci        (1000)      305 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/requirements/private-sample.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/revisions.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.226304 tutor-16.0.3/tutor/templates/build/openedx/settings/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.226304 tutor-16.0.3/tutor/templates/build/openedx/settings/cms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/settings/cms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      317 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/settings/cms/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/settings/cms/i18n.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.226304 tutor-16.0.3/tutor/templates/build/openedx/settings/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/settings/lms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      306 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/settings/lms/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/settings/lms/i18n.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.226304 tutor-16.0.3/tutor/templates/build/openedx/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)      441 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/settings/partials/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      420 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/settings/partials/i18n.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      262 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/settings/uwsgi.ini
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.226304 tutor-16.0.3/tutor/templates/build/openedx/themes/
+-rw-r--r--   0 ci        (1000) ci        (1000)       75 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/openedx/themes/README
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.229637 tutor-16.0.3/tutor/templates/build/permissions/
+-rw-r--r--   0 ci        (1000) ci        (1000)      189 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/permissions/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      302 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/build/permissions/setowner.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.229637 tutor-16.0.3/tutor/templates/config/
+-rw-r--r--   0 ci        (1000) ci        (1000)      515 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/config/base.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2610 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/config/defaults.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.229637 tutor-16.0.3/tutor/templates/dev/
+-rw-r--r--   0 ci        (1000) ci        (1000)      885 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/dev/docker-compose.jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1395 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/dev/docker-compose.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.192971 tutor-16.0.3/tutor/templates/jobs/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.229637 tutor-16.0.3/tutor/templates/jobs/init/
+-rw-r--r--   0 ci        (1000) ci        (1000)      418 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/jobs/init/cms.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1807 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/jobs/init/lms.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)      756 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/jobs/init/mounted-edx-platform.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1455 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/jobs/init/mysql.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.232971 tutor-16.0.3/tutor/templates/k8s/
+-rw-r--r--   0 ci        (1000) ci        (1000)    12952 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/k8s/deployments.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2090 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/k8s/jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)      125 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/k8s/namespace.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/k8s/override.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2358 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/k8s/services.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1428 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/k8s/volumes.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2142 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/kustomization.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.232971 tutor-16.0.3/tutor/templates/local/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2185 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/local/docker-compose.jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)      950 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/local/docker-compose.prod.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     6496 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/local/docker-compose.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)       19 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/templates/version
+-rw-r--r--   0 ci        (1000) ci        (1000)     1327 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/types.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    10935 2023-07-28 20:06:28.000000 tutor-16.0.3/tutor/utils.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-28 20:07:15.206304 tutor-16.0.3/tutor.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6665 2023-07-28 20:07:15.000000 tutor-16.0.3/tutor.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     4098 2023-07-28 20:07:15.000000 tutor-16.0.3/tutor.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-07-28 20:07:15.000000 tutor-16.0.3/tutor.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-07-28 20:07:15.000000 tutor-16.0.3/tutor.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)      397 2023-07-28 20:07:15.000000 tutor-16.0.3/tutor.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        6 2023-07-28 20:07:15.000000 tutor-16.0.3/tutor.egg-info/top_level.txt
```

### Comparing `tutor-16.0.2/LICENSE.txt` & `tutor-16.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/PKG-INFO` & `tutor-16.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor
-Version: 16.0.2
+Version: 16.0.3
 Summary: The Docker-based Open edX distribution designed for peace of mind
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.io
 Author-email: contact@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor
```

### Comparing `tutor-16.0.2/README.rst` & `tutor-16.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/setup.py` & `tutor-16.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tests/test_bindmount.py` & `tutor-16.0.3/tests/test_bindmount.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tests/test_config.py` & `tutor-16.0.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tests/test_env.py` & `tutor-16.0.3/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tests/test_plugin_indexes.py` & `tutor-16.0.3/tests/test_plugin_indexes.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tests/test_plugins_v0.py` & `tutor-16.0.3/tests/test_plugins_v0.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tests/test_serialize.py` & `tutor-16.0.3/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tests/test_utils.py` & `tutor-16.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/__about__.py` & `tutor-16.0.3/tutor/__about__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 # Increment this version number to trigger a new release. See
 # docs/tutor.html#versioning for information on the versioning scheme.
-__version__ = "16.0.2"
+__version__ = "16.0.3"
 
 # The version suffix will be appended to the actual version, separated by a
 # dash. Use this suffix to differentiate between the actual released version and
 # the versions from other branches. For instance: set the suffix to "nightly" in
 # the nightly branch.
 # The suffix is cleanly separated from the __version__ in this module to avoid
 # conflicts when merging branches.
```

### Comparing `tutor-16.0.2/tutor/bindmount.py` & `tutor-16.0.3/tutor/bindmount.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/cli.py` & `tutor-16.0.3/tutor/commands/cli.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/compose.py` & `tutor-16.0.3/tutor/commands/compose.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/config.py` & `tutor-16.0.3/tutor/commands/config.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/context.py` & `tutor-16.0.3/tutor/commands/context.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/dev.py` & `tutor-16.0.3/tutor/commands/dev.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/images.py` & `tutor-16.0.3/tutor/commands/images.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/jobs.py` & `tutor-16.0.3/tutor/commands/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,16 @@
             )
     site, _ = Site.objects.get_or_create(domain=domain)
     if not site.name:
         name_max_length = Site._meta.get_field('name').max_length
         site.name = domain[:name_max_length]
         site.save()
     site.themes.all().delete()
-    site.themes.create(theme_dir_name=name)
+    if name != 'default':
+        site.themes.create(theme_dir_name=name)
 """
     domain_names = domain_names or [
         "{{ LMS_HOST }}",
         "{{ LMS_HOST }}:8000",
         "{{ CMS_HOST }}",
         "{{ CMS_HOST }}:8001",
         "{{ PREVIEW_LMS_HOST }}",
```

### Comparing `tutor-16.0.2/tutor/commands/k8s.py` & `tutor-16.0.3/tutor/commands/k8s.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/local.py` & `tutor-16.0.3/tutor/commands/local.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/mounts.py` & `tutor-16.0.3/tutor/commands/mounts.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/params.py` & `tutor-16.0.3/tutor/commands/params.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/plugins.py` & `tutor-16.0.3/tutor/commands/plugins.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/upgrade/common.py` & `tutor-16.0.3/tutor/commands/upgrade/common.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/upgrade/compose.py` & `tutor-16.0.3/tutor/commands/upgrade/compose.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/commands/upgrade/k8s.py` & `tutor-16.0.3/tutor/commands/upgrade/k8s.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/config.py` & `tutor-16.0.3/tutor/config.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/core/hooks/actions.py` & `tutor-16.0.3/tutor/core/hooks/actions.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/core/hooks/contexts.py` & `tutor-16.0.3/tutor/core/hooks/contexts.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/core/hooks/filters.py` & `tutor-16.0.3/tutor/core/hooks/filters.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/core/hooks/priorities.py` & `tutor-16.0.3/tutor/core/hooks/priorities.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/env.py` & `tutor-16.0.3/tutor/env.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/fmt.py` & `tutor-16.0.3/tutor/fmt.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/hooks/catalog.py` & `tutor-16.0.3/tutor/hooks/catalog.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/images.py` & `tutor-16.0.3/tutor/images.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/interactive.py` & `tutor-16.0.3/tutor/interactive.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/plugins/__init__.py` & `tutor-16.0.3/tutor/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/plugins/base.py` & `tutor-16.0.3/tutor/plugins/base.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/plugins/indexes.py` & `tutor-16.0.3/tutor/plugins/indexes.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/plugins/v0.py` & `tutor-16.0.3/tutor/plugins/v0.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/plugins/v1.py` & `tutor-16.0.3/tutor/plugins/v1.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/serialize.py` & `tutor-16.0.3/tutor/serialize.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/tasks.py` & `tutor-16.0.3/tutor/tasks.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/apps/caddy/Caddyfile` & `tutor-16.0.3/tutor/templates/apps/caddy/Caddyfile`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/apps/openedx/config/cms.env.yml` & `tutor-16.0.3/tutor/templates/apps/openedx/config/cms.env.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/apps/openedx/config/lms.env.yml` & `tutor-16.0.3/tutor/templates/apps/openedx/config/lms.env.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/apps/openedx/config/partials/auth.yml` & `tutor-16.0.3/tutor/templates/apps/openedx/config/partials/auth.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/apps/openedx/settings/cms/development.py` & `tutor-16.0.3/tutor/templates/apps/openedx/settings/cms/development.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/apps/openedx/settings/cms/production.py` & `tutor-16.0.3/tutor/templates/apps/openedx/settings/cms/production.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/apps/openedx/settings/lms/development.py` & `tutor-16.0.3/tutor/templates/apps/openedx/settings/lms/development.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/apps/openedx/settings/lms/production.py` & `tutor-16.0.3/tutor/templates/apps/openedx/settings/lms/production.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/apps/openedx/settings/partials/common_all.py` & `tutor-16.0.3/tutor/templates/apps/openedx/settings/partials/common_all.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/apps/openedx/settings/partials/common_cms.py` & `tutor-16.0.3/tutor/templates/apps/openedx/settings/partials/common_cms.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/apps/openedx/settings/partials/common_lms.py` & `tutor-16.0.3/tutor/templates/apps/openedx/settings/partials/common_lms.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/apps/redis/redis.conf` & `tutor-16.0.3/tutor/templates/apps/redis/redis.conf`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/build/openedx/Dockerfile` & `tutor-16.0.3/tutor/templates/build/openedx/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,17 @@
   && git config --global user.name "Tutor"
 
 {%- if patch("openedx-dockerfile-git-patches-default") %}
 # Custom edx-platform patches
 {{ patch("openedx-dockerfile-git-patches-default") }}
 {%- else %}
 # Patch edx-platform
+# Security advisory: https://github.com/openedx/edx-platform/security/advisories/GHSA-3q74-3rfh-g37j
+# https://github.com/openedx/edx-platform/pull/32838
+RUN curl -fsSL https://github.com/openedx/edx-platform/commit/163259779297a7dccb28e1f8c3dfa4d2cbdb9655.patch | git am
 {%- endif %}
 
 {# Example: RUN curl -fsSL https://github.com/openedx/edx-platform/commit/<GITSHA1>.patch | git am #}
 {{ patch("openedx-dockerfile-post-git-checkout") }}
 
 ##### Empty layer with just the repo at the root.
 # This is useful when overriding the build context with a host repo:
```

### Comparing `tutor-16.0.2/tutor/templates/build/openedx/bin/openedx-assets` & `tutor-16.0.3/tutor/templates/build/openedx/bin/openedx-assets`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/build/openedx/bin/site-configuration` & `tutor-16.0.3/tutor/templates/build/openedx/bin/site-configuration`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/config/base.yml` & `tutor-16.0.3/tutor/templates/config/base.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/config/defaults.yml` & `tutor-16.0.3/tutor/templates/config/defaults.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/dev/docker-compose.jobs.yml` & `tutor-16.0.3/tutor/templates/dev/docker-compose.jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/dev/docker-compose.yml` & `tutor-16.0.3/tutor/templates/dev/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/jobs/init/lms.sh` & `tutor-16.0.3/tutor/templates/jobs/init/lms.sh`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/jobs/init/mounted-edx-platform.sh` & `tutor-16.0.3/tutor/templates/jobs/init/mounted-edx-platform.sh`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/jobs/init/mysql.sh` & `tutor-16.0.3/tutor/templates/jobs/init/mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/k8s/deployments.yml` & `tutor-16.0.3/tutor/templates/k8s/deployments.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/k8s/jobs.yml` & `tutor-16.0.3/tutor/templates/k8s/jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/k8s/services.yml` & `tutor-16.0.3/tutor/templates/k8s/services.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/k8s/volumes.yml` & `tutor-16.0.3/tutor/templates/k8s/volumes.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/kustomization.yml` & `tutor-16.0.3/tutor/templates/kustomization.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/local/docker-compose.jobs.yml` & `tutor-16.0.3/tutor/templates/local/docker-compose.jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/local/docker-compose.prod.yml` & `tutor-16.0.3/tutor/templates/local/docker-compose.prod.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/templates/local/docker-compose.yml` & `tutor-16.0.3/tutor/templates/local/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/types.py` & `tutor-16.0.3/tutor/types.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor/utils.py` & `tutor-16.0.3/tutor/utils.py`

 * *Files identical despite different names*

### Comparing `tutor-16.0.2/tutor.egg-info/PKG-INFO` & `tutor-16.0.3/tutor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor
-Version: 16.0.2
+Version: 16.0.3
 Summary: The Docker-based Open edX distribution designed for peace of mind
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.io
 Author-email: contact@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor
```

### Comparing `tutor-16.0.2/tutor.egg-info/SOURCES.txt` & `tutor-16.0.3/tutor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

