# Comparing `tmp/collective.abovecontentbodyportlets-1.0.0a1.tar.gz` & `tmp/collective.abovecontentbodyportlets-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.abovecontentbodyportlets-1.0.0a1.tar", last modified: Fri Jun 23 20:32:30 2023, max compression
+gzip compressed data, was "collective.abovecontentbodyportlets-1.0.0a2.tar", last modified: Fri Jul 28 14:38:43 2023, max compression
```

## Comparing `collective.abovecontentbodyportlets-1.0.0a1.tar` & `collective.abovecontentbodyportlets-1.0.0a2.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.912253 collective.abovecontentbodyportlets-1.0.0a1/
--rw-r--r--   0 maurits    (501) staff       (20)      103 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1338 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/DEVELOP.rst
--rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      682 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)       86 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     2723 2023-06-23 20:32:30.912366 collective.abovecontentbodyportlets-1.0.0a1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1323 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      349 2023-06-23 20:32:30.912922 collective.abovecontentbodyportlets-1.0.0a1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2094 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.896288 collective.abovecontentbodyportlets-1.0.0a1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.900885 collective.abovecontentbodyportlets-1.0.0a1/src/collective/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.906344 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/
--rw-r--r--   0 maurits    (501) staff       (20)      128 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1494 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      311 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.907710 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      993 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/collective.abovecontentbodyportlets.pot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.896981 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/en/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.908118 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/en/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      858 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.897252 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/nl/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.909106 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)     1210 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po
--rw-r--r--   0 maurits    (501) staff       (20)      861 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/plone.po
--rw-r--r--   0 maurits    (501) staff       (20)      840 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/plone.pot
--rwxr-xr-x   0 maurits    (501) staff       (20)      751 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/update.sh
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.897675 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.910109 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      224 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)       88 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      295 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/profiles/default/portlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.910644 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      138 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      327 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/profiles/uninstall/portlets.xml
--rw-r--r--   0 maurits    (501) staff       (20)      788 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1270 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.912008 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3151 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/tests/test_portlet_manager.py
--rw-r--r--   0 maurits    (501) staff       (20)     3249 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      194 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/viewlet.pt
--rw-r--r--   0 maurits    (501) staff       (20)      568 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/viewlet.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:32:30.903685 collective.abovecontentbodyportlets-1.0.0a1/src/collective.abovecontentbodyportlets.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     2723 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective.abovecontentbodyportlets.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2061 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective.abovecontentbodyportlets.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective.abovecontentbodyportlets.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective.abovecontentbodyportlets.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective.abovecontentbodyportlets.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective.abovecontentbodyportlets.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       61 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective.abovecontentbodyportlets.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-06-23 20:32:30.000000 collective.abovecontentbodyportlets-1.0.0a1/src/collective.abovecontentbodyportlets.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.843742 collective.abovecontentbodyportlets-1.0.0a2/
+-rw-r--r--   0 maurits    (501) staff       (20)      269 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1338 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/DEVELOP.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      682 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       86 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     2889 2023-07-28 14:38:43.843839 collective.abovecontentbodyportlets-1.0.0a2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1323 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      349 2023-07-28 14:38:43.844292 collective.abovecontentbodyportlets-1.0.0a2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2094 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.828935 collective.abovecontentbodyportlets-1.0.0a2/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.833755 collective.abovecontentbodyportlets-1.0.0a2/src/collective/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.838237 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/
+-rw-r--r--   0 maurits    (501) staff       (20)      128 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1494 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      311 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.839305 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      993 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/collective.abovecontentbodyportlets.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.829898 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/en/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.839880 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/en/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      597 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/en/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      858 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.830236 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.840971 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     1022 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     1210 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po
+-rw-r--r--   0 maurits    (501) staff       (20)      600 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      861 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/plone.po
+-rw-r--r--   0 maurits    (501) staff       (20)      840 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/plone.pot
+-rwxr-xr-x   0 maurits    (501) staff       (20)      751 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/update.sh
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.830946 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.841942 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      224 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       88 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      295 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/profiles/default/portlets.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.842559 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      138 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      327 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/profiles/uninstall/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      788 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1270 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.843515 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3151 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/tests/test_portlet_manager.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3249 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)      153 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/viewlet.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      568 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/viewlet.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-28 14:38:43.836196 collective.abovecontentbodyportlets-1.0.0a2/src/collective.abovecontentbodyportlets.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     2889 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective.abovecontentbodyportlets.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2307 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective.abovecontentbodyportlets.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective.abovecontentbodyportlets.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective.abovecontentbodyportlets.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective.abovecontentbodyportlets.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective.abovecontentbodyportlets.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       61 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective.abovecontentbodyportlets.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-07-28 14:38:43.000000 collective.abovecontentbodyportlets-1.0.0a2/src/collective.abovecontentbodyportlets.egg-info/top_level.txt
```

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/DEVELOP.rst` & `collective.abovecontentbodyportlets-1.0.0a2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/LICENSE.GPL` & `collective.abovecontentbodyportlets-1.0.0a2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/LICENSE.rst` & `collective.abovecontentbodyportlets-1.0.0a2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/PKG-INFO` & `collective.abovecontentbodyportlets-1.0.0a2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.abovecontentbodyportlets
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Content Type to show an abovecontentbodyportlets
 Home-page: https://github.com/collective/collective.abovecontentbodyportlets
 Author: Maurits van Rees
 Author-email: m.van.rees@zestsoftware.nl
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.abovecontentbodyportlets/
 Project-URL: Source, https://github.com/collective/collective.abovecontentbodyportlets
@@ -85,12 +85,20 @@
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
-  [mauritsvanrees]
+  [maurits]
```

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/README.rst` & `collective.abovecontentbodyportlets-1.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/setup.py` & `collective.abovecontentbodyportlets-1.0.0a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.abovecontentbodyportlets",
-    version="1.0.0a1",
+    version="1.0.0a2",
     description="Content Type to show an abovecontentbodyportlets",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/configure.zcml` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/collective.abovecontentbodyportlets.pot` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/collective.abovecontentbodyportlets.pot`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/en/LC_MESSAGES/plone.po` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/plone.po` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/plone.pot` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/locales/update.sh` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/setuphandlers.py` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/testing.py` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/testing.py`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/tests/test_portlet_manager.py` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/tests/test_portlet_manager.py`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/tests/test_setup.py` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective/abovecontentbodyportlets/viewlet.py` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective/abovecontentbodyportlets/viewlet.py`

 * *Files identical despite different names*

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective.abovecontentbodyportlets.egg-info/PKG-INFO` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective.abovecontentbodyportlets.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.abovecontentbodyportlets
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Content Type to show an abovecontentbodyportlets
 Home-page: https://github.com/collective/collective.abovecontentbodyportlets
 Author: Maurits van Rees
 Author-email: m.van.rees@zestsoftware.nl
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.abovecontentbodyportlets/
 Project-URL: Source, https://github.com/collective/collective.abovecontentbodyportlets
@@ -85,12 +85,20 @@
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
-  [mauritsvanrees]
+  [maurits]
```

### Comparing `collective.abovecontentbodyportlets-1.0.0a1/src/collective.abovecontentbodyportlets.egg-info/SOURCES.txt` & `collective.abovecontentbodyportlets-1.0.0a2/src/collective.abovecontentbodyportlets.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,19 @@
 src/collective/abovecontentbodyportlets/testing.py
 src/collective/abovecontentbodyportlets/viewlet.pt
 src/collective/abovecontentbodyportlets/viewlet.py
 src/collective/abovecontentbodyportlets/locales/__init__.py
 src/collective/abovecontentbodyportlets/locales/collective.abovecontentbodyportlets.pot
 src/collective/abovecontentbodyportlets/locales/plone.pot
 src/collective/abovecontentbodyportlets/locales/update.sh
+src/collective/abovecontentbodyportlets/locales/en/LC_MESSAGES/plone.mo
 src/collective/abovecontentbodyportlets/locales/en/LC_MESSAGES/plone.po
+src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.mo
 src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/collective.abovecontentbodyportlets.po
+src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/plone.mo
 src/collective/abovecontentbodyportlets/locales/nl/LC_MESSAGES/plone.po
 src/collective/abovecontentbodyportlets/profiles/default/browserlayer.xml
 src/collective/abovecontentbodyportlets/profiles/default/metadata.xml
 src/collective/abovecontentbodyportlets/profiles/default/portlets.xml
 src/collective/abovecontentbodyportlets/profiles/uninstall/browserlayer.xml
 src/collective/abovecontentbodyportlets/profiles/uninstall/portlets.xml
 src/collective/abovecontentbodyportlets/tests/__init__.py
```

