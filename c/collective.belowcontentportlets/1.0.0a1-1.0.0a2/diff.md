# Comparing `tmp/collective.belowcontentportlets-1.0.0a1.tar.gz` & `tmp/collective.belowcontentportlets-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.belowcontentportlets-1.0.0a1.tar", last modified: Wed Jun 28 15:53:02 2023, max compression
+gzip compressed data, was "collective.belowcontentportlets-1.0.0a2.tar", last modified: Fri Jul 28 14:50:48 2023, max compression
```

## Comparing `collective.belowcontentportlets-1.0.0a1.tar` & `collective.belowcontentportlets-1.0.0a2.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.096152 collective.belowcontentportlets-1.0.0a1/
--rw-r--r--   0 maurits    (501) staff       (20)      159 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1338 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/DEVELOP.rst
--rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      678 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)       86 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     3022 2023-06-28 15:53:02.096257 collective.belowcontentportlets-1.0.0a1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1590 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      349 2023-06-28 15:53:02.096748 collective.belowcontentportlets-1.0.0a1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2066 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.082666 collective.belowcontentportlets-1.0.0a1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.086882 collective.belowcontentportlets-1.0.0a1/src/collective/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.091555 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/
--rw-r--r--   0 maurits    (501) staff       (20)      124 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1458 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      307 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.092740 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      973 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/collective.abovecontentbodyportlets.pot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.083483 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/en/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.093012 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/en/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      845 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.083767 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/nl/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.093659 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)     1170 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po
--rw-r--r--   0 maurits    (501) staff       (20)      848 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/plone.po
--rw-r--r--   0 maurits    (501) staff       (20)      832 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/plone.pot
--rwxr-xr-x   0 maurits    (501) staff       (20)      739 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/update.sh
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.084208 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.094536 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      212 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)       88 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      287 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/profiles/default/portlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.095176 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      134 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      319 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/profiles/uninstall/portlets.xml
--rw-r--r--   0 maurits    (501) staff       (20)      780 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1242 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.095927 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3112 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/tests/test_portlet_manager.py
--rw-r--r--   0 maurits    (501) staff       (20)     3159 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      190 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/viewlet.pt
--rw-r--r--   0 maurits    (501) staff       (20)      560 2023-06-28 15:53:01.000000 collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/viewlet.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-28 15:53:02.089237 collective.belowcontentportlets-1.0.0a1/src/collective.belowcontentportlets.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     3022 2023-06-28 15:53:02.000000 collective.belowcontentportlets-1.0.0a1/src/collective.belowcontentportlets.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1941 2023-06-28 15:53:02.000000 collective.belowcontentportlets-1.0.0a1/src/collective.belowcontentportlets.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-28 15:53:02.000000 collective.belowcontentportlets-1.0.0a1/src/collective.belowcontentportlets.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-06-28 15:53:02.000000 collective.belowcontentportlets-1.0.0a1/src/collective.belowcontentportlets.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-06-28 15:53:02.000000 collective.belowcontentportlets-1.0.0a1/src/collective.belowcontentportlets.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-28 15:53:02.000000 collective.belowcontentportlets-1.0.0a1/src/collective.belowcontentportlets.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       61 2023-06-28 15:53:02.000000 collective.belowcontentportlets-1.0.0a1/src/collective.belowcontentportlets.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-06-28 15:53:02.000000 collective.belowcontentportlets-1.0.0a1/src/collective.belowcontentportlets.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.516512 collective.belowcontentportlets-1.0.0a2/
+-rw-r--r--   0 maurits    (501) staff       (20)      325 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1338 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/DEVELOP.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      678 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       86 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     3188 2023-07-28 14:50:48.516671 collective.belowcontentportlets-1.0.0a2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1590 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      349 2023-07-28 14:50:48.517204 collective.belowcontentportlets-1.0.0a2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2066 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.503493 collective.belowcontentportlets-1.0.0a2/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.506906 collective.belowcontentportlets-1.0.0a2/src/collective/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.510969 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/
+-rw-r--r--   0 maurits    (501) staff       (20)      124 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1458 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      307 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.512525 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      973 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/collective.abovecontentbodyportlets.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.503939 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/en/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.513294 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/en/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      584 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/en/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      845 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.504139 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.514290 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      982 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     1170 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po
+-rw-r--r--   0 maurits    (501) staff       (20)      587 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      848 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/plone.po
+-rw-r--r--   0 maurits    (501) staff       (20)      832 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/plone.pot
+-rwxr-xr-x   0 maurits    (501) staff       (20)      739 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/update.sh
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.504454 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.515089 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      212 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       88 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      287 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/profiles/default/portlets.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.515672 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      134 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      319 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/profiles/uninstall/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      780 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1242 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.516317 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3112 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/tests/test_portlet_manager.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3159 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)      150 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/viewlet.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      560 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/viewlet.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:50:48.509054 collective.belowcontentportlets-1.0.0a2/src/collective.belowcontentportlets.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     3188 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective.belowcontentportlets.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2175 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective.belowcontentportlets.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective.belowcontentportlets.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective.belowcontentportlets.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective.belowcontentportlets.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective.belowcontentportlets.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       61 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective.belowcontentportlets.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-07-28 14:50:48.000000 collective.belowcontentportlets-1.0.0a2/src/collective.belowcontentportlets.egg-info/top_level.txt
```

### Comparing `collective.belowcontentportlets-1.0.0a1/DEVELOP.rst` & `collective.belowcontentportlets-1.0.0a2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/LICENSE.GPL` & `collective.belowcontentportlets-1.0.0a2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/LICENSE.rst` & `collective.belowcontentportlets-1.0.0a2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/PKG-INFO` & `collective.belowcontentportlets-1.0.0a2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.belowcontentportlets
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Content Type to show an belowcontentportlets
 Home-page: https://github.com/collective/collective.belowcontentportlets
 Author: Maurits van Rees
 Author-email: m.van.rees@zestsoftware.nl
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.belowcontentportlets/
 Project-URL: Source, https://github.com/collective/collective.belowcontentportlets
@@ -90,12 +90,20 @@
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
 1.0.0a1 (2023-06-28)
 --------------------
 
 - Initial release.  Adapted from ``collective.abovecontenttitleportlets``.
-  [mauritsvanrees]
+  [maurits]
```

### Comparing `collective.belowcontentportlets-1.0.0a1/README.rst` & `collective.belowcontentportlets-1.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/setup.py` & `collective.belowcontentportlets-1.0.0a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.belowcontentportlets",
-    version="1.0.0a1",
+    version="1.0.0a2",
     description="Content Type to show an belowcontentportlets",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/configure.zcml` & `collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/collective.abovecontentbodyportlets.pot` & `collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/collective.abovecontentbodyportlets.pot`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/en/LC_MESSAGES/plone.po` & `collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po` & `collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/plone.po` & `collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/plone.pot` & `collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/locales/update.sh` & `collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/setuphandlers.py` & `collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/testing.py` & `collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/testing.py`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/tests/test_portlet_manager.py` & `collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/tests/test_portlet_manager.py`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/tests/test_setup.py` & `collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective/belowcontentportlets/viewlet.py` & `collective.belowcontentportlets-1.0.0a2/src/collective/belowcontentportlets/viewlet.py`

 * *Files identical despite different names*

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective.belowcontentportlets.egg-info/PKG-INFO` & `collective.belowcontentportlets-1.0.0a2/src/collective.belowcontentportlets.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.belowcontentportlets
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Content Type to show an belowcontentportlets
 Home-page: https://github.com/collective/collective.belowcontentportlets
 Author: Maurits van Rees
 Author-email: m.van.rees@zestsoftware.nl
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.belowcontentportlets/
 Project-URL: Source, https://github.com/collective/collective.belowcontentportlets
@@ -90,12 +90,20 @@
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
 1.0.0a1 (2023-06-28)
 --------------------
 
 - Initial release.  Adapted from ``collective.abovecontenttitleportlets``.
-  [mauritsvanrees]
+  [maurits]
```

### Comparing `collective.belowcontentportlets-1.0.0a1/src/collective.belowcontentportlets.egg-info/SOURCES.txt` & `collective.belowcontentportlets-1.0.0a2/src/collective.belowcontentportlets.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,19 @@
 src/collective/belowcontentportlets/testing.py
 src/collective/belowcontentportlets/viewlet.pt
 src/collective/belowcontentportlets/viewlet.py
 src/collective/belowcontentportlets/locales/__init__.py
 src/collective/belowcontentportlets/locales/collective.abovecontentbodyportlets.pot
 src/collective/belowcontentportlets/locales/plone.pot
 src/collective/belowcontentportlets/locales/update.sh
+src/collective/belowcontentportlets/locales/en/LC_MESSAGES/plone.mo
 src/collective/belowcontentportlets/locales/en/LC_MESSAGES/plone.po
+src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.mo
 src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po
+src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/plone.mo
 src/collective/belowcontentportlets/locales/nl/LC_MESSAGES/plone.po
 src/collective/belowcontentportlets/profiles/default/browserlayer.xml
 src/collective/belowcontentportlets/profiles/default/metadata.xml
 src/collective/belowcontentportlets/profiles/default/portlets.xml
 src/collective/belowcontentportlets/profiles/uninstall/browserlayer.xml
 src/collective/belowcontentportlets/profiles/uninstall/portlets.xml
 src/collective/belowcontentportlets/tests/__init__.py
```

