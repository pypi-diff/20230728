# Comparing `tmp/mypy-boto3-imagebuilder-1.28.12.tar.gz` & `tmp/mypy-boto3-imagebuilder-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-imagebuilder-1.28.12.tar", last modified: Thu Jul 27 05:34:46 2023, max compression
+gzip compressed data, was "mypy-boto3-imagebuilder-1.28.15.tar", last modified: Fri Jul 28 20:42:56 2023, max compression
```

## Comparing `mypy-boto3-imagebuilder-1.28.12.tar` & `mypy-boto3-imagebuilder-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.900492 mypy-boto3-imagebuilder-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20617 2023-07-27 05:34:46.900492 mypy-boto3-imagebuilder-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.900492 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41846 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41783 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-27 05:23:31.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75575 2023-07-27 05:23:32.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75508 2023-07-27 05:23:31.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.900492 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20617 2023-07-27 05:34:46.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 05:34:46.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:46.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:46.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:46.900492 mypy-boto3-imagebuilder-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.269213 mypy-boto3-imagebuilder-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-28 20:42:56.269213 mypy-boto3-imagebuilder-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.265213 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41846 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41783 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-28 20:27:38.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-28 20:27:38.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70382 2023-07-28 20:27:40.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70321 2023-07-28 20:27:39.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.269213 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-28 20:42:56.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 20:42:56.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:56.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:56.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:56.269213 mypy-boto3-imagebuilder-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/setup.py
```

### Comparing `mypy-boto3-imagebuilder-1.28.12/LICENSE` & `mypy-boto3-imagebuilder-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.12/PKG-INFO` & `mypy-boto3-imagebuilder-1.28.15/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-imagebuilder
-Version: 1.28.12
-Summary: Type annotations for boto3.imagebuilder 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 imagebuilder type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-imagebuilder"></a>
 
 # mypy-boto3-imagebuilder
 
 [![PyPI - mypy-boto3-imagebuilder](https://img.shields.io/pypi/v/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-imagebuilder)](https://pepy.tech/project/mypy-boto3-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.imagebuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[boto3.imagebuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [mypy-boto3-imagebuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,155 +284,141 @@
 
 `mypy_boto3_imagebuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_imagebuilder.type_defs import (
     SeverityCountsTypeDef,
-    SystemsManagerAgentOutputTypeDef,
     SystemsManagerAgentTypeDef,
     LaunchPermissionConfigurationOutputTypeDef,
     LaunchPermissionConfigurationTypeDef,
     ImageStateTypeDef,
     CancelImageCreationRequestRequestTypeDef,
-    CancelImageCreationResponseTypeDef,
+    ResponseMetadataTypeDef,
     ComponentParameterOutputTypeDef,
     ComponentParameterTypeDef,
     ComponentParameterDetailTypeDef,
     ComponentStateTypeDef,
     ComponentVersionTypeDef,
-    TargetContainerRepositoryOutputTypeDef,
     TargetContainerRepositoryTypeDef,
     ContainerRecipeSummaryTypeDef,
     ContainerTypeDef,
     CreateComponentRequestRequestTypeDef,
-    CreateComponentResponseTypeDef,
-    CreateContainerRecipeResponseTypeDef,
-    CreateDistributionConfigurationResponseTypeDef,
     ImageTestsConfigurationTypeDef,
     ScheduleTypeDef,
-    CreateImagePipelineResponseTypeDef,
-    CreateImageRecipeResponseTypeDef,
-    CreateImageResponseTypeDef,
     InstanceMetadataOptionsTypeDef,
-    CreateInfrastructureConfigurationResponseTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteComponentRequestRequestTypeDef,
-    DeleteComponentResponseTypeDef,
     DeleteContainerRecipeRequestRequestTypeDef,
-    DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationRequestRequestTypeDef,
-    DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineRequestRequestTypeDef,
-    DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeRequestRequestTypeDef,
-    DeleteImageRecipeResponseTypeDef,
     DeleteImageRequestRequestTypeDef,
-    DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationRequestRequestTypeDef,
-    DeleteInfrastructureConfigurationResponseTypeDef,
     DistributionConfigurationSummaryTypeDef,
-    LaunchTemplateConfigurationOutputTypeDef,
-    S3ExportConfigurationOutputTypeDef,
     LaunchTemplateConfigurationTypeDef,
     S3ExportConfigurationTypeDef,
-    EbsInstanceBlockDeviceSpecificationOutputTypeDef,
     EbsInstanceBlockDeviceSpecificationTypeDef,
     EcrConfigurationOutputTypeDef,
     EcrConfigurationTypeDef,
-    FastLaunchLaunchTemplateSpecificationOutputTypeDef,
-    FastLaunchSnapshotConfigurationOutputTypeDef,
     FastLaunchLaunchTemplateSpecificationTypeDef,
     FastLaunchSnapshotConfigurationTypeDef,
     FilterTypeDef,
     GetComponentPolicyRequestRequestTypeDef,
-    GetComponentPolicyResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetContainerRecipePolicyRequestRequestTypeDef,
-    GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeRequestRequestTypeDef,
     GetDistributionConfigurationRequestRequestTypeDef,
     GetImagePipelineRequestRequestTypeDef,
     GetImagePolicyRequestRequestTypeDef,
-    GetImagePolicyResponseTypeDef,
     GetImageRecipePolicyRequestRequestTypeDef,
-    GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeRequestRequestTypeDef,
     GetImageRequestRequestTypeDef,
     GetInfrastructureConfigurationRequestRequestTypeDef,
     GetWorkflowExecutionRequestRequestTypeDef,
-    GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionRequestRequestTypeDef,
-    GetWorkflowStepExecutionResponseTypeDef,
     ImagePackageTypeDef,
-    ImageTestsConfigurationOutputTypeDef,
-    ScheduleOutputTypeDef,
     ImageRecipeSummaryTypeDef,
     ImageScanFindingsFilterTypeDef,
     ImageScanStateTypeDef,
     ImageVersionTypeDef,
     ImportComponentRequestRequestTypeDef,
-    ImportComponentResponseTypeDef,
     ImportVmImageRequestRequestTypeDef,
-    ImportVmImageResponseTypeDef,
     InfrastructureConfigurationSummaryTypeDef,
-    InstanceMetadataOptionsOutputTypeDef,
     ListComponentBuildVersionsRequestRequestTypeDef,
     ListImagePackagesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkflowExecutionsRequestRequestTypeDef,
     WorkflowExecutionMetadataTypeDef,
     ListWorkflowStepExecutionsRequestRequestTypeDef,
     WorkflowStepMetadataTypeDef,
-    S3LogsOutputTypeDef,
     S3LogsTypeDef,
     VulnerablePackageTypeDef,
     PutComponentPolicyRequestRequestTypeDef,
-    PutComponentPolicyResponseTypeDef,
     PutContainerRecipePolicyRequestRequestTypeDef,
-    PutContainerRecipePolicyResponseTypeDef,
     PutImagePolicyRequestRequestTypeDef,
-    PutImagePolicyResponseTypeDef,
     PutImageRecipePolicyRequestRequestTypeDef,
-    PutImageRecipePolicyResponseTypeDef,
     RemediationRecommendationTypeDef,
-    ResponseMetadataTypeDef,
     StartImagePipelineExecutionRequestRequestTypeDef,
-    StartImagePipelineExecutionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateDistributionConfigurationResponseTypeDef,
-    UpdateImagePipelineResponseTypeDef,
-    UpdateInfrastructureConfigurationResponseTypeDef,
     AccountAggregationTypeDef,
     ImageAggregationTypeDef,
     ImagePipelineAggregationTypeDef,
     VulnerabilityIdAggregationTypeDef,
-    AdditionalInstanceConfigurationOutputTypeDef,
     AdditionalInstanceConfigurationTypeDef,
     AmiDistributionConfigurationOutputTypeDef,
     AmiDistributionConfigurationTypeDef,
     AmiTypeDef,
+    CancelImageCreationResponseTypeDef,
+    CreateComponentResponseTypeDef,
+    CreateContainerRecipeResponseTypeDef,
+    CreateDistributionConfigurationResponseTypeDef,
+    CreateImagePipelineResponseTypeDef,
+    CreateImageRecipeResponseTypeDef,
+    CreateImageResponseTypeDef,
+    CreateInfrastructureConfigurationResponseTypeDef,
+    DeleteComponentResponseTypeDef,
+    DeleteContainerRecipeResponseTypeDef,
+    DeleteDistributionConfigurationResponseTypeDef,
+    DeleteImagePipelineResponseTypeDef,
+    DeleteImageRecipeResponseTypeDef,
+    DeleteImageResponseTypeDef,
+    DeleteInfrastructureConfigurationResponseTypeDef,
+    GetComponentPolicyResponseTypeDef,
+    GetContainerRecipePolicyResponseTypeDef,
+    GetImagePolicyResponseTypeDef,
+    GetImageRecipePolicyResponseTypeDef,
+    GetWorkflowExecutionResponseTypeDef,
+    GetWorkflowStepExecutionResponseTypeDef,
+    ImportComponentResponseTypeDef,
+    ImportVmImageResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutComponentPolicyResponseTypeDef,
+    PutContainerRecipePolicyResponseTypeDef,
+    PutImagePolicyResponseTypeDef,
+    PutImageRecipePolicyResponseTypeDef,
+    StartImagePipelineExecutionResponseTypeDef,
+    UpdateDistributionConfigurationResponseTypeDef,
+    UpdateImagePipelineResponseTypeDef,
+    UpdateInfrastructureConfigurationResponseTypeDef,
     ComponentConfigurationOutputTypeDef,
     ComponentConfigurationTypeDef,
     ComponentSummaryTypeDef,
     ComponentTypeDef,
     ListComponentsResponseTypeDef,
     ContainerDistributionConfigurationOutputTypeDef,
     ContainerDistributionConfigurationTypeDef,
     ListContainerRecipesResponseTypeDef,
     CvssScoreDetailsTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
-    InstanceBlockDeviceMappingOutputTypeDef,
     InstanceBlockDeviceMappingTypeDef,
     ImageScanningConfigurationOutputTypeDef,
     ImageScanningConfigurationTypeDef,
-    FastLaunchConfigurationOutputTypeDef,
     FastLaunchConfigurationTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListContainerRecipesRequestRequestTypeDef,
     ListDistributionConfigurationsRequestRequestTypeDef,
     ListImageBuildVersionsRequestRequestTypeDef,
     ListImagePipelineImagesRequestRequestTypeDef,
     ListImagePipelinesRequestRequestTypeDef,
@@ -475,35 +429,34 @@
     ListImagePackagesResponseTypeDef,
     ListImageRecipesResponseTypeDef,
     ListImageScanFindingsRequestRequestTypeDef,
     ListImagesResponseTypeDef,
     ListInfrastructureConfigurationsResponseTypeDef,
     ListWorkflowExecutionsResponseTypeDef,
     ListWorkflowStepExecutionsResponseTypeDef,
-    LoggingOutputTypeDef,
     LoggingTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ImageScanFindingAggregationTypeDef,
     OutputResourcesTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     GetComponentResponseTypeDef,
     InspectorScoreDetailsTypeDef,
+    CreateImageRecipeRequestRequestTypeDef,
     ImageRecipeTypeDef,
     InstanceConfigurationOutputTypeDef,
-    CreateImageRecipeRequestRequestTypeDef,
     InstanceConfigurationTypeDef,
     ImagePipelineTypeDef,
     CreateImagePipelineRequestRequestTypeDef,
     CreateImageRequestRequestTypeDef,
     UpdateImagePipelineRequestRequestTypeDef,
     DistributionOutputTypeDef,
     DistributionTypeDef,
-    InfrastructureConfigurationTypeDef,
     CreateInfrastructureConfigurationRequestRequestTypeDef,
+    InfrastructureConfigurationTypeDef,
     UpdateInfrastructureConfigurationRequestRequestTypeDef,
     ListImageScanFindingAggregationsResponseTypeDef,
     ImageSummaryTypeDef,
     ImageScanFindingTypeDef,
     GetImageRecipeResponseTypeDef,
     ContainerRecipeTypeDef,
     CreateContainerRecipeRequestRequestTypeDef,
```

### Comparing `mypy-boto3-imagebuilder-1.28.12/README.md` & `mypy-boto3-imagebuilder-1.28.15/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-imagebuilder
+Version: 1.28.15
+Summary: Type annotations for boto3.imagebuilder 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 imagebuilder type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-imagebuilder"></a>
 
 # mypy-boto3-imagebuilder
 
 [![PyPI - mypy-boto3-imagebuilder](https://img.shields.io/pypi/v/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-imagebuilder)](https://pepy.tech/project/mypy-boto3-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.imagebuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[boto3.imagebuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [mypy-boto3-imagebuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -284,155 +316,141 @@
 
 `mypy_boto3_imagebuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_imagebuilder.type_defs import (
     SeverityCountsTypeDef,
-    SystemsManagerAgentOutputTypeDef,
     SystemsManagerAgentTypeDef,
     LaunchPermissionConfigurationOutputTypeDef,
     LaunchPermissionConfigurationTypeDef,
     ImageStateTypeDef,
     CancelImageCreationRequestRequestTypeDef,
-    CancelImageCreationResponseTypeDef,
+    ResponseMetadataTypeDef,
     ComponentParameterOutputTypeDef,
     ComponentParameterTypeDef,
     ComponentParameterDetailTypeDef,
     ComponentStateTypeDef,
     ComponentVersionTypeDef,
-    TargetContainerRepositoryOutputTypeDef,
     TargetContainerRepositoryTypeDef,
     ContainerRecipeSummaryTypeDef,
     ContainerTypeDef,
     CreateComponentRequestRequestTypeDef,
-    CreateComponentResponseTypeDef,
-    CreateContainerRecipeResponseTypeDef,
-    CreateDistributionConfigurationResponseTypeDef,
     ImageTestsConfigurationTypeDef,
     ScheduleTypeDef,
-    CreateImagePipelineResponseTypeDef,
-    CreateImageRecipeResponseTypeDef,
-    CreateImageResponseTypeDef,
     InstanceMetadataOptionsTypeDef,
-    CreateInfrastructureConfigurationResponseTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteComponentRequestRequestTypeDef,
-    DeleteComponentResponseTypeDef,
     DeleteContainerRecipeRequestRequestTypeDef,
-    DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationRequestRequestTypeDef,
-    DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineRequestRequestTypeDef,
-    DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeRequestRequestTypeDef,
-    DeleteImageRecipeResponseTypeDef,
     DeleteImageRequestRequestTypeDef,
-    DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationRequestRequestTypeDef,
-    DeleteInfrastructureConfigurationResponseTypeDef,
     DistributionConfigurationSummaryTypeDef,
-    LaunchTemplateConfigurationOutputTypeDef,
-    S3ExportConfigurationOutputTypeDef,
     LaunchTemplateConfigurationTypeDef,
     S3ExportConfigurationTypeDef,
-    EbsInstanceBlockDeviceSpecificationOutputTypeDef,
     EbsInstanceBlockDeviceSpecificationTypeDef,
     EcrConfigurationOutputTypeDef,
     EcrConfigurationTypeDef,
-    FastLaunchLaunchTemplateSpecificationOutputTypeDef,
-    FastLaunchSnapshotConfigurationOutputTypeDef,
     FastLaunchLaunchTemplateSpecificationTypeDef,
     FastLaunchSnapshotConfigurationTypeDef,
     FilterTypeDef,
     GetComponentPolicyRequestRequestTypeDef,
-    GetComponentPolicyResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetContainerRecipePolicyRequestRequestTypeDef,
-    GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeRequestRequestTypeDef,
     GetDistributionConfigurationRequestRequestTypeDef,
     GetImagePipelineRequestRequestTypeDef,
     GetImagePolicyRequestRequestTypeDef,
-    GetImagePolicyResponseTypeDef,
     GetImageRecipePolicyRequestRequestTypeDef,
-    GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeRequestRequestTypeDef,
     GetImageRequestRequestTypeDef,
     GetInfrastructureConfigurationRequestRequestTypeDef,
     GetWorkflowExecutionRequestRequestTypeDef,
-    GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionRequestRequestTypeDef,
-    GetWorkflowStepExecutionResponseTypeDef,
     ImagePackageTypeDef,
-    ImageTestsConfigurationOutputTypeDef,
-    ScheduleOutputTypeDef,
     ImageRecipeSummaryTypeDef,
     ImageScanFindingsFilterTypeDef,
     ImageScanStateTypeDef,
     ImageVersionTypeDef,
     ImportComponentRequestRequestTypeDef,
-    ImportComponentResponseTypeDef,
     ImportVmImageRequestRequestTypeDef,
-    ImportVmImageResponseTypeDef,
     InfrastructureConfigurationSummaryTypeDef,
-    InstanceMetadataOptionsOutputTypeDef,
     ListComponentBuildVersionsRequestRequestTypeDef,
     ListImagePackagesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkflowExecutionsRequestRequestTypeDef,
     WorkflowExecutionMetadataTypeDef,
     ListWorkflowStepExecutionsRequestRequestTypeDef,
     WorkflowStepMetadataTypeDef,
-    S3LogsOutputTypeDef,
     S3LogsTypeDef,
     VulnerablePackageTypeDef,
     PutComponentPolicyRequestRequestTypeDef,
-    PutComponentPolicyResponseTypeDef,
     PutContainerRecipePolicyRequestRequestTypeDef,
-    PutContainerRecipePolicyResponseTypeDef,
     PutImagePolicyRequestRequestTypeDef,
-    PutImagePolicyResponseTypeDef,
     PutImageRecipePolicyRequestRequestTypeDef,
-    PutImageRecipePolicyResponseTypeDef,
     RemediationRecommendationTypeDef,
-    ResponseMetadataTypeDef,
     StartImagePipelineExecutionRequestRequestTypeDef,
-    StartImagePipelineExecutionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateDistributionConfigurationResponseTypeDef,
-    UpdateImagePipelineResponseTypeDef,
-    UpdateInfrastructureConfigurationResponseTypeDef,
     AccountAggregationTypeDef,
     ImageAggregationTypeDef,
     ImagePipelineAggregationTypeDef,
     VulnerabilityIdAggregationTypeDef,
-    AdditionalInstanceConfigurationOutputTypeDef,
     AdditionalInstanceConfigurationTypeDef,
     AmiDistributionConfigurationOutputTypeDef,
     AmiDistributionConfigurationTypeDef,
     AmiTypeDef,
+    CancelImageCreationResponseTypeDef,
+    CreateComponentResponseTypeDef,
+    CreateContainerRecipeResponseTypeDef,
+    CreateDistributionConfigurationResponseTypeDef,
+    CreateImagePipelineResponseTypeDef,
+    CreateImageRecipeResponseTypeDef,
+    CreateImageResponseTypeDef,
+    CreateInfrastructureConfigurationResponseTypeDef,
+    DeleteComponentResponseTypeDef,
+    DeleteContainerRecipeResponseTypeDef,
+    DeleteDistributionConfigurationResponseTypeDef,
+    DeleteImagePipelineResponseTypeDef,
+    DeleteImageRecipeResponseTypeDef,
+    DeleteImageResponseTypeDef,
+    DeleteInfrastructureConfigurationResponseTypeDef,
+    GetComponentPolicyResponseTypeDef,
+    GetContainerRecipePolicyResponseTypeDef,
+    GetImagePolicyResponseTypeDef,
+    GetImageRecipePolicyResponseTypeDef,
+    GetWorkflowExecutionResponseTypeDef,
+    GetWorkflowStepExecutionResponseTypeDef,
+    ImportComponentResponseTypeDef,
+    ImportVmImageResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutComponentPolicyResponseTypeDef,
+    PutContainerRecipePolicyResponseTypeDef,
+    PutImagePolicyResponseTypeDef,
+    PutImageRecipePolicyResponseTypeDef,
+    StartImagePipelineExecutionResponseTypeDef,
+    UpdateDistributionConfigurationResponseTypeDef,
+    UpdateImagePipelineResponseTypeDef,
+    UpdateInfrastructureConfigurationResponseTypeDef,
     ComponentConfigurationOutputTypeDef,
     ComponentConfigurationTypeDef,
     ComponentSummaryTypeDef,
     ComponentTypeDef,
     ListComponentsResponseTypeDef,
     ContainerDistributionConfigurationOutputTypeDef,
     ContainerDistributionConfigurationTypeDef,
     ListContainerRecipesResponseTypeDef,
     CvssScoreDetailsTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
-    InstanceBlockDeviceMappingOutputTypeDef,
     InstanceBlockDeviceMappingTypeDef,
     ImageScanningConfigurationOutputTypeDef,
     ImageScanningConfigurationTypeDef,
-    FastLaunchConfigurationOutputTypeDef,
     FastLaunchConfigurationTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListContainerRecipesRequestRequestTypeDef,
     ListDistributionConfigurationsRequestRequestTypeDef,
     ListImageBuildVersionsRequestRequestTypeDef,
     ListImagePipelineImagesRequestRequestTypeDef,
     ListImagePipelinesRequestRequestTypeDef,
@@ -443,35 +461,34 @@
     ListImagePackagesResponseTypeDef,
     ListImageRecipesResponseTypeDef,
     ListImageScanFindingsRequestRequestTypeDef,
     ListImagesResponseTypeDef,
     ListInfrastructureConfigurationsResponseTypeDef,
     ListWorkflowExecutionsResponseTypeDef,
     ListWorkflowStepExecutionsResponseTypeDef,
-    LoggingOutputTypeDef,
     LoggingTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ImageScanFindingAggregationTypeDef,
     OutputResourcesTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     GetComponentResponseTypeDef,
     InspectorScoreDetailsTypeDef,
+    CreateImageRecipeRequestRequestTypeDef,
     ImageRecipeTypeDef,
     InstanceConfigurationOutputTypeDef,
-    CreateImageRecipeRequestRequestTypeDef,
     InstanceConfigurationTypeDef,
     ImagePipelineTypeDef,
     CreateImagePipelineRequestRequestTypeDef,
     CreateImageRequestRequestTypeDef,
     UpdateImagePipelineRequestRequestTypeDef,
     DistributionOutputTypeDef,
     DistributionTypeDef,
-    InfrastructureConfigurationTypeDef,
     CreateInfrastructureConfigurationRequestRequestTypeDef,
+    InfrastructureConfigurationTypeDef,
     UpdateInfrastructureConfigurationRequestRequestTypeDef,
     ListImageScanFindingAggregationsResponseTypeDef,
     ImageSummaryTypeDef,
     ImageScanFindingTypeDef,
     GetImageRecipeResponseTypeDef,
     ContainerRecipeTypeDef,
     CreateContainerRecipeRequestRequestTypeDef,
```

### Comparing `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/__main__.py` & `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.imagebuilder 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.imagebuilder 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder\nOther"
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

### Comparing `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/client.py` & `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/client.pyi` & `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/literals.py` & `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/literals.pyi` & `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/type_defs.py` & `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,155 +42,141 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "SeverityCountsTypeDef",
-    "SystemsManagerAgentOutputTypeDef",
     "SystemsManagerAgentTypeDef",
     "LaunchPermissionConfigurationOutputTypeDef",
     "LaunchPermissionConfigurationTypeDef",
     "ImageStateTypeDef",
     "CancelImageCreationRequestRequestTypeDef",
-    "CancelImageCreationResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ComponentParameterOutputTypeDef",
     "ComponentParameterTypeDef",
     "ComponentParameterDetailTypeDef",
     "ComponentStateTypeDef",
     "ComponentVersionTypeDef",
-    "TargetContainerRepositoryOutputTypeDef",
     "TargetContainerRepositoryTypeDef",
     "ContainerRecipeSummaryTypeDef",
     "ContainerTypeDef",
     "CreateComponentRequestRequestTypeDef",
-    "CreateComponentResponseTypeDef",
-    "CreateContainerRecipeResponseTypeDef",
-    "CreateDistributionConfigurationResponseTypeDef",
     "ImageTestsConfigurationTypeDef",
     "ScheduleTypeDef",
-    "CreateImagePipelineResponseTypeDef",
-    "CreateImageRecipeResponseTypeDef",
-    "CreateImageResponseTypeDef",
     "InstanceMetadataOptionsTypeDef",
-    "CreateInfrastructureConfigurationResponseTypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DeleteComponentRequestRequestTypeDef",
-    "DeleteComponentResponseTypeDef",
     "DeleteContainerRecipeRequestRequestTypeDef",
-    "DeleteContainerRecipeResponseTypeDef",
     "DeleteDistributionConfigurationRequestRequestTypeDef",
-    "DeleteDistributionConfigurationResponseTypeDef",
     "DeleteImagePipelineRequestRequestTypeDef",
-    "DeleteImagePipelineResponseTypeDef",
     "DeleteImageRecipeRequestRequestTypeDef",
-    "DeleteImageRecipeResponseTypeDef",
     "DeleteImageRequestRequestTypeDef",
-    "DeleteImageResponseTypeDef",
     "DeleteInfrastructureConfigurationRequestRequestTypeDef",
-    "DeleteInfrastructureConfigurationResponseTypeDef",
     "DistributionConfigurationSummaryTypeDef",
-    "LaunchTemplateConfigurationOutputTypeDef",
-    "S3ExportConfigurationOutputTypeDef",
     "LaunchTemplateConfigurationTypeDef",
     "S3ExportConfigurationTypeDef",
-    "EbsInstanceBlockDeviceSpecificationOutputTypeDef",
     "EbsInstanceBlockDeviceSpecificationTypeDef",
     "EcrConfigurationOutputTypeDef",
     "EcrConfigurationTypeDef",
-    "FastLaunchLaunchTemplateSpecificationOutputTypeDef",
-    "FastLaunchSnapshotConfigurationOutputTypeDef",
     "FastLaunchLaunchTemplateSpecificationTypeDef",
     "FastLaunchSnapshotConfigurationTypeDef",
     "FilterTypeDef",
     "GetComponentPolicyRequestRequestTypeDef",
-    "GetComponentPolicyResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetContainerRecipePolicyRequestRequestTypeDef",
-    "GetContainerRecipePolicyResponseTypeDef",
     "GetContainerRecipeRequestRequestTypeDef",
     "GetDistributionConfigurationRequestRequestTypeDef",
     "GetImagePipelineRequestRequestTypeDef",
     "GetImagePolicyRequestRequestTypeDef",
-    "GetImagePolicyResponseTypeDef",
     "GetImageRecipePolicyRequestRequestTypeDef",
-    "GetImageRecipePolicyResponseTypeDef",
     "GetImageRecipeRequestRequestTypeDef",
     "GetImageRequestRequestTypeDef",
     "GetInfrastructureConfigurationRequestRequestTypeDef",
     "GetWorkflowExecutionRequestRequestTypeDef",
-    "GetWorkflowExecutionResponseTypeDef",
     "GetWorkflowStepExecutionRequestRequestTypeDef",
-    "GetWorkflowStepExecutionResponseTypeDef",
     "ImagePackageTypeDef",
-    "ImageTestsConfigurationOutputTypeDef",
-    "ScheduleOutputTypeDef",
     "ImageRecipeSummaryTypeDef",
     "ImageScanFindingsFilterTypeDef",
     "ImageScanStateTypeDef",
     "ImageVersionTypeDef",
     "ImportComponentRequestRequestTypeDef",
-    "ImportComponentResponseTypeDef",
     "ImportVmImageRequestRequestTypeDef",
-    "ImportVmImageResponseTypeDef",
     "InfrastructureConfigurationSummaryTypeDef",
-    "InstanceMetadataOptionsOutputTypeDef",
     "ListComponentBuildVersionsRequestRequestTypeDef",
     "ListImagePackagesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWorkflowExecutionsRequestRequestTypeDef",
     "WorkflowExecutionMetadataTypeDef",
     "ListWorkflowStepExecutionsRequestRequestTypeDef",
     "WorkflowStepMetadataTypeDef",
-    "S3LogsOutputTypeDef",
     "S3LogsTypeDef",
     "VulnerablePackageTypeDef",
     "PutComponentPolicyRequestRequestTypeDef",
-    "PutComponentPolicyResponseTypeDef",
     "PutContainerRecipePolicyRequestRequestTypeDef",
-    "PutContainerRecipePolicyResponseTypeDef",
     "PutImagePolicyRequestRequestTypeDef",
-    "PutImagePolicyResponseTypeDef",
     "PutImageRecipePolicyRequestRequestTypeDef",
-    "PutImageRecipePolicyResponseTypeDef",
     "RemediationRecommendationTypeDef",
-    "ResponseMetadataTypeDef",
     "StartImagePipelineExecutionRequestRequestTypeDef",
-    "StartImagePipelineExecutionResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateDistributionConfigurationResponseTypeDef",
-    "UpdateImagePipelineResponseTypeDef",
-    "UpdateInfrastructureConfigurationResponseTypeDef",
     "AccountAggregationTypeDef",
     "ImageAggregationTypeDef",
     "ImagePipelineAggregationTypeDef",
     "VulnerabilityIdAggregationTypeDef",
-    "AdditionalInstanceConfigurationOutputTypeDef",
     "AdditionalInstanceConfigurationTypeDef",
     "AmiDistributionConfigurationOutputTypeDef",
     "AmiDistributionConfigurationTypeDef",
     "AmiTypeDef",
+    "CancelImageCreationResponseTypeDef",
+    "CreateComponentResponseTypeDef",
+    "CreateContainerRecipeResponseTypeDef",
+    "CreateDistributionConfigurationResponseTypeDef",
+    "CreateImagePipelineResponseTypeDef",
+    "CreateImageRecipeResponseTypeDef",
+    "CreateImageResponseTypeDef",
+    "CreateInfrastructureConfigurationResponseTypeDef",
+    "DeleteComponentResponseTypeDef",
+    "DeleteContainerRecipeResponseTypeDef",
+    "DeleteDistributionConfigurationResponseTypeDef",
+    "DeleteImagePipelineResponseTypeDef",
+    "DeleteImageRecipeResponseTypeDef",
+    "DeleteImageResponseTypeDef",
+    "DeleteInfrastructureConfigurationResponseTypeDef",
+    "GetComponentPolicyResponseTypeDef",
+    "GetContainerRecipePolicyResponseTypeDef",
+    "GetImagePolicyResponseTypeDef",
+    "GetImageRecipePolicyResponseTypeDef",
+    "GetWorkflowExecutionResponseTypeDef",
+    "GetWorkflowStepExecutionResponseTypeDef",
+    "ImportComponentResponseTypeDef",
+    "ImportVmImageResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutComponentPolicyResponseTypeDef",
+    "PutContainerRecipePolicyResponseTypeDef",
+    "PutImagePolicyResponseTypeDef",
+    "PutImageRecipePolicyResponseTypeDef",
+    "StartImagePipelineExecutionResponseTypeDef",
+    "UpdateDistributionConfigurationResponseTypeDef",
+    "UpdateImagePipelineResponseTypeDef",
+    "UpdateInfrastructureConfigurationResponseTypeDef",
     "ComponentConfigurationOutputTypeDef",
     "ComponentConfigurationTypeDef",
     "ComponentSummaryTypeDef",
     "ComponentTypeDef",
     "ListComponentsResponseTypeDef",
     "ContainerDistributionConfigurationOutputTypeDef",
     "ContainerDistributionConfigurationTypeDef",
     "ListContainerRecipesResponseTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDistributionConfigurationsResponseTypeDef",
-    "InstanceBlockDeviceMappingOutputTypeDef",
     "InstanceBlockDeviceMappingTypeDef",
     "ImageScanningConfigurationOutputTypeDef",
     "ImageScanningConfigurationTypeDef",
-    "FastLaunchConfigurationOutputTypeDef",
     "FastLaunchConfigurationTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListContainerRecipesRequestRequestTypeDef",
     "ListDistributionConfigurationsRequestRequestTypeDef",
     "ListImageBuildVersionsRequestRequestTypeDef",
     "ListImagePipelineImagesRequestRequestTypeDef",
     "ListImagePipelinesRequestRequestTypeDef",
@@ -201,35 +187,34 @@
     "ListImagePackagesResponseTypeDef",
     "ListImageRecipesResponseTypeDef",
     "ListImageScanFindingsRequestRequestTypeDef",
     "ListImagesResponseTypeDef",
     "ListInfrastructureConfigurationsResponseTypeDef",
     "ListWorkflowExecutionsResponseTypeDef",
     "ListWorkflowStepExecutionsResponseTypeDef",
-    "LoggingOutputTypeDef",
     "LoggingTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "ImageScanFindingAggregationTypeDef",
     "OutputResourcesTypeDef",
     "ListComponentBuildVersionsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "InspectorScoreDetailsTypeDef",
+    "CreateImageRecipeRequestRequestTypeDef",
     "ImageRecipeTypeDef",
     "InstanceConfigurationOutputTypeDef",
-    "CreateImageRecipeRequestRequestTypeDef",
     "InstanceConfigurationTypeDef",
     "ImagePipelineTypeDef",
     "CreateImagePipelineRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
     "UpdateImagePipelineRequestRequestTypeDef",
     "DistributionOutputTypeDef",
     "DistributionTypeDef",
-    "InfrastructureConfigurationTypeDef",
     "CreateInfrastructureConfigurationRequestRequestTypeDef",
+    "InfrastructureConfigurationTypeDef",
     "UpdateInfrastructureConfigurationRequestRequestTypeDef",
     "ListImageScanFindingAggregationsResponseTypeDef",
     "ImageSummaryTypeDef",
     "ImageScanFindingTypeDef",
     "GetImageRecipeResponseTypeDef",
     "ContainerRecipeTypeDef",
     "CreateContainerRecipeRequestRequestTypeDef",
@@ -255,22 +240,14 @@
         "critical": int,
         "high": int,
         "medium": int,
     },
     total=False,
 )
 
-SystemsManagerAgentOutputTypeDef = TypedDict(
-    "SystemsManagerAgentOutputTypeDef",
-    {
-        "uninstallAfterBuild": bool,
-    },
-    total=False,
-)
-
 SystemsManagerAgentTypeDef = TypedDict(
     "SystemsManagerAgentTypeDef",
     {
         "uninstallAfterBuild": bool,
     },
     total=False,
 )
@@ -310,21 +287,22 @@
     "CancelImageCreationRequestRequestTypeDef",
     {
         "imageBuildVersionArn": str,
         "clientToken": str,
     },
 )
 
-CancelImageCreationResponseTypeDef = TypedDict(
-    "CancelImageCreationResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "requestId": str,
-        "clientToken": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ComponentParameterOutputTypeDef = TypedDict(
     "ComponentParameterOutputTypeDef",
     {
         "name": str,
@@ -384,22 +362,14 @@
         "type": ComponentTypeType,
         "owner": str,
         "dateCreated": str,
     },
     total=False,
 )
 
-TargetContainerRepositoryOutputTypeDef = TypedDict(
-    "TargetContainerRepositoryOutputTypeDef",
-    {
-        "service": Literal["ECR"],
-        "repositoryName": str,
-    },
-)
-
 TargetContainerRepositoryTypeDef = TypedDict(
     "TargetContainerRepositoryTypeDef",
     {
         "service": Literal["ECR"],
         "repositoryName": str,
     },
 )
@@ -454,44 +424,14 @@
 
 class CreateComponentRequestRequestTypeDef(
     _RequiredCreateComponentRequestRequestTypeDef, _OptionalCreateComponentRequestRequestTypeDef
 ):
     pass
 
 
-CreateComponentResponseTypeDef = TypedDict(
-    "CreateComponentResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "componentBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateContainerRecipeResponseTypeDef = TypedDict(
-    "CreateContainerRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "containerRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDistributionConfigurationResponseTypeDef = TypedDict(
-    "CreateDistributionConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "distributionConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImageTestsConfigurationTypeDef = TypedDict(
     "ImageTestsConfigurationTypeDef",
     {
         "imageTestsEnabled": bool,
         "timeoutMinutes": int,
     },
     total=False,
@@ -503,63 +443,23 @@
         "scheduleExpression": str,
         "timezone": str,
         "pipelineExecutionStartCondition": PipelineExecutionStartConditionType,
     },
     total=False,
 )
 
-CreateImagePipelineResponseTypeDef = TypedDict(
-    "CreateImagePipelineResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imagePipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateImageRecipeResponseTypeDef = TypedDict(
-    "CreateImageRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imageRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateImageResponseTypeDef = TypedDict(
-    "CreateImageResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InstanceMetadataOptionsTypeDef = TypedDict(
     "InstanceMetadataOptionsTypeDef",
     {
         "httpTokens": str,
         "httpPutResponseHopLimit": int,
     },
     total=False,
 )
 
-CreateInfrastructureConfigurationResponseTypeDef = TypedDict(
-    "CreateInfrastructureConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "infrastructureConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CvssScoreAdjustmentTypeDef = TypedDict(
     "CvssScoreAdjustmentTypeDef",
     {
         "metric": str,
         "reason": str,
     },
     total=False,
@@ -579,179 +479,70 @@
 DeleteComponentRequestRequestTypeDef = TypedDict(
     "DeleteComponentRequestRequestTypeDef",
     {
         "componentBuildVersionArn": str,
     },
 )
 
-DeleteComponentResponseTypeDef = TypedDict(
-    "DeleteComponentResponseTypeDef",
-    {
-        "requestId": str,
-        "componentBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteContainerRecipeRequestRequestTypeDef = TypedDict(
     "DeleteContainerRecipeRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
     },
 )
 
-DeleteContainerRecipeResponseTypeDef = TypedDict(
-    "DeleteContainerRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "containerRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteDistributionConfigurationRequestRequestTypeDef",
     {
         "distributionConfigurationArn": str,
     },
 )
 
-DeleteDistributionConfigurationResponseTypeDef = TypedDict(
-    "DeleteDistributionConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "distributionConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImagePipelineRequestRequestTypeDef = TypedDict(
     "DeleteImagePipelineRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
     },
 )
 
-DeleteImagePipelineResponseTypeDef = TypedDict(
-    "DeleteImagePipelineResponseTypeDef",
-    {
-        "requestId": str,
-        "imagePipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImageRecipeRequestRequestTypeDef = TypedDict(
     "DeleteImageRecipeRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
     },
 )
 
-DeleteImageRecipeResponseTypeDef = TypedDict(
-    "DeleteImageRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "imageRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImageRequestRequestTypeDef = TypedDict(
     "DeleteImageRequestRequestTypeDef",
     {
         "imageBuildVersionArn": str,
     },
 )
 
-DeleteImageResponseTypeDef = TypedDict(
-    "DeleteImageResponseTypeDef",
-    {
-        "requestId": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteInfrastructureConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteInfrastructureConfigurationRequestRequestTypeDef",
     {
         "infrastructureConfigurationArn": str,
     },
 )
 
-DeleteInfrastructureConfigurationResponseTypeDef = TypedDict(
-    "DeleteInfrastructureConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "infrastructureConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DistributionConfigurationSummaryTypeDef = TypedDict(
     "DistributionConfigurationSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
         "dateCreated": str,
         "dateUpdated": str,
         "tags": Dict[str, str],
         "regions": List[str],
     },
     total=False,
 )
 
-_RequiredLaunchTemplateConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLaunchTemplateConfigurationOutputTypeDef",
-    {
-        "launchTemplateId": str,
-    },
-)
-_OptionalLaunchTemplateConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLaunchTemplateConfigurationOutputTypeDef",
-    {
-        "accountId": str,
-        "setDefaultVersion": bool,
-    },
-    total=False,
-)
-
-
-class LaunchTemplateConfigurationOutputTypeDef(
-    _RequiredLaunchTemplateConfigurationOutputTypeDef,
-    _OptionalLaunchTemplateConfigurationOutputTypeDef,
-):
-    pass
-
-
-_RequiredS3ExportConfigurationOutputTypeDef = TypedDict(
-    "_RequiredS3ExportConfigurationOutputTypeDef",
-    {
-        "roleName": str,
-        "diskImageFormat": DiskImageFormatType,
-        "s3Bucket": str,
-    },
-)
-_OptionalS3ExportConfigurationOutputTypeDef = TypedDict(
-    "_OptionalS3ExportConfigurationOutputTypeDef",
-    {
-        "s3Prefix": str,
-    },
-    total=False,
-)
-
-
-class S3ExportConfigurationOutputTypeDef(
-    _RequiredS3ExportConfigurationOutputTypeDef, _OptionalS3ExportConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredLaunchTemplateConfigurationTypeDef = TypedDict(
     "_RequiredLaunchTemplateConfigurationTypeDef",
     {
         "launchTemplateId": str,
     },
 )
 _OptionalLaunchTemplateConfigurationTypeDef = TypedDict(
@@ -789,29 +580,14 @@
 
 class S3ExportConfigurationTypeDef(
     _RequiredS3ExportConfigurationTypeDef, _OptionalS3ExportConfigurationTypeDef
 ):
     pass
 
 
-EbsInstanceBlockDeviceSpecificationOutputTypeDef = TypedDict(
-    "EbsInstanceBlockDeviceSpecificationOutputTypeDef",
-    {
-        "encrypted": bool,
-        "deleteOnTermination": bool,
-        "iops": int,
-        "kmsKeyId": str,
-        "snapshotId": str,
-        "volumeSize": int,
-        "volumeType": EbsVolumeTypeType,
-        "throughput": int,
-    },
-    total=False,
-)
-
 EbsInstanceBlockDeviceSpecificationTypeDef = TypedDict(
     "EbsInstanceBlockDeviceSpecificationTypeDef",
     {
         "encrypted": bool,
         "deleteOnTermination": bool,
         "iops": int,
         "kmsKeyId": str,
@@ -837,32 +613,14 @@
     {
         "repositoryName": str,
         "containerTags": Sequence[str],
     },
     total=False,
 )
 
-FastLaunchLaunchTemplateSpecificationOutputTypeDef = TypedDict(
-    "FastLaunchLaunchTemplateSpecificationOutputTypeDef",
-    {
-        "launchTemplateId": str,
-        "launchTemplateName": str,
-        "launchTemplateVersion": str,
-    },
-    total=False,
-)
-
-FastLaunchSnapshotConfigurationOutputTypeDef = TypedDict(
-    "FastLaunchSnapshotConfigurationOutputTypeDef",
-    {
-        "targetResourceCount": int,
-    },
-    total=False,
-)
-
 FastLaunchLaunchTemplateSpecificationTypeDef = TypedDict(
     "FastLaunchLaunchTemplateSpecificationTypeDef",
     {
         "launchTemplateId": str,
         "launchTemplateName": str,
         "launchTemplateVersion": str,
     },
@@ -889,46 +647,28 @@
 GetComponentPolicyRequestRequestTypeDef = TypedDict(
     "GetComponentPolicyRequestRequestTypeDef",
     {
         "componentArn": str,
     },
 )
 
-GetComponentPolicyResponseTypeDef = TypedDict(
-    "GetComponentPolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetComponentRequestRequestTypeDef = TypedDict(
     "GetComponentRequestRequestTypeDef",
     {
         "componentBuildVersionArn": str,
     },
 )
 
 GetContainerRecipePolicyRequestRequestTypeDef = TypedDict(
     "GetContainerRecipePolicyRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
     },
 )
 
-GetContainerRecipePolicyResponseTypeDef = TypedDict(
-    "GetContainerRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetContainerRecipeRequestRequestTypeDef = TypedDict(
     "GetContainerRecipeRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
     },
 )
 
@@ -949,39 +689,21 @@
 GetImagePolicyRequestRequestTypeDef = TypedDict(
     "GetImagePolicyRequestRequestTypeDef",
     {
         "imageArn": str,
     },
 )
 
-GetImagePolicyResponseTypeDef = TypedDict(
-    "GetImagePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetImageRecipePolicyRequestRequestTypeDef = TypedDict(
     "GetImageRecipePolicyRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
     },
 )
 
-GetImageRecipePolicyResponseTypeDef = TypedDict(
-    "GetImageRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetImageRecipeRequestRequestTypeDef = TypedDict(
     "GetImageRecipeRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
     },
 )
 
@@ -1002,93 +724,30 @@
 GetWorkflowExecutionRequestRequestTypeDef = TypedDict(
     "GetWorkflowExecutionRequestRequestTypeDef",
     {
         "workflowExecutionId": str,
     },
 )
 
-GetWorkflowExecutionResponseTypeDef = TypedDict(
-    "GetWorkflowExecutionResponseTypeDef",
-    {
-        "requestId": str,
-        "workflowBuildVersionArn": str,
-        "workflowExecutionId": str,
-        "imageBuildVersionArn": str,
-        "type": WorkflowTypeType,
-        "status": WorkflowExecutionStatusType,
-        "message": str,
-        "totalStepCount": int,
-        "totalStepsSucceeded": int,
-        "totalStepsFailed": int,
-        "totalStepsSkipped": int,
-        "startTime": str,
-        "endTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkflowStepExecutionRequestRequestTypeDef = TypedDict(
     "GetWorkflowStepExecutionRequestRequestTypeDef",
     {
         "stepExecutionId": str,
     },
 )
 
-GetWorkflowStepExecutionResponseTypeDef = TypedDict(
-    "GetWorkflowStepExecutionResponseTypeDef",
-    {
-        "requestId": str,
-        "stepExecutionId": str,
-        "workflowBuildVersionArn": str,
-        "workflowExecutionId": str,
-        "imageBuildVersionArn": str,
-        "name": str,
-        "description": str,
-        "action": str,
-        "status": WorkflowStepExecutionStatusType,
-        "rollbackStatus": WorkflowStepExecutionRollbackStatusType,
-        "message": str,
-        "inputs": str,
-        "outputs": str,
-        "startTime": str,
-        "endTime": str,
-        "onFailure": str,
-        "timeoutSeconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImagePackageTypeDef = TypedDict(
     "ImagePackageTypeDef",
     {
         "packageName": str,
         "packageVersion": str,
     },
     total=False,
 )
 
-ImageTestsConfigurationOutputTypeDef = TypedDict(
-    "ImageTestsConfigurationOutputTypeDef",
-    {
-        "imageTestsEnabled": bool,
-        "timeoutMinutes": int,
-    },
-    total=False,
-)
-
-ScheduleOutputTypeDef = TypedDict(
-    "ScheduleOutputTypeDef",
-    {
-        "scheduleExpression": str,
-        "timezone": str,
-        "pipelineExecutionStartCondition": PipelineExecutionStartConditionType,
-    },
-    total=False,
-)
-
 ImageRecipeSummaryTypeDef = TypedDict(
     "ImageRecipeSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "platform": PlatformType,
         "owner": str,
@@ -1161,24 +820,14 @@
 
 class ImportComponentRequestRequestTypeDef(
     _RequiredImportComponentRequestRequestTypeDef, _OptionalImportComponentRequestRequestTypeDef
 ):
     pass
 
 
-ImportComponentResponseTypeDef = TypedDict(
-    "ImportComponentResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "componentBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredImportVmImageRequestRequestTypeDef = TypedDict(
     "_RequiredImportVmImageRequestRequestTypeDef",
     {
         "name": str,
         "semanticVersion": str,
         "platform": PlatformType,
         "vmImportTaskId": str,
@@ -1198,24 +847,14 @@
 
 class ImportVmImageRequestRequestTypeDef(
     _RequiredImportVmImageRequestRequestTypeDef, _OptionalImportVmImageRequestRequestTypeDef
 ):
     pass
 
 
-ImportVmImageResponseTypeDef = TypedDict(
-    "ImportVmImageResponseTypeDef",
-    {
-        "requestId": str,
-        "imageArn": str,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InfrastructureConfigurationSummaryTypeDef = TypedDict(
     "InfrastructureConfigurationSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
         "dateCreated": str,
@@ -1224,23 +863,14 @@
         "tags": Dict[str, str],
         "instanceTypes": List[str],
         "instanceProfileName": str,
     },
     total=False,
 )
 
-InstanceMetadataOptionsOutputTypeDef = TypedDict(
-    "InstanceMetadataOptionsOutputTypeDef",
-    {
-        "httpTokens": str,
-        "httpPutResponseHopLimit": int,
-    },
-    total=False,
-)
-
 _RequiredListComponentBuildVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentBuildVersionsRequestRequestTypeDef",
     {
         "componentVersionArn": str,
     },
 )
 _OptionalListComponentBuildVersionsRequestRequestTypeDef = TypedDict(
@@ -1285,22 +915,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListWorkflowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkflowExecutionsRequestRequestTypeDef",
     {
         "imageBuildVersionArn": str,
     },
 )
 _OptionalListWorkflowExecutionsRequestRequestTypeDef = TypedDict(
@@ -1375,23 +997,14 @@
         "outputs": str,
         "startTime": str,
         "endTime": str,
     },
     total=False,
 )
 
-S3LogsOutputTypeDef = TypedDict(
-    "S3LogsOutputTypeDef",
-    {
-        "s3BucketName": str,
-        "s3KeyPrefix": str,
-    },
-    total=False,
-)
-
 S3LogsTypeDef = TypedDict(
     "S3LogsTypeDef",
     {
         "s3BucketName": str,
         "s3KeyPrefix": str,
     },
     total=False,
@@ -1418,112 +1031,55 @@
     "PutComponentPolicyRequestRequestTypeDef",
     {
         "componentArn": str,
         "policy": str,
     },
 )
 
-PutComponentPolicyResponseTypeDef = TypedDict(
-    "PutComponentPolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "componentArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutContainerRecipePolicyRequestRequestTypeDef = TypedDict(
     "PutContainerRecipePolicyRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
         "policy": str,
     },
 )
 
-PutContainerRecipePolicyResponseTypeDef = TypedDict(
-    "PutContainerRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "containerRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutImagePolicyRequestRequestTypeDef = TypedDict(
     "PutImagePolicyRequestRequestTypeDef",
     {
         "imageArn": str,
         "policy": str,
     },
 )
 
-PutImagePolicyResponseTypeDef = TypedDict(
-    "PutImagePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "imageArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutImageRecipePolicyRequestRequestTypeDef = TypedDict(
     "PutImageRecipePolicyRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
         "policy": str,
     },
 )
 
-PutImageRecipePolicyResponseTypeDef = TypedDict(
-    "PutImageRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "imageRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemediationRecommendationTypeDef = TypedDict(
     "RemediationRecommendationTypeDef",
     {
         "text": str,
         "url": str,
     },
     total=False,
 )
 
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
 StartImagePipelineExecutionRequestRequestTypeDef = TypedDict(
     "StartImagePipelineExecutionRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
         "clientToken": str,
     },
 )
 
-StartImagePipelineExecutionResponseTypeDef = TypedDict(
-    "StartImagePipelineExecutionResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1532,44 +1088,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateDistributionConfigurationResponseTypeDef = TypedDict(
-    "UpdateDistributionConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "distributionConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateImagePipelineResponseTypeDef = TypedDict(
-    "UpdateImagePipelineResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imagePipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateInfrastructureConfigurationResponseTypeDef = TypedDict(
-    "UpdateInfrastructureConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "infrastructureConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AccountAggregationTypeDef = TypedDict(
     "AccountAggregationTypeDef",
     {
         "accountId": str,
         "severityCounts": SeverityCountsTypeDef,
     },
     total=False,
@@ -1598,23 +1124,14 @@
     {
         "vulnerabilityId": str,
         "severityCounts": SeverityCountsTypeDef,
     },
     total=False,
 )
 
-AdditionalInstanceConfigurationOutputTypeDef = TypedDict(
-    "AdditionalInstanceConfigurationOutputTypeDef",
-    {
-        "systemsManagerAgent": SystemsManagerAgentOutputTypeDef,
-        "userDataOverride": str,
-    },
-    total=False,
-)
-
 AdditionalInstanceConfigurationTypeDef = TypedDict(
     "AdditionalInstanceConfigurationTypeDef",
     {
         "systemsManagerAgent": SystemsManagerAgentTypeDef,
         "userDataOverride": str,
     },
     total=False,
@@ -1655,14 +1172,341 @@
         "description": str,
         "state": ImageStateTypeDef,
         "accountId": str,
     },
     total=False,
 )
 
+CancelImageCreationResponseTypeDef = TypedDict(
+    "CancelImageCreationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateComponentResponseTypeDef = TypedDict(
+    "CreateComponentResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "componentBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateContainerRecipeResponseTypeDef = TypedDict(
+    "CreateContainerRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "containerRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDistributionConfigurationResponseTypeDef = TypedDict(
+    "CreateDistributionConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "distributionConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImagePipelineResponseTypeDef = TypedDict(
+    "CreateImagePipelineResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imagePipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImageRecipeResponseTypeDef = TypedDict(
+    "CreateImageRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImageResponseTypeDef = TypedDict(
+    "CreateImageResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateInfrastructureConfigurationResponseTypeDef = TypedDict(
+    "CreateInfrastructureConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "infrastructureConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteComponentResponseTypeDef = TypedDict(
+    "DeleteComponentResponseTypeDef",
+    {
+        "requestId": str,
+        "componentBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteContainerRecipeResponseTypeDef = TypedDict(
+    "DeleteContainerRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "containerRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDistributionConfigurationResponseTypeDef = TypedDict(
+    "DeleteDistributionConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "distributionConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImagePipelineResponseTypeDef = TypedDict(
+    "DeleteImagePipelineResponseTypeDef",
+    {
+        "requestId": str,
+        "imagePipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImageRecipeResponseTypeDef = TypedDict(
+    "DeleteImageRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "imageRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImageResponseTypeDef = TypedDict(
+    "DeleteImageResponseTypeDef",
+    {
+        "requestId": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteInfrastructureConfigurationResponseTypeDef = TypedDict(
+    "DeleteInfrastructureConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "infrastructureConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetComponentPolicyResponseTypeDef = TypedDict(
+    "GetComponentPolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContainerRecipePolicyResponseTypeDef = TypedDict(
+    "GetContainerRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImagePolicyResponseTypeDef = TypedDict(
+    "GetImagePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImageRecipePolicyResponseTypeDef = TypedDict(
+    "GetImageRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkflowExecutionResponseTypeDef = TypedDict(
+    "GetWorkflowExecutionResponseTypeDef",
+    {
+        "requestId": str,
+        "workflowBuildVersionArn": str,
+        "workflowExecutionId": str,
+        "imageBuildVersionArn": str,
+        "type": WorkflowTypeType,
+        "status": WorkflowExecutionStatusType,
+        "message": str,
+        "totalStepCount": int,
+        "totalStepsSucceeded": int,
+        "totalStepsFailed": int,
+        "totalStepsSkipped": int,
+        "startTime": str,
+        "endTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkflowStepExecutionResponseTypeDef = TypedDict(
+    "GetWorkflowStepExecutionResponseTypeDef",
+    {
+        "requestId": str,
+        "stepExecutionId": str,
+        "workflowBuildVersionArn": str,
+        "workflowExecutionId": str,
+        "imageBuildVersionArn": str,
+        "name": str,
+        "description": str,
+        "action": str,
+        "status": WorkflowStepExecutionStatusType,
+        "rollbackStatus": WorkflowStepExecutionRollbackStatusType,
+        "message": str,
+        "inputs": str,
+        "outputs": str,
+        "startTime": str,
+        "endTime": str,
+        "onFailure": str,
+        "timeoutSeconds": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportComponentResponseTypeDef = TypedDict(
+    "ImportComponentResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "componentBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportVmImageResponseTypeDef = TypedDict(
+    "ImportVmImageResponseTypeDef",
+    {
+        "requestId": str,
+        "imageArn": str,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutComponentPolicyResponseTypeDef = TypedDict(
+    "PutComponentPolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "componentArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutContainerRecipePolicyResponseTypeDef = TypedDict(
+    "PutContainerRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "containerRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutImagePolicyResponseTypeDef = TypedDict(
+    "PutImagePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "imageArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutImageRecipePolicyResponseTypeDef = TypedDict(
+    "PutImageRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "imageRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartImagePipelineExecutionResponseTypeDef = TypedDict(
+    "StartImagePipelineExecutionResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDistributionConfigurationResponseTypeDef = TypedDict(
+    "UpdateDistributionConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "distributionConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateImagePipelineResponseTypeDef = TypedDict(
+    "UpdateImagePipelineResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imagePipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateInfrastructureConfigurationResponseTypeDef = TypedDict(
+    "UpdateInfrastructureConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "infrastructureConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredComponentConfigurationOutputTypeDef = TypedDict(
     "_RequiredComponentConfigurationOutputTypeDef",
     {
         "componentArn": str,
     },
 )
 _OptionalComponentConfigurationOutputTypeDef = TypedDict(
@@ -1749,22 +1593,22 @@
 
 ListComponentsResponseTypeDef = TypedDict(
     "ListComponentsResponseTypeDef",
     {
         "requestId": str,
         "componentVersionList": List[ComponentVersionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredContainerDistributionConfigurationOutputTypeDef = TypedDict(
     "_RequiredContainerDistributionConfigurationOutputTypeDef",
     {
-        "targetRepository": TargetContainerRepositoryOutputTypeDef,
+        "targetRepository": TargetContainerRepositoryTypeDef,
     },
 )
 _OptionalContainerDistributionConfigurationOutputTypeDef = TypedDict(
     "_OptionalContainerDistributionConfigurationOutputTypeDef",
     {
         "description": str,
         "containerTags": List[str],
@@ -1805,15 +1649,15 @@
 
 ListContainerRecipesResponseTypeDef = TypedDict(
     "ListContainerRecipesResponseTypeDef",
     {
         "requestId": str,
         "containerRecipeSummaryList": List[ContainerRecipeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CvssScoreDetailsTypeDef = TypedDict(
     "CvssScoreDetailsTypeDef",
     {
         "scoreSource": str,
@@ -1828,27 +1672,16 @@
 
 ListDistributionConfigurationsResponseTypeDef = TypedDict(
     "ListDistributionConfigurationsResponseTypeDef",
     {
         "requestId": str,
         "distributionConfigurationSummaryList": List[DistributionConfigurationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-InstanceBlockDeviceMappingOutputTypeDef = TypedDict(
-    "InstanceBlockDeviceMappingOutputTypeDef",
-    {
-        "deviceName": str,
-        "ebs": EbsInstanceBlockDeviceSpecificationOutputTypeDef,
-        "virtualName": str,
-        "noDevice": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 InstanceBlockDeviceMappingTypeDef = TypedDict(
     "InstanceBlockDeviceMappingTypeDef",
     {
         "deviceName": str,
         "ebs": EbsInstanceBlockDeviceSpecificationTypeDef,
@@ -1872,38 +1705,14 @@
     {
         "imageScanningEnabled": bool,
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredFastLaunchConfigurationOutputTypeDef = TypedDict(
-    "_RequiredFastLaunchConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-_OptionalFastLaunchConfigurationOutputTypeDef = TypedDict(
-    "_OptionalFastLaunchConfigurationOutputTypeDef",
-    {
-        "snapshotConfiguration": FastLaunchSnapshotConfigurationOutputTypeDef,
-        "maxParallelLaunches": int,
-        "launchTemplate": FastLaunchLaunchTemplateSpecificationOutputTypeDef,
-        "accountId": str,
-    },
-    total=False,
-)
-
-
-class FastLaunchConfigurationOutputTypeDef(
-    _RequiredFastLaunchConfigurationOutputTypeDef, _OptionalFastLaunchConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredFastLaunchConfigurationTypeDef = TypedDict(
     "_RequiredFastLaunchConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalFastLaunchConfigurationTypeDef = TypedDict(
@@ -2060,25 +1869,25 @@
 
 ListImagePackagesResponseTypeDef = TypedDict(
     "ListImagePackagesResponseTypeDef",
     {
         "requestId": str,
         "imagePackageList": List[ImagePackageTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageRecipesResponseTypeDef = TypedDict(
     "ListImageRecipesResponseTypeDef",
     {
         "requestId": str,
         "imageRecipeSummaryList": List[ImageRecipeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageScanFindingsRequestRequestTypeDef = TypedDict(
     "ListImageScanFindingsRequestRequestTypeDef",
     {
         "filters": Sequence[ImageScanFindingsFilterTypeDef],
@@ -2090,62 +1899,54 @@
 
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
         "requestId": str,
         "imageVersionList": List[ImageVersionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInfrastructureConfigurationsResponseTypeDef = TypedDict(
     "ListInfrastructureConfigurationsResponseTypeDef",
     {
         "requestId": str,
         "infrastructureConfigurationSummaryList": List[InfrastructureConfigurationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowExecutionsResponseTypeDef = TypedDict(
     "ListWorkflowExecutionsResponseTypeDef",
     {
         "requestId": str,
         "workflowExecutions": List[WorkflowExecutionMetadataTypeDef],
         "imageBuildVersionArn": str,
         "message": str,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowStepExecutionsResponseTypeDef = TypedDict(
     "ListWorkflowStepExecutionsResponseTypeDef",
     {
         "requestId": str,
         "steps": List[WorkflowStepMetadataTypeDef],
         "workflowBuildVersionArn": str,
         "workflowExecutionId": str,
         "imageBuildVersionArn": str,
         "message": str,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoggingOutputTypeDef = TypedDict(
-    "LoggingOutputTypeDef",
-    {
-        "s3Logs": S3LogsOutputTypeDef,
-    },
-    total=False,
-)
-
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "s3Logs": S3LogsTypeDef,
     },
     total=False,
 )
@@ -2209,65 +2010,35 @@
 
 ListComponentBuildVersionsResponseTypeDef = TypedDict(
     "ListComponentBuildVersionsResponseTypeDef",
     {
         "requestId": str,
         "componentSummaryList": List[ComponentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComponentResponseTypeDef = TypedDict(
     "GetComponentResponseTypeDef",
     {
         "requestId": str,
         "component": ComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InspectorScoreDetailsTypeDef = TypedDict(
     "InspectorScoreDetailsTypeDef",
     {
         "adjustedCvss": CvssScoreDetailsTypeDef,
     },
     total=False,
 )
 
-ImageRecipeTypeDef = TypedDict(
-    "ImageRecipeTypeDef",
-    {
-        "arn": str,
-        "type": ImageTypeType,
-        "name": str,
-        "description": str,
-        "platform": PlatformType,
-        "owner": str,
-        "version": str,
-        "components": List[ComponentConfigurationOutputTypeDef],
-        "parentImage": str,
-        "blockDeviceMappings": List[InstanceBlockDeviceMappingOutputTypeDef],
-        "dateCreated": str,
-        "tags": Dict[str, str],
-        "workingDirectory": str,
-        "additionalInstanceConfiguration": AdditionalInstanceConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-InstanceConfigurationOutputTypeDef = TypedDict(
-    "InstanceConfigurationOutputTypeDef",
-    {
-        "image": str,
-        "blockDeviceMappings": List[InstanceBlockDeviceMappingOutputTypeDef],
-    },
-    total=False,
-)
-
 _RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageRecipeRequestRequestTypeDef",
     {
         "name": str,
         "semanticVersion": str,
         "components": Sequence[ComponentConfigurationTypeDef],
         "parentImage": str,
@@ -2289,14 +2060,44 @@
 
 class CreateImageRecipeRequestRequestTypeDef(
     _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
 ):
     pass
 
 
+ImageRecipeTypeDef = TypedDict(
+    "ImageRecipeTypeDef",
+    {
+        "arn": str,
+        "type": ImageTypeType,
+        "name": str,
+        "description": str,
+        "platform": PlatformType,
+        "owner": str,
+        "version": str,
+        "components": List[ComponentConfigurationOutputTypeDef],
+        "parentImage": str,
+        "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
+        "dateCreated": str,
+        "tags": Dict[str, str],
+        "workingDirectory": str,
+        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
+    },
+    total=False,
+)
+
+InstanceConfigurationOutputTypeDef = TypedDict(
+    "InstanceConfigurationOutputTypeDef",
+    {
+        "image": str,
+        "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
+    },
+    total=False,
+)
+
 InstanceConfigurationTypeDef = TypedDict(
     "InstanceConfigurationTypeDef",
     {
         "image": str,
         "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
     },
     total=False,
@@ -2310,16 +2111,16 @@
         "description": str,
         "platform": PlatformType,
         "enhancedImageMetadataEnabled": bool,
         "imageRecipeArn": str,
         "containerRecipeArn": str,
         "infrastructureConfigurationArn": str,
         "distributionConfigurationArn": str,
-        "imageTestsConfiguration": ImageTestsConfigurationOutputTypeDef,
-        "schedule": ScheduleOutputTypeDef,
+        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
+        "schedule": ScheduleTypeDef,
         "status": PipelineStatusType,
         "dateCreated": str,
         "dateUpdated": str,
         "dateLastRun": str,
         "dateNextRun": str,
         "tags": Dict[str, str],
         "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
@@ -2428,17 +2229,17 @@
 )
 _OptionalDistributionOutputTypeDef = TypedDict(
     "_OptionalDistributionOutputTypeDef",
     {
         "amiDistributionConfiguration": AmiDistributionConfigurationOutputTypeDef,
         "containerDistributionConfiguration": ContainerDistributionConfigurationOutputTypeDef,
         "licenseConfigurationArns": List[str],
-        "launchTemplateConfigurations": List[LaunchTemplateConfigurationOutputTypeDef],
-        "s3ExportConfiguration": S3ExportConfigurationOutputTypeDef,
-        "fastLaunchConfigurations": List[FastLaunchConfigurationOutputTypeDef],
+        "launchTemplateConfigurations": List[LaunchTemplateConfigurationTypeDef],
+        "s3ExportConfiguration": S3ExportConfigurationTypeDef,
+        "fastLaunchConfigurations": List[FastLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
 
 class DistributionOutputTypeDef(
     _RequiredDistributionOutputTypeDef, _OptionalDistributionOutputTypeDef
@@ -2466,37 +2267,14 @@
 )
 
 
 class DistributionTypeDef(_RequiredDistributionTypeDef, _OptionalDistributionTypeDef):
     pass
 
 
-InfrastructureConfigurationTypeDef = TypedDict(
-    "InfrastructureConfigurationTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "instanceTypes": List[str],
-        "instanceProfileName": str,
-        "securityGroupIds": List[str],
-        "subnetId": str,
-        "logging": LoggingOutputTypeDef,
-        "keyPair": str,
-        "terminateInstanceOnFailure": bool,
-        "snsTopicArn": str,
-        "dateCreated": str,
-        "dateUpdated": str,
-        "resourceTags": Dict[str, str],
-        "instanceMetadataOptions": InstanceMetadataOptionsOutputTypeDef,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredCreateInfrastructureConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInfrastructureConfigurationRequestRequestTypeDef",
     {
         "name": str,
         "instanceProfileName": str,
         "clientToken": str,
     },
@@ -2523,14 +2301,37 @@
 class CreateInfrastructureConfigurationRequestRequestTypeDef(
     _RequiredCreateInfrastructureConfigurationRequestRequestTypeDef,
     _OptionalCreateInfrastructureConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+InfrastructureConfigurationTypeDef = TypedDict(
+    "InfrastructureConfigurationTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "instanceTypes": List[str],
+        "instanceProfileName": str,
+        "securityGroupIds": List[str],
+        "subnetId": str,
+        "logging": LoggingTypeDef,
+        "keyPair": str,
+        "terminateInstanceOnFailure": bool,
+        "snsTopicArn": str,
+        "dateCreated": str,
+        "dateUpdated": str,
+        "resourceTags": Dict[str, str],
+        "instanceMetadataOptions": InstanceMetadataOptionsTypeDef,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredUpdateInfrastructureConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInfrastructureConfigurationRequestRequestTypeDef",
     {
         "infrastructureConfigurationArn": str,
         "instanceProfileName": str,
         "clientToken": str,
     },
@@ -2563,15 +2364,15 @@
 ListImageScanFindingAggregationsResponseTypeDef = TypedDict(
     "ListImageScanFindingAggregationsResponseTypeDef",
     {
         "requestId": str,
         "aggregationType": str,
         "responses": List[ImageScanFindingAggregationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageSummaryTypeDef = TypedDict(
     "ImageSummaryTypeDef",
     {
         "arn": str,
@@ -2613,15 +2414,15 @@
 )
 
 GetImageRecipeResponseTypeDef = TypedDict(
     "GetImageRecipeResponseTypeDef",
     {
         "requestId": str,
         "imageRecipe": ImageRecipeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ContainerRecipeTypeDef = TypedDict(
     "ContainerRecipeTypeDef",
     {
         "arn": str,
@@ -2636,15 +2437,15 @@
         "dockerfileTemplateData": str,
         "kmsKeyId": str,
         "encrypted": bool,
         "parentImage": str,
         "dateCreated": str,
         "tags": Dict[str, str],
         "workingDirectory": str,
-        "targetRepository": TargetContainerRepositoryOutputTypeDef,
+        "targetRepository": TargetContainerRepositoryTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerRecipeRequestRequestTypeDef",
     {
@@ -2682,25 +2483,25 @@
 
 
 GetImagePipelineResponseTypeDef = TypedDict(
     "GetImagePipelineResponseTypeDef",
     {
         "requestId": str,
         "imagePipeline": ImagePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImagePipelinesResponseTypeDef = TypedDict(
     "ListImagePipelinesResponseTypeDef",
     {
         "requestId": str,
         "imagePipelineList": List[ImagePipelineTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDistributionConfigurationTypeDef = TypedDict(
     "_RequiredDistributionConfigurationTypeDef",
     {
         "timeoutMinutes": int,
@@ -2777,63 +2578,63 @@
 
 
 GetInfrastructureConfigurationResponseTypeDef = TypedDict(
     "GetInfrastructureConfigurationResponseTypeDef",
     {
         "requestId": str,
         "infrastructureConfiguration": InfrastructureConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageBuildVersionsResponseTypeDef = TypedDict(
     "ListImageBuildVersionsResponseTypeDef",
     {
         "requestId": str,
         "imageSummaryList": List[ImageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImagePipelineImagesResponseTypeDef = TypedDict(
     "ListImagePipelineImagesResponseTypeDef",
     {
         "requestId": str,
         "imageSummaryList": List[ImageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageScanFindingsResponseTypeDef = TypedDict(
     "ListImageScanFindingsResponseTypeDef",
     {
         "requestId": str,
         "findings": List[ImageScanFindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContainerRecipeResponseTypeDef = TypedDict(
     "GetContainerRecipeResponseTypeDef",
     {
         "requestId": str,
         "containerRecipe": ContainerRecipeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDistributionConfigurationResponseTypeDef = TypedDict(
     "GetDistributionConfigurationResponseTypeDef",
     {
         "requestId": str,
         "distributionConfiguration": DistributionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "arn": str,
@@ -2846,15 +2647,15 @@
         "state": ImageStateTypeDef,
         "imageRecipe": ImageRecipeTypeDef,
         "containerRecipe": ContainerRecipeTypeDef,
         "sourcePipelineName": str,
         "sourcePipelineArn": str,
         "infrastructureConfiguration": InfrastructureConfigurationTypeDef,
         "distributionConfiguration": DistributionConfigurationTypeDef,
-        "imageTestsConfiguration": ImageTestsConfigurationOutputTypeDef,
+        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
         "dateCreated": str,
         "outputResources": OutputResourcesTypeDef,
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
         "scanState": ImageScanStateTypeDef,
         "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
@@ -2863,10 +2664,10 @@
 )
 
 GetImageResponseTypeDef = TypedDict(
     "GetImageResponseTypeDef",
     {
         "requestId": str,
         "image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/type_defs.pyi` & `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -41,155 +41,141 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "SeverityCountsTypeDef",
-    "SystemsManagerAgentOutputTypeDef",
     "SystemsManagerAgentTypeDef",
     "LaunchPermissionConfigurationOutputTypeDef",
     "LaunchPermissionConfigurationTypeDef",
     "ImageStateTypeDef",
     "CancelImageCreationRequestRequestTypeDef",
-    "CancelImageCreationResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ComponentParameterOutputTypeDef",
     "ComponentParameterTypeDef",
     "ComponentParameterDetailTypeDef",
     "ComponentStateTypeDef",
     "ComponentVersionTypeDef",
-    "TargetContainerRepositoryOutputTypeDef",
     "TargetContainerRepositoryTypeDef",
     "ContainerRecipeSummaryTypeDef",
     "ContainerTypeDef",
     "CreateComponentRequestRequestTypeDef",
-    "CreateComponentResponseTypeDef",
-    "CreateContainerRecipeResponseTypeDef",
-    "CreateDistributionConfigurationResponseTypeDef",
     "ImageTestsConfigurationTypeDef",
     "ScheduleTypeDef",
-    "CreateImagePipelineResponseTypeDef",
-    "CreateImageRecipeResponseTypeDef",
-    "CreateImageResponseTypeDef",
     "InstanceMetadataOptionsTypeDef",
-    "CreateInfrastructureConfigurationResponseTypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DeleteComponentRequestRequestTypeDef",
-    "DeleteComponentResponseTypeDef",
     "DeleteContainerRecipeRequestRequestTypeDef",
-    "DeleteContainerRecipeResponseTypeDef",
     "DeleteDistributionConfigurationRequestRequestTypeDef",
-    "DeleteDistributionConfigurationResponseTypeDef",
     "DeleteImagePipelineRequestRequestTypeDef",
-    "DeleteImagePipelineResponseTypeDef",
     "DeleteImageRecipeRequestRequestTypeDef",
-    "DeleteImageRecipeResponseTypeDef",
     "DeleteImageRequestRequestTypeDef",
-    "DeleteImageResponseTypeDef",
     "DeleteInfrastructureConfigurationRequestRequestTypeDef",
-    "DeleteInfrastructureConfigurationResponseTypeDef",
     "DistributionConfigurationSummaryTypeDef",
-    "LaunchTemplateConfigurationOutputTypeDef",
-    "S3ExportConfigurationOutputTypeDef",
     "LaunchTemplateConfigurationTypeDef",
     "S3ExportConfigurationTypeDef",
-    "EbsInstanceBlockDeviceSpecificationOutputTypeDef",
     "EbsInstanceBlockDeviceSpecificationTypeDef",
     "EcrConfigurationOutputTypeDef",
     "EcrConfigurationTypeDef",
-    "FastLaunchLaunchTemplateSpecificationOutputTypeDef",
-    "FastLaunchSnapshotConfigurationOutputTypeDef",
     "FastLaunchLaunchTemplateSpecificationTypeDef",
     "FastLaunchSnapshotConfigurationTypeDef",
     "FilterTypeDef",
     "GetComponentPolicyRequestRequestTypeDef",
-    "GetComponentPolicyResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetContainerRecipePolicyRequestRequestTypeDef",
-    "GetContainerRecipePolicyResponseTypeDef",
     "GetContainerRecipeRequestRequestTypeDef",
     "GetDistributionConfigurationRequestRequestTypeDef",
     "GetImagePipelineRequestRequestTypeDef",
     "GetImagePolicyRequestRequestTypeDef",
-    "GetImagePolicyResponseTypeDef",
     "GetImageRecipePolicyRequestRequestTypeDef",
-    "GetImageRecipePolicyResponseTypeDef",
     "GetImageRecipeRequestRequestTypeDef",
     "GetImageRequestRequestTypeDef",
     "GetInfrastructureConfigurationRequestRequestTypeDef",
     "GetWorkflowExecutionRequestRequestTypeDef",
-    "GetWorkflowExecutionResponseTypeDef",
     "GetWorkflowStepExecutionRequestRequestTypeDef",
-    "GetWorkflowStepExecutionResponseTypeDef",
     "ImagePackageTypeDef",
-    "ImageTestsConfigurationOutputTypeDef",
-    "ScheduleOutputTypeDef",
     "ImageRecipeSummaryTypeDef",
     "ImageScanFindingsFilterTypeDef",
     "ImageScanStateTypeDef",
     "ImageVersionTypeDef",
     "ImportComponentRequestRequestTypeDef",
-    "ImportComponentResponseTypeDef",
     "ImportVmImageRequestRequestTypeDef",
-    "ImportVmImageResponseTypeDef",
     "InfrastructureConfigurationSummaryTypeDef",
-    "InstanceMetadataOptionsOutputTypeDef",
     "ListComponentBuildVersionsRequestRequestTypeDef",
     "ListImagePackagesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWorkflowExecutionsRequestRequestTypeDef",
     "WorkflowExecutionMetadataTypeDef",
     "ListWorkflowStepExecutionsRequestRequestTypeDef",
     "WorkflowStepMetadataTypeDef",
-    "S3LogsOutputTypeDef",
     "S3LogsTypeDef",
     "VulnerablePackageTypeDef",
     "PutComponentPolicyRequestRequestTypeDef",
-    "PutComponentPolicyResponseTypeDef",
     "PutContainerRecipePolicyRequestRequestTypeDef",
-    "PutContainerRecipePolicyResponseTypeDef",
     "PutImagePolicyRequestRequestTypeDef",
-    "PutImagePolicyResponseTypeDef",
     "PutImageRecipePolicyRequestRequestTypeDef",
-    "PutImageRecipePolicyResponseTypeDef",
     "RemediationRecommendationTypeDef",
-    "ResponseMetadataTypeDef",
     "StartImagePipelineExecutionRequestRequestTypeDef",
-    "StartImagePipelineExecutionResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateDistributionConfigurationResponseTypeDef",
-    "UpdateImagePipelineResponseTypeDef",
-    "UpdateInfrastructureConfigurationResponseTypeDef",
     "AccountAggregationTypeDef",
     "ImageAggregationTypeDef",
     "ImagePipelineAggregationTypeDef",
     "VulnerabilityIdAggregationTypeDef",
-    "AdditionalInstanceConfigurationOutputTypeDef",
     "AdditionalInstanceConfigurationTypeDef",
     "AmiDistributionConfigurationOutputTypeDef",
     "AmiDistributionConfigurationTypeDef",
     "AmiTypeDef",
+    "CancelImageCreationResponseTypeDef",
+    "CreateComponentResponseTypeDef",
+    "CreateContainerRecipeResponseTypeDef",
+    "CreateDistributionConfigurationResponseTypeDef",
+    "CreateImagePipelineResponseTypeDef",
+    "CreateImageRecipeResponseTypeDef",
+    "CreateImageResponseTypeDef",
+    "CreateInfrastructureConfigurationResponseTypeDef",
+    "DeleteComponentResponseTypeDef",
+    "DeleteContainerRecipeResponseTypeDef",
+    "DeleteDistributionConfigurationResponseTypeDef",
+    "DeleteImagePipelineResponseTypeDef",
+    "DeleteImageRecipeResponseTypeDef",
+    "DeleteImageResponseTypeDef",
+    "DeleteInfrastructureConfigurationResponseTypeDef",
+    "GetComponentPolicyResponseTypeDef",
+    "GetContainerRecipePolicyResponseTypeDef",
+    "GetImagePolicyResponseTypeDef",
+    "GetImageRecipePolicyResponseTypeDef",
+    "GetWorkflowExecutionResponseTypeDef",
+    "GetWorkflowStepExecutionResponseTypeDef",
+    "ImportComponentResponseTypeDef",
+    "ImportVmImageResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutComponentPolicyResponseTypeDef",
+    "PutContainerRecipePolicyResponseTypeDef",
+    "PutImagePolicyResponseTypeDef",
+    "PutImageRecipePolicyResponseTypeDef",
+    "StartImagePipelineExecutionResponseTypeDef",
+    "UpdateDistributionConfigurationResponseTypeDef",
+    "UpdateImagePipelineResponseTypeDef",
+    "UpdateInfrastructureConfigurationResponseTypeDef",
     "ComponentConfigurationOutputTypeDef",
     "ComponentConfigurationTypeDef",
     "ComponentSummaryTypeDef",
     "ComponentTypeDef",
     "ListComponentsResponseTypeDef",
     "ContainerDistributionConfigurationOutputTypeDef",
     "ContainerDistributionConfigurationTypeDef",
     "ListContainerRecipesResponseTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDistributionConfigurationsResponseTypeDef",
-    "InstanceBlockDeviceMappingOutputTypeDef",
     "InstanceBlockDeviceMappingTypeDef",
     "ImageScanningConfigurationOutputTypeDef",
     "ImageScanningConfigurationTypeDef",
-    "FastLaunchConfigurationOutputTypeDef",
     "FastLaunchConfigurationTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListContainerRecipesRequestRequestTypeDef",
     "ListDistributionConfigurationsRequestRequestTypeDef",
     "ListImageBuildVersionsRequestRequestTypeDef",
     "ListImagePipelineImagesRequestRequestTypeDef",
     "ListImagePipelinesRequestRequestTypeDef",
@@ -200,35 +186,34 @@
     "ListImagePackagesResponseTypeDef",
     "ListImageRecipesResponseTypeDef",
     "ListImageScanFindingsRequestRequestTypeDef",
     "ListImagesResponseTypeDef",
     "ListInfrastructureConfigurationsResponseTypeDef",
     "ListWorkflowExecutionsResponseTypeDef",
     "ListWorkflowStepExecutionsResponseTypeDef",
-    "LoggingOutputTypeDef",
     "LoggingTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "ImageScanFindingAggregationTypeDef",
     "OutputResourcesTypeDef",
     "ListComponentBuildVersionsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "InspectorScoreDetailsTypeDef",
+    "CreateImageRecipeRequestRequestTypeDef",
     "ImageRecipeTypeDef",
     "InstanceConfigurationOutputTypeDef",
-    "CreateImageRecipeRequestRequestTypeDef",
     "InstanceConfigurationTypeDef",
     "ImagePipelineTypeDef",
     "CreateImagePipelineRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
     "UpdateImagePipelineRequestRequestTypeDef",
     "DistributionOutputTypeDef",
     "DistributionTypeDef",
-    "InfrastructureConfigurationTypeDef",
     "CreateInfrastructureConfigurationRequestRequestTypeDef",
+    "InfrastructureConfigurationTypeDef",
     "UpdateInfrastructureConfigurationRequestRequestTypeDef",
     "ListImageScanFindingAggregationsResponseTypeDef",
     "ImageSummaryTypeDef",
     "ImageScanFindingTypeDef",
     "GetImageRecipeResponseTypeDef",
     "ContainerRecipeTypeDef",
     "CreateContainerRecipeRequestRequestTypeDef",
@@ -254,22 +239,14 @@
         "critical": int,
         "high": int,
         "medium": int,
     },
     total=False,
 )
 
-SystemsManagerAgentOutputTypeDef = TypedDict(
-    "SystemsManagerAgentOutputTypeDef",
-    {
-        "uninstallAfterBuild": bool,
-    },
-    total=False,
-)
-
 SystemsManagerAgentTypeDef = TypedDict(
     "SystemsManagerAgentTypeDef",
     {
         "uninstallAfterBuild": bool,
     },
     total=False,
 )
@@ -309,21 +286,22 @@
     "CancelImageCreationRequestRequestTypeDef",
     {
         "imageBuildVersionArn": str,
         "clientToken": str,
     },
 )
 
-CancelImageCreationResponseTypeDef = TypedDict(
-    "CancelImageCreationResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "requestId": str,
-        "clientToken": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ComponentParameterOutputTypeDef = TypedDict(
     "ComponentParameterOutputTypeDef",
     {
         "name": str,
@@ -381,22 +359,14 @@
         "type": ComponentTypeType,
         "owner": str,
         "dateCreated": str,
     },
     total=False,
 )
 
-TargetContainerRepositoryOutputTypeDef = TypedDict(
-    "TargetContainerRepositoryOutputTypeDef",
-    {
-        "service": Literal["ECR"],
-        "repositoryName": str,
-    },
-)
-
 TargetContainerRepositoryTypeDef = TypedDict(
     "TargetContainerRepositoryTypeDef",
     {
         "service": Literal["ECR"],
         "repositoryName": str,
     },
 )
@@ -449,44 +419,14 @@
 )
 
 class CreateComponentRequestRequestTypeDef(
     _RequiredCreateComponentRequestRequestTypeDef, _OptionalCreateComponentRequestRequestTypeDef
 ):
     pass
 
-CreateComponentResponseTypeDef = TypedDict(
-    "CreateComponentResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "componentBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateContainerRecipeResponseTypeDef = TypedDict(
-    "CreateContainerRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "containerRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDistributionConfigurationResponseTypeDef = TypedDict(
-    "CreateDistributionConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "distributionConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImageTestsConfigurationTypeDef = TypedDict(
     "ImageTestsConfigurationTypeDef",
     {
         "imageTestsEnabled": bool,
         "timeoutMinutes": int,
     },
     total=False,
@@ -498,63 +438,23 @@
         "scheduleExpression": str,
         "timezone": str,
         "pipelineExecutionStartCondition": PipelineExecutionStartConditionType,
     },
     total=False,
 )
 
-CreateImagePipelineResponseTypeDef = TypedDict(
-    "CreateImagePipelineResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imagePipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateImageRecipeResponseTypeDef = TypedDict(
-    "CreateImageRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imageRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateImageResponseTypeDef = TypedDict(
-    "CreateImageResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InstanceMetadataOptionsTypeDef = TypedDict(
     "InstanceMetadataOptionsTypeDef",
     {
         "httpTokens": str,
         "httpPutResponseHopLimit": int,
     },
     total=False,
 )
 
-CreateInfrastructureConfigurationResponseTypeDef = TypedDict(
-    "CreateInfrastructureConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "infrastructureConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CvssScoreAdjustmentTypeDef = TypedDict(
     "CvssScoreAdjustmentTypeDef",
     {
         "metric": str,
         "reason": str,
     },
     total=False,
@@ -574,175 +474,70 @@
 DeleteComponentRequestRequestTypeDef = TypedDict(
     "DeleteComponentRequestRequestTypeDef",
     {
         "componentBuildVersionArn": str,
     },
 )
 
-DeleteComponentResponseTypeDef = TypedDict(
-    "DeleteComponentResponseTypeDef",
-    {
-        "requestId": str,
-        "componentBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteContainerRecipeRequestRequestTypeDef = TypedDict(
     "DeleteContainerRecipeRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
     },
 )
 
-DeleteContainerRecipeResponseTypeDef = TypedDict(
-    "DeleteContainerRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "containerRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteDistributionConfigurationRequestRequestTypeDef",
     {
         "distributionConfigurationArn": str,
     },
 )
 
-DeleteDistributionConfigurationResponseTypeDef = TypedDict(
-    "DeleteDistributionConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "distributionConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImagePipelineRequestRequestTypeDef = TypedDict(
     "DeleteImagePipelineRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
     },
 )
 
-DeleteImagePipelineResponseTypeDef = TypedDict(
-    "DeleteImagePipelineResponseTypeDef",
-    {
-        "requestId": str,
-        "imagePipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImageRecipeRequestRequestTypeDef = TypedDict(
     "DeleteImageRecipeRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
     },
 )
 
-DeleteImageRecipeResponseTypeDef = TypedDict(
-    "DeleteImageRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "imageRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImageRequestRequestTypeDef = TypedDict(
     "DeleteImageRequestRequestTypeDef",
     {
         "imageBuildVersionArn": str,
     },
 )
 
-DeleteImageResponseTypeDef = TypedDict(
-    "DeleteImageResponseTypeDef",
-    {
-        "requestId": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteInfrastructureConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteInfrastructureConfigurationRequestRequestTypeDef",
     {
         "infrastructureConfigurationArn": str,
     },
 )
 
-DeleteInfrastructureConfigurationResponseTypeDef = TypedDict(
-    "DeleteInfrastructureConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "infrastructureConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DistributionConfigurationSummaryTypeDef = TypedDict(
     "DistributionConfigurationSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
         "dateCreated": str,
         "dateUpdated": str,
         "tags": Dict[str, str],
         "regions": List[str],
     },
     total=False,
 )
 
-_RequiredLaunchTemplateConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLaunchTemplateConfigurationOutputTypeDef",
-    {
-        "launchTemplateId": str,
-    },
-)
-_OptionalLaunchTemplateConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLaunchTemplateConfigurationOutputTypeDef",
-    {
-        "accountId": str,
-        "setDefaultVersion": bool,
-    },
-    total=False,
-)
-
-class LaunchTemplateConfigurationOutputTypeDef(
-    _RequiredLaunchTemplateConfigurationOutputTypeDef,
-    _OptionalLaunchTemplateConfigurationOutputTypeDef,
-):
-    pass
-
-_RequiredS3ExportConfigurationOutputTypeDef = TypedDict(
-    "_RequiredS3ExportConfigurationOutputTypeDef",
-    {
-        "roleName": str,
-        "diskImageFormat": DiskImageFormatType,
-        "s3Bucket": str,
-    },
-)
-_OptionalS3ExportConfigurationOutputTypeDef = TypedDict(
-    "_OptionalS3ExportConfigurationOutputTypeDef",
-    {
-        "s3Prefix": str,
-    },
-    total=False,
-)
-
-class S3ExportConfigurationOutputTypeDef(
-    _RequiredS3ExportConfigurationOutputTypeDef, _OptionalS3ExportConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredLaunchTemplateConfigurationTypeDef = TypedDict(
     "_RequiredLaunchTemplateConfigurationTypeDef",
     {
         "launchTemplateId": str,
     },
 )
 _OptionalLaunchTemplateConfigurationTypeDef = TypedDict(
@@ -776,29 +571,14 @@
 )
 
 class S3ExportConfigurationTypeDef(
     _RequiredS3ExportConfigurationTypeDef, _OptionalS3ExportConfigurationTypeDef
 ):
     pass
 
-EbsInstanceBlockDeviceSpecificationOutputTypeDef = TypedDict(
-    "EbsInstanceBlockDeviceSpecificationOutputTypeDef",
-    {
-        "encrypted": bool,
-        "deleteOnTermination": bool,
-        "iops": int,
-        "kmsKeyId": str,
-        "snapshotId": str,
-        "volumeSize": int,
-        "volumeType": EbsVolumeTypeType,
-        "throughput": int,
-    },
-    total=False,
-)
-
 EbsInstanceBlockDeviceSpecificationTypeDef = TypedDict(
     "EbsInstanceBlockDeviceSpecificationTypeDef",
     {
         "encrypted": bool,
         "deleteOnTermination": bool,
         "iops": int,
         "kmsKeyId": str,
@@ -824,32 +604,14 @@
     {
         "repositoryName": str,
         "containerTags": Sequence[str],
     },
     total=False,
 )
 
-FastLaunchLaunchTemplateSpecificationOutputTypeDef = TypedDict(
-    "FastLaunchLaunchTemplateSpecificationOutputTypeDef",
-    {
-        "launchTemplateId": str,
-        "launchTemplateName": str,
-        "launchTemplateVersion": str,
-    },
-    total=False,
-)
-
-FastLaunchSnapshotConfigurationOutputTypeDef = TypedDict(
-    "FastLaunchSnapshotConfigurationOutputTypeDef",
-    {
-        "targetResourceCount": int,
-    },
-    total=False,
-)
-
 FastLaunchLaunchTemplateSpecificationTypeDef = TypedDict(
     "FastLaunchLaunchTemplateSpecificationTypeDef",
     {
         "launchTemplateId": str,
         "launchTemplateName": str,
         "launchTemplateVersion": str,
     },
@@ -876,46 +638,28 @@
 GetComponentPolicyRequestRequestTypeDef = TypedDict(
     "GetComponentPolicyRequestRequestTypeDef",
     {
         "componentArn": str,
     },
 )
 
-GetComponentPolicyResponseTypeDef = TypedDict(
-    "GetComponentPolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetComponentRequestRequestTypeDef = TypedDict(
     "GetComponentRequestRequestTypeDef",
     {
         "componentBuildVersionArn": str,
     },
 )
 
 GetContainerRecipePolicyRequestRequestTypeDef = TypedDict(
     "GetContainerRecipePolicyRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
     },
 )
 
-GetContainerRecipePolicyResponseTypeDef = TypedDict(
-    "GetContainerRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetContainerRecipeRequestRequestTypeDef = TypedDict(
     "GetContainerRecipeRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
     },
 )
 
@@ -936,39 +680,21 @@
 GetImagePolicyRequestRequestTypeDef = TypedDict(
     "GetImagePolicyRequestRequestTypeDef",
     {
         "imageArn": str,
     },
 )
 
-GetImagePolicyResponseTypeDef = TypedDict(
-    "GetImagePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetImageRecipePolicyRequestRequestTypeDef = TypedDict(
     "GetImageRecipePolicyRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
     },
 )
 
-GetImageRecipePolicyResponseTypeDef = TypedDict(
-    "GetImageRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetImageRecipeRequestRequestTypeDef = TypedDict(
     "GetImageRecipeRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
     },
 )
 
@@ -989,93 +715,30 @@
 GetWorkflowExecutionRequestRequestTypeDef = TypedDict(
     "GetWorkflowExecutionRequestRequestTypeDef",
     {
         "workflowExecutionId": str,
     },
 )
 
-GetWorkflowExecutionResponseTypeDef = TypedDict(
-    "GetWorkflowExecutionResponseTypeDef",
-    {
-        "requestId": str,
-        "workflowBuildVersionArn": str,
-        "workflowExecutionId": str,
-        "imageBuildVersionArn": str,
-        "type": WorkflowTypeType,
-        "status": WorkflowExecutionStatusType,
-        "message": str,
-        "totalStepCount": int,
-        "totalStepsSucceeded": int,
-        "totalStepsFailed": int,
-        "totalStepsSkipped": int,
-        "startTime": str,
-        "endTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkflowStepExecutionRequestRequestTypeDef = TypedDict(
     "GetWorkflowStepExecutionRequestRequestTypeDef",
     {
         "stepExecutionId": str,
     },
 )
 
-GetWorkflowStepExecutionResponseTypeDef = TypedDict(
-    "GetWorkflowStepExecutionResponseTypeDef",
-    {
-        "requestId": str,
-        "stepExecutionId": str,
-        "workflowBuildVersionArn": str,
-        "workflowExecutionId": str,
-        "imageBuildVersionArn": str,
-        "name": str,
-        "description": str,
-        "action": str,
-        "status": WorkflowStepExecutionStatusType,
-        "rollbackStatus": WorkflowStepExecutionRollbackStatusType,
-        "message": str,
-        "inputs": str,
-        "outputs": str,
-        "startTime": str,
-        "endTime": str,
-        "onFailure": str,
-        "timeoutSeconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImagePackageTypeDef = TypedDict(
     "ImagePackageTypeDef",
     {
         "packageName": str,
         "packageVersion": str,
     },
     total=False,
 )
 
-ImageTestsConfigurationOutputTypeDef = TypedDict(
-    "ImageTestsConfigurationOutputTypeDef",
-    {
-        "imageTestsEnabled": bool,
-        "timeoutMinutes": int,
-    },
-    total=False,
-)
-
-ScheduleOutputTypeDef = TypedDict(
-    "ScheduleOutputTypeDef",
-    {
-        "scheduleExpression": str,
-        "timezone": str,
-        "pipelineExecutionStartCondition": PipelineExecutionStartConditionType,
-    },
-    total=False,
-)
-
 ImageRecipeSummaryTypeDef = TypedDict(
     "ImageRecipeSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "platform": PlatformType,
         "owner": str,
@@ -1146,24 +809,14 @@
 )
 
 class ImportComponentRequestRequestTypeDef(
     _RequiredImportComponentRequestRequestTypeDef, _OptionalImportComponentRequestRequestTypeDef
 ):
     pass
 
-ImportComponentResponseTypeDef = TypedDict(
-    "ImportComponentResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "componentBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredImportVmImageRequestRequestTypeDef = TypedDict(
     "_RequiredImportVmImageRequestRequestTypeDef",
     {
         "name": str,
         "semanticVersion": str,
         "platform": PlatformType,
         "vmImportTaskId": str,
@@ -1181,24 +834,14 @@
 )
 
 class ImportVmImageRequestRequestTypeDef(
     _RequiredImportVmImageRequestRequestTypeDef, _OptionalImportVmImageRequestRequestTypeDef
 ):
     pass
 
-ImportVmImageResponseTypeDef = TypedDict(
-    "ImportVmImageResponseTypeDef",
-    {
-        "requestId": str,
-        "imageArn": str,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InfrastructureConfigurationSummaryTypeDef = TypedDict(
     "InfrastructureConfigurationSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
         "dateCreated": str,
@@ -1207,23 +850,14 @@
         "tags": Dict[str, str],
         "instanceTypes": List[str],
         "instanceProfileName": str,
     },
     total=False,
 )
 
-InstanceMetadataOptionsOutputTypeDef = TypedDict(
-    "InstanceMetadataOptionsOutputTypeDef",
-    {
-        "httpTokens": str,
-        "httpPutResponseHopLimit": int,
-    },
-    total=False,
-)
-
 _RequiredListComponentBuildVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentBuildVersionsRequestRequestTypeDef",
     {
         "componentVersionArn": str,
     },
 )
 _OptionalListComponentBuildVersionsRequestRequestTypeDef = TypedDict(
@@ -1264,22 +898,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListWorkflowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkflowExecutionsRequestRequestTypeDef",
     {
         "imageBuildVersionArn": str,
     },
 )
 _OptionalListWorkflowExecutionsRequestRequestTypeDef = TypedDict(
@@ -1350,23 +976,14 @@
         "outputs": str,
         "startTime": str,
         "endTime": str,
     },
     total=False,
 )
 
-S3LogsOutputTypeDef = TypedDict(
-    "S3LogsOutputTypeDef",
-    {
-        "s3BucketName": str,
-        "s3KeyPrefix": str,
-    },
-    total=False,
-)
-
 S3LogsTypeDef = TypedDict(
     "S3LogsTypeDef",
     {
         "s3BucketName": str,
         "s3KeyPrefix": str,
     },
     total=False,
@@ -1393,112 +1010,55 @@
     "PutComponentPolicyRequestRequestTypeDef",
     {
         "componentArn": str,
         "policy": str,
     },
 )
 
-PutComponentPolicyResponseTypeDef = TypedDict(
-    "PutComponentPolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "componentArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutContainerRecipePolicyRequestRequestTypeDef = TypedDict(
     "PutContainerRecipePolicyRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
         "policy": str,
     },
 )
 
-PutContainerRecipePolicyResponseTypeDef = TypedDict(
-    "PutContainerRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "containerRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutImagePolicyRequestRequestTypeDef = TypedDict(
     "PutImagePolicyRequestRequestTypeDef",
     {
         "imageArn": str,
         "policy": str,
     },
 )
 
-PutImagePolicyResponseTypeDef = TypedDict(
-    "PutImagePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "imageArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutImageRecipePolicyRequestRequestTypeDef = TypedDict(
     "PutImageRecipePolicyRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
         "policy": str,
     },
 )
 
-PutImageRecipePolicyResponseTypeDef = TypedDict(
-    "PutImageRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "imageRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemediationRecommendationTypeDef = TypedDict(
     "RemediationRecommendationTypeDef",
     {
         "text": str,
         "url": str,
     },
     total=False,
 )
 
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
 StartImagePipelineExecutionRequestRequestTypeDef = TypedDict(
     "StartImagePipelineExecutionRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
         "clientToken": str,
     },
 )
 
-StartImagePipelineExecutionResponseTypeDef = TypedDict(
-    "StartImagePipelineExecutionResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1507,44 +1067,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateDistributionConfigurationResponseTypeDef = TypedDict(
-    "UpdateDistributionConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "distributionConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateImagePipelineResponseTypeDef = TypedDict(
-    "UpdateImagePipelineResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imagePipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateInfrastructureConfigurationResponseTypeDef = TypedDict(
-    "UpdateInfrastructureConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "infrastructureConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AccountAggregationTypeDef = TypedDict(
     "AccountAggregationTypeDef",
     {
         "accountId": str,
         "severityCounts": SeverityCountsTypeDef,
     },
     total=False,
@@ -1573,23 +1103,14 @@
     {
         "vulnerabilityId": str,
         "severityCounts": SeverityCountsTypeDef,
     },
     total=False,
 )
 
-AdditionalInstanceConfigurationOutputTypeDef = TypedDict(
-    "AdditionalInstanceConfigurationOutputTypeDef",
-    {
-        "systemsManagerAgent": SystemsManagerAgentOutputTypeDef,
-        "userDataOverride": str,
-    },
-    total=False,
-)
-
 AdditionalInstanceConfigurationTypeDef = TypedDict(
     "AdditionalInstanceConfigurationTypeDef",
     {
         "systemsManagerAgent": SystemsManagerAgentTypeDef,
         "userDataOverride": str,
     },
     total=False,
@@ -1630,14 +1151,341 @@
         "description": str,
         "state": ImageStateTypeDef,
         "accountId": str,
     },
     total=False,
 )
 
+CancelImageCreationResponseTypeDef = TypedDict(
+    "CancelImageCreationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateComponentResponseTypeDef = TypedDict(
+    "CreateComponentResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "componentBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateContainerRecipeResponseTypeDef = TypedDict(
+    "CreateContainerRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "containerRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDistributionConfigurationResponseTypeDef = TypedDict(
+    "CreateDistributionConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "distributionConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImagePipelineResponseTypeDef = TypedDict(
+    "CreateImagePipelineResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imagePipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImageRecipeResponseTypeDef = TypedDict(
+    "CreateImageRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImageResponseTypeDef = TypedDict(
+    "CreateImageResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateInfrastructureConfigurationResponseTypeDef = TypedDict(
+    "CreateInfrastructureConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "infrastructureConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteComponentResponseTypeDef = TypedDict(
+    "DeleteComponentResponseTypeDef",
+    {
+        "requestId": str,
+        "componentBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteContainerRecipeResponseTypeDef = TypedDict(
+    "DeleteContainerRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "containerRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDistributionConfigurationResponseTypeDef = TypedDict(
+    "DeleteDistributionConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "distributionConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImagePipelineResponseTypeDef = TypedDict(
+    "DeleteImagePipelineResponseTypeDef",
+    {
+        "requestId": str,
+        "imagePipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImageRecipeResponseTypeDef = TypedDict(
+    "DeleteImageRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "imageRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImageResponseTypeDef = TypedDict(
+    "DeleteImageResponseTypeDef",
+    {
+        "requestId": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteInfrastructureConfigurationResponseTypeDef = TypedDict(
+    "DeleteInfrastructureConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "infrastructureConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetComponentPolicyResponseTypeDef = TypedDict(
+    "GetComponentPolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContainerRecipePolicyResponseTypeDef = TypedDict(
+    "GetContainerRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImagePolicyResponseTypeDef = TypedDict(
+    "GetImagePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImageRecipePolicyResponseTypeDef = TypedDict(
+    "GetImageRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkflowExecutionResponseTypeDef = TypedDict(
+    "GetWorkflowExecutionResponseTypeDef",
+    {
+        "requestId": str,
+        "workflowBuildVersionArn": str,
+        "workflowExecutionId": str,
+        "imageBuildVersionArn": str,
+        "type": WorkflowTypeType,
+        "status": WorkflowExecutionStatusType,
+        "message": str,
+        "totalStepCount": int,
+        "totalStepsSucceeded": int,
+        "totalStepsFailed": int,
+        "totalStepsSkipped": int,
+        "startTime": str,
+        "endTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkflowStepExecutionResponseTypeDef = TypedDict(
+    "GetWorkflowStepExecutionResponseTypeDef",
+    {
+        "requestId": str,
+        "stepExecutionId": str,
+        "workflowBuildVersionArn": str,
+        "workflowExecutionId": str,
+        "imageBuildVersionArn": str,
+        "name": str,
+        "description": str,
+        "action": str,
+        "status": WorkflowStepExecutionStatusType,
+        "rollbackStatus": WorkflowStepExecutionRollbackStatusType,
+        "message": str,
+        "inputs": str,
+        "outputs": str,
+        "startTime": str,
+        "endTime": str,
+        "onFailure": str,
+        "timeoutSeconds": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportComponentResponseTypeDef = TypedDict(
+    "ImportComponentResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "componentBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportVmImageResponseTypeDef = TypedDict(
+    "ImportVmImageResponseTypeDef",
+    {
+        "requestId": str,
+        "imageArn": str,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutComponentPolicyResponseTypeDef = TypedDict(
+    "PutComponentPolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "componentArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutContainerRecipePolicyResponseTypeDef = TypedDict(
+    "PutContainerRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "containerRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutImagePolicyResponseTypeDef = TypedDict(
+    "PutImagePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "imageArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutImageRecipePolicyResponseTypeDef = TypedDict(
+    "PutImageRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "imageRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartImagePipelineExecutionResponseTypeDef = TypedDict(
+    "StartImagePipelineExecutionResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDistributionConfigurationResponseTypeDef = TypedDict(
+    "UpdateDistributionConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "distributionConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateImagePipelineResponseTypeDef = TypedDict(
+    "UpdateImagePipelineResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imagePipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateInfrastructureConfigurationResponseTypeDef = TypedDict(
+    "UpdateInfrastructureConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "infrastructureConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredComponentConfigurationOutputTypeDef = TypedDict(
     "_RequiredComponentConfigurationOutputTypeDef",
     {
         "componentArn": str,
     },
 )
 _OptionalComponentConfigurationOutputTypeDef = TypedDict(
@@ -1720,22 +1568,22 @@
 
 ListComponentsResponseTypeDef = TypedDict(
     "ListComponentsResponseTypeDef",
     {
         "requestId": str,
         "componentVersionList": List[ComponentVersionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredContainerDistributionConfigurationOutputTypeDef = TypedDict(
     "_RequiredContainerDistributionConfigurationOutputTypeDef",
     {
-        "targetRepository": TargetContainerRepositoryOutputTypeDef,
+        "targetRepository": TargetContainerRepositoryTypeDef,
     },
 )
 _OptionalContainerDistributionConfigurationOutputTypeDef = TypedDict(
     "_OptionalContainerDistributionConfigurationOutputTypeDef",
     {
         "description": str,
         "containerTags": List[str],
@@ -1772,15 +1620,15 @@
 
 ListContainerRecipesResponseTypeDef = TypedDict(
     "ListContainerRecipesResponseTypeDef",
     {
         "requestId": str,
         "containerRecipeSummaryList": List[ContainerRecipeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CvssScoreDetailsTypeDef = TypedDict(
     "CvssScoreDetailsTypeDef",
     {
         "scoreSource": str,
@@ -1795,27 +1643,16 @@
 
 ListDistributionConfigurationsResponseTypeDef = TypedDict(
     "ListDistributionConfigurationsResponseTypeDef",
     {
         "requestId": str,
         "distributionConfigurationSummaryList": List[DistributionConfigurationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-InstanceBlockDeviceMappingOutputTypeDef = TypedDict(
-    "InstanceBlockDeviceMappingOutputTypeDef",
-    {
-        "deviceName": str,
-        "ebs": EbsInstanceBlockDeviceSpecificationOutputTypeDef,
-        "virtualName": str,
-        "noDevice": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 InstanceBlockDeviceMappingTypeDef = TypedDict(
     "InstanceBlockDeviceMappingTypeDef",
     {
         "deviceName": str,
         "ebs": EbsInstanceBlockDeviceSpecificationTypeDef,
@@ -1839,36 +1676,14 @@
     {
         "imageScanningEnabled": bool,
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredFastLaunchConfigurationOutputTypeDef = TypedDict(
-    "_RequiredFastLaunchConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-_OptionalFastLaunchConfigurationOutputTypeDef = TypedDict(
-    "_OptionalFastLaunchConfigurationOutputTypeDef",
-    {
-        "snapshotConfiguration": FastLaunchSnapshotConfigurationOutputTypeDef,
-        "maxParallelLaunches": int,
-        "launchTemplate": FastLaunchLaunchTemplateSpecificationOutputTypeDef,
-        "accountId": str,
-    },
-    total=False,
-)
-
-class FastLaunchConfigurationOutputTypeDef(
-    _RequiredFastLaunchConfigurationOutputTypeDef, _OptionalFastLaunchConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredFastLaunchConfigurationTypeDef = TypedDict(
     "_RequiredFastLaunchConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalFastLaunchConfigurationTypeDef = TypedDict(
@@ -2019,25 +1834,25 @@
 
 ListImagePackagesResponseTypeDef = TypedDict(
     "ListImagePackagesResponseTypeDef",
     {
         "requestId": str,
         "imagePackageList": List[ImagePackageTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageRecipesResponseTypeDef = TypedDict(
     "ListImageRecipesResponseTypeDef",
     {
         "requestId": str,
         "imageRecipeSummaryList": List[ImageRecipeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageScanFindingsRequestRequestTypeDef = TypedDict(
     "ListImageScanFindingsRequestRequestTypeDef",
     {
         "filters": Sequence[ImageScanFindingsFilterTypeDef],
@@ -2049,62 +1864,54 @@
 
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
         "requestId": str,
         "imageVersionList": List[ImageVersionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInfrastructureConfigurationsResponseTypeDef = TypedDict(
     "ListInfrastructureConfigurationsResponseTypeDef",
     {
         "requestId": str,
         "infrastructureConfigurationSummaryList": List[InfrastructureConfigurationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowExecutionsResponseTypeDef = TypedDict(
     "ListWorkflowExecutionsResponseTypeDef",
     {
         "requestId": str,
         "workflowExecutions": List[WorkflowExecutionMetadataTypeDef],
         "imageBuildVersionArn": str,
         "message": str,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowStepExecutionsResponseTypeDef = TypedDict(
     "ListWorkflowStepExecutionsResponseTypeDef",
     {
         "requestId": str,
         "steps": List[WorkflowStepMetadataTypeDef],
         "workflowBuildVersionArn": str,
         "workflowExecutionId": str,
         "imageBuildVersionArn": str,
         "message": str,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoggingOutputTypeDef = TypedDict(
-    "LoggingOutputTypeDef",
-    {
-        "s3Logs": S3LogsOutputTypeDef,
-    },
-    total=False,
-)
-
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "s3Logs": S3LogsTypeDef,
     },
     total=False,
 )
@@ -2166,65 +1973,35 @@
 
 ListComponentBuildVersionsResponseTypeDef = TypedDict(
     "ListComponentBuildVersionsResponseTypeDef",
     {
         "requestId": str,
         "componentSummaryList": List[ComponentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComponentResponseTypeDef = TypedDict(
     "GetComponentResponseTypeDef",
     {
         "requestId": str,
         "component": ComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InspectorScoreDetailsTypeDef = TypedDict(
     "InspectorScoreDetailsTypeDef",
     {
         "adjustedCvss": CvssScoreDetailsTypeDef,
     },
     total=False,
 )
 
-ImageRecipeTypeDef = TypedDict(
-    "ImageRecipeTypeDef",
-    {
-        "arn": str,
-        "type": ImageTypeType,
-        "name": str,
-        "description": str,
-        "platform": PlatformType,
-        "owner": str,
-        "version": str,
-        "components": List[ComponentConfigurationOutputTypeDef],
-        "parentImage": str,
-        "blockDeviceMappings": List[InstanceBlockDeviceMappingOutputTypeDef],
-        "dateCreated": str,
-        "tags": Dict[str, str],
-        "workingDirectory": str,
-        "additionalInstanceConfiguration": AdditionalInstanceConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-InstanceConfigurationOutputTypeDef = TypedDict(
-    "InstanceConfigurationOutputTypeDef",
-    {
-        "image": str,
-        "blockDeviceMappings": List[InstanceBlockDeviceMappingOutputTypeDef],
-    },
-    total=False,
-)
-
 _RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageRecipeRequestRequestTypeDef",
     {
         "name": str,
         "semanticVersion": str,
         "components": Sequence[ComponentConfigurationTypeDef],
         "parentImage": str,
@@ -2244,14 +2021,44 @@
 )
 
 class CreateImageRecipeRequestRequestTypeDef(
     _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
 ):
     pass
 
+ImageRecipeTypeDef = TypedDict(
+    "ImageRecipeTypeDef",
+    {
+        "arn": str,
+        "type": ImageTypeType,
+        "name": str,
+        "description": str,
+        "platform": PlatformType,
+        "owner": str,
+        "version": str,
+        "components": List[ComponentConfigurationOutputTypeDef],
+        "parentImage": str,
+        "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
+        "dateCreated": str,
+        "tags": Dict[str, str],
+        "workingDirectory": str,
+        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
+    },
+    total=False,
+)
+
+InstanceConfigurationOutputTypeDef = TypedDict(
+    "InstanceConfigurationOutputTypeDef",
+    {
+        "image": str,
+        "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
+    },
+    total=False,
+)
+
 InstanceConfigurationTypeDef = TypedDict(
     "InstanceConfigurationTypeDef",
     {
         "image": str,
         "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
     },
     total=False,
@@ -2265,16 +2072,16 @@
         "description": str,
         "platform": PlatformType,
         "enhancedImageMetadataEnabled": bool,
         "imageRecipeArn": str,
         "containerRecipeArn": str,
         "infrastructureConfigurationArn": str,
         "distributionConfigurationArn": str,
-        "imageTestsConfiguration": ImageTestsConfigurationOutputTypeDef,
-        "schedule": ScheduleOutputTypeDef,
+        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
+        "schedule": ScheduleTypeDef,
         "status": PipelineStatusType,
         "dateCreated": str,
         "dateUpdated": str,
         "dateLastRun": str,
         "dateNextRun": str,
         "tags": Dict[str, str],
         "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
@@ -2377,17 +2184,17 @@
 )
 _OptionalDistributionOutputTypeDef = TypedDict(
     "_OptionalDistributionOutputTypeDef",
     {
         "amiDistributionConfiguration": AmiDistributionConfigurationOutputTypeDef,
         "containerDistributionConfiguration": ContainerDistributionConfigurationOutputTypeDef,
         "licenseConfigurationArns": List[str],
-        "launchTemplateConfigurations": List[LaunchTemplateConfigurationOutputTypeDef],
-        "s3ExportConfiguration": S3ExportConfigurationOutputTypeDef,
-        "fastLaunchConfigurations": List[FastLaunchConfigurationOutputTypeDef],
+        "launchTemplateConfigurations": List[LaunchTemplateConfigurationTypeDef],
+        "s3ExportConfiguration": S3ExportConfigurationTypeDef,
+        "fastLaunchConfigurations": List[FastLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
 class DistributionOutputTypeDef(
     _RequiredDistributionOutputTypeDef, _OptionalDistributionOutputTypeDef
 ):
@@ -2411,37 +2218,14 @@
     },
     total=False,
 )
 
 class DistributionTypeDef(_RequiredDistributionTypeDef, _OptionalDistributionTypeDef):
     pass
 
-InfrastructureConfigurationTypeDef = TypedDict(
-    "InfrastructureConfigurationTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "instanceTypes": List[str],
-        "instanceProfileName": str,
-        "securityGroupIds": List[str],
-        "subnetId": str,
-        "logging": LoggingOutputTypeDef,
-        "keyPair": str,
-        "terminateInstanceOnFailure": bool,
-        "snsTopicArn": str,
-        "dateCreated": str,
-        "dateUpdated": str,
-        "resourceTags": Dict[str, str],
-        "instanceMetadataOptions": InstanceMetadataOptionsOutputTypeDef,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredCreateInfrastructureConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInfrastructureConfigurationRequestRequestTypeDef",
     {
         "name": str,
         "instanceProfileName": str,
         "clientToken": str,
     },
@@ -2466,14 +2250,37 @@
 
 class CreateInfrastructureConfigurationRequestRequestTypeDef(
     _RequiredCreateInfrastructureConfigurationRequestRequestTypeDef,
     _OptionalCreateInfrastructureConfigurationRequestRequestTypeDef,
 ):
     pass
 
+InfrastructureConfigurationTypeDef = TypedDict(
+    "InfrastructureConfigurationTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "instanceTypes": List[str],
+        "instanceProfileName": str,
+        "securityGroupIds": List[str],
+        "subnetId": str,
+        "logging": LoggingTypeDef,
+        "keyPair": str,
+        "terminateInstanceOnFailure": bool,
+        "snsTopicArn": str,
+        "dateCreated": str,
+        "dateUpdated": str,
+        "resourceTags": Dict[str, str],
+        "instanceMetadataOptions": InstanceMetadataOptionsTypeDef,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredUpdateInfrastructureConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInfrastructureConfigurationRequestRequestTypeDef",
     {
         "infrastructureConfigurationArn": str,
         "instanceProfileName": str,
         "clientToken": str,
     },
@@ -2504,15 +2311,15 @@
 ListImageScanFindingAggregationsResponseTypeDef = TypedDict(
     "ListImageScanFindingAggregationsResponseTypeDef",
     {
         "requestId": str,
         "aggregationType": str,
         "responses": List[ImageScanFindingAggregationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageSummaryTypeDef = TypedDict(
     "ImageSummaryTypeDef",
     {
         "arn": str,
@@ -2554,15 +2361,15 @@
 )
 
 GetImageRecipeResponseTypeDef = TypedDict(
     "GetImageRecipeResponseTypeDef",
     {
         "requestId": str,
         "imageRecipe": ImageRecipeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ContainerRecipeTypeDef = TypedDict(
     "ContainerRecipeTypeDef",
     {
         "arn": str,
@@ -2577,15 +2384,15 @@
         "dockerfileTemplateData": str,
         "kmsKeyId": str,
         "encrypted": bool,
         "parentImage": str,
         "dateCreated": str,
         "tags": Dict[str, str],
         "workingDirectory": str,
-        "targetRepository": TargetContainerRepositoryOutputTypeDef,
+        "targetRepository": TargetContainerRepositoryTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerRecipeRequestRequestTypeDef",
     {
@@ -2621,25 +2428,25 @@
     pass
 
 GetImagePipelineResponseTypeDef = TypedDict(
     "GetImagePipelineResponseTypeDef",
     {
         "requestId": str,
         "imagePipeline": ImagePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImagePipelinesResponseTypeDef = TypedDict(
     "ListImagePipelinesResponseTypeDef",
     {
         "requestId": str,
         "imagePipelineList": List[ImagePipelineTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDistributionConfigurationTypeDef = TypedDict(
     "_RequiredDistributionConfigurationTypeDef",
     {
         "timeoutMinutes": int,
@@ -2710,63 +2517,63 @@
     pass
 
 GetInfrastructureConfigurationResponseTypeDef = TypedDict(
     "GetInfrastructureConfigurationResponseTypeDef",
     {
         "requestId": str,
         "infrastructureConfiguration": InfrastructureConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageBuildVersionsResponseTypeDef = TypedDict(
     "ListImageBuildVersionsResponseTypeDef",
     {
         "requestId": str,
         "imageSummaryList": List[ImageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImagePipelineImagesResponseTypeDef = TypedDict(
     "ListImagePipelineImagesResponseTypeDef",
     {
         "requestId": str,
         "imageSummaryList": List[ImageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageScanFindingsResponseTypeDef = TypedDict(
     "ListImageScanFindingsResponseTypeDef",
     {
         "requestId": str,
         "findings": List[ImageScanFindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContainerRecipeResponseTypeDef = TypedDict(
     "GetContainerRecipeResponseTypeDef",
     {
         "requestId": str,
         "containerRecipe": ContainerRecipeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDistributionConfigurationResponseTypeDef = TypedDict(
     "GetDistributionConfigurationResponseTypeDef",
     {
         "requestId": str,
         "distributionConfiguration": DistributionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "arn": str,
@@ -2779,15 +2586,15 @@
         "state": ImageStateTypeDef,
         "imageRecipe": ImageRecipeTypeDef,
         "containerRecipe": ContainerRecipeTypeDef,
         "sourcePipelineName": str,
         "sourcePipelineArn": str,
         "infrastructureConfiguration": InfrastructureConfigurationTypeDef,
         "distributionConfiguration": DistributionConfigurationTypeDef,
-        "imageTestsConfiguration": ImageTestsConfigurationOutputTypeDef,
+        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
         "dateCreated": str,
         "outputResources": OutputResourcesTypeDef,
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
         "scanState": ImageScanStateTypeDef,
         "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
@@ -2796,10 +2603,10 @@
 )
 
 GetImageResponseTypeDef = TypedDict(
     "GetImageResponseTypeDef",
     {
         "requestId": str,
         "image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/PKG-INFO` & `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-imagebuilder
-Version: 1.28.12
-Summary: Type annotations for boto3.imagebuilder 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.imagebuilder 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-imagebuilder)](https://pepy.tech/project/mypy-boto3-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.imagebuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[boto3.imagebuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [mypy-boto3-imagebuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,155 +316,141 @@
 
 `mypy_boto3_imagebuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_imagebuilder.type_defs import (
     SeverityCountsTypeDef,
-    SystemsManagerAgentOutputTypeDef,
     SystemsManagerAgentTypeDef,
     LaunchPermissionConfigurationOutputTypeDef,
     LaunchPermissionConfigurationTypeDef,
     ImageStateTypeDef,
     CancelImageCreationRequestRequestTypeDef,
-    CancelImageCreationResponseTypeDef,
+    ResponseMetadataTypeDef,
     ComponentParameterOutputTypeDef,
     ComponentParameterTypeDef,
     ComponentParameterDetailTypeDef,
     ComponentStateTypeDef,
     ComponentVersionTypeDef,
-    TargetContainerRepositoryOutputTypeDef,
     TargetContainerRepositoryTypeDef,
     ContainerRecipeSummaryTypeDef,
     ContainerTypeDef,
     CreateComponentRequestRequestTypeDef,
-    CreateComponentResponseTypeDef,
-    CreateContainerRecipeResponseTypeDef,
-    CreateDistributionConfigurationResponseTypeDef,
     ImageTestsConfigurationTypeDef,
     ScheduleTypeDef,
-    CreateImagePipelineResponseTypeDef,
-    CreateImageRecipeResponseTypeDef,
-    CreateImageResponseTypeDef,
     InstanceMetadataOptionsTypeDef,
-    CreateInfrastructureConfigurationResponseTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteComponentRequestRequestTypeDef,
-    DeleteComponentResponseTypeDef,
     DeleteContainerRecipeRequestRequestTypeDef,
-    DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationRequestRequestTypeDef,
-    DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineRequestRequestTypeDef,
-    DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeRequestRequestTypeDef,
-    DeleteImageRecipeResponseTypeDef,
     DeleteImageRequestRequestTypeDef,
-    DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationRequestRequestTypeDef,
-    DeleteInfrastructureConfigurationResponseTypeDef,
     DistributionConfigurationSummaryTypeDef,
-    LaunchTemplateConfigurationOutputTypeDef,
-    S3ExportConfigurationOutputTypeDef,
     LaunchTemplateConfigurationTypeDef,
     S3ExportConfigurationTypeDef,
-    EbsInstanceBlockDeviceSpecificationOutputTypeDef,
     EbsInstanceBlockDeviceSpecificationTypeDef,
     EcrConfigurationOutputTypeDef,
     EcrConfigurationTypeDef,
-    FastLaunchLaunchTemplateSpecificationOutputTypeDef,
-    FastLaunchSnapshotConfigurationOutputTypeDef,
     FastLaunchLaunchTemplateSpecificationTypeDef,
     FastLaunchSnapshotConfigurationTypeDef,
     FilterTypeDef,
     GetComponentPolicyRequestRequestTypeDef,
-    GetComponentPolicyResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetContainerRecipePolicyRequestRequestTypeDef,
-    GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeRequestRequestTypeDef,
     GetDistributionConfigurationRequestRequestTypeDef,
     GetImagePipelineRequestRequestTypeDef,
     GetImagePolicyRequestRequestTypeDef,
-    GetImagePolicyResponseTypeDef,
     GetImageRecipePolicyRequestRequestTypeDef,
-    GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeRequestRequestTypeDef,
     GetImageRequestRequestTypeDef,
     GetInfrastructureConfigurationRequestRequestTypeDef,
     GetWorkflowExecutionRequestRequestTypeDef,
-    GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionRequestRequestTypeDef,
-    GetWorkflowStepExecutionResponseTypeDef,
     ImagePackageTypeDef,
-    ImageTestsConfigurationOutputTypeDef,
-    ScheduleOutputTypeDef,
     ImageRecipeSummaryTypeDef,
     ImageScanFindingsFilterTypeDef,
     ImageScanStateTypeDef,
     ImageVersionTypeDef,
     ImportComponentRequestRequestTypeDef,
-    ImportComponentResponseTypeDef,
     ImportVmImageRequestRequestTypeDef,
-    ImportVmImageResponseTypeDef,
     InfrastructureConfigurationSummaryTypeDef,
-    InstanceMetadataOptionsOutputTypeDef,
     ListComponentBuildVersionsRequestRequestTypeDef,
     ListImagePackagesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkflowExecutionsRequestRequestTypeDef,
     WorkflowExecutionMetadataTypeDef,
     ListWorkflowStepExecutionsRequestRequestTypeDef,
     WorkflowStepMetadataTypeDef,
-    S3LogsOutputTypeDef,
     S3LogsTypeDef,
     VulnerablePackageTypeDef,
     PutComponentPolicyRequestRequestTypeDef,
-    PutComponentPolicyResponseTypeDef,
     PutContainerRecipePolicyRequestRequestTypeDef,
-    PutContainerRecipePolicyResponseTypeDef,
     PutImagePolicyRequestRequestTypeDef,
-    PutImagePolicyResponseTypeDef,
     PutImageRecipePolicyRequestRequestTypeDef,
-    PutImageRecipePolicyResponseTypeDef,
     RemediationRecommendationTypeDef,
-    ResponseMetadataTypeDef,
     StartImagePipelineExecutionRequestRequestTypeDef,
-    StartImagePipelineExecutionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateDistributionConfigurationResponseTypeDef,
-    UpdateImagePipelineResponseTypeDef,
-    UpdateInfrastructureConfigurationResponseTypeDef,
     AccountAggregationTypeDef,
     ImageAggregationTypeDef,
     ImagePipelineAggregationTypeDef,
     VulnerabilityIdAggregationTypeDef,
-    AdditionalInstanceConfigurationOutputTypeDef,
     AdditionalInstanceConfigurationTypeDef,
     AmiDistributionConfigurationOutputTypeDef,
     AmiDistributionConfigurationTypeDef,
     AmiTypeDef,
+    CancelImageCreationResponseTypeDef,
+    CreateComponentResponseTypeDef,
+    CreateContainerRecipeResponseTypeDef,
+    CreateDistributionConfigurationResponseTypeDef,
+    CreateImagePipelineResponseTypeDef,
+    CreateImageRecipeResponseTypeDef,
+    CreateImageResponseTypeDef,
+    CreateInfrastructureConfigurationResponseTypeDef,
+    DeleteComponentResponseTypeDef,
+    DeleteContainerRecipeResponseTypeDef,
+    DeleteDistributionConfigurationResponseTypeDef,
+    DeleteImagePipelineResponseTypeDef,
+    DeleteImageRecipeResponseTypeDef,
+    DeleteImageResponseTypeDef,
+    DeleteInfrastructureConfigurationResponseTypeDef,
+    GetComponentPolicyResponseTypeDef,
+    GetContainerRecipePolicyResponseTypeDef,
+    GetImagePolicyResponseTypeDef,
+    GetImageRecipePolicyResponseTypeDef,
+    GetWorkflowExecutionResponseTypeDef,
+    GetWorkflowStepExecutionResponseTypeDef,
+    ImportComponentResponseTypeDef,
+    ImportVmImageResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutComponentPolicyResponseTypeDef,
+    PutContainerRecipePolicyResponseTypeDef,
+    PutImagePolicyResponseTypeDef,
+    PutImageRecipePolicyResponseTypeDef,
+    StartImagePipelineExecutionResponseTypeDef,
+    UpdateDistributionConfigurationResponseTypeDef,
+    UpdateImagePipelineResponseTypeDef,
+    UpdateInfrastructureConfigurationResponseTypeDef,
     ComponentConfigurationOutputTypeDef,
     ComponentConfigurationTypeDef,
     ComponentSummaryTypeDef,
     ComponentTypeDef,
     ListComponentsResponseTypeDef,
     ContainerDistributionConfigurationOutputTypeDef,
     ContainerDistributionConfigurationTypeDef,
     ListContainerRecipesResponseTypeDef,
     CvssScoreDetailsTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
-    InstanceBlockDeviceMappingOutputTypeDef,
     InstanceBlockDeviceMappingTypeDef,
     ImageScanningConfigurationOutputTypeDef,
     ImageScanningConfigurationTypeDef,
-    FastLaunchConfigurationOutputTypeDef,
     FastLaunchConfigurationTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListContainerRecipesRequestRequestTypeDef,
     ListDistributionConfigurationsRequestRequestTypeDef,
     ListImageBuildVersionsRequestRequestTypeDef,
     ListImagePipelineImagesRequestRequestTypeDef,
     ListImagePipelinesRequestRequestTypeDef,
@@ -475,35 +461,34 @@
     ListImagePackagesResponseTypeDef,
     ListImageRecipesResponseTypeDef,
     ListImageScanFindingsRequestRequestTypeDef,
     ListImagesResponseTypeDef,
     ListInfrastructureConfigurationsResponseTypeDef,
     ListWorkflowExecutionsResponseTypeDef,
     ListWorkflowStepExecutionsResponseTypeDef,
-    LoggingOutputTypeDef,
     LoggingTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ImageScanFindingAggregationTypeDef,
     OutputResourcesTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     GetComponentResponseTypeDef,
     InspectorScoreDetailsTypeDef,
+    CreateImageRecipeRequestRequestTypeDef,
     ImageRecipeTypeDef,
     InstanceConfigurationOutputTypeDef,
-    CreateImageRecipeRequestRequestTypeDef,
     InstanceConfigurationTypeDef,
     ImagePipelineTypeDef,
     CreateImagePipelineRequestRequestTypeDef,
     CreateImageRequestRequestTypeDef,
     UpdateImagePipelineRequestRequestTypeDef,
     DistributionOutputTypeDef,
     DistributionTypeDef,
-    InfrastructureConfigurationTypeDef,
     CreateInfrastructureConfigurationRequestRequestTypeDef,
+    InfrastructureConfigurationTypeDef,
     UpdateInfrastructureConfigurationRequestRequestTypeDef,
     ListImageScanFindingAggregationsResponseTypeDef,
     ImageSummaryTypeDef,
     ImageScanFindingTypeDef,
     GetImageRecipeResponseTypeDef,
     ContainerRecipeTypeDef,
     CreateContainerRecipeRequestRequestTypeDef,
```

### Comparing `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/SOURCES.txt` & `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.12/setup.py` & `mypy-boto3-imagebuilder-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-imagebuilder",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_imagebuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.imagebuilder 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.imagebuilder 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

