# Comparing `tmp/collective.captchacontactinfo-3.0.0.tar.gz` & `tmp/collective.captchacontactinfo-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.captchacontactinfo-3.0.0.tar", last modified: Thu Nov  3 15:37:02 2022, max compression
+gzip compressed data, was "dist/collective.captchacontactinfo-3.0.1.tar", last modified: Fri Jul 28 12:37:32 2023, max compression
```

## Comparing `collective.captchacontactinfo-3.0.0.tar` & `collective.captchacontactinfo-3.0.1.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.281029 collective.captchacontactinfo-3.0.0/
--rw-r--r--   0 cekk       (501) staff       (20)      110 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     4959 2022-11-03 15:37:02.280782 collective.captchacontactinfo-3.0.0/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     1298 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/README.rst
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.267865 collective.captchacontactinfo-3.0.0/collective/
--rw-r--r--   0 cekk       (501) staff       (20)      244 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.272193 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/
--rw-r--r--   0 cekk       (501) staff       (20)      155 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.272943 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/
--rw-r--r--   0 cekk       (501) staff       (20)       23 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.273709 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/ajax/
--rw-r--r--   0 cekk       (501) staff       (20)       23 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/ajax/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      457 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/ajax/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      678 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/ajax/utils.py
--rw-r--r--   0 cekk       (501) staff       (20)      671 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1151 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/contact_form_view.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.265267 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/static/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.273976 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/static/css/
--rw-r--r--   0 cekk       (501) staff       (20)      191 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/static/css/captchacontactinfo.css
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.274229 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/static/scripts/
--rw-r--r--   0 cekk       (501) staff       (20)     1132 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/static/scripts/policy_ajax.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.274482 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/templates/
--rw-r--r--   0 cekk       (501) staff       (20)     1858 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/templates/contact-info.pt
--rw-r--r--   0 cekk       (501) staff       (20)     1246 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.275772 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/controlpanel/
--rw-r--r--   0 cekk       (501) staff       (20)       23 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/controlpanel/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      541 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/controlpanel/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      704 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/controlpanel/interfaces.py
--rw-r--r--   0 cekk       (501) staff       (20)      618 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/controlpanel/view.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      413 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/i18n.sh
--rw-r--r--   0 cekk       (501) staff       (20)      269 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.276072 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/locales/
--rw-r--r--   0 cekk       (501) staff       (20)     2222 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/locales/collective.captchacontactinfo.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.265918 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/locales/de/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.276714 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/locales/de/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)      663 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/locales/de/LC_MESSAGES/collective.captchacontactinfo.mo
--rw-r--r--   0 cekk       (501) staff       (20)     2314 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/locales/de/LC_MESSAGES/collective.captchacontactinfo.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.266152 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.277347 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     1280 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/locales/it/LC_MESSAGES/collective.captchacontactinfo.mo
--rw-r--r--   0 cekk       (501) staff       (20)     2634 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/locales/it/LC_MESSAGES/collective.captchacontactinfo.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.266736 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.278971 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      452 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/profiles/default/actions.xml
--rw-r--r--   0 cekk       (501) staff       (20)      196 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)       10 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/profiles/default/captchacontactinfo-various.txt
--rw-r--r--   0 cekk       (501) staff       (20)      537 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/profiles/default/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)       71 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/profiles/default/metadata.xml
--rw-r--r--   0 cekk       (501) staff       (20)     1042 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/profiles/default/registry.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.279579 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      122 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      496 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/profiles/uninstall/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      774 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/setuphandlers.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.270843 collective.captchacontactinfo-3.0.0/collective.captchacontactinfo.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     4959 2022-11-03 15:37:02.000000 collective.captchacontactinfo-3.0.0/collective.captchacontactinfo.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     2436 2022-11-03 15:37:02.000000 collective.captchacontactinfo-3.0.0/collective.captchacontactinfo.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2022-11-03 15:37:02.000000 collective.captchacontactinfo-3.0.0/collective.captchacontactinfo.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)       89 2022-11-03 15:37:02.000000 collective.captchacontactinfo-3.0.0/collective.captchacontactinfo.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2022-11-03 15:37:02.000000 collective.captchacontactinfo-3.0.0/collective.captchacontactinfo.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2022-11-03 15:37:02.000000 collective.captchacontactinfo-3.0.0/collective.captchacontactinfo.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)       31 2022-11-03 15:37:02.000000 collective.captchacontactinfo-3.0.0/collective.captchacontactinfo.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2022-11-03 15:37:02.000000 collective.captchacontactinfo-3.0.0/collective.captchacontactinfo.egg-info/top_level.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-03 15:37:02.280373 collective.captchacontactinfo-3.0.0/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     1672 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/docs/HISTORY.rst
--rw-r--r--   0 cekk       (501) staff       (20)    17987 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/docs/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      762 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/docs/LICENSE.txt
--rw-r--r--   0 cekk       (501) staff       (20)       38 2022-11-03 15:37:02.281108 collective.captchacontactinfo-3.0.0/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     1417 2022-11-03 15:37:01.000000 collective.captchacontactinfo-3.0.0/setup.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/
+-rw-r--r--   0 daniele    (501) staff       (20)     5119 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/PKG-INFO
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/
+-rw-r--r--   0 daniele    (501) staff       (20)      269 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/interfaces.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/controlpanel/
+-rw-r--r--   0 daniele    (501) staff       (20)      704 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/controlpanel/interfaces.py
+-rw-r--r--   0 daniele    (501) staff       (20)      541 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/controlpanel/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)       23 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/controlpanel/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      618 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/controlpanel/view.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1246 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/configure.zcml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/locales/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/locales/it/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/locales/it/LC_MESSAGES/
+-rw-r--r--   0 daniele    (501) staff       (20)     2708 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/locales/it/LC_MESSAGES/collective.captchacontactinfo.po
+-rw-r--r--   0 daniele    (501) staff       (20)     2168 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/locales/collective.captchacontactinfo.pot
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/locales/de/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/locales/de/LC_MESSAGES/
+-rw-r--r--   0 daniele    (501) staff       (20)     2260 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/locales/de/LC_MESSAGES/collective.captchacontactinfo.po
+-rwxr-xr-x   0 daniele    (501) staff       (20)      413 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/i18n.sh
+-rw-r--r--   0 daniele    (501) staff       (20)      155 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      774 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/setuphandlers.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/
+-rw-r--r--   0 daniele    (501) staff       (20)      938 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)       23 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/__init__.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/static/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/static/css/
+-rw-r--r--   0 daniele    (501) staff       (20)      191 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/static/css/captchacontactinfo.css
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/static/scripts/
+-rw-r--r--   0 daniele    (501) staff       (20)     1132 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/static/scripts/policy_ajax.js
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/templates/
+-rw-r--r--   0 daniele    (501) staff       (20)     1858 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/templates/contact-info.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     1382 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/templates/contact-info-email.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     1457 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/contact_form_view.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/ajax/
+-rw-r--r--   0 daniele    (501) staff       (20)      457 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/ajax/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)       23 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/ajax/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      678 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/ajax/utils.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/profiles/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/profiles/default/
+-rw-r--r--   0 daniele    (501) staff       (20)      452 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/profiles/default/actions.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      537 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/profiles/default/controlpanel.xml
+-rw-r--r--   0 daniele    (501) staff       (20)       10 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/profiles/default/captchacontactinfo-various.txt
+-rw-r--r--   0 daniele    (501) staff       (20)     1042 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/profiles/default/registry.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      196 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/profiles/default/browserlayer.xml
+-rw-r--r--   0 daniele    (501) staff       (20)       71 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/profiles/default/metadata.xml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/profiles/uninstall/
+-rw-r--r--   0 daniele    (501) staff       (20)      496 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/profiles/uninstall/registry.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      122 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      244 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective/__init__.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective.captchacontactinfo.egg-info/
+-rw-r--r--   0 daniele    (501) staff       (20)     5119 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective.captchacontactinfo.egg-info/PKG-INFO
+-rw-r--r--   0 daniele    (501) staff       (20)        1 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective.captchacontactinfo.egg-info/not-zip-safe
+-rw-r--r--   0 daniele    (501) staff       (20)       11 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective.captchacontactinfo.egg-info/namespace_packages.txt
+-rw-r--r--   0 daniele    (501) staff       (20)     2334 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective.captchacontactinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 daniele    (501) staff       (20)       89 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective.captchacontactinfo.egg-info/entry_points.txt
+-rw-r--r--   0 daniele    (501) staff       (20)       31 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective.captchacontactinfo.egg-info/requires.txt
+-rw-r--r--   0 daniele    (501) staff       (20)       11 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective.captchacontactinfo.egg-info/top_level.txt
+-rw-r--r--   0 daniele    (501) staff       (20)        1 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/collective.captchacontactinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 daniele    (501) staff       (20)      110 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/MANIFEST.in
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/docs/
+-rw-r--r--   0 daniele    (501) staff       (20)    17987 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/docs/LICENSE.GPL
+-rw-r--r--   0 daniele    (501) staff       (20)     1776 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/docs/HISTORY.rst
+-rw-r--r--   0 daniele    (501) staff       (20)      762 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/docs/LICENSE.txt
+-rw-r--r--   0 daniele    (501) staff       (20)     1417 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/setup.py
+-rw-r--r--   0 daniele    (501) staff       (20)       38 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/setup.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     1298 2023-07-28 12:37:32.000000 collective.captchacontactinfo-3.0.1/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `collective.captchacontactinfo-3.0.0/PKG-INFO` & `collective.captchacontactinfo-3.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: collective.captchacontactinfo
-Version: 3.0.0
+Version: 3.0.1
 Summary: A simple customization for Plone contact-info that add a validation for anonymous users
 Home-page: http://plone.org/products/collective.captchacontactinfo
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL
 Description: Introduction
         ============
@@ -54,14 +54,21 @@
         .. image:: http://www.redturtle.it/redturtle_banner.png
            :alt: RedTurtle Technology Site
            :target: http://www.redturtle.it/
         
         Changelog
         =========
         
+        3.0.1 (2023-07-28)
+        ------------------
+        
+        - Added original URL to contact-info form (#27527)
+          [daniele]
+        
+        
         3.0.0 (2022-11-03)
         ------------------
         
         - Drop recaptcha dependency: use collective.honeypot.
           [cekk]
```

### Comparing `collective.captchacontactinfo-3.0.0/README.rst` & `collective.captchacontactinfo-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/ajax/utils.py` & `collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/ajax/utils.py`

 * *Files identical despite different names*

### Comparing `collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/static/scripts/policy_ajax.js` & `collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/static/scripts/policy_ajax.js`

 * *Files identical despite different names*

### Comparing `collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/browser/templates/contact-info.pt` & `collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/browser/templates/contact-info.pt`

 * *Files identical despite different names*

### Comparing `collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/configure.zcml` & `collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/controlpanel/configure.zcml` & `collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/controlpanel/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/controlpanel/interfaces.py` & `collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/controlpanel/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/controlpanel/view.py` & `collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/controlpanel/view.py`

 * *Files identical despite different names*

### Comparing `collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/locales/collective.captchacontactinfo.pot` & `collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/locales/collective.captchacontactinfo.pot`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2021-02-02 09:30+0000\n"
+"POT-Creation-Date: 2023-07-26 13:22+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -17,26 +17,14 @@
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: collective.captchacontactinfo\n"
 
 #: ./profiles/default/controlpanel.xml
 msgid "Captcha Contact Info"
 msgstr ""
 
-#: ./configure.zcml:21
-msgid "Captcha contact-info"
-msgstr ""
-
-#: ./configure.zcml:21
-msgid "Installs the collective.captchacontactinfo package"
-msgstr ""
-
-#: ./configure.zcml:29
-msgid "Uninstalls the collective.captchacontactinfo package"
-msgstr ""
-
 #. Default: "Policy page"
 #: ./controlpanel/interfaces.py:11
 msgid "contactinfo-config-policy"
 msgstr ""
 
 #. Default: "Insert the path for the Page used for Policy text. For example: folder-a/policy-page"
 #: ./controlpanel/interfaces.py:13
@@ -55,25 +43,26 @@
 
 #. Default: "Contact form"
 #: ./browser/templates/contact-info.pt:22
 msgid "heading_contact_form"
 msgstr ""
 
 #. Default: "Please enter your e-mail address if you want to receive an answer"
-#: ./browser/contact_form_view.py:55
+#: ./browser/contact_form_view.py:31
 msgid "help_sender_from_address_customized"
 msgstr ""
 
-#. Default: "Send"
-#: ./browser/contact_form_view.py:63
-msgid "label_send"
+#. Default: "The page from where the request has been originally submitted was ${starting_url}"
+#: ./browser/templates/contact-info-email.pt:22
+msgid "original_url_to_contact-info"
 msgstr ""
 
-#. Default: "The code you entered was wrong, please enter the new one."
-#: ./browser/contact_form_view.py:84
-msgid "not_compile_captcha"
+#. Default: "You are receiving this mail because ${fullname} ${from_address} is sending feedback about the site you administer at ${url}."
+#: ./browser/templates/contact-info-email.pt:19
+msgid "site_feedback_mailtemplate_body"
 msgstr ""
 
 #. Default: "This site doesn't have a valid email setup, so you cannot use any contact forms."
 #: ./browser/templates/contact-info.pt:28
 msgid "text_no_email_setup"
 msgstr ""
+
```

### Comparing `collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/locales/de/LC_MESSAGES/collective.captchacontactinfo.po` & `collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/locales/de/LC_MESSAGES/collective.captchacontactinfo.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2021-02-02 09:30+0000\n"
+"POT-Creation-Date: 2023-07-26 13:22+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: Eggert Ehmke <eggert@eehmke.de>\n"
 "Language-Team: LANGUAGE <DE@de.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -17,26 +17,14 @@
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: collective.captchacontactinfo\n"
 
 #: ./profiles/default/controlpanel.xml
 msgid "Captcha Contact Info"
 msgstr ""
 
-#: ./configure.zcml:21
-msgid "Captcha contact-info"
-msgstr ""
-
-#: ./configure.zcml:21
-msgid "Installs the collective.captchacontactinfo package"
-msgstr ""
-
-#: ./configure.zcml:29
-msgid "Uninstalls the collective.captchacontactinfo package"
-msgstr ""
-
 #. Default: "Policy page"
 #: ./controlpanel/interfaces.py:11
 msgid "contactinfo-config-policy"
 msgstr "Erklärung"
 
 #. Default: "Insert the path for the Page used for Policy text. For example: folder-a/policy-page"
 #: ./controlpanel/interfaces.py:13
@@ -55,25 +43,26 @@
 
 #. Default: "Contact form"
 #: ./browser/templates/contact-info.pt:22
 msgid "heading_contact_form"
 msgstr ""
 
 #. Default: "Please enter your e-mail address if you want to receive an answer"
-#: ./browser/contact_form_view.py:55
+#: ./browser/contact_form_view.py:31
 msgid "help_sender_from_address_customized"
 msgstr ""
 
-#. Default: "Send"
-#: ./browser/contact_form_view.py:63
-msgid "label_send"
+#. Default: "The page from where the request has been originally submitted was ${starting_url}"
+#: ./browser/templates/contact-info-email.pt:22
+msgid "original_url_to_contact-info"
 msgstr ""
 
-#. Default: "The code you entered was wrong, please enter the new one."
-#: ./browser/contact_form_view.py:84
-msgid "not_compile_captcha"
+#. Default: "You are receiving this mail because ${fullname} ${from_address} is sending feedback about the site you administer at ${url}."
+#: ./browser/templates/contact-info-email.pt:19
+msgid "site_feedback_mailtemplate_body"
 msgstr ""
 
 #. Default: "This site doesn't have a valid email setup, so you cannot use any contact forms."
 #: ./browser/templates/contact-info.pt:28
 msgid "text_no_email_setup"
 msgstr ""
+
```

### Comparing `collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/locales/it/LC_MESSAGES/collective.captchacontactinfo.po` & `collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/locales/it/LC_MESSAGES/collective.captchacontactinfo.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2021-02-02 09:30+0000\n"
+"POT-Creation-Date: 2023-07-26 13:22+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -17,26 +17,14 @@
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: collective.captchacontactinfo\n"
 
 #: ./profiles/default/controlpanel.xml
 msgid "Captcha Contact Info"
 msgstr ""
 
-#: ./configure.zcml:21
-msgid "Captcha contact-info"
-msgstr ""
-
-#: ./configure.zcml:21
-msgid "Installs the collective.captchacontactinfo package"
-msgstr ""
-
-#: ./configure.zcml:29
-msgid "Uninstalls the collective.captchacontactinfo package"
-msgstr ""
-
 #. Default: "Policy page"
 #: ./controlpanel/interfaces.py:11
 msgid "contactinfo-config-policy"
 msgstr "Pagina per l'informativa sulla privacy"
 
 #. Default: "Insert the path for the Page used for Policy text. For example: folder-a/policy-page"
 #: ./controlpanel/interfaces.py:13
@@ -55,25 +43,26 @@
 
 #. Default: "Contact form"
 #: ./browser/templates/contact-info.pt:22
 msgid "heading_contact_form"
 msgstr "Contatti"
 
 #. Default: "Please enter your e-mail address if you want to receive an answer"
-#: ./browser/contact_form_view.py:55
+#: ./browser/contact_form_view.py:31
 msgid "help_sender_from_address_customized"
 msgstr "Inserisci la tua e-mail se vuoi ricevere una risposta"
 
-#. Default: "Send"
-#: ./browser/contact_form_view.py:63
-msgid "label_send"
-msgstr "Invia"
-
-#. Default: "The code you entered was wrong, please enter the new one."
-#: ./browser/contact_form_view.py:84
-msgid "not_compile_captcha"
-msgstr "La verifica del captcha non è andata a buon fine."
+#. Default: "The page from where the request has been originally submitted was ${starting_url}"
+#: ./browser/templates/contact-info-email.pt:22
+msgid "original_url_to_contact-info"
+msgstr "La pagina da cui è partita la richiesta è ${starting_url}"
+
+#. Default: "You are receiving this mail because ${fullname} ${from_address} is sending feedback about the site you administer at ${url}."
+#: ./browser/templates/contact-info-email.pt:19
+msgid "site_feedback_mailtemplate_body"
+msgstr "Ricevi questo messaggio perché ${fullname} ${from_address} ha inserito una nota relativa al sito ${url} da te amministrato."
 
 #. Default: "This site doesn't have a valid email setup, so you cannot use any contact forms."
 #: ./browser/templates/contact-info.pt:28
 msgid "text_no_email_setup"
 msgstr "Prima di procedere occorre impostare la configurazione di Posta del sito"
+
```

### Comparing `collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/profiles/default/controlpanel.xml` & `collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/profiles/default/registry.xml` & `collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.captchacontactinfo-3.0.0/collective/captchacontactinfo/setuphandlers.py` & `collective.captchacontactinfo-3.0.1/collective/captchacontactinfo/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.captchacontactinfo-3.0.0/collective.captchacontactinfo.egg-info/PKG-INFO` & `collective.captchacontactinfo-3.0.1/collective.captchacontactinfo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: collective.captchacontactinfo
-Version: 3.0.0
+Version: 3.0.1
 Summary: A simple customization for Plone contact-info that add a validation for anonymous users
 Home-page: http://plone.org/products/collective.captchacontactinfo
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL
 Description: Introduction
         ============
@@ -54,14 +54,21 @@
         .. image:: http://www.redturtle.it/redturtle_banner.png
            :alt: RedTurtle Technology Site
            :target: http://www.redturtle.it/
         
         Changelog
         =========
         
+        3.0.1 (2023-07-28)
+        ------------------
+        
+        - Added original URL to contact-info form (#27527)
+          [daniele]
+        
+        
         3.0.0 (2022-11-03)
         ------------------
         
         - Drop recaptcha dependency: use collective.honeypot.
           [cekk]
```

### Comparing `collective.captchacontactinfo-3.0.0/collective.captchacontactinfo.egg-info/SOURCES.txt` & `collective.captchacontactinfo-3.0.1/collective.captchacontactinfo.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,23 +19,22 @@
 collective/captchacontactinfo/browser/configure.zcml
 collective/captchacontactinfo/browser/contact_form_view.py
 collective/captchacontactinfo/browser/ajax/__init__.py
 collective/captchacontactinfo/browser/ajax/configure.zcml
 collective/captchacontactinfo/browser/ajax/utils.py
 collective/captchacontactinfo/browser/static/css/captchacontactinfo.css
 collective/captchacontactinfo/browser/static/scripts/policy_ajax.js
+collective/captchacontactinfo/browser/templates/contact-info-email.pt
 collective/captchacontactinfo/browser/templates/contact-info.pt
 collective/captchacontactinfo/controlpanel/__init__.py
 collective/captchacontactinfo/controlpanel/configure.zcml
 collective/captchacontactinfo/controlpanel/interfaces.py
 collective/captchacontactinfo/controlpanel/view.py
 collective/captchacontactinfo/locales/collective.captchacontactinfo.pot
-collective/captchacontactinfo/locales/de/LC_MESSAGES/collective.captchacontactinfo.mo
 collective/captchacontactinfo/locales/de/LC_MESSAGES/collective.captchacontactinfo.po
-collective/captchacontactinfo/locales/it/LC_MESSAGES/collective.captchacontactinfo.mo
 collective/captchacontactinfo/locales/it/LC_MESSAGES/collective.captchacontactinfo.po
 collective/captchacontactinfo/profiles/default/actions.xml
 collective/captchacontactinfo/profiles/default/browserlayer.xml
 collective/captchacontactinfo/profiles/default/captchacontactinfo-various.txt
 collective/captchacontactinfo/profiles/default/controlpanel.xml
 collective/captchacontactinfo/profiles/default/metadata.xml
 collective/captchacontactinfo/profiles/default/registry.xml
```

### Comparing `collective.captchacontactinfo-3.0.0/docs/HISTORY.rst` & `collective.captchacontactinfo-3.0.1/docs/HISTORY.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+3.0.1 (2023-07-28)
+------------------
+
+- Added original URL to contact-info form (#27527)
+  [daniele]
+
+
 3.0.0 (2022-11-03)
 ------------------
 
 - Drop recaptcha dependency: use collective.honeypot.
   [cekk]
```

### Comparing `collective.captchacontactinfo-3.0.0/docs/LICENSE.GPL` & `collective.captchacontactinfo-3.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.captchacontactinfo-3.0.0/docs/LICENSE.txt` & `collective.captchacontactinfo-3.0.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.captchacontactinfo-3.0.0/setup.py` & `collective.captchacontactinfo-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-version = "3.0.0"
+version = "3.0.1"
 
 setup(
     name="collective.captchacontactinfo",
     version=version,
     description="A simple customization for Plone contact-info that add a validation for anonymous users",
     long_description=open("README.rst").read()
     + "\n"
```

