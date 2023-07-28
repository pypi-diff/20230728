# Comparing `tmp/skill-sdk-2.1.tar.gz` & `tmp/skill-sdk-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skill-sdk-2.1.tar", last modified: Wed May  3 09:56:17 2023, max compression
+gzip compressed data, was "skill-sdk-2.2.tar", last modified: Fri Jul 28 08:32:19 2023, max compression
```

## Comparing `skill-sdk-2.1.tar` & `skill-sdk-2.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.353810 skill-sdk-2.1/
--rw-r--r--   0 python-user  (1000) python-user  (1000)      844 2023-05-03 09:56:17.353810 skill-sdk-2.1/PKG-INFO
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     7428 2023-05-03 09:54:29.000000 skill-sdk-2.1/README.md
--rw-r--r--   0 python-user  (1000) python-user  (1000)       38 2023-05-03 09:56:17.353810 skill-sdk-2.1/setup.cfg
--rwxrwxrwx   0 python-user  (1000) python-user  (1000)     2517 2023-05-03 09:54:29.000000 skill-sdk-2.1/setup.py
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.321809 skill-sdk-2.1/skill_sdk/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1027 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/__init__.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1499 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/__main__.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1064 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/__version__.py
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.325809 skill-sdk-2.1/skill_sdk/cli/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     3782 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/__init__.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2733 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/develop.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2105 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/init.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1804 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/run.py
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.325809 skill-sdk-2.1/skill_sdk/cli/scaffold/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)      181 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/Dockerfile
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)      100 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/README.md
--rwxrwxrwx   0 python-user  (1000) python-user  (1000)      233 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/app.py
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.325809 skill-sdk-2.1/skill_sdk/cli/scaffold/impl/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)      743 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/impl/__init__.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)      951 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/impl/test_impl.py
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.325809 skill-sdk-2.1/skill_sdk/cli/scaffold/locale/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)      247 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/locale/de.po
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)      247 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/locale/en.po
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)      249 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/locale/fr.po
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)        7 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/requirements-dev.txt
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)       10 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/requirements.txt
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.325809 skill-sdk-2.1/skill_sdk/cli/scaffold/scripts/
--rwxrwxrwx   0 python-user  (1000) python-user  (1000)       40 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/scripts/develop
--rwxrwxrwx   0 python-user  (1000) python-user  (1000)      118 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/scripts/run
--rwxrwxrwx   0 python-user  (1000) python-user  (1000)       37 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/scripts/test
--rwxrwxrwx   0 python-user  (1000) python-user  (1000)       33 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/scripts/version
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)       85 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/scaffold/skill.conf
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2691 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/translate.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1406 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/cli/version.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)    11927 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/config.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)    13435 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/i18n.py
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.329809 skill-sdk-2.1/skill_sdk/intents/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)      513 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/intents/__init__.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)    13255 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/intents/entities.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)    12455 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/intents/handlers.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     5504 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/intents/request.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     8061 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/log.py
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.329809 skill-sdk-2.1/skill_sdk/middleware/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1145 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/middleware/__init__.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2612 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/middleware/error.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1544 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/middleware/log.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     4779 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/middleware/prometheus.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2545 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/middleware/skillassessment.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1796 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/middleware/tracing.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     6621 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/requests.py
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.329809 skill-sdk-2.1/skill_sdk/responses/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1849 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/responses/__init__.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     7800 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/responses/card.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     7909 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/responses/command.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1559 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/responses/error.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)      938 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/responses/info.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2401 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/responses/reprompt.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)    10468 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/responses/response.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1192 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/responses/response_facets.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     5000 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/responses/task.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1781 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/responses/touchpoint_instructions.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     6135 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/routes.py
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.329809 skill-sdk-2.1/skill_sdk/services/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)       32 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/services/__init__.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     3666 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/services/base.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2087 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/services/centraltoken.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     6192 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/services/location.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2641 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/services/persistence.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2809 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/services/text.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     9905 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/skill.py
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.329809 skill-sdk-2.1/skill_sdk/tools/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)       16 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/tools/__init__.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     7320 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/tools/translate.py
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.329809 skill-sdk-2.1/skill_sdk/ui/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)    13858 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/ui/__init__.py
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.329809 skill-sdk-2.1/skill_sdk/ui/css/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)      312 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/ui/css/app.d8642850.css
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)   416690 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/ui/css/chunk-vendors.905e374c.css
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     4286 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/ui/favicon.ico
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1093 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/ui/index.html
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.341810 skill-sdk-2.1/skill_sdk/ui/js/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)    20963 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/ui/js/app.2f455c99.js
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)    79104 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/ui/js/app.2f455c99.js.map
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)   428472 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/ui/js/chunk-vendors.77a4059f.js
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)  1514140 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/ui/js/chunk-vendors.77a4059f.js.map
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.349810 skill-sdk-2.1/skill_sdk/ui/templates/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)      385 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/ui/templates/app.j2
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)      571 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/ui/templates/impl.j2
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)      623 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/ui/templates/tests.j2
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.349810 skill-sdk-2.1/skill_sdk/utils/
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:15.000000 skill-sdk-2.1/skill_sdk/utils/__init__.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1963 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/utils/access_token_helper.py
--rw-rw-rw-   0 python-user  (1000) python-user  (1000)    11491 2023-05-03 09:54:29.000000 skill-sdk-2.1/skill_sdk/utils/util.py
-drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-05-03 09:56:17.325809 skill-sdk-2.1/skill_sdk.egg-info/
--rw-r--r--   0 python-user  (1000) python-user  (1000)      844 2023-05-03 09:56:17.000000 skill-sdk-2.1/skill_sdk.egg-info/PKG-INFO
--rw-r--r--   0 python-user  (1000) python-user  (1000)     2479 2023-05-03 09:56:17.000000 skill-sdk-2.1/skill_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 python-user  (1000) python-user  (1000)        1 2023-05-03 09:56:17.000000 skill-sdk-2.1/skill_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 python-user  (1000) python-user  (1000)       48 2023-05-03 09:56:17.000000 skill-sdk-2.1/skill_sdk.egg-info/entry_points.txt
--rw-r--r--   0 python-user  (1000) python-user  (1000)      466 2023-05-03 09:56:17.000000 skill-sdk-2.1/skill_sdk.egg-info/requires.txt
--rw-r--r--   0 python-user  (1000) python-user  (1000)       10 2023-05-03 09:56:17.000000 skill-sdk-2.1/skill_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.666532 skill-sdk-2.2/
+-rw-r--r--   0 python-user  (1000) python-user  (1000)      844 2023-07-28 08:32:19.666532 skill-sdk-2.2/PKG-INFO
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     7428 2023-07-28 08:32:17.000000 skill-sdk-2.2/README.md
+-rw-r--r--   0 python-user  (1000) python-user  (1000)       38 2023-07-28 08:32:19.666532 skill-sdk-2.2/setup.cfg
+-rwxrwxrwx   0 python-user  (1000) python-user  (1000)     2517 2023-07-28 08:32:17.000000 skill-sdk-2.2/setup.py
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.658532 skill-sdk-2.2/skill_sdk/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1027 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/__init__.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1499 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/__main__.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1064 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/__version__.py
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.658532 skill-sdk-2.2/skill_sdk/cli/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     3782 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/__init__.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2733 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/develop.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2105 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/init.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1804 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/run.py
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.658532 skill-sdk-2.2/skill_sdk/cli/scaffold/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)      181 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/Dockerfile
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)      100 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/README.md
+-rwxrwxrwx   0 python-user  (1000) python-user  (1000)      233 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/app.py
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.658532 skill-sdk-2.2/skill_sdk/cli/scaffold/impl/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)      743 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/impl/__init__.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)      951 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/impl/test_impl.py
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.658532 skill-sdk-2.2/skill_sdk/cli/scaffold/locale/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)      247 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/locale/de.po
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)      247 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/locale/en.po
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)      249 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/locale/fr.po
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)        7 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/requirements-dev.txt
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)       10 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/requirements.txt
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.662532 skill-sdk-2.2/skill_sdk/cli/scaffold/scripts/
+-rwxrwxrwx   0 python-user  (1000) python-user  (1000)       40 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/scripts/develop
+-rwxrwxrwx   0 python-user  (1000) python-user  (1000)      118 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/scripts/run
+-rwxrwxrwx   0 python-user  (1000) python-user  (1000)       37 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/scripts/test
+-rwxrwxrwx   0 python-user  (1000) python-user  (1000)       33 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/scripts/version
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)       85 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/scaffold/skill.conf
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2691 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/translate.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1406 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/cli/version.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)    11927 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/config.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)    13435 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/i18n.py
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.662532 skill-sdk-2.2/skill_sdk/intents/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)      513 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/intents/__init__.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)    13255 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/intents/entities.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)    12455 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/intents/handlers.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     5504 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/intents/request.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     8061 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/log.py
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.662532 skill-sdk-2.2/skill_sdk/middleware/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1145 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/middleware/__init__.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2612 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/middleware/error.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1544 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/middleware/log.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     4779 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/middleware/prometheus.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2545 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/middleware/skillassessment.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1796 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/middleware/tracing.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     6621 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/requests.py
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.662532 skill-sdk-2.2/skill_sdk/responses/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1849 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/responses/__init__.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     7800 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/responses/card.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     7909 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/responses/command.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1559 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/responses/error.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)      938 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/responses/info.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2401 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/responses/reprompt.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)    10557 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/responses/response.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1192 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/responses/response_facets.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     5000 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/responses/task.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1781 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/responses/touchpoint_instructions.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     6135 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/routes.py
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.662532 skill-sdk-2.2/skill_sdk/services/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)       32 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/services/__init__.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     3666 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/services/base.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2087 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/services/centraltoken.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     6192 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/services/location.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2641 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/services/persistence.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     2809 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/services/text.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     9905 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/skill.py
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.662532 skill-sdk-2.2/skill_sdk/tools/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)       16 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/tools/__init__.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     7320 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/tools/translate.py
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.662532 skill-sdk-2.2/skill_sdk/ui/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)    13858 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/ui/__init__.py
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.662532 skill-sdk-2.2/skill_sdk/ui/css/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)      312 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/ui/css/app.d8642850.css
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)   416690 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/ui/css/chunk-vendors.905e374c.css
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     4286 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/ui/favicon.ico
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1093 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/ui/index.html
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.666532 skill-sdk-2.2/skill_sdk/ui/js/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)    20963 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/ui/js/app.2f455c99.js
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)    79104 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/ui/js/app.2f455c99.js.map
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)   428472 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/ui/js/chunk-vendors.77a4059f.js
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)  1514140 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/ui/js/chunk-vendors.77a4059f.js.map
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.666532 skill-sdk-2.2/skill_sdk/ui/templates/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)      385 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/ui/templates/app.j2
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)      571 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/ui/templates/impl.j2
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)      623 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/ui/templates/tests.j2
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.666532 skill-sdk-2.2/skill_sdk/utils/
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/utils/__init__.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)     1963 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/utils/access_token_helper.py
+-rw-rw-rw-   0 python-user  (1000) python-user  (1000)    11491 2023-07-28 08:32:17.000000 skill-sdk-2.2/skill_sdk/utils/util.py
+drwxr-xr-x   0 python-user  (1000) python-user  (1000)        0 2023-07-28 08:32:19.658532 skill-sdk-2.2/skill_sdk.egg-info/
+-rw-r--r--   0 python-user  (1000) python-user  (1000)      844 2023-07-28 08:32:19.000000 skill-sdk-2.2/skill_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 python-user  (1000) python-user  (1000)     2479 2023-07-28 08:32:19.000000 skill-sdk-2.2/skill_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 python-user  (1000) python-user  (1000)        1 2023-07-28 08:32:19.000000 skill-sdk-2.2/skill_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 python-user  (1000) python-user  (1000)       48 2023-07-28 08:32:19.000000 skill-sdk-2.2/skill_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 python-user  (1000) python-user  (1000)      466 2023-07-28 08:32:19.000000 skill-sdk-2.2/skill_sdk.egg-info/requires.txt
+-rw-r--r--   0 python-user  (1000) python-user  (1000)       10 2023-07-28 08:32:19.000000 skill-sdk-2.2/skill_sdk.egg-info/top_level.txt
```

### Comparing `skill-sdk-2.1/PKG-INFO` & `skill-sdk-2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skill-sdk
-Version: 2.1
+Version: 2.2
 Summary: Magenta Voice Skill SDK for Python
 Home-page: https://github.com/telekom/voice-skill-sdk/
 Author: Deutsche Telekom Voicification Suite
 Author-email: vineet.hingorani@telekom.de
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `skill-sdk-2.1/README.md` & `skill-sdk-2.2/README.md`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/setup.py` & `skill-sdk-2.2/setup.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/__init__.py` & `skill-sdk-2.2/skill_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/__main__.py` & `skill-sdk-2.2/skill_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/__version__.py` & `skill-sdk-2.2/skill_sdk/__version__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 #
 
 """Magenta Voice Skill SDK: version info"""
 
 __name__ = "skill-sdk"
 __description__ = "Magenta Voice Skill SDK for Python"
 __url__ = "https://github.com/telekom/voice-skill-sdk/"
-__version__ = "2.1"
+__version__ = "2.2"
 __author__ = "Deutsche Telekom Voicification Suite"
 __author_email__ = "vineet.hingorani@telekom.de"
 __license__ = "MIT"
 __copyright__ = "Copyright 2021, Deutsche Telekom AG"
 
 __spi_version__ = "2.0"
```

### Comparing `skill-sdk-2.1/skill_sdk/cli/__init__.py` & `skill-sdk-2.2/skill_sdk/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/cli/develop.py` & `skill-sdk-2.2/skill_sdk/cli/develop.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/cli/init.py` & `skill-sdk-2.2/skill_sdk/cli/init.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/cli/run.py` & `skill-sdk-2.2/skill_sdk/cli/run.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/cli/scaffold/impl/__init__.py` & `skill-sdk-2.2/skill_sdk/cli/scaffold/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/cli/scaffold/impl/test_impl.py` & `skill-sdk-2.2/skill_sdk/cli/scaffold/impl/test_impl.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/cli/translate.py` & `skill-sdk-2.2/skill_sdk/cli/translate.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/cli/version.py` & `skill-sdk-2.2/skill_sdk/cli/version.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/config.py` & `skill-sdk-2.2/skill_sdk/config.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/i18n.py` & `skill-sdk-2.2/skill_sdk/i18n.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/intents/__init__.py` & `skill-sdk-2.2/skill_sdk/intents/__init__.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/intents/entities.py` & `skill-sdk-2.2/skill_sdk/intents/entities.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/intents/handlers.py` & `skill-sdk-2.2/skill_sdk/intents/handlers.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/intents/request.py` & `skill-sdk-2.2/skill_sdk/intents/request.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/log.py` & `skill-sdk-2.2/skill_sdk/log.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/middleware/__init__.py` & `skill-sdk-2.2/skill_sdk/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/middleware/error.py` & `skill-sdk-2.2/skill_sdk/middleware/error.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/middleware/log.py` & `skill-sdk-2.2/skill_sdk/middleware/log.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/middleware/prometheus.py` & `skill-sdk-2.2/skill_sdk/middleware/prometheus.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/middleware/skillassessment.py` & `skill-sdk-2.2/skill_sdk/middleware/skillassessment.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/middleware/tracing.py` & `skill-sdk-2.2/skill_sdk/middleware/tracing.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/requests.py` & `skill-sdk-2.2/skill_sdk/requests.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/responses/__init__.py` & `skill-sdk-2.2/skill_sdk/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/responses/card.py` & `skill-sdk-2.2/skill_sdk/responses/card.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/responses/command.py` & `skill-sdk-2.2/skill_sdk/responses/command.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/responses/error.py` & `skill-sdk-2.2/skill_sdk/responses/error.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/responses/info.py` & `skill-sdk-2.2/skill_sdk/responses/info.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/responses/reprompt.py` & `skill-sdk-2.2/skill_sdk/responses/reprompt.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/responses/response.py` & `skill-sdk-2.2/skill_sdk/responses/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,16 @@
             *,
             command: Optional[Command] = None,
             task: Optional[ClientTask] = None,
             target_device_id: Optional[Text] = None,
             masked_response: Optional[Text] = None,
             ssml: Optional[Text] = None,
             card: Optional[CardFacet] = None,
-            error: Optional[ErrorFacet] = None
+            error: Optional[ErrorFacet] = None,
+            **kwargs
     ) -> "SkillInvokeResponse":
 
         facets: Dict[Text, Any] = {}
         if command is not None or task is not None:
             instructions = self.response_facets.touchpoint_instructions or TouchpointInstructionsFacet(data={})
             if command is not None:
                 instructions.update(command.dict())
@@ -189,14 +190,16 @@
             facets.update(vast=VastFacet(masked_response=masked_response))
         if ssml is not None:
             facets.update(tts=TtsFacet(ssml=ssml))
         if card is not None:
             facets.update(card=card)
         if error is not None:
             facets.update(error=error)
+        if kwargs is not None:
+            facets.update(**kwargs)
 
         if len(facets) != 0:
             return self.copy(update=dict(response_facets=self.response_facets.copy(update=facets)))
         return self
 
     def with_command(self, command: Command) -> "SkillInvokeResponse":
         """
```

### Comparing `skill-sdk-2.1/skill_sdk/responses/response_facets.py` & `skill-sdk-2.2/skill_sdk/responses/response_facets.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/responses/task.py` & `skill-sdk-2.2/skill_sdk/responses/task.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/responses/touchpoint_instructions.py` & `skill-sdk-2.2/skill_sdk/responses/touchpoint_instructions.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/routes.py` & `skill-sdk-2.2/skill_sdk/routes.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/services/base.py` & `skill-sdk-2.2/skill_sdk/services/base.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/services/centraltoken.py` & `skill-sdk-2.2/skill_sdk/services/centraltoken.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/services/location.py` & `skill-sdk-2.2/skill_sdk/services/location.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/services/persistence.py` & `skill-sdk-2.2/skill_sdk/services/persistence.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/services/text.py` & `skill-sdk-2.2/skill_sdk/services/text.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/skill.py` & `skill-sdk-2.2/skill_sdk/skill.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/tools/translate.py` & `skill-sdk-2.2/skill_sdk/tools/translate.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/ui/__init__.py` & `skill-sdk-2.2/skill_sdk/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/ui/css/chunk-vendors.905e374c.css` & `skill-sdk-2.2/skill_sdk/ui/css/chunk-vendors.905e374c.css`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/ui/favicon.ico` & `skill-sdk-2.2/skill_sdk/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/ui/index.html` & `skill-sdk-2.2/skill_sdk/ui/index.html`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/ui/js/app.2f455c99.js` & `skill-sdk-2.2/skill_sdk/ui/js/app.2f455c99.js`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/ui/js/app.2f455c99.js.map` & `skill-sdk-2.2/skill_sdk/ui/js/app.2f455c99.js.map`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/ui/js/chunk-vendors.77a4059f.js` & `skill-sdk-2.2/skill_sdk/ui/js/chunk-vendors.77a4059f.js`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/ui/js/chunk-vendors.77a4059f.js.map` & `skill-sdk-2.2/skill_sdk/ui/js/chunk-vendors.77a4059f.js.map`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/ui/templates/impl.j2` & `skill-sdk-2.2/skill_sdk/ui/templates/impl.j2`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/ui/templates/tests.j2` & `skill-sdk-2.2/skill_sdk/ui/templates/tests.j2`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/utils/access_token_helper.py` & `skill-sdk-2.2/skill_sdk/utils/access_token_helper.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk/utils/util.py` & `skill-sdk-2.2/skill_sdk/utils/util.py`

 * *Files identical despite different names*

### Comparing `skill-sdk-2.1/skill_sdk.egg-info/PKG-INFO` & `skill-sdk-2.2/skill_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skill-sdk
-Version: 2.1
+Version: 2.2
 Summary: Magenta Voice Skill SDK for Python
 Home-page: https://github.com/telekom/voice-skill-sdk/
 Author: Deutsche Telekom Voicification Suite
 Author-email: vineet.hingorani@telekom.de
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `skill-sdk-2.1/skill_sdk.egg-info/SOURCES.txt` & `skill-sdk-2.2/skill_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

