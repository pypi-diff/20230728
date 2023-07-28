# Comparing `tmp/osm_easy_api-1.0.2.tar.gz` & `tmp/osm_easy_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm_easy_api-1.0.2.tar", last modified: Wed Jul 26 11:08:54 2023, max compression
+gzip compressed data, was "osm_easy_api-1.1.0.tar", last modified: Fri Jul 28 18:12:54 2023, max compression
```

## Comparing `osm_easy_api-1.0.2.tar` & `osm_easy_api-1.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 11:08:54.985700 osm_easy_api-1.0.2/
--rw-rw-rw-   0        0        0     3668 2023-07-26 11:02:43.000000 osm_easy_api-1.0.2/CHANGELOG.md
--rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-1.0.2/LICENSE.md
--rw-rw-rw-   0        0        0    45353 2023-07-26 11:08:54.986804 osm_easy_api-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4947 2023-07-24 09:37:44.000000 osm_easy_api-1.0.2/README.md
--rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1197 2023-07-26 11:08:54.996166 osm_easy_api-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:08:54.856004 osm_easy_api-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:08:54.889743 osm_easy_api-1.0.2/src/osm_easy_api/
--rw-rw-rw-   0        0        0      107 2023-07-26 11:00:49.000000 osm_easy_api-1.0.2/src/osm_easy_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:08:54.940925 osm_easy_api-1.0.2/src/osm_easy_api/api/
--rw-rw-rw-   0        0        0     3033 2023-03-07 21:14:41.000000 osm_easy_api-1.0.2/src/osm_easy_api/api/_URLs.py
--rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-1.0.2/src/osm_easy_api/api/__init__.py
--rw-rw-rw-   0        0        0     4368 2023-07-26 10:59:57.000000 osm_easy_api-1.0.2/src/osm_easy_api/api/api.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:08:54.956048 osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/
--rw-rw-rw-   0        0        0      520 2023-03-07 21:14:41.000000 osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/__init__.py
--rw-rw-rw-   0        0        0    14641 2023-06-18 20:57:38.000000 osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/changeset.py
--rw-rw-rw-   0        0        0     4464 2023-06-18 20:57:49.000000 osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/changeset_discussion.py
--rw-rw-rw-   0        0        0    17201 2023-06-18 20:56:56.000000 osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/elements.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 21:14:41.000000 osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/gpx.py
--rw-rw-rw-   0        0        0     5559 2023-06-18 20:56:12.000000 osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/misc.py
--rw-rw-rw-   0        0        0    11507 2023-07-24 09:44:18.000000 osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/notes.py
--rw-rw-rw-   0        0        0     7047 2023-04-02 18:18:25.000000 osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/user.py
--rw-rw-rw-   0        0        0     1025 2023-03-07 21:14:41.000000 osm_easy_api-1.0.2/src/osm_easy_api/api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:08:54.975690 osm_easy_api-1.0.2/src/osm_easy_api/data_classes/
--rw-rw-rw-   0        0        0     8062 2023-06-18 17:27:38.000000 osm_easy_api-1.0.2/src/osm_easy_api/data_classes/OsmChange.py
--rw-rw-rw-   0        0        0      432 2023-03-22 23:03:24.000000 osm_easy_api-1.0.2/src/osm_easy_api/data_classes/__init__.py
--rw-rw-rw-   0        0        0     1785 2023-03-14 14:11:03.000000 osm_easy_api-1.0.2/src/osm_easy_api/data_classes/changeset.py
--rw-rw-rw-   0        0        0     1144 2023-06-10 21:48:54.000000 osm_easy_api-1.0.2/src/osm_easy_api/data_classes/node.py
--rw-rw-rw-   0        0        0     4022 2023-03-22 21:29:55.000000 osm_easy_api-1.0.2/src/osm_easy_api/data_classes/note.py
--rw-rw-rw-   0        0        0     2635 2023-05-03 15:23:00.000000 osm_easy_api-1.0.2/src/osm_easy_api/data_classes/osm_object_primitive.py
--rw-rw-rw-   0        0        0     2786 2023-06-10 21:42:40.000000 osm_easy_api-1.0.2/src/osm_easy_api/data_classes/relation.py
--rw-rw-rw-   0        0        0     1403 2023-03-22 23:13:07.000000 osm_easy_api-1.0.2/src/osm_easy_api/data_classes/tags.py
--rw-rw-rw-   0        0        0     2099 2023-03-22 20:09:45.000000 osm_easy_api-1.0.2/src/osm_easy_api/data_classes/user.py
--rw-rw-rw-   0        0        0     1725 2023-06-10 21:48:37.000000 osm_easy_api-1.0.2/src/osm_easy_api/data_classes/way.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:08:54.980637 osm_easy_api-1.0.2/src/osm_easy_api/diff/
--rw-rw-rw-   0        0        0      111 2023-03-07 21:14:41.000000 osm_easy_api-1.0.2/src/osm_easy_api/diff/__init__.py
--rw-rw-rw-   0        0        0     6164 2023-04-01 19:34:36.000000 osm_easy_api-1.0.2/src/osm_easy_api/diff/diff.py
--rw-rw-rw-   0        0        0     9075 2023-03-07 21:24:24.000000 osm_easy_api-1.0.2/src/osm_easy_api/diff/diff_parser.py
--rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-1.0.2/src/osm_easy_api/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-26 11:08:54.984352 osm_easy_api-1.0.2/src/osm_easy_api/utils/
--rw-rw-rw-   0        0        0       82 2023-03-07 21:14:41.000000 osm_easy_api-1.0.2/src/osm_easy_api/utils/__init__.py
--rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-1.0.2/src/osm_easy_api/utils/join_url.py
--rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-1.0.2/src/osm_easy_api/utils/write_gzip_to_file.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:08:54.932623 osm_easy_api-1.0.2/src/osm_easy_api.egg-info/
--rw-rw-rw-   0        0        0    45353 2023-07-26 11:08:54.000000 osm_easy_api-1.0.2/src/osm_easy_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-07-26 11:08:54.000000 osm_easy_api-1.0.2/src/osm_easy_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 11:08:54.000000 osm_easy_api-1.0.2/src/osm_easy_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-24 09:45:20.000000 osm_easy_api-1.0.2/src/osm_easy_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2023-07-26 11:08:54.000000 osm_easy_api-1.0.2/src/osm_easy_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-26 11:08:54.000000 osm_easy_api-1.0.2/src/osm_easy_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 18:12:54.039069 osm_easy_api-1.1.0/
+-rw-rw-rw-   0        0        0     3874 2023-07-28 18:02:48.000000 osm_easy_api-1.1.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0    45559 2023-07-28 18:12:54.040069 osm_easy_api-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4947 2023-07-24 09:37:44.000000 osm_easy_api-1.1.0/README.md
+-rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1197 2023-07-28 18:12:54.064991 osm_easy_api-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:12:53.906185 osm_easy_api-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 18:12:53.936883 osm_easy_api-1.1.0/src/osm_easy_api/
+-rw-rw-rw-   0        0        0      107 2023-07-28 18:03:22.000000 osm_easy_api-1.1.0/src/osm_easy_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:12:53.984165 osm_easy_api-1.1.0/src/osm_easy_api/api/
+-rw-rw-rw-   0        0        0     3033 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/_URLs.py
+-rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/__init__.py
+-rw-rw-rw-   0        0        0     4368 2023-07-28 17:51:03.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/api.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:12:54.000993 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/
+-rw-rw-rw-   0        0        0      520 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0    14856 2023-07-28 17:56:51.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/changeset.py
+-rw-rw-rw-   0        0        0     4464 2023-06-18 20:57:49.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/changeset_discussion.py
+-rw-rw-rw-   0        0        0    17201 2023-06-18 20:56:56.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/elements.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/gpx.py
+-rw-rw-rw-   0        0        0     5559 2023-06-18 20:56:12.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/misc.py
+-rw-rw-rw-   0        0        0    11507 2023-07-24 09:44:18.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/notes.py
+-rw-rw-rw-   0        0        0     7047 2023-04-02 18:18:25.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/user.py
+-rw-rw-rw-   0        0        0     1025 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:12:54.024094 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/
+-rw-rw-rw-   0        0        0     8062 2023-06-18 17:27:38.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/OsmChange.py
+-rw-rw-rw-   0        0        0      432 2023-03-22 23:03:24.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/__init__.py
+-rw-rw-rw-   0        0        0     1785 2023-03-14 14:11:03.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/changeset.py
+-rw-rw-rw-   0        0        0     1144 2023-06-10 21:48:54.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/node.py
+-rw-rw-rw-   0        0        0     4022 2023-03-22 21:29:55.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/note.py
+-rw-rw-rw-   0        0        0     2635 2023-05-03 15:23:00.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/osm_object_primitive.py
+-rw-rw-rw-   0        0        0     2786 2023-06-10 21:42:40.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/relation.py
+-rw-rw-rw-   0        0        0     1403 2023-03-22 23:13:07.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/tags.py
+-rw-rw-rw-   0        0        0     2099 2023-03-22 20:09:45.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/user.py
+-rw-rw-rw-   0        0        0     1725 2023-06-10 21:48:37.000000 osm_easy_api-1.1.0/src/osm_easy_api/data_classes/way.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:12:54.030530 osm_easy_api-1.1.0/src/osm_easy_api/diff/
+-rw-rw-rw-   0        0        0      111 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/diff/__init__.py
+-rw-rw-rw-   0        0        0     6164 2023-04-01 19:34:36.000000 osm_easy_api-1.1.0/src/osm_easy_api/diff/diff.py
+-rw-rw-rw-   0        0        0     9075 2023-03-07 21:24:24.000000 osm_easy_api-1.1.0/src/osm_easy_api/diff/diff_parser.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-28 18:12:54.037071 osm_easy_api-1.1.0/src/osm_easy_api/utils/
+-rw-rw-rw-   0        0        0       82 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/utils/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/utils/join_url.py
+-rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-1.1.0/src/osm_easy_api/utils/write_gzip_to_file.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:12:53.975348 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/
+-rw-rw-rw-   0        0        0    45559 2023-07-28 18:12:53.000000 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-07-28 18:12:53.000000 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 18:12:53.000000 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 09:45:20.000000 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-07-28 18:12:53.000000 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-28 18:12:53.000000 osm_easy_api-1.1.0/src/osm_easy_api.egg-info/top_level.txt
```

### Comparing `osm_easy_api-1.0.2/CHANGELOG.md` & `osm_easy_api-1.1.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.1.0]
+### Added
+- `limit` parameter for `api.changeset.get_query()` endpoint.
+
+### Fixed
+- Corrected character when adding parameters in endpoint `api.changeset.get_query()` (from `;` to `&`).
+
 ## [1.0.2]
 ### Fixed
 - Auth problems in API when using characters unsupported by latin-1 codec.
 
 ## [1.0.1]
 ### Fixed
 - `api.notes.create()` created only anonymous notes.
```

### Comparing `osm_easy_api-1.0.2/LICENSE.md` & `osm_easy_api-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/PKG-INFO` & `osm_easy_api-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm_easy_api
-Version: 1.0.2
+Version: 1.1.0
 Summary: Python package for parsing osm diffs and communicating with the osm api.
 Home-page: https://github.com/docentYT/osm_easy_api
 License: GPLv3
 Keywords: openstreetmap,osm,api,wrapper,diff
 Platform: unix
 Platform: linux
 Platform: osx
@@ -171,14 +171,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.1.0]
+### Added
+- `limit` parameter for `api.changeset.get_query()` endpoint.
+
+### Fixed
+- Corrected character when adding parameters in endpoint `api.changeset.get_query()` (from `;` to `&`).
+
 ## [1.0.2]
 ### Fixed
 - Auth problems in API when using characters unsupported by latin-1 codec.
 
 ## [1.0.1]
 ### Fixed
 - `api.notes.create()` created only anonymous notes.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osm_easy_api Version: 1.0.2 Summary: Python package
+Metadata-Version: 2.1 Name: osm_easy_api Version: 1.1.0 Summary: Python package
 for parsing osm diffs and communicating with the osm api. Home-page: https://
 github.com/docentYT/osm_easy_api License: GPLv3 Keywords:
 openstreetmap,osm,api,wrapper,diff Platform: unix Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Topic :: Scientific/Engineering :: GIS Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
@@ -65,45 +65,48 @@
 d.get(generator=False) deleted_nodes = osmChange.get(Node, Action.DELETE) for
 node in deleted_nodes: print(node.id) ``` but it can consume large amounts of
 ram and use of this method is not recommended for large diff's. # Tests You
 will need to install `test-requirements.txt`. You can use tox. To run tests
 manually use `python -m unittest discover`. # Changelog All notable changes to
 this project will be documented in this file. The format is based on [Keep a
 Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to
-[Semantic Versioning](https://semver.org/spec/v2.0.0.html). ## [1.0.2] ###
-Fixed - Auth problems in API when using characters unsupported by latin-
-1 codec. ## [1.0.1] ### Fixed - `api.notes.create()` created only anonymous
-notes. ## [1.0.0] ### Added - `to_xml()` method in `OsmChange`. - `upload()`
-method in `changeset` `endpoint` has new optional arguments. - Test for `to_xml
-()` method in `OsmChange`. - `# pragma: no cover` for unexpected api errors
-(Those that are not in the specification on the wiki). ### Changed - Private
-`_to_xml()` method in `OsmChange` is now static. ## [0.4.2] ### Changed - Order
-of elements in xml generated by `Way._to_xml()`. First tags, then nodes. ###
-Fixed - `Relation._to_xml()` was returning an xml without osm tags. - Deleted
-disused variable in `Node._to_xml()`. - Fixed incorrect relation parsing of
-data recived by `full` endpoint. ## [0.4.1] ### Changed - Updated `requests`
-from `2.28.1` to `2.31.0`. ## [0.4.0] ### Added - `to_dict()` method and
-`from_dict()` class method to `Note`. - `to_dict()` method and `from_dict()`
-class method to `Comment`. - `to_dict()` method and `from_dict()` class method
-to `User`. - Documentation about `Meta` and `Action` class. - Assert error
-(with information to report it on github) when api returns an error code not
-described on the wiki. - `to_dict()` method and `from_dict()` class method to `
-(relation) Member`. ### Fixed - `Note` can now be imported from package. -
-`Comment` can now be imported from package. - `User` can now be imported from
-package. - `Member` can now be imported from package. - Pdoc command in
-`README.md`. - `Relation.to_dict()` method now recursively serialises members.
-- `Way.to_dict()` method now recursively serialises nodes. ### Changed -
-Changed imports in `Relation.py` to use importing through a module rather than
-directly from a file. - Added `sample_dataclasses.py` file in tests fixtures to
-reduce code duplication. - Changed function name and deleted unnecessary
-argument in `append_elements_to_master_element()` nested inside private method
-`_to_xml()` in `OsmChange`. ## [0.3.0] - 2023-03-14 ### Added - `to_dict()`
-method and `from_dict()` class method to Changeset. [#7](https://github.com/
-docentYT/osm_easy_api/issues/7) - Ability to set user_agent in `Diff` and `Api`
-class. [#5](https://github.com/docentYT/osm_easy_api/issues/5) -
+[Semantic Versioning](https://semver.org/spec/v2.0.0.html). ## [1.1.0] ###
+Added - `limit` parameter for `api.changeset.get_query()` endpoint. ### Fixed -
+Corrected character when adding parameters in endpoint `api.changeset.get_query
+()` (from `;` to `&`). ## [1.0.2] ### Fixed - Auth problems in API when using
+characters unsupported by latin-1 codec. ## [1.0.1] ### Fixed -
+`api.notes.create()` created only anonymous notes. ## [1.0.0] ### Added -
+`to_xml()` method in `OsmChange`. - `upload()` method in `changeset` `endpoint`
+has new optional arguments. - Test for `to_xml()` method in `OsmChange`. - `#
+pragma: no cover` for unexpected api errors (Those that are not in the
+specification on the wiki). ### Changed - Private `_to_xml()` method in
+`OsmChange` is now static. ## [0.4.2] ### Changed - Order of elements in xml
+generated by `Way._to_xml()`. First tags, then nodes. ### Fixed -
+`Relation._to_xml()` was returning an xml without osm tags. - Deleted disused
+variable in `Node._to_xml()`. - Fixed incorrect relation parsing of data
+recived by `full` endpoint. ## [0.4.1] ### Changed - Updated `requests` from
+`2.28.1` to `2.31.0`. ## [0.4.0] ### Added - `to_dict()` method and `from_dict
+()` class method to `Note`. - `to_dict()` method and `from_dict()` class method
+to `Comment`. - `to_dict()` method and `from_dict()` class method to `User`. -
+Documentation about `Meta` and `Action` class. - Assert error (with information
+to report it on github) when api returns an error code not described on the
+wiki. - `to_dict()` method and `from_dict()` class method to `(relation)
+Member`. ### Fixed - `Note` can now be imported from package. - `Comment` can
+now be imported from package. - `User` can now be imported from package. -
+`Member` can now be imported from package. - Pdoc command in `README.md`. -
+`Relation.to_dict()` method now recursively serialises members. - `Way.to_dict
+()` method now recursively serialises nodes. ### Changed - Changed imports in
+`Relation.py` to use importing through a module rather than directly from a
+file. - Added `sample_dataclasses.py` file in tests fixtures to reduce code
+duplication. - Changed function name and deleted unnecessary argument in
+`append_elements_to_master_element()` nested inside private method `_to_xml()`
+in `OsmChange`. ## [0.3.0] - 2023-03-14 ### Added - `to_dict()` method and
+`from_dict()` class method to Changeset. [#7](https://github.com/docentYT/
+osm_easy_api/issues/7) - Ability to set user_agent in `Diff` and `Api` class.
+[#5](https://github.com/docentYT/osm_easy_api/issues/5) -
 `osm_object_primitive` `from_dict()` class method now raises `ValueError` if
 the `type` key is not found. ### Changed - `Changeset` is now exported from
 data_classes module. - More tests. ## [0.2.0] - 2023-03-07 ### Added - `to_dict
 ()` method and `from_dict()` class method to `osm_object_primitive`. (An object
 that is inherited by a `Node`, `Way`, `Relation`). [#3](https://github.com/
 docentYT/osm_easy_api/issues/3) - Support for historical anonymous edits and
 edits made by deleted accounts. [#4](https://github.com/docentYT/osm_easy_api/
```

### Comparing `osm_easy_api-1.0.2/README.md` & `osm_easy_api-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/setup.cfg` & `osm_easy_api-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/api/_URLs.py` & `osm_easy_api-1.1.0/src/osm_easy_api/api/_URLs.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/api/api.py` & `osm_easy_api-1.1.0/src/osm_easy_api/api/api.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/__init__.py` & `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/changeset.py` & `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/changeset.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,16 @@
 
         return self._xml_to_changeset(generator, include_discussion)[0] # type: ignore
 
     def get_query(self, left: float | None = None, bottom: float | None = None, right: float | None = None, top: float | None = None,
     user_id: str | None = None, display_name: str | None = None,
     time_one: str | None = None, time_two: str | None = None,
     open: bool = False, closed: bool = False,
-    changesets_id: list[int] | None = None
+    changesets_id: list[int] | None = None,
+    limit: int = 100
     ) -> list[Changeset]:
         """Get changesets with given criteria.
 
         Args:
             left (float | None, optional): Left side of bounding box (min_lon / west) Use left, bottom, right, top together. Defaults to None.
             bottom (float | None, optional): Bottom side of bounding box (min_lat / south). Use left, bottom, right, top together. Defaults to None.
             right (float | None, optional): Right side of bounding box (max_lon / east). Use left, bottom, right, top together. Defaults to None.
@@ -134,35 +135,38 @@
             user_id (str | None, optional): User id. Defaults to None.
             display_name (str | None, optional): User display name. Defaults to None.
             time_one (str | None, optional): Find changesets closed after time_one. Defaults to None.
             time_two (str | None, optional): Requires time_one. Find changesets created before time_two. (Range time_one - time_two). Defaults to None.
             open (bool, optional): Find only open changesets. Defaults to False.
             closed (bool, optional): Find only closed changesets. Defaults to False.
             changesets_id (list[int] | None, optional): List of ids to search for. Defaults to None.
+            limit (int, optional): Specifies the maximum number of changesets returned. Must be between 1 and 100. Defaults to 100.
 
         Raises:
             ValueError: Invalid arguments.
             exceptions.IdNotFoundError: user_id or display_name not found.
 
         Returns:
             list[Changeset]: List of Changeset objects.
         """
         param = "?"
-        if (left or bottom or right or top): param += f"bbox={left},{bottom},{right},{top};"
-        if (user_id): param += f"user={user_id};"
-        if (display_name): param += f"display_name={display_name};"
-        if (time_one): param += f"time={time_one};"
-        if (time_two): param += f",{time_two};"
-        if (open): param += f"open={open};"
-        if (closed): param += f"closed={closed};"
+        if (left or bottom or right or top): param += f"bbox={left},{bottom},{right},{top}&"
+        if (user_id): param += f"user={user_id}&"
+        if (display_name): param += f"display_name={display_name}&"
+        if (time_one): param += f"time={time_one}&"
+        if (time_two): param += f",{time_two}&"
+        if (open): param += f"open={open}&"
+        if (closed): param += f"closed={closed}&"
         if (changesets_id):
             param += f"changesets={changesets_id[0]}"
             changesets_id.pop(0)
             for id in changesets_id:
                 param += f",{id}"
+            param += "&"
+        param+=f"limit={limit}"
 
         status_code, generator = self.outer._get_generator(
             url=join_url(self.outer._url.changeset["get_query"], param),
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
 
         match status_code:
```

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/changeset_discussion.py` & `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/changeset_discussion.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/elements.py` & `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/elements.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/gpx.py` & `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/gpx.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/misc.py` & `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/notes.py` & `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/notes.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/api/endpoints/user.py` & `osm_easy_api-1.1.0/src/osm_easy_api/api/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/api/exceptions.py` & `osm_easy_api-1.1.0/src/osm_easy_api/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/data_classes/OsmChange.py` & `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/OsmChange.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/data_classes/changeset.py` & `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/changeset.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/data_classes/node.py` & `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/node.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/data_classes/note.py` & `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/note.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/data_classes/osm_object_primitive.py` & `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/osm_object_primitive.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/data_classes/relation.py` & `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/relation.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/data_classes/tags.py` & `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/tags.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/data_classes/user.py` & `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/user.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/data_classes/way.py` & `osm_easy_api-1.1.0/src/osm_easy_api/data_classes/way.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/diff/diff.py` & `osm_easy_api-1.1.0/src/osm_easy_api/diff/diff.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api/diff/diff_parser.py` & `osm_easy_api-1.1.0/src/osm_easy_api/diff/diff_parser.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api.egg-info/PKG-INFO` & `osm_easy_api-1.1.0/src/osm_easy_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-easy-api
-Version: 1.0.2
+Version: 1.1.0
 Summary: Python package for parsing osm diffs and communicating with the osm api.
 Home-page: https://github.com/docentYT/osm_easy_api
 License: GPLv3
 Keywords: openstreetmap,osm,api,wrapper,diff
 Platform: unix
 Platform: linux
 Platform: osx
@@ -171,14 +171,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.1.0]
+### Added
+- `limit` parameter for `api.changeset.get_query()` endpoint.
+
+### Fixed
+- Corrected character when adding parameters in endpoint `api.changeset.get_query()` (from `;` to `&`).
+
 ## [1.0.2]
 ### Fixed
 - Auth problems in API when using characters unsupported by latin-1 codec.
 
 ## [1.0.1]
 ### Fixed
 - `api.notes.create()` created only anonymous notes.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osm-easy-api Version: 1.0.2 Summary: Python package
+Metadata-Version: 2.1 Name: osm-easy-api Version: 1.1.0 Summary: Python package
 for parsing osm diffs and communicating with the osm api. Home-page: https://
 github.com/docentYT/osm_easy_api License: GPLv3 Keywords:
 openstreetmap,osm,api,wrapper,diff Platform: unix Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Topic :: Scientific/Engineering :: GIS Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
@@ -65,45 +65,48 @@
 d.get(generator=False) deleted_nodes = osmChange.get(Node, Action.DELETE) for
 node in deleted_nodes: print(node.id) ``` but it can consume large amounts of
 ram and use of this method is not recommended for large diff's. # Tests You
 will need to install `test-requirements.txt`. You can use tox. To run tests
 manually use `python -m unittest discover`. # Changelog All notable changes to
 this project will be documented in this file. The format is based on [Keep a
 Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to
-[Semantic Versioning](https://semver.org/spec/v2.0.0.html). ## [1.0.2] ###
-Fixed - Auth problems in API when using characters unsupported by latin-
-1 codec. ## [1.0.1] ### Fixed - `api.notes.create()` created only anonymous
-notes. ## [1.0.0] ### Added - `to_xml()` method in `OsmChange`. - `upload()`
-method in `changeset` `endpoint` has new optional arguments. - Test for `to_xml
-()` method in `OsmChange`. - `# pragma: no cover` for unexpected api errors
-(Those that are not in the specification on the wiki). ### Changed - Private
-`_to_xml()` method in `OsmChange` is now static. ## [0.4.2] ### Changed - Order
-of elements in xml generated by `Way._to_xml()`. First tags, then nodes. ###
-Fixed - `Relation._to_xml()` was returning an xml without osm tags. - Deleted
-disused variable in `Node._to_xml()`. - Fixed incorrect relation parsing of
-data recived by `full` endpoint. ## [0.4.1] ### Changed - Updated `requests`
-from `2.28.1` to `2.31.0`. ## [0.4.0] ### Added - `to_dict()` method and
-`from_dict()` class method to `Note`. - `to_dict()` method and `from_dict()`
-class method to `Comment`. - `to_dict()` method and `from_dict()` class method
-to `User`. - Documentation about `Meta` and `Action` class. - Assert error
-(with information to report it on github) when api returns an error code not
-described on the wiki. - `to_dict()` method and `from_dict()` class method to `
-(relation) Member`. ### Fixed - `Note` can now be imported from package. -
-`Comment` can now be imported from package. - `User` can now be imported from
-package. - `Member` can now be imported from package. - Pdoc command in
-`README.md`. - `Relation.to_dict()` method now recursively serialises members.
-- `Way.to_dict()` method now recursively serialises nodes. ### Changed -
-Changed imports in `Relation.py` to use importing through a module rather than
-directly from a file. - Added `sample_dataclasses.py` file in tests fixtures to
-reduce code duplication. - Changed function name and deleted unnecessary
-argument in `append_elements_to_master_element()` nested inside private method
-`_to_xml()` in `OsmChange`. ## [0.3.0] - 2023-03-14 ### Added - `to_dict()`
-method and `from_dict()` class method to Changeset. [#7](https://github.com/
-docentYT/osm_easy_api/issues/7) - Ability to set user_agent in `Diff` and `Api`
-class. [#5](https://github.com/docentYT/osm_easy_api/issues/5) -
+[Semantic Versioning](https://semver.org/spec/v2.0.0.html). ## [1.1.0] ###
+Added - `limit` parameter for `api.changeset.get_query()` endpoint. ### Fixed -
+Corrected character when adding parameters in endpoint `api.changeset.get_query
+()` (from `;` to `&`). ## [1.0.2] ### Fixed - Auth problems in API when using
+characters unsupported by latin-1 codec. ## [1.0.1] ### Fixed -
+`api.notes.create()` created only anonymous notes. ## [1.0.0] ### Added -
+`to_xml()` method in `OsmChange`. - `upload()` method in `changeset` `endpoint`
+has new optional arguments. - Test for `to_xml()` method in `OsmChange`. - `#
+pragma: no cover` for unexpected api errors (Those that are not in the
+specification on the wiki). ### Changed - Private `_to_xml()` method in
+`OsmChange` is now static. ## [0.4.2] ### Changed - Order of elements in xml
+generated by `Way._to_xml()`. First tags, then nodes. ### Fixed -
+`Relation._to_xml()` was returning an xml without osm tags. - Deleted disused
+variable in `Node._to_xml()`. - Fixed incorrect relation parsing of data
+recived by `full` endpoint. ## [0.4.1] ### Changed - Updated `requests` from
+`2.28.1` to `2.31.0`. ## [0.4.0] ### Added - `to_dict()` method and `from_dict
+()` class method to `Note`. - `to_dict()` method and `from_dict()` class method
+to `Comment`. - `to_dict()` method and `from_dict()` class method to `User`. -
+Documentation about `Meta` and `Action` class. - Assert error (with information
+to report it on github) when api returns an error code not described on the
+wiki. - `to_dict()` method and `from_dict()` class method to `(relation)
+Member`. ### Fixed - `Note` can now be imported from package. - `Comment` can
+now be imported from package. - `User` can now be imported from package. -
+`Member` can now be imported from package. - Pdoc command in `README.md`. -
+`Relation.to_dict()` method now recursively serialises members. - `Way.to_dict
+()` method now recursively serialises nodes. ### Changed - Changed imports in
+`Relation.py` to use importing through a module rather than directly from a
+file. - Added `sample_dataclasses.py` file in tests fixtures to reduce code
+duplication. - Changed function name and deleted unnecessary argument in
+`append_elements_to_master_element()` nested inside private method `_to_xml()`
+in `OsmChange`. ## [0.3.0] - 2023-03-14 ### Added - `to_dict()` method and
+`from_dict()` class method to Changeset. [#7](https://github.com/docentYT/
+osm_easy_api/issues/7) - Ability to set user_agent in `Diff` and `Api` class.
+[#5](https://github.com/docentYT/osm_easy_api/issues/5) -
 `osm_object_primitive` `from_dict()` class method now raises `ValueError` if
 the `type` key is not found. ### Changed - `Changeset` is now exported from
 data_classes module. - More tests. ## [0.2.0] - 2023-03-07 ### Added - `to_dict
 ()` method and `from_dict()` class method to `osm_object_primitive`. (An object
 that is inherited by a `Node`, `Way`, `Relation`). [#3](https://github.com/
 docentYT/osm_easy_api/issues/3) - Support for historical anonymous edits and
 edits made by deleted accounts. [#4](https://github.com/docentYT/osm_easy_api/
```

### Comparing `osm_easy_api-1.0.2/src/osm_easy_api.egg-info/SOURCES.txt` & `osm_easy_api-1.1.0/src/osm_easy_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

