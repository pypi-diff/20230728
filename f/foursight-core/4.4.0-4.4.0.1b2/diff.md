# Comparing `tmp/foursight_core-4.4.0.tar.gz` & `tmp/foursight_core-4.4.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.4.0.tar", max compression
+gzip compressed data, was "foursight_core-4.4.0.1b2.tar", max compression
```

## Comparing `foursight_core-4.4.0.tar` & `foursight_core-4.4.0.1b2.tar`

### file list

```diff
@@ -1,76 +1,78 @@
--rw-r--r--   0        0        0     1083 2023-07-16 13:33:02.440657 foursight_core-4.4.0/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-07-16 13:33:02.444657 foursight_core-4.4.0/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-07-16 13:33:02.444657 foursight_core-4.4.0/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-07-16 13:33:02.444657 foursight_core-4.4.0/foursight_core/app.py
--rw-r--r--   0        0        0   103901 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/app_utils.py
--rw-r--r--   0        0        0     1283 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/boto_s3.py
--rw-r--r--   0        0        0     1305 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/boto_sqs.py
--rw-r--r--   0        0        0     2589 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     7293 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/decorators.py
--rw-r--r--   0        0        0    15846 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/deploy.py
--rw-r--r--   0        0        0     8235 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/environment.py
--rw-r--r--   0        0        0    11948 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5641 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     7218 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3061 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6098 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6373 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     4096 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0    10609 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5214 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    98198 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    36818 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    12028 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1868943 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/routes.py
--rw-r--r--   0        0        0    22941 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/run_result.py
--rw-r--r--   0        0        0     6380 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     5442 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1471 2023-07-16 13:33:02.460657 foursight_core-4.4.0/pyproject.toml
--rw-r--r--   0        0        0     1236 1970-01-01 00:00:00.000000 foursight_core-4.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-28 03:54:22.034038 foursight_core-4.4.0.1b2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/app.py
+-rw-r--r--   0        0        0   103901 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     1283 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/boto_s3.py
+-rw-r--r--   0        0        0     1305 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/boto_sqs.py
+-rw-r--r--   0        0        0     2589 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/buckets.py
+-rw-r--r--   0        0        0     3122 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/captured_output.py
+-rw-r--r--   0        0        0      638 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    30084 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     7293 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    12197 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15846 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8235 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/environment.py
+-rw-r--r--   0        0        0    11948 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5663 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     7218 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3061 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6098 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6373 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     4096 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0    10609 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5214 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    98198 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    36818 2023-07-28 03:54:22.042038 foursight_core-4.4.0.1b2/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-07-28 03:54:22.046038 foursight_core-4.4.0.1b2/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-07-28 03:54:22.046038 foursight_core-4.4.0.1b2/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-07-28 03:54:22.046038 foursight_core-4.4.0.1b2/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-07-28 03:54:22.046038 foursight_core-4.4.0.1b2/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-07-28 03:54:22.046038 foursight_core-4.4.0.1b2/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    12028 2023-07-28 03:54:22.046038 foursight_core-4.4.0.1b2/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1868943 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/routes.py
+-rw-r--r--   0        0        0    22941 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6380 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     8854 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/scripts/local_check_execution.py
+-rw-r--r--   0        0        0     5442 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-07-28 03:54:22.054038 foursight_core-4.4.0.1b2/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1500 2023-07-28 03:54:22.058039 foursight_core-4.4.0.1b2/pyproject.toml
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 foursight_core-4.4.0.1b2/PKG-INFO
```

### Comparing `foursight_core-4.4.0/LICENSE.txt` & `foursight_core-4.4.0.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/abstract_connection.py` & `foursight_core-4.4.0.1b2/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/app_utils.py` & `foursight_core-4.4.0.1b2/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/boto_s3.py` & `foursight_core-4.4.0.1b2/foursight_core/boto_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/boto_sqs.py` & `foursight_core-4.4.0.1b2/foursight_core/boto_sqs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/buckets.py` & `foursight_core-4.4.0.1b2/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/check_schema.py` & `foursight_core-4.4.0.1b2/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/check_utils.py` & `foursight_core-4.4.0.1b2/foursight_core/check_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import os
-import importlib
+from collections import namedtuple
 import copy
+import importlib
 import json
 import logging
+import os
+from typing import Callable, Optional
 from dcicutils.env_base import EnvBase
 from dcicutils.env_utils import infer_foursight_from_env
 from dcicutils.misc_utils import json_leaf_subst
 from foursight_core.check_schema import CheckSchema
 from foursight_core.exceptions import BadCheckSetup
 from foursight_core.environment import Environment
 from foursight_core.decorators import Decorators
@@ -35,15 +37,15 @@
         # that the passed path exists - Will 5/26/21
 
         # The check_setup_file is now pass in. It is supposed to ultimately come from chalicelib_cgap or
         # chalicelib_fourfront via the AppUtils there (derived from AppUtilsCore here in foursight-core),
         # which calls back to the locate_check_setup_file function AppUtilsCore here in foursight-core).
         if not os.path.exists(check_setup_file):
             raise BadCheckSetup(f"Did not locate the specified check setup file: {check_setup_file}")
-        self.CHECK_SETUP_FILE = check_setup_file # for display/troubleshooting
+        self.CHECK_SETUP_FILE = check_setup_file  # for display/troubleshooting
         with open(check_setup_file, 'r') as jfile:
             self.CHECK_SETUP = json.load(jfile)
         logger.debug(f"foursight_core/CheckHandler: Loaded check_setup.json file: {check_setup_file} ...")
         logger.debug(self.CHECK_SETUP)
         # Validate and finalize CHECK_SETUP
         logger.debug(f"foursight_core/CheckHandler: Validating check_setup.json file: {check_setup_file}")
         self.CHECK_SETUP = self.expand_check_setup(self.CHECK_SETUP, env)
@@ -356,15 +358,15 @@
                 grouped_results[group][setup_info['title']] = res
                 if res['status'] in grouped_results[group]['_statuses']:
                     grouped_results[group]['_statuses'][res['status']] += 1
         # format into a list and sort alphabetically
         grouped_list = [group for group in grouped_results.values()]
         return sorted(grouped_list, key=lambda v: v['_name'])
 
-    def run_check_or_action(self, connection, check_str, check_kwargs):
+    def obsolete_run_check_or_action(self, connection, check_str, check_kwargs):
         """
         Does validation of provided check_str, it's module, and kwargs.
         Determines by decorator whether the method is a check or action, then runs
         it. All errors are taken care of within the running of the check/action.
 
         Takes a FS_connection object, a check string formatted as: <str check module/name>
         and a dictionary of check arguments.
@@ -396,14 +398,161 @@
         if not check_method:
             return ' '.join(['ERROR. Check name is not valid.', error_str])
         if not self.check_method_deco(check_method, self.CHECK_DECO) and \
            not self.check_method_deco(check_method, self.ACTION_DECO):
             return ' '.join(['ERROR. Check or action must use a decorator.', error_str])
         return check_method(connection, **check_kwargs)
 
+    def run_check_or_action(self, connection, check_str, check_kwargs):
+        """
+        Does validation of provided check_str, it's module, and kwargs.
+        Determines by decorator whether the method is a check or action, then runs
+        it. All errors are taken care of within the running of the check/action.
+
+        Takes a FS_connection object, a check string formatted as: <str check module/name>
+        and a dictionary of check arguments.
+        For example:
+        check_str: 'system_checks/my_check'
+        check_kwargs: '{"foo":123}'
+        Fetches the check function and runs it (returning whatever it returns)
+        Return a string for failed results, CheckResult/ActionResult object otherwise.
+        """
+        check_method = None
+        try:
+            check_method = self._get_check_or_action_function(check_str)
+        except Exception as e:
+            return f"ERROR: {str(e)}"
+        if not isinstance(check_kwargs, dict):
+            return "ERROR: Check kwargs must be a dictionary: {check_str}"
+        return check_method(connection, **check_kwargs)
+
+    def _get_check_or_action_function(self, check_or_action_string: str, check_or_action: str = "check") -> Callable:
+        if len(check_or_action_string.strip().split('/')) != 2:
+            raise Exception(f"{check_or_action.title()} string must be of form"
+                            "module_name/{check_or_action}_function_name: {check_or_action_string}")
+        module_name = check_or_action_string.strip().split('/')[0]
+        function_name = check_or_action_string.strip().split('/')[1]
+        module = None
+        for package_name in [self.check_package_name, 'foursight_core']:
+            try:
+                module = self.import_check_module(package_name, module_name)
+            except ModuleNotFoundError:
+                continue
+            except Exception as e:
+                raise e
+        if not module:
+            raise Exception(f"Cannot find check module: {module_name}")
+        function = module.__dict__.get(function_name)
+        if not function:
+            raise Exception(f"Cannot find check function: {module_name}/{function_name}")
+        if not self.check_method_deco(function, self.CHECK_DECO) and \
+           not self.check_method_deco(function, self.ACTION_DECO):
+            raise Exception(f"{check_or_action.title()} function must use"
+                            "@{check_or_action}_function decorator: {module_name}/{function_name}")
+        return function
+
+    @staticmethod
+    def get_checks_info(search: str = None) -> list:
+        checks = []
+        registry = Decorators.get_registry()
+        for item in registry:
+            info = CheckHandler._create_check_or_action_info(registry[item])
+            if search and search not in info.qualified_name.lower():
+                continue
+            if info.is_check:
+                checks.append(info)
+        return sorted(checks, key=lambda item: item.qualified_name)
+
+    @staticmethod
+    def get_actions_info(search: str = None) -> list:
+        actions = []
+        registry = Decorators.get_registry()
+        for item in registry:
+            info = CheckHandler._create_check_or_action_info(registry[item])
+            if search and search not in info.qualified_name.lower():
+                continue
+            if info.is_action:
+                actions.append(info)
+        return sorted(actions, key=lambda item: item.qualified_name)
+
+    @staticmethod
+    def get_check_info(check_function_name: str, check_module_name: str = None) -> Optional[namedtuple]:
+        return CheckHandler._get_check_or_action_info(check_function_name, check_module_name, "check")
+
+    @staticmethod
+    def get_action_info(action_function_name: str, action_module_name: str = None) -> Optional[namedtuple]:
+        return CheckHandler._get_check_or_action_info(action_function_name, action_module_name, "action")
+
+    @staticmethod
+    def _get_check_or_action_info(function_name: str,
+                                  module_name: str = None, kind: str = None) -> Optional[namedtuple]:
+
+        function_name = function_name.strip();
+        if module_name:
+            module_name = module_name.strip();
+        if not module_name:
+            if len(function_name.split("/")) == 2:
+                module_name = function_name.split("/")[0].strip()
+                function_name = function_name.split("/")[1].strip()
+            elif len(function_name.split(".")) == 2:
+                module_name = function_name.split(".")[0].strip()
+                function_name = function_name.split(".")[1].strip()
+        registry = Decorators.get_registry()
+        for name in registry:
+            if not kind or registry[name]["kind"] == kind:
+                item = registry[name]
+                if item["name"] == function_name:
+                    if not module_name:
+                        return CheckHandler._create_check_or_action_info(item)
+                    if item["module"].endswith("." + module_name):
+                        return CheckHandler._create_check_or_action_info(item)
+
+    @staticmethod
+    def _create_check_or_action_info(info: dict) -> Optional[namedtuple]:
+
+        def unqualified_module_name(module_name: str) -> str:
+            return module_name.rsplit(".", 1)[-1] if "." in module_name else module_name
+
+        def qualified_check_or_action_name(check_or_action_name: str, module_name: str) -> str:
+            unqualified_module = unqualified_module_name(module_name)
+            return f"{unqualified_module}/{check_or_action_name}" if unqualified_module else check_or_action_name
+
+        Info = namedtuple("CheckInfo", ["kind",
+                                        "is_check",
+                                        "is_action",
+                                        "name",
+                                        "qualified_name",
+                                        "file",
+                                        "line",
+                                        "module",
+                                        "unqualified_module",
+                                        "package",
+                                        "github_url",
+                                        "args",
+                                        "kwargs",
+                                        "function",
+                                        "associated_action",
+                                        "associated_check"])
+        return Info(info["kind"],
+                    info["kind"] == "check",
+                    info["kind"] == "action",
+                    info["name"],
+                    qualified_check_or_action_name(info["name"], info["module"]),
+                    info["file"],
+                    info["line"],
+                    info["module"],
+                    unqualified_module_name(info["module"]),
+                    info["package"],
+                    info["github_url"],
+                    info["args"],
+                    info["kwargs"],
+                    info["function"],
+                    info.get("action"),
+                    info.get("check"))
+
     def init_check_or_action_res(self, connection, check):
         """
         Use in cases where a string is provided that could be a check or an action
         Returns None if neither are valid. Tries checks first then actions.
         If successful, returns a CheckResult or ActionResult
         """
         is_action = False
```

### Comparing `foursight_core-4.4.0/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.4.0.1b2/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.4.0.1b2/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/checks/ecs_checks.py` & `foursight_core-4.4.0.1b2/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.4.0.1b2/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.4.0.1b2/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.4.0.1b2/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/checks/scaling_checks.py` & `foursight_core-4.4.0.1b2/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/checks/test_checks.py` & `foursight_core-4.4.0.1b2/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/decorators.py` & `foursight_core-4.4.0.1b2/foursight_core/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,18 +83,24 @@
             "name": func_name,
             "file": func_file,
             "line": func_line,
             "module": func_module,
             "package": func_package,
             "github_url": get_github_url(func_package, func_file, func_line),
             "args": default_args,
-            "kwargs": default_kwargs
+            "kwargs": default_kwargs,
+            "function": func
         }
         if associated_action:
             registry_record["action"] = associated_action
+        elif kind == "action":
+            for name in _decorator_registry:
+                item = _decorator_registry[name]
+                if item.get("action") == func_name:
+                    registry_record["check"] = item["name"] 
         _decorator_registry[func_name] = registry_record
 
     def check_function(self, *default_args, **default_kwargs):
         """
         Import decorator, used to decorate all checks.
         Sets the check_decorator attribute so that methods can be fetched.
         Any kwargs provided to the decorator will be passed to the function
```

### Comparing `foursight_core-4.4.0/foursight_core/deploy.py` & `foursight_core-4.4.0.1b2/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/environment.py` & `foursight_core-4.4.0.1b2/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/es_connection.py` & `foursight_core-4.4.0.1b2/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/exceptions.py` & `foursight_core-4.4.0.1b2/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/fs_connection.py` & `foursight_core-4.4.0.1b2/foursight_core/fs_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self.connections = {
             's3': S3Connection(fs_environ_info.get('bucket')),
             'es': es
         }
         # FOURFRONT information
         self.ff_server = fs_environ_info['fourfront']
         self.ff_env = fs_environ_info['ff_env']
-        self.ff_es = fs_environ_info['es']
+        self.ff_es = fs_environ_info['es'] if not host else host
         self.ff_bucket = fs_environ_info['bucket']
         self.redis = None
         self.redis_url = None
         try:
             if 'redis' in fs_environ_info:
                 self.redis_url = fs_environ_info['redis']
             elif 'REDIS_HOST' in os.environ:  # temporary patch in until env config is fully sorted - Will
```

### Comparing `foursight_core-4.4.0/foursight_core/identity.py` & `foursight_core-4.4.0.1b2/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/mapping.json` & `foursight_core-4.4.0.1b2/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/package.py` & `foursight_core-4.4.0.1b2/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/auth.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/auth0_config.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/aws_network.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/aws_s3.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/checks.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/cognito.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/encryption.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/envs.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/gac.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/misc_utils.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/react_api.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/react_api.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/react_api_base.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/react_routes.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/react_ui.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.4.0.1b2/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/ui/index.html` & `foursight_core-4.4.0.1b2/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.4.0.1b2/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.4.0.1b2/foursight_core/react/ui/static/js/main.js`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/route_prefixes.py` & `foursight_core-4.4.0.1b2/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/routes.py` & `foursight_core-4.4.0.1b2/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/run_result.py` & `foursight_core-4.4.0.1b2/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/s3_connection.py` & `foursight_core-4.4.0.1b2/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/schedule_decorator.py` & `foursight_core-4.4.0.1b2/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/sqs_utils.py` & `foursight_core-4.4.0.1b2/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/stage.py` & `foursight_core-4.4.0.1b2/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/templates/base.html` & `foursight_core-4.4.0.1b2/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/templates/header.html` & `foursight_core-4.4.0.1b2/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/templates/history.html` & `foursight_core-4.4.0.1b2/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/templates/info.html` & `foursight_core-4.4.0.1b2/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/templates/unused.html` & `foursight_core-4.4.0.1b2/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/templates/user.html` & `foursight_core-4.4.0.1b2/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/templates/users.html` & `foursight_core-4.4.0.1b2/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/templates/view_checks.html` & `foursight_core-4.4.0.1b2/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/foursight_core/templates/view_groups.html` & `foursight_core-4.4.0.1b2/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.4.0/pyproject.toml` & `foursight_core-4.4.0.1b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.4.0"
+version = "4.4.0.1b2"  # TODO: To become 4.4.1
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.4.0/PKG-INFO` & `foursight_core-4.4.0.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.4.0
+Version: 4.4.0.1b2
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

