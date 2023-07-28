# Comparing `tmp/autonomous-app-0.1.6.tar.gz` & `tmp/autonomous-app-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomous-app-0.1.6.tar", last modified: Thu Jul 27 17:55:28 2023, max compression
+gzip compressed data, was "autonomous-app-0.1.7.tar", last modified: Fri Jul 28 15:59:43 2023, max compression
```

## Comparing `autonomous-app-0.1.6.tar` & `autonomous-app-0.1.7.tar`

### file list

```diff
@@ -1,228 +1,67 @@
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.750192 autonomous-app-0.1.6/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-03-07 12:36:40.000000 autonomous-app-0.1.6/LICENSE
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-27 17:55:28.749192 autonomous-app-0.1.6/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2011 2023-06-20 21:09:23.000000 autonomous-app-0.1.6/README.md
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1469 2023-07-20 14:57:42.000000 autonomous-app-0.1.6/pyproject.toml
--rw-r--r--   0 samoore   (1000) samoore   (1000)      523 2023-07-27 14:43:37.000000 autonomous-app-0.1.6/requirements.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-27 17:55:28.750192 autonomous-app-0.1.6/setup.cfg
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-04-04 14:14:59.000000 autonomous-app-0.1.6/setup.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.710193 autonomous-app-0.1.6/src/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.712192 autonomous-app-0.1.6/src/autonomous/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       86 2023-07-27 17:54:34.000000 autonomous-app-0.1.6/src/autonomous/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.739192 autonomous-app-0.1.6/src/autonomous/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-06-20 19:34:19.000000 autonomous-app-0.1.6/src/autonomous/apis/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2149 2023-07-07 13:12:31.000000 autonomous-app-0.1.6/src/autonomous/apis/openai.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.740192 autonomous-app-0.1.6/src/autonomous/apis/version_control/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-03-07 16:24:11.000000 autonomous-app-0.1.6/src/autonomous/apis/version_control/GHCallbacks.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-03-07 21:09:26.000000 autonomous-app-0.1.6/src/autonomous/apis/version_control/GHOrganization.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-03-07 16:24:11.000000 autonomous-app-0.1.6/src/autonomous/apis/version_control/GHRepo.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-03-07 16:24:11.000000 autonomous-app-0.1.6/src/autonomous/apis/version_control/GHVersionControl.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-03-07 16:24:11.000000 autonomous-app-0.1.6/src/autonomous/apis/version_control/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.710193 autonomous-app-0.1.6/src/autonomous/app_template/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.741192 autonomous-app-0.1.6/src/autonomous/app_template/app/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       29 2023-04-04 14:32:12.000000 autonomous-app-0.1.6/src/autonomous/app_template/app/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1598 2023-07-27 16:48:05.000000 autonomous-app-0.1.6/src/autonomous/app_template/app/app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1316 2023-07-27 17:51:13.000000 autonomous-app-0.1.6/src/autonomous/app_template/app/config.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.742192 autonomous-app-0.1.6/src/autonomous/app_template/app/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-04-04 14:32:12.000000 autonomous-app-0.1.6/src/autonomous/app_template/app/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      203 2023-04-04 15:41:08.000000 autonomous-app-0.1.6/src/autonomous/app_template/app/models/model.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      517 2023-07-27 17:30:04.000000 autonomous-app-0.1.6/src/autonomous/app_template/app/tasks.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.743192 autonomous-app-0.1.6/src/autonomous/app_template/app/views/
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-04 14:32:12.000000 autonomous-app-0.1.6/src/autonomous/app_template/app/views/admin.py
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-28 17:48:57.000000 autonomous-app-0.1.6/src/autonomous/app_template/app/views/index.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.743192 autonomous-app-0.1.6/src/autonomous/app_template/tests/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-04 14:32:12.000000 autonomous-app-0.1.6/src/autonomous/app_template/tests/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      553 2023-07-27 16:58:09.000000 autonomous-app-0.1.6/src/autonomous/app_template/tests/conftest.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      204 2023-04-04 18:40:47.000000 autonomous-app-0.1.6/src/autonomous/app_template/tests/test_app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1018 2023-07-27 17:36:21.000000 autonomous-app-0.1.6/src/autonomous/app_template/tests/test_tasks.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.744192 autonomous-app-0.1.6/src/autonomous/app_template/vendor/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1124 2023-04-13 17:57:17.000000 autonomous-app-0.1.6/src/autonomous/app_template/vendor/gunicorn.conf.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2252 2023-06-08 19:19:57.000000 autonomous-app-0.1.6/src/autonomous/assets.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-04-04 14:14:59.000000 autonomous-app-0.1.6/src/autonomous/cli.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.744192 autonomous-app-0.1.6/src/autonomous/db/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       94 2023-07-07 12:00:23.000000 autonomous-app-0.1.6/src/autonomous/db/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      812 2023-07-07 12:05:15.000000 autonomous-app-0.1.6/src/autonomous/db/autodb.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      531 2023-04-04 14:14:59.000000 autonomous-app-0.1.6/src/autonomous/db/storage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2521 2023-06-20 21:17:55.000000 autonomous-app-0.1.6/src/autonomous/db/table.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1245 2023-06-01 20:06:24.000000 autonomous-app-0.1.6/src/autonomous/logger.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.745192 autonomous-app-0.1.6/src/autonomous/model/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-02 18:01:05.000000 autonomous-app-0.1.6/src/autonomous/model/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4035 2023-07-20 15:46:58.000000 autonomous-app-0.1.6/src/autonomous/model/automodel.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      650 2023-06-13 18:03:23.000000 autonomous-app-0.1.6/src/autonomous/model/orm.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.745192 autonomous-app-0.1.6/src/autonomous/storage/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       88 2023-06-13 18:11:53.000000 autonomous-app-0.1.6/src/autonomous/storage/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      447 2023-06-05 17:49:27.000000 autonomous-app-0.1.6/src/autonomous/storage/basestorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1620 2023-07-07 13:13:20.000000 autonomous-app-0.1.6/src/autonomous/storage/cloudinarystorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      156 2023-06-13 18:11:43.000000 autonomous-app-0.1.6/src/autonomous/storage/localstorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1381 2023-06-13 18:12:16.000000 autonomous-app-0.1.6/src/autonomous/storage/s3storage.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.746192 autonomous-app-0.1.6/src/autonomous/tasks/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       34 2023-07-27 15:55:55.000000 autonomous-app-0.1.6/src/autonomous/tasks/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      616 2023-07-27 17:54:09.000000 autonomous-app-0.1.6/src/autonomous/tasks/task.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.712192 autonomous-app-0.1.6/src/autonomous-app/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.703193 autonomous-app-0.1.6/src/autonomous-app/build/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.703193 autonomous-app-0.1.6/src/autonomous-app/build/lib/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.714192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       48 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.715192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/apis/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      834 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/apis/ai.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      769 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/apis/openai.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      834 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/apis/openapi.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.715192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/apis/opendnd/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/apis/opendnd/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2076 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/apis/opendnd/opendnd.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2076 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/apis/opendnd.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.705192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.717193 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/app/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       29 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/app/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1349 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/app/app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      667 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/app/config.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.717193 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/app/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/app/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      203 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/app/models/model.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.718192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/app/views/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      589 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/app/views/admin.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      584 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/app/views/index.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.719192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/tests/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/tests/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      252 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/tests/test_app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      538 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/tests/test_modules.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.719192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/vendor/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      738 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/app_template/vendor/gunicorn.conf.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1415 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/assets.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      604 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/autodb.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2313 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/autoencoder.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2192 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/automodel.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/cli.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.720192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      343 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      439 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/autodb.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      104 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/field.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      562 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/firestore.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      558 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/local.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      451 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/mongo.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1150 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.720192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       29 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.722192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      420 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)       35 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/async_redis.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      751 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/checks.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      524 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/connections.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.723192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/model/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      180 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/model/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.723192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/model/cli/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/model/cli/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      443 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/model/cli/migrate.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     6537 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/model/encoders.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.724192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/model/migrations/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/model/migrations/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     5204 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/model/migrations/migrator.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)    64005 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/model/model.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2210 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/model/query_resolver.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2140 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/model/render_tree.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      824 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/model/token_escaper.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)       13 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/sync_redis.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      218 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/aredis_om/util.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      994 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/make_sync.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.725192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/tests/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/tests/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1347 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/tests/conftest.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)    21344 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/tests/test_hash_model.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)    24483 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/tests/test_json_model.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4259 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/tests/test_oss_redis_features.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1120 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/tests/test_pydantic_integrations.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      284 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/database/redis_om/tests/test_redis_type.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.727192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/db/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      297 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/db/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      499 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/db/autodb.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      104 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/db/field.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      562 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/db/firestore.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      558 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/db/local.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      451 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/db/mongo.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1150 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/db/redis.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      531 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/db/storage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2501 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/db/table.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      757 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/logger.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.727192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/model/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/model/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2664 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/model/automodel.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      515 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/model/orm.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.728192 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/version_control/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/version_control/GHCallbacks.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/version_control/GHOrganization.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/version_control/GHRepo.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/version_control/GHVersionControl.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/build/lib/autonomous/version_control/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/setup.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.707193 autonomous-app-0.1.6/src/autonomous-app/src/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.729192 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       86 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.729192 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/apis/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2149 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/apis/openai.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.730192 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/apis/version_control/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/apis/version_control/GHCallbacks.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/apis/version_control/GHOrganization.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/apis/version_control/GHRepo.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/apis/version_control/GHVersionControl.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/apis/version_control/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.708192 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.731192 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/app/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       29 2023-07-26 18:49:21.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/app/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1495 2023-07-26 18:49:21.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/app/app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      574 2023-07-26 18:49:21.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/app/config.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.732192 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/app/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-26 18:49:21.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/app/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      203 2023-07-26 18:49:21.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/app/models/model.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.732192 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/app/views/
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-07-26 18:49:21.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/app/views/admin.py
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-07-26 18:49:21.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/app/views/index.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.733192 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/tests/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-07-26 18:49:21.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/tests/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      204 2023-07-26 18:49:21.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/tests/test_app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      558 2023-07-26 18:49:21.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/tests/test_modules.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.733192 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/vendor/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1124 2023-07-26 18:49:21.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/app_template/vendor/gunicorn.conf.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2252 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/assets.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/cli.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.734192 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/db/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       94 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/db/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      812 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/db/autodb.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      531 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/db/storage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2521 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/db/table.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1245 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/logger.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.735192 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/model/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/model/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4035 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/model/automodel.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      650 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/model/orm.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.736192 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/storage/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       88 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/storage/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      447 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/storage/basestorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1620 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/storage/cloudinarystorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      156 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/storage/localstorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1381 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/storage/s3storage.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.736192 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/tasks/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       23 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/tasks/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2201 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/tasks/task.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      529 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/src/autonomous/tasks/taskqueue.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.737192 autonomous-app-0.1.6/src/autonomous-app/tests/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/tests/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      154 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/tests/conftest.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.737192 autonomous-app-0.1.6/src/autonomous-app/tests/integration/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     5404 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/tests/integration/test_int_automodel.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.738192 autonomous-app-0.1.6/src/autonomous-app/tests/unit/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      972 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/tests/unit/test_assets.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     5569 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/tests/unit/test_automodel.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1835 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/tests/unit/test_db.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      401 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/tests/unit/test_modules.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1764 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/tests/unit/test_openAI.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1409 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/tests/unit/test_storage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3746 2023-07-26 18:49:20.000000 autonomous-app-0.1.6/src/autonomous-app/tests/unit/test_tasks.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-27 17:55:28.748192 autonomous-app-0.1.6/src/autonomous_app.egg-info/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-27 17:55:28.000000 autonomous-app-0.1.6/src/autonomous_app.egg-info/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     9466 2023-07-27 17:55:28.000000 autonomous-app-0.1.6/src/autonomous_app.egg-info/SOURCES.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-27 17:55:28.000000 autonomous-app-0.1.6/src/autonomous_app.egg-info/dependency_links.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       53 2023-07-27 17:55:28.000000 autonomous-app-0.1.6/src/autonomous_app.egg-info/entry_points.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)      162 2023-07-27 17:55:28.000000 autonomous-app-0.1.6/src/autonomous_app.egg-info/requires.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       26 2023-07-27 17:55:28.000000 autonomous-app-0.1.6/src/autonomous_app.egg-info/top_level.txt
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.880172 autonomous-app-0.1.7/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-03-07 12:36:40.000000 autonomous-app-0.1.7/LICENSE
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-28 15:59:43.880172 autonomous-app-0.1.7/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2011 2023-06-20 21:09:23.000000 autonomous-app-0.1.7/README.md
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1469 2023-07-20 14:57:42.000000 autonomous-app-0.1.7/pyproject.toml
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      523 2023-07-27 14:43:37.000000 autonomous-app-0.1.7/requirements.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-28 15:59:43.880172 autonomous-app-0.1.7/setup.cfg
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-04-04 14:14:59.000000 autonomous-app-0.1.7/setup.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.875172 autonomous-app-0.1.7/src/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.876172 autonomous-app-0.1.7/src/autonomous/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       86 2023-07-28 15:57:58.000000 autonomous-app-0.1.7/src/autonomous/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.876172 autonomous-app-0.1.7/src/autonomous/apis/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-06-20 19:34:19.000000 autonomous-app-0.1.7/src/autonomous/apis/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2149 2023-07-07 13:12:31.000000 autonomous-app-0.1.7/src/autonomous/apis/openai.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.876172 autonomous-app-0.1.7/src/autonomous/apis/version_control/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-03-07 16:24:11.000000 autonomous-app-0.1.7/src/autonomous/apis/version_control/GHCallbacks.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-03-07 21:09:26.000000 autonomous-app-0.1.7/src/autonomous/apis/version_control/GHOrganization.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-03-07 16:24:11.000000 autonomous-app-0.1.7/src/autonomous/apis/version_control/GHRepo.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-03-07 16:24:11.000000 autonomous-app-0.1.7/src/autonomous/apis/version_control/GHVersionControl.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-03-07 16:24:11.000000 autonomous-app-0.1.7/src/autonomous/apis/version_control/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.875172 autonomous-app-0.1.7/src/autonomous/app_template/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.877172 autonomous-app-0.1.7/src/autonomous/app_template/app/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       54 2023-07-28 15:13:30.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1598 2023-07-27 16:48:05.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/app.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1316 2023-07-27 17:51:13.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/config.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.877172 autonomous-app-0.1.7/src/autonomous/app_template/app/models/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-04-04 14:32:12.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/models/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      203 2023-04-04 15:41:08.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/models/model.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      517 2023-07-28 15:15:34.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/tasks.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.877172 autonomous-app-0.1.7/src/autonomous/app_template/app/views/
+-rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-04 14:32:12.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/views/admin.py
+-rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-28 17:48:57.000000 autonomous-app-0.1.7/src/autonomous/app_template/app/views/index.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.878172 autonomous-app-0.1.7/src/autonomous/app_template/tests/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-04 14:32:12.000000 autonomous-app-0.1.7/src/autonomous/app_template/tests/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      545 2023-07-28 15:11:47.000000 autonomous-app-0.1.7/src/autonomous/app_template/tests/conftest.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      204 2023-04-04 18:40:47.000000 autonomous-app-0.1.7/src/autonomous/app_template/tests/test_app.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1021 2023-07-28 15:54:14.000000 autonomous-app-0.1.7/src/autonomous/app_template/tests/test_tasks.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.878172 autonomous-app-0.1.7/src/autonomous/app_template/vendor/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1124 2023-04-13 17:57:17.000000 autonomous-app-0.1.7/src/autonomous/app_template/vendor/gunicorn.conf.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2252 2023-06-08 19:19:57.000000 autonomous-app-0.1.7/src/autonomous/assets.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-04-04 14:14:59.000000 autonomous-app-0.1.7/src/autonomous/cli.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.878172 autonomous-app-0.1.7/src/autonomous/db/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       94 2023-07-07 12:00:23.000000 autonomous-app-0.1.7/src/autonomous/db/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      812 2023-07-07 12:05:15.000000 autonomous-app-0.1.7/src/autonomous/db/autodb.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      531 2023-04-04 14:14:59.000000 autonomous-app-0.1.7/src/autonomous/db/storage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2521 2023-06-20 21:17:55.000000 autonomous-app-0.1.7/src/autonomous/db/table.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1245 2023-06-01 20:06:24.000000 autonomous-app-0.1.7/src/autonomous/logger.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.879172 autonomous-app-0.1.7/src/autonomous/model/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-02 18:01:05.000000 autonomous-app-0.1.7/src/autonomous/model/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4035 2023-07-20 15:46:58.000000 autonomous-app-0.1.7/src/autonomous/model/automodel.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      650 2023-06-13 18:03:23.000000 autonomous-app-0.1.7/src/autonomous/model/orm.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.879172 autonomous-app-0.1.7/src/autonomous/storage/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       88 2023-06-13 18:11:53.000000 autonomous-app-0.1.7/src/autonomous/storage/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      447 2023-06-05 17:49:27.000000 autonomous-app-0.1.7/src/autonomous/storage/basestorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1620 2023-07-07 13:13:20.000000 autonomous-app-0.1.7/src/autonomous/storage/cloudinarystorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      156 2023-06-13 18:11:43.000000 autonomous-app-0.1.7/src/autonomous/storage/localstorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1381 2023-06-13 18:12:16.000000 autonomous-app-0.1.7/src/autonomous/storage/s3storage.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.879172 autonomous-app-0.1.7/src/autonomous/tasks/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       34 2023-07-27 15:55:55.000000 autonomous-app-0.1.7/src/autonomous/tasks/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      615 2023-07-28 14:38:22.000000 autonomous-app-0.1.7/src/autonomous/tasks/task.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-28 15:59:43.880172 autonomous-app-0.1.7/src/autonomous_app.egg-info/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-28 15:59:43.000000 autonomous-app-0.1.7/src/autonomous_app.egg-info/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1788 2023-07-28 15:59:43.000000 autonomous-app-0.1.7/src/autonomous_app.egg-info/SOURCES.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-28 15:59:43.000000 autonomous-app-0.1.7/src/autonomous_app.egg-info/dependency_links.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       53 2023-07-28 15:59:43.000000 autonomous-app-0.1.7/src/autonomous_app.egg-info/entry_points.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      162 2023-07-28 15:59:43.000000 autonomous-app-0.1.7/src/autonomous_app.egg-info/requires.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       11 2023-07-28 15:59:43.000000 autonomous-app-0.1.7/src/autonomous_app.egg-info/top_level.txt
```

### Comparing `autonomous-app-0.1.6/LICENSE` & `autonomous-app-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/PKG-INFO` & `autonomous-app-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.6
+Version: 0.1.7
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous-app-0.1.6/README.md` & `autonomous-app-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/pyproject.toml` & `autonomous-app-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/requirements.txt` & `autonomous-app-0.1.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/apis/openai.py` & `autonomous-app-0.1.7/src/autonomous/apis/openai.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/apis/version_control/GHCallbacks.py` & `autonomous-app-0.1.7/src/autonomous/apis/version_control/GHCallbacks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/apis/version_control/GHOrganization.py` & `autonomous-app-0.1.7/src/autonomous/apis/version_control/GHOrganization.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/apis/version_control/GHRepo.py` & `autonomous-app-0.1.7/src/autonomous/apis/version_control/GHRepo.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/app_template/app/app.py` & `autonomous-app-0.1.7/src/autonomous/app_template/app/app.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/app_template/app/config.py` & `autonomous-app-0.1.7/src/autonomous/app_template/app/config.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/app_template/app/views/admin.py` & `autonomous-app-0.1.7/src/autonomous/app_template/app/views/admin.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/app_template/app/views/index.py` & `autonomous-app-0.1.7/src/autonomous/app_template/app/views/index.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/app_template/tests/conftest.py` & `autonomous-app-0.1.7/src/autonomous/app_template/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import os
 import pytest
-from app.app import create_app
+from app import create_app
 
 # Add the 'app' directory to the Python path
-sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "../app")))
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
 
 @pytest.fixture()
 def app():
     app = create_app()
     app.config.update(
         {
```

### Comparing `autonomous-app-0.1.6/src/autonomous/app_template/tests/test_tasks.py` & `autonomous-app-0.1.7/src/autonomous/app_template/tests/test_tasks.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 import time
 from celery.result import AsyncResult
 import pytest
 
 
 def test_base_task(app):
     results = mocktask.delay()
-    # breakpoint()
-    while results.status != "SUCCESS":
-        log(results.status)
-        time.sleep(1)
+    time.sleep(2)
+    log(results.status)
+    assert results.status == "SUCCESS"
     assert results.get() == "success"
 
 
 def test_param_task(app):
-    results = parametermocktask.delay("hello", "world", key="value")
-    while results.status != "SUCCESS":
-        time.sleep(1)
-        log(results.status)
-    assert results.get() == "success"
+    results = parametermocktask.delay(1, 2, "hello", key="value")
+    time.sleep(1)
+    log(results.status)
+    assert results.status == "SUCCESS"
+    assert results.get() == 3
 
 
 def test_error_task(app):
+    results = errormocktask.delay()
+    time.sleep(2)
+    log(results.status)
+    assert results.status == "FAILURE"
     try:
-        results = errormocktask.delay()
+        response = results.get()
     except Exception as e:
         log(e)
-
-    while results.status != "SUCCESS":
-        time.sleep(1)
-        log(results.status)
-    assert results.get() == "success"
+    else:
+        pytest.fail(f"Exception not raised: {response}")
 
 
 def test_base_long_task(app):
     task = longmocktask.delay()
     result = AsyncResult(task.id)
     log(result.status)
     result.ready()
```

### Comparing `autonomous-app-0.1.6/src/autonomous/app_template/vendor/gunicorn.conf.py` & `autonomous-app-0.1.7/src/autonomous/app_template/vendor/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/assets.py` & `autonomous-app-0.1.7/src/autonomous/assets.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/db/autodb.py` & `autonomous-app-0.1.7/src/autonomous/db/autodb.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/db/storage.py` & `autonomous-app-0.1.7/src/autonomous/db/storage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/db/table.py` & `autonomous-app-0.1.7/src/autonomous/db/table.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/logger.py` & `autonomous-app-0.1.7/src/autonomous/logger.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/model/automodel.py` & `autonomous-app-0.1.7/src/autonomous/model/automodel.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/model/orm.py` & `autonomous-app-0.1.7/src/autonomous/model/orm.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/storage/cloudinarystorage.py` & `autonomous-app-0.1.7/src/autonomous/storage/cloudinarystorage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/storage/s3storage.py` & `autonomous-app-0.1.7/src/autonomous/storage/s3storage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.6/src/autonomous/tasks/task.py` & `autonomous-app-0.1.7/src/autonomous/tasks/task.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def make_taskrunner(app):
     class AutoTask(celery.Task):
         def __call__(self, *args, **kwargs):
             with app.app_context():
                 return self.run(*args, **kwargs)
 
     celery_app = celery.Celery(
-        app.name,
+        "tasks",
         task_cls=AutoTask,
         backend=os.environ.get("CELERY_BACKEND", "rpc://user:bitnami@rabbitmq"),
         broker=os.environ.get("CELERY_BROKER_URL", "pyamqp://user:bitnami@rabbitmq"),
     )
 
     celery_app.config_from_object(app.config["CELERY"])
     celery_app.set_default()
```

### Comparing `autonomous-app-0.1.6/src/autonomous_app.egg-info/PKG-INFO` & `autonomous-app-0.1.7/src/autonomous_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.6
+Version: 0.1.7
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

