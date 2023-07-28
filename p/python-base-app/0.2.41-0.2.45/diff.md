# Comparing `tmp/python-base-app-0.2.41.tar.gz` & `tmp/python-base-app-0.2.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-base-app-0.2.41.tar", last modified: Sat Jul  2 15:21:11 2022, max compression
+gzip compressed data, was "python-base-app-0.2.45.tar", last modified: Fri Jul 28 21:17:08 2023, max compression
```

## Comparing `python-base-app-0.2.41.tar` & `python-base-app-0.2.45.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.553773 python-base-app-0.2.41/
--rw-r--r--   0 root         (0) root         (0)    35149 2022-07-02 15:21:09.000000 python-base-app-0.2.41/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1140 2022-07-02 15:21:09.000000 python-base-app-0.2.41/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6881 2022-07-02 15:21:11.553773 python-base-app-0.2.41/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6523 2022-07-02 15:21:09.000000 python-base-app-0.2.41/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.545772 python-base-app-0.2.41/python_base_app/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1735 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/actuator.py
--rw-r--r--   0 root         (0) root         (0)     8578 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/audio_handler.py
--rw-r--r--   0 root         (0) root         (0)     5167 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/auth_view_handler.py
--rw-r--r--   0 root         (0) root         (0)    22176 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/base_app.py
--rw-r--r--   0 root         (0) root         (0)     1163 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/base_audio_player.py
--rw-r--r--   0 root         (0) root         (0)    46660 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/base_ci_toolbox.py
--rw-r--r--   0 root         (0) root         (0)     9130 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/base_rest_api_access.py
--rw-r--r--   0 root         (0) root         (0)     2530 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/base_user_handler.py
--rw-r--r--   0 root         (0) root         (0)     7982 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/base_web_server.py
--rw-r--r--   0 root         (0) root         (0)    16667 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5780 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/custom_fields.py
--rw-r--r--   0 root         (0) root         (0)     1594 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/custom_form.py
--rw-r--r--   0 root         (0) root         (0)     7878 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/daemon.py
--rw-r--r--   0 root         (0) root         (0)     3484 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1279 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/git.py
--rw-r--r--   0 root         (0) root         (0)      146 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/git_metadata.py
--rw-r--r--   0 root         (0) root         (0)     2099 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/locale_helper.py
--rw-r--r--   0 root         (0) root         (0)     4069 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/log_handling.py
--rw-r--r--   0 root         (0) root         (0)     2205 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/mpg123_audio_player.py
--rw-r--r--   0 root         (0) root         (0)     2838 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/notification_handler.py
--rw-r--r--   0 root         (0) root         (0)     6425 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/pinger.py
--rw-r--r--   0 root         (0) root         (0)     1488 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/playsound_audio_player.py
--rw-r--r--   0 root         (0) root         (0)     1953 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/pyglet_audio_player.py
--rw-r--r--   0 root         (0) root         (0)     1189 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.545772 python-base-app-0.2.41/python_base_app/static/icons/
--rw-r--r--   0 root         (0) root         (0)     6743 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/static/icons/icon-python-base-app-128x128.png
--rw-r--r--   0 root         (0) root         (0)     1792 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/templates/
--rw-r--r--   0 root         (0) root         (0)     3100 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/analyze-app.template.sh
--rwxr-xr-x   0 root         (0) root         (0)     3458 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/build-docker-images.template.sh
--rw-r--r--   0 root         (0) root         (0)     8015 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/circle-ci.template.yml
--rw-r--r--   0 root         (0) root         (0)     1433 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/codacy.template.yml
--rw-r--r--   0 root         (0) root         (0)     2122 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/coveragerc.template
--rw-r--r--   0 root         (0) root         (0)      640 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/debian_control.template.conf
--rw-r--r--   0 root         (0) root         (0)    10490 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/debian_postinst.template.sh
--rw-r--r--   0 root         (0) root         (0)     1268 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/git.template.py
--rw-r--r--   0 root         (0) root         (0)     8069 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/gitlab-ci.template.yml
--rw-r--r--   0 root         (0) root         (0)     1643 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/install-debian-package.template.sh
--rw-r--r--   0 root         (0) root         (0)     2610 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/install-pypi-package.template.sh
--rwxr-xr-x   0 root         (0) root         (0)     4746 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/make-debian-package.template.sh
--rw-r--r--   0 root         (0) root         (0)     3049 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/pip3.template.sh
--rw-r--r--   0 root         (0) root         (0)     2535 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/publish-debian-package.template.sh
--rw-r--r--   0 root         (0) root         (0)     4050 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/publish-pypi-package.template.sh
--rw-r--r--   0 root         (0) root         (0)     4387 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/templates/test-app.template.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/test/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6950 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/base_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/test/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/test/resources/ci_toolbox/
--rw-r--r--   0 root         (0) root         (0)       73 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/resources/ci_toolbox/.gitignore
--rw-r--r--   0 root         (0) root         (0)       17 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/resources/ci_toolbox/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/test/resources/ci_toolbox/a_package/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/resources/ci_toolbox/a_package/__init__.py
--rw-r--r--   0 root         (0) root         (0)      213 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/resources/ci_toolbox/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1117 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/resources/ci_toolbox/settings.py
--rwxr-xr-x   0 root         (0) root         (0)     2214 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/resources/ci_toolbox/setup.py
--rw-r--r--   0 root         (0) root         (0)     4911 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/test_audio_handler.py
--rw-r--r--   0 root         (0) root         (0)     1429 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/test_audio_player.py
--rw-r--r--   0 root         (0) root         (0)     3930 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/test_base_ci_toolbox.py
--rw-r--r--   0 root         (0) root         (0)     2018 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/test_base_web_server.py
--rw-r--r--   0 root         (0) root         (0)     8682 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/test_configuration.py
--rw-r--r--   0 root         (0) root         (0)      980 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/test_pytest.py
--rwxr-xr-x   0 root         (0) root         (0)     2916 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/test_suite.py
--rw-r--r--   0 root         (0) root         (0)     7365 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/test/test_unix_user_handler.py
--rw-r--r--   0 root         (0) root         (0)    16170 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/bn/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/translations/bn/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      742 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/bn/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/da/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/translations/da/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      705 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/da/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/translations/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      961 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/de/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/translations/es/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      625 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/es/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/translations/fi/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      688 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/fi/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/translations/fr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      812 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/fr/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/translations/hr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      696 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/hr/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/hu/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/translations/hu/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      438 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/hu/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/it/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/translations/it/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      952 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/it/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.549773 python-base-app-0.2.41/python_base_app/translations/ja/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      722 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/ja/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/lt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.553773 python-base-app-0.2.41/python_base_app/translations/lt/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      508 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/lt/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.553773 python-base-app-0.2.41/python_base_app/translations/nl/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      674 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/nl/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.553773 python-base-app-0.2.41/python_base_app/translations/ru/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      794 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/ru/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/sr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.553773 python-base-app-0.2.41/python_base_app/translations/sr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      519 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/sr/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/th/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.553773 python-base-app-0.2.41/python_base_app/translations/th/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      770 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/th/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.537772 python-base-app-0.2.41/python_base_app/translations/tr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.553773 python-base-app-0.2.41/python_base_app/translations/tr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      668 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 root         (0) root         (0)     3371 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/unix_user_handler.py
--rw-r--r--   0 root         (0) root         (0)     1269 2022-07-02 15:21:09.000000 python-base-app-0.2.41/python_base_app/view_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-02 15:21:11.545772 python-base-app-0.2.41/python_base_app.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6881 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3755 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      283 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-02 15:21:11.000000 python-base-app-0.2.41/python_base_app.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      369 2022-07-02 15:21:09.000000 python-base-app-0.2.41/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)     1010 2022-07-02 15:21:09.000000 python-base-app-0.2.41/run_python_base_app_test_suite.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-02 15:21:11.553773 python-base-app-0.2.41/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2423 2022-07-02 15:21:09.000000 python-base-app-0.2.41/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.130382 python-base-app-0.2.45/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-07-28 21:17:06.000000 python-base-app-0.2.45/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-07-28 21:17:06.000000 python-base-app-0.2.45/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6881 2023-07-28 21:17:08.130382 python-base-app-0.2.45/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6523 2023-07-28 21:17:06.000000 python-base-app-0.2.45/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.122382 python-base-app-0.2.45/python_base_app/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/actuator.py
+-rw-r--r--   0 root         (0) root         (0)     8578 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/audio_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5167 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/auth_view_handler.py
+-rw-r--r--   0 root         (0) root         (0)    22176 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/base_app.py
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/base_audio_player.py
+-rw-r--r--   0 root         (0) root         (0)    46660 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/base_ci_toolbox.py
+-rw-r--r--   0 root         (0) root         (0)     9130 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/base_rest_api_access.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/base_user_handler.py
+-rw-r--r--   0 root         (0) root         (0)     7982 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/base_web_server.py
+-rw-r--r--   0 root         (0) root         (0)    16667 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/custom_fields.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/custom_form.py
+-rw-r--r--   0 root         (0) root         (0)     7878 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     3484 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/git.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/git_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2099 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/locale_helper.py
+-rw-r--r--   0 root         (0) root         (0)     4069 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/log_handling.py
+-rw-r--r--   0 root         (0) root         (0)     2205 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/mpg123_audio_player.py
+-rw-r--r--   0 root         (0) root         (0)     2838 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/notification_handler.py
+-rw-r--r--   0 root         (0) root         (0)     6425 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/pinger.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/playsound_audio_player.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/pyglet_audio_player.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.122382 python-base-app-0.2.45/python_base_app/static/icons/
+-rw-r--r--   0 root         (0) root         (0)     6743 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/static/icons/icon-python-base-app-128x128.png
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.126382 python-base-app-0.2.45/python_base_app/templates/
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/analyze-app.template.sh
+-rwxr-xr-x   0 root         (0) root         (0)     3458 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/build-docker-images.template.sh
+-rw-r--r--   0 root         (0) root         (0)     8015 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/circle-ci.template.yml
+-rw-r--r--   0 root         (0) root         (0)     1433 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/codacy.template.yml
+-rw-r--r--   0 root         (0) root         (0)     2122 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/coveragerc.template
+-rw-r--r--   0 root         (0) root         (0)      640 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/debian_control.template.conf
+-rw-r--r--   0 root         (0) root         (0)    10509 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/debian_postinst.template.sh
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/git.template.py
+-rw-r--r--   0 root         (0) root         (0)     8069 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/gitlab-ci.template.yml
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/install-debian-package.template.sh
+-rw-r--r--   0 root         (0) root         (0)     2610 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/install-pypi-package.template.sh
+-rwxr-xr-x   0 root         (0) root         (0)     4746 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/make-debian-package.template.sh
+-rw-r--r--   0 root         (0) root         (0)     3049 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/pip3.template.sh
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/publish-debian-package.template.sh
+-rw-r--r--   0 root         (0) root         (0)     4050 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/publish-pypi-package.template.sh
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/templates/test-app.template.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.126382 python-base-app-0.2.45/python_base_app/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6951 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/base_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/test/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.126382 python-base-app-0.2.45/python_base_app/test/resources/ci_toolbox/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/resources/ci_toolbox/.gitignore
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/resources/ci_toolbox/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.126382 python-base-app-0.2.45/python_base_app/test/resources/ci_toolbox/a_package/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/resources/ci_toolbox/a_package/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/resources/ci_toolbox/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/resources/ci_toolbox/settings.py
+-rwxr-xr-x   0 root         (0) root         (0)     2214 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/resources/ci_toolbox/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4911 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/test_audio_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/test_audio_player.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/test_base_ci_toolbox.py
+-rw-r--r--   0 root         (0) root         (0)     2018 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/test_base_web_server.py
+-rw-r--r--   0 root         (0) root         (0)     8682 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/test_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      980 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/test_pytest.py
+-rwxr-xr-x   0 root         (0) root         (0)     2916 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/test_suite.py
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/test/test_unix_user_handler.py
+-rw-r--r--   0 root         (0) root         (0)    16379 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/bn/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.126382 python-base-app-0.2.45/python_base_app/translations/bn/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/bn/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/da/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.126382 python-base-app-0.2.45/python_base_app/translations/da/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      705 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/da/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.126382 python-base-app-0.2.45/python_base_app/translations/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/de/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.126382 python-base-app-0.2.45/python_base_app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      625 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/es/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.126382 python-base-app-0.2.45/python_base_app/translations/fi/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      688 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/fi/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.126382 python-base-app-0.2.45/python_base_app/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      812 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/fr/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.130382 python-base-app-0.2.45/python_base_app/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      696 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/hr/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/hu/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.130382 python-base-app-0.2.45/python_base_app/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      438 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/hu/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/it/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.130382 python-base-app-0.2.45/python_base_app/translations/it/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      952 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/it/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.130382 python-base-app-0.2.45/python_base_app/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      722 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/ja/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/lt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.130382 python-base-app-0.2.45/python_base_app/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      508 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/lt/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.130382 python-base-app-0.2.45/python_base_app/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      674 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/nl/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.130382 python-base-app-0.2.45/python_base_app/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      794 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/ru/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/sr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.130382 python-base-app-0.2.45/python_base_app/translations/sr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      519 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/sr/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/th/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.130382 python-base-app-0.2.45/python_base_app/translations/th/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      770 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/th/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.118382 python-base-app-0.2.45/python_base_app/translations/tr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.130382 python-base-app-0.2.45/python_base_app/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      668 2023-07-28 21:17:07.000000 python-base-app-0.2.45/python_base_app/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 root         (0) root         (0)     3371 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/unix_user_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-07-28 21:17:06.000000 python-base-app-0.2.45/python_base_app/view_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 21:17:08.122382 python-base-app-0.2.45/python_base_app.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6881 2023-07-28 21:17:08.000000 python-base-app-0.2.45/python_base_app.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-07-28 21:17:08.000000 python-base-app-0.2.45/python_base_app.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 21:17:08.000000 python-base-app-0.2.45/python_base_app.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      248 2023-07-28 21:17:08.000000 python-base-app-0.2.45/python_base_app.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-28 21:17:08.000000 python-base-app-0.2.45/python_base_app.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      248 2023-07-28 21:17:06.000000 python-base-app-0.2.45/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)     1010 2023-07-28 21:17:06.000000 python-base-app-0.2.45/run_python_base_app_test_suite.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 21:17:08.130382 python-base-app-0.2.45/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2423 2023-07-28 21:17:06.000000 python-base-app-0.2.45/setup.py
```

### Comparing `python-base-app-0.2.41/LICENSE` & `python-base-app-0.2.45/LICENSE`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/MANIFEST.in` & `python-base-app-0.2.45/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/PKG-INFO` & `python-base-app-0.2.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-base-app
-Version: 0.2.41
+Version: 0.2.45
 Summary: Generic tools and base classes for Python applications with web interface.
 Home-page: https://github.com/marcus67/python_base_app
 Author: Marcus Rickert
 Author-email: marcus.rickert@web.de
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-base-app Version: 0.2.41 Summary: Generic
+Metadata-Version: 2.1 Name: python-base-app Version: 0.2.45 Summary: Generic
 tools and base classes for Python applications with web interface. Home-page:
 https://github.com/marcus67/python_base_app Author: Marcus Rickert Author-
 email: marcus.rickert@web.de License: UNKNOWN Platform: UNKNOWN Description-
 Content-Type: text/markdown License-File: LICENSE ![PythonBaseApp-Logo]
 (python_base_app/static/icons/icon-python-base-app-128x128.png) # Python
 Application Framework `python_base_app` ## Overview `python_base_app` is a
 simple framework for Python applications with a web frontend using [Flask]
```

### Comparing `python-base-app-0.2.41/README.md` & `python-base-app-0.2.45/README.md`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/actuator.py` & `python-base-app-0.2.45/python_base_app/actuator.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/audio_handler.py` & `python-base-app-0.2.45/python_base_app/audio_handler.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/auth_view_handler.py` & `python-base-app-0.2.45/python_base_app/auth_view_handler.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/base_app.py` & `python-base-app-0.2.45/python_base_app/base_app.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/base_audio_player.py` & `python-base-app-0.2.45/python_base_app/base_audio_player.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/base_ci_toolbox.py` & `python-base-app-0.2.45/python_base_app/base_ci_toolbox.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/base_rest_api_access.py` & `python-base-app-0.2.45/python_base_app/base_rest_api_access.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/base_user_handler.py` & `python-base-app-0.2.45/python_base_app/base_user_handler.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/base_web_server.py` & `python-base-app-0.2.45/python_base_app/base_web_server.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/configuration.py` & `python-base-app-0.2.45/python_base_app/configuration.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/custom_fields.py` & `python-base-app-0.2.45/python_base_app/custom_fields.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/custom_form.py` & `python-base-app-0.2.45/python_base_app/custom_form.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/daemon.py` & `python-base-app-0.2.45/python_base_app/daemon.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/exceptions.py` & `python-base-app-0.2.45/python_base_app/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/git.py` & `python-base-app-0.2.45/python_base_app/git.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/locale_helper.py` & `python-base-app-0.2.45/python_base_app/locale_helper.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/log_handling.py` & `python-base-app-0.2.45/python_base_app/log_handling.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/mpg123_audio_player.py` & `python-base-app-0.2.45/python_base_app/mpg123_audio_player.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/notification_handler.py` & `python-base-app-0.2.45/python_base_app/notification_handler.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/pinger.py` & `python-base-app-0.2.45/python_base_app/pinger.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/playsound_audio_player.py` & `python-base-app-0.2.45/python_base_app/playsound_audio_player.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/pyglet_audio_player.py` & `python-base-app-0.2.45/python_base_app/pyglet_audio_player.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/settings.py` & `python-base-app-0.2.45/python_base_app/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 settings = {
     "name": "python-base-app",
-    "version": "0.2.41",
+    "version": "0.2.45",
     "description": "Generic tools and base classes for Python applications with web interface.",
     "author": "Marcus Rickert",
     "author_email": "marcus.rickert@web.de",
     "url": "https://github.com/marcus67/python_base_app",
 }
 
 extended_settings = {
```

### Comparing `python-base-app-0.2.41/python_base_app/static/icons/icon-python-base-app-128x128.png` & `python-base-app-0.2.45/python_base_app/static/icons/icon-python-base-app-128x128.png`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/stats.py` & `python-base-app-0.2.45/python_base_app/stats.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/analyze-app.template.sh` & `python-base-app-0.2.45/python_base_app/templates/analyze-app.template.sh`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/build-docker-images.template.sh` & `python-base-app-0.2.45/python_base_app/templates/build-docker-images.template.sh`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/circle-ci.template.yml` & `python-base-app-0.2.45/python_base_app/templates/circle-ci.template.yml`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/codacy.template.yml` & `python-base-app-0.2.45/python_base_app/templates/codacy.template.yml`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/coveragerc.template` & `python-base-app-0.2.45/python_base_app/templates/coveragerc.template`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/debian_control.template.conf` & `python-base-app-0.2.45/python_base_app/templates/debian_control.template.conf`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/debian_postinst.template.sh` & `python-base-app-0.2.45/python_base_app/templates/debian_postinst.template.sh`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,15 @@
 
 ${PIP3} install wheel # setuptools
 echo "Installing PIP packages..."
 {%- for package_name in python_packages %}
 echo "  * {{ package_name[1] }}"
 {%- endfor %}
 # see https://stackoverflow.com/questions/19548957/can-i-force-pip-to-reinstall-the-current-version
-${PIP3} install --upgrade {% for package_name in python_packages %}\
+${PIP3} install --upgrade --ignore-installed {% for package_name in python_packages %}\
      ${LIB_DIR}/{{ package_name[1] }}{% endfor %}
 
 {% for package_name in python_packages %}
 echo "Removing installation file ${LIB_DIR}/{{ package_name[1] }}..."
 rm ${LIB_DIR}/{{ package_name[1] }}
 {%- endfor %}
```

### Comparing `python-base-app-0.2.41/python_base_app/templates/git.template.py` & `python-base-app-0.2.45/python_base_app/templates/git.template.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/gitlab-ci.template.yml` & `python-base-app-0.2.45/python_base_app/templates/gitlab-ci.template.yml`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/install-debian-package.template.sh` & `python-base-app-0.2.45/python_base_app/templates/install-debian-package.template.sh`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/install-pypi-package.template.sh` & `python-base-app-0.2.45/python_base_app/templates/install-pypi-package.template.sh`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/make-debian-package.template.sh` & `python-base-app-0.2.45/python_base_app/templates/make-debian-package.template.sh`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/pip3.template.sh` & `python-base-app-0.2.45/python_base_app/templates/pip3.template.sh`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/publish-debian-package.template.sh` & `python-base-app-0.2.45/python_base_app/templates/publish-debian-package.template.sh`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/publish-pypi-package.template.sh` & `python-base-app-0.2.45/python_base_app/templates/publish-pypi-package.template.sh`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/templates/test-app.template.sh` & `python-base-app-0.2.45/python_base_app/templates/test-app.template.sh`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/test/base_test.py` & `python-base-app-0.2.45/python_base_app/test/base_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 
         if self._test_data_base_dir is None:
             msg = "No base path specified for test case '{testcase}'"
             raise configuration.ConfigurationException(msg.format(testcase=self.__class__.__name__))
 
         return join(self._test_data_base_dir, p_rel_path)
 
-    def execute_pytest(self, p_base_dir=None, p_rel_path="pytest"):
+    def execute_pytest(self, p_base_dir=None, p_rel_path="pytests"):
 
         if p_base_dir is None:
             p_base_dir = os.path.dirname(__file__)
 
         pytest_dir = os.path.join(p_base_dir, p_rel_path)
 
         fmt = "Executing pytest tests in directory {dirname}"
```

### Comparing `python-base-app-0.2.41/python_base_app/test/resources/ci_toolbox/settings.py` & `python-base-app-0.2.45/python_base_app/test/resources/ci_toolbox/settings.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/test/resources/ci_toolbox/setup.py` & `python-base-app-0.2.45/python_base_app/test/resources/ci_toolbox/setup.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/test/test_audio_handler.py` & `python-base-app-0.2.45/python_base_app/test/test_audio_handler.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/test/test_audio_player.py` & `python-base-app-0.2.45/python_base_app/test/test_audio_player.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/test/test_base_ci_toolbox.py` & `python-base-app-0.2.45/python_base_app/test/test_base_ci_toolbox.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/test/test_base_web_server.py` & `python-base-app-0.2.45/python_base_app/test/test_base_web_server.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/test/test_configuration.py` & `python-base-app-0.2.45/python_base_app/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/test/test_pytest.py` & `python-base-app-0.2.45/python_base_app/test/test_pytest.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/test/test_suite.py` & `python-base-app-0.2.45/python_base_app/test/test_suite.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/test/test_unix_user_handler.py` & `python-base-app-0.2.45/python_base_app/test/test_unix_user_handler.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/tools.py` & `python-base-app-0.2.45/python_base_app/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-#    Copyright (C) 2019-2021  Marcus Rickert
+#    Copyright (C) 2019-2022  Marcus Rickert
 #
 #    See https://github.com/marcus67/python_base_app
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 3 of the License, or
 #    (at your option) any later version.
@@ -504,24 +504,29 @@
         result = socket.gethostbyaddr(p_ip_address)
         return result[0]
 
     except Exception:
         return p_ip_address
 
 
-def get_ip_address_by_dns_name(p_dns_name:str) -> str:
-
+def get_ip_address_by_dns_name(p_dns_name: str) -> str:
     if REGEX_IP_ADDRESS.match(p_dns_name.strip()):
         return p_dns_name.strip()
 
     return socket.gethostbyname(p_dns_name)
 
 
-def is_valid_ip_address_or_dns_name(p_dns_name:str) -> bool:
+def get_ip_addresses_by_dns_name(p_dns_name: str) -> set[str]:
+    if REGEX_IP_ADDRESS.match(p_dns_name.strip()):
+        return {p_dns_name.strip()}
+
+    return set(socket.gethostbyname_ex(p_dns_name)[2])
 
+
+def is_valid_ip_address_or_dns_name(p_dns_name: str) -> bool:
     try:
         get_ip_address_by_dns_name(p_dns_name)
         return True
 
     except Exception:
         return False
 
@@ -572,14 +577,15 @@
     else:
         return p_value
 
 
 def running_in_docker():
     return os.getenv("RUNNING_IN_DOCKER") is not None
 
+
 def running_in_snap():
     return os.getenv("RUNNING_IN_SNAP") is not None
 
 
 def copy_attributes(p_from: object, p_to: object, p_only_existing=False) -> None:
     for (key, value) in p_from.__dict__.items():
         if not key.startswith('_'):
```

### Comparing `python-base-app-0.2.41/python_base_app/translations/bn/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/bn/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/translations/da/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/translations/de/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/translations/es/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/translations/fi/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/fi/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/translations/fr/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/translations/hr/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/translations/it/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/translations/ja/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/translations/nl/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/translations/ru/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/translations/sr/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/sr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/translations/th/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/th/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/translations/tr/LC_MESSAGES/messages.mo` & `python-base-app-0.2.45/python_base_app/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/unix_user_handler.py` & `python-base-app-0.2.45/python_base_app/unix_user_handler.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app/view_info.py` & `python-base-app-0.2.45/python_base_app/view_info.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/python_base_app.egg-info/PKG-INFO` & `python-base-app-0.2.45/python_base_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-base-app
-Version: 0.2.41
+Version: 0.2.45
 Summary: Generic tools and base classes for Python applications with web interface.
 Home-page: https://github.com/marcus67/python_base_app
 Author: Marcus Rickert
 Author-email: marcus.rickert@web.de
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-base-app Version: 0.2.41 Summary: Generic
+Metadata-Version: 2.1 Name: python-base-app Version: 0.2.45 Summary: Generic
 tools and base classes for Python applications with web interface. Home-page:
 https://github.com/marcus67/python_base_app Author: Marcus Rickert Author-
 email: marcus.rickert@web.de License: UNKNOWN Platform: UNKNOWN Description-
 Content-Type: text/markdown License-File: LICENSE ![PythonBaseApp-Logo]
 (python_base_app/static/icons/icon-python-base-app-128x128.png) # Python
 Application Framework `python_base_app` ## Overview `python_base_app` is a
 simple framework for Python applications with a web frontend using [Flask]
```

### Comparing `python-base-app-0.2.41/python_base_app.egg-info/SOURCES.txt` & `python-base-app-0.2.45/python_base_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/run_python_base_app_test_suite.py` & `python-base-app-0.2.45/run_python_base_app_test_suite.py`

 * *Files identical despite different names*

### Comparing `python-base-app-0.2.41/setup.py` & `python-base-app-0.2.45/setup.py`

 * *Files identical despite different names*

