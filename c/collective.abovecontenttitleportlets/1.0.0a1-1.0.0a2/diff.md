# Comparing `tmp/collective.abovecontenttitleportlets-1.0.0a1.tar.gz` & `tmp/collective.abovecontenttitleportlets-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.abovecontenttitleportlets-1.0.0a1.tar", last modified: Fri Jun 23 21:05:13 2023, max compression
+gzip compressed data, was "collective.abovecontenttitleportlets-1.0.0a2.tar", last modified: Fri Jul 28 14:34:49 2023, max compression
```

## Comparing `collective.abovecontenttitleportlets-1.0.0a1.tar` & `collective.abovecontenttitleportlets-1.0.0a2.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.435701 collective.abovecontenttitleportlets-1.0.0a1/
--rw-r--r--   0 maurits    (501) staff       (20)      103 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1338 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/DEVELOP.rst
--rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      683 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)       86 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     2855 2023-06-23 21:05:13.435955 collective.abovecontenttitleportlets-1.0.0a1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1449 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      349 2023-06-23 21:05:13.436547 collective.abovecontenttitleportlets-1.0.0a1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2101 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.421569 collective.abovecontenttitleportlets-1.0.0a1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.425982 collective.abovecontenttitleportlets-1.0.0a1/src/collective/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.430727 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/
--rw-r--r--   0 maurits    (501) staff       (20)      129 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1503 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      312 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.432092 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      998 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/collective.abovecontentbodyportlets.pot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.422248 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/en/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.432386 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/en/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      861 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.422692 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/nl/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.433019 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)     1220 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po
--rw-r--r--   0 maurits    (501) staff       (20)      864 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/plone.po
--rw-r--r--   0 maurits    (501) staff       (20)      842 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/plone.pot
--rwxr-xr-x   0 maurits    (501) staff       (20)      754 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/update.sh
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.423116 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.433968 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      227 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)       88 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      297 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/profiles/default/portlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.434662 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      139 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      329 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/profiles/uninstall/portlets.xml
--rw-r--r--   0 maurits    (501) staff       (20)      790 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1277 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.435498 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3230 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/tests/test_portlet_manager.py
--rw-r--r--   0 maurits    (501) staff       (20)     3266 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      195 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/viewlet.pt
--rw-r--r--   0 maurits    (501) staff       (20)      570 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/viewlet.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 21:05:13.428790 collective.abovecontenttitleportlets-1.0.0a1/src/collective.abovecontenttitleportlets.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     2855 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective.abovecontenttitleportlets.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2091 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective.abovecontenttitleportlets.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective.abovecontenttitleportlets.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective.abovecontenttitleportlets.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective.abovecontenttitleportlets.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective.abovecontenttitleportlets.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       61 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective.abovecontenttitleportlets.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-06-23 21:05:13.000000 collective.abovecontenttitleportlets-1.0.0a1/src/collective.abovecontenttitleportlets.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.467327 collective.abovecontenttitleportlets-1.0.0a2/
+-rw-r--r--   0 maurits    (501) staff       (20)      276 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1338 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/DEVELOP.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      683 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       86 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     3028 2023-07-28 14:34:49.467433 collective.abovecontenttitleportlets-1.0.0a2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1449 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      349 2023-07-28 14:34:49.467846 collective.abovecontenttitleportlets-1.0.0a2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2101 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.453199 collective.abovecontenttitleportlets-1.0.0a2/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.457484 collective.abovecontenttitleportlets-1.0.0a2/src/collective/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.462216 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/
+-rw-r--r--   0 maurits    (501) staff       (20)      129 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1503 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      312 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.463168 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      998 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/collective.abovecontentbodyportlets.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.453636 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/en/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.463815 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/en/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      600 2023-07-28 14:34:49.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/en/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      861 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.453836 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.464987 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     1032 2023-07-28 14:34:49.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     1220 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po
+-rw-r--r--   0 maurits    (501) staff       (20)      603 2023-07-28 14:34:49.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      864 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/plone.po
+-rw-r--r--   0 maurits    (501) staff       (20)      842 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/plone.pot
+-rwxr-xr-x   0 maurits    (501) staff       (20)      754 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/update.sh
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.454143 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.465843 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      227 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       88 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      297 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/profiles/default/portlets.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.466346 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      139 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      329 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/profiles/uninstall/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      790 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1277 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.467091 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3230 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/tests/test_portlet_manager.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3266 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)      155 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/viewlet.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      570 2023-07-28 14:34:48.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/viewlet.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:34:49.460204 collective.abovecontenttitleportlets-1.0.0a2/src/collective.abovecontenttitleportlets.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     3028 2023-07-28 14:34:49.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective.abovecontenttitleportlets.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2340 2023-07-28 14:34:49.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective.abovecontenttitleportlets.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-28 14:34:49.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective.abovecontenttitleportlets.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-07-28 14:34:49.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective.abovecontenttitleportlets.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-07-28 14:34:49.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective.abovecontenttitleportlets.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-28 14:34:49.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective.abovecontenttitleportlets.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       61 2023-07-28 14:34:49.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective.abovecontenttitleportlets.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-07-28 14:34:49.000000 collective.abovecontenttitleportlets-1.0.0a2/src/collective.abovecontenttitleportlets.egg-info/top_level.txt
```

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/DEVELOP.rst` & `collective.abovecontenttitleportlets-1.0.0a2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/LICENSE.GPL` & `collective.abovecontenttitleportlets-1.0.0a2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/LICENSE.rst` & `collective.abovecontenttitleportlets-1.0.0a2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/PKG-INFO` & `collective.abovecontenttitleportlets-1.0.0a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.abovecontenttitleportlets
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Content Type to show an abovecontenttitleportlets
 Home-page: https://github.com/collective/collective.abovecontenttitleportlets
 Author: Maurits van Rees
 Author-email: m.van.rees@zestsoftware.nl
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.abovecontenttitleportlets/
 Project-URL: Source, https://github.com/collective/collective.abovecontenttitleportlets
@@ -87,12 +87,20 @@
 The project is licensed under the GPLv2.
 
 
 Changelog
 =========
 
 
+1.0.0a2 (2023-07-28)
+--------------------
+
+- Removed unneeded div with class col-xs-12 from page template.
+  We already have a surrounding div with class row.
+  [maurits]
+
+
 1.0.0a1 (2023-06-23)
 --------------------
 
 - Initial release.
   [mauritsvanrees]
```

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/README.rst` & `collective.abovecontenttitleportlets-1.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/setup.py` & `collective.abovecontenttitleportlets-1.0.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.abovecontenttitleportlets",
-    version="1.0.0a1",
+    version="1.0.0a2",
     description="Content Type to show an abovecontenttitleportlets",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/configure.zcml` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/collective.abovecontentbodyportlets.pot` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/collective.abovecontentbodyportlets.pot`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/en/LC_MESSAGES/plone.po` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/plone.po` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/plone.pot` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/locales/update.sh` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/setuphandlers.py` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/testing.py` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/testing.py`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/tests/test_portlet_manager.py` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/tests/test_portlet_manager.py`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/tests/test_setup.py` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective/abovecontenttitleportlets/viewlet.py` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective/abovecontenttitleportlets/viewlet.py`

 * *Files identical despite different names*

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective.abovecontenttitleportlets.egg-info/PKG-INFO` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective.abovecontenttitleportlets.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.abovecontenttitleportlets
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Content Type to show an abovecontenttitleportlets
 Home-page: https://github.com/collective/collective.abovecontenttitleportlets
 Author: Maurits van Rees
 Author-email: m.van.rees@zestsoftware.nl
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.abovecontenttitleportlets/
 Project-URL: Source, https://github.com/collective/collective.abovecontenttitleportlets
@@ -87,12 +87,20 @@
 The project is licensed under the GPLv2.
 
 
 Changelog
 =========
 
 
+1.0.0a2 (2023-07-28)
+--------------------
+
+- Removed unneeded div with class col-xs-12 from page template.
+  We already have a surrounding div with class row.
+  [maurits]
+
+
 1.0.0a1 (2023-06-23)
 --------------------
 
 - Initial release.
   [mauritsvanrees]
```

### Comparing `collective.abovecontenttitleportlets-1.0.0a1/src/collective.abovecontenttitleportlets.egg-info/SOURCES.txt` & `collective.abovecontenttitleportlets-1.0.0a2/src/collective.abovecontenttitleportlets.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,19 @@
 src/collective/abovecontenttitleportlets/testing.py
 src/collective/abovecontenttitleportlets/viewlet.pt
 src/collective/abovecontenttitleportlets/viewlet.py
 src/collective/abovecontenttitleportlets/locales/__init__.py
 src/collective/abovecontenttitleportlets/locales/collective.abovecontentbodyportlets.pot
 src/collective/abovecontenttitleportlets/locales/plone.pot
 src/collective/abovecontenttitleportlets/locales/update.sh
+src/collective/abovecontenttitleportlets/locales/en/LC_MESSAGES/plone.mo
 src/collective/abovecontenttitleportlets/locales/en/LC_MESSAGES/plone.po
+src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.mo
 src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po
+src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/plone.mo
 src/collective/abovecontenttitleportlets/locales/nl/LC_MESSAGES/plone.po
 src/collective/abovecontenttitleportlets/profiles/default/browserlayer.xml
 src/collective/abovecontenttitleportlets/profiles/default/metadata.xml
 src/collective/abovecontenttitleportlets/profiles/default/portlets.xml
 src/collective/abovecontenttitleportlets/profiles/uninstall/browserlayer.xml
 src/collective/abovecontenttitleportlets/profiles/uninstall/portlets.xml
 src/collective/abovecontenttitleportlets/tests/__init__.py
```

