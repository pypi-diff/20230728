# Comparing `tmp/mypy-boto3-clouddirectory-1.28.12.tar.gz` & `tmp/mypy-boto3-clouddirectory-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-clouddirectory-1.28.12.tar", last modified: Thu Jul 27 05:34:25 2023, max compression
+gzip compressed data, was "mypy-boto3-clouddirectory-1.28.15.tar", last modified: Fri Jul 28 20:42:25 2023, max compression
```

## Comparing `mypy-boto3-clouddirectory-1.28.12.tar` & `mypy-boto3-clouddirectory-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.000563 mypy-boto3-clouddirectory-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26363 2023-07-27 05:34:24.992563 mypy-boto3-clouddirectory-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24848 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.992563 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56752 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    56660 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-07-27 05:18:28.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-27 05:18:28.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24367 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    91171 2023-07-27 05:18:30.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    91038 2023-07-27 05:18:29.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.992563 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26363 2023-07-27 05:34:24.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:24.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:24.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:25.000563 mypy-boto3-clouddirectory-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.424781 mypy-boto3-clouddirectory-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26158 2023-07-28 20:42:25.424781 mypy-boto3-clouddirectory-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24643 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.424781 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56752 2023-07-28 20:20:53.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56660 2023-07-28 20:20:53.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-07-28 20:20:54.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-28 20:20:53.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-07-28 20:20:53.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-07-28 20:20:53.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    89831 2023-07-28 20:20:57.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89698 2023-07-28 20:20:55.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.424781 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26158 2023-07-28 20:42:25.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:42:25.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:25.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:42:25.000000 mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:25.424781 mypy-boto3-clouddirectory-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:20:52.000000 mypy-boto3-clouddirectory-1.28.15/setup.py
```

### Comparing `mypy-boto3-clouddirectory-1.28.12/LICENSE` & `mypy-boto3-clouddirectory-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.12/PKG-INFO` & `mypy-boto3-clouddirectory-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-clouddirectory
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudDirectory 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudDirectory 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-clouddirectory)](https://pepy.tech/project/mypy-boto3-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudDirectory 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[boto3.CloudDirectory 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
 
@@ -419,117 +419,69 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_clouddirectory.type_defs import (
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
-    ApplySchemaResponseTypeDef,
-    AttachObjectResponseTypeDef,
-    AttachToIndexResponseTypeDef,
+    ResponseMetadataTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
-    AttributeKeyOutputTypeDef,
-    TypedAttributeValueOutputTypeDef,
     AttributeKeyTypeDef,
+    TypedAttributeValueOutputTypeDef,
     TypedAttributeValueTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
     BatchDetachFromIndexResponseTypeDef,
     BatchDetachObjectResponseTypeDef,
-    SchemaFacetOutputTypeDef,
     BatchListObjectChildrenResponseTypeDef,
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
     CreateDirectoryRequestRequestTypeDef,
-    CreateDirectoryResponseTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateObjectResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
-    DeleteDirectoryResponseTypeDef,
     DeleteFacetRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
-    DeleteSchemaResponseTypeDef,
     DeleteTypedLinkFacetRequestRequestTypeDef,
-    DetachFromIndexResponseTypeDef,
-    DetachObjectResponseTypeDef,
     DirectoryTypeDef,
     DisableDirectoryRequestRequestTypeDef,
-    DisableDirectoryResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableDirectoryRequestRequestTypeDef,
-    EnableDirectoryResponseTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
-    FacetAttributeReferenceOutputTypeDef,
     FacetAttributeReferenceTypeDef,
     FacetTypeDef,
     GetAppliedSchemaVersionRequestRequestTypeDef,
-    GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryRequestRequestTypeDef,
     GetFacetRequestRequestTypeDef,
     GetSchemaAsJsonRequestRequestTypeDef,
-    GetSchemaAsJsonResponseTypeDef,
     GetTypedLinkFacetInformationRequestRequestTypeDef,
-    GetTypedLinkFacetInformationResponseTypeDef,
-    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAppliedSchemaArnsRequestRequestTypeDef,
-    ListAppliedSchemaArnsResponseTypeDef,
-    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
     ListDevelopmentSchemaArnsRequestRequestTypeDef,
-    ListDevelopmentSchemaArnsResponseTypeDef,
-    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
     ListDirectoriesRequestRequestTypeDef,
-    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
     ListFacetAttributesRequestRequestTypeDef,
-    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
     ListFacetNamesRequestRequestTypeDef,
-    ListFacetNamesResponseTypeDef,
-    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
     ListManagedSchemaArnsRequestRequestTypeDef,
-    ListManagedSchemaArnsResponseTypeDef,
-    ListObjectChildrenResponseTypeDef,
-    ListObjectPoliciesResponseTypeDef,
-    ListPolicyAttachmentsResponseTypeDef,
-    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
     ListPublishedSchemaArnsRequestRequestTypeDef,
-    ListPublishedSchemaArnsResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    TagTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
-    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
-    ListTypedLinkFacetNamesResponseTypeDef,
-    ObjectReferenceOutputTypeDef,
-    PaginatorConfigTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
-    PublishSchemaResponseTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
-    PutSchemaFromJsonResponseTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
-    TypedLinkSchemaAndFacetNameOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
-    UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
-    UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
-    UpgradePublishedSchemaResponseTypeDef,
     AttachObjectRequestRequestTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachToIndexRequestRequestTypeDef,
     BatchAttachObjectTypeDef,
     BatchAttachPolicyTypeDef,
     BatchAttachToIndexTypeDef,
     BatchDeleteObjectTypeDef,
@@ -545,58 +497,100 @@
     BatchListPolicyAttachmentsTypeDef,
     BatchLookupPolicyTypeDef,
     DeleteObjectRequestRequestTypeDef,
     DetachFromIndexRequestRequestTypeDef,
     DetachObjectRequestRequestTypeDef,
     DetachPolicyRequestRequestTypeDef,
     GetObjectInformationRequestRequestTypeDef,
-    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
     ListAttachedIndicesRequestRequestTypeDef,
     ListObjectChildrenRequestRequestTypeDef,
-    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
     ListObjectParentPathsRequestRequestTypeDef,
     ListObjectParentsRequestRequestTypeDef,
-    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
     ListObjectPoliciesRequestRequestTypeDef,
-    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
     ListPolicyAttachmentsRequestRequestTypeDef,
-    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     LookupPolicyRequestRequestTypeDef,
     BatchGetObjectAttributesTypeDef,
+    BatchGetObjectInformationResponseTypeDef,
     BatchListObjectAttributesTypeDef,
     BatchRemoveFacetFromObjectTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
-    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
     ListObjectAttributesRequestRequestTypeDef,
     RemoveFacetFromObjectRequestRequestTypeDef,
-    AttributeKeyAndValueOutputTypeDef,
-    AttributeNameAndValueOutputTypeDef,
+    ApplySchemaResponseTypeDef,
+    AttachObjectResponseTypeDef,
+    AttachToIndexResponseTypeDef,
+    CreateDirectoryResponseTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateObjectResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    DeleteDirectoryResponseTypeDef,
+    DeleteSchemaResponseTypeDef,
+    DetachFromIndexResponseTypeDef,
+    DetachObjectResponseTypeDef,
+    DisableDirectoryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnableDirectoryResponseTypeDef,
+    GetAppliedSchemaVersionResponseTypeDef,
+    GetObjectInformationResponseTypeDef,
+    GetSchemaAsJsonResponseTypeDef,
+    GetTypedLinkFacetInformationResponseTypeDef,
+    ListAppliedSchemaArnsResponseTypeDef,
+    ListDevelopmentSchemaArnsResponseTypeDef,
+    ListFacetNamesResponseTypeDef,
+    ListManagedSchemaArnsResponseTypeDef,
+    ListObjectChildrenResponseTypeDef,
+    ListObjectPoliciesResponseTypeDef,
+    ListPolicyAttachmentsResponseTypeDef,
+    ListPublishedSchemaArnsResponseTypeDef,
+    ListTypedLinkFacetNamesResponseTypeDef,
+    PublishSchemaResponseTypeDef,
+    PutSchemaFromJsonResponseTypeDef,
+    UpdateObjectAttributesResponseTypeDef,
+    UpdateSchemaResponseTypeDef,
+    UpgradeAppliedSchemaResponseTypeDef,
+    UpgradePublishedSchemaResponseTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
+    AttributeKeyAndValueOutputTypeDef,
+    AttributeNameAndValueOutputTypeDef,
     AttributeKeyAndValueTypeDef,
     AttributeNameAndValueTypeDef,
     LinkAttributeActionTypeDef,
     ObjectAttributeActionTypeDef,
     TypedAttributeValueRangeTypeDef,
-    BatchGetObjectInformationResponseTypeDef,
-    GetObjectInformationResponseTypeDef,
     BatchListObjectParentPathsResponseTypeDef,
     ListObjectParentPathsResponseTypeDef,
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
     FacetAttributeDefinitionOutputTypeDef,
     TypedLinkAttributeDefinitionOutputTypeDef,
     FacetAttributeDefinitionTypeDef,
     TypedLinkAttributeDefinitionTypeDef,
     GetFacetResponseTypeDef,
+    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
+    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
+    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
+    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
+    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PolicyToPathTypeDef,
     TagResourceRequestRequestTypeDef,
+    PolicyToPathTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
     BatchGetObjectAttributesResponseTypeDef,
     BatchListObjectAttributesResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     IndexAttachmentTypeDef,
     ListObjectAttributesResponseTypeDef,
```

### Comparing `mypy-boto3-clouddirectory-1.28.12/README.md` & `mypy-boto3-clouddirectory-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-clouddirectory)](https://pepy.tech/project/mypy-boto3-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudDirectory 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[boto3.CloudDirectory 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
 
@@ -387,117 +387,69 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_clouddirectory.type_defs import (
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
-    ApplySchemaResponseTypeDef,
-    AttachObjectResponseTypeDef,
-    AttachToIndexResponseTypeDef,
+    ResponseMetadataTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
-    AttributeKeyOutputTypeDef,
-    TypedAttributeValueOutputTypeDef,
     AttributeKeyTypeDef,
+    TypedAttributeValueOutputTypeDef,
     TypedAttributeValueTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
     BatchDetachFromIndexResponseTypeDef,
     BatchDetachObjectResponseTypeDef,
-    SchemaFacetOutputTypeDef,
     BatchListObjectChildrenResponseTypeDef,
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
     CreateDirectoryRequestRequestTypeDef,
-    CreateDirectoryResponseTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateObjectResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
-    DeleteDirectoryResponseTypeDef,
     DeleteFacetRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
-    DeleteSchemaResponseTypeDef,
     DeleteTypedLinkFacetRequestRequestTypeDef,
-    DetachFromIndexResponseTypeDef,
-    DetachObjectResponseTypeDef,
     DirectoryTypeDef,
     DisableDirectoryRequestRequestTypeDef,
-    DisableDirectoryResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableDirectoryRequestRequestTypeDef,
-    EnableDirectoryResponseTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
-    FacetAttributeReferenceOutputTypeDef,
     FacetAttributeReferenceTypeDef,
     FacetTypeDef,
     GetAppliedSchemaVersionRequestRequestTypeDef,
-    GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryRequestRequestTypeDef,
     GetFacetRequestRequestTypeDef,
     GetSchemaAsJsonRequestRequestTypeDef,
-    GetSchemaAsJsonResponseTypeDef,
     GetTypedLinkFacetInformationRequestRequestTypeDef,
-    GetTypedLinkFacetInformationResponseTypeDef,
-    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAppliedSchemaArnsRequestRequestTypeDef,
-    ListAppliedSchemaArnsResponseTypeDef,
-    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
     ListDevelopmentSchemaArnsRequestRequestTypeDef,
-    ListDevelopmentSchemaArnsResponseTypeDef,
-    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
     ListDirectoriesRequestRequestTypeDef,
-    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
     ListFacetAttributesRequestRequestTypeDef,
-    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
     ListFacetNamesRequestRequestTypeDef,
-    ListFacetNamesResponseTypeDef,
-    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
     ListManagedSchemaArnsRequestRequestTypeDef,
-    ListManagedSchemaArnsResponseTypeDef,
-    ListObjectChildrenResponseTypeDef,
-    ListObjectPoliciesResponseTypeDef,
-    ListPolicyAttachmentsResponseTypeDef,
-    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
     ListPublishedSchemaArnsRequestRequestTypeDef,
-    ListPublishedSchemaArnsResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    TagTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
-    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
-    ListTypedLinkFacetNamesResponseTypeDef,
-    ObjectReferenceOutputTypeDef,
-    PaginatorConfigTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
-    PublishSchemaResponseTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
-    PutSchemaFromJsonResponseTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
-    TypedLinkSchemaAndFacetNameOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
-    UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
-    UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
-    UpgradePublishedSchemaResponseTypeDef,
     AttachObjectRequestRequestTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachToIndexRequestRequestTypeDef,
     BatchAttachObjectTypeDef,
     BatchAttachPolicyTypeDef,
     BatchAttachToIndexTypeDef,
     BatchDeleteObjectTypeDef,
@@ -513,58 +465,100 @@
     BatchListPolicyAttachmentsTypeDef,
     BatchLookupPolicyTypeDef,
     DeleteObjectRequestRequestTypeDef,
     DetachFromIndexRequestRequestTypeDef,
     DetachObjectRequestRequestTypeDef,
     DetachPolicyRequestRequestTypeDef,
     GetObjectInformationRequestRequestTypeDef,
-    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
     ListAttachedIndicesRequestRequestTypeDef,
     ListObjectChildrenRequestRequestTypeDef,
-    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
     ListObjectParentPathsRequestRequestTypeDef,
     ListObjectParentsRequestRequestTypeDef,
-    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
     ListObjectPoliciesRequestRequestTypeDef,
-    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
     ListPolicyAttachmentsRequestRequestTypeDef,
-    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     LookupPolicyRequestRequestTypeDef,
     BatchGetObjectAttributesTypeDef,
+    BatchGetObjectInformationResponseTypeDef,
     BatchListObjectAttributesTypeDef,
     BatchRemoveFacetFromObjectTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
-    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
     ListObjectAttributesRequestRequestTypeDef,
     RemoveFacetFromObjectRequestRequestTypeDef,
-    AttributeKeyAndValueOutputTypeDef,
-    AttributeNameAndValueOutputTypeDef,
+    ApplySchemaResponseTypeDef,
+    AttachObjectResponseTypeDef,
+    AttachToIndexResponseTypeDef,
+    CreateDirectoryResponseTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateObjectResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    DeleteDirectoryResponseTypeDef,
+    DeleteSchemaResponseTypeDef,
+    DetachFromIndexResponseTypeDef,
+    DetachObjectResponseTypeDef,
+    DisableDirectoryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnableDirectoryResponseTypeDef,
+    GetAppliedSchemaVersionResponseTypeDef,
+    GetObjectInformationResponseTypeDef,
+    GetSchemaAsJsonResponseTypeDef,
+    GetTypedLinkFacetInformationResponseTypeDef,
+    ListAppliedSchemaArnsResponseTypeDef,
+    ListDevelopmentSchemaArnsResponseTypeDef,
+    ListFacetNamesResponseTypeDef,
+    ListManagedSchemaArnsResponseTypeDef,
+    ListObjectChildrenResponseTypeDef,
+    ListObjectPoliciesResponseTypeDef,
+    ListPolicyAttachmentsResponseTypeDef,
+    ListPublishedSchemaArnsResponseTypeDef,
+    ListTypedLinkFacetNamesResponseTypeDef,
+    PublishSchemaResponseTypeDef,
+    PutSchemaFromJsonResponseTypeDef,
+    UpdateObjectAttributesResponseTypeDef,
+    UpdateSchemaResponseTypeDef,
+    UpgradeAppliedSchemaResponseTypeDef,
+    UpgradePublishedSchemaResponseTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
+    AttributeKeyAndValueOutputTypeDef,
+    AttributeNameAndValueOutputTypeDef,
     AttributeKeyAndValueTypeDef,
     AttributeNameAndValueTypeDef,
     LinkAttributeActionTypeDef,
     ObjectAttributeActionTypeDef,
     TypedAttributeValueRangeTypeDef,
-    BatchGetObjectInformationResponseTypeDef,
-    GetObjectInformationResponseTypeDef,
     BatchListObjectParentPathsResponseTypeDef,
     ListObjectParentPathsResponseTypeDef,
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
     FacetAttributeDefinitionOutputTypeDef,
     TypedLinkAttributeDefinitionOutputTypeDef,
     FacetAttributeDefinitionTypeDef,
     TypedLinkAttributeDefinitionTypeDef,
     GetFacetResponseTypeDef,
+    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
+    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
+    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
+    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
+    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PolicyToPathTypeDef,
     TagResourceRequestRequestTypeDef,
+    PolicyToPathTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
     BatchGetObjectAttributesResponseTypeDef,
     BatchListObjectAttributesResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     IndexAttachmentTypeDef,
     ListObjectAttributesResponseTypeDef,
```

### Comparing `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/__init__.py` & `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/__init__.pyi` & `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/__main__.py` & `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudDirectory 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CloudDirectory 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory\nOther"
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

### Comparing `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/client.py` & `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/client.pyi` & `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/literals.py` & `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/literals.pyi` & `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/paginator.py` & `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         SchemaArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAppliedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAppliedSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listappliedschemaarnspaginator)
         """
 
 
@@ -148,75 +148,75 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         TargetReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttachedIndicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAttachedIndices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listattachedindicespaginator)
         """
 
 
 class ListDevelopmentSchemaArnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdevelopmentschemaarnspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevelopmentSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdevelopmentschemaarnspaginator)
         """
 
 
 class ListDirectoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDirectories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdirectoriespaginator)
     """
 
     def paginate(
-        self, *, state: DirectoryStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, state: DirectoryStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDirectoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDirectories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdirectoriespaginator)
         """
 
 
 class ListFacetAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetattributespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFacetAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetattributespaginator)
         """
 
 
 class ListFacetNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetnamespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFacetNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetnamespaginator)
         """
 
 
@@ -230,15 +230,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIncomingTypedLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIncomingTypedLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listincomingtypedlinkspaginator)
         """
 
 
@@ -251,30 +251,30 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
         RangesOnIndexedValues: Sequence[ObjectAttributeRangeTypeDef] = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIndexResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIndex.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listindexpaginator)
         """
 
 
 class ListManagedSchemaArnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListManagedSchemaArns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listmanagedschemaarnspaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListManagedSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listmanagedschemaarnspaginator)
         """
 
 
@@ -287,15 +287,15 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
         FacetFilter: SchemaFacetTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listobjectattributespaginator)
         """
 
 
@@ -306,15 +306,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectParentPathsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectParentPaths.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listobjectparentpathspaginator)
         """
 
 
@@ -326,15 +326,15 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listobjectpoliciespaginator)
         """
 
 
@@ -348,15 +348,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOutgoingTypedLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListOutgoingTypedLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listoutgoingtypedlinkspaginator)
         """
 
 
@@ -368,75 +368,75 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPolicyAttachmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPolicyAttachments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listpolicyattachmentspaginator)
         """
 
 
 class ListPublishedSchemaArnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPublishedSchemaArns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listpublishedschemaarnspaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPublishedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPublishedSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listpublishedschemaarnspaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListTypedLinkFacetAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetattributespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTypedLinkFacetAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetattributespaginator)
         """
 
 
 class ListTypedLinkFacetNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetnamespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTypedLinkFacetNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetnamespaginator)
         """
 
 
@@ -447,13 +447,13 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[LookupPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.LookupPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#lookuppolicypaginator)
         """
```

### Comparing `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/paginator.pyi` & `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         SchemaArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAppliedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAppliedSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listappliedschemaarnspaginator)
         """
 
 class ListAttachedIndicesPaginator(Paginator):
@@ -144,71 +144,71 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         TargetReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttachedIndicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAttachedIndices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listattachedindicespaginator)
         """
 
 class ListDevelopmentSchemaArnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdevelopmentschemaarnspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevelopmentSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdevelopmentschemaarnspaginator)
         """
 
 class ListDirectoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDirectories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdirectoriespaginator)
     """
 
     def paginate(
-        self, *, state: DirectoryStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, state: DirectoryStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDirectoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDirectories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdirectoriespaginator)
         """
 
 class ListFacetAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetattributespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFacetAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetattributespaginator)
         """
 
 class ListFacetNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetnamespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFacetNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetnamespaginator)
         """
 
 class ListIncomingTypedLinksPaginator(Paginator):
@@ -221,15 +221,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIncomingTypedLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIncomingTypedLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listincomingtypedlinkspaginator)
         """
 
 class ListIndexPaginator(Paginator):
@@ -241,29 +241,29 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
         RangesOnIndexedValues: Sequence[ObjectAttributeRangeTypeDef] = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIndexResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIndex.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listindexpaginator)
         """
 
 class ListManagedSchemaArnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListManagedSchemaArns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listmanagedschemaarnspaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListManagedSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listmanagedschemaarnspaginator)
         """
 
 class ListObjectAttributesPaginator(Paginator):
@@ -275,15 +275,15 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
         FacetFilter: SchemaFacetTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listobjectattributespaginator)
         """
 
 class ListObjectParentPathsPaginator(Paginator):
@@ -293,15 +293,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectParentPathsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectParentPaths.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listobjectparentpathspaginator)
         """
 
 class ListObjectPoliciesPaginator(Paginator):
@@ -312,15 +312,15 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listobjectpoliciespaginator)
         """
 
 class ListOutgoingTypedLinksPaginator(Paginator):
@@ -333,15 +333,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOutgoingTypedLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListOutgoingTypedLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listoutgoingtypedlinkspaginator)
         """
 
 class ListPolicyAttachmentsPaginator(Paginator):
@@ -352,71 +352,71 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPolicyAttachmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPolicyAttachments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listpolicyattachmentspaginator)
         """
 
 class ListPublishedSchemaArnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPublishedSchemaArns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listpublishedschemaarnspaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPublishedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPublishedSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listpublishedschemaarnspaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtagsforresourcepaginator)
         """
 
 class ListTypedLinkFacetAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetattributespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTypedLinkFacetAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetattributespaginator)
         """
 
 class ListTypedLinkFacetNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetnamespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTypedLinkFacetNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetnamespaginator)
         """
 
 class LookupPolicyPaginator(Paginator):
@@ -426,13 +426,13 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[LookupPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.LookupPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#lookuppolicypaginator)
         """
```

### Comparing `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/type_defs.py` & `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,117 +36,69 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ObjectReferenceTypeDef",
     "SchemaFacetTypeDef",
     "ApplySchemaRequestRequestTypeDef",
-    "ApplySchemaResponseTypeDef",
-    "AttachObjectResponseTypeDef",
-    "AttachToIndexResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TypedLinkSchemaAndFacetNameTypeDef",
-    "AttributeKeyOutputTypeDef",
-    "TypedAttributeValueOutputTypeDef",
     "AttributeKeyTypeDef",
+    "TypedAttributeValueOutputTypeDef",
     "TypedAttributeValueTypeDef",
     "BatchAttachObjectResponseTypeDef",
     "BatchAttachToIndexResponseTypeDef",
     "BatchCreateIndexResponseTypeDef",
     "BatchCreateObjectResponseTypeDef",
     "BatchDetachFromIndexResponseTypeDef",
     "BatchDetachObjectResponseTypeDef",
-    "SchemaFacetOutputTypeDef",
     "BatchListObjectChildrenResponseTypeDef",
     "PathToObjectIdentifiersTypeDef",
     "ObjectIdentifierAndLinkNameTupleTypeDef",
     "BatchListObjectPoliciesResponseTypeDef",
     "BatchListPolicyAttachmentsResponseTypeDef",
     "BatchReadExceptionTypeDef",
     "BatchUpdateObjectAttributesResponseTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
-    "CreateDirectoryResponseTypeDef",
-    "CreateIndexResponseTypeDef",
-    "CreateObjectResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
-    "CreateSchemaResponseTypeDef",
     "DeleteDirectoryRequestRequestTypeDef",
-    "DeleteDirectoryResponseTypeDef",
     "DeleteFacetRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
-    "DeleteSchemaResponseTypeDef",
     "DeleteTypedLinkFacetRequestRequestTypeDef",
-    "DetachFromIndexResponseTypeDef",
-    "DetachObjectResponseTypeDef",
     "DirectoryTypeDef",
     "DisableDirectoryRequestRequestTypeDef",
-    "DisableDirectoryResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableDirectoryRequestRequestTypeDef",
-    "EnableDirectoryResponseTypeDef",
     "RuleOutputTypeDef",
     "RuleTypeDef",
-    "FacetAttributeReferenceOutputTypeDef",
     "FacetAttributeReferenceTypeDef",
     "FacetTypeDef",
     "GetAppliedSchemaVersionRequestRequestTypeDef",
-    "GetAppliedSchemaVersionResponseTypeDef",
     "GetDirectoryRequestRequestTypeDef",
     "GetFacetRequestRequestTypeDef",
     "GetSchemaAsJsonRequestRequestTypeDef",
-    "GetSchemaAsJsonResponseTypeDef",
     "GetTypedLinkFacetInformationRequestRequestTypeDef",
-    "GetTypedLinkFacetInformationResponseTypeDef",
-    "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAppliedSchemaArnsRequestRequestTypeDef",
-    "ListAppliedSchemaArnsResponseTypeDef",
-    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
     "ListDevelopmentSchemaArnsRequestRequestTypeDef",
-    "ListDevelopmentSchemaArnsResponseTypeDef",
-    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
     "ListDirectoriesRequestRequestTypeDef",
-    "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
     "ListFacetAttributesRequestRequestTypeDef",
-    "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
     "ListFacetNamesRequestRequestTypeDef",
-    "ListFacetNamesResponseTypeDef",
-    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
     "ListManagedSchemaArnsRequestRequestTypeDef",
-    "ListManagedSchemaArnsResponseTypeDef",
-    "ListObjectChildrenResponseTypeDef",
-    "ListObjectPoliciesResponseTypeDef",
-    "ListPolicyAttachmentsResponseTypeDef",
-    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
     "ListPublishedSchemaArnsRequestRequestTypeDef",
-    "ListPublishedSchemaArnsResponseTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    "TagTypeDef",
     "ListTypedLinkFacetAttributesRequestRequestTypeDef",
-    "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     "ListTypedLinkFacetNamesRequestRequestTypeDef",
-    "ListTypedLinkFacetNamesResponseTypeDef",
-    "ObjectReferenceOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PolicyAttachmentTypeDef",
     "PublishSchemaRequestRequestTypeDef",
-    "PublishSchemaResponseTypeDef",
     "PutSchemaFromJsonRequestRequestTypeDef",
-    "PutSchemaFromJsonResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "TagTypeDef",
-    "TypedLinkSchemaAndFacetNameOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateObjectAttributesResponseTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
-    "UpdateSchemaResponseTypeDef",
     "UpgradeAppliedSchemaRequestRequestTypeDef",
-    "UpgradeAppliedSchemaResponseTypeDef",
     "UpgradePublishedSchemaRequestRequestTypeDef",
-    "UpgradePublishedSchemaResponseTypeDef",
     "AttachObjectRequestRequestTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachToIndexRequestRequestTypeDef",
     "BatchAttachObjectTypeDef",
     "BatchAttachPolicyTypeDef",
     "BatchAttachToIndexTypeDef",
     "BatchDeleteObjectTypeDef",
@@ -162,58 +114,100 @@
     "BatchListPolicyAttachmentsTypeDef",
     "BatchLookupPolicyTypeDef",
     "DeleteObjectRequestRequestTypeDef",
     "DetachFromIndexRequestRequestTypeDef",
     "DetachObjectRequestRequestTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "GetObjectInformationRequestRequestTypeDef",
-    "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     "ListAttachedIndicesRequestRequestTypeDef",
     "ListObjectChildrenRequestRequestTypeDef",
-    "ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
     "ListObjectParentPathsRequestRequestTypeDef",
     "ListObjectParentsRequestRequestTypeDef",
-    "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
     "ListObjectPoliciesRequestRequestTypeDef",
-    "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
     "ListPolicyAttachmentsRequestRequestTypeDef",
-    "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "LookupPolicyRequestRequestTypeDef",
     "BatchGetObjectAttributesTypeDef",
+    "BatchGetObjectInformationResponseTypeDef",
     "BatchListObjectAttributesTypeDef",
     "BatchRemoveFacetFromObjectTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
-    "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     "ListObjectAttributesRequestRequestTypeDef",
     "RemoveFacetFromObjectRequestRequestTypeDef",
-    "AttributeKeyAndValueOutputTypeDef",
-    "AttributeNameAndValueOutputTypeDef",
+    "ApplySchemaResponseTypeDef",
+    "AttachObjectResponseTypeDef",
+    "AttachToIndexResponseTypeDef",
+    "CreateDirectoryResponseTypeDef",
+    "CreateIndexResponseTypeDef",
+    "CreateObjectResponseTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "DeleteDirectoryResponseTypeDef",
+    "DeleteSchemaResponseTypeDef",
+    "DetachFromIndexResponseTypeDef",
+    "DetachObjectResponseTypeDef",
+    "DisableDirectoryResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EnableDirectoryResponseTypeDef",
+    "GetAppliedSchemaVersionResponseTypeDef",
+    "GetObjectInformationResponseTypeDef",
+    "GetSchemaAsJsonResponseTypeDef",
+    "GetTypedLinkFacetInformationResponseTypeDef",
+    "ListAppliedSchemaArnsResponseTypeDef",
+    "ListDevelopmentSchemaArnsResponseTypeDef",
+    "ListFacetNamesResponseTypeDef",
+    "ListManagedSchemaArnsResponseTypeDef",
+    "ListObjectChildrenResponseTypeDef",
+    "ListObjectPoliciesResponseTypeDef",
+    "ListPolicyAttachmentsResponseTypeDef",
+    "ListPublishedSchemaArnsResponseTypeDef",
+    "ListTypedLinkFacetNamesResponseTypeDef",
+    "PublishSchemaResponseTypeDef",
+    "PutSchemaFromJsonResponseTypeDef",
+    "UpdateObjectAttributesResponseTypeDef",
+    "UpdateSchemaResponseTypeDef",
+    "UpgradeAppliedSchemaResponseTypeDef",
+    "UpgradePublishedSchemaResponseTypeDef",
     "BatchCreateIndexTypeDef",
     "CreateIndexRequestRequestTypeDef",
+    "AttributeKeyAndValueOutputTypeDef",
+    "AttributeNameAndValueOutputTypeDef",
     "AttributeKeyAndValueTypeDef",
     "AttributeNameAndValueTypeDef",
     "LinkAttributeActionTypeDef",
     "ObjectAttributeActionTypeDef",
     "TypedAttributeValueRangeTypeDef",
-    "BatchGetObjectInformationResponseTypeDef",
-    "GetObjectInformationResponseTypeDef",
     "BatchListObjectParentPathsResponseTypeDef",
     "ListObjectParentPathsResponseTypeDef",
     "BatchListObjectParentsResponseTypeDef",
     "ListObjectParentsResponseTypeDef",
     "GetDirectoryResponseTypeDef",
     "ListDirectoriesResponseTypeDef",
     "FacetAttributeDefinitionOutputTypeDef",
     "TypedLinkAttributeDefinitionOutputTypeDef",
     "FacetAttributeDefinitionTypeDef",
     "TypedLinkAttributeDefinitionTypeDef",
     "GetFacetResponseTypeDef",
+    "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
+    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
+    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
+    "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
+    "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
+    "ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
+    "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PolicyToPathTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "PolicyToPathTypeDef",
     "BatchGetLinkAttributesResponseTypeDef",
     "BatchGetObjectAttributesResponseTypeDef",
     "BatchListObjectAttributesResponseTypeDef",
     "GetLinkAttributesResponseTypeDef",
     "GetObjectAttributesResponseTypeDef",
     "IndexAttachmentTypeDef",
     "ListObjectAttributesResponseTypeDef",
@@ -301,49 +295,35 @@
     "ApplySchemaRequestRequestTypeDef",
     {
         "PublishedSchemaArn": str,
         "DirectoryArn": str,
     },
 )
 
-ApplySchemaResponseTypeDef = TypedDict(
-    "ApplySchemaResponseTypeDef",
-    {
-        "AppliedSchemaArn": str,
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AttachObjectResponseTypeDef = TypedDict(
-    "AttachObjectResponseTypeDef",
-    {
-        "AttachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AttachToIndexResponseTypeDef = TypedDict(
-    "AttachToIndexResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AttachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TypedLinkSchemaAndFacetNameTypeDef = TypedDict(
     "TypedLinkSchemaAndFacetNameTypeDef",
     {
         "SchemaArn": str,
         "TypedLinkName": str,
     },
 )
 
-AttributeKeyOutputTypeDef = TypedDict(
-    "AttributeKeyOutputTypeDef",
+AttributeKeyTypeDef = TypedDict(
+    "AttributeKeyTypeDef",
     {
         "SchemaArn": str,
         "FacetName": str,
         "Name": str,
     },
 )
 
@@ -355,23 +335,14 @@
         "BooleanValue": bool,
         "NumberValue": str,
         "DatetimeValue": datetime,
     },
     total=False,
 )
 
-AttributeKeyTypeDef = TypedDict(
-    "AttributeKeyTypeDef",
-    {
-        "SchemaArn": str,
-        "FacetName": str,
-        "Name": str,
-    },
-)
-
 TypedAttributeValueTypeDef = TypedDict(
     "TypedAttributeValueTypeDef",
     {
         "StringValue": str,
         "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
         "BooleanValue": bool,
         "NumberValue": str,
@@ -424,23 +395,14 @@
     "BatchDetachObjectResponseTypeDef",
     {
         "detachedObjectIdentifier": str,
     },
     total=False,
 )
 
-SchemaFacetOutputTypeDef = TypedDict(
-    "SchemaFacetOutputTypeDef",
-    {
-        "SchemaArn": str,
-        "FacetName": str,
-    },
-    total=False,
-)
-
 BatchListObjectChildrenResponseTypeDef = TypedDict(
     "BatchListObjectChildrenResponseTypeDef",
     {
         "Children": Dict[str, str],
         "NextToken": str,
     },
     total=False,
@@ -503,71 +465,28 @@
     "CreateDirectoryRequestRequestTypeDef",
     {
         "Name": str,
         "SchemaArn": str,
     },
 )
 
-CreateDirectoryResponseTypeDef = TypedDict(
-    "CreateDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "Name": str,
-        "ObjectIdentifier": str,
-        "AppliedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateIndexResponseTypeDef = TypedDict(
-    "CreateIndexResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateObjectResponseTypeDef = TypedDict(
-    "CreateObjectResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSchemaRequestRequestTypeDef = TypedDict(
     "CreateSchemaRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDirectoryRequestRequestTypeDef = TypedDict(
     "DeleteDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-DeleteDirectoryResponseTypeDef = TypedDict(
-    "DeleteDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFacetRequestRequestTypeDef = TypedDict(
     "DeleteFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -575,46 +494,22 @@
 DeleteSchemaRequestRequestTypeDef = TypedDict(
     "DeleteSchemaRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
-DeleteSchemaResponseTypeDef = TypedDict(
-    "DeleteSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTypedLinkFacetRequestRequestTypeDef = TypedDict(
     "DeleteTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-DetachFromIndexResponseTypeDef = TypedDict(
-    "DetachFromIndexResponseTypeDef",
-    {
-        "DetachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DetachObjectResponseTypeDef = TypedDict(
-    "DetachObjectResponseTypeDef",
-    {
-        "DetachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DirectoryTypeDef = TypedDict(
     "DirectoryTypeDef",
     {
         "Name": str,
         "DirectoryArn": str,
         "State": DirectoryStateType,
         "CreationDateTime": datetime,
@@ -625,44 +520,21 @@
 DisableDirectoryRequestRequestTypeDef = TypedDict(
     "DisableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-DisableDirectoryResponseTypeDef = TypedDict(
-    "DisableDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
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
 EnableDirectoryRequestRequestTypeDef = TypedDict(
     "EnableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-EnableDirectoryResponseTypeDef = TypedDict(
-    "EnableDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RuleOutputTypeDef = TypedDict(
     "RuleOutputTypeDef",
     {
         "Type": RuleTypeType,
         "Parameters": Dict[str, str],
     },
     total=False,
@@ -673,22 +545,14 @@
     {
         "Type": RuleTypeType,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
-FacetAttributeReferenceOutputTypeDef = TypedDict(
-    "FacetAttributeReferenceOutputTypeDef",
-    {
-        "TargetFacetName": str,
-        "TargetAttributeName": str,
-    },
-)
-
 FacetAttributeReferenceTypeDef = TypedDict(
     "FacetAttributeReferenceTypeDef",
     {
         "TargetFacetName": str,
         "TargetAttributeName": str,
     },
 )
@@ -706,22 +570,14 @@
 GetAppliedSchemaVersionRequestRequestTypeDef = TypedDict(
     "GetAppliedSchemaVersionRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
-GetAppliedSchemaVersionResponseTypeDef = TypedDict(
-    "GetAppliedSchemaVersionResponseTypeDef",
-    {
-        "AppliedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDirectoryRequestRequestTypeDef = TypedDict(
     "GetDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
@@ -736,62 +592,32 @@
 GetSchemaAsJsonRequestRequestTypeDef = TypedDict(
     "GetSchemaAsJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
-GetSchemaAsJsonResponseTypeDef = TypedDict(
-    "GetSchemaAsJsonResponseTypeDef",
-    {
-        "Name": str,
-        "Document": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTypedLinkFacetInformationRequestRequestTypeDef = TypedDict(
     "GetTypedLinkFacetInformationRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-GetTypedLinkFacetInformationResponseTypeDef = TypedDict(
-    "GetTypedLinkFacetInformationResponseTypeDef",
-    {
-        "IdentityAttributeOrder": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
-    "_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-    },
-)
-_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
-    "_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "SchemaArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef(
-    _RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-    _OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAppliedSchemaArnsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppliedSchemaArnsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 _OptionalListAppliedSchemaArnsRequestRequestTypeDef = TypedDict(
@@ -808,91 +634,33 @@
 class ListAppliedSchemaArnsRequestRequestTypeDef(
     _RequiredListAppliedSchemaArnsRequestRequestTypeDef,
     _OptionalListAppliedSchemaArnsRequestRequestTypeDef,
 ):
     pass
 
 
-ListAppliedSchemaArnsResponseTypeDef = TypedDict(
-    "ListAppliedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef = TypedDict(
-    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDevelopmentSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListDevelopmentSchemaArnsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDevelopmentSchemaArnsResponseTypeDef = TypedDict(
-    "ListDevelopmentSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDirectoriesRequestListDirectoriesPaginateTypeDef = TypedDict(
-    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
-    {
-        "state": DirectoryStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDirectoriesRequestRequestTypeDef = TypedDict(
     "ListDirectoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "state": DirectoryStateType,
     },
     total=False,
 )
 
-_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFacetAttributesRequestListFacetAttributesPaginateTypeDef(
-    _RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-    _OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFacetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacetAttributesRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -909,36 +677,14 @@
 class ListFacetAttributesRequestRequestTypeDef(
     _RequiredListFacetAttributesRequestRequestTypeDef,
     _OptionalListFacetAttributesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
-    "_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-    },
-)
-_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
-    "_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFacetNamesRequestListFacetNamesPaginateTypeDef(
-    _RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef,
-    _OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFacetNamesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacetNamesRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 _OptionalListFacetNamesRequestRequestTypeDef = TypedDict(
@@ -953,128 +699,34 @@
 
 class ListFacetNamesRequestRequestTypeDef(
     _RequiredListFacetNamesRequestRequestTypeDef, _OptionalListFacetNamesRequestRequestTypeDef
 ):
     pass
 
 
-ListFacetNamesResponseTypeDef = TypedDict(
-    "ListFacetNamesResponseTypeDef",
-    {
-        "FacetNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef = TypedDict(
-    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListManagedSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListManagedSchemaArnsRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListManagedSchemaArnsResponseTypeDef = TypedDict(
-    "ListManagedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListObjectChildrenResponseTypeDef = TypedDict(
-    "ListObjectChildrenResponseTypeDef",
-    {
-        "Children": Dict[str, str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListObjectPoliciesResponseTypeDef = TypedDict(
-    "ListObjectPoliciesResponseTypeDef",
-    {
-        "AttachedPolicyIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPolicyAttachmentsResponseTypeDef = TypedDict(
-    "ListPolicyAttachmentsResponseTypeDef",
-    {
-        "ObjectIdentifiers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef = TypedDict(
-    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPublishedSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListPublishedSchemaArnsRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListPublishedSchemaArnsResponseTypeDef = TypedDict(
-    "ListPublishedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1090,46 +742,23 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef(
-    _RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-    _OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTypedLinkFacetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypedLinkFacetAttributesRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -1146,36 +775,14 @@
 class ListTypedLinkFacetAttributesRequestRequestTypeDef(
     _RequiredListTypedLinkFacetAttributesRequestRequestTypeDef,
     _OptionalListTypedLinkFacetAttributesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
-    "_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-    },
-)
-_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
-    "_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef(
-    _RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-    _OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTypedLinkFacetNamesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypedLinkFacetNamesRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 _OptionalListTypedLinkFacetNamesRequestRequestTypeDef = TypedDict(
@@ -1191,41 +798,14 @@
 class ListTypedLinkFacetNamesRequestRequestTypeDef(
     _RequiredListTypedLinkFacetNamesRequestRequestTypeDef,
     _OptionalListTypedLinkFacetNamesRequestRequestTypeDef,
 ):
     pass
 
 
-ListTypedLinkFacetNamesResponseTypeDef = TypedDict(
-    "ListTypedLinkFacetNamesResponseTypeDef",
-    {
-        "FacetNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ObjectReferenceOutputTypeDef = TypedDict(
-    "ObjectReferenceOutputTypeDef",
-    {
-        "Selector": str,
-    },
-    total=False,
-)
-
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
 PolicyAttachmentTypeDef = TypedDict(
     "PolicyAttachmentTypeDef",
     {
         "PolicyId": str,
         "ObjectIdentifier": str,
         "PolicyType": str,
     },
@@ -1251,98 +831,38 @@
 
 class PublishSchemaRequestRequestTypeDef(
     _RequiredPublishSchemaRequestRequestTypeDef, _OptionalPublishSchemaRequestRequestTypeDef
 ):
     pass
 
 
-PublishSchemaResponseTypeDef = TypedDict(
-    "PublishSchemaResponseTypeDef",
-    {
-        "PublishedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutSchemaFromJsonRequestRequestTypeDef = TypedDict(
     "PutSchemaFromJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Document": str,
     },
 )
 
-PutSchemaFromJsonResponseTypeDef = TypedDict(
-    "PutSchemaFromJsonResponseTypeDef",
-    {
-        "Arn": str,
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
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-TypedLinkSchemaAndFacetNameOutputTypeDef = TypedDict(
-    "TypedLinkSchemaAndFacetNameOutputTypeDef",
-    {
-        "SchemaArn": str,
-        "TypedLinkName": str,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateObjectAttributesResponseTypeDef = TypedDict(
-    "UpdateObjectAttributesResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSchemaRequestRequestTypeDef = TypedDict(
     "UpdateSchemaRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-UpdateSchemaResponseTypeDef = TypedDict(
-    "UpdateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpgradeAppliedSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradeAppliedSchemaRequestRequestTypeDef",
     {
         "PublishedSchemaArn": str,
         "DirectoryArn": str,
     },
 )
@@ -1358,23 +878,14 @@
 class UpgradeAppliedSchemaRequestRequestTypeDef(
     _RequiredUpgradeAppliedSchemaRequestRequestTypeDef,
     _OptionalUpgradeAppliedSchemaRequestRequestTypeDef,
 ):
     pass
 
 
-UpgradeAppliedSchemaResponseTypeDef = TypedDict(
-    "UpgradeAppliedSchemaResponseTypeDef",
-    {
-        "UpgradedSchemaArn": str,
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpgradePublishedSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradePublishedSchemaRequestRequestTypeDef",
     {
         "DevelopmentSchemaArn": str,
         "PublishedSchemaArn": str,
         "MinorVersion": str,
     },
@@ -1391,22 +902,14 @@
 class UpgradePublishedSchemaRequestRequestTypeDef(
     _RequiredUpgradePublishedSchemaRequestRequestTypeDef,
     _OptionalUpgradePublishedSchemaRequestRequestTypeDef,
 ):
     pass
 
 
-UpgradePublishedSchemaResponseTypeDef = TypedDict(
-    "UpgradePublishedSchemaResponseTypeDef",
-    {
-        "UpgradedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttachObjectRequestRequestTypeDef = TypedDict(
     "AttachObjectRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ParentReference": ObjectReferenceTypeDef,
         "ChildReference": ObjectReferenceTypeDef,
         "LinkName": str,
@@ -1716,38 +1219,14 @@
 class GetObjectInformationRequestRequestTypeDef(
     _RequiredGetObjectInformationRequestRequestTypeDef,
     _OptionalGetObjectInformationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "TargetReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef(
-    _RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-    _OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAttachedIndicesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedIndicesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "TargetReference": ObjectReferenceTypeDef,
     },
 )
@@ -1790,37 +1269,14 @@
 class ListObjectChildrenRequestRequestTypeDef(
     _RequiredListObjectChildrenRequestRequestTypeDef,
     _OptionalListObjectChildrenRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef(
-    _RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-    _OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListObjectParentPathsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectParentPathsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1862,38 +1318,14 @@
 
 class ListObjectParentsRequestRequestTypeDef(
     _RequiredListObjectParentsRequestRequestTypeDef, _OptionalListObjectParentsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef(
-    _RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-    _OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListObjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectPoliciesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1911,38 +1343,14 @@
 class ListObjectPoliciesRequestRequestTypeDef(
     _RequiredListObjectPoliciesRequestRequestTypeDef,
     _OptionalListObjectPoliciesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "PolicyReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef(
-    _RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-    _OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPolicyAttachmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyAttachmentsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "PolicyReference": ObjectReferenceTypeDef,
     },
 )
@@ -1960,37 +1368,14 @@
 class ListPolicyAttachmentsRequestRequestTypeDef(
     _RequiredListPolicyAttachmentsRequestRequestTypeDef,
     _OptionalListPolicyAttachmentsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
-    "_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
-    "_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class LookupPolicyRequestLookupPolicyPaginateTypeDef(
-    _RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef,
-    _OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef,
-):
-    pass
-
-
 _RequiredLookupPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredLookupPolicyRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -2015,14 +1400,23 @@
     {
         "ObjectReference": ObjectReferenceTypeDef,
         "SchemaFacet": SchemaFacetTypeDef,
         "AttributeNames": Sequence[str],
     },
 )
 
+BatchGetObjectInformationResponseTypeDef = TypedDict(
+    "BatchGetObjectInformationResponseTypeDef",
+    {
+        "SchemaFacets": List[SchemaFacetTypeDef],
+        "ObjectIdentifier": str,
+    },
+    total=False,
+)
+
 _RequiredBatchListObjectAttributesTypeDef = TypedDict(
     "_RequiredBatchListObjectAttributesTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListObjectAttributesTypeDef = TypedDict(
@@ -2071,39 +1465,14 @@
 class GetObjectAttributesRequestRequestTypeDef(
     _RequiredGetObjectAttributesRequestRequestTypeDef,
     _OptionalGetObjectAttributesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "FacetFilter": SchemaFacetTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListObjectAttributesRequestListObjectAttributesPaginateTypeDef(
-    _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-    _OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListObjectAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectAttributesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -2131,27 +1500,290 @@
     {
         "DirectoryArn": str,
         "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 
-AttributeKeyAndValueOutputTypeDef = TypedDict(
-    "AttributeKeyAndValueOutputTypeDef",
+ApplySchemaResponseTypeDef = TypedDict(
+    "ApplySchemaResponseTypeDef",
     {
-        "Key": AttributeKeyOutputTypeDef,
-        "Value": TypedAttributeValueOutputTypeDef,
+        "AppliedSchemaArn": str,
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AttributeNameAndValueOutputTypeDef = TypedDict(
-    "AttributeNameAndValueOutputTypeDef",
+AttachObjectResponseTypeDef = TypedDict(
+    "AttachObjectResponseTypeDef",
     {
-        "AttributeName": str,
-        "Value": TypedAttributeValueOutputTypeDef,
+        "AttachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachToIndexResponseTypeDef = TypedDict(
+    "AttachToIndexResponseTypeDef",
+    {
+        "AttachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDirectoryResponseTypeDef = TypedDict(
+    "CreateDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "Name": str,
+        "ObjectIdentifier": str,
+        "AppliedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIndexResponseTypeDef = TypedDict(
+    "CreateIndexResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateObjectResponseTypeDef = TypedDict(
+    "CreateObjectResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDirectoryResponseTypeDef = TypedDict(
+    "DeleteDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSchemaResponseTypeDef = TypedDict(
+    "DeleteSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachFromIndexResponseTypeDef = TypedDict(
+    "DetachFromIndexResponseTypeDef",
+    {
+        "DetachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachObjectResponseTypeDef = TypedDict(
+    "DetachObjectResponseTypeDef",
+    {
+        "DetachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableDirectoryResponseTypeDef = TypedDict(
+    "DisableDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
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
+EnableDirectoryResponseTypeDef = TypedDict(
+    "EnableDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppliedSchemaVersionResponseTypeDef = TypedDict(
+    "GetAppliedSchemaVersionResponseTypeDef",
+    {
+        "AppliedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetObjectInformationResponseTypeDef = TypedDict(
+    "GetObjectInformationResponseTypeDef",
+    {
+        "SchemaFacets": List[SchemaFacetTypeDef],
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSchemaAsJsonResponseTypeDef = TypedDict(
+    "GetSchemaAsJsonResponseTypeDef",
+    {
+        "Name": str,
+        "Document": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTypedLinkFacetInformationResponseTypeDef = TypedDict(
+    "GetTypedLinkFacetInformationResponseTypeDef",
+    {
+        "IdentityAttributeOrder": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAppliedSchemaArnsResponseTypeDef = TypedDict(
+    "ListAppliedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDevelopmentSchemaArnsResponseTypeDef = TypedDict(
+    "ListDevelopmentSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFacetNamesResponseTypeDef = TypedDict(
+    "ListFacetNamesResponseTypeDef",
+    {
+        "FacetNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListManagedSchemaArnsResponseTypeDef = TypedDict(
+    "ListManagedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListObjectChildrenResponseTypeDef = TypedDict(
+    "ListObjectChildrenResponseTypeDef",
+    {
+        "Children": Dict[str, str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListObjectPoliciesResponseTypeDef = TypedDict(
+    "ListObjectPoliciesResponseTypeDef",
+    {
+        "AttachedPolicyIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPolicyAttachmentsResponseTypeDef = TypedDict(
+    "ListPolicyAttachmentsResponseTypeDef",
+    {
+        "ObjectIdentifiers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPublishedSchemaArnsResponseTypeDef = TypedDict(
+    "ListPublishedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTypedLinkFacetNamesResponseTypeDef = TypedDict(
+    "ListTypedLinkFacetNamesResponseTypeDef",
+    {
+        "FacetNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishSchemaResponseTypeDef = TypedDict(
+    "PublishSchemaResponseTypeDef",
+    {
+        "PublishedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutSchemaFromJsonResponseTypeDef = TypedDict(
+    "PutSchemaFromJsonResponseTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateObjectAttributesResponseTypeDef = TypedDict(
+    "UpdateObjectAttributesResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSchemaResponseTypeDef = TypedDict(
+    "UpdateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpgradeAppliedSchemaResponseTypeDef = TypedDict(
+    "UpgradeAppliedSchemaResponseTypeDef",
+    {
+        "UpgradedSchemaArn": str,
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpgradePublishedSchemaResponseTypeDef = TypedDict(
+    "UpgradePublishedSchemaResponseTypeDef",
+    {
+        "UpgradedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchCreateIndexTypeDef = TypedDict(
     "_RequiredBatchCreateIndexTypeDef",
     {
         "OrderedIndexedAttributeList": Sequence[AttributeKeyTypeDef],
@@ -2193,14 +1825,30 @@
 
 class CreateIndexRequestRequestTypeDef(
     _RequiredCreateIndexRequestRequestTypeDef, _OptionalCreateIndexRequestRequestTypeDef
 ):
     pass
 
 
+AttributeKeyAndValueOutputTypeDef = TypedDict(
+    "AttributeKeyAndValueOutputTypeDef",
+    {
+        "Key": AttributeKeyTypeDef,
+        "Value": TypedAttributeValueOutputTypeDef,
+    },
+)
+
+AttributeNameAndValueOutputTypeDef = TypedDict(
+    "AttributeNameAndValueOutputTypeDef",
+    {
+        "AttributeName": str,
+        "Value": TypedAttributeValueOutputTypeDef,
+    },
+)
+
 AttributeKeyAndValueTypeDef = TypedDict(
     "AttributeKeyAndValueTypeDef",
     {
         "Key": AttributeKeyTypeDef,
         "Value": TypedAttributeValueTypeDef,
     },
 )
@@ -2250,47 +1898,29 @@
 
 class TypedAttributeValueRangeTypeDef(
     _RequiredTypedAttributeValueRangeTypeDef, _OptionalTypedAttributeValueRangeTypeDef
 ):
     pass
 
 
-BatchGetObjectInformationResponseTypeDef = TypedDict(
-    "BatchGetObjectInformationResponseTypeDef",
-    {
-        "SchemaFacets": List[SchemaFacetOutputTypeDef],
-        "ObjectIdentifier": str,
-    },
-    total=False,
-)
-
-GetObjectInformationResponseTypeDef = TypedDict(
-    "GetObjectInformationResponseTypeDef",
-    {
-        "SchemaFacets": List[SchemaFacetOutputTypeDef],
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchListObjectParentPathsResponseTypeDef = TypedDict(
     "BatchListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
 ListObjectParentPathsResponseTypeDef = TypedDict(
     "ListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchListObjectParentsResponseTypeDef = TypedDict(
     "BatchListObjectParentsResponseTypeDef",
     {
         "ParentLinks": List[ObjectIdentifierAndLinkNameTupleTypeDef],
@@ -2301,32 +1931,32 @@
 
 ListObjectParentsResponseTypeDef = TypedDict(
     "ListObjectParentsResponseTypeDef",
     {
         "Parents": Dict[str, str],
         "NextToken": str,
         "ParentLinks": List[ObjectIdentifierAndLinkNameTupleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDirectoryResponseTypeDef = TypedDict(
     "GetDirectoryResponseTypeDef",
     {
         "Directory": DirectoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDirectoriesResponseTypeDef = TypedDict(
     "ListDirectoriesResponseTypeDef",
     {
         "Directories": List[DirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFacetAttributeDefinitionOutputTypeDef = TypedDict(
     "_RequiredFacetAttributeDefinitionOutputTypeDef",
     {
         "Type": FacetAttributeTypeType,
@@ -2423,44 +2053,357 @@
     pass
 
 
 GetFacetResponseTypeDef = TypedDict(
     "GetFacetResponseTypeDef",
     {
         "Facet": FacetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
+    "_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DirectoryArn": str,
+    },
+)
+_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
+    "_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-PolicyToPathTypeDef = TypedDict(
-    "PolicyToPathTypeDef",
+
+class ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef(
+    _RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    _OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     {
-        "Path": str,
-        "Policies": List[PolicyAttachmentTypeDef],
+        "DirectoryArn": str,
+        "TargetReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
+class ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef(
+    _RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+    _OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+):
+    pass
+
+
+ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef = TypedDict(
+    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDirectoriesRequestListDirectoriesPaginateTypeDef = TypedDict(
+    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
+    {
+        "state": DirectoryStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFacetAttributesRequestListFacetAttributesPaginateTypeDef(
+    _RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+    _OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
+    "_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+    },
+)
+_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
+    "_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFacetNamesRequestListFacetNamesPaginateTypeDef(
+    _RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef,
+    _OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef,
+):
+    pass
+
+
+ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef = TypedDict(
+    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "FacetFilter": SchemaFacetTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListObjectAttributesRequestListObjectAttributesPaginateTypeDef(
+    _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+    _OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef(
+    _RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+    _OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef(
+    _RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+    _OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "PolicyReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef(
+    _RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+    _OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+):
+    pass
+
+
+ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef = TypedDict(
+    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef(
+    _RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    _OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
+    "_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+    },
+)
+_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
+    "_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef(
+    _RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+    _OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
+    "_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
+    "_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class LookupPolicyRequestLookupPolicyPaginateTypeDef(
+    _RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef,
+    _OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef,
+):
+    pass
+
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+PolicyToPathTypeDef = TypedDict(
+    "PolicyToPathTypeDef",
+    {
+        "Path": str,
+        "Policies": List[PolicyAttachmentTypeDef],
+    },
+    total=False,
+)
+
 BatchGetLinkAttributesResponseTypeDef = TypedDict(
     "BatchGetLinkAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueOutputTypeDef],
     },
     total=False,
 )
@@ -2482,23 +2425,23 @@
     total=False,
 )
 
 GetLinkAttributesResponseTypeDef = TypedDict(
     "GetLinkAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectAttributesResponseTypeDef = TypedDict(
     "GetObjectAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IndexAttachmentTypeDef = TypedDict(
     "IndexAttachmentTypeDef",
     {
         "IndexedAttributes": List[AttributeKeyAndValueOutputTypeDef],
@@ -2508,24 +2451,24 @@
 )
 
 ListObjectAttributesResponseTypeDef = TypedDict(
     "ListObjectAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TypedLinkSpecifierOutputTypeDef = TypedDict(
     "TypedLinkSpecifierOutputTypeDef",
     {
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameOutputTypeDef,
-        "SourceObjectReference": ObjectReferenceOutputTypeDef,
-        "TargetObjectReference": ObjectReferenceOutputTypeDef,
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
+        "SourceObjectReference": ObjectReferenceTypeDef,
+        "TargetObjectReference": ObjectReferenceTypeDef,
         "IdentityAttributeValues": List[AttributeNameAndValueOutputTypeDef],
     },
 )
 
 _RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
     "_RequiredAddFacetToObjectRequestRequestTypeDef",
     {
@@ -2691,15 +2634,15 @@
         "Name": str,
     },
 )
 _OptionalFacetAttributeOutputTypeDef = TypedDict(
     "_OptionalFacetAttributeOutputTypeDef",
     {
         "AttributeDefinition": FacetAttributeDefinitionOutputTypeDef,
-        "AttributeReference": FacetAttributeReferenceOutputTypeDef,
+        "AttributeReference": FacetAttributeReferenceTypeDef,
         "RequiredBehavior": RequiredAttributeBehaviorType,
     },
     total=False,
 )
 
 
 class FacetAttributeOutputTypeDef(
@@ -2709,15 +2652,15 @@
 
 
 ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
     "ListTypedLinkFacetAttributesResponseTypeDef",
     {
         "Attributes": List[TypedLinkAttributeDefinitionOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFacetAttributeTypeDef = TypedDict(
     "_RequiredFacetAttributeTypeDef",
     {
         "Name": str,
@@ -2765,15 +2708,15 @@
 )
 
 LookupPolicyResponseTypeDef = TypedDict(
     "LookupPolicyResponseTypeDef",
     {
         "PolicyToPathList": List[PolicyToPathTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchListAttachedIndicesResponseTypeDef = TypedDict(
     "BatchListAttachedIndicesResponseTypeDef",
     {
         "IndexAttachments": List[IndexAttachmentTypeDef],
@@ -2792,32 +2735,32 @@
 )
 
 ListAttachedIndicesResponseTypeDef = TypedDict(
     "ListAttachedIndicesResponseTypeDef",
     {
         "IndexAttachments": List[IndexAttachmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIndexResponseTypeDef = TypedDict(
     "ListIndexResponseTypeDef",
     {
         "IndexAttachments": List[IndexAttachmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachTypedLinkResponseTypeDef = TypedDict(
     "AttachTypedLinkResponseTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchAttachTypedLinkResponseTypeDef = TypedDict(
     "BatchAttachTypedLinkResponseTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
@@ -2844,24 +2787,24 @@
 )
 
 ListIncomingTypedLinksResponseTypeDef = TypedDict(
     "ListIncomingTypedLinksResponseTypeDef",
     {
         "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOutgoingTypedLinksResponseTypeDef = TypedDict(
     "ListOutgoingTypedLinksResponseTypeDef",
     {
         "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetachTypedLinkTypeDef = TypedDict(
     "BatchDetachTypedLinkTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
@@ -2970,15 +2913,15 @@
     },
 )
 _OptionalListIndexRequestListIndexPaginateTypeDef = TypedDict(
     "_OptionalListIndexRequestListIndexPaginateTypeDef",
     {
         "RangesOnIndexedValues": Sequence[ObjectAttributeRangeTypeDef],
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListIndexRequestListIndexPaginateTypeDef(
     _RequiredListIndexRequestListIndexPaginateTypeDef,
@@ -3069,15 +3012,15 @@
 )
 _OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef = TypedDict(
     "_OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     {
         "FilterAttributeRanges": Sequence[TypedLinkAttributeRangeTypeDef],
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef(
     _RequiredListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
@@ -3122,15 +3065,15 @@
 )
 _OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef = TypedDict(
     "_OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     {
         "FilterAttributeRanges": Sequence[TypedLinkAttributeRangeTypeDef],
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef(
     _RequiredListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
@@ -3167,15 +3110,15 @@
 
 
 ListFacetAttributesResponseTypeDef = TypedDict(
     "ListFacetAttributesResponseTypeDef",
     {
         "Attributes": List[FacetAttributeOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFacetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
@@ -3335,15 +3278,15 @@
     pass
 
 
 BatchWriteResponseTypeDef = TypedDict(
     "BatchWriteResponseTypeDef",
     {
         "Responses": List[BatchWriteOperationResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchReadOperationResponseTypeDef = TypedDict(
     "BatchReadOperationResponseTypeDef",
     {
         "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
@@ -3382,10 +3325,10 @@
     pass
 
 
 BatchReadResponseTypeDef = TypedDict(
     "BatchReadResponseTypeDef",
     {
         "Responses": List[BatchReadOperationResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/type_defs.pyi` & `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -35,117 +35,69 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ObjectReferenceTypeDef",
     "SchemaFacetTypeDef",
     "ApplySchemaRequestRequestTypeDef",
-    "ApplySchemaResponseTypeDef",
-    "AttachObjectResponseTypeDef",
-    "AttachToIndexResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TypedLinkSchemaAndFacetNameTypeDef",
-    "AttributeKeyOutputTypeDef",
-    "TypedAttributeValueOutputTypeDef",
     "AttributeKeyTypeDef",
+    "TypedAttributeValueOutputTypeDef",
     "TypedAttributeValueTypeDef",
     "BatchAttachObjectResponseTypeDef",
     "BatchAttachToIndexResponseTypeDef",
     "BatchCreateIndexResponseTypeDef",
     "BatchCreateObjectResponseTypeDef",
     "BatchDetachFromIndexResponseTypeDef",
     "BatchDetachObjectResponseTypeDef",
-    "SchemaFacetOutputTypeDef",
     "BatchListObjectChildrenResponseTypeDef",
     "PathToObjectIdentifiersTypeDef",
     "ObjectIdentifierAndLinkNameTupleTypeDef",
     "BatchListObjectPoliciesResponseTypeDef",
     "BatchListPolicyAttachmentsResponseTypeDef",
     "BatchReadExceptionTypeDef",
     "BatchUpdateObjectAttributesResponseTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
-    "CreateDirectoryResponseTypeDef",
-    "CreateIndexResponseTypeDef",
-    "CreateObjectResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
-    "CreateSchemaResponseTypeDef",
     "DeleteDirectoryRequestRequestTypeDef",
-    "DeleteDirectoryResponseTypeDef",
     "DeleteFacetRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
-    "DeleteSchemaResponseTypeDef",
     "DeleteTypedLinkFacetRequestRequestTypeDef",
-    "DetachFromIndexResponseTypeDef",
-    "DetachObjectResponseTypeDef",
     "DirectoryTypeDef",
     "DisableDirectoryRequestRequestTypeDef",
-    "DisableDirectoryResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableDirectoryRequestRequestTypeDef",
-    "EnableDirectoryResponseTypeDef",
     "RuleOutputTypeDef",
     "RuleTypeDef",
-    "FacetAttributeReferenceOutputTypeDef",
     "FacetAttributeReferenceTypeDef",
     "FacetTypeDef",
     "GetAppliedSchemaVersionRequestRequestTypeDef",
-    "GetAppliedSchemaVersionResponseTypeDef",
     "GetDirectoryRequestRequestTypeDef",
     "GetFacetRequestRequestTypeDef",
     "GetSchemaAsJsonRequestRequestTypeDef",
-    "GetSchemaAsJsonResponseTypeDef",
     "GetTypedLinkFacetInformationRequestRequestTypeDef",
-    "GetTypedLinkFacetInformationResponseTypeDef",
-    "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAppliedSchemaArnsRequestRequestTypeDef",
-    "ListAppliedSchemaArnsResponseTypeDef",
-    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
     "ListDevelopmentSchemaArnsRequestRequestTypeDef",
-    "ListDevelopmentSchemaArnsResponseTypeDef",
-    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
     "ListDirectoriesRequestRequestTypeDef",
-    "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
     "ListFacetAttributesRequestRequestTypeDef",
-    "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
     "ListFacetNamesRequestRequestTypeDef",
-    "ListFacetNamesResponseTypeDef",
-    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
     "ListManagedSchemaArnsRequestRequestTypeDef",
-    "ListManagedSchemaArnsResponseTypeDef",
-    "ListObjectChildrenResponseTypeDef",
-    "ListObjectPoliciesResponseTypeDef",
-    "ListPolicyAttachmentsResponseTypeDef",
-    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
     "ListPublishedSchemaArnsRequestRequestTypeDef",
-    "ListPublishedSchemaArnsResponseTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    "TagTypeDef",
     "ListTypedLinkFacetAttributesRequestRequestTypeDef",
-    "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     "ListTypedLinkFacetNamesRequestRequestTypeDef",
-    "ListTypedLinkFacetNamesResponseTypeDef",
-    "ObjectReferenceOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PolicyAttachmentTypeDef",
     "PublishSchemaRequestRequestTypeDef",
-    "PublishSchemaResponseTypeDef",
     "PutSchemaFromJsonRequestRequestTypeDef",
-    "PutSchemaFromJsonResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "TagTypeDef",
-    "TypedLinkSchemaAndFacetNameOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateObjectAttributesResponseTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
-    "UpdateSchemaResponseTypeDef",
     "UpgradeAppliedSchemaRequestRequestTypeDef",
-    "UpgradeAppliedSchemaResponseTypeDef",
     "UpgradePublishedSchemaRequestRequestTypeDef",
-    "UpgradePublishedSchemaResponseTypeDef",
     "AttachObjectRequestRequestTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachToIndexRequestRequestTypeDef",
     "BatchAttachObjectTypeDef",
     "BatchAttachPolicyTypeDef",
     "BatchAttachToIndexTypeDef",
     "BatchDeleteObjectTypeDef",
@@ -161,58 +113,100 @@
     "BatchListPolicyAttachmentsTypeDef",
     "BatchLookupPolicyTypeDef",
     "DeleteObjectRequestRequestTypeDef",
     "DetachFromIndexRequestRequestTypeDef",
     "DetachObjectRequestRequestTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "GetObjectInformationRequestRequestTypeDef",
-    "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     "ListAttachedIndicesRequestRequestTypeDef",
     "ListObjectChildrenRequestRequestTypeDef",
-    "ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
     "ListObjectParentPathsRequestRequestTypeDef",
     "ListObjectParentsRequestRequestTypeDef",
-    "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
     "ListObjectPoliciesRequestRequestTypeDef",
-    "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
     "ListPolicyAttachmentsRequestRequestTypeDef",
-    "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "LookupPolicyRequestRequestTypeDef",
     "BatchGetObjectAttributesTypeDef",
+    "BatchGetObjectInformationResponseTypeDef",
     "BatchListObjectAttributesTypeDef",
     "BatchRemoveFacetFromObjectTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
-    "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     "ListObjectAttributesRequestRequestTypeDef",
     "RemoveFacetFromObjectRequestRequestTypeDef",
-    "AttributeKeyAndValueOutputTypeDef",
-    "AttributeNameAndValueOutputTypeDef",
+    "ApplySchemaResponseTypeDef",
+    "AttachObjectResponseTypeDef",
+    "AttachToIndexResponseTypeDef",
+    "CreateDirectoryResponseTypeDef",
+    "CreateIndexResponseTypeDef",
+    "CreateObjectResponseTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "DeleteDirectoryResponseTypeDef",
+    "DeleteSchemaResponseTypeDef",
+    "DetachFromIndexResponseTypeDef",
+    "DetachObjectResponseTypeDef",
+    "DisableDirectoryResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EnableDirectoryResponseTypeDef",
+    "GetAppliedSchemaVersionResponseTypeDef",
+    "GetObjectInformationResponseTypeDef",
+    "GetSchemaAsJsonResponseTypeDef",
+    "GetTypedLinkFacetInformationResponseTypeDef",
+    "ListAppliedSchemaArnsResponseTypeDef",
+    "ListDevelopmentSchemaArnsResponseTypeDef",
+    "ListFacetNamesResponseTypeDef",
+    "ListManagedSchemaArnsResponseTypeDef",
+    "ListObjectChildrenResponseTypeDef",
+    "ListObjectPoliciesResponseTypeDef",
+    "ListPolicyAttachmentsResponseTypeDef",
+    "ListPublishedSchemaArnsResponseTypeDef",
+    "ListTypedLinkFacetNamesResponseTypeDef",
+    "PublishSchemaResponseTypeDef",
+    "PutSchemaFromJsonResponseTypeDef",
+    "UpdateObjectAttributesResponseTypeDef",
+    "UpdateSchemaResponseTypeDef",
+    "UpgradeAppliedSchemaResponseTypeDef",
+    "UpgradePublishedSchemaResponseTypeDef",
     "BatchCreateIndexTypeDef",
     "CreateIndexRequestRequestTypeDef",
+    "AttributeKeyAndValueOutputTypeDef",
+    "AttributeNameAndValueOutputTypeDef",
     "AttributeKeyAndValueTypeDef",
     "AttributeNameAndValueTypeDef",
     "LinkAttributeActionTypeDef",
     "ObjectAttributeActionTypeDef",
     "TypedAttributeValueRangeTypeDef",
-    "BatchGetObjectInformationResponseTypeDef",
-    "GetObjectInformationResponseTypeDef",
     "BatchListObjectParentPathsResponseTypeDef",
     "ListObjectParentPathsResponseTypeDef",
     "BatchListObjectParentsResponseTypeDef",
     "ListObjectParentsResponseTypeDef",
     "GetDirectoryResponseTypeDef",
     "ListDirectoriesResponseTypeDef",
     "FacetAttributeDefinitionOutputTypeDef",
     "TypedLinkAttributeDefinitionOutputTypeDef",
     "FacetAttributeDefinitionTypeDef",
     "TypedLinkAttributeDefinitionTypeDef",
     "GetFacetResponseTypeDef",
+    "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
+    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
+    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
+    "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
+    "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
+    "ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
+    "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PolicyToPathTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "PolicyToPathTypeDef",
     "BatchGetLinkAttributesResponseTypeDef",
     "BatchGetObjectAttributesResponseTypeDef",
     "BatchListObjectAttributesResponseTypeDef",
     "GetLinkAttributesResponseTypeDef",
     "GetObjectAttributesResponseTypeDef",
     "IndexAttachmentTypeDef",
     "ListObjectAttributesResponseTypeDef",
@@ -300,49 +294,35 @@
     "ApplySchemaRequestRequestTypeDef",
     {
         "PublishedSchemaArn": str,
         "DirectoryArn": str,
     },
 )
 
-ApplySchemaResponseTypeDef = TypedDict(
-    "ApplySchemaResponseTypeDef",
-    {
-        "AppliedSchemaArn": str,
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AttachObjectResponseTypeDef = TypedDict(
-    "AttachObjectResponseTypeDef",
-    {
-        "AttachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AttachToIndexResponseTypeDef = TypedDict(
-    "AttachToIndexResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AttachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TypedLinkSchemaAndFacetNameTypeDef = TypedDict(
     "TypedLinkSchemaAndFacetNameTypeDef",
     {
         "SchemaArn": str,
         "TypedLinkName": str,
     },
 )
 
-AttributeKeyOutputTypeDef = TypedDict(
-    "AttributeKeyOutputTypeDef",
+AttributeKeyTypeDef = TypedDict(
+    "AttributeKeyTypeDef",
     {
         "SchemaArn": str,
         "FacetName": str,
         "Name": str,
     },
 )
 
@@ -354,23 +334,14 @@
         "BooleanValue": bool,
         "NumberValue": str,
         "DatetimeValue": datetime,
     },
     total=False,
 )
 
-AttributeKeyTypeDef = TypedDict(
-    "AttributeKeyTypeDef",
-    {
-        "SchemaArn": str,
-        "FacetName": str,
-        "Name": str,
-    },
-)
-
 TypedAttributeValueTypeDef = TypedDict(
     "TypedAttributeValueTypeDef",
     {
         "StringValue": str,
         "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
         "BooleanValue": bool,
         "NumberValue": str,
@@ -423,23 +394,14 @@
     "BatchDetachObjectResponseTypeDef",
     {
         "detachedObjectIdentifier": str,
     },
     total=False,
 )
 
-SchemaFacetOutputTypeDef = TypedDict(
-    "SchemaFacetOutputTypeDef",
-    {
-        "SchemaArn": str,
-        "FacetName": str,
-    },
-    total=False,
-)
-
 BatchListObjectChildrenResponseTypeDef = TypedDict(
     "BatchListObjectChildrenResponseTypeDef",
     {
         "Children": Dict[str, str],
         "NextToken": str,
     },
     total=False,
@@ -502,71 +464,28 @@
     "CreateDirectoryRequestRequestTypeDef",
     {
         "Name": str,
         "SchemaArn": str,
     },
 )
 
-CreateDirectoryResponseTypeDef = TypedDict(
-    "CreateDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "Name": str,
-        "ObjectIdentifier": str,
-        "AppliedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateIndexResponseTypeDef = TypedDict(
-    "CreateIndexResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateObjectResponseTypeDef = TypedDict(
-    "CreateObjectResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSchemaRequestRequestTypeDef = TypedDict(
     "CreateSchemaRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDirectoryRequestRequestTypeDef = TypedDict(
     "DeleteDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-DeleteDirectoryResponseTypeDef = TypedDict(
-    "DeleteDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFacetRequestRequestTypeDef = TypedDict(
     "DeleteFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -574,46 +493,22 @@
 DeleteSchemaRequestRequestTypeDef = TypedDict(
     "DeleteSchemaRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
-DeleteSchemaResponseTypeDef = TypedDict(
-    "DeleteSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTypedLinkFacetRequestRequestTypeDef = TypedDict(
     "DeleteTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-DetachFromIndexResponseTypeDef = TypedDict(
-    "DetachFromIndexResponseTypeDef",
-    {
-        "DetachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DetachObjectResponseTypeDef = TypedDict(
-    "DetachObjectResponseTypeDef",
-    {
-        "DetachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DirectoryTypeDef = TypedDict(
     "DirectoryTypeDef",
     {
         "Name": str,
         "DirectoryArn": str,
         "State": DirectoryStateType,
         "CreationDateTime": datetime,
@@ -624,44 +519,21 @@
 DisableDirectoryRequestRequestTypeDef = TypedDict(
     "DisableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-DisableDirectoryResponseTypeDef = TypedDict(
-    "DisableDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
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
 EnableDirectoryRequestRequestTypeDef = TypedDict(
     "EnableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-EnableDirectoryResponseTypeDef = TypedDict(
-    "EnableDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RuleOutputTypeDef = TypedDict(
     "RuleOutputTypeDef",
     {
         "Type": RuleTypeType,
         "Parameters": Dict[str, str],
     },
     total=False,
@@ -672,22 +544,14 @@
     {
         "Type": RuleTypeType,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
-FacetAttributeReferenceOutputTypeDef = TypedDict(
-    "FacetAttributeReferenceOutputTypeDef",
-    {
-        "TargetFacetName": str,
-        "TargetAttributeName": str,
-    },
-)
-
 FacetAttributeReferenceTypeDef = TypedDict(
     "FacetAttributeReferenceTypeDef",
     {
         "TargetFacetName": str,
         "TargetAttributeName": str,
     },
 )
@@ -705,22 +569,14 @@
 GetAppliedSchemaVersionRequestRequestTypeDef = TypedDict(
     "GetAppliedSchemaVersionRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
-GetAppliedSchemaVersionResponseTypeDef = TypedDict(
-    "GetAppliedSchemaVersionResponseTypeDef",
-    {
-        "AppliedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDirectoryRequestRequestTypeDef = TypedDict(
     "GetDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
@@ -735,60 +591,32 @@
 GetSchemaAsJsonRequestRequestTypeDef = TypedDict(
     "GetSchemaAsJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
-GetSchemaAsJsonResponseTypeDef = TypedDict(
-    "GetSchemaAsJsonResponseTypeDef",
-    {
-        "Name": str,
-        "Document": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTypedLinkFacetInformationRequestRequestTypeDef = TypedDict(
     "GetTypedLinkFacetInformationRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-GetTypedLinkFacetInformationResponseTypeDef = TypedDict(
-    "GetTypedLinkFacetInformationResponseTypeDef",
-    {
-        "IdentityAttributeOrder": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
-    "_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-    },
-)
-_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
-    "_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "SchemaArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef(
-    _RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-    _OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAppliedSchemaArnsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppliedSchemaArnsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 _OptionalListAppliedSchemaArnsRequestRequestTypeDef = TypedDict(
@@ -803,89 +631,33 @@
 
 class ListAppliedSchemaArnsRequestRequestTypeDef(
     _RequiredListAppliedSchemaArnsRequestRequestTypeDef,
     _OptionalListAppliedSchemaArnsRequestRequestTypeDef,
 ):
     pass
 
-ListAppliedSchemaArnsResponseTypeDef = TypedDict(
-    "ListAppliedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef = TypedDict(
-    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDevelopmentSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListDevelopmentSchemaArnsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDevelopmentSchemaArnsResponseTypeDef = TypedDict(
-    "ListDevelopmentSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDirectoriesRequestListDirectoriesPaginateTypeDef = TypedDict(
-    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
-    {
-        "state": DirectoryStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDirectoriesRequestRequestTypeDef = TypedDict(
     "ListDirectoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "state": DirectoryStateType,
     },
     total=False,
 )
 
-_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFacetAttributesRequestListFacetAttributesPaginateTypeDef(
-    _RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-    _OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-):
-    pass
-
 _RequiredListFacetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacetAttributesRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -900,34 +672,14 @@
 
 class ListFacetAttributesRequestRequestTypeDef(
     _RequiredListFacetAttributesRequestRequestTypeDef,
     _OptionalListFacetAttributesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
-    "_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-    },
-)
-_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
-    "_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFacetNamesRequestListFacetNamesPaginateTypeDef(
-    _RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef,
-    _OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef,
-):
-    pass
-
 _RequiredListFacetNamesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacetNamesRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 _OptionalListFacetNamesRequestRequestTypeDef = TypedDict(
@@ -940,126 +692,34 @@
 )
 
 class ListFacetNamesRequestRequestTypeDef(
     _RequiredListFacetNamesRequestRequestTypeDef, _OptionalListFacetNamesRequestRequestTypeDef
 ):
     pass
 
-ListFacetNamesResponseTypeDef = TypedDict(
-    "ListFacetNamesResponseTypeDef",
-    {
-        "FacetNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef = TypedDict(
-    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListManagedSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListManagedSchemaArnsRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListManagedSchemaArnsResponseTypeDef = TypedDict(
-    "ListManagedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListObjectChildrenResponseTypeDef = TypedDict(
-    "ListObjectChildrenResponseTypeDef",
-    {
-        "Children": Dict[str, str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListObjectPoliciesResponseTypeDef = TypedDict(
-    "ListObjectPoliciesResponseTypeDef",
-    {
-        "AttachedPolicyIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPolicyAttachmentsResponseTypeDef = TypedDict(
-    "ListPolicyAttachmentsResponseTypeDef",
-    {
-        "ObjectIdentifiers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef = TypedDict(
-    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPublishedSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListPublishedSchemaArnsRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListPublishedSchemaArnsResponseTypeDef = TypedDict(
-    "ListPublishedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1073,44 +733,23 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef(
-    _RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-    _OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-):
-    pass
-
 _RequiredListTypedLinkFacetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypedLinkFacetAttributesRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -1125,34 +764,14 @@
 
 class ListTypedLinkFacetAttributesRequestRequestTypeDef(
     _RequiredListTypedLinkFacetAttributesRequestRequestTypeDef,
     _OptionalListTypedLinkFacetAttributesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
-    "_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-    },
-)
-_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
-    "_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef(
-    _RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-    _OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-):
-    pass
-
 _RequiredListTypedLinkFacetNamesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypedLinkFacetNamesRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 _OptionalListTypedLinkFacetNamesRequestRequestTypeDef = TypedDict(
@@ -1166,41 +785,14 @@
 
 class ListTypedLinkFacetNamesRequestRequestTypeDef(
     _RequiredListTypedLinkFacetNamesRequestRequestTypeDef,
     _OptionalListTypedLinkFacetNamesRequestRequestTypeDef,
 ):
     pass
 
-ListTypedLinkFacetNamesResponseTypeDef = TypedDict(
-    "ListTypedLinkFacetNamesResponseTypeDef",
-    {
-        "FacetNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ObjectReferenceOutputTypeDef = TypedDict(
-    "ObjectReferenceOutputTypeDef",
-    {
-        "Selector": str,
-    },
-    total=False,
-)
-
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
 PolicyAttachmentTypeDef = TypedDict(
     "PolicyAttachmentTypeDef",
     {
         "PolicyId": str,
         "ObjectIdentifier": str,
         "PolicyType": str,
     },
@@ -1224,98 +816,38 @@
 )
 
 class PublishSchemaRequestRequestTypeDef(
     _RequiredPublishSchemaRequestRequestTypeDef, _OptionalPublishSchemaRequestRequestTypeDef
 ):
     pass
 
-PublishSchemaResponseTypeDef = TypedDict(
-    "PublishSchemaResponseTypeDef",
-    {
-        "PublishedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutSchemaFromJsonRequestRequestTypeDef = TypedDict(
     "PutSchemaFromJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Document": str,
     },
 )
 
-PutSchemaFromJsonResponseTypeDef = TypedDict(
-    "PutSchemaFromJsonResponseTypeDef",
-    {
-        "Arn": str,
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
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-TypedLinkSchemaAndFacetNameOutputTypeDef = TypedDict(
-    "TypedLinkSchemaAndFacetNameOutputTypeDef",
-    {
-        "SchemaArn": str,
-        "TypedLinkName": str,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateObjectAttributesResponseTypeDef = TypedDict(
-    "UpdateObjectAttributesResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSchemaRequestRequestTypeDef = TypedDict(
     "UpdateSchemaRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-UpdateSchemaResponseTypeDef = TypedDict(
-    "UpdateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpgradeAppliedSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradeAppliedSchemaRequestRequestTypeDef",
     {
         "PublishedSchemaArn": str,
         "DirectoryArn": str,
     },
 )
@@ -1329,23 +861,14 @@
 
 class UpgradeAppliedSchemaRequestRequestTypeDef(
     _RequiredUpgradeAppliedSchemaRequestRequestTypeDef,
     _OptionalUpgradeAppliedSchemaRequestRequestTypeDef,
 ):
     pass
 
-UpgradeAppliedSchemaResponseTypeDef = TypedDict(
-    "UpgradeAppliedSchemaResponseTypeDef",
-    {
-        "UpgradedSchemaArn": str,
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpgradePublishedSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradePublishedSchemaRequestRequestTypeDef",
     {
         "DevelopmentSchemaArn": str,
         "PublishedSchemaArn": str,
         "MinorVersion": str,
     },
@@ -1360,22 +883,14 @@
 
 class UpgradePublishedSchemaRequestRequestTypeDef(
     _RequiredUpgradePublishedSchemaRequestRequestTypeDef,
     _OptionalUpgradePublishedSchemaRequestRequestTypeDef,
 ):
     pass
 
-UpgradePublishedSchemaResponseTypeDef = TypedDict(
-    "UpgradePublishedSchemaResponseTypeDef",
-    {
-        "UpgradedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttachObjectRequestRequestTypeDef = TypedDict(
     "AttachObjectRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ParentReference": ObjectReferenceTypeDef,
         "ChildReference": ObjectReferenceTypeDef,
         "LinkName": str,
@@ -1667,36 +1182,14 @@
 
 class GetObjectInformationRequestRequestTypeDef(
     _RequiredGetObjectInformationRequestRequestTypeDef,
     _OptionalGetObjectInformationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "TargetReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef(
-    _RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-    _OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAttachedIndicesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedIndicesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "TargetReference": ObjectReferenceTypeDef,
     },
 )
@@ -1735,35 +1228,14 @@
 
 class ListObjectChildrenRequestRequestTypeDef(
     _RequiredListObjectChildrenRequestRequestTypeDef,
     _OptionalListObjectChildrenRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef(
-    _RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-    _OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-):
-    pass
-
 _RequiredListObjectParentPathsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectParentPathsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1801,36 +1273,14 @@
 )
 
 class ListObjectParentsRequestRequestTypeDef(
     _RequiredListObjectParentsRequestRequestTypeDef, _OptionalListObjectParentsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef(
-    _RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-    _OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredListObjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectPoliciesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1846,36 +1296,14 @@
 
 class ListObjectPoliciesRequestRequestTypeDef(
     _RequiredListObjectPoliciesRequestRequestTypeDef,
     _OptionalListObjectPoliciesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "PolicyReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef(
-    _RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-    _OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPolicyAttachmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyAttachmentsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "PolicyReference": ObjectReferenceTypeDef,
     },
 )
@@ -1891,35 +1319,14 @@
 
 class ListPolicyAttachmentsRequestRequestTypeDef(
     _RequiredListPolicyAttachmentsRequestRequestTypeDef,
     _OptionalListPolicyAttachmentsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
-    "_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
-    "_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class LookupPolicyRequestLookupPolicyPaginateTypeDef(
-    _RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef,
-    _OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef,
-):
-    pass
-
 _RequiredLookupPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredLookupPolicyRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1942,14 +1349,23 @@
     {
         "ObjectReference": ObjectReferenceTypeDef,
         "SchemaFacet": SchemaFacetTypeDef,
         "AttributeNames": Sequence[str],
     },
 )
 
+BatchGetObjectInformationResponseTypeDef = TypedDict(
+    "BatchGetObjectInformationResponseTypeDef",
+    {
+        "SchemaFacets": List[SchemaFacetTypeDef],
+        "ObjectIdentifier": str,
+    },
+    total=False,
+)
+
 _RequiredBatchListObjectAttributesTypeDef = TypedDict(
     "_RequiredBatchListObjectAttributesTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListObjectAttributesTypeDef = TypedDict(
@@ -1994,37 +1410,14 @@
 
 class GetObjectAttributesRequestRequestTypeDef(
     _RequiredGetObjectAttributesRequestRequestTypeDef,
     _OptionalGetObjectAttributesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "FacetFilter": SchemaFacetTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListObjectAttributesRequestListObjectAttributesPaginateTypeDef(
-    _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-    _OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-):
-    pass
-
 _RequiredListObjectAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectAttributesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -2050,27 +1443,290 @@
     {
         "DirectoryArn": str,
         "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 
-AttributeKeyAndValueOutputTypeDef = TypedDict(
-    "AttributeKeyAndValueOutputTypeDef",
+ApplySchemaResponseTypeDef = TypedDict(
+    "ApplySchemaResponseTypeDef",
     {
-        "Key": AttributeKeyOutputTypeDef,
-        "Value": TypedAttributeValueOutputTypeDef,
+        "AppliedSchemaArn": str,
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AttributeNameAndValueOutputTypeDef = TypedDict(
-    "AttributeNameAndValueOutputTypeDef",
+AttachObjectResponseTypeDef = TypedDict(
+    "AttachObjectResponseTypeDef",
     {
-        "AttributeName": str,
-        "Value": TypedAttributeValueOutputTypeDef,
+        "AttachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachToIndexResponseTypeDef = TypedDict(
+    "AttachToIndexResponseTypeDef",
+    {
+        "AttachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDirectoryResponseTypeDef = TypedDict(
+    "CreateDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "Name": str,
+        "ObjectIdentifier": str,
+        "AppliedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIndexResponseTypeDef = TypedDict(
+    "CreateIndexResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateObjectResponseTypeDef = TypedDict(
+    "CreateObjectResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDirectoryResponseTypeDef = TypedDict(
+    "DeleteDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSchemaResponseTypeDef = TypedDict(
+    "DeleteSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachFromIndexResponseTypeDef = TypedDict(
+    "DetachFromIndexResponseTypeDef",
+    {
+        "DetachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachObjectResponseTypeDef = TypedDict(
+    "DetachObjectResponseTypeDef",
+    {
+        "DetachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableDirectoryResponseTypeDef = TypedDict(
+    "DisableDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
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
+EnableDirectoryResponseTypeDef = TypedDict(
+    "EnableDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppliedSchemaVersionResponseTypeDef = TypedDict(
+    "GetAppliedSchemaVersionResponseTypeDef",
+    {
+        "AppliedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetObjectInformationResponseTypeDef = TypedDict(
+    "GetObjectInformationResponseTypeDef",
+    {
+        "SchemaFacets": List[SchemaFacetTypeDef],
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSchemaAsJsonResponseTypeDef = TypedDict(
+    "GetSchemaAsJsonResponseTypeDef",
+    {
+        "Name": str,
+        "Document": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTypedLinkFacetInformationResponseTypeDef = TypedDict(
+    "GetTypedLinkFacetInformationResponseTypeDef",
+    {
+        "IdentityAttributeOrder": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAppliedSchemaArnsResponseTypeDef = TypedDict(
+    "ListAppliedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDevelopmentSchemaArnsResponseTypeDef = TypedDict(
+    "ListDevelopmentSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFacetNamesResponseTypeDef = TypedDict(
+    "ListFacetNamesResponseTypeDef",
+    {
+        "FacetNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListManagedSchemaArnsResponseTypeDef = TypedDict(
+    "ListManagedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListObjectChildrenResponseTypeDef = TypedDict(
+    "ListObjectChildrenResponseTypeDef",
+    {
+        "Children": Dict[str, str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListObjectPoliciesResponseTypeDef = TypedDict(
+    "ListObjectPoliciesResponseTypeDef",
+    {
+        "AttachedPolicyIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPolicyAttachmentsResponseTypeDef = TypedDict(
+    "ListPolicyAttachmentsResponseTypeDef",
+    {
+        "ObjectIdentifiers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPublishedSchemaArnsResponseTypeDef = TypedDict(
+    "ListPublishedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTypedLinkFacetNamesResponseTypeDef = TypedDict(
+    "ListTypedLinkFacetNamesResponseTypeDef",
+    {
+        "FacetNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishSchemaResponseTypeDef = TypedDict(
+    "PublishSchemaResponseTypeDef",
+    {
+        "PublishedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutSchemaFromJsonResponseTypeDef = TypedDict(
+    "PutSchemaFromJsonResponseTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateObjectAttributesResponseTypeDef = TypedDict(
+    "UpdateObjectAttributesResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSchemaResponseTypeDef = TypedDict(
+    "UpdateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpgradeAppliedSchemaResponseTypeDef = TypedDict(
+    "UpgradeAppliedSchemaResponseTypeDef",
+    {
+        "UpgradedSchemaArn": str,
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpgradePublishedSchemaResponseTypeDef = TypedDict(
+    "UpgradePublishedSchemaResponseTypeDef",
+    {
+        "UpgradedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchCreateIndexTypeDef = TypedDict(
     "_RequiredBatchCreateIndexTypeDef",
     {
         "OrderedIndexedAttributeList": Sequence[AttributeKeyTypeDef],
@@ -2108,14 +1764,30 @@
 )
 
 class CreateIndexRequestRequestTypeDef(
     _RequiredCreateIndexRequestRequestTypeDef, _OptionalCreateIndexRequestRequestTypeDef
 ):
     pass
 
+AttributeKeyAndValueOutputTypeDef = TypedDict(
+    "AttributeKeyAndValueOutputTypeDef",
+    {
+        "Key": AttributeKeyTypeDef,
+        "Value": TypedAttributeValueOutputTypeDef,
+    },
+)
+
+AttributeNameAndValueOutputTypeDef = TypedDict(
+    "AttributeNameAndValueOutputTypeDef",
+    {
+        "AttributeName": str,
+        "Value": TypedAttributeValueOutputTypeDef,
+    },
+)
+
 AttributeKeyAndValueTypeDef = TypedDict(
     "AttributeKeyAndValueTypeDef",
     {
         "Key": AttributeKeyTypeDef,
         "Value": TypedAttributeValueTypeDef,
     },
 )
@@ -2163,47 +1835,29 @@
 )
 
 class TypedAttributeValueRangeTypeDef(
     _RequiredTypedAttributeValueRangeTypeDef, _OptionalTypedAttributeValueRangeTypeDef
 ):
     pass
 
-BatchGetObjectInformationResponseTypeDef = TypedDict(
-    "BatchGetObjectInformationResponseTypeDef",
-    {
-        "SchemaFacets": List[SchemaFacetOutputTypeDef],
-        "ObjectIdentifier": str,
-    },
-    total=False,
-)
-
-GetObjectInformationResponseTypeDef = TypedDict(
-    "GetObjectInformationResponseTypeDef",
-    {
-        "SchemaFacets": List[SchemaFacetOutputTypeDef],
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchListObjectParentPathsResponseTypeDef = TypedDict(
     "BatchListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
 ListObjectParentPathsResponseTypeDef = TypedDict(
     "ListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchListObjectParentsResponseTypeDef = TypedDict(
     "BatchListObjectParentsResponseTypeDef",
     {
         "ParentLinks": List[ObjectIdentifierAndLinkNameTupleTypeDef],
@@ -2214,32 +1868,32 @@
 
 ListObjectParentsResponseTypeDef = TypedDict(
     "ListObjectParentsResponseTypeDef",
     {
         "Parents": Dict[str, str],
         "NextToken": str,
         "ParentLinks": List[ObjectIdentifierAndLinkNameTupleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDirectoryResponseTypeDef = TypedDict(
     "GetDirectoryResponseTypeDef",
     {
         "Directory": DirectoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDirectoriesResponseTypeDef = TypedDict(
     "ListDirectoriesResponseTypeDef",
     {
         "Directories": List[DirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFacetAttributeDefinitionOutputTypeDef = TypedDict(
     "_RequiredFacetAttributeDefinitionOutputTypeDef",
     {
         "Type": FacetAttributeTypeType,
@@ -2328,44 +1982,333 @@
 ):
     pass
 
 GetFacetResponseTypeDef = TypedDict(
     "GetFacetResponseTypeDef",
     {
         "Facet": FacetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
+    "_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DirectoryArn": str,
+    },
+)
+_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
+    "_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-PolicyToPathTypeDef = TypedDict(
-    "PolicyToPathTypeDef",
+class ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef(
+    _RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    _OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+):
+    pass
+
+_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     {
-        "Path": str,
-        "Policies": List[PolicyAttachmentTypeDef],
+        "DirectoryArn": str,
+        "TargetReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef(
+    _RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+    _OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+):
+    pass
+
+ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef = TypedDict(
+    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDirectoriesRequestListDirectoriesPaginateTypeDef = TypedDict(
+    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
+    {
+        "state": DirectoryStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFacetAttributesRequestListFacetAttributesPaginateTypeDef(
+    _RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+    _OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+):
+    pass
+
+_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
+    "_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+    },
+)
+_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
+    "_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFacetNamesRequestListFacetNamesPaginateTypeDef(
+    _RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef,
+    _OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef,
+):
+    pass
+
+ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef = TypedDict(
+    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "FacetFilter": SchemaFacetTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListObjectAttributesRequestListObjectAttributesPaginateTypeDef(
+    _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+    _OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+):
+    pass
+
+_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef(
+    _RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+    _OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+):
+    pass
+
+_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef(
+    _RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+    _OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "PolicyReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef(
+    _RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+    _OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+):
+    pass
+
+ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef = TypedDict(
+    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef(
+    _RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    _OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+):
+    pass
+
+_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
+    "_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+    },
+)
+_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
+    "_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef(
+    _RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+    _OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+):
+    pass
+
+_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
+    "_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
+    "_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class LookupPolicyRequestLookupPolicyPaginateTypeDef(
+    _RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef,
+    _OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef,
+):
+    pass
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+PolicyToPathTypeDef = TypedDict(
+    "PolicyToPathTypeDef",
+    {
+        "Path": str,
+        "Policies": List[PolicyAttachmentTypeDef],
+    },
+    total=False,
+)
+
 BatchGetLinkAttributesResponseTypeDef = TypedDict(
     "BatchGetLinkAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueOutputTypeDef],
     },
     total=False,
 )
@@ -2387,23 +2330,23 @@
     total=False,
 )
 
 GetLinkAttributesResponseTypeDef = TypedDict(
     "GetLinkAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectAttributesResponseTypeDef = TypedDict(
     "GetObjectAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IndexAttachmentTypeDef = TypedDict(
     "IndexAttachmentTypeDef",
     {
         "IndexedAttributes": List[AttributeKeyAndValueOutputTypeDef],
@@ -2413,24 +2356,24 @@
 )
 
 ListObjectAttributesResponseTypeDef = TypedDict(
     "ListObjectAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TypedLinkSpecifierOutputTypeDef = TypedDict(
     "TypedLinkSpecifierOutputTypeDef",
     {
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameOutputTypeDef,
-        "SourceObjectReference": ObjectReferenceOutputTypeDef,
-        "TargetObjectReference": ObjectReferenceOutputTypeDef,
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
+        "SourceObjectReference": ObjectReferenceTypeDef,
+        "TargetObjectReference": ObjectReferenceTypeDef,
         "IdentityAttributeValues": List[AttributeNameAndValueOutputTypeDef],
     },
 )
 
 _RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
     "_RequiredAddFacetToObjectRequestRequestTypeDef",
     {
@@ -2588,15 +2531,15 @@
         "Name": str,
     },
 )
 _OptionalFacetAttributeOutputTypeDef = TypedDict(
     "_OptionalFacetAttributeOutputTypeDef",
     {
         "AttributeDefinition": FacetAttributeDefinitionOutputTypeDef,
-        "AttributeReference": FacetAttributeReferenceOutputTypeDef,
+        "AttributeReference": FacetAttributeReferenceTypeDef,
         "RequiredBehavior": RequiredAttributeBehaviorType,
     },
     total=False,
 )
 
 class FacetAttributeOutputTypeDef(
     _RequiredFacetAttributeOutputTypeDef, _OptionalFacetAttributeOutputTypeDef
@@ -2604,15 +2547,15 @@
     pass
 
 ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
     "ListTypedLinkFacetAttributesResponseTypeDef",
     {
         "Attributes": List[TypedLinkAttributeDefinitionOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFacetAttributeTypeDef = TypedDict(
     "_RequiredFacetAttributeTypeDef",
     {
         "Name": str,
@@ -2658,15 +2601,15 @@
 )
 
 LookupPolicyResponseTypeDef = TypedDict(
     "LookupPolicyResponseTypeDef",
     {
         "PolicyToPathList": List[PolicyToPathTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchListAttachedIndicesResponseTypeDef = TypedDict(
     "BatchListAttachedIndicesResponseTypeDef",
     {
         "IndexAttachments": List[IndexAttachmentTypeDef],
@@ -2685,32 +2628,32 @@
 )
 
 ListAttachedIndicesResponseTypeDef = TypedDict(
     "ListAttachedIndicesResponseTypeDef",
     {
         "IndexAttachments": List[IndexAttachmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIndexResponseTypeDef = TypedDict(
     "ListIndexResponseTypeDef",
     {
         "IndexAttachments": List[IndexAttachmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachTypedLinkResponseTypeDef = TypedDict(
     "AttachTypedLinkResponseTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchAttachTypedLinkResponseTypeDef = TypedDict(
     "BatchAttachTypedLinkResponseTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
@@ -2737,24 +2680,24 @@
 )
 
 ListIncomingTypedLinksResponseTypeDef = TypedDict(
     "ListIncomingTypedLinksResponseTypeDef",
     {
         "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOutgoingTypedLinksResponseTypeDef = TypedDict(
     "ListOutgoingTypedLinksResponseTypeDef",
     {
         "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDetachTypedLinkTypeDef = TypedDict(
     "BatchDetachTypedLinkTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
@@ -2859,15 +2802,15 @@
     },
 )
 _OptionalListIndexRequestListIndexPaginateTypeDef = TypedDict(
     "_OptionalListIndexRequestListIndexPaginateTypeDef",
     {
         "RangesOnIndexedValues": Sequence[ObjectAttributeRangeTypeDef],
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListIndexRequestListIndexPaginateTypeDef(
     _RequiredListIndexRequestListIndexPaginateTypeDef,
     _OptionalListIndexRequestListIndexPaginateTypeDef,
@@ -2950,15 +2893,15 @@
 )
 _OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef = TypedDict(
     "_OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     {
         "FilterAttributeRanges": Sequence[TypedLinkAttributeRangeTypeDef],
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef(
     _RequiredListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
     _OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
@@ -2999,15 +2942,15 @@
 )
 _OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef = TypedDict(
     "_OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     {
         "FilterAttributeRanges": Sequence[TypedLinkAttributeRangeTypeDef],
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef(
     _RequiredListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
     _OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
@@ -3040,15 +2983,15 @@
     pass
 
 ListFacetAttributesResponseTypeDef = TypedDict(
     "ListFacetAttributesResponseTypeDef",
     {
         "Attributes": List[FacetAttributeOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFacetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
@@ -3204,15 +3147,15 @@
 ):
     pass
 
 BatchWriteResponseTypeDef = TypedDict(
     "BatchWriteResponseTypeDef",
     {
         "Responses": List[BatchWriteOperationResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchReadOperationResponseTypeDef = TypedDict(
     "BatchReadOperationResponseTypeDef",
     {
         "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
@@ -3249,10 +3192,10 @@
 ):
     pass
 
 BatchReadResponseTypeDef = TypedDict(
     "BatchReadResponseTypeDef",
     {
         "Responses": List[BatchReadOperationResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/PKG-INFO` & `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-clouddirectory
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudDirectory 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudDirectory 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-clouddirectory)](https://pepy.tech/project/mypy-boto3-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudDirectory 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[boto3.CloudDirectory 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
 
@@ -419,117 +419,69 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_clouddirectory.type_defs import (
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
-    ApplySchemaResponseTypeDef,
-    AttachObjectResponseTypeDef,
-    AttachToIndexResponseTypeDef,
+    ResponseMetadataTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
-    AttributeKeyOutputTypeDef,
-    TypedAttributeValueOutputTypeDef,
     AttributeKeyTypeDef,
+    TypedAttributeValueOutputTypeDef,
     TypedAttributeValueTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
     BatchDetachFromIndexResponseTypeDef,
     BatchDetachObjectResponseTypeDef,
-    SchemaFacetOutputTypeDef,
     BatchListObjectChildrenResponseTypeDef,
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
     CreateDirectoryRequestRequestTypeDef,
-    CreateDirectoryResponseTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateObjectResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
-    DeleteDirectoryResponseTypeDef,
     DeleteFacetRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
-    DeleteSchemaResponseTypeDef,
     DeleteTypedLinkFacetRequestRequestTypeDef,
-    DetachFromIndexResponseTypeDef,
-    DetachObjectResponseTypeDef,
     DirectoryTypeDef,
     DisableDirectoryRequestRequestTypeDef,
-    DisableDirectoryResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableDirectoryRequestRequestTypeDef,
-    EnableDirectoryResponseTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
-    FacetAttributeReferenceOutputTypeDef,
     FacetAttributeReferenceTypeDef,
     FacetTypeDef,
     GetAppliedSchemaVersionRequestRequestTypeDef,
-    GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryRequestRequestTypeDef,
     GetFacetRequestRequestTypeDef,
     GetSchemaAsJsonRequestRequestTypeDef,
-    GetSchemaAsJsonResponseTypeDef,
     GetTypedLinkFacetInformationRequestRequestTypeDef,
-    GetTypedLinkFacetInformationResponseTypeDef,
-    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAppliedSchemaArnsRequestRequestTypeDef,
-    ListAppliedSchemaArnsResponseTypeDef,
-    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
     ListDevelopmentSchemaArnsRequestRequestTypeDef,
-    ListDevelopmentSchemaArnsResponseTypeDef,
-    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
     ListDirectoriesRequestRequestTypeDef,
-    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
     ListFacetAttributesRequestRequestTypeDef,
-    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
     ListFacetNamesRequestRequestTypeDef,
-    ListFacetNamesResponseTypeDef,
-    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
     ListManagedSchemaArnsRequestRequestTypeDef,
-    ListManagedSchemaArnsResponseTypeDef,
-    ListObjectChildrenResponseTypeDef,
-    ListObjectPoliciesResponseTypeDef,
-    ListPolicyAttachmentsResponseTypeDef,
-    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
     ListPublishedSchemaArnsRequestRequestTypeDef,
-    ListPublishedSchemaArnsResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    TagTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
-    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
-    ListTypedLinkFacetNamesResponseTypeDef,
-    ObjectReferenceOutputTypeDef,
-    PaginatorConfigTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
-    PublishSchemaResponseTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
-    PutSchemaFromJsonResponseTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
-    TypedLinkSchemaAndFacetNameOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
-    UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
-    UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
-    UpgradePublishedSchemaResponseTypeDef,
     AttachObjectRequestRequestTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachToIndexRequestRequestTypeDef,
     BatchAttachObjectTypeDef,
     BatchAttachPolicyTypeDef,
     BatchAttachToIndexTypeDef,
     BatchDeleteObjectTypeDef,
@@ -545,58 +497,100 @@
     BatchListPolicyAttachmentsTypeDef,
     BatchLookupPolicyTypeDef,
     DeleteObjectRequestRequestTypeDef,
     DetachFromIndexRequestRequestTypeDef,
     DetachObjectRequestRequestTypeDef,
     DetachPolicyRequestRequestTypeDef,
     GetObjectInformationRequestRequestTypeDef,
-    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
     ListAttachedIndicesRequestRequestTypeDef,
     ListObjectChildrenRequestRequestTypeDef,
-    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
     ListObjectParentPathsRequestRequestTypeDef,
     ListObjectParentsRequestRequestTypeDef,
-    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
     ListObjectPoliciesRequestRequestTypeDef,
-    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
     ListPolicyAttachmentsRequestRequestTypeDef,
-    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     LookupPolicyRequestRequestTypeDef,
     BatchGetObjectAttributesTypeDef,
+    BatchGetObjectInformationResponseTypeDef,
     BatchListObjectAttributesTypeDef,
     BatchRemoveFacetFromObjectTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
-    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
     ListObjectAttributesRequestRequestTypeDef,
     RemoveFacetFromObjectRequestRequestTypeDef,
-    AttributeKeyAndValueOutputTypeDef,
-    AttributeNameAndValueOutputTypeDef,
+    ApplySchemaResponseTypeDef,
+    AttachObjectResponseTypeDef,
+    AttachToIndexResponseTypeDef,
+    CreateDirectoryResponseTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateObjectResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    DeleteDirectoryResponseTypeDef,
+    DeleteSchemaResponseTypeDef,
+    DetachFromIndexResponseTypeDef,
+    DetachObjectResponseTypeDef,
+    DisableDirectoryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnableDirectoryResponseTypeDef,
+    GetAppliedSchemaVersionResponseTypeDef,
+    GetObjectInformationResponseTypeDef,
+    GetSchemaAsJsonResponseTypeDef,
+    GetTypedLinkFacetInformationResponseTypeDef,
+    ListAppliedSchemaArnsResponseTypeDef,
+    ListDevelopmentSchemaArnsResponseTypeDef,
+    ListFacetNamesResponseTypeDef,
+    ListManagedSchemaArnsResponseTypeDef,
+    ListObjectChildrenResponseTypeDef,
+    ListObjectPoliciesResponseTypeDef,
+    ListPolicyAttachmentsResponseTypeDef,
+    ListPublishedSchemaArnsResponseTypeDef,
+    ListTypedLinkFacetNamesResponseTypeDef,
+    PublishSchemaResponseTypeDef,
+    PutSchemaFromJsonResponseTypeDef,
+    UpdateObjectAttributesResponseTypeDef,
+    UpdateSchemaResponseTypeDef,
+    UpgradeAppliedSchemaResponseTypeDef,
+    UpgradePublishedSchemaResponseTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
+    AttributeKeyAndValueOutputTypeDef,
+    AttributeNameAndValueOutputTypeDef,
     AttributeKeyAndValueTypeDef,
     AttributeNameAndValueTypeDef,
     LinkAttributeActionTypeDef,
     ObjectAttributeActionTypeDef,
     TypedAttributeValueRangeTypeDef,
-    BatchGetObjectInformationResponseTypeDef,
-    GetObjectInformationResponseTypeDef,
     BatchListObjectParentPathsResponseTypeDef,
     ListObjectParentPathsResponseTypeDef,
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
     FacetAttributeDefinitionOutputTypeDef,
     TypedLinkAttributeDefinitionOutputTypeDef,
     FacetAttributeDefinitionTypeDef,
     TypedLinkAttributeDefinitionTypeDef,
     GetFacetResponseTypeDef,
+    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
+    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
+    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
+    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
+    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PolicyToPathTypeDef,
     TagResourceRequestRequestTypeDef,
+    PolicyToPathTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
     BatchGetObjectAttributesResponseTypeDef,
     BatchListObjectAttributesResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     IndexAttachmentTypeDef,
     ListObjectAttributesResponseTypeDef,
```

### Comparing `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/SOURCES.txt` & `mypy-boto3-clouddirectory-1.28.15/mypy_boto3_clouddirectory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.12/setup.py` & `mypy-boto3-clouddirectory-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-clouddirectory",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_clouddirectory"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudDirectory 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CloudDirectory 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

