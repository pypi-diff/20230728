# Comparing `tmp/mypy-boto3-cloudsearch-1.28.12.tar.gz` & `tmp/mypy-boto3-cloudsearch-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudsearch-1.28.12.tar", last modified: Thu Jul 27 05:34:26 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudsearch-1.28.15.tar", last modified: Fri Jul 28 20:42:25 2023, max compression
```

## Comparing `mypy-boto3-cloudsearch-1.28.12.tar` & `mypy-boto3-cloudsearch-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.068559 mypy-boto3-cloudsearch-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15955 2023-07-27 05:34:26.056559 mypy-boto3-cloudsearch-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14452 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.056559 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-07-27 05:18:45.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-07-27 05:18:45.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-07-27 05:18:45.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32448 2023-07-27 05:18:45.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32417 2023-07-27 05:18:45.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.056559 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15955 2023-07-27 05:34:25.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-27 05:34:25.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:25.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:25.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:25.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:25.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:26.068559 mypy-boto3-cloudsearch-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.564783 mypy-boto3-cloudsearch-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15318 2023-07-28 20:42:25.556783 mypy-boto3-cloudsearch-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.556783 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25479 2023-07-28 20:21:02.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25454 2023-07-28 20:21:02.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.556783 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15318 2023-07-28 20:42:25.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-28 20:42:25.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:25.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:42:25.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:25.564783 mypy-boto3-cloudsearch-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/setup.py
```

### Comparing `mypy-boto3-cloudsearch-1.28.12/LICENSE` & `mypy-boto3-cloudsearch-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.12/PKG-INFO` & `mypy-boto3-cloudsearch-1.28.15/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-cloudsearch
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudSearch 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cloudsearch type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-cloudsearch"></a>
 
 # mypy-boto3-cloudsearch
 
 [![PyPI - mypy-boto3-cloudsearch](https://img.shields.io/pypi/v/mypy-boto3-cloudsearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudsearch)](https://pepy.tech/project/mypy-boto3-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
+[boto3.CloudSearch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
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
 [mypy-boto3-cloudsearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,22 +271,19 @@
 
 `mypy_boto3_cloudsearch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudsearch.type_defs import (
     OptionStatusTypeDef,
-    AnalysisOptionsOutputTypeDef,
     AnalysisOptionsTypeDef,
     BuildSuggestersRequestRequestTypeDef,
-    BuildSuggestersResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDomainRequestRequestTypeDef,
-    DateArrayOptionsOutputTypeDef,
     DateArrayOptionsTypeDef,
-    DateOptionsOutputTypeDef,
     DateOptionsTypeDef,
     ExpressionTypeDef,
     DeleteAnalysisSchemeRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteExpressionRequestRequestTypeDef,
     DeleteIndexFieldRequestRequestTypeDef,
     DeleteSuggesterRequestRequestTypeDef,
@@ -327,80 +292,64 @@
     DescribeDomainEndpointOptionsRequestRequestTypeDef,
     DescribeDomainsRequestRequestTypeDef,
     DescribeExpressionsRequestRequestTypeDef,
     DescribeIndexFieldsRequestRequestTypeDef,
     DescribeScalingParametersRequestRequestTypeDef,
     DescribeServiceAccessPoliciesRequestRequestTypeDef,
     DescribeSuggestersRequestRequestTypeDef,
-    DocumentSuggesterOptionsOutputTypeDef,
     DocumentSuggesterOptionsTypeDef,
-    DomainEndpointOptionsOutputTypeDef,
     DomainEndpointOptionsTypeDef,
     LimitsTypeDef,
     ServiceEndpointTypeDef,
-    DoubleArrayOptionsOutputTypeDef,
     DoubleArrayOptionsTypeDef,
-    DoubleOptionsOutputTypeDef,
     DoubleOptionsTypeDef,
-    ExpressionOutputTypeDef,
     IndexDocumentsRequestRequestTypeDef,
-    IndexDocumentsResponseTypeDef,
-    IntArrayOptionsOutputTypeDef,
-    IntOptionsOutputTypeDef,
-    LatLonOptionsOutputTypeDef,
-    LiteralArrayOptionsOutputTypeDef,
-    LiteralOptionsOutputTypeDef,
-    TextArrayOptionsOutputTypeDef,
-    TextOptionsOutputTypeDef,
     IntArrayOptionsTypeDef,
     IntOptionsTypeDef,
     LatLonOptionsTypeDef,
     LiteralArrayOptionsTypeDef,
     LiteralOptionsTypeDef,
     TextArrayOptionsTypeDef,
     TextOptionsTypeDef,
-    ListDomainNamesResponseTypeDef,
-    ResponseMetadataTypeDef,
-    ScalingParametersOutputTypeDef,
     ScalingParametersTypeDef,
     UpdateAvailabilityOptionsRequestRequestTypeDef,
     UpdateServiceAccessPoliciesRequestRequestTypeDef,
     AccessPoliciesStatusTypeDef,
     AvailabilityOptionsStatusTypeDef,
-    AnalysisSchemeOutputTypeDef,
     AnalysisSchemeTypeDef,
+    BuildSuggestersResponseTypeDef,
+    IndexDocumentsResponseTypeDef,
+    ListDomainNamesResponseTypeDef,
     DefineExpressionRequestRequestTypeDef,
-    SuggesterOutputTypeDef,
+    ExpressionStatusTypeDef,
     SuggesterTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     UpdateDomainEndpointOptionsRequestRequestTypeDef,
     DomainStatusTypeDef,
-    ExpressionStatusTypeDef,
-    IndexFieldOutputTypeDef,
     IndexFieldTypeDef,
     ScalingParametersStatusTypeDef,
     UpdateScalingParametersRequestRequestTypeDef,
     DescribeServiceAccessPoliciesResponseTypeDef,
     UpdateServiceAccessPoliciesResponseTypeDef,
     DescribeAvailabilityOptionsResponseTypeDef,
     UpdateAvailabilityOptionsResponseTypeDef,
     AnalysisSchemeStatusTypeDef,
     DefineAnalysisSchemeRequestRequestTypeDef,
-    SuggesterStatusTypeDef,
+    DefineExpressionResponseTypeDef,
+    DeleteExpressionResponseTypeDef,
+    DescribeExpressionsResponseTypeDef,
     DefineSuggesterRequestRequestTypeDef,
+    SuggesterStatusTypeDef,
     DescribeDomainEndpointOptionsResponseTypeDef,
     UpdateDomainEndpointOptionsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DescribeDomainsResponseTypeDef,
-    DefineExpressionResponseTypeDef,
-    DeleteExpressionResponseTypeDef,
-    DescribeExpressionsResponseTypeDef,
-    IndexFieldStatusTypeDef,
     DefineIndexFieldRequestRequestTypeDef,
+    IndexFieldStatusTypeDef,
     DescribeScalingParametersResponseTypeDef,
     UpdateScalingParametersResponseTypeDef,
     DefineAnalysisSchemeResponseTypeDef,
     DeleteAnalysisSchemeResponseTypeDef,
     DescribeAnalysisSchemesResponseTypeDef,
     DefineSuggesterResponseTypeDef,
     DeleteSuggesterResponseTypeDef,
```

### Comparing `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/__main__.py` & `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudSearch 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.CloudSearch 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch\nOther"
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

### Comparing `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/client.py` & `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/client.pyi` & `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/literals.py` & `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/literals.pyi` & `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/type_defs.py` & `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/type_defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,22 +29,19 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "OptionStatusTypeDef",
-    "AnalysisOptionsOutputTypeDef",
     "AnalysisOptionsTypeDef",
     "BuildSuggestersRequestRequestTypeDef",
-    "BuildSuggestersResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "DateArrayOptionsOutputTypeDef",
     "DateArrayOptionsTypeDef",
-    "DateOptionsOutputTypeDef",
     "DateOptionsTypeDef",
     "ExpressionTypeDef",
     "DeleteAnalysisSchemeRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteExpressionRequestRequestTypeDef",
     "DeleteIndexFieldRequestRequestTypeDef",
     "DeleteSuggesterRequestRequestTypeDef",
@@ -53,80 +50,64 @@
     "DescribeDomainEndpointOptionsRequestRequestTypeDef",
     "DescribeDomainsRequestRequestTypeDef",
     "DescribeExpressionsRequestRequestTypeDef",
     "DescribeIndexFieldsRequestRequestTypeDef",
     "DescribeScalingParametersRequestRequestTypeDef",
     "DescribeServiceAccessPoliciesRequestRequestTypeDef",
     "DescribeSuggestersRequestRequestTypeDef",
-    "DocumentSuggesterOptionsOutputTypeDef",
     "DocumentSuggesterOptionsTypeDef",
-    "DomainEndpointOptionsOutputTypeDef",
     "DomainEndpointOptionsTypeDef",
     "LimitsTypeDef",
     "ServiceEndpointTypeDef",
-    "DoubleArrayOptionsOutputTypeDef",
     "DoubleArrayOptionsTypeDef",
-    "DoubleOptionsOutputTypeDef",
     "DoubleOptionsTypeDef",
-    "ExpressionOutputTypeDef",
     "IndexDocumentsRequestRequestTypeDef",
-    "IndexDocumentsResponseTypeDef",
-    "IntArrayOptionsOutputTypeDef",
-    "IntOptionsOutputTypeDef",
-    "LatLonOptionsOutputTypeDef",
-    "LiteralArrayOptionsOutputTypeDef",
-    "LiteralOptionsOutputTypeDef",
-    "TextArrayOptionsOutputTypeDef",
-    "TextOptionsOutputTypeDef",
     "IntArrayOptionsTypeDef",
     "IntOptionsTypeDef",
     "LatLonOptionsTypeDef",
     "LiteralArrayOptionsTypeDef",
     "LiteralOptionsTypeDef",
     "TextArrayOptionsTypeDef",
     "TextOptionsTypeDef",
-    "ListDomainNamesResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "ScalingParametersOutputTypeDef",
     "ScalingParametersTypeDef",
     "UpdateAvailabilityOptionsRequestRequestTypeDef",
     "UpdateServiceAccessPoliciesRequestRequestTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AvailabilityOptionsStatusTypeDef",
-    "AnalysisSchemeOutputTypeDef",
     "AnalysisSchemeTypeDef",
+    "BuildSuggestersResponseTypeDef",
+    "IndexDocumentsResponseTypeDef",
+    "ListDomainNamesResponseTypeDef",
     "DefineExpressionRequestRequestTypeDef",
-    "SuggesterOutputTypeDef",
+    "ExpressionStatusTypeDef",
     "SuggesterTypeDef",
     "DomainEndpointOptionsStatusTypeDef",
     "UpdateDomainEndpointOptionsRequestRequestTypeDef",
     "DomainStatusTypeDef",
-    "ExpressionStatusTypeDef",
-    "IndexFieldOutputTypeDef",
     "IndexFieldTypeDef",
     "ScalingParametersStatusTypeDef",
     "UpdateScalingParametersRequestRequestTypeDef",
     "DescribeServiceAccessPoliciesResponseTypeDef",
     "UpdateServiceAccessPoliciesResponseTypeDef",
     "DescribeAvailabilityOptionsResponseTypeDef",
     "UpdateAvailabilityOptionsResponseTypeDef",
     "AnalysisSchemeStatusTypeDef",
     "DefineAnalysisSchemeRequestRequestTypeDef",
-    "SuggesterStatusTypeDef",
+    "DefineExpressionResponseTypeDef",
+    "DeleteExpressionResponseTypeDef",
+    "DescribeExpressionsResponseTypeDef",
     "DefineSuggesterRequestRequestTypeDef",
+    "SuggesterStatusTypeDef",
     "DescribeDomainEndpointOptionsResponseTypeDef",
     "UpdateDomainEndpointOptionsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DeleteDomainResponseTypeDef",
     "DescribeDomainsResponseTypeDef",
-    "DefineExpressionResponseTypeDef",
-    "DeleteExpressionResponseTypeDef",
-    "DescribeExpressionsResponseTypeDef",
-    "IndexFieldStatusTypeDef",
     "DefineIndexFieldRequestRequestTypeDef",
+    "IndexFieldStatusTypeDef",
     "DescribeScalingParametersResponseTypeDef",
     "UpdateScalingParametersResponseTypeDef",
     "DefineAnalysisSchemeResponseTypeDef",
     "DeleteAnalysisSchemeResponseTypeDef",
     "DescribeAnalysisSchemesResponseTypeDef",
     "DefineSuggesterResponseTypeDef",
     "DeleteSuggesterResponseTypeDef",
@@ -154,26 +135,14 @@
 )
 
 
 class OptionStatusTypeDef(_RequiredOptionStatusTypeDef, _OptionalOptionStatusTypeDef):
     pass
 
 
-AnalysisOptionsOutputTypeDef = TypedDict(
-    "AnalysisOptionsOutputTypeDef",
-    {
-        "Synonyms": str,
-        "Stopwords": str,
-        "StemmingDictionary": str,
-        "JapaneseTokenizationDictionary": str,
-        "AlgorithmicStemming": AlgorithmicStemmingType,
-    },
-    total=False,
-)
-
 AnalysisOptionsTypeDef = TypedDict(
     "AnalysisOptionsTypeDef",
     {
         "Synonyms": str,
         "Stopwords": str,
         "StemmingDictionary": str,
         "JapaneseTokenizationDictionary": str,
@@ -185,66 +154,44 @@
 BuildSuggestersRequestRequestTypeDef = TypedDict(
     "BuildSuggestersRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-BuildSuggestersResponseTypeDef = TypedDict(
-    "BuildSuggestersResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FieldNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DateArrayOptionsOutputTypeDef = TypedDict(
-    "DateArrayOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceFields": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-    },
-    total=False,
-)
-
 DateArrayOptionsTypeDef = TypedDict(
     "DateArrayOptionsTypeDef",
     {
         "DefaultValue": str,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
         "ReturnEnabled": bool,
     },
     total=False,
 )
 
-DateOptionsOutputTypeDef = TypedDict(
-    "DateOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceField": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-        "SortEnabled": bool,
-    },
-    total=False,
-)
-
 DateOptionsTypeDef = TypedDict(
     "DateOptionsTypeDef",
     {
         "DefaultValue": str,
         "SourceField": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
@@ -470,36 +417,14 @@
 class DescribeSuggestersRequestRequestTypeDef(
     _RequiredDescribeSuggestersRequestRequestTypeDef,
     _OptionalDescribeSuggestersRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDocumentSuggesterOptionsOutputTypeDef = TypedDict(
-    "_RequiredDocumentSuggesterOptionsOutputTypeDef",
-    {
-        "SourceField": str,
-    },
-)
-_OptionalDocumentSuggesterOptionsOutputTypeDef = TypedDict(
-    "_OptionalDocumentSuggesterOptionsOutputTypeDef",
-    {
-        "FuzzyMatching": SuggesterFuzzyMatchingType,
-        "SortExpression": str,
-    },
-    total=False,
-)
-
-
-class DocumentSuggesterOptionsOutputTypeDef(
-    _RequiredDocumentSuggesterOptionsOutputTypeDef, _OptionalDocumentSuggesterOptionsOutputTypeDef
-):
-    pass
-
-
 _RequiredDocumentSuggesterOptionsTypeDef = TypedDict(
     "_RequiredDocumentSuggesterOptionsTypeDef",
     {
         "SourceField": str,
     },
 )
 _OptionalDocumentSuggesterOptionsTypeDef = TypedDict(
@@ -514,23 +439,14 @@
 
 class DocumentSuggesterOptionsTypeDef(
     _RequiredDocumentSuggesterOptionsTypeDef, _OptionalDocumentSuggesterOptionsTypeDef
 ):
     pass
 
 
-DomainEndpointOptionsOutputTypeDef = TypedDict(
-    "DomainEndpointOptionsOutputTypeDef",
-    {
-        "EnforceHTTPS": bool,
-        "TLSSecurityPolicy": TLSSecurityPolicyType,
-    },
-    total=False,
-)
-
 DomainEndpointOptionsTypeDef = TypedDict(
     "DomainEndpointOptionsTypeDef",
     {
         "EnforceHTTPS": bool,
         "TLSSecurityPolicy": TLSSecurityPolicyType,
     },
     total=False,
@@ -548,175 +464,46 @@
     "ServiceEndpointTypeDef",
     {
         "Endpoint": str,
     },
     total=False,
 )
 
-DoubleArrayOptionsOutputTypeDef = TypedDict(
-    "DoubleArrayOptionsOutputTypeDef",
-    {
-        "DefaultValue": float,
-        "SourceFields": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-    },
-    total=False,
-)
-
 DoubleArrayOptionsTypeDef = TypedDict(
     "DoubleArrayOptionsTypeDef",
     {
         "DefaultValue": float,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
         "ReturnEnabled": bool,
     },
     total=False,
 )
 
-DoubleOptionsOutputTypeDef = TypedDict(
-    "DoubleOptionsOutputTypeDef",
-    {
-        "DefaultValue": float,
-        "SourceField": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-        "SortEnabled": bool,
-    },
-    total=False,
-)
-
 DoubleOptionsTypeDef = TypedDict(
     "DoubleOptionsTypeDef",
     {
         "DefaultValue": float,
         "SourceField": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
         "ReturnEnabled": bool,
         "SortEnabled": bool,
     },
     total=False,
 )
 
-ExpressionOutputTypeDef = TypedDict(
-    "ExpressionOutputTypeDef",
-    {
-        "ExpressionName": str,
-        "ExpressionValue": str,
-    },
-)
-
 IndexDocumentsRequestRequestTypeDef = TypedDict(
     "IndexDocumentsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-IndexDocumentsResponseTypeDef = TypedDict(
-    "IndexDocumentsResponseTypeDef",
-    {
-        "FieldNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IntArrayOptionsOutputTypeDef = TypedDict(
-    "IntArrayOptionsOutputTypeDef",
-    {
-        "DefaultValue": int,
-        "SourceFields": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-    },
-    total=False,
-)
-
-IntOptionsOutputTypeDef = TypedDict(
-    "IntOptionsOutputTypeDef",
-    {
-        "DefaultValue": int,
-        "SourceField": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-        "SortEnabled": bool,
-    },
-    total=False,
-)
-
-LatLonOptionsOutputTypeDef = TypedDict(
-    "LatLonOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceField": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-        "SortEnabled": bool,
-    },
-    total=False,
-)
-
-LiteralArrayOptionsOutputTypeDef = TypedDict(
-    "LiteralArrayOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceFields": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-    },
-    total=False,
-)
-
-LiteralOptionsOutputTypeDef = TypedDict(
-    "LiteralOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceField": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-        "SortEnabled": bool,
-    },
-    total=False,
-)
-
-TextArrayOptionsOutputTypeDef = TypedDict(
-    "TextArrayOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceFields": str,
-        "ReturnEnabled": bool,
-        "HighlightEnabled": bool,
-        "AnalysisScheme": str,
-    },
-    total=False,
-)
-
-TextOptionsOutputTypeDef = TypedDict(
-    "TextOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceField": str,
-        "ReturnEnabled": bool,
-        "SortEnabled": bool,
-        "HighlightEnabled": bool,
-        "AnalysisScheme": str,
-    },
-    total=False,
-)
-
 IntArrayOptionsTypeDef = TypedDict(
     "IntArrayOptionsTypeDef",
     {
         "DefaultValue": int,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
@@ -797,43 +584,14 @@
         "SortEnabled": bool,
         "HighlightEnabled": bool,
         "AnalysisScheme": str,
     },
     total=False,
 )
 
-ListDomainNamesResponseTypeDef = TypedDict(
-    "ListDomainNamesResponseTypeDef",
-    {
-        "DomainNames": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
-ScalingParametersOutputTypeDef = TypedDict(
-    "ScalingParametersOutputTypeDef",
-    {
-        "DesiredInstanceType": PartitionInstanceTypeType,
-        "DesiredReplicationCount": int,
-        "DesiredPartitionCount": int,
-    },
-    total=False,
-)
-
 ScalingParametersTypeDef = TypedDict(
     "ScalingParametersTypeDef",
     {
         "DesiredInstanceType": PartitionInstanceTypeType,
         "DesiredReplicationCount": int,
         "DesiredPartitionCount": int,
     },
@@ -868,84 +626,86 @@
     "AvailabilityOptionsStatusTypeDef",
     {
         "Options": bool,
         "Status": OptionStatusTypeDef,
     },
 )
 
-_RequiredAnalysisSchemeOutputTypeDef = TypedDict(
-    "_RequiredAnalysisSchemeOutputTypeDef",
+_RequiredAnalysisSchemeTypeDef = TypedDict(
+    "_RequiredAnalysisSchemeTypeDef",
     {
         "AnalysisSchemeName": str,
         "AnalysisSchemeLanguage": AnalysisSchemeLanguageType,
     },
 )
-_OptionalAnalysisSchemeOutputTypeDef = TypedDict(
-    "_OptionalAnalysisSchemeOutputTypeDef",
+_OptionalAnalysisSchemeTypeDef = TypedDict(
+    "_OptionalAnalysisSchemeTypeDef",
     {
-        "AnalysisOptions": AnalysisOptionsOutputTypeDef,
+        "AnalysisOptions": AnalysisOptionsTypeDef,
     },
     total=False,
 )
 
 
-class AnalysisSchemeOutputTypeDef(
-    _RequiredAnalysisSchemeOutputTypeDef, _OptionalAnalysisSchemeOutputTypeDef
-):
+class AnalysisSchemeTypeDef(_RequiredAnalysisSchemeTypeDef, _OptionalAnalysisSchemeTypeDef):
     pass
 
 
-_RequiredAnalysisSchemeTypeDef = TypedDict(
-    "_RequiredAnalysisSchemeTypeDef",
+BuildSuggestersResponseTypeDef = TypedDict(
+    "BuildSuggestersResponseTypeDef",
     {
-        "AnalysisSchemeName": str,
-        "AnalysisSchemeLanguage": AnalysisSchemeLanguageType,
+        "FieldNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAnalysisSchemeTypeDef = TypedDict(
-    "_OptionalAnalysisSchemeTypeDef",
+
+IndexDocumentsResponseTypeDef = TypedDict(
+    "IndexDocumentsResponseTypeDef",
     {
-        "AnalysisOptions": AnalysisOptionsTypeDef,
+        "FieldNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class AnalysisSchemeTypeDef(_RequiredAnalysisSchemeTypeDef, _OptionalAnalysisSchemeTypeDef):
-    pass
-
+ListDomainNamesResponseTypeDef = TypedDict(
+    "ListDomainNamesResponseTypeDef",
+    {
+        "DomainNames": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 DefineExpressionRequestRequestTypeDef = TypedDict(
     "DefineExpressionRequestRequestTypeDef",
     {
         "DomainName": str,
         "Expression": ExpressionTypeDef,
     },
 )
 
-SuggesterOutputTypeDef = TypedDict(
-    "SuggesterOutputTypeDef",
+ExpressionStatusTypeDef = TypedDict(
+    "ExpressionStatusTypeDef",
     {
-        "SuggesterName": str,
-        "DocumentSuggesterOptions": DocumentSuggesterOptionsOutputTypeDef,
+        "Options": ExpressionTypeDef,
+        "Status": OptionStatusTypeDef,
     },
 )
 
 SuggesterTypeDef = TypedDict(
     "SuggesterTypeDef",
     {
         "SuggesterName": str,
         "DocumentSuggesterOptions": DocumentSuggesterOptionsTypeDef,
     },
 )
 
 DomainEndpointOptionsStatusTypeDef = TypedDict(
     "DomainEndpointOptionsStatusTypeDef",
     {
-        "Options": DomainEndpointOptionsOutputTypeDef,
+        "Options": DomainEndpointOptionsTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 UpdateDomainEndpointOptionsRequestRequestTypeDef = TypedDict(
     "UpdateDomainEndpointOptionsRequestRequestTypeDef",
     {
@@ -980,52 +740,14 @@
 )
 
 
 class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
     pass
 
 
-ExpressionStatusTypeDef = TypedDict(
-    "ExpressionStatusTypeDef",
-    {
-        "Options": ExpressionOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-_RequiredIndexFieldOutputTypeDef = TypedDict(
-    "_RequiredIndexFieldOutputTypeDef",
-    {
-        "IndexFieldName": str,
-        "IndexFieldType": IndexFieldTypeType,
-    },
-)
-_OptionalIndexFieldOutputTypeDef = TypedDict(
-    "_OptionalIndexFieldOutputTypeDef",
-    {
-        "IntOptions": IntOptionsOutputTypeDef,
-        "DoubleOptions": DoubleOptionsOutputTypeDef,
-        "LiteralOptions": LiteralOptionsOutputTypeDef,
-        "TextOptions": TextOptionsOutputTypeDef,
-        "DateOptions": DateOptionsOutputTypeDef,
-        "LatLonOptions": LatLonOptionsOutputTypeDef,
-        "IntArrayOptions": IntArrayOptionsOutputTypeDef,
-        "DoubleArrayOptions": DoubleArrayOptionsOutputTypeDef,
-        "LiteralArrayOptions": LiteralArrayOptionsOutputTypeDef,
-        "TextArrayOptions": TextArrayOptionsOutputTypeDef,
-        "DateArrayOptions": DateArrayOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class IndexFieldOutputTypeDef(_RequiredIndexFieldOutputTypeDef, _OptionalIndexFieldOutputTypeDef):
-    pass
-
-
 _RequiredIndexFieldTypeDef = TypedDict(
     "_RequiredIndexFieldTypeDef",
     {
         "IndexFieldName": str,
         "IndexFieldType": IndexFieldTypeType,
     },
 )
@@ -1051,15 +773,15 @@
 class IndexFieldTypeDef(_RequiredIndexFieldTypeDef, _OptionalIndexFieldTypeDef):
     pass
 
 
 ScalingParametersStatusTypeDef = TypedDict(
     "ScalingParametersStatusTypeDef",
     {
-        "Options": ScalingParametersOutputTypeDef,
+        "Options": ScalingParametersTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 UpdateScalingParametersRequestRequestTypeDef = TypedDict(
     "UpdateScalingParametersRequestRequestTypeDef",
     {
@@ -1068,234 +790,234 @@
     },
 )
 
 DescribeServiceAccessPoliciesResponseTypeDef = TypedDict(
     "DescribeServiceAccessPoliciesResponseTypeDef",
     {
         "AccessPolicies": AccessPoliciesStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceAccessPoliciesResponseTypeDef = TypedDict(
     "UpdateServiceAccessPoliciesResponseTypeDef",
     {
         "AccessPolicies": AccessPoliciesStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAvailabilityOptionsResponseTypeDef = TypedDict(
     "DescribeAvailabilityOptionsResponseTypeDef",
     {
         "AvailabilityOptions": AvailabilityOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAvailabilityOptionsResponseTypeDef = TypedDict(
     "UpdateAvailabilityOptionsResponseTypeDef",
     {
         "AvailabilityOptions": AvailabilityOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AnalysisSchemeStatusTypeDef = TypedDict(
     "AnalysisSchemeStatusTypeDef",
     {
-        "Options": AnalysisSchemeOutputTypeDef,
+        "Options": AnalysisSchemeTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 DefineAnalysisSchemeRequestRequestTypeDef = TypedDict(
     "DefineAnalysisSchemeRequestRequestTypeDef",
     {
         "DomainName": str,
         "AnalysisScheme": AnalysisSchemeTypeDef,
     },
 )
 
-SuggesterStatusTypeDef = TypedDict(
-    "SuggesterStatusTypeDef",
+DefineExpressionResponseTypeDef = TypedDict(
+    "DefineExpressionResponseTypeDef",
     {
-        "Options": SuggesterOutputTypeDef,
-        "Status": OptionStatusTypeDef,
+        "Expression": ExpressionStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteExpressionResponseTypeDef = TypedDict(
+    "DeleteExpressionResponseTypeDef",
+    {
+        "Expression": ExpressionStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeExpressionsResponseTypeDef = TypedDict(
+    "DescribeExpressionsResponseTypeDef",
+    {
+        "Expressions": List[ExpressionStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineSuggesterRequestRequestTypeDef = TypedDict(
     "DefineSuggesterRequestRequestTypeDef",
     {
         "DomainName": str,
         "Suggester": SuggesterTypeDef,
     },
 )
 
+SuggesterStatusTypeDef = TypedDict(
+    "SuggesterStatusTypeDef",
+    {
+        "Options": SuggesterTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
 DescribeDomainEndpointOptionsResponseTypeDef = TypedDict(
     "DescribeDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainEndpointOptionsResponseTypeDef = TypedDict(
     "UpdateDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResponseTypeDef = TypedDict(
     "DeleteDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainsResponseTypeDef = TypedDict(
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DefineExpressionResponseTypeDef = TypedDict(
-    "DefineExpressionResponseTypeDef",
-    {
-        "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteExpressionResponseTypeDef = TypedDict(
-    "DeleteExpressionResponseTypeDef",
-    {
-        "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeExpressionsResponseTypeDef = TypedDict(
-    "DescribeExpressionsResponseTypeDef",
+DefineIndexFieldRequestRequestTypeDef = TypedDict(
+    "DefineIndexFieldRequestRequestTypeDef",
     {
-        "Expressions": List[ExpressionStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DomainName": str,
+        "IndexField": IndexFieldTypeDef,
     },
 )
 
 IndexFieldStatusTypeDef = TypedDict(
     "IndexFieldStatusTypeDef",
     {
-        "Options": IndexFieldOutputTypeDef,
+        "Options": IndexFieldTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
-DefineIndexFieldRequestRequestTypeDef = TypedDict(
-    "DefineIndexFieldRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "IndexField": IndexFieldTypeDef,
-    },
-)
-
 DescribeScalingParametersResponseTypeDef = TypedDict(
     "DescribeScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateScalingParametersResponseTypeDef = TypedDict(
     "UpdateScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineAnalysisSchemeResponseTypeDef = TypedDict(
     "DefineAnalysisSchemeResponseTypeDef",
     {
         "AnalysisScheme": AnalysisSchemeStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAnalysisSchemeResponseTypeDef = TypedDict(
     "DeleteAnalysisSchemeResponseTypeDef",
     {
         "AnalysisScheme": AnalysisSchemeStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAnalysisSchemesResponseTypeDef = TypedDict(
     "DescribeAnalysisSchemesResponseTypeDef",
     {
         "AnalysisSchemes": List[AnalysisSchemeStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineSuggesterResponseTypeDef = TypedDict(
     "DefineSuggesterResponseTypeDef",
     {
         "Suggester": SuggesterStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSuggesterResponseTypeDef = TypedDict(
     "DeleteSuggesterResponseTypeDef",
     {
         "Suggester": SuggesterStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSuggestersResponseTypeDef = TypedDict(
     "DescribeSuggestersResponseTypeDef",
     {
         "Suggesters": List[SuggesterStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineIndexFieldResponseTypeDef = TypedDict(
     "DefineIndexFieldResponseTypeDef",
     {
         "IndexField": IndexFieldStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteIndexFieldResponseTypeDef = TypedDict(
     "DeleteIndexFieldResponseTypeDef",
     {
         "IndexField": IndexFieldStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIndexFieldsResponseTypeDef = TypedDict(
     "DescribeIndexFieldsResponseTypeDef",
     {
         "IndexFields": List[IndexFieldStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/type_defs.pyi` & `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -28,22 +28,19 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "OptionStatusTypeDef",
-    "AnalysisOptionsOutputTypeDef",
     "AnalysisOptionsTypeDef",
     "BuildSuggestersRequestRequestTypeDef",
-    "BuildSuggestersResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "DateArrayOptionsOutputTypeDef",
     "DateArrayOptionsTypeDef",
-    "DateOptionsOutputTypeDef",
     "DateOptionsTypeDef",
     "ExpressionTypeDef",
     "DeleteAnalysisSchemeRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteExpressionRequestRequestTypeDef",
     "DeleteIndexFieldRequestRequestTypeDef",
     "DeleteSuggesterRequestRequestTypeDef",
@@ -52,80 +49,64 @@
     "DescribeDomainEndpointOptionsRequestRequestTypeDef",
     "DescribeDomainsRequestRequestTypeDef",
     "DescribeExpressionsRequestRequestTypeDef",
     "DescribeIndexFieldsRequestRequestTypeDef",
     "DescribeScalingParametersRequestRequestTypeDef",
     "DescribeServiceAccessPoliciesRequestRequestTypeDef",
     "DescribeSuggestersRequestRequestTypeDef",
-    "DocumentSuggesterOptionsOutputTypeDef",
     "DocumentSuggesterOptionsTypeDef",
-    "DomainEndpointOptionsOutputTypeDef",
     "DomainEndpointOptionsTypeDef",
     "LimitsTypeDef",
     "ServiceEndpointTypeDef",
-    "DoubleArrayOptionsOutputTypeDef",
     "DoubleArrayOptionsTypeDef",
-    "DoubleOptionsOutputTypeDef",
     "DoubleOptionsTypeDef",
-    "ExpressionOutputTypeDef",
     "IndexDocumentsRequestRequestTypeDef",
-    "IndexDocumentsResponseTypeDef",
-    "IntArrayOptionsOutputTypeDef",
-    "IntOptionsOutputTypeDef",
-    "LatLonOptionsOutputTypeDef",
-    "LiteralArrayOptionsOutputTypeDef",
-    "LiteralOptionsOutputTypeDef",
-    "TextArrayOptionsOutputTypeDef",
-    "TextOptionsOutputTypeDef",
     "IntArrayOptionsTypeDef",
     "IntOptionsTypeDef",
     "LatLonOptionsTypeDef",
     "LiteralArrayOptionsTypeDef",
     "LiteralOptionsTypeDef",
     "TextArrayOptionsTypeDef",
     "TextOptionsTypeDef",
-    "ListDomainNamesResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "ScalingParametersOutputTypeDef",
     "ScalingParametersTypeDef",
     "UpdateAvailabilityOptionsRequestRequestTypeDef",
     "UpdateServiceAccessPoliciesRequestRequestTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AvailabilityOptionsStatusTypeDef",
-    "AnalysisSchemeOutputTypeDef",
     "AnalysisSchemeTypeDef",
+    "BuildSuggestersResponseTypeDef",
+    "IndexDocumentsResponseTypeDef",
+    "ListDomainNamesResponseTypeDef",
     "DefineExpressionRequestRequestTypeDef",
-    "SuggesterOutputTypeDef",
+    "ExpressionStatusTypeDef",
     "SuggesterTypeDef",
     "DomainEndpointOptionsStatusTypeDef",
     "UpdateDomainEndpointOptionsRequestRequestTypeDef",
     "DomainStatusTypeDef",
-    "ExpressionStatusTypeDef",
-    "IndexFieldOutputTypeDef",
     "IndexFieldTypeDef",
     "ScalingParametersStatusTypeDef",
     "UpdateScalingParametersRequestRequestTypeDef",
     "DescribeServiceAccessPoliciesResponseTypeDef",
     "UpdateServiceAccessPoliciesResponseTypeDef",
     "DescribeAvailabilityOptionsResponseTypeDef",
     "UpdateAvailabilityOptionsResponseTypeDef",
     "AnalysisSchemeStatusTypeDef",
     "DefineAnalysisSchemeRequestRequestTypeDef",
-    "SuggesterStatusTypeDef",
+    "DefineExpressionResponseTypeDef",
+    "DeleteExpressionResponseTypeDef",
+    "DescribeExpressionsResponseTypeDef",
     "DefineSuggesterRequestRequestTypeDef",
+    "SuggesterStatusTypeDef",
     "DescribeDomainEndpointOptionsResponseTypeDef",
     "UpdateDomainEndpointOptionsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DeleteDomainResponseTypeDef",
     "DescribeDomainsResponseTypeDef",
-    "DefineExpressionResponseTypeDef",
-    "DeleteExpressionResponseTypeDef",
-    "DescribeExpressionsResponseTypeDef",
-    "IndexFieldStatusTypeDef",
     "DefineIndexFieldRequestRequestTypeDef",
+    "IndexFieldStatusTypeDef",
     "DescribeScalingParametersResponseTypeDef",
     "UpdateScalingParametersResponseTypeDef",
     "DefineAnalysisSchemeResponseTypeDef",
     "DeleteAnalysisSchemeResponseTypeDef",
     "DescribeAnalysisSchemesResponseTypeDef",
     "DefineSuggesterResponseTypeDef",
     "DeleteSuggesterResponseTypeDef",
@@ -151,26 +132,14 @@
     },
     total=False,
 )
 
 class OptionStatusTypeDef(_RequiredOptionStatusTypeDef, _OptionalOptionStatusTypeDef):
     pass
 
-AnalysisOptionsOutputTypeDef = TypedDict(
-    "AnalysisOptionsOutputTypeDef",
-    {
-        "Synonyms": str,
-        "Stopwords": str,
-        "StemmingDictionary": str,
-        "JapaneseTokenizationDictionary": str,
-        "AlgorithmicStemming": AlgorithmicStemmingType,
-    },
-    total=False,
-)
-
 AnalysisOptionsTypeDef = TypedDict(
     "AnalysisOptionsTypeDef",
     {
         "Synonyms": str,
         "Stopwords": str,
         "StemmingDictionary": str,
         "JapaneseTokenizationDictionary": str,
@@ -182,66 +151,44 @@
 BuildSuggestersRequestRequestTypeDef = TypedDict(
     "BuildSuggestersRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-BuildSuggestersResponseTypeDef = TypedDict(
-    "BuildSuggestersResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FieldNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DateArrayOptionsOutputTypeDef = TypedDict(
-    "DateArrayOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceFields": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-    },
-    total=False,
-)
-
 DateArrayOptionsTypeDef = TypedDict(
     "DateArrayOptionsTypeDef",
     {
         "DefaultValue": str,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
         "ReturnEnabled": bool,
     },
     total=False,
 )
 
-DateOptionsOutputTypeDef = TypedDict(
-    "DateOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceField": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-        "SortEnabled": bool,
-    },
-    total=False,
-)
-
 DateOptionsTypeDef = TypedDict(
     "DateOptionsTypeDef",
     {
         "DefaultValue": str,
         "SourceField": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
@@ -453,34 +400,14 @@
 
 class DescribeSuggestersRequestRequestTypeDef(
     _RequiredDescribeSuggestersRequestRequestTypeDef,
     _OptionalDescribeSuggestersRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDocumentSuggesterOptionsOutputTypeDef = TypedDict(
-    "_RequiredDocumentSuggesterOptionsOutputTypeDef",
-    {
-        "SourceField": str,
-    },
-)
-_OptionalDocumentSuggesterOptionsOutputTypeDef = TypedDict(
-    "_OptionalDocumentSuggesterOptionsOutputTypeDef",
-    {
-        "FuzzyMatching": SuggesterFuzzyMatchingType,
-        "SortExpression": str,
-    },
-    total=False,
-)
-
-class DocumentSuggesterOptionsOutputTypeDef(
-    _RequiredDocumentSuggesterOptionsOutputTypeDef, _OptionalDocumentSuggesterOptionsOutputTypeDef
-):
-    pass
-
 _RequiredDocumentSuggesterOptionsTypeDef = TypedDict(
     "_RequiredDocumentSuggesterOptionsTypeDef",
     {
         "SourceField": str,
     },
 )
 _OptionalDocumentSuggesterOptionsTypeDef = TypedDict(
@@ -493,23 +420,14 @@
 )
 
 class DocumentSuggesterOptionsTypeDef(
     _RequiredDocumentSuggesterOptionsTypeDef, _OptionalDocumentSuggesterOptionsTypeDef
 ):
     pass
 
-DomainEndpointOptionsOutputTypeDef = TypedDict(
-    "DomainEndpointOptionsOutputTypeDef",
-    {
-        "EnforceHTTPS": bool,
-        "TLSSecurityPolicy": TLSSecurityPolicyType,
-    },
-    total=False,
-)
-
 DomainEndpointOptionsTypeDef = TypedDict(
     "DomainEndpointOptionsTypeDef",
     {
         "EnforceHTTPS": bool,
         "TLSSecurityPolicy": TLSSecurityPolicyType,
     },
     total=False,
@@ -527,175 +445,46 @@
     "ServiceEndpointTypeDef",
     {
         "Endpoint": str,
     },
     total=False,
 )
 
-DoubleArrayOptionsOutputTypeDef = TypedDict(
-    "DoubleArrayOptionsOutputTypeDef",
-    {
-        "DefaultValue": float,
-        "SourceFields": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-    },
-    total=False,
-)
-
 DoubleArrayOptionsTypeDef = TypedDict(
     "DoubleArrayOptionsTypeDef",
     {
         "DefaultValue": float,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
         "ReturnEnabled": bool,
     },
     total=False,
 )
 
-DoubleOptionsOutputTypeDef = TypedDict(
-    "DoubleOptionsOutputTypeDef",
-    {
-        "DefaultValue": float,
-        "SourceField": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-        "SortEnabled": bool,
-    },
-    total=False,
-)
-
 DoubleOptionsTypeDef = TypedDict(
     "DoubleOptionsTypeDef",
     {
         "DefaultValue": float,
         "SourceField": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
         "ReturnEnabled": bool,
         "SortEnabled": bool,
     },
     total=False,
 )
 
-ExpressionOutputTypeDef = TypedDict(
-    "ExpressionOutputTypeDef",
-    {
-        "ExpressionName": str,
-        "ExpressionValue": str,
-    },
-)
-
 IndexDocumentsRequestRequestTypeDef = TypedDict(
     "IndexDocumentsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-IndexDocumentsResponseTypeDef = TypedDict(
-    "IndexDocumentsResponseTypeDef",
-    {
-        "FieldNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IntArrayOptionsOutputTypeDef = TypedDict(
-    "IntArrayOptionsOutputTypeDef",
-    {
-        "DefaultValue": int,
-        "SourceFields": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-    },
-    total=False,
-)
-
-IntOptionsOutputTypeDef = TypedDict(
-    "IntOptionsOutputTypeDef",
-    {
-        "DefaultValue": int,
-        "SourceField": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-        "SortEnabled": bool,
-    },
-    total=False,
-)
-
-LatLonOptionsOutputTypeDef = TypedDict(
-    "LatLonOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceField": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-        "SortEnabled": bool,
-    },
-    total=False,
-)
-
-LiteralArrayOptionsOutputTypeDef = TypedDict(
-    "LiteralArrayOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceFields": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-    },
-    total=False,
-)
-
-LiteralOptionsOutputTypeDef = TypedDict(
-    "LiteralOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceField": str,
-        "FacetEnabled": bool,
-        "SearchEnabled": bool,
-        "ReturnEnabled": bool,
-        "SortEnabled": bool,
-    },
-    total=False,
-)
-
-TextArrayOptionsOutputTypeDef = TypedDict(
-    "TextArrayOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceFields": str,
-        "ReturnEnabled": bool,
-        "HighlightEnabled": bool,
-        "AnalysisScheme": str,
-    },
-    total=False,
-)
-
-TextOptionsOutputTypeDef = TypedDict(
-    "TextOptionsOutputTypeDef",
-    {
-        "DefaultValue": str,
-        "SourceField": str,
-        "ReturnEnabled": bool,
-        "SortEnabled": bool,
-        "HighlightEnabled": bool,
-        "AnalysisScheme": str,
-    },
-    total=False,
-)
-
 IntArrayOptionsTypeDef = TypedDict(
     "IntArrayOptionsTypeDef",
     {
         "DefaultValue": int,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
@@ -776,43 +565,14 @@
         "SortEnabled": bool,
         "HighlightEnabled": bool,
         "AnalysisScheme": str,
     },
     total=False,
 )
 
-ListDomainNamesResponseTypeDef = TypedDict(
-    "ListDomainNamesResponseTypeDef",
-    {
-        "DomainNames": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
-ScalingParametersOutputTypeDef = TypedDict(
-    "ScalingParametersOutputTypeDef",
-    {
-        "DesiredInstanceType": PartitionInstanceTypeType,
-        "DesiredReplicationCount": int,
-        "DesiredPartitionCount": int,
-    },
-    total=False,
-)
-
 ScalingParametersTypeDef = TypedDict(
     "ScalingParametersTypeDef",
     {
         "DesiredInstanceType": PartitionInstanceTypeType,
         "DesiredReplicationCount": int,
         "DesiredPartitionCount": int,
     },
@@ -847,80 +607,84 @@
     "AvailabilityOptionsStatusTypeDef",
     {
         "Options": bool,
         "Status": OptionStatusTypeDef,
     },
 )
 
-_RequiredAnalysisSchemeOutputTypeDef = TypedDict(
-    "_RequiredAnalysisSchemeOutputTypeDef",
+_RequiredAnalysisSchemeTypeDef = TypedDict(
+    "_RequiredAnalysisSchemeTypeDef",
     {
         "AnalysisSchemeName": str,
         "AnalysisSchemeLanguage": AnalysisSchemeLanguageType,
     },
 )
-_OptionalAnalysisSchemeOutputTypeDef = TypedDict(
-    "_OptionalAnalysisSchemeOutputTypeDef",
+_OptionalAnalysisSchemeTypeDef = TypedDict(
+    "_OptionalAnalysisSchemeTypeDef",
     {
-        "AnalysisOptions": AnalysisOptionsOutputTypeDef,
+        "AnalysisOptions": AnalysisOptionsTypeDef,
     },
     total=False,
 )
 
-class AnalysisSchemeOutputTypeDef(
-    _RequiredAnalysisSchemeOutputTypeDef, _OptionalAnalysisSchemeOutputTypeDef
-):
+class AnalysisSchemeTypeDef(_RequiredAnalysisSchemeTypeDef, _OptionalAnalysisSchemeTypeDef):
     pass
 
-_RequiredAnalysisSchemeTypeDef = TypedDict(
-    "_RequiredAnalysisSchemeTypeDef",
+BuildSuggestersResponseTypeDef = TypedDict(
+    "BuildSuggestersResponseTypeDef",
     {
-        "AnalysisSchemeName": str,
-        "AnalysisSchemeLanguage": AnalysisSchemeLanguageType,
+        "FieldNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAnalysisSchemeTypeDef = TypedDict(
-    "_OptionalAnalysisSchemeTypeDef",
+
+IndexDocumentsResponseTypeDef = TypedDict(
+    "IndexDocumentsResponseTypeDef",
     {
-        "AnalysisOptions": AnalysisOptionsTypeDef,
+        "FieldNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class AnalysisSchemeTypeDef(_RequiredAnalysisSchemeTypeDef, _OptionalAnalysisSchemeTypeDef):
-    pass
+ListDomainNamesResponseTypeDef = TypedDict(
+    "ListDomainNamesResponseTypeDef",
+    {
+        "DomainNames": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 DefineExpressionRequestRequestTypeDef = TypedDict(
     "DefineExpressionRequestRequestTypeDef",
     {
         "DomainName": str,
         "Expression": ExpressionTypeDef,
     },
 )
 
-SuggesterOutputTypeDef = TypedDict(
-    "SuggesterOutputTypeDef",
+ExpressionStatusTypeDef = TypedDict(
+    "ExpressionStatusTypeDef",
     {
-        "SuggesterName": str,
-        "DocumentSuggesterOptions": DocumentSuggesterOptionsOutputTypeDef,
+        "Options": ExpressionTypeDef,
+        "Status": OptionStatusTypeDef,
     },
 )
 
 SuggesterTypeDef = TypedDict(
     "SuggesterTypeDef",
     {
         "SuggesterName": str,
         "DocumentSuggesterOptions": DocumentSuggesterOptionsTypeDef,
     },
 )
 
 DomainEndpointOptionsStatusTypeDef = TypedDict(
     "DomainEndpointOptionsStatusTypeDef",
     {
-        "Options": DomainEndpointOptionsOutputTypeDef,
+        "Options": DomainEndpointOptionsTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 UpdateDomainEndpointOptionsRequestRequestTypeDef = TypedDict(
     "UpdateDomainEndpointOptionsRequestRequestTypeDef",
     {
@@ -953,50 +717,14 @@
     },
     total=False,
 )
 
 class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
     pass
 
-ExpressionStatusTypeDef = TypedDict(
-    "ExpressionStatusTypeDef",
-    {
-        "Options": ExpressionOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-_RequiredIndexFieldOutputTypeDef = TypedDict(
-    "_RequiredIndexFieldOutputTypeDef",
-    {
-        "IndexFieldName": str,
-        "IndexFieldType": IndexFieldTypeType,
-    },
-)
-_OptionalIndexFieldOutputTypeDef = TypedDict(
-    "_OptionalIndexFieldOutputTypeDef",
-    {
-        "IntOptions": IntOptionsOutputTypeDef,
-        "DoubleOptions": DoubleOptionsOutputTypeDef,
-        "LiteralOptions": LiteralOptionsOutputTypeDef,
-        "TextOptions": TextOptionsOutputTypeDef,
-        "DateOptions": DateOptionsOutputTypeDef,
-        "LatLonOptions": LatLonOptionsOutputTypeDef,
-        "IntArrayOptions": IntArrayOptionsOutputTypeDef,
-        "DoubleArrayOptions": DoubleArrayOptionsOutputTypeDef,
-        "LiteralArrayOptions": LiteralArrayOptionsOutputTypeDef,
-        "TextArrayOptions": TextArrayOptionsOutputTypeDef,
-        "DateArrayOptions": DateArrayOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-class IndexFieldOutputTypeDef(_RequiredIndexFieldOutputTypeDef, _OptionalIndexFieldOutputTypeDef):
-    pass
-
 _RequiredIndexFieldTypeDef = TypedDict(
     "_RequiredIndexFieldTypeDef",
     {
         "IndexFieldName": str,
         "IndexFieldType": IndexFieldTypeType,
     },
 )
@@ -1020,15 +748,15 @@
 
 class IndexFieldTypeDef(_RequiredIndexFieldTypeDef, _OptionalIndexFieldTypeDef):
     pass
 
 ScalingParametersStatusTypeDef = TypedDict(
     "ScalingParametersStatusTypeDef",
     {
-        "Options": ScalingParametersOutputTypeDef,
+        "Options": ScalingParametersTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 UpdateScalingParametersRequestRequestTypeDef = TypedDict(
     "UpdateScalingParametersRequestRequestTypeDef",
     {
@@ -1037,234 +765,234 @@
     },
 )
 
 DescribeServiceAccessPoliciesResponseTypeDef = TypedDict(
     "DescribeServiceAccessPoliciesResponseTypeDef",
     {
         "AccessPolicies": AccessPoliciesStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceAccessPoliciesResponseTypeDef = TypedDict(
     "UpdateServiceAccessPoliciesResponseTypeDef",
     {
         "AccessPolicies": AccessPoliciesStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAvailabilityOptionsResponseTypeDef = TypedDict(
     "DescribeAvailabilityOptionsResponseTypeDef",
     {
         "AvailabilityOptions": AvailabilityOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAvailabilityOptionsResponseTypeDef = TypedDict(
     "UpdateAvailabilityOptionsResponseTypeDef",
     {
         "AvailabilityOptions": AvailabilityOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AnalysisSchemeStatusTypeDef = TypedDict(
     "AnalysisSchemeStatusTypeDef",
     {
-        "Options": AnalysisSchemeOutputTypeDef,
+        "Options": AnalysisSchemeTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 DefineAnalysisSchemeRequestRequestTypeDef = TypedDict(
     "DefineAnalysisSchemeRequestRequestTypeDef",
     {
         "DomainName": str,
         "AnalysisScheme": AnalysisSchemeTypeDef,
     },
 )
 
-SuggesterStatusTypeDef = TypedDict(
-    "SuggesterStatusTypeDef",
+DefineExpressionResponseTypeDef = TypedDict(
+    "DefineExpressionResponseTypeDef",
     {
-        "Options": SuggesterOutputTypeDef,
-        "Status": OptionStatusTypeDef,
+        "Expression": ExpressionStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteExpressionResponseTypeDef = TypedDict(
+    "DeleteExpressionResponseTypeDef",
+    {
+        "Expression": ExpressionStatusTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeExpressionsResponseTypeDef = TypedDict(
+    "DescribeExpressionsResponseTypeDef",
+    {
+        "Expressions": List[ExpressionStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineSuggesterRequestRequestTypeDef = TypedDict(
     "DefineSuggesterRequestRequestTypeDef",
     {
         "DomainName": str,
         "Suggester": SuggesterTypeDef,
     },
 )
 
+SuggesterStatusTypeDef = TypedDict(
+    "SuggesterStatusTypeDef",
+    {
+        "Options": SuggesterTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
 DescribeDomainEndpointOptionsResponseTypeDef = TypedDict(
     "DescribeDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainEndpointOptionsResponseTypeDef = TypedDict(
     "UpdateDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResponseTypeDef = TypedDict(
     "DeleteDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainsResponseTypeDef = TypedDict(
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DefineExpressionResponseTypeDef = TypedDict(
-    "DefineExpressionResponseTypeDef",
-    {
-        "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteExpressionResponseTypeDef = TypedDict(
-    "DeleteExpressionResponseTypeDef",
-    {
-        "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeExpressionsResponseTypeDef = TypedDict(
-    "DescribeExpressionsResponseTypeDef",
+DefineIndexFieldRequestRequestTypeDef = TypedDict(
+    "DefineIndexFieldRequestRequestTypeDef",
     {
-        "Expressions": List[ExpressionStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DomainName": str,
+        "IndexField": IndexFieldTypeDef,
     },
 )
 
 IndexFieldStatusTypeDef = TypedDict(
     "IndexFieldStatusTypeDef",
     {
-        "Options": IndexFieldOutputTypeDef,
+        "Options": IndexFieldTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
-DefineIndexFieldRequestRequestTypeDef = TypedDict(
-    "DefineIndexFieldRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "IndexField": IndexFieldTypeDef,
-    },
-)
-
 DescribeScalingParametersResponseTypeDef = TypedDict(
     "DescribeScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateScalingParametersResponseTypeDef = TypedDict(
     "UpdateScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineAnalysisSchemeResponseTypeDef = TypedDict(
     "DefineAnalysisSchemeResponseTypeDef",
     {
         "AnalysisScheme": AnalysisSchemeStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAnalysisSchemeResponseTypeDef = TypedDict(
     "DeleteAnalysisSchemeResponseTypeDef",
     {
         "AnalysisScheme": AnalysisSchemeStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAnalysisSchemesResponseTypeDef = TypedDict(
     "DescribeAnalysisSchemesResponseTypeDef",
     {
         "AnalysisSchemes": List[AnalysisSchemeStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineSuggesterResponseTypeDef = TypedDict(
     "DefineSuggesterResponseTypeDef",
     {
         "Suggester": SuggesterStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSuggesterResponseTypeDef = TypedDict(
     "DeleteSuggesterResponseTypeDef",
     {
         "Suggester": SuggesterStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSuggestersResponseTypeDef = TypedDict(
     "DescribeSuggestersResponseTypeDef",
     {
         "Suggesters": List[SuggesterStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefineIndexFieldResponseTypeDef = TypedDict(
     "DefineIndexFieldResponseTypeDef",
     {
         "IndexField": IndexFieldStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteIndexFieldResponseTypeDef = TypedDict(
     "DeleteIndexFieldResponseTypeDef",
     {
         "IndexField": IndexFieldStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIndexFieldsResponseTypeDef = TypedDict(
     "DescribeIndexFieldsResponseTypeDef",
     {
         "IndexFields": List[IndexFieldStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/PKG-INFO` & `mypy-boto3-cloudsearch-1.28.15/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudsearch
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudSearch 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudSearch 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudsearch)](https://pepy.tech/project/mypy-boto3-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
+[boto3.CloudSearch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
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
 [mypy-boto3-cloudsearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,22 +303,19 @@
 
 `mypy_boto3_cloudsearch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudsearch.type_defs import (
     OptionStatusTypeDef,
-    AnalysisOptionsOutputTypeDef,
     AnalysisOptionsTypeDef,
     BuildSuggestersRequestRequestTypeDef,
-    BuildSuggestersResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDomainRequestRequestTypeDef,
-    DateArrayOptionsOutputTypeDef,
     DateArrayOptionsTypeDef,
-    DateOptionsOutputTypeDef,
     DateOptionsTypeDef,
     ExpressionTypeDef,
     DeleteAnalysisSchemeRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteExpressionRequestRequestTypeDef,
     DeleteIndexFieldRequestRequestTypeDef,
     DeleteSuggesterRequestRequestTypeDef,
@@ -327,80 +324,64 @@
     DescribeDomainEndpointOptionsRequestRequestTypeDef,
     DescribeDomainsRequestRequestTypeDef,
     DescribeExpressionsRequestRequestTypeDef,
     DescribeIndexFieldsRequestRequestTypeDef,
     DescribeScalingParametersRequestRequestTypeDef,
     DescribeServiceAccessPoliciesRequestRequestTypeDef,
     DescribeSuggestersRequestRequestTypeDef,
-    DocumentSuggesterOptionsOutputTypeDef,
     DocumentSuggesterOptionsTypeDef,
-    DomainEndpointOptionsOutputTypeDef,
     DomainEndpointOptionsTypeDef,
     LimitsTypeDef,
     ServiceEndpointTypeDef,
-    DoubleArrayOptionsOutputTypeDef,
     DoubleArrayOptionsTypeDef,
-    DoubleOptionsOutputTypeDef,
     DoubleOptionsTypeDef,
-    ExpressionOutputTypeDef,
     IndexDocumentsRequestRequestTypeDef,
-    IndexDocumentsResponseTypeDef,
-    IntArrayOptionsOutputTypeDef,
-    IntOptionsOutputTypeDef,
-    LatLonOptionsOutputTypeDef,
-    LiteralArrayOptionsOutputTypeDef,
-    LiteralOptionsOutputTypeDef,
-    TextArrayOptionsOutputTypeDef,
-    TextOptionsOutputTypeDef,
     IntArrayOptionsTypeDef,
     IntOptionsTypeDef,
     LatLonOptionsTypeDef,
     LiteralArrayOptionsTypeDef,
     LiteralOptionsTypeDef,
     TextArrayOptionsTypeDef,
     TextOptionsTypeDef,
-    ListDomainNamesResponseTypeDef,
-    ResponseMetadataTypeDef,
-    ScalingParametersOutputTypeDef,
     ScalingParametersTypeDef,
     UpdateAvailabilityOptionsRequestRequestTypeDef,
     UpdateServiceAccessPoliciesRequestRequestTypeDef,
     AccessPoliciesStatusTypeDef,
     AvailabilityOptionsStatusTypeDef,
-    AnalysisSchemeOutputTypeDef,
     AnalysisSchemeTypeDef,
+    BuildSuggestersResponseTypeDef,
+    IndexDocumentsResponseTypeDef,
+    ListDomainNamesResponseTypeDef,
     DefineExpressionRequestRequestTypeDef,
-    SuggesterOutputTypeDef,
+    ExpressionStatusTypeDef,
     SuggesterTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     UpdateDomainEndpointOptionsRequestRequestTypeDef,
     DomainStatusTypeDef,
-    ExpressionStatusTypeDef,
-    IndexFieldOutputTypeDef,
     IndexFieldTypeDef,
     ScalingParametersStatusTypeDef,
     UpdateScalingParametersRequestRequestTypeDef,
     DescribeServiceAccessPoliciesResponseTypeDef,
     UpdateServiceAccessPoliciesResponseTypeDef,
     DescribeAvailabilityOptionsResponseTypeDef,
     UpdateAvailabilityOptionsResponseTypeDef,
     AnalysisSchemeStatusTypeDef,
     DefineAnalysisSchemeRequestRequestTypeDef,
-    SuggesterStatusTypeDef,
+    DefineExpressionResponseTypeDef,
+    DeleteExpressionResponseTypeDef,
+    DescribeExpressionsResponseTypeDef,
     DefineSuggesterRequestRequestTypeDef,
+    SuggesterStatusTypeDef,
     DescribeDomainEndpointOptionsResponseTypeDef,
     UpdateDomainEndpointOptionsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DescribeDomainsResponseTypeDef,
-    DefineExpressionResponseTypeDef,
-    DeleteExpressionResponseTypeDef,
-    DescribeExpressionsResponseTypeDef,
-    IndexFieldStatusTypeDef,
     DefineIndexFieldRequestRequestTypeDef,
+    IndexFieldStatusTypeDef,
     DescribeScalingParametersResponseTypeDef,
     UpdateScalingParametersResponseTypeDef,
     DefineAnalysisSchemeResponseTypeDef,
     DeleteAnalysisSchemeResponseTypeDef,
     DescribeAnalysisSchemesResponseTypeDef,
     DefineSuggesterResponseTypeDef,
     DeleteSuggesterResponseTypeDef,
```

### Comparing `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/SOURCES.txt` & `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.12/setup.py` & `mypy-boto3-cloudsearch-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudsearch",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cloudsearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudSearch 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CloudSearch 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

