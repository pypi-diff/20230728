# Comparing `tmp/kiwi_keg-2.0.2.tar.gz` & `tmp/kiwi_keg-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kiwi_keg-2.0.2.tar", last modified: Fri Nov 18 21:03:58 2022, max compression
+gzip compressed data, was "kiwi_keg-2.1.1.tar", last modified: Fri Jul 28 15:34:10 2023, max compression
```

## Comparing `kiwi_keg-2.0.2.tar` & `kiwi_keg-2.1.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/.virtualenv.dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/kiwi_keg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/kiwi_keg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/kiwi_keg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/kiwi_keg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/kiwi_keg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/kiwi_keg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     2753 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/kiwi_keg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/kiwi_keg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/kiwi_keg/
--rw-r--r--   0 runner    (1001) docker     (121)     8725 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/source_info_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7539 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/script_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7084 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/image_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     4858 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/kiwi_description.py
--rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/logger_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)    17567 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7195 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/keg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/kiwi_keg/obs_service/
--rw-r--r--   0 runner    (1001) docker     (121)    11035 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/obs_service/compose_kiwi_description.py
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/obs_service/compose_kiwi_description.service
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/obs_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/kiwi_keg/changelog_generator/
--rw-r--r--   0 runner    (1001) docker     (121)     5973 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/changelog_generator/generate_recipes_changelog.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/changelog_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2541 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/annotated_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     8302 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/image_definition.py
--rw-r--r--   0 runner    (1001) docker     (121)     7270 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/kiwi_keg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/DC-keg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/doc/source/
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3443 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/doc/source/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     3377 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/source/commands/keg.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/source/commands/generate_recipes_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4828 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/source/data_modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/source/commands.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/source/obs_source_service.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3045 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/source/changelog_generator.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4287 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/source/recipes_basics.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/doc/source/intersphinx_mapping/
--rw-r--r--   0 runner    (1001) docker     (121)   129526 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/source/intersphinx_mapping/objects.inv
--rw-r--r--   0 runner    (1001) docker     (121)     5591 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/source/overview.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13577 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/source/image_definition.rst
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/doc/xml/
--rw-r--r--   0 runner    (1001) docker     (121)    29310 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/xml/book.xml
--rw-r--r--   0 runner    (1001) docker     (121)     6682 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/.virtualenv.requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3189 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/tox.ini
--rwxr-xr-x   0 runner    (1001) docker     (121)     1875 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2174 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2753 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 21:03:58.000000 kiwi_keg-2.0.2/package/
--rw-r--r--   0 runner    (1001) docker     (121)     4486 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/package/python-kiwi-keg.spec
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/package/python-kiwi-keg.changes
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-18 21:03:17.000000 kiwi_keg-2.0.2/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:10.960710 kiwi_keg-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/.coveragerc_py36
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/.virtualenv.dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/.virtualenv.requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-28 15:34:10.960710 kiwi_keg-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:10.952710 kiwi_keg-2.1.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/DC-keg
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:10.956710 kiwi_keg-2.1.1/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/source/changelog_generator.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:10.956710 kiwi_keg-2.1.1/doc/source/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/source/commands/generate_recipes_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/source/commands/keg.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/source/commands.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/source/data_modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/source/image_definition.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:10.956710 kiwi_keg-2.1.1/doc/source/intersphinx_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)   129526 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/source/intersphinx_mapping/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/source/obs_source_service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/source/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/source/recipes_basics.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:10.956710 kiwi_keg-2.1.1/doc/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)    64433 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/doc/xml/book.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:10.956710 kiwi_keg-2.1.1/kiwi_keg/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/annotated_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/image_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/image_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/keg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/kiwi_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/logger_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/script_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/source_info_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:10.960710 kiwi_keg-2.1.1/kiwi_keg/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/tools/compose_kiwi_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/tools/generate_recipes_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/kiwi_keg/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:10.960710 kiwi_keg-2.1.1/kiwi_keg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-28 15:34:10.000000 kiwi_keg-2.1.1/kiwi_keg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-28 15:34:10.000000 kiwi_keg-2.1.1/kiwi_keg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:34:10.000000 kiwi_keg-2.1.1/kiwi_keg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-28 15:34:10.000000 kiwi_keg-2.1.1/kiwi_keg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:34:10.000000 kiwi_keg-2.1.1/kiwi_keg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 15:34:10.000000 kiwi_keg-2.1.1/kiwi_keg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 15:34:10.000000 kiwi_keg-2.1.1/kiwi_keg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:10.960710 kiwi_keg-2.1.1/obs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/obs/compose_kiwi_description.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:10.960710 kiwi_keg-2.1.1/package/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/package/python-kiwi-keg.changes
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/package/python-kiwi-keg.spec
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-28 15:34:10.960710 kiwi_keg-2.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1843 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-28 15:34:00.000000 kiwi_keg-2.1.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kiwi_keg-2.0.2/kiwi_keg.egg-info/SOURCES.txt` & `kiwi_keg-2.1.1/kiwi_keg.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .bumpversion.cfg
+.coveragerc_py36
 .virtualenv.dev-requirements.txt
 .virtualenv.requirements.txt
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 setup.cfg
@@ -42,14 +43,13 @@
 kiwi_keg.egg-info/PKG-INFO
 kiwi_keg.egg-info/SOURCES.txt
 kiwi_keg.egg-info/dependency_links.txt
 kiwi_keg.egg-info/entry_points.txt
 kiwi_keg.egg-info/not-zip-safe
 kiwi_keg.egg-info/requires.txt
 kiwi_keg.egg-info/top_level.txt
-kiwi_keg/changelog_generator/__init__.py
-kiwi_keg/changelog_generator/generate_recipes_changelog.py
-kiwi_keg/obs_service/__init__.py
-kiwi_keg/obs_service/compose_kiwi_description.py
-kiwi_keg/obs_service/compose_kiwi_description.service
+kiwi_keg/tools/__init__.py
+kiwi_keg/tools/compose_kiwi_description.py
+kiwi_keg/tools/generate_recipes_changelog.py
+obs/compose_kiwi_description.service
 package/python-kiwi-keg.changes
 package/python-kiwi-keg.spec
```

### Comparing `kiwi_keg-2.0.2/kiwi_keg.egg-info/PKG-INFO` & `kiwi_keg-2.1.1/kiwi_keg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kiwi-keg
-Version: 2.0.2
+Version: 2.1.1
 Summary: KEG - Image Composition Tool
 Home-page: https://github.com/SUSE-Enceladus/keg
+Download-URL: https://download.opensuse.org
 Author: Public Cloud Team
-Author-email: public-cloud-dev@suse.de
+Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
-Download-URL: https://download.opensuse.org
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Operating System
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 KEG - Image Compositon Tool
 ===========================
 
@@ -26,14 +26,16 @@
 
 |GitHub CI Action|
 
 keg is a command line tool that creates a
 `kiwi <https://github.com/OSInside/kiwi>`_ image description based on
 description snippets in a given GIT repository.
 
+`User documentation <https://documentation.suse.com/appliance/keg-2/html/keg/index.html>`_.
+
 Contributing
 ------------
 
 keg is written in Python, it uses `tox <https://tox.readthedocs.io/en/latest/>`_
 to setup a development environment for the desired Python version. Make
 sure the Python development headers are installed (e.g. `python36-devel`).
 KIWI uses `jing` for detailed error reporting in case schema validation fails.
@@ -41,27 +43,27 @@
 installed on your system.
 
 Currently, there are 5 targets for tox:
 
 - **check**: for code quality and integrity
 - **devel**: for development
 - **doc**: for building man pages
-- **unit_py3_8**: to run unit tests with Python version set to *3.8*
+- **unit_py3_10**: to run unit tests with Python version set to *3.10*
 - **unit_py3_6**: to run unit tests with Python version set to *3.6*
 
 The following procedure describes how to create the development environment:
 
 1. Let tox create the virtual environment(s):
 
    .. code:: bash
 
        $ tox -e devel
 
 2. Activate the virtual environment
-    
+
    .. code:: bash
 
        $ source .tox/3/bin/activate
 
 3. Install requirements inside the virtual environment:
 
    .. code:: bash
@@ -83,9 +85,7 @@
 .. code:: bash
 
    $ deactivate
 
 To resume your work, change into your local Git repository and
 run `source .tox/3/bin/activate` again. Skip step 3 and 4 as
 the requirements are already installed.
-
-
```

### Comparing `kiwi_keg-2.0.2/LICENSE` & `kiwi_keg-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/kiwi_keg/source_info_generator.py` & `kiwi_keg-2.1.1/kiwi_keg/source_info_generator.py`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/kiwi_keg/script_utils.py` & `kiwi_keg-2.1.1/kiwi_keg/script_utils.py`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/kiwi_keg/image_schema.py` & `kiwi_keg-2.1.1/kiwi_keg/image_schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,25 +17,51 @@
 #
 from schema import (
     Schema, And, Or, Optional
 )
 from kiwi_keg.annotated_mapping import AnnotatedMapping
 
 
-class ImageSchema:
+class NamespaceSchema(Schema):
+    def __init__(self, schema, **kwargs):
+        # Generally ignore extra keys; this schema is a sub-set of the full
+        # kiwi schema.
+        kwargs['ignore_extra_keys'] = True
+        super().__init__(schema, **kwargs)
+
+    def validate(self, data):
+        if isinstance(data, dict) and '_namespace' in [x[:10] for x in data.keys()]:
+            namespaces = [x for x in data.keys() if x.startswith('_namespace')]
+            # We create a copy of the input data, remove all namespace keys,
+            # then copy each namespace into the copied dict and validate.
+            # This way namespaces seem invisible and don't have to be accounted
+            # for in the schema, but all namespaced data is validated against
+            # the schema.
+            for ns in namespaces:
+                tmp = data.copy()
+                for del_ns in namespaces:
+                    del tmp[del_ns]
+                tmp.update(data[ns])
+                val = super().validate(tmp)
+        else:
+            val = super().validate(data)
+        return val
+
+
+class ImageSchema():
     def __init__(self):
         self._schema = Schema(
             {
                 Optional('schema'): And(str),
                 Optional('include-paths'): [And(str)],
-                'image': {
+                'image': NamespaceSchema({
                     '_attributes': {
                         'schemaversion': And(str),
                         'name': And(str),
-                        'displayname': And(str),
+                        Optional('displayname'): And(str),
                     },
                     'description': {
                         '_attributes': {
                             'type': And(str),
                         },
                         'author': And(str),
                         'contact': And(str),
@@ -45,32 +71,38 @@
                         Optional('profile'): [{
                             '_attributes': {
                                 'name': And(str),
                                 'description': And(str)
                             }
                         }],
                     },
-                    'preferences': [
-                        {
-                            'version': And(str),
-                        },
-                        Optional(
+                    'preferences': Or(
+                        [
                             {
-                                '_attributes': {
-                                    'profiles': [str],
-                                },
-                                'type': {
+                                'version': And(str),
+                            },
+                            Optional(
+                                {
                                     '_attributes': {
-                                        'image': And(str)
+                                        'profiles': [str],
+                                        Optional('arch'): And(str)
+                                    },
+                                    'type': {
+                                        '_attributes': {
+                                            'image': And(str)
+                                        }
                                     }
-                                }
-                            },
-                            ignore_extra_keys=True
-                        )
-                    ],
+                                }, ignore_extra_keys=True
+                            )
+                        ],
+                        {
+                            'version': And(str),
+                        },
+                        ignore_extra_keys=True
+                    ),
                     'repository': [
                         {
                             '_attributes': {
                                 'type': And(str)
                             },
                             'source': {
                                 '_attributes': {
@@ -89,29 +121,46 @@
                             Optional('archive'): [
                                 {
                                     '_attributes': {
                                         'name': And(str),
                                     }
                                 }
                             ],
-                            str: {
-                                'package': [Or(
+                            'package': [
+                                Or(
                                     str,
                                     {
                                         '_attributes': {
                                             'name': And(str),
                                             Optional('arch'): Or(str, [str])
                                         }
                                     },
                                     ignore_extra_keys=True
-                                )]
-                            }
+                                )
+                            ]
                         }
-                    ]
-                },
+                    ],
+                    Optional('drivers'): [
+                        {
+                            Optional('_map_attribute'): And(str),
+                            'file': [
+                                Or(
+                                    str,
+                                    {
+                                        '_attributes': {
+                                            'name': And(str),
+                                            Optional('arch'): Or(str, [str])
+                                        }
+                                    },
+                                    ignore_extra_keys=True
+                                )
+                            ]
+                        }
+                    ],
+                }),
                 Optional('config'): [
                     Or(
                         {
                             'files': {
                                 str: [{
                                     Optional('append'): And(bool),
                                     'content': And(str),
@@ -169,14 +218,20 @@
                 Optional('archive'): [
                     {
                         'name': And(str),
                         str: {
                             '_include_overlays': [str]
                         }
                     }
+                ],
+                Optional('xmlfiles'): [
+                    {
+                        'name': And(str),
+                        'content': And(dict)
+                    }
                 ]
             },
             ignore_extra_keys=True
         )
 
     def validate(self, data):
         if isinstance(data, AnnotatedMapping):
```

### Comparing `kiwi_keg-2.0.2/kiwi_keg/kiwi_description.py` & `kiwi_keg-2.1.1/kiwi_keg/kiwi_description.py`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/kiwi_keg/logger_filter.py` & `kiwi_keg-2.1.1/kiwi_keg/logger_filter.py`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/kiwi_keg/generator.py` & `kiwi_keg-2.1.1/kiwi_keg/generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 SUSE Software Solutions Germany GmbH. All rights reserved.
+# Copyright (c) 2023 SUSE Software Solutions Germany GmbH. All rights reserved.
 #
 # This file is part of keg.
 #
 # keg is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -70,14 +70,17 @@
         self.gen_profiles_comment = gen_profiles_comment
         loaders = []
         for root in reversed(image_definition.recipes_roots):
             loaders.append(FileSystemLoader(os.path.join(root, 'schemas')))
         self.env = Environment(
             loader=ChoiceLoader(loaders)
         )
+        self.filter_def = {}
+        if self.archs:
+            self.filter_def = {'arch': self.archs}
 
         self.image_definition.populate()
 
         self.image_schema: Optional[str] = self.image_definition.data.get('schema')
 
     def create_kiwi_description(self, overwrite: bool = False) -> None:
         file_utils.raise_on_file_exists(self.kiwi_description, overwrite)
@@ -133,18 +136,15 @@
             if self.archs:
                 arch_comment = 'OBS-ExclusiveArch: {}'.format(
                     ' '.join(self.archs)
                 )
                 content_handler.comment(arch_comment)
                 content_handler.ignorableWhitespace('\n')
             content_handler.ignorableWhitespace('\n')
-            filter_arg = {}
-            if self.archs:
-                filter_arg = {'arch': self.archs}
-            self._create_xml_node('image', self.image_definition.data['image'], content_handler, filter_attributes=filter_arg)
+            self._create_xml_node('image', self.image_definition.data['image'], content_handler, filter_attributes=self.filter_def)
             content_handler.endDocument()
 
     def validate_kiwi_description(self) -> None:
         kiwi = KiwiDescription(self.kiwi_description)
         kiwi.validate_description()
 
     def format_kiwi_description(self, markup: str = 'xml') -> None:
@@ -245,14 +245,19 @@
                 mbuild_obj.write('<multibuild>\n')
                 for profile in profiles:
                     profile_name = dict_utils.get_attribute(profile, 'name')
                     if profile_name:
                         mbuild_obj.write('    <flavor>{}</flavor>\n'.format(profile_name))
                 mbuild_obj.write('</multibuild>\n')
 
+    def create_custom_files(self, overwrite: bool = False):
+        if self.image_definition.data.get('xmlfiles'):
+            for custom_file in self.image_definition.data['xmlfiles']:
+                self._write_xml_file(custom_file, overwrite)
+
     @staticmethod
     def _tarinfo_set_root(tarinfo):
         tarinfo.uid = tarinfo.gid = 0
         tarinfo.uname = tarinfo.gname = 'root'
         return tarinfo
 
     def _add_dir_to_tar(self, tar, src_dir, subdir=''):
@@ -384,33 +389,49 @@
             indent,
             map_attribute,
             filter_attributes
     ):
         child_indent = 0
         content_handler.ignorableWhitespace(depth * indent)
         if key.startswith('_namespace'):
-            content_handler.comment(f'begin namespace {key[11:]}')
+            if key != '_namespace':
+                content_handler.comment(f'begin namespace {key[11:]}')
         else:
             content_handler.startElement(key, attr)
             child_indent = 1
         if children:
             content_handler.ignorableWhitespace('\n')
         for ck, cv in children:
             self._create_xml_node(ck, cv, content_handler, depth + child_indent,
                                   indent, map_attribute, filter_attributes)
         if cdata:
             content_handler.characters(cdata)
         if children:
             content_handler.ignorableWhitespace(depth * indent)
         if key.startswith('_namespace'):
-            content_handler.comment(f'end namespace {key[11:]}')
+            if key != '_namespace':
+                content_handler.comment(f'end namespace {key[11:]}')
         else:
             content_handler.endElement(key)
         content_handler.ignorableWhitespace('\n')
 
+    def _write_xml_file(self, data, overwrite: bool = False):
+        outpath = os.path.join(self.dest_dir, data['name'])
+        if os.path.exists(outpath) and not overwrite:
+            raise KegError(
+                '{target} exists, use force to overwrite.'.format(
+                    target=outpath
+                )
+            )
+        with open(outpath, 'w') as outf:
+            content_handler = ContentGenerator(out=outf, encoding='utf-8', short_empty_elements=True)
+            for node_name, node_data in data['content'].items():
+                self._create_xml_node(node_name, node_data, content_handler, filter_attributes=self.filter_def)
+            content_handler.endDocument()
+
 
 class ContentGenerator(XMLGenerator):
     def comment(self, text):
         self._finish_pending_start_element()
         self._write('<!-- {} -->'.format(text))
```

### Comparing `kiwi_keg-2.0.2/kiwi_keg/keg.py` & `kiwi_keg-2.1.1/kiwi_keg/keg.py`

 * *Files 13% similar despite different names*

```diff
@@ -118,26 +118,44 @@
         images = {}
         for image_src in sorted(image_dirs):
             try:
                 image_definition = KegImageDefinition(
                     image_name=image_src,
                     recipes_roots=roots
                 )
-                image_definition.populate()
+                image_definition.populate_header()
                 image_spec = image_definition.data['image']
+                if isinstance(image_spec['preferences'], list):
+                    ver = image_spec['preferences'][0].get('version', 'n/a')
+                else:
+                    ver = image_spec['preferences'].get('version', 'n/a')
                 images[image_src] = {
                     'name': image_spec['_attributes']['name'],
                     'desc': image_spec['description']['specification'],
-                    'ver': image_spec['preferences'][0].get('version', 'n/a')
+                    'ver': ver
                 }
             except KegError as e:
-                log.error('{} is not a valid image: {}'.format(image_src, e))
-        print('{:30s} {:30s} {:8s} {}'.format('Source', 'Name', 'Version', 'Description'))
+                log.error('{} is not a valid image definition: {}'.format(image_src, e))
+            except KeyError as e:
+                log.error('{} is not a valid image definition, missing key "{}"'.format(image_src, e))
+
+        header = ['Source', 'Name', 'Version', 'Description']
+        max_src = len(header[0])
+        max_name = len(header[1])
+        max_ver = len(header[2])
+        max_desc = len(header[3])
+        for image, spec in images.items():
+            max_src = len(image) if len(image) > max_src else max_src
+            max_name = len(spec['name']) if len(spec['name']) > max_name else max_name
+            max_ver = len(spec['ver']) if len(spec['ver']) > max_ver else max_ver
+            max_desc = len(spec['desc']) if len(spec['desc']) > max_desc else max_desc
+
+        print(f'{header[0]:{max_src}s} {header[1]:{max_name}s} {header[2]:{max_ver}s} {header[3]}')
         for image, spec in images.items():
-            print('{:30s} {:30s} {:8s} {}'.format(image, spec['name'], spec['ver'], spec['desc']))
+            print(f'{image:{max_src}s} {spec["name"]:{max_name}s} {spec["ver"]:{max_ver}s} {spec["desc"]}')
         return
 
     try:
         image_definition = KegImageDefinition(
             image_name=args['SOURCE'],
             recipes_roots=roots,
             image_version=args['--image-version'],
@@ -169,14 +187,17 @@
         image_generator.create_custom_scripts(
             overwrite=args['--force']
         )
         image_generator.create_overlays(
             disable_root_tar=args['--disable-root-tar'],
             overwrite=args['--force']
         )
+        image_generator.create_custom_files(
+            overwrite=args['--force']
+        )
         if not args['--disable-multibuild']:
             image_generator.create_multibuild_file(
                 overwrite=args['--force']
             )
         if args['--write-source-info']:
             source_info_generator = SourceInfoGenerator(
                 image_definition=image_definition,
```

### Comparing `kiwi_keg-2.0.2/kiwi_keg/obs_service/compose_kiwi_description.py` & `kiwi_keg-2.1.1/kiwi_keg/tools/compose_kiwi_description.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         [--image-version=<VERSION>]
         [--arch=<arch>] ...
         [--version-bump=<true|false>]
         [--update-changelogs=<true|false>]
         [--update-revisions=<true|false>]
         [--force=<true|false>]
         [--generate-multibuild=<true|false>]
+        [--new-image-change=<changelog_entry>]
+        [--changelog-format=<format>]
     compose_kiwi_description -h | --help
     compose_kiwi_description --version
 
 Options:
     --git-recipes=<git_clone_source>
         Remote git repository containing keg-recipes (multiples allowed).
 
@@ -68,26 +70,43 @@
     --force=<true|false>
         If true, refresh image description even if there are no new commits.
         [default: false]
 
     --generate-multibuild=<true|false>
         If true, generate a _multibuild file if the image definition has
         profiles defined. [default: true]
+
+    --new-image-change=<changelog_entry>
+        If set, when generating a net new image description, use
+        changelog_entry as the sole entry in the generated change log instead
+        of using the full commit history. [default: None]
+
+    --changelog-format=<format>
+        Use format as output format for the generated change log. Supported
+        values are 'yaml', 'json', and 'osc'. Existing change logs will be
+        converted if necessary. Conversion from 'osc' is not supported.
+        [default: json]
+
+
 """
-import glob
 import docopt
+import glob
 import itertools
+import json
 import logging
 import os
+import pathlib
+import subprocess
 import sys
+import tempfile
+import yaml
+import xml.etree.ElementTree as ET
+
+from datetime import datetime, timezone
 
-from kiwi.xml_description import XMLDescription
-from kiwi.utils.temporary import Temporary
-from kiwi.command import Command
-from kiwi.path import Path
 from kiwi_keg.version import __version__
 from kiwi_keg.image_definition import KegImageDefinition
 from kiwi_keg.generator import KegGenerator
 from kiwi_keg.source_info_generator import SourceInfoGenerator
 
 
 log = logging.getLogger('compose_keg_description')
@@ -100,52 +119,60 @@
         self._head_commit = get_head_commit_hash(path.name)
         self._start_commit = None
 
     def set_start_commit(self, commit):
         self._start_commit = commit
 
     @property
-    def path(self):
+    def pathname(self):
         return self._path.name
 
     @property
     def head_commit(self):
         return self._head_commit
 
     @property
     def start_commit(self):
         return self._start_commit
 
     def has_commits(self):
         return self._start_commit != self._head_commit
 
 
-def get_kiwi_data(kiwi_config):
-    description = XMLDescription(kiwi_config)
-    return description.load()
+def repr_mstr(dumper, data):
+    if '\n' in data:
+        tag = u'tag:yaml.org,2002:str'
+        return dumper.represent_scalar(tag, data, style='|')
+    return dumper.represent_str(data)
 
 
 def get_head_commit_hash(repo_path):
-    result = Command.run(['git', '-C', repo_path, 'show', '--no-patch', '--format=%H', 'HEAD'])
-    return result.output.strip('\n')
+    result = subprocess.run(
+        ['git', '-C', repo_path, 'show', '--no-patch', '--format=%H', 'HEAD'],
+        capture_output=True,
+        encoding='UTF-8'
+    )
+    return result.stdout.strip('\n')
 
 
 def get_image_version(kiwi_config):
     # It is expected that the <version> setting exists only once
     # in a keg generated image description. KIWI allows for profiled
     # <preferences> which in theory also allows to distribute the
     # <version> information between several <preferences> sections
     # but this would be in general questionable and should not be
     # be done any case by keg managed recipes. Thus the following
     # code takes the first version setting it can find and takes
     # it as the only version information available
-    for preferences in get_kiwi_data(kiwi_config).get_preferences():
-        image_version = preferences.get_version()
-        if image_version:
-            return image_version[0]
+    tree = ET.parse(kiwi_config)
+    root = tree.getroot()
+    for preferences in root.findall('preferences'):
+        image_version = preferences.find('version')
+        if image_version is not None:
+            return image_version.text
     if not image_version:
         sys.exit('Cannot determine image version.')
 
 
 def parse_revisions(repos):
     if os.path.exists('_keg_revisions'):
         with open('_keg_revisions') as inf:
@@ -155,82 +182,170 @@
                     sys.exit('Malformed revision spec "{}".'.format(line.strip('\n')))
                 repo = repos.get(rev_spec[0])
                 if not repo:
                     log.warning('Cannot map URL "{}" to repository.'.format(rev_spec[0]))
                 else:
                     repo.set_start_commit(rev_spec[1])
     else:
-        log.warning(
-            'No _keg_revision file. '
-            'Changes file(s) will contain all applicable commit messages.'
+        log.info(
+            'No _keg_revision file.'
         )
 
 
 def get_revision_args(repos):
     rev_args = []
     for repo in repos.values():
         if repo.start_commit:
-            rev_args += ['-r', '{}:{}..'.format(repo.path, repo.start_commit)]
+            rev_args += ['-r', '{}:{}..'.format(repo.pathname, repo.start_commit)]
     return rev_args
 
 
-def generate_changelog(source_log, changes_file, image_version, rev_args):
-    result = Command.run(
+def generate_changelog(source_log, changes_file, log_format, image_version, rev_args):
+    result = subprocess.run(
         [
             'generate_recipes_changelog',
             '-o', changes_file,
-            '-f', 'yaml',
+            '-f', log_format,
             '-t', image_version,
             *rev_args,
             source_log
-        ], raise_on_error=False
+        ]
     )
     if result.returncode == 1:
-        sys.exit('Error generating change log: {}'.format(result.error))
+        sys.exit('Error generating change log.')
     # generate_recipes_changelog returns 2 in case there were no changes
     # return True or False accordingly
     return result.returncode == 0
 
 
-def update_changelog(changes_old, changes_new):
-    if os.path.exists(changes_old):
-        with open(changes_new, 'a') as outf, open(changes_old) as inf:
+def read_changelog(log_file):
+    changes = None
+    if log_file.endswith('.txt'):
+        with open(log_file, 'r') as inf:  # pragma: no cover
+            changes = inf.read()          # pragma: no cover
+    elif log_file.endswith('.yaml'):
+        with open(log_file, 'r') as inf:
+            changes = yaml.safe_load(inf)
+    elif log_file.endswith('.json'):
+        with open(log_file, 'r') as inf:
+            changes = json.load(inf)
+    else:
+        log.warning('Unsupported log format {}'.format(log_file))
+    return changes
+
+
+def update_changelog(log_file, log_format):
+    old_logs = glob.glob(pathlib.Path(log_file).stem + '.*')
+    if old_logs:
+        old_log = old_logs[0]
+        if len(old_logs) > 1:
+            log.warning('More than one format for old log, using {}'.format(old_log))
+    else:
+        log.info('No old log')
+        return
+
+    old_log_format = pathlib.Path(old_log).suffix[1:]
+    if old_log_format == 'txt':
+        old_log_format = 'osc'
+
+    if log_format != 'json' and log_format == old_log_format:
+        # simply concatenate old log to new one
+        with open(log_file, 'a') as outf, open(old_log) as inf:
+            log.info('Appending old changes to {}'.format(log_file))
             outf.write(inf.read())
+    else:
+        if old_log_format == 'osc':
+            log.warning('Converting text log files is not supported, losing history')
+            return
+        else:
+            # different formats, or both json which needs merge
+            log.info('Reading old changes from {}'.format(old_log))
+            old_changes = read_changelog(old_log)
+            if old_changes:
+                if log_format == 'osc':
+                    log.info('Appending old changes to {}'.format(pathlib.Path(log_file).name))
+                    write_changelog(log_file, log_format, old_changes, append=True)
+                else:
+                    new_changes = read_changelog(log_file)
+                    new_changes.update(old_changes)
+                    log.info('Writing merged changes to {}'.format(pathlib.Path(log_file).name))
+                    write_changelog(log_file, log_format, new_changes)
+
+
+def get_osc_log(ver, entries):
+    change = '-------------------------------------------------------------------\n'
+    if hasattr(datetime, 'fromisoformat'):
+        change += datetime.fromisoformat(entries[0]['date']).strftime('%c UTC')  # pragma: nocover_py36
+    else:
+        import iso8601  # pragma: nocover
+        change += iso8601.parse_date(entries[0]['date']).strftime('%c UTC')  # pragma: nocover
+    change += '\n'
+    indent = '- '
+    if ver:
+        change += '\n- Update to {}\n'.format(ver)
+        indent = '  + '
+    for entry in entries:
+        change += indent
+        change += '{}\n'.format(entry['change'])
+    return change
 
 
 def update_revisions(repos, outdir):
     with open(os.path.join(outdir, '_keg_revisions'), 'w') as outf:
         for rname, rinfo in repos.items():
             print('{} {}'.format(rname, rinfo.head_commit), file=outf)
 
 
 def get_log_sources(logdir):
     for source_log in glob.glob(os.path.join(logdir, 'log_sources*')):
         flavor = source_log[len(os.path.join(logdir, 'log_sources')) + 1:]
         yield source_log, flavor
 
 
+def write_changelog(log_file, log_format, changes, append=False):
+    open_mode = 'w'
+    if append:
+        open_mode = 'a'
+    with open(log_file, open_mode) as outf:
+        if log_format == 'osc':
+            for image_version in changes:
+                if changes[image_version]:
+                    print(get_osc_log(image_version, changes[image_version]), file=outf)
+        elif log_format == 'yaml':
+            yaml.add_representer(str, repr_mstr, Dumper=yaml.SafeDumper)
+            yaml.safe_dump(changes, outf, sort_keys=False)
+        elif log_format == 'json':
+            json.dump(changes, outf, indent=2, default=str)
+
+
 def main() -> None:
     args = docopt.docopt(__doc__, version=__version__)
 
-    if not os.path.exists(args['--outdir']):
-        Path.create(args['--outdir'])
-
     if len(args['--git-branch']) > len(args['--git-recipes']):
         sys.exit('Number of --git-branch arguments must not exceed number of git repos.')
 
     handle_changelog = args['--update-changelogs'] == 'true'
 
+    if args['--changelog-format'] == 'osc':
+        log_ext = 'txt'
+    elif args['--changelog-format'] in ['yaml', 'json']:
+        log_ext = args['--changelog-format']
+    else:
+        sys.exit('Unknown changelog format {}'.format(args['--changelog-format']))
+
+    if not os.path.exists(args['--outdir']):
+        os.mkdir(args['--outdir'])
+
     repos = {}
     for repo, branch in itertools.zip_longest(args['--git-recipes'], args['--git-branch']):
-        temp_git_dir = Temporary(prefix='keg_recipes.').new_dir()
+        temp_git_dir = tempfile.TemporaryDirectory(prefix='keg_recipes.', dir='.')
         if branch:
-            Command.run(['git', 'clone', '-b', branch, repo, temp_git_dir.name])
+            subprocess.run(['git', 'clone', '-b', branch, repo, temp_git_dir.name])
         else:
-            Command.run(['git', 'clone', repo, temp_git_dir.name])
+            subprocess.run(['git', 'clone', repo, temp_git_dir.name])
         repos[repo] = RepoInfo(temp_git_dir)
 
     parse_revisions(repos)
     repos_with_commits = list(filter(lambda x: x.has_commits() is True, repos.values()))
     if not repos_with_commits:
         log.warning('No repository has new commits.')
         if args['--force'] != 'true':
@@ -247,17 +362,18 @@
             # if old config.kiwi exists, increment patch version number
             version = get_image_version(old_kiwi_config)
             if version:
                 ver_elements = version.split('.')
                 ver_elements[2] = f'{int(ver_elements[2]) + 1}'
                 image_version = '.'.join(ver_elements)
 
+    logging.getLogger('keg').setLevel(logging.INFO)
     image_definition = KegImageDefinition(
         image_name=args['--image-source'],
-        recipes_roots=[x.path for x in repos.values()],
+        recipes_roots=[x.pathname for x in repos.values()],
         track_sources=handle_changelog,
         image_version=image_version
     )
     image_generator = KegGenerator(
         image_definition=image_definition,
         dest_dir=args['--outdir'],
         archs=args['--arch']
@@ -267,42 +383,64 @@
     )
     image_generator.create_custom_scripts(
         overwrite=True
     )
     image_generator.create_overlays(
         disable_root_tar=False, overwrite=True
     )
+    image_generator.create_custom_files(
+        overwrite=True
+    )
     if args['--generate-multibuild']:
         image_generator.create_multibuild_file(overwrite=True)
 
     if handle_changelog:
         sig = SourceInfoGenerator(image_definition, dest_dir=args['--outdir'])
         sig.write_source_info()
         rev_args = get_revision_args(repos)
         have_changes = False
 
         if not image_version:
             image_version = get_image_version(os.path.join(args['--outdir'], 'config.kiwi'))
 
-        for source_log, flavor in get_log_sources(os.path.join(args['--outdir'])):
-            changes_filename = f'{flavor}{"." if flavor else ""}changes.yaml'
-            changes_path = os.path.join(args['--outdir'], changes_filename)
-            have_changes |= generate_changelog(source_log, changes_path, image_version, rev_args)
-
-        if not have_changes:
-            log.warning('Image has no changes.')
-            if args['--force'] != 'true':
-                log.info('Deleting generated files.')
-                for f in next(os.walk(args['--outdir']))[2]:
-                    os.remove(os.path.join(args['--outdir'], f))
-                sys.exit()
-
-        for source_log, flavor in get_log_sources(os.path.join(args['--outdir'])):
-            changes_filename = f'{flavor}{"." if flavor else ""}changes.yaml'
-            changes_new = os.path.join(args['--outdir'], changes_filename)
-            update_changelog(changes_filename, changes_new)
-            # clean up source log
-            os.remove(source_log)
+        if not old_kiwi_config and args['--new-image-change']:
+            # net new image, use supplied change log entry instead of generating
+            # full log from commit history
+            new_changes = {
+                image_version: [
+                    {
+                        'change': args['--new-image-change'],
+                        'date': datetime.now(timezone.utc).isoformat(timespec='minutes')
+                    }
+                ]
+            }
+            for source_log, flavor in get_log_sources(args['--outdir']):
+                changes_filename = f'{flavor}{"." if flavor else ""}changes.{log_ext}'
+                changes_path = os.path.join(args['--outdir'], changes_filename)
+                log.info('Writing {}'.format(changes_path))
+                write_changelog(changes_path, args['--changelog-format'], new_changes)
+                # clean up source log
+                os.remove(source_log)
+        else:
+            for source_log, flavor in get_log_sources(args['--outdir']):
+                changes_filename = f'{flavor}{"." if flavor else ""}changes.{log_ext}'
+                changes_path = os.path.join(args['--outdir'], changes_filename)
+                have_changes |= generate_changelog(source_log, changes_path, args['--changelog-format'], image_version, rev_args)
+
+            if not have_changes:
+                log.warning('Image has no changes.')
+                if args['--force'] != 'true':
+                    log.info('Deleting generated files.')
+                    for f in next(os.walk(args['--outdir']))[2]:
+                        os.remove(os.path.join(args['--outdir'], f))
+                    sys.exit()
+
+            for source_log, flavor in get_log_sources(os.path.join(args['--outdir'])):
+                changes_filename = f'{flavor}{"." if flavor else ""}changes.{log_ext}'
+                changes_path = os.path.join(args['--outdir'], changes_filename)
+                update_changelog(changes_path, args['--changelog-format'])
+                # clean up source log
+                os.remove(source_log)
 
     if args['--update-revisions'] == 'true':
         # capture current commits
         update_revisions(repos, args['--outdir'])
```

### Comparing `kiwi_keg-2.0.2/kiwi_keg/obs_service/compose_kiwi_description.service` & `kiwi_keg-2.1.1/obs/compose_kiwi_description.service`

 * *Files 22% similar despite different names*

```diff
@@ -19,19 +19,25 @@
     <description>set build architecture (multiples allowed, optional)</description>
   </parameter>
   <parameter name="version-bump">
     <description>Whether the patch version number should be incremented. Ignored if '--image-version' is set. If set to 'false' and '--image-version' is not set, the image version defined in the recipes will be used. If no image version is defined, image description generation will fail.  [default: true]
     </description>
   </parameter>
   <parameter name="update-changelogs">
-    <description> Whether 'changes.yaml' files should be updated. [default: true]</description>
+    <description>Whether 'changes.yaml' files should be updated. [default: true]</description>
   </parameter>
   <parameter name="update-revisions">
     <description>Whether '_keg_revisions' should be updated. [default: true]</description>
   </parameter>
   <parameter name="force">
     <description>If 'true' refresh image description even if there are no new commits [default: false]</description>
   </parameter>
   <parameter name="generate-multibuild">
     <description>If 'true', generate a _multibuild file if the image definition has profiles defined. [default: true]</description>
   </parameter>
+  <parameter name="new-image-change">
+    <description>If set, when generating a net new image description, use the given string as the sole entry in the generated change log instead of using the full commit history. [default: None]</description>
+  </parameter>
+  <parameter name="changelog-format">
+    <description>Set output format for generated change log. Supported values are 'yaml', 'json', and 'osc'. Existing change logs will be converted if necessary. Conversion from 'osc' is not supported.  [default: json]</description>
+  </parameter>
 </service>
```

### Comparing `kiwi_keg-2.0.2/kiwi_keg/logger.py` & `kiwi_keg-2.1.1/kiwi_keg/logger.py`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/kiwi_keg/changelog_generator/generate_recipes_changelog.py` & `kiwi_keg-2.1.1/kiwi_keg/tools/generate_recipes_changelog.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,43 +14,47 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with keg. If not, see <http://www.gnu.org/licenses/>
 #
 
 """
 Usage: generate_recipes_changelog [-o OUTPUT_FILE] [-r REV]... [-f FORMAT]
-                                  [-m MSG_FORMAT] [-t ROOT_TAG] LOGFILE
+                                  [-m MSG_FORMAT] [-t ROOT_TAG] [-a AUTHOR_STRING] LOGFILE
        generate_recipes_changelog -h | --help
 
 Arguments:
     LOGFILE    Path to file contaning Keg source log
 
 Options:
     -o OUTPUT_FILE
         Write output to OUTPUT_FILE (stdout if omitted)
 
     -r PATH:REV
         Set git revision range to REV for repo at PATH
 
     -f FORMAT
-        Output format, 'text' or 'yaml' [default: yaml]
+        Output format, 'text','yaml', 'json', or 'osc' [default: json]
 
     -m MSG_FORMAT
         Format spec for commit messages (see 'format:<string>' in 'man git-log')
         [default: - %s] (only used with text format)
 
     -t ROOT_TAG
-        Use ROOT_TAG for yaml output (e.g. image version)
+        Use ROOT_TAG for yaml or json output (e.g. image version)
+
+    -a AUTHOR_STRING
+        Use AUTHOR_STRING (typically name + email) for OSC change log entries
 """
 
 import docopt
+import json
 import subprocess
 import sys
 import yaml
-from datetime import datetime
+from datetime import datetime, timezone
 
 
 class MultiStr(str):
     pass
 
 
 def get_commits_from_range(start, end, filespec, gitroot, rev=None):
@@ -111,15 +115,15 @@
 def get_date_from_epoch(epoch):
     return datetime.utcfromtimestamp(int(epoch)).isoformat()
 
 
 def main():
     args = docopt.docopt(__doc__, version='0.1')
 
-    if args['-f'] not in ['text', 'yaml']:
+    if args['-f'] not in ['text', 'yaml', 'json', 'osc']:
         sys.exit('Unsupported output format "{}".'.format(args['-f']))
 
     with open(args['LOGFILE'], 'r') as inf:
         sources = inf.read().splitlines()
 
     revisions = {}
     if args['-r']:
@@ -164,20 +168,42 @@
                         'date': get_date_from_epoch(commit[0]),
                         'details': body
                     }
                 )
             else:
                 msgs.append({'change': sub,
                              'date': get_date_from_epoch(commit[0])})
-        yaml.add_representer(MultiStr, repr_mstr, Dumper=yaml.SafeDumper)
-        if args['-t']:
-            log = {args['-t']: msgs}
-        else:
-            log = msgs
-        yaml.safe_dump(log, outp)
+        if args['-f'] == 'yaml':
+            yaml.add_representer(MultiStr, repr_mstr, Dumper=yaml.SafeDumper)
+            if args['-t']:
+                log = {args['-t']: msgs}
+            else:
+                log = msgs
+            yaml.safe_dump(log, outp)
+        elif args['-f'] == 'json':
+            if args['-t']:
+                log = {args['-t']: msgs}
+            else:
+                log = msgs
+            json.dump(log, outp, indent=2)
+        elif args['-f'] == 'osc':
+            print('-------------------------------------------------------------------', file=outp)
+            outp.write((datetime.now(timezone.utc).strftime('%c %Z')))
+            if args['-a']:
+                outp.write(' - ')
+                outp.write(args['-a'])
+            outp.write('\n\n')
+            indent = '- '
+            if args['-t']:
+                print('- Update to {}'.format(args['-t']), file=outp)
+                indent = '  + '
+            for msg in msgs:
+                outp.write(indent)
+                print(msg['change'], file=outp)
+            outp.write('\n')
 
     if args['-o']:
         outp.close()
 
     if not commits:
         sys.exit(2)
```

### Comparing `kiwi_keg-2.0.2/kiwi_keg/exceptions.py` & `kiwi_keg-2.1.1/kiwi_keg/exceptions.py`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/kiwi_keg/dict_utils.py` & `kiwi_keg-2.1.1/kiwi_keg/dict_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,23 +35,23 @@
     src = {'a': 'foo', 'b': {'c': 'bar'}}
     dest = {'a': 'baz', 'b': {'d': 'more_bar'}}
 
     Result: {'a': 'foo', 'b': {'d': 'more_bar', 'c': 'bar'}}
     """
     if not isinstance(dest, dict) and not isinstance(dest, AnnotatedMapping):
         raise KegDataError(
-            'Cannot rmerge, destination is not a mapping: {} {}'.format(dest, type(dest))
+            'Cannot rmerge, destination is not a mapping: {} {} {}'.format(dest, type(dest), src)
         )
     if isinstance(src, dict):
         items = src.items()
     elif isinstance(src, AnnotatedMapping):
         items = src.all_items()
     else:
         raise KegDataError(
-            'Cannot rmerge, source mapping type not supported: {}'.format(type(src))
+            'Cannot rmerge, source mapping type not supported: {} {}'.format(src, type(src))
         )
 
     for key, value in items:
         if isinstance(value, dict) or isinstance(value, AnnotatedMapping):
             node = dest.setdefault(key, type(value)({}))
             rmerge(value, node)
         elif value is None:
```

### Comparing `kiwi_keg-2.0.2/kiwi_keg/version.py` & `kiwi_keg-2.1.1/kiwi_keg/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with keg. If not, see <http://www.gnu.org/licenses/>
 #
 """
 Global version information used in keg and the package
 """
-__version__ = '2.0.2'
+__version__ = '2.1.1'
 __githash__ = '$Format:%H$'
```

### Comparing `kiwi_keg-2.0.2/kiwi_keg/annotated_mapping.py` & `kiwi_keg-2.1.1/kiwi_keg/annotated_mapping.py`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/kiwi_keg/image_definition.py` & `kiwi_keg-2.1.1/kiwi_keg/image_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,25 +125,45 @@
             raise KegDataError(
                 'Error parsing image data: {error}'.format(error=issue)
             )
 
         try:
             self._expand_includes(self._data)
             if self._image_version:
-                self._data['image']['preferences'][0]['version'] = self._image_version
+                if isinstance(self._data['image']['preferences'], list):
+                    self._data['image']['preferences'][0]['version'] = self._image_version
+                else:
+                    self._data['image']['preferences']['version'] = self._image_version
             ImageSchema().validate(self._data)
             self._generate_config_scripts()
             self._generate_overlay_info()
+            self._check_archive_refs()
         except SchemaError as err:
             raise KegDataError('Image definition malformed: {}'.format(err))
         except Exception as issue:
             raise KegDataError(
                 'Error generating profile data: {error}'.format(error=issue)
             )
 
+    def populate_header(self) -> None:
+        """
+        Parse recipes data but only expand 'image: description'.
+        Used by list command for faster operation.
+        """
+        try:
+            img_dict = file_utils.get_recipes(
+                self.image_roots, [self.image_name], track_sources=self._track_sources
+            )
+            self._data.update(img_dict)
+            self._expand_includes(self._data['image']['description'])
+        except Exception as issue:
+            raise KegDataError(
+                'Error parsing image data: {error}'.format(error=issue)
+            )
+
     def _check_recipes_paths_exist(self):
         for recipes_root in self._recipes_roots:
             if not os.path.isdir(recipes_root):
                 raise KegDataError(
                     'Recipes root "{root}" does not exist'.format(
                         root=recipes_root
                     )
@@ -158,14 +178,24 @@
         if not image_dir_exists:
             raise KegDataError(
                 'Image source path "{image}" does not exist'.format(
                     image=self._image_name
                 )
             )
 
+    def _check_archive_refs(self):
+        pkg_sections = self._data['image'].get('packages')
+        for sect in pkg_sections:
+            archives = sect.get('archive')
+            if archives:
+                for arch_ref in archives:
+                    arch_name = dict_utils.get_attribute(arch_ref, 'name')
+                    if arch_name not in self._data.get('archives', []):
+                        log.warning(f'Referenced archive "{arch_name}" not defined')
+
     def _expand_includes(self, data, key=None):
         if not hasattr(data, '__iter__') or isinstance(data, str):
             return
         if isinstance(data, list):
             for item in data:
                 self._expand_includes(item, key)
             return
```

### Comparing `kiwi_keg-2.0.2/kiwi_keg/file_utils.py` & `kiwi_keg-2.1.1/kiwi_keg/file_utils.py`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/doc/source/installation.rst` & `kiwi_keg-2.1.1/doc/source/installation.rst`

 * *Files 14% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 Installation
 ============
 
 .. note::
 
     This document describes how to install Keg. Currently `keg` is
-    available from `PyPi <https://pypi.org/project/kiwi_keg/>`__ and from the
+    available from `PyPi <https://pypi.org/project/kiwi-keg/>`__ and from the
     `openSUSE Build Service
-    <https://build.opensuse.org/package/show/Cloud:Tools/python-kiwi_keg/>`__
-    for several openSUSE distributions.
+    <https://build.opensuse.org/package/show/Cloud:Toolr/python-kiwi-keg/>`__
+    for several openSUSE distributions. It is included in openSUSE Tumbleweed.
 
 
 Installation from openSUSE Cloud:Tools repository
 -------------------------------------------------
 
 `Keg` is available for various openSUSE distributions from the `Cloud:Tools
 repository <https://download.opensuse.org/repositories/Cloud:/Tools/>`__ in the
-openSUSE Build Service. Package name is `python[py_version]-kiwi_keg`.
+openSUSE Build Service. Package name is `python[py_version]-kiwi-keg`.
 
 Installation from PyPI
 ----------------------
 
 `Keg` can be obtained from the Python Package Index (PyPi) via Python's
 package manager pip:
```

### Comparing `kiwi_keg-2.0.2/doc/source/conf.py` & `kiwi_keg-2.1.1/doc/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Keg documentation build configuration file
 #
 import sys
-from os.path import abspath, dirname, join, normpath
-import shlex
+from os.path import dirname, join, normpath
 import sphinx_rtd_theme
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 _path = normpath(join(dirname(__file__), "../.."))
 sys.path.insert(0, _path)
@@ -33,27 +32,27 @@
 
 # The encoding of source files.
 source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
-default_role="py:obj"
+default_role = "py:obj"
 
 # General information about the project.
 project = 'Keg - Image Composition Tool'
 copyright = '2022, SUSE - Public Cloud Team'
 author = 'public-cloud-dev@susecloud.net'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '2.0.2'
+version = '2.1.1'
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
@@ -78,18 +77,18 @@
 
 
 autosummary_generate = True
 
 # -- Options for HTML output ----------------------------------------------
 
 html_sidebars = {
-   '**': [
-          'localtoc.html', 'relations.html',
-          'about.html', 'searchbox.html',
-         ]
+    '**': [
+        'localtoc.html', 'relations.html',
+        'about.html', 'searchbox.html',
+    ]
 }
 
 html_theme = "sphinx_rtd_theme"
 
 html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 
 html_theme_options = {
```

### Comparing `kiwi_keg-2.0.2/doc/source/commands/keg.rst` & `kiwi_keg-2.1.1/doc/source/commands/keg.rst`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 .. _keg_synopsis:
 
 SYNOPSIS
 --------
 
 **keg** [*options*] <*source*>
 
+.. _keg_description:
+
 DESCRIPTION
 -----------
 
 :program:`keg` is a tool which helps to create and manage image descriptions
 suitable for the `KIWI <https://osinside.github.io/kiwi/>`__ appliance builder.
 While :program:`keg` can be used to manage a single image definition the tool
 provides no considerable advantage in such a use case. The primary use case for
@@ -24,106 +26,110 @@
 :ref:`recipes_basics` for more information about `recipes`.
 
 The `recipes` used for generating SUSE Public Cloud image descriptions
 can be found in the
 `Public Cloud Keg Recipes <https://github.com/SUSE-Enceladus/keg-recipes>`__
 repository.
 
-.. _keg_options:
+.. _keg_args:
 
 ARGUMENTS
 ---------
 
 source
 
   Path to image source under RECIPES_ROOT/images
 
+.. _keg_options:
+
 OPTIONS
 -------
 
 .. program:: keg
 
-.. option:: -r RECIPES_ROOT, --recipes-root=RECIPES_ROOT
+-r RECIPES_ROOT, --recipes-root=RECIPES_ROOT
 
    Root directory of keg recipes. Can be used more than once. Elements
    from later roots may overwrite earlier one.
 
-.. option:: -d DEST_DIR, --dest-dir=DEST_DIR
+-d DEST_DIR, --dest-dir=DEST_DIR
 
    Destination directory for generated description [default: .]
 
-.. option:: --disable-multibuild
+--disable-multibuild
 
    Option to disable creation of OBS _multibuild file (for image
    definitions with multiple profiles). [default: false]
 
-.. option:: --disable-root-tar
+--disable-root-tar
 
    Option to disable the creation of root.tar.gz in destination directory.
    If present, an overlay tree will be created instead.
    [default: false]
 
-.. option:: --dump-dict
+--dump-dict
 
    Dump generated data dictionary to stdout instead of generating an image
    description. Useful for debugging.
 
-.. option:: -l, --list-recipes
+-l, --list-recipes
 
    List available images that can be created with the current recipes
 
-.. option:: -f, --force
+-f, --force
 
    Force mode (ignore errors, overwrite files)
 
-.. option:: --format-yaml
+--format-yaml
 
    Format/Update Keg written image description to installed
    KIWI schema and write the result description in YAML markup
 
    .. note::
       Currently no translation of comment blocks from the Keg
       generated KIWI description to the YAML markup will be
       performed.
 
-.. option:: --format-xml
+--format-xml
 
    Format/Update Keg written image description to installed
    KIWI schema and write the result description in XML markup
 
    .. note::
       Currently only top-level header comments from the Keg
       written image description will be preserved into the
       formatted/updated KIWI XML file. Inline comments will
       not be preserved.
 
-.. option:: -i IMAGE_VERSION, --image-version=IMAGE_VERSION
+-i IMAGE_VERSION, --image-version=IMAGE_VERSION
 
    Set image version
 
-.. option:: -a ARCH
+-a ARCH
 
    Generate image description for architecture ARCH (can be used
    multiple times)
 
-.. option:: -s, --write-source-info
+-s, --write-source-info
 
    Write a file per profile containing a list of all used source
    locations. The files can used to generate a change log from the
    recipes repository commit log.
 
-.. option:: -v, --verbose
+-v, --verbose
 
    Enable verbose output
 
-.. option:: --version
+--version
 
    Print version
 
 
+.. _keg_example:
+
 EXAMPLE
 -------
 
 .. code:: bash
 
    git clone https://github.com/SUSE-Enceladus/keg-recipes.git
```

### Comparing `kiwi_keg-2.0.2/doc/source/commands/generate_recipes_changelog.rst` & `kiwi_keg-2.1.1/doc/source/commands/generate_recipes_changelog.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,75 @@
 .. _generate_recipes_changelog:
 
-generated_recipes_changelog
-===========================
+generate_recipes_changelog
+==========================
 
 .. _generate_recipes_changelog_synopsis:
 
 SYNOPSIS
 --------
 
 **generate_recipes_changelog** [*options*] <logfile>
 
+.. _generate_recipes_changelog_description:
+
 DESCRIPTION
 -----------
 
 :program:`generate_recipes_changelog` generates a change log from the git
 commit history of one or more `keg-recipes` repositories. The input file is a
 source info log that is generated by :program:`keg` when run with source
 tracking enabled (`-s` command line switch).
 
 The exit status is 0 in case a change log was generated successfully, 1
 in case an error occurred, or 2 in case no error occurred but generated
 change log is empty.
 
-.. _generate_recipes_changelog_options:
+.. _generate_recipes_changelog_args:
 
 ARGUMENTS
 ---------
 
 logfile
 
   A source info log file produced by :program:`keg`.
 
+.. _generate_recipes_changelog_options:
+
 OPTIONS
 -------
 
-.. option:: -o OUTPUT_FILE
+-o OUTPUT_FILE
 
    Write output to OUTPUT_FILE (stdout if omitted)
 
-.. option:: -r PATH:REV
+-r PATH:REV
 
    Set git revision range to REV for repo at PATH
 
    .. note::
       This limits the applicable set of commits to the given revision spec.
       This can be used to select only newer changes from a previous change log
       generator run. See EXAMPLE below.
 
-.. option:: -f FORMAT
+-f FORMAT
 
    Output format, 'text' or 'yaml' [default: yaml]
 
-.. option:: -m MSG_FORMAT
+-m MSG_FORMAT
 
    Format spec for commit messages (see 'format:<string>' in 'man git-log')
    [default: - %s] (only used with text format)
 
-.. option:: -t ROOT_TAG
+-t ROOT_TAG
 
    Use ROOT_TAG for yaml output (e.g. image version)
 
+.. _generate_recipes_changelog_example:
+
 EXAMPLE
 -------
 
 .. code:: bash
 
    generate_recipes_changelog -r /path/to/repo:12345678.. -t 1.1.8 log_sources
```

### Comparing `kiwi_keg-2.0.2/doc/source/data_modules.rst` & `kiwi_keg-2.1.1/doc/source/data_modules.rst`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/doc/source/obs_source_service.rst` & `kiwi_keg-2.1.1/doc/source/obs_source_service.rst`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/doc/source/changelog_generator.rst` & `kiwi_keg-2.1.1/doc/source/changelog_generator.rst`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/doc/source/recipes_basics.rst` & `kiwi_keg-2.1.1/doc/source/recipes_basics.rst`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/doc/source/intersphinx_mapping/objects.inv` & `kiwi_keg-2.1.1/doc/source/intersphinx_mapping/objects.inv`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/doc/source/overview.rst` & `kiwi_keg-2.1.1/doc/source/overview.rst`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/doc/source/image_definition.rst` & `kiwi_keg-2.1.1/doc/source/image_definition.rst`

 * *Files 3% similar despite different names*

```diff
@@ -384,14 +384,40 @@
   Keg generates some comments automatically. In case the image definition has
   multiple profiles and the `--disable-multibuild` command line switch is not
   set, it will add an `OBS-Profiles: @BUILD_FLAVOR@` comment. In case the
   image description is generated for one or more specific architectures
   via the `-a` command line option, the apprpriate `OBS-ExclusiveArch`
   comment is added.
 
+
+xmlfiles
+^^^^^^^^
+
+This optional section allows generating additional custom XML files. The format
+is as follows:
+
+.. code:: yaml
+
+  xmlfiles:
+    - name: <filename>
+      content:
+        <content_dictionary>
+    ...
+
+For each list item in this section, an XML file named :file:`<filename>` will
+be created, with the content being generated from the `<content_dictionary>`.
+For this dictionary the same rules about formatting, including, namespacing,
+etc., apply as for the image dictionary.
+
+Custom XML files can be useful when generating image descriptions for use in
+the Open Build Service, which accepts build configuration directives via XML
+source files, like the :file:`_constraints` file. See
+`<https://openbuildservice.org/help/manuals/obs-user-guide/cha.obs.build_job_constraints.html>`__
+for details.
+
 schema
 ^^^^^^
 
 `Keg` starting with version 2.0.0 has an internal XML generator to produce
 `KIWI` image descriptions. Previously, a Jinja2 template was used to convert
 the image dictionary that `keg` constructed into a `KIWI` image description.
 Using a Jinja2 template is still supported and can be configured as follows
```

### Comparing `kiwi_keg-2.0.2/doc/Makefile` & `kiwi_keg-2.1.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `kiwi_keg-2.0.2/README.rst` & `kiwi_keg-2.1.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 |GitHub CI Action|
 
 keg is a command line tool that creates a
 `kiwi <https://github.com/OSInside/kiwi>`_ image description based on
 description snippets in a given GIT repository.
 
+`User documentation <https://documentation.suse.com/appliance/keg-2/html/keg/index.html>`_.
+
 Contributing
 ------------
 
 keg is written in Python, it uses `tox <https://tox.readthedocs.io/en/latest/>`_
 to setup a development environment for the desired Python version. Make
 sure the Python development headers are installed (e.g. `python36-devel`).
 KIWI uses `jing` for detailed error reporting in case schema validation fails.
@@ -21,27 +23,27 @@
 installed on your system.
 
 Currently, there are 5 targets for tox:
 
 - **check**: for code quality and integrity
 - **devel**: for development
 - **doc**: for building man pages
-- **unit_py3_8**: to run unit tests with Python version set to *3.8*
+- **unit_py3_10**: to run unit tests with Python version set to *3.10*
 - **unit_py3_6**: to run unit tests with Python version set to *3.6*
 
 The following procedure describes how to create the development environment:
 
 1. Let tox create the virtual environment(s):
 
    .. code:: bash
 
        $ tox -e devel
 
 2. Activate the virtual environment
-    
+
    .. code:: bash
 
        $ source .tox/3/bin/activate
 
 3. Install requirements inside the virtual environment:
 
    .. code:: bash
```

### Comparing `kiwi_keg-2.0.2/tox.ini` & `kiwi_keg-2.1.1/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -10,109 +10,95 @@
 #    $ tox -e doc
 #
 [tox]
 skip_missing_interpreters = True
 skipsdist = True
 envlist =
     check,
-    unit_py3_8,
-    unit_py3_6,
-    devel,
+    unit_py36,
+    unit_py37,
+    unit_py38,
+    unit_py39,
+    unit_py310,
+    unit_py311,
+    unit_py312,
     doc
 
 [testenv]
-whitelist_externals = *
+allowlist_externals = *
 basepython =
-    {check,devel,doc,doc_suse}: python3
-    unit_py3_8: python3.8
-    unit_py3_6: python3.6
-    release: python3.6
-envdir =
-    {check,devel,doc,doc_suse}: {toxworkdir}/3
-    unit_py3_8: {toxworkdir}/3.8
-    unit_py3_6: {toxworkdir}/3.6
-    release: {toxworkdir}/3.6
+    unit_py36: {env:TOXPYTHON:python3.6}
+    unit_py37: {env:TOXPYTHON:python3.7}
+    unit_py38: {env:TOXPYTHON:python3.8}
+    unit_py39: {env:TOXPYTHON:python3.9}
+    unit_py310: {env:TOXPYTHON:python3.10}
+    unit_py311: {env:TOXPYTHON:python3.11}
+    unit_py312: {env:TOXPYTHON:python3.12}
+    {check,doc,doc_suse,unit}: {env:TOXPYTHON:python3}
 passenv =
     *
 usedevelop = True
-deps =
-    -r.virtualenv.dev-requirements.txt
-
-
-# Unit Test run with basepython set to 3.6
-[testenv:unit_py3_6]
-skip_install = True
-usedevelop = True
 setenv =
-    PYTHONPATH={toxinidir}/test
+    PYTHONPATH={toxinidir}
     PYTHONUNBUFFERED=yes
     WITH_COVERAGE=yes
-passenv =
-    *
-deps = {[testenv]deps}
-changedir=test/unit
+deps = -r.virtualenv.dev-requirements.txt
+changedir = test/unit
+description = Unit test
 commands =
-    bash -c 'cd ../../ && ./setup.py develop'
-
-    {envdir}/bin/mypy --ignore-missing-imports {toxinidir}/kiwi_keg/
-
     pytest --no-cov-on-fail --cov=kiwi_keg \
         --cov-report=term-missing \
         --cov-fail-under=100 {posargs}
 
-
-# Unit Test run with basepython set to 3.8
-[testenv:unit_py3_8]
-skip_install = True
-usedevelop = True
-setenv =
-    PYTHONPATH={toxinidir}/test
-    PYTHONUNBUFFERED=yes
-    WITH_COVERAGE=yes
-passenv =
-    *
-deps = {[testenv]deps}
-changedir=test/unit
+[testenv:unit]
+description = Unit test
 commands =
-    bash -c 'cd ../../ && ./setup.py develop'
-
-    {envdir}/bin/mypy --ignore-missing-imports {toxinidir}/kiwi_keg/
+    pytest --no-cov-on-fail --cov=kiwi_keg \
+        --cov-report=term-missing \
+        --cov-fail-under=100 {posargs}
 
+# Unit Test run with system python3
+[testenv:unit_py36]
+description = Unit test Python 3.6
+deps = -r.virtualenv.dev-requirements-py36.txt
+changedir = test/unit
+commands =
     pytest --doctest-modules --no-cov-on-fail --cov=kiwi_keg \
         --cov-report=term-missing \
-        --cov-fail-under=100 {posargs}
+        --cov-fail-under=100 {posargs} \
+        --cov-config=.coveragerc_py36
 
 # Documentation build
 [testenv:doc]
+description = Test documentation build
 skip_install = True
 usedevelop = True
 deps = {[testenv]deps}
-changedir=doc
+changedir = doc
 commands =
     {[testenv:doc.html]commands}
     {[testenv:doc.man]commands}
 
 [testenv:doc_suse]
 description = Documentation build suitable for SUSE documentation
 skip_install = True
-usedevelop = True
 deps = {[testenv:doc]deps}
-changedir=doc
+changedir = doc
 commands =
     {[testenv:doc.xml]commands}
     rstxml2docbook -v --no-split -o xml/book.xml build/restxml/index.xml
     cp -a xml build/
     cp DC-keg build/
     bash -c 'cd build && daps -d DC-keg html'
 
 [testenv:doc.html]
 description = Documentation build html result
 skip_install = True
 deps = {[testenv:doc]deps}
-changedir=doc
+changedir = doc
 commands =
     make html
 
 [testenv:doc.xml]
 description = Documentation build xml result
 skip_install = True
 deps = {[testenv:doc]deps}
@@ -131,19 +117,11 @@
     make man
 
 
 # Source code quality/integrity check
 [testenv:check]
 deps = {[testenv]deps}
 skip_install = True
-usedevelop = True
 commands =
     flake8 --statistics -j auto --count {toxinidir}/kiwi_keg
     flake8 --statistics -j auto --count {toxinidir}/test/unit
-
-# PyPi prepare for upload
-[testenv:release]
-deps = {[testenv]deps}
-skip_install = True
-usedevelop = True
-commands =
-    python setup.py sdist
+    mypy --ignore-missing-imports {toxinidir}/kiwi_keg/
```

### Comparing `kiwi_keg-2.0.2/setup.py` & `kiwi_keg-2.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 from os import path
 from setuptools import setup
-from setuptools.command import sdist as setuptools_sdist
-
-import distutils
-import subprocess
 
 from kiwi_keg.version import __version__
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.rst'), encoding='utf-8') as readme:
     long_description = readme.read()
 
@@ -19,41 +15,43 @@
     'long_description': long_description,
     'long_description_content_type': 'text/x-rst',
     'description': 'KEG - Image Composition Tool',
     'author': 'Public Cloud Team',
     'url': 'https://github.com/SUSE-Enceladus/keg',
     'download_url':
         'https://download.opensuse.org',
-    'author_email': 'public-cloud-dev@suse.de',
+    'author_email': 'public-cloud-dev@susecloud.net',
     'version': __version__,
-    'license' : 'GPLv3+',
+    'license': 'GPLv3+',
     'install_requires': [
         'docopt',
         'Jinja2',
         'kiwi>=9.21.21',
         'PyYAML',
-        'schema'
+        'schema',
+        'iso8601; python_version < "3.7.0"'
     ],
-    'packages': ['kiwi_keg','kiwi_keg.changelog_generator','kiwi_keg.obs_service'],
+    'packages': ['kiwi_keg', 'kiwi_keg.tools'],
     'entry_points': {
         'console_scripts': [
             'keg=kiwi_keg.keg:main',
-            'compose_kiwi_description=kiwi_keg.obs_service.compose_kiwi_description:main',
-            'generate_recipes_changelog=kiwi_keg.changelog_generator.generate_recipes_changelog:main'
+            'compose_kiwi_description=kiwi_keg.tools.compose_kiwi_description:main',
+            'generate_recipes_changelog=kiwi_keg.tools.generate_recipes_changelog:main'
         ]
     },
     'include_package_data': True,
     'zip_safe': False,
     'classifiers': [
-       # classifier: http://pypi.python.org/pypi?%3Aaction=list_classifiers
-       'Development Status :: 2 - Pre-Alpha',
-       'Intended Audience :: Developers',
-       'License :: OSI Approved :: '
-       'GNU General Public License v3 or later (GPLv3+)',
-       'Operating System :: POSIX :: Linux',
-       'Programming Language :: Python :: 3.6',
-       'Programming Language :: Python :: 3.8',
-       'Topic :: System :: Operating System',
+        # classifier: http://pypi.python.org/pypi?%3Aaction=list_classifiers
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: '
+        'GNU General Public License v3 or later (GPLv3+)',
+        'Operating System :: POSIX :: Linux',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.10',
+        'Topic :: System :: Operating System',
     ]
 }
 
 setup(**config)
```

### Comparing `kiwi_keg-2.0.2/Makefile` & `kiwi_keg-2.1.1/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -13,34 +13,31 @@
 )
 
 install_package_docs:
 	install -d -m 755 ${buildroot}${docdir}/$(PKG)
 	install -m 644 LICENSE \
 		${buildroot}${docdir}/$(PKG)/LICENSE
 	install -m 644 README.rst \
-		${buildroot}${docdir}/$(PKG)/README
+		${buildroot}${docdir}/$(PKG)/README.rst
 
 install:
 	# manual pages
 	install -d -m 755 ${buildroot}usr/share/man/man1
-	for man in doc/build/man/*.1; do \
-		test -e $$man && gzip -f $$man || true ;\
-	done
-	for man in doc/build/man/*.1.gz; do \
+	for man in doc/build/man/*.1 ; do \
 		install -m 644 $$man ${buildroot}usr/share/man/man1 ;\
 	done
 	# keg obs service
 	install -d -m 755 ${buildroot}usr/lib/obs/service
 	mv ${buildroot}usr/bin/compose_kiwi_description \
 		${buildroot}usr/lib/obs/service
-	install -m 644 kiwi_keg/obs_service/compose_kiwi_description.service \
+	install -m 644 obs/compose_kiwi_description.service \
 		${buildroot}usr/lib/obs/service
 
 tox:
-	tox "-n 5"
+	tox "-p 4"
 
 git_attributes:
 	# the following is required to update the $Format:%H$ git attribute
 	# for details on when this target is called see setup.py
 	git archive HEAD kiwi_keg/version.py | tar -x
 
 clean_git_attributes:
@@ -51,15 +48,15 @@
 build: clean tox
 	# create setup.py variant for rpm build.
 	# delete module versions from setup.py for building an rpm
 	# the dependencies to the python module rpm packages is
 	# managed in the spec file
 	sed -ie "s@>=[0-9.]*'@'@g" setup.py
 	# build the sdist source tarball
-	$(python) setup.py sdist
+	$(python) -m build
 	# restore original setup.py backed up from sed
 	mv setup.pye setup.py
 	# update rpm changelog using reference file
 	helper/update_changelog.py --since package/$(PKG).changes > \
 		dist/$(PKG).changes
 	helper/update_changelog.py --file package/$(PKG).changes >> \
 		dist/$(PKG).changes
```

### Comparing `kiwi_keg-2.0.2/PKG-INFO` & `kiwi_keg-2.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kiwi_keg
-Version: 2.0.2
+Version: 2.1.1
 Summary: KEG - Image Composition Tool
 Home-page: https://github.com/SUSE-Enceladus/keg
+Download-URL: https://download.opensuse.org
 Author: Public Cloud Team
-Author-email: public-cloud-dev@suse.de
+Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
-Download-URL: https://download.opensuse.org
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Operating System
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 KEG - Image Compositon Tool
 ===========================
 
@@ -26,14 +26,16 @@
 
 |GitHub CI Action|
 
 keg is a command line tool that creates a
 `kiwi <https://github.com/OSInside/kiwi>`_ image description based on
 description snippets in a given GIT repository.
 
+`User documentation <https://documentation.suse.com/appliance/keg-2/html/keg/index.html>`_.
+
 Contributing
 ------------
 
 keg is written in Python, it uses `tox <https://tox.readthedocs.io/en/latest/>`_
 to setup a development environment for the desired Python version. Make
 sure the Python development headers are installed (e.g. `python36-devel`).
 KIWI uses `jing` for detailed error reporting in case schema validation fails.
@@ -41,27 +43,27 @@
 installed on your system.
 
 Currently, there are 5 targets for tox:
 
 - **check**: for code quality and integrity
 - **devel**: for development
 - **doc**: for building man pages
-- **unit_py3_8**: to run unit tests with Python version set to *3.8*
+- **unit_py3_10**: to run unit tests with Python version set to *3.10*
 - **unit_py3_6**: to run unit tests with Python version set to *3.6*
 
 The following procedure describes how to create the development environment:
 
 1. Let tox create the virtual environment(s):
 
    .. code:: bash
 
        $ tox -e devel
 
 2. Activate the virtual environment
-    
+
    .. code:: bash
 
        $ source .tox/3/bin/activate
 
 3. Install requirements inside the virtual environment:
 
    .. code:: bash
@@ -83,9 +85,7 @@
 .. code:: bash
 
    $ deactivate
 
 To resume your work, change into your local Git repository and
 run `source .tox/3/bin/activate` again. Skip step 3 and 4 as
 the requirements are already installed.
-
-
```

