# Comparing `tmp/mypy-boto3-health-1.28.12.tar.gz` & `tmp/mypy-boto3-health-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-health-1.28.12.tar", last modified: Thu Jul 27 05:34:45 2023, max compression
+gzip compressed data, was "mypy-boto3-health-1.28.15.tar", last modified: Fri Jul 28 20:42:53 2023, max compression
```

## Comparing `mypy-boto3-health-1.28.12.tar` & `mypy-boto3-health-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.536496 mypy-boto3-health-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:16.000000 mypy-boto3-health-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-27 05:34:45.532497 mypy-boto3-health-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-07-27 05:23:16.000000 mypy-boto3-health-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.528497 mypy-boto3-health-1.28.12/mypy_boto3_health/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-27 05:23:16.000000 mypy-boto3-health-1.28.12/mypy_boto3_health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-27 05:23:16.000000 mypy-boto3-health-1.28.12/mypy_boto3_health/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:23:16.000000 mypy-boto3-health-1.28.12/mypy_boto3_health/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-07-27 05:23:16.000000 mypy-boto3-health-1.28.12/mypy_boto3_health/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-07-27 05:23:16.000000 mypy-boto3-health-1.28.12/mypy_boto3_health/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-07-27 05:23:17.000000 mypy-boto3-health-1.28.12/mypy_boto3_health/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-07-27 05:23:17.000000 mypy-boto3-health-1.28.12/mypy_boto3_health/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-07-27 05:23:17.000000 mypy-boto3-health-1.28.12/mypy_boto3_health/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-07-27 05:23:17.000000 mypy-boto3-health-1.28.12/mypy_boto3_health/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:16.000000 mypy-boto3-health-1.28.12/mypy_boto3_health/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21653 2023-07-27 05:23:17.000000 mypy-boto3-health-1.28.12/mypy_boto3_health/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21628 2023-07-27 05:23:17.000000 mypy-boto3-health-1.28.12/mypy_boto3_health/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:16.000000 mypy-boto3-health-1.28.12/mypy_boto3_health/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.532497 mypy-boto3-health-1.28.12/mypy_boto3_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-27 05:34:45.000000 mypy-boto3-health-1.28.12/mypy_boto3_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:34:45.000000 mypy-boto3-health-1.28.12/mypy_boto3_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:45.000000 mypy-boto3-health-1.28.12/mypy_boto3_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:45.000000 mypy-boto3-health-1.28.12/mypy_boto3_health.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:45.000000 mypy-boto3-health-1.28.12/mypy_boto3_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:45.000000 mypy-boto3-health-1.28.12/mypy_boto3_health.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:45.536496 mypy-boto3-health-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:23:16.000000 mypy-boto3-health-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.405174 mypy-boto3-health-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-28 20:42:53.405174 mypy-boto3-health-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.405174 mypy-boto3-health-1.28.15/mypy_boto3_health/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/mypy_boto3_health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/mypy_boto3_health/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/mypy_boto3_health/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/mypy_boto3_health/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/mypy_boto3_health/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/mypy_boto3_health/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/mypy_boto3_health/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/mypy_boto3_health/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/mypy_boto3_health/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/mypy_boto3_health/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21615 2023-07-28 20:27:19.000000 mypy-boto3-health-1.28.15/mypy_boto3_health/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-07-28 20:27:19.000000 mypy-boto3-health-1.28.15/mypy_boto3_health/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/mypy_boto3_health/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.405174 mypy-boto3-health-1.28.15/mypy_boto3_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-28 20:42:53.000000 mypy-boto3-health-1.28.15/mypy_boto3_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:42:53.000000 mypy-boto3-health-1.28.15/mypy_boto3_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-health-1.28.15/mypy_boto3_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-health-1.28.15/mypy_boto3_health.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:53.000000 mypy-boto3-health-1.28.15/mypy_boto3_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:42:53.000000 mypy-boto3-health-1.28.15/mypy_boto3_health.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:53.405174 mypy-boto3-health-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:27:17.000000 mypy-boto3-health-1.28.15/setup.py
```

### Comparing `mypy-boto3-health-1.28.12/LICENSE` & `mypy-boto3-health-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.12/PKG-INFO` & `mypy-boto3-health-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-health
-Version: 1.28.12
-Summary: Type annotations for boto3.Health 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Health 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-health)](https://pepy.tech/project/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-health docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,38 +357,38 @@
 `mypy_boto3_health.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_health.type_defs import (
     AffectedEntityTypeDef,
     DateTimeRangeTypeDef,
-    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
-    DescribeAffectedAccountsForOrganizationResponseTypeDef,
+    ResponseMetadataTypeDef,
     EventAccountFilterTypeDef,
     OrganizationAffectedEntitiesErrorItemTypeDef,
     DescribeEntityAggregatesRequestRequestTypeDef,
     EntityAggregateTypeDef,
     EventAggregateTypeDef,
     OrganizationEventDetailsErrorItemTypeDef,
     DescribeEventDetailsRequestRequestTypeDef,
     EventDetailsErrorItemTypeDef,
     EventTypeFilterTypeDef,
     EventTypeTypeDef,
     OrganizationEventTypeDef,
     EventTypeDef,
-    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventDescriptionTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeAffectedEntitiesResponseTypeDef,
     EntityFilterTypeDef,
     EventFilterTypeDef,
     OrganizationEventFilterTypeDef,
+    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    DescribeAffectedAccountsForOrganizationResponseTypeDef,
+    DescribeAffectedEntitiesResponseTypeDef,
+    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
     DescribeEventDetailsForOrganizationRequestRequestTypeDef,
     DescribeAffectedEntitiesForOrganizationResponseTypeDef,
     DescribeEntityAggregatesResponseTypeDef,
     DescribeEventAggregatesResponseTypeDef,
     DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef,
```

### Comparing `mypy-boto3-health-1.28.12/README.md` & `mypy-boto3-health-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-health)](https://pepy.tech/project/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-health docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,38 +325,38 @@
 `mypy_boto3_health.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_health.type_defs import (
     AffectedEntityTypeDef,
     DateTimeRangeTypeDef,
-    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
-    DescribeAffectedAccountsForOrganizationResponseTypeDef,
+    ResponseMetadataTypeDef,
     EventAccountFilterTypeDef,
     OrganizationAffectedEntitiesErrorItemTypeDef,
     DescribeEntityAggregatesRequestRequestTypeDef,
     EntityAggregateTypeDef,
     EventAggregateTypeDef,
     OrganizationEventDetailsErrorItemTypeDef,
     DescribeEventDetailsRequestRequestTypeDef,
     EventDetailsErrorItemTypeDef,
     EventTypeFilterTypeDef,
     EventTypeTypeDef,
     OrganizationEventTypeDef,
     EventTypeDef,
-    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventDescriptionTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeAffectedEntitiesResponseTypeDef,
     EntityFilterTypeDef,
     EventFilterTypeDef,
     OrganizationEventFilterTypeDef,
+    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    DescribeAffectedAccountsForOrganizationResponseTypeDef,
+    DescribeAffectedEntitiesResponseTypeDef,
+    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
     DescribeEventDetailsForOrganizationRequestRequestTypeDef,
     DescribeAffectedEntitiesForOrganizationResponseTypeDef,
     DescribeEntityAggregatesResponseTypeDef,
     DescribeEventAggregatesResponseTypeDef,
     DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef,
```

### Comparing `mypy-boto3-health-1.28.12/mypy_boto3_health/__init__.py` & `mypy-boto3-health-1.28.15/mypy_boto3_health/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.12/mypy_boto3_health/__init__.pyi` & `mypy-boto3-health-1.28.15/mypy_boto3_health/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.12/mypy_boto3_health/__main__.py` & `mypy-boto3-health-1.28.15/mypy_boto3_health/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Health 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Health 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-health-1.28.12/mypy_boto3_health/client.py` & `mypy-boto3-health-1.28.15/mypy_boto3_health/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.12/mypy_boto3_health/client.pyi` & `mypy-boto3-health-1.28.15/mypy_boto3_health/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.12/mypy_boto3_health/literals.py` & `mypy-boto3-health-1.28.15/mypy_boto3_health/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.12/mypy_boto3_health/literals.pyi` & `mypy-boto3-health-1.28.15/mypy_boto3_health/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.12/mypy_boto3_health/paginator.py` & `mypy-boto3-health-1.28.15/mypy_boto3_health/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 class DescribeAffectedAccountsForOrganizationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedAccountsForOrganization)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedaccountsfororganizationpaginator)
     """
 
     def paginate(
-        self, *, eventArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, eventArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAffectedAccountsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedAccountsForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedaccountsfororganizationpaginator)
         """
 
 
@@ -101,15 +101,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EntityFilterTypeDef,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAffectedEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedentitiespaginator)
         """
 
 
@@ -120,15 +120,15 @@
     """
 
     def paginate(
         self,
         *,
         organizationEntityFilters: Sequence[EventAccountFilterTypeDef],
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAffectedEntitiesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntitiesForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedentitiesfororganizationpaginator)
         """
 
 
@@ -139,15 +139,15 @@
     """
 
     def paginate(
         self,
         *,
         aggregateField: Literal["eventTypeCategory"],
         filter: EventFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventAggregates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventaggregatespaginator)
         """
 
 
@@ -158,15 +158,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventTypeFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventtypespaginator)
         """
 
 
@@ -177,15 +177,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventspaginator)
         """
 
 
@@ -196,13 +196,13 @@
     """
 
     def paginate(
         self,
         *,
         filter: OrganizationEventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventsForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventsfororganizationpaginator)
         """
```

### Comparing `mypy-boto3-health-1.28.12/mypy_boto3_health/paginator.pyi` & `mypy-boto3-health-1.28.15/mypy_boto3_health/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 class DescribeAffectedAccountsForOrganizationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedAccountsForOrganization)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedaccountsfororganizationpaginator)
     """
 
     def paginate(
-        self, *, eventArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, eventArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAffectedAccountsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedAccountsForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedaccountsfororganizationpaginator)
         """
 
 class DescribeAffectedEntitiesPaginator(Paginator):
@@ -96,15 +96,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EntityFilterTypeDef,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAffectedEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedentitiespaginator)
         """
 
 class DescribeAffectedEntitiesForOrganizationPaginator(Paginator):
@@ -114,15 +114,15 @@
     """
 
     def paginate(
         self,
         *,
         organizationEntityFilters: Sequence[EventAccountFilterTypeDef],
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAffectedEntitiesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeAffectedEntitiesForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeaffectedentitiesfororganizationpaginator)
         """
 
 class DescribeEventAggregatesPaginator(Paginator):
@@ -132,15 +132,15 @@
     """
 
     def paginate(
         self,
         *,
         aggregateField: Literal["eventTypeCategory"],
         filter: EventFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventAggregatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventAggregates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventaggregatespaginator)
         """
 
 class DescribeEventTypesPaginator(Paginator):
@@ -150,15 +150,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventTypeFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventtypespaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
@@ -168,15 +168,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: EventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventspaginator)
         """
 
 class DescribeEventsForOrganizationPaginator(Paginator):
@@ -186,13 +186,13 @@
     """
 
     def paginate(
         self,
         *,
         filter: OrganizationEventFilterTypeDef = ...,
         locale: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Paginator.DescribeEventsForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/paginators/#describeeventsfororganizationpaginator)
         """
```

### Comparing `mypy-boto3-health-1.28.12/mypy_boto3_health/type_defs.py` & `mypy-boto3-health-1.28.15/mypy_boto3_health/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,38 +31,38 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AffectedEntityTypeDef",
     "DateTimeRangeTypeDef",
-    "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
-    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "EventAccountFilterTypeDef",
     "OrganizationAffectedEntitiesErrorItemTypeDef",
     "DescribeEntityAggregatesRequestRequestTypeDef",
     "EntityAggregateTypeDef",
     "EventAggregateTypeDef",
     "OrganizationEventDetailsErrorItemTypeDef",
     "DescribeEventDetailsRequestRequestTypeDef",
     "EventDetailsErrorItemTypeDef",
     "EventTypeFilterTypeDef",
     "EventTypeTypeDef",
     "OrganizationEventTypeDef",
     "EventTypeDef",
-    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventDescriptionTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "DescribeAffectedEntitiesResponseTypeDef",
     "EntityFilterTypeDef",
     "EventFilterTypeDef",
     "OrganizationEventFilterTypeDef",
+    "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
+    "DescribeAffectedEntitiesResponseTypeDef",
+    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef",
     "DescribeEventDetailsForOrganizationRequestRequestTypeDef",
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     "DescribeEntityAggregatesResponseTypeDef",
     "DescribeEventAggregatesResponseTypeDef",
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
@@ -104,36 +104,24 @@
     {
         "from": Union[datetime, str],
         "to": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
-    {
-        "eventArn": str,
-    },
-)
-_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
-    _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-    _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
     {
         "eventArn": str,
     },
 )
 _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef = TypedDict(
@@ -149,21 +137,22 @@
 class DescribeAffectedAccountsForOrganizationRequestRequestTypeDef(
     _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
     _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
-    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "affectedAccounts": List[str],
-        "eventScopeCode": eventScopeCodeType,
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredEventAccountFilterTypeDef = TypedDict(
     "_RequiredEventAccountFilterTypeDef",
     {
         "eventArn": str,
@@ -315,67 +304,22 @@
         "lastUpdatedTime": datetime,
         "statusCode": eventStatusCodeType,
         "eventScopeCode": eventScopeCodeType,
     },
     total=False,
 )
 
-DescribeHealthServiceStatusForOrganizationResponseTypeDef = TypedDict(
-    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
-    {
-        "healthServiceAccessStatusForOrganization": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventDescriptionTypeDef = TypedDict(
     "EventDescriptionTypeDef",
     {
         "latestDescription": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
-DescribeAffectedEntitiesResponseTypeDef = TypedDict(
-    "DescribeAffectedEntitiesResponseTypeDef",
-    {
-        "entities": List[AffectedEntityTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEntityFilterTypeDef = TypedDict(
     "_RequiredEntityFilterTypeDef",
     {
         "eventArns": Sequence[str],
     },
 )
 _OptionalEntityFilterTypeDef = TypedDict(
@@ -429,25 +373,81 @@
         "entityValues": Sequence[str],
         "eventTypeCategories": Sequence[eventTypeCategoryType],
         "eventStatusCodes": Sequence[eventStatusCodeType],
     },
     total=False,
 )
 
+_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    {
+        "eventArn": str,
+    },
+)
+_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
+    _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+):
+    pass
+
+
+DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
+    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
+    {
+        "affectedAccounts": List[str],
+        "eventScopeCode": eventScopeCodeType,
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAffectedEntitiesResponseTypeDef = TypedDict(
+    "DescribeAffectedEntitiesResponseTypeDef",
+    {
+        "entities": List[AffectedEntityTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeHealthServiceStatusForOrganizationResponseTypeDef = TypedDict(
+    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
+    {
+        "healthServiceAccessStatusForOrganization": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     {
         "organizationEntityFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef = TypedDict(
     "_OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     {
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
@@ -504,41 +504,41 @@
 
 DescribeAffectedEntitiesForOrganizationResponseTypeDef = TypedDict(
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     {
         "entities": List[AffectedEntityTypeDef],
         "failedSet": List[OrganizationAffectedEntitiesErrorItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntityAggregatesResponseTypeDef = TypedDict(
     "DescribeEntityAggregatesResponseTypeDef",
     {
         "entityAggregates": List[EntityAggregateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventAggregatesResponseTypeDef = TypedDict(
     "DescribeEventAggregatesResponseTypeDef",
     {
         "eventAggregates": List[EventAggregateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef = TypedDict(
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
     {
         "filter": EventTypeFilterTypeDef,
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeEventTypesRequestRequestTypeDef = TypedDict(
     "DescribeEventTypesRequestRequestTypeDef",
     {
@@ -551,33 +551,33 @@
 )
 
 DescribeEventTypesResponseTypeDef = TypedDict(
     "DescribeEventTypesResponseTypeDef",
     {
         "eventTypes": List[EventTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsForOrganizationResponseTypeDef = TypedDict(
     "DescribeEventsForOrganizationResponseTypeDef",
     {
         "events": List[OrganizationEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "events": List[EventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventDetailsTypeDef = TypedDict(
     "EventDetailsTypeDef",
     {
         "event": EventTypeDef,
@@ -604,15 +604,15 @@
         "filter": EntityFilterTypeDef,
     },
 )
 _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef = TypedDict(
     "_OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     {
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
@@ -651,15 +651,15 @@
         "aggregateField": Literal["eventTypeCategory"],
     },
 )
 _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef = TypedDict(
     "_OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef(
     _RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
@@ -693,15 +693,15 @@
 
 
 DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeEventsRequestRequestTypeDef = TypedDict(
     "DescribeEventsRequestRequestTypeDef",
     {
@@ -714,15 +714,15 @@
 )
 
 DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef = TypedDict(
     "DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef",
     {
         "filter": OrganizationEventFilterTypeDef,
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeEventsForOrganizationRequestRequestTypeDef = TypedDict(
     "DescribeEventsForOrganizationRequestRequestTypeDef",
     {
@@ -735,19 +735,19 @@
 )
 
 DescribeEventDetailsResponseTypeDef = TypedDict(
     "DescribeEventDetailsResponseTypeDef",
     {
         "successfulSet": List[EventDetailsTypeDef],
         "failedSet": List[EventDetailsErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventDetailsForOrganizationResponseTypeDef = TypedDict(
     "DescribeEventDetailsForOrganizationResponseTypeDef",
     {
         "successfulSet": List[OrganizationEventDetailsTypeDef],
         "failedSet": List[OrganizationEventDetailsErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-health-1.28.12/mypy_boto3_health/type_defs.pyi` & `mypy-boto3-health-1.28.15/mypy_boto3_health/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -30,38 +30,38 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AffectedEntityTypeDef",
     "DateTimeRangeTypeDef",
-    "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
-    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "EventAccountFilterTypeDef",
     "OrganizationAffectedEntitiesErrorItemTypeDef",
     "DescribeEntityAggregatesRequestRequestTypeDef",
     "EntityAggregateTypeDef",
     "EventAggregateTypeDef",
     "OrganizationEventDetailsErrorItemTypeDef",
     "DescribeEventDetailsRequestRequestTypeDef",
     "EventDetailsErrorItemTypeDef",
     "EventTypeFilterTypeDef",
     "EventTypeTypeDef",
     "OrganizationEventTypeDef",
     "EventTypeDef",
-    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventDescriptionTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "DescribeAffectedEntitiesResponseTypeDef",
     "EntityFilterTypeDef",
     "EventFilterTypeDef",
     "OrganizationEventFilterTypeDef",
+    "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
+    "DescribeAffectedEntitiesResponseTypeDef",
+    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef",
     "DescribeEventDetailsForOrganizationRequestRequestTypeDef",
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     "DescribeEntityAggregatesResponseTypeDef",
     "DescribeEventAggregatesResponseTypeDef",
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
@@ -103,34 +103,24 @@
     {
         "from": Union[datetime, str],
         "to": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
-    {
-        "eventArn": str,
-    },
-)
-_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
-    _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-    _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
     {
         "eventArn": str,
     },
 )
 _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef = TypedDict(
@@ -144,21 +134,22 @@
 
 class DescribeAffectedAccountsForOrganizationRequestRequestTypeDef(
     _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
     _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
-DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
-    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "affectedAccounts": List[str],
-        "eventScopeCode": eventScopeCodeType,
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredEventAccountFilterTypeDef = TypedDict(
     "_RequiredEventAccountFilterTypeDef",
     {
         "eventArn": str,
@@ -306,67 +297,22 @@
         "lastUpdatedTime": datetime,
         "statusCode": eventStatusCodeType,
         "eventScopeCode": eventScopeCodeType,
     },
     total=False,
 )
 
-DescribeHealthServiceStatusForOrganizationResponseTypeDef = TypedDict(
-    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
-    {
-        "healthServiceAccessStatusForOrganization": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventDescriptionTypeDef = TypedDict(
     "EventDescriptionTypeDef",
     {
         "latestDescription": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
-DescribeAffectedEntitiesResponseTypeDef = TypedDict(
-    "DescribeAffectedEntitiesResponseTypeDef",
-    {
-        "entities": List[AffectedEntityTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEntityFilterTypeDef = TypedDict(
     "_RequiredEntityFilterTypeDef",
     {
         "eventArns": Sequence[str],
     },
 )
 _OptionalEntityFilterTypeDef = TypedDict(
@@ -418,25 +364,79 @@
         "entityValues": Sequence[str],
         "eventTypeCategories": Sequence[eventTypeCategoryType],
         "eventStatusCodes": Sequence[eventStatusCodeType],
     },
     total=False,
 )
 
+_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    {
+        "eventArn": str,
+    },
+)
+_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
+    _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+):
+    pass
+
+DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
+    "DescribeAffectedAccountsForOrganizationResponseTypeDef",
+    {
+        "affectedAccounts": List[str],
+        "eventScopeCode": eventScopeCodeType,
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAffectedEntitiesResponseTypeDef = TypedDict(
+    "DescribeAffectedEntitiesResponseTypeDef",
+    {
+        "entities": List[AffectedEntityTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeHealthServiceStatusForOrganizationResponseTypeDef = TypedDict(
+    "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
+    {
+        "healthServiceAccessStatusForOrganization": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     {
         "organizationEntityFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef = TypedDict(
     "_OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     {
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     _OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
@@ -487,41 +487,41 @@
 
 DescribeAffectedEntitiesForOrganizationResponseTypeDef = TypedDict(
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     {
         "entities": List[AffectedEntityTypeDef],
         "failedSet": List[OrganizationAffectedEntitiesErrorItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEntityAggregatesResponseTypeDef = TypedDict(
     "DescribeEntityAggregatesResponseTypeDef",
     {
         "entityAggregates": List[EntityAggregateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventAggregatesResponseTypeDef = TypedDict(
     "DescribeEventAggregatesResponseTypeDef",
     {
         "eventAggregates": List[EventAggregateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef = TypedDict(
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
     {
         "filter": EventTypeFilterTypeDef,
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeEventTypesRequestRequestTypeDef = TypedDict(
     "DescribeEventTypesRequestRequestTypeDef",
     {
@@ -534,33 +534,33 @@
 )
 
 DescribeEventTypesResponseTypeDef = TypedDict(
     "DescribeEventTypesResponseTypeDef",
     {
         "eventTypes": List[EventTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsForOrganizationResponseTypeDef = TypedDict(
     "DescribeEventsForOrganizationResponseTypeDef",
     {
         "events": List[OrganizationEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "events": List[EventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventDetailsTypeDef = TypedDict(
     "EventDetailsTypeDef",
     {
         "event": EventTypeDef,
@@ -587,15 +587,15 @@
         "filter": EntityFilterTypeDef,
     },
 )
 _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef = TypedDict(
     "_OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     {
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
     _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
@@ -630,15 +630,15 @@
         "aggregateField": Literal["eventTypeCategory"],
     },
 )
 _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef = TypedDict(
     "_OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef(
     _RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
     _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
@@ -668,15 +668,15 @@
     pass
 
 DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeEventsRequestRequestTypeDef = TypedDict(
     "DescribeEventsRequestRequestTypeDef",
     {
@@ -689,15 +689,15 @@
 )
 
 DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef = TypedDict(
     "DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef",
     {
         "filter": OrganizationEventFilterTypeDef,
         "locale": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeEventsForOrganizationRequestRequestTypeDef = TypedDict(
     "DescribeEventsForOrganizationRequestRequestTypeDef",
     {
@@ -710,19 +710,19 @@
 )
 
 DescribeEventDetailsResponseTypeDef = TypedDict(
     "DescribeEventDetailsResponseTypeDef",
     {
         "successfulSet": List[EventDetailsTypeDef],
         "failedSet": List[EventDetailsErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventDetailsForOrganizationResponseTypeDef = TypedDict(
     "DescribeEventDetailsForOrganizationResponseTypeDef",
     {
         "successfulSet": List[OrganizationEventDetailsTypeDef],
         "failedSet": List[OrganizationEventDetailsErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-health-1.28.12/mypy_boto3_health.egg-info/PKG-INFO` & `mypy-boto3-health-1.28.15/mypy_boto3_health.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-health
-Version: 1.28.12
-Summary: Type annotations for boto3.Health 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Health 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-health)](https://pepy.tech/project/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-health docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,38 +357,38 @@
 `mypy_boto3_health.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_health.type_defs import (
     AffectedEntityTypeDef,
     DateTimeRangeTypeDef,
-    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
-    DescribeAffectedAccountsForOrganizationResponseTypeDef,
+    ResponseMetadataTypeDef,
     EventAccountFilterTypeDef,
     OrganizationAffectedEntitiesErrorItemTypeDef,
     DescribeEntityAggregatesRequestRequestTypeDef,
     EntityAggregateTypeDef,
     EventAggregateTypeDef,
     OrganizationEventDetailsErrorItemTypeDef,
     DescribeEventDetailsRequestRequestTypeDef,
     EventDetailsErrorItemTypeDef,
     EventTypeFilterTypeDef,
     EventTypeTypeDef,
     OrganizationEventTypeDef,
     EventTypeDef,
-    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventDescriptionTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeAffectedEntitiesResponseTypeDef,
     EntityFilterTypeDef,
     EventFilterTypeDef,
     OrganizationEventFilterTypeDef,
+    DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
+    DescribeAffectedAccountsForOrganizationResponseTypeDef,
+    DescribeAffectedEntitiesResponseTypeDef,
+    DescribeHealthServiceStatusForOrganizationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
     DescribeEventDetailsForOrganizationRequestRequestTypeDef,
     DescribeAffectedEntitiesForOrganizationResponseTypeDef,
     DescribeEntityAggregatesResponseTypeDef,
     DescribeEventAggregatesResponseTypeDef,
     DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef,
```

### Comparing `mypy-boto3-health-1.28.12/mypy_boto3_health.egg-info/SOURCES.txt` & `mypy-boto3-health-1.28.15/mypy_boto3_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.12/setup.py` & `mypy-boto3-health-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-health",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_health"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Health 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Health 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

