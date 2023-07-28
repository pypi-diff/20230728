# Comparing `tmp/django-versionator-0.0.1b0.tar.gz` & `tmp/django-versionator-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-versionator-0.0.1b0.tar", last modified: Mon Mar 13 17:38:01 2023, max compression
+gzip compressed data, was "django-versionator-0.2.0b0.tar", last modified: Fri Jul 28 19:08:07 2023, max compression
```

## Comparing `django-versionator-0.0.1b0.tar` & `django-versionator-0.2.0b0.tar`

### file list

```diff
@@ -1,17 +1,56 @@
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-03-13 17:38:01.606702 django-versionator-0.0.1b0/
--rw-r--r--   0 acl        (501) staff       (20)      369 2023-03-13 17:38:01.606536 django-versionator-0.0.1b0/PKG-INFO
--rw-r--r--   0 acl        (501) staff       (20)       38 2023-03-13 16:36:16.000000 django-versionator-0.0.1b0/README.md
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-03-13 17:38:01.605623 django-versionator-0.0.1b0/django_versionator.egg-info/
--rw-r--r--   0 acl        (501) staff       (20)      369 2023-03-13 17:38:01.000000 django-versionator-0.0.1b0/django_versionator.egg-info/PKG-INFO
--rw-r--r--   0 acl        (501) staff       (20)      316 2023-03-13 17:38:01.000000 django-versionator-0.0.1b0/django_versionator.egg-info/SOURCES.txt
--rw-r--r--   0 acl        (501) staff       (20)        1 2023-03-13 17:38:01.000000 django-versionator-0.0.1b0/django_versionator.egg-info/dependency_links.txt
--rw-r--r--   0 acl        (501) staff       (20)       12 2023-03-13 17:38:01.000000 django-versionator-0.0.1b0/django_versionator.egg-info/top_level.txt
--rw-r--r--   0 acl        (501) staff       (20)       38 2023-03-13 17:38:01.606752 django-versionator-0.0.1b0/setup.cfg
--rw-r--r--   0 acl        (501) staff       (20)      867 2023-03-13 16:35:30.000000 django-versionator-0.0.1b0/setup.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-03-13 17:38:01.605909 django-versionator-0.0.1b0/tests/
--rw-r--r--   0 acl        (501) staff       (20)      652 2023-03-13 15:50:58.000000 django-versionator-0.0.1b0/tests/test_edited_by_versioning.py
--rw-r--r--   0 acl        (501) staff       (20)     6195 2023-03-13 15:50:58.000000 django-versionator-0.0.1b0/tests/test_versioning.py
-drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-03-13 17:38:01.606350 django-versionator-0.0.1b0/versionator/
--rw-r--r--   0 acl        (501) staff       (20)       64 2023-03-13 14:43:23.000000 django-versionator-0.0.1b0/versionator/__init__.py
--rw-r--r--   0 acl        (501) staff       (20)    11352 2023-03-13 17:24:33.000000 django-versionator-0.0.1b0/versionator/core.py
--rw-r--r--   0 acl        (501) staff       (20)     1158 2023-03-13 14:43:23.000000 django-versionator-0.0.1b0/versionator/middleware.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.606867 django-versionator-0.2.0b0/
+-rw-r--r--   0 acl        (501) staff       (20)      395 2023-07-28 19:08:07.606681 django-versionator-0.2.0b0/PKG-INFO
+-rw-r--r--   0 acl        (501) staff       (20)       38 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/README.md
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.599297 django-versionator-0.2.0b0/django_versionator.egg-info/
+-rw-r--r--   0 acl        (501) staff       (20)      395 2023-07-28 19:08:07.000000 django-versionator-0.2.0b0/django_versionator.egg-info/PKG-INFO
+-rw-r--r--   0 acl        (501) staff       (20)     1898 2023-07-28 19:08:07.000000 django-versionator-0.2.0b0/django_versionator.egg-info/SOURCES.txt
+-rw-r--r--   0 acl        (501) staff       (20)        1 2023-07-28 19:08:07.000000 django-versionator-0.2.0b0/django_versionator.egg-info/dependency_links.txt
+-rw-r--r--   0 acl        (501) staff       (20)      108 2023-07-28 19:08:07.000000 django-versionator-0.2.0b0/django_versionator.egg-info/requires.txt
+-rw-r--r--   0 acl        (501) staff       (20)       12 2023-07-28 19:08:07.000000 django-versionator-0.2.0b0/django_versionator.egg-info/top_level.txt
+-rw-r--r--   0 acl        (501) staff       (20)       38 2023-07-28 19:08:07.606927 django-versionator-0.2.0b0/setup.cfg
+-rw-r--r--   0 acl        (501) staff       (20)     1161 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/setup.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.600084 django-versionator-0.2.0b0/tests/
+-rw-r--r--   0 acl        (501) staff       (20)     4030 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/tests/test_changelog.py
+-rw-r--r--   0 acl        (501) staff       (20)      652 2023-03-13 15:50:58.000000 django-versionator-0.2.0b0/tests/test_edited_by_versioning.py
+-rw-r--r--   0 acl        (501) staff       (20)     6195 2023-03-13 15:50:58.000000 django-versionator-0.2.0b0/tests/test_versioning.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.601189 django-versionator-0.2.0b0/versionator/
+-rw-r--r--   0 acl        (501) staff       (20)       64 2023-03-13 14:43:23.000000 django-versionator-0.2.0b0/versionator/__init__.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.602550 django-versionator-0.2.0b0/versionator/changelog/
+-rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/__init__.py
+-rw-r--r--   0 acl        (501) staff       (20)     2433 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/arbitrary_version_pair_fetcher.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.602826 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/
+-rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/__init__.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.604085 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/
+-rw-r--r--   0 acl        (501) staff       (20)      236 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/__init__.py
+-rw-r--r--   0 acl        (501) staff       (20)     3720 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/changelog_entry.py
+-rw-r--r--   0 acl        (501) staff       (20)     1949 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/changelog_entry_field_entry.py
+-rw-r--r--   0 acl        (501) staff       (20)     1162 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/changelog_page.py
+-rw-r--r--   0 acl        (501) staff       (20)    10146 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/diff.py
+-rw-r--r--   0 acl        (501) staff       (20)      753 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/version.py
+-rw-r--r--   0 acl        (501) staff       (20)     2801 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/types/version_comparison_entry.py
+-rw-r--r--   0 acl        (501) staff       (20)     3836 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/changelog_graphql/util.py
+-rw-r--r--   0 acl        (501) staff       (20)     8109 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/consecutive_versions_fetcher.py
+-rw-r--r--   0 acl        (501) staff       (20)     3279 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/diff_utils.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.605329 django-versionator-0.2.0b0/versionator/changelog/graphql/
+-rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/__init__.py
+-rw-r--r--   0 acl        (501) staff       (20)     2364 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/dataloader.py
+-rw-r--r--   0 acl        (501) staff       (20)     1758 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/graphiql_view_base.py
+-rw-r--r--   0 acl        (501) staff       (20)      180 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/graphql_context.py
+-rw-r--r--   0 acl        (501) staff       (20)     2741 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/internal_query_executor_base.py
+-rw-r--r--   0 acl        (501) staff       (20)     1235 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/middleware.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.605649 django-versionator-0.2.0b0/versionator/changelog/graphql/testing/
+-rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/testing/__init__.py
+-rw-r--r--   0 acl        (501) staff       (20)      683 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/testing/fixtures.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.606090 django-versionator-0.2.0b0/versionator/changelog/graphql/types/
+-rw-r--r--   0 acl        (501) staff       (20)        0 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/types/__init__.py
+-rw-r--r--   0 acl        (501) staff       (20)      634 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/types/has_non_serializable_record_mixin.py
+-rw-r--r--   0 acl        (501) staff       (20)      966 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/types/version.py
+-rw-r--r--   0 acl        (501) staff       (20)     2535 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/graphql/utils.py
+-rw-r--r--   0 acl        (501) staff       (20)     2850 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/simple_changelog.py
+-rw-r--r--   0 acl        (501) staff       (20)      490 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/util.py
+drwxr-xr-x   0 acl        (501) staff       (20)        0 2023-07-28 19:08:07.606435 django-versionator-0.2.0b0/versionator/changelog/views/
+-rw-r--r--   0 acl        (501) staff       (20)       59 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/views/__init__.py
+-rw-r--r--   0 acl        (501) staff       (20)     2060 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/changelog/views/abstract_changelog_view.py
+-rw-r--r--   0 acl        (501) staff       (20)    11348 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/core.py
+-rw-r--r--   0 acl        (501) staff       (20)     1158 2023-03-13 14:43:23.000000 django-versionator-0.2.0b0/versionator/middleware.py
+-rw-r--r--   0 acl        (501) staff       (20)      343 2023-07-28 19:07:13.000000 django-versionator-0.2.0b0/versionator/utils.py
```

### Comparing `django-versionator-0.0.1b0/setup.py` & `django-versionator-0.2.0b0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-versionator",
-    version="0.0.1b",
+    version="0.2.0b",
     author="AlexCLeduc",
     # author_email="author@example.com",
     # description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AlexCleduc/django-versionator",
     packages=[
-        # find_packages() also includes extraneous stuff, like testing and django_sample
+        # find_packages() also includes extraneous stuff, like testing and sample_app
         package
         for package in setuptools.find_packages()
         if package.startswith("versionator")
     ],
     install_requires=[],
+    # to install these subdeps, use pip install django-versionator[changelog]
+    extras_require={
+        "changelog": [
+            "pleasant-promises>=1.1",
+            "graphene>=3.1.1, <4",
+            "graphene-django>=3, <4",
+            "graphql-core-promise>=3.2.3,<4",
+        ],
+    },
     tests_require=["django"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `django-versionator-0.0.1b0/tests/test_edited_by_versioning.py` & `django-versionator-0.2.0b0/tests/test_edited_by_versioning.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.0.1b0/tests/test_versioning.py` & `django-versionator-0.2.0b0/tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `django-versionator-0.0.1b0/versionator/core.py` & `django-versionator-0.2.0b0/versionator/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 class HistoryQueryset(QuerySet):
     def with_previous_version_id(self):
         # we need a non-filtered QS clone of the same type
         another_qs = HistoryQueryset(self.model, self._db)
         prev_version_id_subquery = Subquery(
             another_qs.filter(
                 eternal_id=OuterRef("eternal_id"),
-                business_date__lt=OuterRef("timestamp"),
+                timestamp__lt=OuterRef("timestamp"),
             )
             .order_by("-timestamp")
             .values("id")[:1]
         )
         return self.annotate(previous_version_id=prev_version_id_subquery)
 
     def with_most_recent_version_id(self):
```

### Comparing `django-versionator-0.0.1b0/versionator/middleware.py` & `django-versionator-0.2.0b0/versionator/middleware.py`

 * *Files identical despite different names*

