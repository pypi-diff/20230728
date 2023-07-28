# Comparing `tmp/honeybee-doe2-0.8.1.tar.gz` & `tmp/honeybee-doe2-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-doe2-0.8.1.tar", last modified: Tue Jun 27 17:31:04 2023, max compression
+gzip compressed data, was "dist/honeybee-doe2-0.8.2.tar", last modified: Fri Jul 28 02:47:16 2023, max compression
```

## Comparing `honeybee-doe2-0.8.1.tar` & `honeybee-doe2-0.8.2.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/honeybee_doe2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/_extend_honeybee_doe2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/honeybee_doe2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/cli/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/honeybee_doe2/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/geometry/polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/adiabaticfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/adiabaticroof.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/aperture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/constructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/exposedfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/groundcontact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/hvac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/inputils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/inputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/inputils/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/inputils/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/inputils/glass_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/inputils/run_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/inputils/sitebldg.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/inputils/title.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/interiorfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/roof.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/shades.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/story.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/properties/wall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/honeybee_doe2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/utils/doe_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/honeybee_doe2/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/honeybee_doe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/honeybee_doe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/honeybee_doe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/honeybee_doe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/honeybee_doe2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/honeybee_doe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/honeybee_doe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 17:31:04.000000 honeybee-doe2-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-27 17:30:03.000000 honeybee-doe2-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/honeybee_doe2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/_extend_honeybee_doe2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/honeybee_doe2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/cli/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/honeybee_doe2/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/geometry/polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/adiabaticfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/adiabaticroof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/constructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/exposedfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/groundcontact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/hvac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/inputils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/inputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/inputils/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/inputils/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/inputils/glass_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/inputils/run_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/inputils/sitebldg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/inputils/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/interiorfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/roof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/shades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/properties/wall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/honeybee_doe2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/utils/doe_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/honeybee_doe2/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/honeybee_doe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/honeybee_doe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/honeybee_doe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/honeybee_doe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/honeybee_doe2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/honeybee_doe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/honeybee_doe2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 02:47:16.000000 honeybee-doe2-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-28 02:46:14.000000 honeybee-doe2-0.8.2/setup.py
```

### Comparing `honeybee-doe2-0.8.1/LICENSE` & `honeybee-doe2-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/PKG-INFO` & `honeybee-doe2-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.8.1
+Version: 0.8.2
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.8.1/README.md` & `honeybee-doe2-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/_extend_honeybee_doe2.py` & `honeybee-doe2-0.8.2/honeybee_doe2/_extend_honeybee_doe2.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/cli/translate.py` & `honeybee-doe2-0.8.2/honeybee_doe2/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/geometry/polygon.py` & `honeybee-doe2-0.8.2/honeybee_doe2/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/adiabaticfloor.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/adiabaticfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/adiabaticroof.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/adiabaticroof.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/constructions.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/constructions.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/exposedfloor.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/exposedfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/face.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/groundcontact.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/groundcontact.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/hvac.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/hvac.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/inputils/blocks.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/inputils/blocks.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/inputils/compliance.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/inputils/compliance.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/inputils/glass_types.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/inputils/glass_types.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/inputils/run_period.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/inputils/run_period.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/inputils/sitebldg.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/inputils/sitebldg.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/interiorfloor.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/interiorfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/materials.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/materials.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/model.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,27 +55,23 @@
         NOTE: The header is currently read-only
         """
         return '\n'.join([fb.top_level, fb.abort_diag])
 
     @property
     def stories(self):
         # * do tuple, (geom, 'space room whatever') for each 'inpblock' per story
-        return self._make_doe_stories(self.host)
-
-    @staticmethod
-    def _make_doe_stories(obj):
         stories = []
-        if not obj.rooms:
+        model = self.host
+        tol = model.tolerance
+        if not model.rooms:
             return stories
-
-        grouped = Room.group_by_floor_height(obj.rooms, 0.1)
+        grouped = Room.group_by_floor_height(model.rooms, 0.1)
         for i, story in enumerate(grouped[0]):
-            stories.append(Doe2Story(story, i))
-        # nl = ''
-        # return str(nl.join(str(s) for s in stories))
+            stories.append(Doe2Story(story, i, tolerance=tol))
+
         return stories
 
     @property
     def header(self):
         return '\n'.join([fb.top_level, fb.abort_diag])
 
     @property
```

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/roof.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/roof.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/room.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/room.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,58 @@
 # -*- coding: utf-8 -*-
 from honeybee_energy.boundarycondition import Adiabatic
 
 from honeybee.boundarycondition import Ground, Outdoors, Surface
 from honeybee.facetype import Wall, Floor, RoofCeiling
 from honeybee.face import Face
-from honeybee.room import Room, Point3D
+from honeybee.room import Room
 from typing import List
+from uuid import uuid4
 
 from ..utils.doe_formatters import short_name
-from ..utils.geometry import get_room_rep_poly
 from .wall import DoeWall
 from .roof import DoeRoof
 from .groundcontact import GroundFloor
 from .exposedfloor import ExposedFloor
 from .interiorfloor import InteriorFloor
 from .adiabaticfloor import AdiabaticFloor
 from .adiabaticroof import AdiabaticRoof
 
 
 class RoomDoe2Properties(object):
     """Properties for a DOE2 Space."""
 
     def __init__(self, _host: Room):
         self._host = _host
+        self._boundary = None
 
     @property
     def host(self) -> Room:
         return self._host
 
-    @property
-    def boundary(self) -> Face:
-        return self._get_boundary_geometry(self._host)
-
-    @property
-    def origin(self) -> Point3D:
-        """Origin point of the room."""
-        return self.boundary.geometry.lower_left_corner
+    def boundary(self, tolerance) -> Face:
+        if self._boundary:
+            return self._boundary
+        tol = tolerance
+        _boundary = self._host.horizontal_boundary(match_walls=False, tolerance=tol)
+        _boundary = _boundary.remove_colinear_vertices(tolerance=tol)
+        boundary_face = Face(identifier=str(uuid4()), geometry=_boundary)
+        boundary_face.display_name = self._host.display_name
+        self._boundary = boundary_face
+        return boundary_face
 
     def duplicate(self, new_host=None):
 
         _host = new_host or self._host
         new_properties_obj = RoomDoe2Properties(_host)
         return new_properties_obj
 
-    @property
-    def poly(self):
+    def poly(self, tolerance):
         # * return self's floor's face's poly
-        return self.boundary.properties.doe2.poly
-
-    @staticmethod
-    def _get_boundary_geometry(room: Room):
-        return get_room_rep_poly(room)
+        return self.boundary(tolerance).properties.doe2.poly
 
     @property
     def walls(self) -> List[DoeWall]:
         # * Needs to return list of DoeWall objects
 
         walls = [
             DoeWall(face) for face in self.host.faces
@@ -133,41 +131,47 @@
         pass
     # TODO add activity disc // loads support etc
 
     def space(self, floor_origin):
         # chances that a space is defined by a different azimuth than 0 is very low
         azimuth = 0
         # this value should be set in relation to the Floor object
-        origin_pt = self.origin - floor_origin
+        if not self._boundary:
+            raise ValueError(
+                'You must call the `poly` method to create the boundary before calling '
+                'this method.'
+            )
+        origin = self._boundary.geometry.lower_left_corner
+        origin_pt = origin - floor_origin
         obj_lines = []
         obj_lines.append('"{}" = SPACE\n'.format(short_name(self.host.display_name)))
         obj_lines.append('   SHAPE           = POLYGON\n')
         obj_lines.append('   POLYGON         = "{} Plg"\n'.format(
-            self.boundary.display_name))
+            self.host.display_name))
         obj_lines.append('   AZIMUTH         = {}\n'.format(azimuth))
         obj_lines.append('   X               = {}\n'.format(origin_pt.x))
         obj_lines.append('   Y               = {}\n'.format(origin_pt.y))
         obj_lines.append('   Z               = {}\n'.format(origin_pt.z))
         obj_lines.append('   VOLUME          = {}\n'.format(self.host.volume))
         obj_lines.append('  ..\n')
         # obj_lines.append('   C-ACTIVITY-DESC = *{}*\n   ..\n'.format(str(obj.properties.energy.program_type)))
         spaces = ''.join(obj_lines)
-        walls = '\n'.join([w.to_inp(self.origin) for w in self.walls])
-        roofs = '\n'.join([r.to_inp(self.origin) for r in self.roofs])
+        walls = '\n'.join([w.to_inp(origin) for w in self.walls])
+        roofs = '\n'.join([r.to_inp(origin) for r in self.roofs])
         ground_floors = '\n'.join(
-            [g.to_inp(self.origin) for g in self.ground_contact_surfaces]
+            [g.to_inp(origin) for g in self.ground_contact_surfaces]
         )
         exposed_floors = '\n'.join(
-            [ef.to_inp(self.origin) for ef in self.exposed_floor_surfaces]
+            [ef.to_inp(origin) for ef in self.exposed_floor_surfaces]
         )
         interior_floors = '\n'.join(
-            [inf.to_inp(self.origin) for inf in self.interior_floor_surfaces]
+            [inf.to_inp(origin) for inf in self.interior_floor_surfaces]
         )
         adiabatic_floors = '\n'.join(
-            [af.to_inp(self.origin) for af in self.adiabatic_floor_surfaces]
+            [af.to_inp(origin) for af in self.adiabatic_floor_surfaces]
         )
         adiabatic_roofs = '\n'.join(
-            [ar.to_inp(self.origin) for ar in self.adiabatic_roofs]
+            [ar.to_inp(origin) for ar in self.adiabatic_roofs]
         )
         return '\n'.join(
             [spaces, walls, roofs, adiabatic_roofs, ground_floors, exposed_floors,
              interior_floors, adiabatic_floors])
```

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/shades.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/shades.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/story.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/story.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 # -*- coding: utf-8 -*-
 # -*- Python Version: 2.7 -*
 """ Doe2 'Story' Object."""
 from typing import List
 from honeybee.room import Room
 from honeybee.face import Face
-from ..utils.geometry import get_floor_boundary
 
 
 class Doe2Story:
     """This class represents a DOE2 FLOOR object."""
 
-    def __init__(self, rooms: List[Room], _story_no: int):
+    def __init__(self, rooms: List[Room], story_number: int, tolerance: float):
         self.rooms = rooms
-        self.story_no = _story_no
+        self.story_no = story_number
+        self.tolerance = tolerance
         self.story_poly, self.boundary_geometry = self._story_poly
 
-    # TODO Model use doe2story object to get geometry of each story and stories rooms/zones
     @property
     def _story_poly(self):
-        vertices = get_floor_boundary(self.rooms)
+        tol = self.tolerance
+        boundaries = Room.grouped_horizontal_boundary(self.rooms, tolerance=tol)
+        if len(boundaries) != 1:
+            raise ValueError(
+                'Failed to create the boundary using grouped horizontal boundary.'
+                f'for Level {self.story_no} using a tolerance value of {tol}. Check '
+                'The input model and ensure there are any gaps between the rooms.'
+            )
+
+        vertices = boundaries[0].boundary  # use boundary to ignore holes if any
         story_geom = Face.from_vertices(
             identifier="Level_{}".format(self.story_no),
             vertices=vertices)
         story_geom.display_name = "Level_{}".format(self.story_no)
 
         story_rm_geom = []
 
         story_rm_geom.append(story_geom.properties.doe2.poly)
 
         for room in self.rooms:
-            story_rm_geom.append(room.properties.doe2.poly)
+            story_rm_geom.append(room.properties.doe2.poly(tol))
             for face in room.faces:
                 story_rm_geom.append(face.properties.doe2.poly)
-
         story_rm_geom = '\n'.join(story_rm_geom)
 
         return '\n'.join([story_rm_geom]), story_geom
 
     @property
     def space_height(self):
         # TODO un-hardcode this
@@ -55,19 +62,15 @@
 
         ceil_h = ceil_heights / ceil_areas
         ceil_l = rooms[0].average_floor_height
         return ceil_h - ceil_l
 
     @property
     def display_name(self):
-        return self._get_display_name(self.story_no)
-
-    @staticmethod
-    def _get_display_name(story_no):
-        return "Level_{}".format(story_no)
+        return "Level_{}".format(self.story_no)
 
     def to_inp(self):
         origin_pt = self.boundary_geometry.geometry.lower_left_corner
         azimuth = self.boundary_geometry.azimuth
         room_objs = [f.properties.doe2.space(origin_pt) for f in self.rooms]
 
         inp_obj = '\n"{self.display_name}"= FLOOR'.format(self=self) + \
```

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/properties/wall.py` & `honeybee-doe2-0.8.2/honeybee_doe2/properties/wall.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/utils/doe_formatters.py` & `honeybee-doe2-0.8.2/honeybee_doe2/utils/doe_formatters.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2/writer.py` & `honeybee-doe2-0.8.2/honeybee_doe2/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,20 @@
 
 def model_to_inp(hb_model):
     # type: (Model) -> str
     rp = RunPeriod()
     comp_data = ComplianceData()
     sb_data = sbd()
 
-    hb_model.convert_to_units(units='Feet')
+    hb_model = hb_model.duplicate()
+
+    if hb_model.units != 'Feet':
+        hb_model.convert_to_units(units='Feet')
+    hb_model.remove_degenerate_geometry()
+    hb_model.rectangularize_apertures(subdivision_distance=0.5, max_separation=0)
 
     room_names = {}
     face_names = {}
     for room in hb_model.rooms:
         room.display_name = room.display_name.replace('..', '_')
         if room.display_name in room_names:
             original_name = room.display_name
@@ -59,18 +64,17 @@
         shade.display_name = f'shade_{i}'
     for face in hb_model.faces:
         if isinstance(face.boundary_condition, Surface):
             adj_room_identifier = face.boundary_condition.boundary_condition_objects[1]
             face.user_data = {'adjacent_room': room_mapper[adj_room_identifier]}
 
     for i, room in enumerate(hb_model.rooms):
-        room_name = room.display_name
-        for ii, face in enumerate(room.faces):
+        for face in room.faces:
             try:
-                face_dir = face.horizontal_orientation()
+                _ = face.horizontal_orientation()
             except ZeroDivisionError:
                 face.display_name = short_name(
                     clean_and_id_string(face.display_name)).replace(
                     '..', '_')
             else:
                 face.display_name = short_name(
                     clean_and_id_string(face.display_name)).replace(
```

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2.egg-info/PKG-INFO` & `honeybee-doe2-0.8.2/honeybee_doe2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.8.1
+Version: 0.8.2
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.8.1/honeybee_doe2.egg-info/SOURCES.txt` & `honeybee-doe2-0.8.2/honeybee_doe2.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -45,9 +45,8 @@
 honeybee_doe2/properties/inputils/compliance.py
 honeybee_doe2/properties/inputils/glass_types.py
 honeybee_doe2/properties/inputils/run_period.py
 honeybee_doe2/properties/inputils/sitebldg.py
 honeybee_doe2/properties/inputils/title.py
 honeybee_doe2/utils/__init__.py
 honeybee_doe2/utils/doe_formatters.py
-honeybee_doe2/utils/geometry.py
 honeybee_doe2/utils/vector.py
```

### Comparing `honeybee-doe2-0.8.1/setup.py` & `honeybee-doe2-0.8.2/setup.py`

 * *Files identical despite different names*

