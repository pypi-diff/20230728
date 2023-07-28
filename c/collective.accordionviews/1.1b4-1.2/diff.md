# Comparing `tmp/collective.accordionviews-1.1b4.tar.gz` & `tmp/collective.accordionviews-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.accordionviews-1.1b4.tar", last modified: Mon Oct 31 15:47:16 2022, max compression
+gzip compressed data, was "collective.accordionviews-1.2.tar", last modified: Fri Jul 28 07:06:49 2023, max compression
```

## Comparing `collective.accordionviews-1.1b4.tar` & `collective.accordionviews-1.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.579001 collective.accordionviews-1.1b4/
--rw-r--r--   0 maik      (1000) maik      (1000)      520 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/CHANGES.rst
--rw-r--r--   0 maik      (1000) maik      (1000)       59 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/CONTRIBUTORS.rst
--rw-r--r--   0 maik      (1000) maik      (1000)     1338 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/DEVELOP.rst
--rw-r--r--   0 maik      (1000) maik      (1000)    18092 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/LICENSE.GPL
--rw-r--r--   0 maik      (1000) maik      (1000)      671 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/LICENSE.rst
--rw-r--r--   0 maik      (1000) maik      (1000)       67 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/MANIFEST.in
--rw-r--r--   0 maik      (1000) maik      (1000)     4461 2022-10-31 15:47:16.579001 collective.accordionviews-1.1b4/PKG-INFO
--rw-r--r--   0 maik      (1000) maik      (1000)     2695 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/README.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.575001 collective.accordionviews-1.1b4/docs/
--rw-r--r--   0 maik      (1000) maik      (1000)     7937 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/docs/conf.py
--rw-r--r--   0 maik      (1000) maik      (1000)       98 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/docs/index.rst
--rw-r--r--   0 maik      (1000) maik      (1000)      334 2022-10-31 15:47:16.579001 collective.accordionviews-1.1b4/setup.cfg
--rw-r--r--   0 maik      (1000) maik      (1000)     2556 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/setup.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.573001 collective.accordionviews-1.1b4/src/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.575001 collective.accordionviews-1.1b4/src/collective/
--rw-r--r--   0 maik      (1000) maik      (1000)       80 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/__init__.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.575001 collective.accordionviews-1.1b4/src/collective/accordionviews/
--rw-r--r--   0 maik      (1000) maik      (1000)      141 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/__init__.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.577001 collective.accordionviews-1.1b4/src/collective/accordionviews/browser/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/browser/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      618 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/browser/configure.zcml
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.577001 collective.accordionviews-1.1b4/src/collective/accordionviews/browser/overrides/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/browser/overrides/.gitkeep
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.577001 collective.accordionviews-1.1b4/src/collective/accordionviews/browser/static/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/browser/static/.gitkeep
--rw-r--r--   0 maik      (1000) maik      (1000)     1476 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/configure.zcml
--rw-r--r--   0 maik      (1000) maik      (1000)      274 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/interfaces.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.577001 collective.accordionviews-1.1b4/src/collective/accordionviews/locales/
--rw-r--r--   0 maik      (1000) maik      (1000)      611 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/locales/README.rst
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/locales/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1206 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/locales/collective.accordionviews.pot
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.573001 collective.accordionviews-1.1b4/src/collective/accordionviews/locales/de/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.577001 collective.accordionviews-1.1b4/src/collective/accordionviews/locales/de/LC_MESSAGES/
--rw-r--r--   0 maik      (1000) maik      (1000)     1122 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/locales/de/LC_MESSAGES/collective.accordionviews.po
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.573001 collective.accordionviews-1.1b4/src/collective/accordionviews/locales/en/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.577001 collective.accordionviews-1.1b4/src/collective/accordionviews/locales/en/LC_MESSAGES/
--rw-r--r--   0 maik      (1000) maik      (1000)     1079 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/locales/en/LC_MESSAGES/collective.accordionviews.po
--rw-r--r--   0 maik      (1000) maik      (1000)      650 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/locales/manual.pot
--rw-r--r--   0 maik      (1000) maik      (1000)     1799 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/locales/update.py
--rw-r--r--   0 maik      (1000) maik      (1000)      260 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/permissions.zcml
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.573001 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.577001 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/default/
--rw-r--r--   0 maik      (1000) maik      (1000)      201 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/default/browserlayer.xml
--rw-r--r--   0 maik      (1000) maik      (1000)      105 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/default/catalog.xml
--rw-r--r--   0 maik      (1000) maik      (1000)      195 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/default/metadata.xml
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.577001 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/default/registry/
--rw-r--r--   0 maik      (1000) maik      (1000)      183 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/default/registry/main.xml
--rw-r--r--   0 maik      (1000) maik      (1000)      118 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/default/rolemap.xml
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.577001 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/default/types/
--rw-r--r--   0 maik      (1000) maik      (1000)      339 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/default/types/Collection.xml
--rw-r--r--   0 maik      (1000) maik      (1000)      448 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/default/types/Folder.xml
--rw-r--r--   0 maik      (1000) maik      (1000)      303 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/default/types.xml
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.577001 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/uninstall/
--rw-r--r--   0 maik      (1000) maik      (1000)      135 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maik      (1000) maik      (1000)      800 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/setuphandlers.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1619 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/testing.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.577001 collective.accordionviews-1.1b4/src/collective/accordionviews/tests/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/tests/__init__.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.579001 collective.accordionviews-1.1b4/src/collective/accordionviews/tests/robot/
--rw-r--r--   0 maik      (1000) maik      (1000)     2031 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/tests/robot/test_example.robot
--rw-r--r--   0 maik      (1000) maik      (1000)      971 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_robot.py
--rw-r--r--   0 maik      (1000) maik      (1000)     2537 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_setup.py
--rw-r--r--   0 maik      (1000) maik      (1000)      886 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_upgrade_step_1001.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1511 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_view_accordion_folders_view.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1578 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_view_accordion_view.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1578 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_view_slideshow_view.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1560 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_view_tabbed_view.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.579001 collective.accordionviews-1.1b4/src/collective/accordionviews/upgrades/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.579001 collective.accordionviews-1.1b4/src/collective/accordionviews/upgrades/1001/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/upgrades/1001/.gitkeep
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/upgrades/1001/metadata.txt
--rw-r--r--   0 maik      (1000) maik      (1000)      848 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/upgrades/1001.zcml
--rw-r--r--   0 maik      (1000) maik      (1000)       97 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/upgrades/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      217 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/upgrades/base.py
--rw-r--r--   0 maik      (1000) maik      (1000)      187 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/upgrades/configure.zcml
--rw-r--r--   0 maik      (1000) maik      (1000)      283 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/upgrades/v1001.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.579001 collective.accordionviews-1.1b4/src/collective/accordionviews/views/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/views/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)     2176 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/views/accordion_folders_view.pt
--rw-r--r--   0 maik      (1000) maik      (1000)     1330 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/views/accordion_folders_view.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1814 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/views/accordion_view.pt
--rw-r--r--   0 maik      (1000) maik      (1000)     1325 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/views/accordion_view.py
--rw-r--r--   0 maik      (1000) maik      (1000)     2021 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/views/configure.zcml
--rw-r--r--   0 maik      (1000) maik      (1000)     1978 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/views/slides_view.pt
--rw-r--r--   0 maik      (1000) maik      (1000)      653 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/views/slides_view.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1434 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/views/tabbed_view.pt
--rw-r--r--   0 maik      (1000) maik      (1000)     1938 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective/accordionviews/views/tabbed_view.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2022-10-31 15:47:16.575001 collective.accordionviews-1.1b4/src/collective.accordionviews.egg-info/
--rw-r--r--   0 maik      (1000) maik      (1000)     4461 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective.accordionviews.egg-info/PKG-INFO
--rw-r--r--   0 maik      (1000) maik      (1000)     3491 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective.accordionviews.egg-info/SOURCES.txt
--rw-r--r--   0 maik      (1000) maik      (1000)        1 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective.accordionviews.egg-info/dependency_links.txt
--rw-r--r--   0 maik      (1000) maik      (1000)      150 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective.accordionviews.egg-info/entry_points.txt
--rw-r--r--   0 maik      (1000) maik      (1000)       11 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective.accordionviews.egg-info/namespace_packages.txt
--rw-r--r--   0 maik      (1000) maik      (1000)        1 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective.accordionviews.egg-info/not-zip-safe
--rw-r--r--   0 maik      (1000) maik      (1000)      159 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective.accordionviews.egg-info/requires.txt
--rw-r--r--   0 maik      (1000) maik      (1000)       11 2022-10-31 15:47:16.000000 collective.accordionviews-1.1b4/src/collective.accordionviews.egg-info/top_level.txt
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.888399 collective.accordionviews-1.2/
+-rw-r--r--   0 maik      (1000) maik      (1000)      722 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/CHANGES.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)       59 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/CONTRIBUTORS.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)     1338 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/DEVELOP.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)    18092 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/LICENSE.GPL
+-rw-r--r--   0 maik      (1000) maik      (1000)      671 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/LICENSE.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)      210 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/MANIFEST.in
+-rw-r--r--   0 maik      (1000) maik      (1000)     4661 2023-07-28 07:06:49.888399 collective.accordionviews-1.2/PKG-INFO
+-rw-r--r--   0 maik      (1000) maik      (1000)     2695 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/README.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.884399 collective.accordionviews-1.2/docs/
+-rw-r--r--   0 maik      (1000) maik      (1000)     7937 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/docs/conf.py
+-rw-r--r--   0 maik      (1000) maik      (1000)       98 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/docs/index.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)      334 2023-07-28 07:06:49.888399 collective.accordionviews-1.2/setup.cfg
+-rw-r--r--   0 maik      (1000) maik      (1000)     2554 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/setup.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.882399 collective.accordionviews-1.2/src/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.884399 collective.accordionviews-1.2/src/collective/
+-rw-r--r--   0 maik      (1000) maik      (1000)       80 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/__init__.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.884399 collective.accordionviews-1.2/src/collective/accordionviews/
+-rw-r--r--   0 maik      (1000) maik      (1000)      141 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/__init__.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.884399 collective.accordionviews-1.2/src/collective/accordionviews/browser/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/browser/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      618 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/browser/configure.zcml
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.884399 collective.accordionviews-1.2/src/collective/accordionviews/browser/overrides/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/browser/overrides/.gitkeep
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.884399 collective.accordionviews-1.2/src/collective/accordionviews/browser/static/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/browser/static/.gitkeep
+-rw-r--r--   0 maik      (1000) maik      (1000)     1476 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/configure.zcml
+-rw-r--r--   0 maik      (1000) maik      (1000)      274 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/interfaces.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.886399 collective.accordionviews-1.2/src/collective/accordionviews/locales/
+-rw-r--r--   0 maik      (1000) maik      (1000)      611 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/locales/README.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/locales/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1206 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/locales/collective.accordionviews.pot
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.882399 collective.accordionviews-1.2/src/collective/accordionviews/locales/de/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.886399 collective.accordionviews-1.2/src/collective/accordionviews/locales/de/LC_MESSAGES/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1122 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/locales/de/LC_MESSAGES/collective.accordionviews.po
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.882399 collective.accordionviews-1.2/src/collective/accordionviews/locales/en/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.886399 collective.accordionviews-1.2/src/collective/accordionviews/locales/en/LC_MESSAGES/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1079 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/locales/en/LC_MESSAGES/collective.accordionviews.po
+-rw-r--r--   0 maik      (1000) maik      (1000)      650 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/locales/manual.pot
+-rw-r--r--   0 maik      (1000) maik      (1000)     1799 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/locales/update.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      260 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/permissions.zcml
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.882399 collective.accordionviews-1.2/src/collective/accordionviews/profiles/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.886399 collective.accordionviews-1.2/src/collective/accordionviews/profiles/default/
+-rw-r--r--   0 maik      (1000) maik      (1000)      201 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/profiles/default/browserlayer.xml
+-rw-r--r--   0 maik      (1000) maik      (1000)      105 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/profiles/default/catalog.xml
+-rw-r--r--   0 maik      (1000) maik      (1000)      195 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/profiles/default/metadata.xml
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.886399 collective.accordionviews-1.2/src/collective/accordionviews/profiles/default/registry/
+-rw-r--r--   0 maik      (1000) maik      (1000)      183 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/profiles/default/registry/main.xml
+-rw-r--r--   0 maik      (1000) maik      (1000)      118 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/profiles/default/rolemap.xml
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.886399 collective.accordionviews-1.2/src/collective/accordionviews/profiles/default/types/
+-rw-r--r--   0 maik      (1000) maik      (1000)      339 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/profiles/default/types/Collection.xml
+-rw-r--r--   0 maik      (1000) maik      (1000)      448 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/profiles/default/types/Folder.xml
+-rw-r--r--   0 maik      (1000) maik      (1000)      303 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/profiles/default/types.xml
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.886399 collective.accordionviews-1.2/src/collective/accordionviews/profiles/uninstall/
+-rw-r--r--   0 maik      (1000) maik      (1000)      135 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maik      (1000) maik      (1000)      800 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/setuphandlers.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1619 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/testing.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.886399 collective.accordionviews-1.2/src/collective/accordionviews/tests/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/tests/__init__.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.886399 collective.accordionviews-1.2/src/collective/accordionviews/tests/robot/
+-rw-r--r--   0 maik      (1000) maik      (1000)     2031 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/tests/robot/test_example.robot
+-rw-r--r--   0 maik      (1000) maik      (1000)      971 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/tests/test_robot.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     2537 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/tests/test_setup.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      886 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/tests/test_upgrade_step_1001.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1511 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/tests/test_view_accordion_folders_view.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1578 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/tests/test_view_accordion_view.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1578 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/tests/test_view_slideshow_view.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1560 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/tests/test_view_tabbed_view.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.888399 collective.accordionviews-1.2/src/collective/accordionviews/upgrades/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.888399 collective.accordionviews-1.2/src/collective/accordionviews/upgrades/1001/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/upgrades/1001/.gitkeep
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/upgrades/1001/metadata.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)      848 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/upgrades/1001.zcml
+-rw-r--r--   0 maik      (1000) maik      (1000)       97 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/upgrades/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      217 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/upgrades/base.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      187 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/upgrades/configure.zcml
+-rw-r--r--   0 maik      (1000) maik      (1000)      283 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/upgrades/v1001.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.888399 collective.accordionviews-1.2/src/collective/accordionviews/views/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/views/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     2176 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/views/accordion_folders_view.pt
+-rw-r--r--   0 maik      (1000) maik      (1000)     1330 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/views/accordion_folders_view.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1819 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/views/accordion_view.pt
+-rw-r--r--   0 maik      (1000) maik      (1000)     1377 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/views/accordion_view.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     2021 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/views/configure.zcml
+-rw-r--r--   0 maik      (1000) maik      (1000)     1978 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/views/slides_view.pt
+-rw-r--r--   0 maik      (1000) maik      (1000)      653 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/views/slides_view.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1434 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/views/tabbed_view.pt
+-rw-r--r--   0 maik      (1000) maik      (1000)     1938 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective/accordionviews/views/tabbed_view.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-07-28 07:06:49.884399 collective.accordionviews-1.2/src/collective.accordionviews.egg-info/
+-rw-r--r--   0 maik      (1000) maik      (1000)     4661 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective.accordionviews.egg-info/PKG-INFO
+-rw-r--r--   0 maik      (1000) maik      (1000)     3491 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective.accordionviews.egg-info/SOURCES.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)        1 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective.accordionviews.egg-info/dependency_links.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)      150 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective.accordionviews.egg-info/entry_points.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)       11 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective.accordionviews.egg-info/namespace_packages.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)        1 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective.accordionviews.egg-info/not-zip-safe
+-rw-r--r--   0 maik      (1000) maik      (1000)      159 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective.accordionviews.egg-info/requires.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)       11 2023-07-28 07:06:49.000000 collective.accordionviews-1.2/src/collective.accordionviews.egg-info/top_level.txt
```

### Comparing `collective.accordionviews-1.1b4/CHANGES.rst` & `collective.accordionviews-1.2/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 Changelog
 =========
 
 
+1.2 (2023-07-28)
+----------------
+
+- prevent error when #content-core was not found in clean_html method
+  [MrTango]
+
+
+1.1 (2022-12-22)
+----------------
+
+- fix accordion collapsed markers
+  [MrTango]
+
+
 1.1b4 (2022-10-31)
 ------------------
 
 - Add slideshow_view for Folder
   [MrTango]
```

### Comparing `collective.accordionviews-1.1b4/DEVELOP.rst` & `collective.accordionviews-1.2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/LICENSE.GPL` & `collective.accordionviews-1.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/LICENSE.rst` & `collective.accordionviews-1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/PKG-INFO` & `collective.accordionviews-1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.accordionviews
-Version: 1.1b4
+Version: 1.2
 Summary: Accordion views for Plone CMS, which can be used on Folders and Collections.
 Home-page: https://github.com/collective/collective.accordionviews
 Author: Maik Derstappen
 Author-email: md@derico.de
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.accordionviews
 Project-URL: Source, https://github.com/collective/collective.accordionviews
@@ -137,14 +137,28 @@
 - Maik Derstappen, md@derico.de
 
 
 Changelog
 =========
 
 
+1.2 (2023-07-28)
+----------------
+
+- prevent error when #content-core was not found in clean_html method
+  [MrTango]
+
+
+1.1 (2022-12-22)
+----------------
+
+- fix accordion collapsed markers
+  [MrTango]
+
+
 1.1b4 (2022-10-31)
 ------------------
 
 - Add slideshow_view for Folder
   [MrTango]
```

### Comparing `collective.accordionviews-1.1b4/README.rst` & `collective.accordionviews-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/docs/conf.py` & `collective.accordionviews-1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/setup.py` & `collective.accordionviews-1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.accordionviews",
-    version="1.1b4",
+    version="1.2",
     description="Accordion views for Plone CMS, which can be used on Folders and Collections.",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/browser/configure.zcml` & `collective.accordionviews-1.2/src/collective/accordionviews/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/configure.zcml` & `collective.accordionviews-1.2/src/collective/accordionviews/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/locales/README.rst` & `collective.accordionviews-1.2/src/collective/accordionviews/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/locales/collective.accordionviews.pot` & `collective.accordionviews-1.2/src/collective/accordionviews/locales/collective.accordionviews.pot`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/locales/de/LC_MESSAGES/collective.accordionviews.po` & `collective.accordionviews-1.2/src/collective/accordionviews/locales/de/LC_MESSAGES/collective.accordionviews.po`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/locales/en/LC_MESSAGES/collective.accordionviews.po` & `collective.accordionviews-1.2/src/collective/accordionviews/locales/en/LC_MESSAGES/collective.accordionviews.po`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/locales/manual.pot` & `collective.accordionviews-1.2/src/collective/accordionviews/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/locales/update.py` & `collective.accordionviews-1.2/src/collective/accordionviews/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/setuphandlers.py` & `collective.accordionviews-1.2/src/collective/accordionviews/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/testing.py` & `collective.accordionviews-1.2/src/collective/accordionviews/testing.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/tests/robot/test_example.robot` & `collective.accordionviews-1.2/src/collective/accordionviews/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_robot.py` & `collective.accordionviews-1.2/src/collective/accordionviews/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_setup.py` & `collective.accordionviews-1.2/src/collective/accordionviews/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_upgrade_step_1001.py` & `collective.accordionviews-1.2/src/collective/accordionviews/tests/test_upgrade_step_1001.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_view_accordion_folders_view.py` & `collective.accordionviews-1.2/src/collective/accordionviews/tests/test_view_accordion_folders_view.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_view_accordion_view.py` & `collective.accordionviews-1.2/src/collective/accordionviews/tests/test_view_accordion_view.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_view_slideshow_view.py` & `collective.accordionviews-1.2/src/collective/accordionviews/tests/test_view_slideshow_view.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/tests/test_view_tabbed_view.py` & `collective.accordionviews-1.2/src/collective/accordionviews/tests/test_view_tabbed_view.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/upgrades/1001.zcml` & `collective.accordionviews-1.2/src/collective/accordionviews/upgrades/1001.zcml`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/views/accordion_folders_view.pt` & `collective.accordionviews-1.2/src/collective/accordionviews/views/accordion_folders_view.pt`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/views/accordion_folders_view.py` & `collective.accordionviews-1.2/src/collective/accordionviews/views/accordion_folders_view.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/views/accordion_view.pt` & `collective.accordionviews-1.2/src/collective/accordionviews/views/accordion_view.pt`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       <metal:block define-macro="content-core">
         <div class="accordion"
           id="accordion-${python: context.UID()}">
           <div tal:repeat="item python:context.restrictedTraverse('@@contentlisting')(exclude_from_nav=False)"
             class="accordion-item">
             <h2 class="accordion-header"
               id="heading-${python: item.uuid()}">
-              <button class="accordion-button ${python: repeat.item.start and 'collapsed' or ''}"
+              <button class="accordion-button ${python: repeat.item.start and 'first' or 'collapsed'}"
                 type="button"
                 data-bs-toggle="collapse"
                 data-bs-target="#collapse-${python: item.uuid()}"
                 aria-expanded="${python: repeat.item.start and 'true' or 'false'}"
                 aria-controls="collapse-${python: item.uuid()}">
               ${item/Title}
               </button>
```

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/views/accordion_view.py` & `collective.accordionviews-1.2/src/collective/accordionviews/views/accordion_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,8 +26,10 @@
         alsoProvides(self.context_view, IViewView)
         html_str = self.context_view()
         return self._clean_html(html_str)
 
     def _clean_html(self, raw_html):
         content_soup = BeautifulSoup(raw_html, "html.parser")
         content = content_soup.select_one("#content-core")
+        if not content:
+            return raw_html
         return content.prettify()
```

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/views/configure.zcml` & `collective.accordionviews-1.2/src/collective/accordionviews/views/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/views/slides_view.pt` & `collective.accordionviews-1.2/src/collective/accordionviews/views/slides_view.pt`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/views/slides_view.py` & `collective.accordionviews-1.2/src/collective/accordionviews/views/slides_view.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/views/tabbed_view.pt` & `collective.accordionviews-1.2/src/collective/accordionviews/views/tabbed_view.pt`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective/accordionviews/views/tabbed_view.py` & `collective.accordionviews-1.2/src/collective/accordionviews/views/tabbed_view.py`

 * *Files identical despite different names*

### Comparing `collective.accordionviews-1.1b4/src/collective.accordionviews.egg-info/PKG-INFO` & `collective.accordionviews-1.2/src/collective.accordionviews.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.accordionviews
-Version: 1.1b4
+Version: 1.2
 Summary: Accordion views for Plone CMS, which can be used on Folders and Collections.
 Home-page: https://github.com/collective/collective.accordionviews
 Author: Maik Derstappen
 Author-email: md@derico.de
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.accordionviews
 Project-URL: Source, https://github.com/collective/collective.accordionviews
@@ -137,14 +137,28 @@
 - Maik Derstappen, md@derico.de
 
 
 Changelog
 =========
 
 
+1.2 (2023-07-28)
+----------------
+
+- prevent error when #content-core was not found in clean_html method
+  [MrTango]
+
+
+1.1 (2022-12-22)
+----------------
+
+- fix accordion collapsed markers
+  [MrTango]
+
+
 1.1b4 (2022-10-31)
 ------------------
 
 - Add slideshow_view for Folder
   [MrTango]
```

### Comparing `collective.accordionviews-1.1b4/src/collective.accordionviews.egg-info/SOURCES.txt` & `collective.accordionviews-1.2/src/collective.accordionviews.egg-info/SOURCES.txt`

 * *Files identical despite different names*

