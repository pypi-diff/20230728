# Comparing `tmp/tabcmd-2.0.8.tar.gz` & `tmp/tabcmd-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabcmd-2.0.8.tar", last modified: Thu Dec  8 22:41:05 2022, max compression
+gzip compressed data, was "tabcmd-2.0.9.tar", last modified: Fri Dec 16 07:16:26 2022, max compression
```

## Comparing `tabcmd-2.0.8.tar` & `tabcmd-2.0.9.tar`

### file list

```diff
@@ -1,279 +1,279 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.684636 tabcmd-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    69632 2022-12-08 22:40:39.000000 tabcmd-2.0.8/.coverage
--rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-08 22:40:39.000000 tabcmd-2.0.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.656636 tabcmd-2.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2022-12-08 22:40:39.000000 tabcmd-2.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.656636 tabcmd-2.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2022-12-08 22:40:39.000000 tabcmd-2.0.8/.github/workflows/check-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2022-12-08 22:40:39.000000 tabcmd-2.0.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2022-12-08 22:40:39.000000 tabcmd-2.0.8/.github/workflows/generate-metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2022-12-08 22:40:39.000000 tabcmd-2.0.8/.github/workflows/package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2022-12-08 22:40:39.000000 tabcmd-2.0.8/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      973 2022-12-08 22:40:39.000000 tabcmd-2.0.8/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2022-12-08 22:40:39.000000 tabcmd-2.0.8/.github/workflows/run-e2-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      917 2022-12-08 22:40:39.000000 tabcmd-2.0.8/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2022-12-08 22:40:39.000000 tabcmd-2.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2022-12-08 22:40:39.000000 tabcmd-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2022-12-08 22:41:05.684636 tabcmd-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2022-12-08 22:40:39.000000 tabcmd-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-08 22:40:39.000000 tabcmd-2.0.8/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2022-12-08 22:40:39.000000 tabcmd-2.0.8/World Indicators.tdsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.656636 tabcmd-2.0.8/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2022-12-08 22:40:39.000000 tabcmd-2.0.8/bin/coverage.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.656636 tabcmd-2.0.8/bin/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2022-12-08 22:40:39.000000 tabcmd-2.0.8/bin/i18n/makelocalealias.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7660 2022-12-08 22:40:39.000000 tabcmd-2.0.8/bin/i18n/msgfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2022-12-08 22:40:39.000000 tabcmd-2.0.8/bin/i18n/prop2po.py
--rw-r--r--   0 runner    (1001) docker     (123)    24195 2022-12-08 22:40:39.000000 tabcmd-2.0.8/bin/i18n/pygettext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2022-12-08 22:40:39.000000 tabcmd-2.0.8/bin/license-checker.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-08 22:40:39.000000 tabcmd-2.0.8/bin/pyinstaller.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2022-12-08 22:40:39.000000 tabcmd-2.0.8/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2022-12-08 22:40:39.000000 tabcmd-2.0.8/dodo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2022-12-08 22:40:39.000000 tabcmd-2.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.656636 tabcmd-2.0.8/res/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-08 22:40:39.000000 tabcmd-2.0.8/res/metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)    28088 2022-12-08 22:40:39.000000 tabcmd-2.0.8/res/tabcmd.icns
--rw-r--r--   0 runner    (1001) docker     (123)   197222 2022-12-08 22:40:39.000000 tabcmd-2.0.8/res/tabcmd.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2022-12-08 22:40:39.000000 tabcmd-2.0.8/res/tabcmd.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 22:41:05.684636 tabcmd-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-08 22:40:39.000000 tabcmd-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.656636 tabcmd-2.0.8/tabcmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.660636 tabcmd-2.0.8/tabcmd/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.660636 tabcmd-2.0.8/tabcmd/commands/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/auth/login_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/auth/logout_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    14970 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/auth/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.660636 tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/datasources_and_workbooks_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/delete_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     8271 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/export_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/get_url_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/publish_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/runschedule_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.660636 tabcmd-2.0.8/tabcmd/commands/extracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/extracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/extracts/create_extracts_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/extracts/decrypt_extracts_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/extracts/delete_extracts_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/extracts/encrypt_extracts_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/extracts/reencrypt_extracts_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/extracts/refresh_extracts_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.660636 tabcmd-2.0.8/tabcmd/commands/group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/group/create_group_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/group/delete_group_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.664636 tabcmd-2.0.8/tabcmd/commands/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/project/create_project_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/project/delete_project_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/project/publish_samples_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.664636 tabcmd-2.0.8/tabcmd/commands/site/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/site/create_site_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/site/delete_site_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/site/edit_site_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/site/list_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/site/list_sites_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.664636 tabcmd-2.0.8/tabcmd/commands/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/user/add_users_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/user/create_site_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/user/create_users_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/user/delete_site_users_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/user/remove_users_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    10862 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/commands/user/user_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.664636 tabcmd-2.0.8/tabcmd/execution/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/execution/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/execution/global_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/execution/localize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/execution/logger_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/execution/map_of_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/execution/parent_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/execution/tabcmd_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.652636 tabcmd-2.0.8/tabcmd/locales/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.664636 tabcmd-2.0.8/tabcmd/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.664636 tabcmd-2.0.8/tabcmd/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/de/LC_MESSAGES/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/de/LC_MESSAGES/de.po
--rw-r--r--   0 runner    (1001) docker     (123)    56423 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/de/LC_MESSAGES/shared_wg_de.po
--rw-r--r--   0 runner    (1001) docker     (123)   107475 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/de/LC_MESSAGES/tabcmd.mo
--rw-r--r--   0 runner    (1001) docker     (123)   107842 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/de/LC_MESSAGES/tabcmd.po
--rw-r--r--   0 runner    (1001) docker     (123)    49134 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/de/LC_MESSAGES/tabcmd_messages_de.po
--rw-r--r--   0 runner    (1001) docker     (123)    47749 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/de/shared_wg_de.properties
--rw-r--r--   0 runner    (1001) docker     (123)    41636 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/de/tabcmd_messages_de.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.668636 tabcmd-2.0.8/tabcmd/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.668636 tabcmd-2.0.8/tabcmd/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/en/LC_MESSAGES/en-US.po
--rw-r--r--   0 runner    (1001) docker     (123)    49184 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/en/LC_MESSAGES/shared_wg_en.po
--rw-r--r--   0 runner    (1001) docker     (123)    89267 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/en/LC_MESSAGES/tabcmd.mo
--rw-r--r--   0 runner    (1001) docker     (123)    94193 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/en/LC_MESSAGES/tabcmd.po
--rw-r--r--   0 runner    (1001) docker     (123)    42162 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/en/LC_MESSAGES/tabcmd_messages_en.po
--rw-r--r--   0 runner    (1001) docker     (123)    40435 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/en/shared_wg_en.properties
--rw-r--r--   0 runner    (1001) docker     (123)    34960 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/en/tabcmd_messages_en.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.668636 tabcmd-2.0.8/tabcmd/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.668636 tabcmd-2.0.8/tabcmd/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/es/LC_MESSAGES/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/es/LC_MESSAGES/es.po
--rw-r--r--   0 runner    (1001) docker     (123)    54744 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/es/LC_MESSAGES/shared_wg_es.po
--rw-r--r--   0 runner    (1001) docker     (123)   104863 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/es/LC_MESSAGES/tabcmd.mo
--rw-r--r--   0 runner    (1001) docker     (123)   105231 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/es/LC_MESSAGES/tabcmd.po
--rw-r--r--   0 runner    (1001) docker     (123)    48201 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/es/LC_MESSAGES/tabcmd_messages_es.po
--rw-r--r--   0 runner    (1001) docker     (123)    46047 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/es/shared_wg_es.properties
--rw-r--r--   0 runner    (1001) docker     (123)    40679 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/es/tabcmd_messages_es.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.668636 tabcmd-2.0.8/tabcmd/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.668636 tabcmd-2.0.8/tabcmd/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/fr/LC_MESSAGES/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/fr/LC_MESSAGES/fr.po
--rw-r--r--   0 runner    (1001) docker     (123)    56049 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/fr/LC_MESSAGES/shared_wg_fr.po
--rw-r--r--   0 runner    (1001) docker     (123)   106904 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/fr/LC_MESSAGES/tabcmd.mo
--rw-r--r--   0 runner    (1001) docker     (123)   107271 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/fr/LC_MESSAGES/tabcmd.po
--rw-r--r--   0 runner    (1001) docker     (123)    48937 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/fr/LC_MESSAGES/tabcmd_messages_fr.po
--rw-r--r--   0 runner    (1001) docker     (123)    47362 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/fr/shared_wg_fr.properties
--rw-r--r--   0 runner    (1001) docker     (123)    41417 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/fr/tabcmd_messages_fr.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.668636 tabcmd-2.0.8/tabcmd/locales/ga/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.672636 tabcmd-2.0.8/tabcmd/locales/ga/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ga/LC_MESSAGES/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ga/LC_MESSAGES/ga.po
--rw-r--r--   0 runner    (1001) docker     (123)    65255 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ga/LC_MESSAGES/shared_wg_ga.po
--rw-r--r--   0 runner    (1001) docker     (123)   124810 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ga/LC_MESSAGES/tabcmd.mo
--rw-r--r--   0 runner    (1001) docker     (123)   125165 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ga/LC_MESSAGES/tabcmd.po
--rw-r--r--   0 runner    (1001) docker     (123)    57625 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ga/LC_MESSAGES/tabcmd_messages_ga.po
--rw-r--r--   0 runner    (1001) docker     (123)    56777 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ga/shared_wg_ga.properties
--rw-r--r--   0 runner    (1001) docker     (123)    50105 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ga/tabcmd_messages_ga.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.672636 tabcmd-2.0.8/tabcmd/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.672636 tabcmd-2.0.8/tabcmd/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/it/LC_MESSAGES/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/it/LC_MESSAGES/it.po
--rw-r--r--   0 runner    (1001) docker     (123)    54914 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/it/LC_MESSAGES/shared_wg_it.po
--rw-r--r--   0 runner    (1001) docker     (123)   104631 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/it/LC_MESSAGES/tabcmd.mo
--rw-r--r--   0 runner    (1001) docker     (123)   104998 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/it/LC_MESSAGES/tabcmd.po
--rw-r--r--   0 runner    (1001) docker     (123)    47799 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/it/LC_MESSAGES/tabcmd_messages_it.po
--rw-r--r--   0 runner    (1001) docker     (123)    46190 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/it/shared_wg_it.properties
--rw-r--r--   0 runner    (1001) docker     (123)    40279 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/it/tabcmd_messages_it.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.672636 tabcmd-2.0.8/tabcmd/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.672636 tabcmd-2.0.8/tabcmd/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ja/LC_MESSAGES/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ja/LC_MESSAGES/ja.po
--rw-r--r--   0 runner    (1001) docker     (123)    60517 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ja/LC_MESSAGES/shared_wg_ja.po
--rw-r--r--   0 runner    (1001) docker     (123)   117650 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ja/LC_MESSAGES/tabcmd.mo
--rw-r--r--   0 runner    (1001) docker     (123)   118017 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ja/LC_MESSAGES/tabcmd.po
--rw-r--r--   0 runner    (1001) docker     (123)    55215 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ja/LC_MESSAGES/tabcmd_messages_ja.po
--rw-r--r--   0 runner    (1001) docker     (123)    51979 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ja/shared_wg_ja.properties
--rw-r--r--   0 runner    (1001) docker     (123)    47693 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ja/tabcmd_messages_ja.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.672636 tabcmd-2.0.8/tabcmd/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.676636 tabcmd-2.0.8/tabcmd/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ko/LC_MESSAGES/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ko/LC_MESSAGES/ko.po
--rw-r--r--   0 runner    (1001) docker     (123)    55995 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ko/LC_MESSAGES/shared_wg_ko.po
--rw-r--r--   0 runner    (1001) docker     (123)   107787 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ko/LC_MESSAGES/tabcmd.mo
--rw-r--r--   0 runner    (1001) docker     (123)   108156 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ko/LC_MESSAGES/tabcmd.po
--rw-r--r--   0 runner    (1001) docker     (123)    49874 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ko/LC_MESSAGES/tabcmd_messages_ko.po
--rw-r--r--   0 runner    (1001) docker     (123)    47357 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ko/shared_wg_ko.properties
--rw-r--r--   0 runner    (1001) docker     (123)    42352 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/ko/tabcmd_messages_ko.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.676636 tabcmd-2.0.8/tabcmd/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.676636 tabcmd-2.0.8/tabcmd/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/pt/LC_MESSAGES/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/pt/LC_MESSAGES/pt.po
--rw-r--r--   0 runner    (1001) docker     (123)    54338 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/pt/LC_MESSAGES/shared_wg_pt.po
--rw-r--r--   0 runner    (1001) docker     (123)   102596 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/pt/LC_MESSAGES/tabcmd.mo
--rw-r--r--   0 runner    (1001) docker     (123)   102963 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/pt/LC_MESSAGES/tabcmd.po
--rw-r--r--   0 runner    (1001) docker     (123)    46340 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/pt/LC_MESSAGES/tabcmd_messages_pt.po
--rw-r--r--   0 runner    (1001) docker     (123)    45631 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/pt/shared_wg_pt.properties
--rw-r--r--   0 runner    (1001) docker     (123)    38818 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/pt/tabcmd_messages_pt.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.676636 tabcmd-2.0.8/tabcmd/locales/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.676636 tabcmd-2.0.8/tabcmd/locales/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/sv/LC_MESSAGES/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)    52464 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/sv/LC_MESSAGES/shared_wg_sv.po
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/sv/LC_MESSAGES/sv.po
--rw-r--r--   0 runner    (1001) docker     (123)   100092 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/sv/LC_MESSAGES/tabcmd.mo
--rw-r--r--   0 runner    (1001) docker     (123)   100459 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/sv/LC_MESSAGES/tabcmd.po
--rw-r--r--   0 runner    (1001) docker     (123)    45710 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/sv/LC_MESSAGES/tabcmd_messages_sv.po
--rw-r--r--   0 runner    (1001) docker     (123)    43754 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/sv/shared_wg_sv.properties
--rw-r--r--   0 runner    (1001) docker     (123)    38190 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/sv/tabcmd_messages_sv.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.676636 tabcmd-2.0.8/tabcmd/locales/zh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.680636 tabcmd-2.0.8/tabcmd/locales/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/zh/LC_MESSAGES/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)    47568 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/zh/LC_MESSAGES/shared_wg_zh.po
--rw-r--r--   0 runner    (1001) docker     (123)    90198 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/zh/LC_MESSAGES/tabcmd.mo
--rw-r--r--   0 runner    (1001) docker     (123)    90565 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/zh/LC_MESSAGES/tabcmd.po
--rw-r--r--   0 runner    (1001) docker     (123)    40712 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/zh/LC_MESSAGES/tabcmd_messages_zh.po
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/zh/LC_MESSAGES/zh.po
--rw-r--r--   0 runner    (1001) docker     (123)    38897 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/zh/shared_wg_zh.properties
--rw-r--r--   0 runner    (1001) docker     (123)    33190 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/locales/zh/tabcmd_messages_zh.properties
--rw-r--r--   0 runner    (1001) docker     (123)      678 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd/tabcmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd-linux.spec
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd-mac.spec
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd-windows.spec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.660636 tabcmd-2.0.8/tabcmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2022-12-08 22:41:05.000000 tabcmd-2.0.8/tabcmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2022-12-08 22:41:05.000000 tabcmd-2.0.8/tabcmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 22:41:05.000000 tabcmd-2.0.8/tabcmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-08 22:41:05.000000 tabcmd-2.0.8/tabcmd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      352 2022-12-08 22:41:05.000000 tabcmd-2.0.8/tabcmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-08 22:41:05.000000 tabcmd-2.0.8/tabcmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tabcmd.spec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.680636 tabcmd-2.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.680636 tabcmd-2.0.8/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/assets/SampleDS.tds
--rw-r--r--   0 runner    (1001) docker     (123)    22544 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/assets/World Indicators.tds
--rw-r--r--   0 runner    (1001) docker     (123)    64084 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/assets/World Indicators.tdsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.680636 tabcmd-2.0.8/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/commands/test_credential_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/commands/test_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/commands/test_geturl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/commands/test_localize.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/commands/test_projects_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15834 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/commands/test_run_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/commands/test_server_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    15625 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/commands/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/commands/test_user_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.680636 tabcmd-2.0.8/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/e2e/language_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/e2e/online_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/e2e/setup_e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/e2e/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/e2e/tests_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:41:05.684636 tabcmd-2.0.8/tests/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/common_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_login_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_logout_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_add_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_create_extracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_create_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_create_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_create_site.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_create_site_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_create_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_decrypt_extracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_delete_extracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_delete_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_delete_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_delete_site.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_delete_site_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_edit_site.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_encrypt_extracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_get_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_list_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_publish_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_reencrypt_extracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_refresh_extracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_remove_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2022-12-08 22:40:39.000000 tabcmd-2.0.8/tests/parsers/test_parser_runschedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.901852 tabcmd-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    69632 2022-12-16 07:15:59.000000 tabcmd-2.0.9/.coverage
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-16 07:15:59.000000 tabcmd-2.0.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.849851 tabcmd-2.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2022-12-16 07:15:59.000000 tabcmd-2.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.849851 tabcmd-2.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2022-12-16 07:15:59.000000 tabcmd-2.0.9/.github/workflows/check-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2022-12-16 07:15:59.000000 tabcmd-2.0.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2022-12-16 07:15:59.000000 tabcmd-2.0.9/.github/workflows/generate-metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2022-12-16 07:15:59.000000 tabcmd-2.0.9/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2022-12-16 07:15:59.000000 tabcmd-2.0.9/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2022-12-16 07:15:59.000000 tabcmd-2.0.9/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2022-12-16 07:15:59.000000 tabcmd-2.0.9/.github/workflows/run-e2-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2022-12-16 07:15:59.000000 tabcmd-2.0.9/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2022-12-16 07:15:59.000000 tabcmd-2.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2022-12-16 07:15:59.000000 tabcmd-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2022-12-16 07:16:26.901852 tabcmd-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2022-12-16 07:15:59.000000 tabcmd-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-16 07:15:59.000000 tabcmd-2.0.9/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2022-12-16 07:15:59.000000 tabcmd-2.0.9/World Indicators.tdsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.849851 tabcmd-2.0.9/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2022-12-16 07:15:59.000000 tabcmd-2.0.9/bin/coverage.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.849851 tabcmd-2.0.9/bin/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2022-12-16 07:15:59.000000 tabcmd-2.0.9/bin/i18n/makelocalealias.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7660 2022-12-16 07:15:59.000000 tabcmd-2.0.9/bin/i18n/msgfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2022-12-16 07:15:59.000000 tabcmd-2.0.9/bin/i18n/prop2po.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24195 2022-12-16 07:15:59.000000 tabcmd-2.0.9/bin/i18n/pygettext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2022-12-16 07:15:59.000000 tabcmd-2.0.9/bin/license-checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-16 07:15:59.000000 tabcmd-2.0.9/bin/pyinstaller.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2022-12-16 07:15:59.000000 tabcmd-2.0.9/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2022-12-16 07:15:59.000000 tabcmd-2.0.9/dodo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2022-12-16 07:15:59.000000 tabcmd-2.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.853851 tabcmd-2.0.9/res/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-16 07:15:59.000000 tabcmd-2.0.9/res/metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    28088 2022-12-16 07:15:59.000000 tabcmd-2.0.9/res/tabcmd.icns
+-rw-r--r--   0 runner    (1001) docker     (123)   197222 2022-12-16 07:15:59.000000 tabcmd-2.0.9/res/tabcmd.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2022-12-16 07:15:59.000000 tabcmd-2.0.9/res/tabcmd.png
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-16 07:16:26.901852 tabcmd-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-16 07:15:59.000000 tabcmd-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.853851 tabcmd-2.0.9/tabcmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.853851 tabcmd-2.0.9/tabcmd/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.853851 tabcmd-2.0.9/tabcmd/commands/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/auth/login_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/auth/logout_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17170 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/auth/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.857851 tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/datasources_and_workbooks_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/delete_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/export_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12456 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/get_url_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/publish_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/runschedule_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.857851 tabcmd-2.0.9/tabcmd/commands/extracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/extracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/extracts/create_extracts_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/extracts/decrypt_extracts_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/extracts/delete_extracts_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/extracts/encrypt_extracts_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/extracts/reencrypt_extracts_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/extracts/refresh_extracts_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.857851 tabcmd-2.0.9/tabcmd/commands/group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/group/create_group_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/group/delete_group_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.857851 tabcmd-2.0.9/tabcmd/commands/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/project/create_project_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/project/delete_project_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/project/publish_samples_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.861851 tabcmd-2.0.9/tabcmd/commands/site/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/site/create_site_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/site/delete_site_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/site/edit_site_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/site/list_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/site/list_sites_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.865851 tabcmd-2.0.9/tabcmd/commands/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/user/add_users_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/user/create_site_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/user/create_users_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/user/delete_site_users_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/user/remove_users_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12208 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/commands/user/user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.865851 tabcmd-2.0.9/tabcmd/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/execution/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/execution/global_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/execution/localize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/execution/logger_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/execution/map_of_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/execution/parent_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/execution/tabcmd_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.845851 tabcmd-2.0.9/tabcmd/locales/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.865851 tabcmd-2.0.9/tabcmd/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.869851 tabcmd-2.0.9/tabcmd/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/de/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/de/LC_MESSAGES/de.po
+-rw-r--r--   0 runner    (1001) docker     (123)    56423 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/de/LC_MESSAGES/shared_wg_de.po
+-rw-r--r--   0 runner    (1001) docker     (123)   107475 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/de/LC_MESSAGES/tabcmd.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   107842 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/de/LC_MESSAGES/tabcmd.po
+-rw-r--r--   0 runner    (1001) docker     (123)    49134 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/de/LC_MESSAGES/tabcmd_messages_de.po
+-rw-r--r--   0 runner    (1001) docker     (123)    47749 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/de/shared_wg_de.properties
+-rw-r--r--   0 runner    (1001) docker     (123)    41636 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/de/tabcmd_messages_de.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.869851 tabcmd-2.0.9/tabcmd/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.869851 tabcmd-2.0.9/tabcmd/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/en/LC_MESSAGES/en-US.po
+-rw-r--r--   0 runner    (1001) docker     (123)    49184 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/en/LC_MESSAGES/shared_wg_en.po
+-rw-r--r--   0 runner    (1001) docker     (123)    89267 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/en/LC_MESSAGES/tabcmd.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    93255 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/en/LC_MESSAGES/tabcmd.po
+-rw-r--r--   0 runner    (1001) docker     (123)    42162 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/en/LC_MESSAGES/tabcmd_messages_en.po
+-rw-r--r--   0 runner    (1001) docker     (123)    40435 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/en/shared_wg_en.properties
+-rw-r--r--   0 runner    (1001) docker     (123)    34960 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/en/tabcmd_messages_en.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.869851 tabcmd-2.0.9/tabcmd/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.873851 tabcmd-2.0.9/tabcmd/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/es/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/es/LC_MESSAGES/es.po
+-rw-r--r--   0 runner    (1001) docker     (123)    54744 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/es/LC_MESSAGES/shared_wg_es.po
+-rw-r--r--   0 runner    (1001) docker     (123)   104863 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/es/LC_MESSAGES/tabcmd.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   105231 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/es/LC_MESSAGES/tabcmd.po
+-rw-r--r--   0 runner    (1001) docker     (123)    48201 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/es/LC_MESSAGES/tabcmd_messages_es.po
+-rw-r--r--   0 runner    (1001) docker     (123)    46047 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/es/shared_wg_es.properties
+-rw-r--r--   0 runner    (1001) docker     (123)    40679 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/es/tabcmd_messages_es.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.873851 tabcmd-2.0.9/tabcmd/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.873851 tabcmd-2.0.9/tabcmd/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/fr/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/fr/LC_MESSAGES/fr.po
+-rw-r--r--   0 runner    (1001) docker     (123)    56049 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/fr/LC_MESSAGES/shared_wg_fr.po
+-rw-r--r--   0 runner    (1001) docker     (123)   106904 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/fr/LC_MESSAGES/tabcmd.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   107271 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/fr/LC_MESSAGES/tabcmd.po
+-rw-r--r--   0 runner    (1001) docker     (123)    48937 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/fr/LC_MESSAGES/tabcmd_messages_fr.po
+-rw-r--r--   0 runner    (1001) docker     (123)    47362 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/fr/shared_wg_fr.properties
+-rw-r--r--   0 runner    (1001) docker     (123)    41417 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/fr/tabcmd_messages_fr.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.873851 tabcmd-2.0.9/tabcmd/locales/ga/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.877852 tabcmd-2.0.9/tabcmd/locales/ga/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ga/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ga/LC_MESSAGES/ga.po
+-rw-r--r--   0 runner    (1001) docker     (123)    65255 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ga/LC_MESSAGES/shared_wg_ga.po
+-rw-r--r--   0 runner    (1001) docker     (123)   124810 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ga/LC_MESSAGES/tabcmd.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   125165 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ga/LC_MESSAGES/tabcmd.po
+-rw-r--r--   0 runner    (1001) docker     (123)    57625 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ga/LC_MESSAGES/tabcmd_messages_ga.po
+-rw-r--r--   0 runner    (1001) docker     (123)    56777 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ga/shared_wg_ga.properties
+-rw-r--r--   0 runner    (1001) docker     (123)    50105 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ga/tabcmd_messages_ga.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.877852 tabcmd-2.0.9/tabcmd/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.877852 tabcmd-2.0.9/tabcmd/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/it/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/it/LC_MESSAGES/it.po
+-rw-r--r--   0 runner    (1001) docker     (123)    54914 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/it/LC_MESSAGES/shared_wg_it.po
+-rw-r--r--   0 runner    (1001) docker     (123)   104631 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/it/LC_MESSAGES/tabcmd.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   104998 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/it/LC_MESSAGES/tabcmd.po
+-rw-r--r--   0 runner    (1001) docker     (123)    47799 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/it/LC_MESSAGES/tabcmd_messages_it.po
+-rw-r--r--   0 runner    (1001) docker     (123)    46190 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/it/shared_wg_it.properties
+-rw-r--r--   0 runner    (1001) docker     (123)    40279 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/it/tabcmd_messages_it.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.877852 tabcmd-2.0.9/tabcmd/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.881852 tabcmd-2.0.9/tabcmd/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ja/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ja/LC_MESSAGES/ja.po
+-rw-r--r--   0 runner    (1001) docker     (123)    60517 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ja/LC_MESSAGES/shared_wg_ja.po
+-rw-r--r--   0 runner    (1001) docker     (123)   117650 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ja/LC_MESSAGES/tabcmd.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   118017 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ja/LC_MESSAGES/tabcmd.po
+-rw-r--r--   0 runner    (1001) docker     (123)    55215 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ja/LC_MESSAGES/tabcmd_messages_ja.po
+-rw-r--r--   0 runner    (1001) docker     (123)    51979 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ja/shared_wg_ja.properties
+-rw-r--r--   0 runner    (1001) docker     (123)    47693 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ja/tabcmd_messages_ja.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.881852 tabcmd-2.0.9/tabcmd/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.885852 tabcmd-2.0.9/tabcmd/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ko/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ko/LC_MESSAGES/ko.po
+-rw-r--r--   0 runner    (1001) docker     (123)    55995 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ko/LC_MESSAGES/shared_wg_ko.po
+-rw-r--r--   0 runner    (1001) docker     (123)   107787 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ko/LC_MESSAGES/tabcmd.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   108156 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ko/LC_MESSAGES/tabcmd.po
+-rw-r--r--   0 runner    (1001) docker     (123)    49874 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ko/LC_MESSAGES/tabcmd_messages_ko.po
+-rw-r--r--   0 runner    (1001) docker     (123)    47357 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ko/shared_wg_ko.properties
+-rw-r--r--   0 runner    (1001) docker     (123)    42352 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/ko/tabcmd_messages_ko.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.885852 tabcmd-2.0.9/tabcmd/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.885852 tabcmd-2.0.9/tabcmd/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/pt/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/pt/LC_MESSAGES/pt.po
+-rw-r--r--   0 runner    (1001) docker     (123)    54338 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/pt/LC_MESSAGES/shared_wg_pt.po
+-rw-r--r--   0 runner    (1001) docker     (123)   102596 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/pt/LC_MESSAGES/tabcmd.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   102963 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/pt/LC_MESSAGES/tabcmd.po
+-rw-r--r--   0 runner    (1001) docker     (123)    46340 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/pt/LC_MESSAGES/tabcmd_messages_pt.po
+-rw-r--r--   0 runner    (1001) docker     (123)    45631 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/pt/shared_wg_pt.properties
+-rw-r--r--   0 runner    (1001) docker     (123)    38818 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/pt/tabcmd_messages_pt.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.885852 tabcmd-2.0.9/tabcmd/locales/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.889852 tabcmd-2.0.9/tabcmd/locales/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/sv/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)    52464 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/sv/LC_MESSAGES/shared_wg_sv.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/sv/LC_MESSAGES/sv.po
+-rw-r--r--   0 runner    (1001) docker     (123)   100092 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/sv/LC_MESSAGES/tabcmd.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   100459 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/sv/LC_MESSAGES/tabcmd.po
+-rw-r--r--   0 runner    (1001) docker     (123)    45710 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/sv/LC_MESSAGES/tabcmd_messages_sv.po
+-rw-r--r--   0 runner    (1001) docker     (123)    43754 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/sv/shared_wg_sv.properties
+-rw-r--r--   0 runner    (1001) docker     (123)    38190 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/sv/tabcmd_messages_sv.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.889852 tabcmd-2.0.9/tabcmd/locales/zh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.889852 tabcmd-2.0.9/tabcmd/locales/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/zh/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)    47568 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/zh/LC_MESSAGES/shared_wg_zh.po
+-rw-r--r--   0 runner    (1001) docker     (123)    90198 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/zh/LC_MESSAGES/tabcmd.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    90565 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/zh/LC_MESSAGES/tabcmd.po
+-rw-r--r--   0 runner    (1001) docker     (123)    40712 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/zh/LC_MESSAGES/tabcmd_messages_zh.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/zh/LC_MESSAGES/zh.po
+-rw-r--r--   0 runner    (1001) docker     (123)    38897 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/zh/shared_wg_zh.properties
+-rw-r--r--   0 runner    (1001) docker     (123)    33190 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/locales/zh/tabcmd_messages_zh.properties
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd/tabcmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd-linux.spec
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd-mac.spec
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd-windows.spec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.853851 tabcmd-2.0.9/tabcmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2022-12-16 07:16:26.000000 tabcmd-2.0.9/tabcmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2022-12-16 07:16:26.000000 tabcmd-2.0.9/tabcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 07:16:26.000000 tabcmd-2.0.9/tabcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-16 07:16:26.000000 tabcmd-2.0.9/tabcmd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2022-12-16 07:16:26.000000 tabcmd-2.0.9/tabcmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-16 07:16:26.000000 tabcmd-2.0.9/tabcmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tabcmd.spec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.889852 tabcmd-2.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.893852 tabcmd-2.0.9/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/assets/SampleDS.tds
+-rw-r--r--   0 runner    (1001) docker     (123)    22544 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/assets/World Indicators.tds
+-rw-r--r--   0 runner    (1001) docker     (123)    64084 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/assets/World Indicators.tdsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.893852 tabcmd-2.0.9/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/commands/test_credential_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/commands/test_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/commands/test_geturl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/commands/test_localize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/commands/test_projects_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/commands/test_run_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/commands/test_server_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/commands/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/commands/test_user_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.897852 tabcmd-2.0.9/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/e2e/language_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/e2e/online_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/e2e/setup_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/e2e/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/e2e/tests_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 07:16:26.901852 tabcmd-2.0.9/tests/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/common_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_login_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_logout_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_add_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_create_extracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_create_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_create_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_create_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_create_site_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_create_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_decrypt_extracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_delete_extracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_delete_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_delete_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_delete_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_delete_site_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_edit_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_encrypt_extracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_list_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_publish_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_reencrypt_extracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_refresh_extracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_remove_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2022-12-16 07:15:59.000000 tabcmd-2.0.9/tests/parsers/test_parser_runschedule.py
```

### Comparing `tabcmd-2.0.8/.coverage` & `tabcmd-2.0.9/.coverage`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/.github/dependabot.yml` & `tabcmd-2.0.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/.github/workflows/check-coverage.yml` & `tabcmd-2.0.9/.github/workflows/check-coverage.yml`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/.github/workflows/codeql-analysis.yml` & `tabcmd-2.0.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/.github/workflows/generate-metadata.yml` & `tabcmd-2.0.9/.github/workflows/generate-metadata.yml`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/.github/workflows/package.yml` & `tabcmd-2.0.9/.github/workflows/package.yml`

 * *Files 20% similar despite different names*

```diff
@@ -22,31 +22,30 @@
       fail-fast: false
       matrix:
         include:
           - os: windows-latest
             TARGET: windows
             CMD_BUILD: >
               pyinstaller tabcmd-windows.spec --clean --noconfirm --distpath ./dist/windows
-            OUT_FILE_NAME: tabcmd-windows.exe
+            OUT_FILE_NAME: tabcmd.exe
             ASSET_MIME: application/vnd.microsoft.portable-executable
           - os: macos-latest
             TARGET: macos
             CMD_BUILD:  >
-              pyinstaller tabcmd-mac.spec --clean --noconfirm --distpath ./dist/macos && ls && ls dist
-            # zip -r9 mac tabcmd-mac*
-            OUT_FILE_NAME: tabcmd-mac.app  # tabcmd.zip
+              pyinstaller tabcmd-mac.spec --clean --noconfirm --distpath ./dist/macos
+            OUT_FILE_NAME: tabcmd.app
             ASSET_MIME: application/zip
           - os: ubuntu-latest
             TARGET: ubuntu
           # https://stackoverflow.com/questions/31259856
           # /how-to-create-an-executable-file-for-linux-machine-using-pyinstaller
             CMD_BUILD: >
-              pyinstaller --clean -y --distpath ./dist/linux tabcmd-linux.spec &&
-              chown -R --reference=. ./dist/linux
-            OUT_FILE_NAME: tab-for-linux
+              pyinstaller --clean -y --distpath ./dist/ubuntu tabcmd-linux.spec &&
+              chown -R --reference=. ./dist/ubuntu
+            OUT_FILE_NAME: tabcmd
 
     steps:
     - uses: actions/checkout@v3
 
     - uses: actions/setup-python@v4
       with:
         python-version: 3.8
@@ -60,16 +59,13 @@
         pip install .[package]
         doit version
         python -m build
 
     - name: Package with pyinstaller for ${{matrix.TARGET}}
       run: ${{matrix.CMD_BUILD}}
 
-    - name: Upload assets to release
-      uses: WebFreak001/upload-asset@v1.0.0
-      env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }} # automatically provided by github actions
-        OS: windows # a variable we use in the name pattern?
+    - name: Validate package for ${{matrix.TARGET}}
+      run: ./dist/${{ matrix.TARGET }}/${{matrix.OUT_FILE_NAME}}
+
+    - uses: actions/upload-artifact@v3
       with:
-        file: ./dist/${{ matrix.TARGET }}/tabcmd/${{ matrix.OUT_FILE_NAME}}
-        mime: ${{ matrix.ASSET_MIME}} # required by GitHub API
-        name: ${{ matrix.OUT_FILE_NAME}} # name pattern to upload the file as
+        path: ./dist/${{ matrix.TARGET }}/${{ matrix.OUT_FILE_NAME }}/
```

### Comparing `tabcmd-2.0.8/.github/workflows/publish-pypi.yml` & `tabcmd-2.0.9/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/.github/workflows/python-app.yml` & `tabcmd-2.0.9/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/.github/workflows/run-e2-tests.yml` & `tabcmd-2.0.9/.github/workflows/run-e2-tests.yml`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/.github/workflows/run-tests.yml` & `tabcmd-2.0.9/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/LICENSE` & `tabcmd-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/PKG-INFO` & `tabcmd-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabcmd
-Version: 2.0.8
+Version: 2.0.9
 Summary: A command line client for working with Tableau Server.
 Author-email: Tableau <github@tableau.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 Tableau
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tabcmd-2.0.8/README.md` & `tabcmd-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/World Indicators.tdsx` & `tabcmd-2.0.9/World Indicators.tdsx`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/bin/i18n/makelocalealias.py` & `tabcmd-2.0.9/bin/i18n/makelocalealias.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/bin/i18n/msgfmt.py` & `tabcmd-2.0.9/bin/i18n/msgfmt.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/bin/i18n/prop2po.py` & `tabcmd-2.0.9/bin/i18n/prop2po.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/bin/i18n/pygettext.py` & `tabcmd-2.0.9/bin/i18n/pygettext.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/bin/license-checker.py` & `tabcmd-2.0.9/bin/license-checker.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/contributing.md` & `tabcmd-2.0.9/contributing.md`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/dodo.py` & `tabcmd-2.0.9/dodo.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/pyproject.toml` & `tabcmd-2.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/res/tabcmd.icns` & `tabcmd-2.0.9/res/tabcmd.icns`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/res/tabcmd.ico` & `tabcmd-2.0.9/res/tabcmd.ico`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/res/tabcmd.png` & `tabcmd-2.0.9/res/tabcmd.png`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/auth/login_command.py` & `tabcmd-2.0.9/tabcmd/commands/auth/login_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/auth/logout_command.py` & `tabcmd-2.0.9/tabcmd/commands/auth/logout_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/auth/session.py` & `tabcmd-2.0.9/tabcmd/commands/auth/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import getpass
 import json
 import os
 
 import requests
 import tableauserverclient as TSC
+import urllib3
 from urllib3.exceptions import InsecureRequestWarning
 
 from tabcmd.commands.constants import Errors
 from tabcmd.execution.localize import _
 from tabcmd.execution.logger_config import log
 
 
@@ -70,15 +71,34 @@
         self.token_value = args.token_value or self.token_value
 
         self.no_prompt = args.no_prompt or self.no_prompt
         self.certificate = args.certificate or self.certificate
         self.no_certcheck = args.no_certcheck or self.no_certcheck
         self.no_proxy = args.no_proxy or self.no_proxy
         self.proxy = args.proxy or self.proxy
-        self.timeout = args.timeout or self.timeout
+        self.timeout = self.timeout_as_integer(self.logger, args.timeout, self.timeout)
+
+    @staticmethod
+    def timeout_as_integer(logger, option_1, option_2):
+        result = None
+        if option_1:
+            try:
+                result = int(option_1)
+            except Exception as anyE:
+                result = 0
+        if option_2 and (not result or result <= 0):
+            try:
+                result = int(option_2)
+            except Exception as anyE:
+                result = 0
+        if not option_1 and not option_2:
+            logger.debug(_("setsetting.status").format("timeout", "None"))
+        elif not result or result <= 0:
+            logger.warning(_("sessionoptions.errors.bad_timeout").format("--timeout", result))
+        return result or 0
 
     @staticmethod
     def _read_password_from_file(filename):
         credential = None
         with open(str(filename), "r") as file_contents:
             reader = file_contents.readlines()
             for row in reader:
@@ -104,15 +124,15 @@
             credentials = TSC.TableauAuth(self.username, password, site_id=self.site_name)
             self.last_login_using = "username"
             return credentials
         elif credential_type == Session.TOKEN_CRED_TYPE and self.token_name:
             credentials = self._create_new_token_credential()
             return credentials
         else:
-            Errors.exit_with_error(self.logger, "Couldn't find credentials")
+            Errors.exit_with_error(self.logger, _("session.errors.missing_arguments").format(""))
 
     def _create_new_token_credential(self):
         if self.token_value:
             token = self.token_value
         elif self.password_file:
             token = Session._read_password_from_file(self.password_file)
         elif self._allow_prompt():
@@ -123,39 +143,68 @@
         if self.token_name and token:
             credentials = TSC.PersonalAccessTokenAuth(self.token_name, token, site_id=self.site_name)
             self.last_login_using = "token"
             return credentials
         else:
             Errors.exit_with_error(self.logger, _("session.errors.missing_arguments").format("token name"))
 
-    def _set_connection_options(self):
+    def _set_connection_options(self) -> TSC.Server:
+        self.logger.debug("Setting up request options")
         # args still to be handled here:
         # proxy, --no-proxy,
         # cert
-        # timeout
         http_options = {}
         if self.no_certcheck:
-            http_options = {"verify": False}
-            requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
+            http_options["verify"] = False
+            urllib3.disable_warnings(category=InsecureRequestWarning)
+        if self.proxy:
+            # do we catch this error? "sessionoptions.errors.bad_proxy_format"
+            self.logger.debug("Setting proxy: ", self.proxy)
+        if self.timeout:
+            http_options["timeout"] = self.timeout
         try:
-            tableau_server = TSC.Server(self.server_url, use_server_version=True, http_options=http_options)
+            self.logger.debug(http_options)
+            tableau_server = TSC.Server(self.server_url, http_options=http_options)
+
         except Exception as e:
+            self.logger.debug(
+                "Connection args: server {}, site {}, proxy {}, cert {}".format(
+                    self.server_url, self.site_name, self.proxy, self.certificate
+                )
+            )
             Errors.exit_with_error(self.logger, "Failed to connect to server", e)
 
+        self.logger.debug("Finished setting up connection")
         return tableau_server
 
-    def _create_new_connection(self):
+    def _verify_server_connection_unauthed(self):
+        try:
+            self.tableau_server.use_server_version()
+        except requests.exceptions.ReadTimeout as timeout_error:
+            Errors.exit_with_error(
+                self.logger,
+                message="Timed out after {} seconds attempting to connect to server".format(self.timeout),
+                exception=timeout_error,
+            )
+        except requests.exceptions.RequestException as requests_error:
+            Errors.exit_with_error(
+                self.logger, message="Error attempting to connect to the server", exception=requests_error
+            )
+        except Exception as e:
+            Errors.exit_with_error(self.logger, exception=e)
+
+    def _create_new_connection(self) -> TSC.Server:
         self.logger.info(_("session.new_session"))
-        self.tableau_server = self._set_connection_options()
         self._print_server_info()
         self.logger.info(_("session.connecting"))
         try:
-            self.tableau_server.use_server_version()  # this will attempt to contact the server
+            self.tableau_server = self._set_connection_options()
         except Exception as e:
             Errors.exit_with_error(self.logger, "Failed to connect to server", e)
+        return self.tableau_server
 
     def _read_existing_state(self):
         if self._check_json():
             self._read_from_json()
 
     def _print_server_info(self):
         self.logger.info("=====   Server: {}".format(self.server_url))
@@ -164,28 +213,29 @@
         else:
             self.logger.info("=====   Token Name: {}".format(self.token_name))
         site_display_name = self.site_name or "Default Site"
         self.logger.info(_("dataconnections.classes.tableau_server_site") + ": {}".format(site_display_name))
 
     def _validate_existing_signin(self):
         self.logger.info(_("session.continuing_session"))
-        self.tableau_server = self._set_connection_options()
+        # when do these two messages show up? self.logger.info(_("session.auto_site_login"))
         try:
             if self.tableau_server and self.tableau_server.is_signed_in():
                 response = self.tableau_server.users.get_by_id(self.user_id)
                 self.logger.debug(response)
                 if response.status_code.startswith("200"):
                     return self.tableau_server
         except TSC.ServerResponseError as e:
             self.logger.info(_("publish.errors.unexpected_server_response"), e)
         except Exception as e:
             self.logger.info(_("errors.internal_error.request.message"), e)
         return None
 
-    def _sign_in(self, tableau_auth):
+    # server connection created, not yet logged in
+    def _sign_in(self, tableau_auth) -> TSC.Server:
         self.logger.debug(_("session.login") + self.server_url)
         self.logger.debug(_("listsites.output").format("", self.username or self.token_name, self.site_name))
         try:
             self.tableau_server.auth.sign_in(tableau_auth)  # it's the same call for token or user-pass
         except Exception as e:
             Errors.exit_with_error(self.logger, exception=e)
         try:
@@ -241,15 +291,16 @@
             self.logger.debug(signed_in_object)
             # or maybe we at least have the credentials saved
             if not signed_in_object:
                 credentials = self._get_saved_credentials()
 
         if credentials and not signed_in_object:
             # logging in, not using an existing session
-            self._create_new_connection()
+            self.tableau_server = self._create_new_connection()
+            self._verify_server_connection_unauthed()
             signed_in_object = self._sign_in(credentials)
 
         if not signed_in_object:
             message = "Run 'tabcmd login -h' for details on required arguments"
             Errors.exit_with_error(self.logger, _("session.errors.missing_arguments").format(message))
         if args.no_cookie:
             self._remove_json()
```

### Comparing `tabcmd-2.0.8/tabcmd/commands/constants.py` & `tabcmd-2.0.9/tabcmd/commands/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def is_expired_session(error):
         if hasattr(error, "code"):
             return error.code == Constants.invalid_credentials
 
     @staticmethod
     def is_resource_conflict(error):
         if hasattr(error, "code"):
-            return error.code.startswith(Constants.resource_conflict_general)
+            return error.code == Constants.source_already_exists
 
     @staticmethod
     def is_login_error(error):
         if hasattr(error, "code"):
             return error.code == Constants.login_error
 
     @staticmethod
@@ -82,11 +82,11 @@
             if Errors.is_expired_session(exception):
                 logger.error(_("session.errors.session_expired"))
                 # TODO: add session as an argument to this method
                 #  and add the full command line as a field in Session?
                 # "session.session_expired_login"))
                 # session.renew_session
                 return
-            if exception.code.startswith(Constants.source_not_found):
+            if exception.code == Constants.source_not_found:
                 logger.error(_("publish.errors.server_resource_not_found"), exception)
         else:
             logger.error(exception)
```

### Comparing `tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/datasources_and_workbooks_command.py` & `tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/datasources_and_workbooks_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/delete_command.py` & `tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/delete_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/export_command.py` & `tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/export_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
             "--pagelayout",
             choices=["landscape", "portrait"],
             type=str.lower,
             default=None,
             help="page orientation (landscape or portrait) of the exported PDF",
         )
         group.add_argument(
-
             "--pagesize",
             choices=[
                 pagesize.A3,
                 pagesize.A4,
                 pagesize.A5,
                 pagesize.B4,
                 pagesize.B5,
```

### Comparing `tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/get_url_command.py` & `tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/get_url_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,49 +42,58 @@
         logger.debug(_("tabcmd.launching"))
         session = Session()
         server = session.create_session(args)
         if " " in args.url:
             Errors.exit_with_error(logger, _("export.errors.white_space_workbook_view"))
 
         url = args.url.lstrip("/")  # strip opening / if present
+        content_type = GetUrl.evaluate_content_type(logger, url)
+        file_type = GetUrl.get_file_type_from_filename(logger, url, args.filename)
+
+        GetUrl.get_content_as_file(file_type, content_type, logger, args, server, url)
 
     ## this first set of methods is all parsing the url and file input from the user
 
     @staticmethod
     def evaluate_content_type(logger, url):
         # specify a view to get using "/views/<workbookname>/<viewname>.<extension>"
         # specify a workbook to get using "/workbooks/<workbookname>.<extension>".
         # specify a datasource to get using "/datasources/<datasourcename>.<extension>"
         content_type = ""
         for content_type in GetUrl.valid_content_types:
             if url.find(content_type) == 0:
                 return content_type
         Errors.exit_with_error(logger, message=_("get.errors.invalid_content_type").format(url))
 
-
     @staticmethod
     def explain_expected_url(logger, url: str, command: str):
         view_example = "/views/<workbookname>/<viewname>[.ext]"
         wb_example = "/workbooks/<workbookname>[.ext]"
         ds_example = "/datasources/<datasourcename[.ext]"
         # todo when strings are updated # message:str = _("export.errors.requires_resource_param").format(
         message = (
             "The ''{0}'' command requires a resource path in a specific format."
             "Given: {1}. Accepted values: {2}, {3}, {4}".format(command, url, view_example, wb_example, ds_example)
         )
         Errors.exit_with_error(logger, message)
 
     @staticmethod
-    def get_file_type_from_filename(logger, file_name, url):
+    def get_file_type_from_filename(logger, url, file_name):
+        logger.debug("Choosing between {}, {}".format(file_name, url))
         file_name = file_name or url
         logger.debug(_("get.options.file") + ": {}".format(file_name))
         type_of_file = GetUrl.get_file_extension(file_name)
 
-        if not type_of_file:
-            Errors.exit_with_error(logger, _("tabcmd.get.extension.not_found").format(file_name))
+        if not type_of_file and file_name is not None:
+            # check the url
+            backup = GetUrl.get_file_extension(url)
+            if backup is not None:
+                type_of_file = backup
+            else:
+                Errors.exit_with_error(logger, _("tabcmd.get.extension.not_found").format(file_name))
 
         logger.debug("filetype: {}".format(type_of_file))
         if type_of_file in ["pdf", "csv", "png", "twb", "twbx", "tdsx"]:
             return type_of_file
 
         Errors.exit_with_error(logger, _("tabcmd.get.extension.not_found").format(file_name))
 
@@ -130,22 +139,25 @@
         view_name = GetUrl.strip_query_params(view_name)
         view_name = GetUrl.get_name_without_possible_extension(view_name)
         return DatasourcesAndWorkbooks.get_view_url_from_names(workbook_name, view_name)
 
     @staticmethod
     def filename_from_args(file_argument, item_name, filetype):
         if file_argument is None:
-            file_argument = "{}.{}".format(item_name, filetype)
+            file_argument = item_name
+        if not file_argument.endswith(filetype):
+            file_argument = "{}.{}".format(file_argument, filetype)
         return file_argument
 
     ## methods below here have done all the parsing and just have to do the download and saving
     ## these should be able to be shared with export
 
     @staticmethod
     def get_content_as_file(file_type, content_type, logger, args, server, url):
+        logger.debug("fetching {} as {}".format(content_type, file_type))
         if content_type == "workbook":
             return GetUrl.generate_twb(logger, server, args, file_type, url)
         elif content_type == "datasource":
             return GetUrl.generate_tds(logger, server, args, file_type)
         elif content_type == "view":
             view_url = GetUrl.get_view_url(url, logger)
             if file_type == "pdf":
@@ -203,26 +215,32 @@
     def generate_twb(logger, server, args, file_extension, url):
         logger.trace("Entered method " + inspect.stack()[0].function)
         workbook_name = GetUrl.get_resource_name(url, logger)
         try:
             target_workbook = GetUrl.get_wb_by_content_url(logger, server, workbook_name)
             logger.debug(_("content_type.workbook") + ": {}".format(workbook_name))
             file_name_with_path = GetUrl.filename_from_args(args.filename, workbook_name, file_extension)
-            logger.debug("Saving as {}".format(file_name_with_path))
-            server.workbooks.download(target_workbook.id, filepath=None, no_extract=False)
-            logger.info(_("export.success").format(target_workbook.name, file_name_with_path))
+            # the download method will add an extension. How do I tell which one?
+            file_name_with_path = GetUrl.get_name_without_possible_extension(file_name_with_path)
+            file_name_with_ext = "{}.{}".format(file_name_with_path, file_extension)
+            logger.debug("Saving as {}".format(file_name_with_ext))
+            server.workbooks.download(target_workbook.id, filepath=file_name_with_path, no_extract=False)
+            logger.info(_("export.success").format(target_workbook.name, file_name_with_ext))
         except Exception as e:
             Errors.exit_with_error(logger, e)
 
     @staticmethod
     def generate_tds(logger, server, args, file_extension):
         logger.trace("Entered method " + inspect.stack()[0].function)
         datasource_name = GetUrl.get_resource_name(args.url, logger)
         try:
             target_datasource = GetUrl.get_ds_by_content_url(logger, server, datasource_name)
             logger.debug(_("content_type.datasource") + ": {}".format(datasource_name))
             file_name_with_path = GetUrl.filename_from_args(args.filename, datasource_name, file_extension)
-            logger.debug("Saving as {}".format(file_name_with_path))
-            server.datasources.download(target_datasource.id, filepath=None, no_extract=False)
-            logger.info(_("export.success").format(target_datasource.name, file_name_with_path))
+            # the download method will add an extension
+            file_name_with_path = GetUrl.get_name_without_possible_extension(file_name_with_path)
+            file_name_with_ext = "{}.{}".format(file_name_with_path, file_extension)
+            logger.debug("Saving as {}".format(file_name_with_ext))
+            server.datasources.download(target_datasource.id, filepath=file_name_with_path, no_extract=False)
+            logger.info(_("export.success").format(target_datasource.name, file_name_with_ext))
         except Exception as e:
             Errors.exit_with_error(logger, e)
```

### Comparing `tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/publish_command.py` & `tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/publish_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/datasources_and_workbooks/runschedule_command.py` & `tabcmd-2.0.9/tabcmd/commands/datasources_and_workbooks/runschedule_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/extracts/create_extracts_command.py` & `tabcmd-2.0.9/tabcmd/commands/extracts/create_extracts_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/extracts/decrypt_extracts_command.py` & `tabcmd-2.0.9/tabcmd/commands/extracts/decrypt_extracts_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/extracts/delete_extracts_command.py` & `tabcmd-2.0.9/tabcmd/commands/extracts/delete_extracts_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/extracts/encrypt_extracts_command.py` & `tabcmd-2.0.9/tabcmd/commands/extracts/encrypt_extracts_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/extracts/reencrypt_extracts_command.py` & `tabcmd-2.0.9/tabcmd/commands/extracts/reencrypt_extracts_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/extracts/refresh_extracts_command.py` & `tabcmd-2.0.9/tabcmd/commands/extracts/refresh_extracts_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/group/create_group_command.py` & `tabcmd-2.0.9/tabcmd/commands/group/create_group_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/group/delete_group_command.py` & `tabcmd-2.0.9/tabcmd/commands/group/delete_group_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/project/create_project_command.py` & `tabcmd-2.0.9/tabcmd/commands/project/create_project_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,20 @@
             except Exception as exc:
                 Errors.exit_with_error(logger, exc)
             readable_name = "{0}/{1}".format(args.parent_project_path, args.project_name)
             parent_id = parent.id
             logger.debug("parent project = `{0}`, id = {1}".format(args.parent_project_path, parent_id))
         logger.info(_("createproject.status").format(readable_name))
         new_project = TSC.ProjectItem(args.project_name, args.description, None, parent_id)
+        project_item = None
         try:
             project_item = server.projects.create(new_project)
             logger.info(_("common.output.succeeded"))
             return project_item
         except Exception as e:
             if Errors.is_resource_conflict(e) and args.continue_if_exists:
                 logger.info(_("tabcmd.result.already_exists").format(_("content_type.project"), args.project_name))
-                return
-            Errors.exit_with_error(logger, e)
+                logger.info(_("common.output.succeeded"))
+            else:
+                Errors.exit_with_error(logger, e)
+
+        return project_item
```

### Comparing `tabcmd-2.0.8/tabcmd/commands/project/delete_project_command.py` & `tabcmd-2.0.9/tabcmd/commands/project/delete_project_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/project/publish_samples_command.py` & `tabcmd-2.0.9/tabcmd/commands/project/publish_samples_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/server.py` & `tabcmd-2.0.9/tabcmd/commands/server.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/site/create_site_command.py` & `tabcmd-2.0.9/tabcmd/commands/site/create_site_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/site/delete_site_command.py` & `tabcmd-2.0.9/tabcmd/commands/site/delete_site_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/site/edit_site_command.py` & `tabcmd-2.0.9/tabcmd/commands/site/edit_site_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/site/list_command.py` & `tabcmd-2.0.9/tabcmd/commands/site/list_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/site/list_sites_command.py` & `tabcmd-2.0.9/tabcmd/commands/site/list_sites_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/user/add_users_command.py` & `tabcmd-2.0.9/tabcmd/commands/user/add_users_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/user/create_site_users.py` & `tabcmd-2.0.9/tabcmd/commands/user/create_site_users.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import tableauserverclient as TSC
 
 from tabcmd.commands.auth.session import Session
+from tabcmd.commands.constants import Errors
 from tabcmd.execution.global_options import *
 from tabcmd.execution.localize import _
 from tabcmd.execution.logger_config import log
 from .user_data import UserCommand
 
 
 class CreateSiteUsersCommand(UserCommand):
@@ -16,17 +17,18 @@
 
     name: str = "createsiteusers"
     description: str = _("createsiteusers.short_description")
 
     @staticmethod
     def define_args(create_site_users_parser):
         args_group = create_site_users_parser.add_argument_group(title=CreateSiteUsersCommand.name)
-        set_role_arg(args_group)
+        UserCommand.set_role_arg(args_group)
         set_users_file_positional(args_group)
         set_completeness_options(args_group)
+        UserCommand.set_auth_arg(args_group)
 
     @staticmethod
     def run_command(args):
         logger = log(__class__.__name__, args.logging_level)
         logger.debug(_("tabcmd.launching"))
         session = Session()
         server = session.create_session(args)
@@ -34,27 +36,37 @@
         number_of_users_added = 0
         number_of_errors = 0
 
         creation_site = "current site"
 
         UserCommand.validate_file_for_import(args.filename, logger, detailed=True, strict=args.require_all_valid)
 
-        logger.info(_("tabcmd.add.users.to_x").format(args.filename.name, creation_site))
+        logger.info(_("tabcmd.add.users.to_site").format(args.filename.name, creation_site))
         user_obj_list = UserCommand.get_users_from_file(args.filename, logger)
         logger.info(_("session.monitorjob.percent_complete").format(0))
         error_list = []
         for user_obj in user_obj_list:
             try:
+                if args.role:
+                    user_obj.site_role = args.role  # tsc is case sensitive
+                if args.auth_type:
+                    user_obj.auth_setting = args.auth_type
                 number_of_users_listed += 1
                 result = server.users.add(user_obj)
                 logger.info(_("tabcmd.result.success.create_user").format(user_obj.name))
                 number_of_users_added += 1
             except TSC.ServerResponseError as e:
-                number_of_errors += 1
-                error_list.append(e)
                 logger.debug(e)
+                if Errors.is_resource_conflict(e) and args.continue_if_exists:
+                    logger.debug(_("createsite.errors.site_name_already_exists").format(user_obj.name))
+                else:
+                    number_of_errors += 1
+                    logger.debug(number_of_errors)
+                    error_list.append(e.summary + ": " + e.detail)
+                logger.debug(error_list)
         logger.info(_("session.monitorjob.percent_complete").format(100))
         logger.info(_("importcsvsummary.line.processed").format(number_of_users_listed))
         logger.info(_("importcsvsummary.line.skipped").format(number_of_errors))
         logger.info(_("importcsvsummary.users.added.count").format(number_of_users_added))
         if number_of_errors > 0:
-            logger.info(_("importcsvsummary.error.details").format(error_list))
+            logger.info(_("importcsvsummary.error.details"))
+            logger.info(error_list)
```

### Comparing `tabcmd-2.0.8/tabcmd/commands/user/create_users_command.py` & `tabcmd-2.0.9/tabcmd/commands/user/delete_site_users_command.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,58 @@
-import tableauserverclient as TSC
-
 from tabcmd.commands.auth.session import Session
 from tabcmd.commands.constants import Errors
+from tabcmd.commands.server import Server
+from tabcmd.commands.user.user_data import UserCommand
 from tabcmd.execution.global_options import *
 from tabcmd.execution.localize import _
 from tabcmd.execution.logger_config import log
-from .user_data import UserCommand
 
 
-class CreateUsersCommand(UserCommand):
+class DeleteSiteUsersCommand(Server):
     """
-    Command to add users to a site, based on information supplied in a comma-separated values (CSV) file.
-    If the user is not already created on the server, the command creates the user before adding
-    that user to the site
+    Command to Remove users from the site that user is logged in to.
+    The users to be removed are specified in a file that contains
+    a simple list of one user name per line.
     """
 
-    name: str = "createUsers"
-    description: str = _("createusers.short_description")
+    name: str = "deletesiteusers"
+    description: str = _("deletesiteusers.short_description")
 
     @staticmethod
-    def define_args(create_users_parser):
-        args_group = create_users_parser.add_argument_group(title=CreateUsersCommand.name)
-        set_role_arg(args_group)
+    def define_args(delete_site_users_parser):
+        args_group = delete_site_users_parser.add_argument_group(title=DeleteSiteUsersCommand.name)
         set_users_file_positional(args_group)
         set_completeness_options(args_group)
 
     @staticmethod
     def run_command(args):
         logger = log(__class__.__name__, args.logging_level)
         logger.debug(_("tabcmd.launching"))
         session = Session()
         server = session.create_session(args)
-        number_of_users_listed = 0
-        number_of_users_added = 0
-        number_of_errors = 0
 
-        if args.site_name:
-            creation_site = args.site_name
-        else:
-            creation_site = "current site"
+        logger.info(_("deleteusers.status").format(args.filename.name))
 
-        UserCommand.validate_file_for_import(args.filename, logger, detailed=True, strict=args.require_all_valid)
-
-        logger.info(_("createusers.status").format(args.filename.name))
+        UserCommand.validate_file_for_import(args.filename, logger, strict=args.require_all_valid)
+        number_of_users_deleted = 0
+        number_of_errors = 0
         user_obj_list = UserCommand.get_users_from_file(args.filename, logger)
-        logger.info(_("session.monitorjob.percent_complete").format(0))
+
+        logger.debug("Users: {}".format(len(user_obj_list)))
+
         error_list = []
         for user_obj in user_obj_list:
+            logger.info(_("importcsvsummary.line.processed").format(number_of_users_deleted))
             try:
-                number_of_users_listed += 1
-                # TODO: bring in other attributes in file, actually act on specific site
-                new_user = TSC.UserItem(user_obj.name, args.role)
-                server.users.add(new_user)
-                logger.info(_("tabcmd.result.success.create_user").format(user_obj.name))
-                number_of_users_added += 1
+                user_id = UserCommand.find_user(logger, server, user_obj.name).id
+                server.users.remove(user_id)
+                logger.debug(_("tabcmd.result.success.delete_user").format(user_obj.name, user_id))
+                number_of_users_deleted += 1
             except Exception as e:
+                Errors.check_common_error_codes_and_explain(logger, e)
                 number_of_errors += 1
                 error_list.append(e)
-                logger.debug(e)
-        logger.info(_("session.monitorjob.percent_complete").format(100))
-        logger.info(_("importcsvsummary.line.processed").format(number_of_users_listed))
-        logger.info(_("importcsvsummary.line.skipped").format(number_of_errors))
-        logger.info(_("tabcmd.report.users_added").format(number_of_users_added))
+
+        logger.info(_("importcsvsummary.line.processed").format(number_of_users_deleted))
+        logger.info(_("importcsvsummary.errors.count").format(number_of_errors))
         if number_of_errors > 0:
-            logger.debug(_("tabcmd.report.errors").format(number_of_errors))
-        for exception in error_list:
-            Errors.check_common_error_codes_and_explain(logger, exception)
+            logger.info(_("importcsvsummary.error.details").format(error_list))
```

### Comparing `tabcmd-2.0.8/tabcmd/commands/user/remove_users_command.py` & `tabcmd-2.0.9/tabcmd/commands/user/remove_users_command.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/commands/user/user_data.py` & `tabcmd-2.0.9/tabcmd/commands/user/user_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import List, Callable, Optional
 
 import tableauserverclient as TSC
 
 from tabcmd.commands.constants import Errors
 from tabcmd.commands.server import Server
 from tabcmd.execution.localize import _
+from tabcmd.execution.global_options import case_insensitive_string_type
 
 
 class Userdata:
     def __init__(self):
         self.name = None
         self.password = None
         self.fullname = None
@@ -54,37 +55,77 @@
     [],
     [],
     [],
     ["creator", "explorer", "viewer", "unlicensed"],  # license
     ["system", "site", "none", "no"],  # admin
     ["yes", "true", "1", "no", "false", "0"],  # publisher
     [],
-    [TSC.UserItem.Auth.SAML, TSC.UserItem.Auth.OpenID, TSC.UserItem.Auth.ServerDefault],  # auth
 ]
 
+site_roles = [
+    "ServerAdministrator",
+    "SiteAdministratorCreator",
+    "SiteAdministratorExplorer",
+    "SiteAdministrator",
+    "Creator",
+    "ExplorerCanPublish",
+    "Publisher",
+    "Explorer",
+    "Interactor",
+    "Viewer",
+    "Unlicensed",
+]
+
+auth_types = ["Local", TSC.UserItem.Auth.SAML, TSC.UserItem.Auth.OpenID, TSC.UserItem.Auth.ServerDefault, "TableauId"]
+
 
 # username, password, display_name, license, admin_level, publishing, email, auth type
 class Column(IntEnum):
     USERNAME = 0
     PASS = 1
     DISPLAY_NAME = 2
     LICENSE = 3  # aka site role
     ADMIN = 4
     PUBLISHER = 5
     EMAIL = 6
-    AUTH = 7
 
-    MAX = 7
+    MAX = 7  # number of columns
 
 
 class UserCommand(Server):
     """
     This class acts as a base class for user related group of commands
     """
 
+    @staticmethod
+    def set_role_arg(parser):
+        parser.add_argument(
+            "-r",
+            "--role",
+            choices=site_roles,
+            type=case_insensitive_string_type(site_roles),
+            help="Specifies a site role for all users in the .csv file. Possible roles: " + ", ".join(site_roles),
+            metavar="SITE_ROLE",
+        )
+        return parser
+
+    @staticmethod
+    def set_auth_arg(parser):
+        parser.add_argument(
+            "--auth-type",
+            metavar="TYPE",
+            choices=auth_types,
+            type=case_insensitive_string_type(auth_types),
+            # default="TableauID",  # default is Local for on-prem, TableauID for Online. Does the server apply the default?
+            help="Assigns the authentication type for all users in the CSV file. \
+    For Tableau Online, TYPE may be TableauID (default) or SAML. \
+    For Tableau Server, TYPE may be Local (default) or SAML.",
+        )
+        return parser
+
     # read the file containing usernames or user details and validate each line
     # log out any errors encountered
     # returns the number of valid lines in the file
     # @param boolean strict: if true, die if any errors are found
     @staticmethod
     def validate_file_for_import(csv_file: io.TextIOWrapper, logger, detailed=False, strict=False) -> int:
         num_errors = 0
```

### Comparing `tabcmd-2.0.8/tabcmd/execution/global_options.py` & `tabcmd-2.0.9/tabcmd/execution/global_options.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,28 @@
 e.g add_argument(site, metavar='site-name')
 FOR site-name, project-name, workbook-name, datasource-name, group-name, schedule-name, token-name
 -> in args: site, project, workbook, ....
 BUT filename, username -> filename, username in command/parser
 
 """
 
+# argparse does case-sensitive comparisons of string inputs by default
+# I want the user to be able to enter e.g. "viewer" and have it accepted as "Viewer"
+# https://stackoverflow.com/questions/56838004/
+# case-insensitive-argparse-choices-without-losing-case-information-in-choices-lis
+def case_insensitive_string_type(choices):
+    def find_choice(choice):
+        for key, item in enumerate([choice.lower() for choice in choices]):
+            if choice.lower() == item:
+                return choices[key]
+        else:
+            return choice
+
+    return find_choice
+
 
 def set_parent_project_arg(parser):
     parser.add_argument("--parent-project-path", default=None, help="path of parent project")
     return parser
 
 
 # add/remove-user
@@ -61,41 +75,14 @@
         "--no-wait",
         action="store_true",
         help="Do not wait for asynchronous jobs to complete.",
     )
     return parser
 
 
-site_roles = [
-    "ServerAdministrator",
-    "SiteAdministratorCreator",
-    "SiteAdministratorExplorer",
-    "SiteAdministrator",
-    "Creator",
-    "ExplorerCanPublish",
-    "Publisher",
-    "Explorer",
-    "Interactor",
-    "Viewer",
-    "Unlicensed",
-]
-
-
-def set_role_arg(parser):
-    parser.add_argument(
-        "-r",
-        "--role",
-        choices=list(map(lambda x: x.lower(), site_roles)),
-        type=str.lower,
-        help="Specifies a site role for all users in the .csv file. Possible roles: " + ", ".join(site_roles),
-        metavar="SITE_ROLE",
-    )
-    return parser
-
-
 def set_silent_option(parser):
     parser.add_argument(
         "--silent-progress", action="store_true", help="Do not display progress messages for the command."
     )
     return parser
 
 
@@ -114,18 +101,18 @@
         help="Allows a change to succeed when not all rows are valid. If not specified --complete is used.",
     )
     completeness_group.set_defaults(require_all_valid=True)
     return parser
 
 
 # used in create/delete extract
-# docs don't say it, but --embedded-datasources and --include-all could be mutually exclusive
 def set_embedded_datasources_options(parser):
+    # one of these is required IFF we are using a workbook instead of datasource
     embedded_group = parser.add_mutually_exclusive_group()
-    embedded_group.add_argument(
+    embedded_group.add_argument(  # nargs?
         "--embedded-datasources",
         help="A space-separated list of embedded data source names within the target workbook.",
     )
     embedded_group.add_argument(
         "--include-all",
         action="store_true",
         help="Include all embedded data sources within target workbook.",
@@ -185,18 +172,20 @@
     target_type_group = parser.add_mutually_exclusive_group(required=False)
     target_type_group.add_argument("-d", "--datasource", action="store_true", help="The name of the target datasource.")
     target_type_group.add_argument("-w", "--workbook", action="store_true", help="The name of the target workbook.")
     return parser
 
 
 # pass arguments for either --datasource or --workbook
-def set_ds_xor_wb_args(parser):
+def set_ds_xor_wb_args(parser, url=False):
     target_type_group = parser.add_mutually_exclusive_group(required=True)
     target_type_group.add_argument("-d", "--datasource", help="The name of the target datasource.")
     target_type_group.add_argument("-w", "--workbook", help="The name of the target workbook.")
+    if url:
+        target_type_group.add_argument("--url", "-U", help=_("deleteextracts.options.url"))
     return parser
 
 
 def set_description_arg(parser):
     parser.add_argument("-d", "--description", help="Specifies a description for the item.")
     return parser
 
@@ -237,24 +226,25 @@
 
     parser.add_argument(
         "--storage-quota",
         type=int,
         help="In MB, the amount of data that can be stored on the site.",
     )
 
+    encryption_modes = ["enforced", "enabled", "disabled"]
     parser.add_argument(
         "--extract-encryption-mode",
-        choices=["enforced", "enabled", "disabled"],
+        choices=encryption_modes,
+        type=case_insensitive_string_type(encryption_modes),
         help="The extract encryption mode for the site can be enforced, enabled or disabled. ",
     )
 
     parser.add_argument(
         "--run-now-enabled",
         choices=["true", "false"],
-        type=str.lower,
         help="Allow or deny users from running extract refreshes, flows, or schedules manually.",
     )
     return parser
 
 
 def set_site_mode_option(parser):
     site_help = "Allows or denies site administrators the ability to add users to or remove users from the site."
@@ -328,14 +318,15 @@
     )
     thumbnails = parser.add_mutually_exclusive_group()
     thumbnails.add_argument("--thumbnail-username", help="Not yet implemented")
     thumbnails.add_argument("--thumbnail-group", help="Not yet implemented")  # not implemented in the REST API
 
     parser.add_argument("--use-tableau-bridge", action="store_true", help="Refresh datasource through Tableau Bridge")
 
+
 def set_overwrite_option(parser):
     append_group = parser.add_mutually_exclusive_group()
     append_group.add_argument(
         "-o",
         "--overwrite",
         action="store_true",
         help="Overwrites the workbook, data source, or data extract if it already exists on the server.",
@@ -401,19 +392,22 @@
 # set setting
 # choices: allow_scheduling, embedded_credentials, remember_passwords_forever
 # use !setting-name to disable them
 # hmmmm
 
 
 # sync-group
+license_modes = ["on-login", "on-sync"]
+
+
 def set_update_group_args(parser):
     parser.add_argument(
         "--grant-license-mode",
-        choices=["on-login", "on-sync"],
-        type=str.lower,
+        choices=license_modes,
+        type=case_insensitive_string_type(license_modes),
         help="Specifies whether a role should be granted on sign in. ",
     )
     parser.add_argument(
         "--overwritesiterole",
         action="store_true",
         help="Allows a user’s site role to be overwritten with a less privileged one when using --role.",
     )
```

### Comparing `tabcmd-2.0.8/tabcmd/execution/localize.py` & `tabcmd-2.0.9/tabcmd/execution/localize.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/execution/logger_config.py` & `tabcmd-2.0.9/tabcmd/execution/logger_config.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/execution/map_of_commands.py` & `tabcmd-2.0.9/tabcmd/execution/map_of_commands.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/execution/parent_parser.py` & `tabcmd-2.0.9/tabcmd/execution/parent_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         metavar="<SECONDS>",  # can't use -t, it's already used for --site
         help=_("session.options.timeout"),
     )
 
     # general behavioral options
     parser.add_argument(
         "--continue-if-exists",
-        action="store_false",
+        action="store_true",  # default behavior matches old tabcmd
         help=strings[9],
     )
 
     parser.add_argument(
         "--country",
         choices=["de", "en", "es", "fr", "it", "ja", "ko", "pt", "sv", "zh"],
         type=str.lower,  # coerce input to lowercase to act case insensitive
```

### Comparing `tabcmd-2.0.8/tabcmd/execution/tabcmd_controller.py` & `tabcmd-2.0.9/tabcmd/execution/tabcmd_controller.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/de/LC_MESSAGES/de.po` & `tabcmd-2.0.9/tabcmd/locales/de/LC_MESSAGES/de.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/de/LC_MESSAGES/shared_wg_de.po` & `tabcmd-2.0.9/tabcmd/locales/de/LC_MESSAGES/shared_wg_de.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/de/LC_MESSAGES/tabcmd.mo` & `tabcmd-2.0.9/tabcmd/locales/de/LC_MESSAGES/tabcmd.mo`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/de/LC_MESSAGES/tabcmd.po` & `tabcmd-2.0.9/tabcmd/locales/de/LC_MESSAGES/tabcmd.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/de/LC_MESSAGES/tabcmd_messages_de.po` & `tabcmd-2.0.9/tabcmd/locales/de/LC_MESSAGES/tabcmd_messages_de.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/de/shared_wg_de.properties` & `tabcmd-2.0.9/tabcmd/locales/de/shared_wg_de.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/de/tabcmd_messages_de.properties` & `tabcmd-2.0.9/tabcmd/locales/de/tabcmd_messages_de.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/en/LC_MESSAGES/en-US.po` & `tabcmd-2.0.9/tabcmd/locales/en/LC_MESSAGES/en-US.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/en/LC_MESSAGES/shared_wg_en.po` & `tabcmd-2.0.9/tabcmd/locales/en/LC_MESSAGES/shared_wg_en.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/en/LC_MESSAGES/tabcmd.mo` & `tabcmd-2.0.9/tabcmd/locales/en/LC_MESSAGES/tabcmd.mo`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/en/LC_MESSAGES/tabcmd.po` & `tabcmd-2.0.9/tabcmd/locales/en/LC_MESSAGES/tabcmd.po`

 * *Files 1% similar despite different names*

```diff
@@ -1851,38 +1851,14 @@
 msgstr "name cannot be empty"
 
 #:
 msgid "askdata.title"
 msgstr "Ask Data"
 
 #:
-msgid "slack.app.upgrade.email.notification.subject"
-msgstr "Tableau App for Slack Update"
-
-#:
-msgid "slack.app.upgrade.email.notification.introduction"
-msgstr "An update is available for the Tableau app for Slack and can be reinstalled now to work with the next Tableau Online release. Tableau recommends reinstalling the app to maintain app performance and use new features. Look for new features and changes in <a styl"
-
-#:
-msgid "slack.app.upgrade.email.notification.action"
-msgstr "For update and reinstallation steps, see <a styl"
-
-#:
-msgid "slack.app.upgrade.email.notification.steps"
-msgstr "This service notification has been published by Tableau Online."
-
-#:
-msgid "slack.app.upgrade.email.notification.reason"
-msgstr "You are receiving this notification because you are an administrator of a Tableau Online site connected to Slack."
-
-#:
-msgid "slack.app.upgrade.email.notification.footer.privacy"
-msgstr "Read our <a styl"
-
-#:
 msgid "unifiedconsumption.tcrm.folders.private"
 msgstr "My Private App"
 
 
 msgid ""
 msgstr ""
 "MIME-Version: 1.0"
```

### Comparing `tabcmd-2.0.8/tabcmd/locales/en/LC_MESSAGES/tabcmd_messages_en.po` & `tabcmd-2.0.9/tabcmd/locales/en/LC_MESSAGES/tabcmd_messages_en.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/en/shared_wg_en.properties` & `tabcmd-2.0.9/tabcmd/locales/en/shared_wg_en.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/en/tabcmd_messages_en.properties` & `tabcmd-2.0.9/tabcmd/locales/en/tabcmd_messages_en.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/es/LC_MESSAGES/es.po` & `tabcmd-2.0.9/tabcmd/locales/es/LC_MESSAGES/es.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/es/LC_MESSAGES/shared_wg_es.po` & `tabcmd-2.0.9/tabcmd/locales/es/LC_MESSAGES/shared_wg_es.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/es/LC_MESSAGES/tabcmd.mo` & `tabcmd-2.0.9/tabcmd/locales/es/LC_MESSAGES/tabcmd.mo`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/es/LC_MESSAGES/tabcmd.po` & `tabcmd-2.0.9/tabcmd/locales/es/LC_MESSAGES/tabcmd.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/es/LC_MESSAGES/tabcmd_messages_es.po` & `tabcmd-2.0.9/tabcmd/locales/es/LC_MESSAGES/tabcmd_messages_es.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/es/shared_wg_es.properties` & `tabcmd-2.0.9/tabcmd/locales/es/shared_wg_es.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/es/tabcmd_messages_es.properties` & `tabcmd-2.0.9/tabcmd/locales/es/tabcmd_messages_es.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/fr/LC_MESSAGES/fr.po` & `tabcmd-2.0.9/tabcmd/locales/fr/LC_MESSAGES/fr.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/fr/LC_MESSAGES/shared_wg_fr.po` & `tabcmd-2.0.9/tabcmd/locales/fr/LC_MESSAGES/shared_wg_fr.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/fr/LC_MESSAGES/tabcmd.mo` & `tabcmd-2.0.9/tabcmd/locales/fr/LC_MESSAGES/tabcmd.mo`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/fr/LC_MESSAGES/tabcmd.po` & `tabcmd-2.0.9/tabcmd/locales/fr/LC_MESSAGES/tabcmd.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/fr/LC_MESSAGES/tabcmd_messages_fr.po` & `tabcmd-2.0.9/tabcmd/locales/fr/LC_MESSAGES/tabcmd_messages_fr.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/fr/shared_wg_fr.properties` & `tabcmd-2.0.9/tabcmd/locales/fr/shared_wg_fr.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/fr/tabcmd_messages_fr.properties` & `tabcmd-2.0.9/tabcmd/locales/fr/tabcmd_messages_fr.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ga/LC_MESSAGES/ga.po` & `tabcmd-2.0.9/tabcmd/locales/ga/LC_MESSAGES/ga.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ga/LC_MESSAGES/shared_wg_ga.po` & `tabcmd-2.0.9/tabcmd/locales/ga/LC_MESSAGES/shared_wg_ga.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ga/LC_MESSAGES/tabcmd.mo` & `tabcmd-2.0.9/tabcmd/locales/ga/LC_MESSAGES/tabcmd.mo`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ga/LC_MESSAGES/tabcmd.po` & `tabcmd-2.0.9/tabcmd/locales/ga/LC_MESSAGES/tabcmd.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ga/LC_MESSAGES/tabcmd_messages_ga.po` & `tabcmd-2.0.9/tabcmd/locales/ga/LC_MESSAGES/tabcmd_messages_ga.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ga/shared_wg_ga.properties` & `tabcmd-2.0.9/tabcmd/locales/ga/shared_wg_ga.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ga/tabcmd_messages_ga.properties` & `tabcmd-2.0.9/tabcmd/locales/ga/tabcmd_messages_ga.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/it/LC_MESSAGES/it.po` & `tabcmd-2.0.9/tabcmd/locales/it/LC_MESSAGES/it.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/it/LC_MESSAGES/shared_wg_it.po` & `tabcmd-2.0.9/tabcmd/locales/it/LC_MESSAGES/shared_wg_it.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/it/LC_MESSAGES/tabcmd.mo` & `tabcmd-2.0.9/tabcmd/locales/it/LC_MESSAGES/tabcmd.mo`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/it/LC_MESSAGES/tabcmd.po` & `tabcmd-2.0.9/tabcmd/locales/it/LC_MESSAGES/tabcmd.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/it/LC_MESSAGES/tabcmd_messages_it.po` & `tabcmd-2.0.9/tabcmd/locales/it/LC_MESSAGES/tabcmd_messages_it.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/it/shared_wg_it.properties` & `tabcmd-2.0.9/tabcmd/locales/it/shared_wg_it.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/it/tabcmd_messages_it.properties` & `tabcmd-2.0.9/tabcmd/locales/it/tabcmd_messages_it.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ja/LC_MESSAGES/ja.po` & `tabcmd-2.0.9/tabcmd/locales/ja/LC_MESSAGES/ja.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ja/LC_MESSAGES/shared_wg_ja.po` & `tabcmd-2.0.9/tabcmd/locales/ja/LC_MESSAGES/shared_wg_ja.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ja/LC_MESSAGES/tabcmd.mo` & `tabcmd-2.0.9/tabcmd/locales/ja/LC_MESSAGES/tabcmd.mo`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ja/LC_MESSAGES/tabcmd.po` & `tabcmd-2.0.9/tabcmd/locales/ja/LC_MESSAGES/tabcmd.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ja/LC_MESSAGES/tabcmd_messages_ja.po` & `tabcmd-2.0.9/tabcmd/locales/ja/LC_MESSAGES/tabcmd_messages_ja.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ja/shared_wg_ja.properties` & `tabcmd-2.0.9/tabcmd/locales/ja/shared_wg_ja.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ja/tabcmd_messages_ja.properties` & `tabcmd-2.0.9/tabcmd/locales/ja/tabcmd_messages_ja.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ko/LC_MESSAGES/ko.po` & `tabcmd-2.0.9/tabcmd/locales/ko/LC_MESSAGES/ko.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ko/LC_MESSAGES/shared_wg_ko.po` & `tabcmd-2.0.9/tabcmd/locales/ko/LC_MESSAGES/shared_wg_ko.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ko/LC_MESSAGES/tabcmd.mo` & `tabcmd-2.0.9/tabcmd/locales/ko/LC_MESSAGES/tabcmd.mo`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ko/LC_MESSAGES/tabcmd.po` & `tabcmd-2.0.9/tabcmd/locales/ko/LC_MESSAGES/tabcmd.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ko/LC_MESSAGES/tabcmd_messages_ko.po` & `tabcmd-2.0.9/tabcmd/locales/ko/LC_MESSAGES/tabcmd_messages_ko.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ko/shared_wg_ko.properties` & `tabcmd-2.0.9/tabcmd/locales/ko/shared_wg_ko.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/ko/tabcmd_messages_ko.properties` & `tabcmd-2.0.9/tabcmd/locales/ko/tabcmd_messages_ko.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/pt/LC_MESSAGES/pt.po` & `tabcmd-2.0.9/tabcmd/locales/pt/LC_MESSAGES/pt.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/pt/LC_MESSAGES/shared_wg_pt.po` & `tabcmd-2.0.9/tabcmd/locales/pt/LC_MESSAGES/shared_wg_pt.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/pt/LC_MESSAGES/tabcmd.mo` & `tabcmd-2.0.9/tabcmd/locales/pt/LC_MESSAGES/tabcmd.mo`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/pt/LC_MESSAGES/tabcmd.po` & `tabcmd-2.0.9/tabcmd/locales/pt/LC_MESSAGES/tabcmd.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/pt/LC_MESSAGES/tabcmd_messages_pt.po` & `tabcmd-2.0.9/tabcmd/locales/pt/LC_MESSAGES/tabcmd_messages_pt.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/pt/shared_wg_pt.properties` & `tabcmd-2.0.9/tabcmd/locales/pt/shared_wg_pt.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/pt/tabcmd_messages_pt.properties` & `tabcmd-2.0.9/tabcmd/locales/pt/tabcmd_messages_pt.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/sv/LC_MESSAGES/shared_wg_sv.po` & `tabcmd-2.0.9/tabcmd/locales/sv/LC_MESSAGES/shared_wg_sv.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/sv/LC_MESSAGES/sv.po` & `tabcmd-2.0.9/tabcmd/locales/sv/LC_MESSAGES/sv.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/sv/LC_MESSAGES/tabcmd.mo` & `tabcmd-2.0.9/tabcmd/locales/sv/LC_MESSAGES/tabcmd.mo`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/sv/LC_MESSAGES/tabcmd.po` & `tabcmd-2.0.9/tabcmd/locales/sv/LC_MESSAGES/tabcmd.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/sv/LC_MESSAGES/tabcmd_messages_sv.po` & `tabcmd-2.0.9/tabcmd/locales/sv/LC_MESSAGES/tabcmd_messages_sv.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/sv/shared_wg_sv.properties` & `tabcmd-2.0.9/tabcmd/locales/sv/shared_wg_sv.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/sv/tabcmd_messages_sv.properties` & `tabcmd-2.0.9/tabcmd/locales/sv/tabcmd_messages_sv.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/zh/LC_MESSAGES/shared_wg_zh.po` & `tabcmd-2.0.9/tabcmd/locales/zh/LC_MESSAGES/shared_wg_zh.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/zh/LC_MESSAGES/tabcmd.mo` & `tabcmd-2.0.9/tabcmd/locales/zh/LC_MESSAGES/tabcmd.mo`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/zh/LC_MESSAGES/tabcmd.po` & `tabcmd-2.0.9/tabcmd/locales/zh/LC_MESSAGES/tabcmd.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/zh/LC_MESSAGES/tabcmd_messages_zh.po` & `tabcmd-2.0.9/tabcmd/locales/zh/LC_MESSAGES/tabcmd_messages_zh.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/zh/LC_MESSAGES/zh.po` & `tabcmd-2.0.9/tabcmd/locales/zh/LC_MESSAGES/zh.po`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/zh/shared_wg_zh.properties` & `tabcmd-2.0.9/tabcmd/locales/zh/shared_wg_zh.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/locales/zh/tabcmd_messages_zh.properties` & `tabcmd-2.0.9/tabcmd/locales/zh/tabcmd_messages_zh.properties`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd/tabcmd.py` & `tabcmd-2.0.9/tabcmd/tabcmd.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,17 @@
         raise ImportError(
             "Tabcmd requires Python 3.7 but you are on " + sys.version_info + " - please update your python version."
         )
 
     try:
         parser = TabcmdController.initialize()
         TabcmdController.run(parser)
+    except KeyboardInterrupt as ke:
+        print("Keyboard Interrupt: exiting")
+        sys.exit(1)
     except Exception as e:
         print(sys.stderr, "Unhandled exception: {}".format(type(e).__name__))
         print(
             sys.stderr,
             f"{type(e).__name__} at line {e.__traceback__.tb_lineno} of {__file__}: {e}",
         )
         sys.exit(1)
```

### Comparing `tabcmd-2.0.8/tabcmd-linux.spec` & `tabcmd-2.0.9/tabcmd-windows.spec`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 block_cipher = None
 
 a = Analysis(
     ['tabcmd\\tabcmd.py'],
     pathex=[],
     binaries=[],
     datas=datas,
-    hiddenimports=['tableauserverclient', 'requests.packages.urllib3', 'pkg_resources'],
+    hiddenimports=['tableauserverclient', 'requests', 'pkg_resources'],
     hookspath=[],
     hooksconfig={},
     runtime_hooks=[],
     excludes=[],
     win_no_prefer_redirects=False,
     win_private_assemblies=False,
     cipher=block_cipher,
@@ -27,15 +27,15 @@
 exe = EXE(
     pyz,
     a.scripts,
     a.binaries,
     a.zipfiles,
     a.datas,
     [],
-    name='tabcmd-windows',
+    name='tabcmd',
     debug=False,
     bootloader_ignore_signals=False,
     strip=False,
     upx=True,
     upx_exclude=[],
     runtime_tmpdir=None,
     console=True,
```

### Comparing `tabcmd-2.0.8/tabcmd-mac.spec` & `tabcmd-2.0.9/tabcmd-mac.spec`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 a = Analysis(
     ['tabcmd/tabcmd.py'],
     pathex=[],
     binaries=[],
     datas=datas,
-    hiddenimports=['tableauserverclient', 'requests.packages.urllib3', 'pkg_resources'],
+    hiddenimports=['tableauserverclient', 'requests', 'urllib3', 'pkg_resources'],
     hookspath=[],
     hooksconfig={},
     runtime_hooks=[],
     excludes=[],
     win_no_prefer_redirects=False,
     win_private_assemblies=False,
     cipher=block_cipher,
@@ -28,23 +28,24 @@
 exe = EXE(
     pyz,
     a.scripts,
     a.binaries,
     a.zipfiles,
     a.datas,
     [],
-    name='tabcmd-mac',
+    name='tabcmd.app',
     debug=False,
     bootloader_ignore_signals=False,
     strip=False,
     upx=True,
-    upx_exclude=[],
     runtime_tmpdir=None,
     console=True,
-    disable_windowed_traceback=False,
-    argv_emulation=False,
-    target_arch=None,
     codesign_identity=None,
-    entitlements_file=None,
     version='program_metadata.txt',
+)
+
+app = BUNDLE(
+    exe,
+    name = 'tabcmd-app',
     icon='res/tabcmd.icns',
+    bundle_identifier = None,
 )
```

### Comparing `tabcmd-2.0.8/tabcmd-windows.spec` & `tabcmd-2.0.9/tabcmd-linux.spec`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 datas = []
 datas += collect_data_files('tabcmd.locales')
 print(datas)
 
 block_cipher = None
 
 a = Analysis(
-    ['tabcmd\\tabcmd.py'],
+    ['tabcmd.py'],
     pathex=[],
     binaries=[],
     datas=datas,
-    hiddenimports=['tableauserverclient', 'requests', 'pkg_resources'],
+    hiddenimports=['tableauserverclient', 'requests', 'urllib3', 'pkg_resources'],
     hookspath=[],
     hooksconfig={},
     runtime_hooks=[],
     excludes=[],
     win_no_prefer_redirects=False,
     win_private_assemblies=False,
     cipher=block_cipher,
@@ -27,15 +27,15 @@
 exe = EXE(
     pyz,
     a.scripts,
     a.binaries,
     a.zipfiles,
     a.datas,
     [],
-    name='tabcmd-windows',
+    name='tabcmd',
     debug=False,
     bootloader_ignore_signals=False,
     strip=False,
     upx=True,
     upx_exclude=[],
     runtime_tmpdir=None,
     console=True,
```

### Comparing `tabcmd-2.0.8/tabcmd.egg-info/PKG-INFO` & `tabcmd-2.0.9/tabcmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabcmd
-Version: 2.0.8
+Version: 2.0.9
 Summary: A command line client for working with Tableau Server.
 Author-email: Tableau <github@tableau.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 Tableau
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tabcmd-2.0.8/tabcmd.egg-info/SOURCES.txt` & `tabcmd-2.0.9/tabcmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tabcmd.spec` & `tabcmd-2.0.9/tabcmd.spec`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/assets/SampleDS.tds` & `tabcmd-2.0.9/tests/assets/SampleDS.tds`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/assets/World Indicators.tds` & `tabcmd-2.0.9/tests/assets/World Indicators.tds`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/assets/World Indicators.tdsx` & `tabcmd-2.0.9/tests/assets/World Indicators.tdsx`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/commands/test_execution.py` & `tabcmd-2.0.9/tests/commands/test_execution.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/commands/test_geturl_utils.py` & `tabcmd-2.0.9/tests/commands/test_geturl_utils.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/commands/test_localize.py` & `tabcmd-2.0.9/tests/commands/test_localize.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/commands/test_projects_utils.py` & `tabcmd-2.0.9/tests/commands/test_projects_utils.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/commands/test_run_commands.py` & `tabcmd-2.0.9/tests/commands/test_run_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,14 +355,16 @@
         mock_session.assert_called()
 
     def test_create_site_users(self, mock_session, mock_server):
         RunCommandsTest._set_up_session(mock_session, mock_server)
         mock_args.filename = RunCommandsTest._set_up_file()
         mock_args.require_all_valid = False
         mock_args.site_name = None
+        mock_args.role = "Viewer"
+        mock_args.auth_type = "SAML"
         create_site_users.CreateSiteUsersCommand.run_command(mock_args)
         mock_session.assert_called()
 
     def test_delete_site_users(self, mock_session, mock_server):
         RunCommandsTest._set_up_session(mock_session, mock_server)
         mock_server.users = getter
         mock_args.filename = RunCommandsTest._set_up_file()
```

### Comparing `tabcmd-2.0.8/tests/commands/test_server_handler.py` & `tabcmd-2.0.9/tests/commands/test_server_handler.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/commands/test_session.py` & `tabcmd-2.0.9/tests/commands/test_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from argparse import Namespace
 import unittest
 from unittest import mock
 from unittest.mock import patch, mock_open
 
 from tabcmd.commands.auth.session import Session
 import os
@@ -42,14 +43,15 @@
     proxy=None,
     no_proxy=True,
     timeout=None,
     no_prompt=False,
 )
 
 fakeserver = "http://SRVR".lower()
+logger = logging.getLogger("tests")
 
 
 def _set_mocks_for_json_file_saved_username(mock_json_load, auth_token, username):
     mock_auth = vars(mock_data_from_json)
     mock_json_load.return_value = {"tableau_auth": [mock_auth]}
     mock_auth["auth_token"] = auth_token
     mock_auth["username"] = username
@@ -345,14 +347,47 @@
         tscauth_mock = mock.MagicMock(name="tsc.auth")
         mock_tsc.auth = tscauth_mock
         mock_tsc.auth_token = "cookiieeeee"
         mock_tsc.site_id = "1"
         mock_tsc.user_id = "0"
 
 
+class TimeoutArgTests(unittest.TestCase):
+    def test_timeout_as_integer_stored_int(self):
+        result = Session.timeout_as_integer(logger, 1, None)
+        assert result == 1
+
+    def test_timeout_as_integer_new_int(self):
+        result = Session.timeout_as_integer(logger, None, 3)
+        assert result == 3
+
+    def test_timeout_as_integer_no_value(self):
+        result = Session.timeout_as_integer(logger, None, None)
+        assert result == 0
+
+    def test_timeout_as_integer_stored_char(self):
+        result = Session.timeout_as_integer(logger, "ab", None)
+        assert result == 0
+
+
+class TimeoutIntegrationTest(unittest.TestCase):
+    def test_connection_times_out(self):
+        test_args = Namespace(**vars(args_to_mock))
+        new_session = Session()
+        test_args.timeout = 10
+        test_args.username = "u"
+        test_args.password = "p"
+
+        test_args.server = "https://nothere.com"
+        with self.assertRaises(SystemExit):
+            new_session.create_session(test_args)
+
+    # should test connection doesn't time out?
+
+
 @mock.patch("tableauserverclient.Server")
 class ConnectionOptionsTest(unittest.TestCase):
     def test_certcheck_on(self, mock_tsc):
         mock_tsc.add_http_options = mock.MagicMock()
         mock_session = mock.MagicMock()
         mock_session.no_certcheck = True
         mock_session.site_id = "s"
```

### Comparing `tabcmd-2.0.8/tests/commands/test_user_utils.py` & `tabcmd-2.0.9/tests/commands/test_user_utils.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/e2e/language_tests.py` & `tabcmd-2.0.9/tests/e2e/language_tests.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/e2e/online_tests.py` & `tabcmd-2.0.9/tests/e2e/online_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,21 @@
 
     def _get_view_with_filters(self):
         command = "get"
 
     def _get_workbook(self, server_file):
         command = "get"
         server_file = "/workbooks/" + server_file
+        arguments = [command, server_file, "-f", "get_workbook.twbx"]
+        _test_command(arguments)
+        os.path.exists("get_workbook.twbx")
+
+    def _get_datasource(self, server_file):
+        command = "get"
+        server_file = "/datasources/" + server_file
         arguments = [command, server_file]
         _test_command(arguments)
 
     def _get_datasource(self, server_file):
         command = "get"
         server_file = "/datasources/" + server_file
         arguments = [command, server_file]
```

### Comparing `tabcmd-2.0.8/tests/e2e/setup_e2e.py` & `tabcmd-2.0.9/tests/e2e/setup_e2e.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/e2e/tests.py` & `tabcmd-2.0.9/tests/e2e/tests.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/e2e/tests_integration.py` & `tabcmd-2.0.9/tests/e2e/tests_integration.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/common_setup.py` & `tabcmd-2.0.9/tests/parsers/common_setup.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_login_parser.py` & `tabcmd-2.0.9/tests/parsers/test_login_parser.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_logout_parser.py` & `tabcmd-2.0.9/tests/parsers/test_logout_parser.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_add_user.py` & `tabcmd-2.0.9/tests/parsers/test_parser_add_user.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_create_extracts.py` & `tabcmd-2.0.9/tests/parsers/test_parser_create_extracts.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_create_group.py` & `tabcmd-2.0.9/tests/parsers/test_parser_create_group.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_create_project.py` & `tabcmd-2.0.9/tests/parsers/test_parser_create_project.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_create_site.py` & `tabcmd-2.0.9/tests/parsers/test_parser_create_site.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_create_site_users.py` & `tabcmd-2.0.9/tests/parsers/test_parser_create_site_users.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_create_user.py` & `tabcmd-2.0.9/tests/parsers/test_parser_create_user.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_decrypt_extracts.py` & `tabcmd-2.0.9/tests/parsers/test_parser_decrypt_extracts.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_delete.py` & `tabcmd-2.0.9/tests/parsers/test_parser_delete.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_delete_extracts.py` & `tabcmd-2.0.9/tests/parsers/test_parser_delete_extracts.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_delete_group.py` & `tabcmd-2.0.9/tests/parsers/test_parser_delete_group.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_delete_project.py` & `tabcmd-2.0.9/tests/parsers/test_parser_delete_project.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_delete_site.py` & `tabcmd-2.0.9/tests/parsers/test_parser_delete_site.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_delete_site_user.py` & `tabcmd-2.0.9/tests/parsers/test_parser_delete_site_user.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_edit_site.py` & `tabcmd-2.0.9/tests/parsers/test_parser_edit_site.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_encrypt_extracts.py` & `tabcmd-2.0.9/tests/parsers/test_parser_encrypt_extracts.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_export.py` & `tabcmd-2.0.9/tests/parsers/test_parser_export.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_get_url.py` & `tabcmd-2.0.9/tests/parsers/test_parser_get_url.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_list_sites.py` & `tabcmd-2.0.9/tests/parsers/test_parser_list_sites.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_publish.py` & `tabcmd-2.0.9/tests/parsers/test_parser_publish.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_publish_samples.py` & `tabcmd-2.0.9/tests/parsers/test_parser_publish_samples.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_reencrypt_extracts.py` & `tabcmd-2.0.9/tests/parsers/test_parser_reencrypt_extracts.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_refresh_extracts.py` & `tabcmd-2.0.9/tests/parsers/test_parser_refresh_extracts.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_remove_user.py` & `tabcmd-2.0.9/tests/parsers/test_parser_remove_user.py`

 * *Files identical despite different names*

### Comparing `tabcmd-2.0.8/tests/parsers/test_parser_runschedule.py` & `tabcmd-2.0.9/tests/parsers/test_parser_runschedule.py`

 * *Files identical despite different names*

