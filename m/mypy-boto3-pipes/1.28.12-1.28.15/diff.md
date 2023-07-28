# Comparing `tmp/mypy-boto3-pipes-1.28.12.tar.gz` & `tmp/mypy-boto3-pipes-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pipes-1.28.12.tar", last modified: Thu Jul 27 11:49:24 2023, max compression
+gzip compressed data, was "mypy-boto3-pipes-1.28.15.tar", last modified: Fri Jul 28 20:43:29 2023, max compression
```

## Comparing `mypy-boto3-pipes-1.28.12.tar` & `mypy-boto3-pipes-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.893162 mypy-boto3-pipes-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18250 2023-07-27 11:49:24.885162 mypy-boto3-pipes-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52078 2023-07-27 11:41:42.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52026 2023-07-27 11:41:41.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18250 2023-07-27 11:49:24.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 11:49:24.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:24.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 11:49:24.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:24.893162 mypy-boto3-pipes-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:29.193665 mypy-boto3-pipes-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-07-28 20:43:29.189665 mypy-boto3-pipes-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:29.173665 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42541 2023-07-28 20:33:32.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42499 2023-07-28 20:33:32.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:29.189665 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-07-28 20:43:28.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 20:43:28.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:28.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:28.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:28.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:43:28.000000 mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:29.193665 mypy-boto3-pipes-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-28 20:33:31.000000 mypy-boto3-pipes-1.28.15/setup.py
```

### Comparing `mypy-boto3-pipes-1.28.12/LICENSE` & `mypy-boto3-pipes-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.12/PKG-INFO` & `mypy-boto3-pipes-1.28.15/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pipes
-Version: 1.28.12
-Summary: Type annotations for boto3.EventBridgePipes 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.EventBridgePipes 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pipes)](https://pepy.tech/project/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,82 +338,56 @@
 `mypy_boto3_pipes.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pipes.type_defs import (
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
-    BatchArrayPropertiesOutputTypeDef,
     BatchArrayPropertiesTypeDef,
-    BatchEnvironmentVariableOutputTypeDef,
-    BatchResourceRequirementOutputTypeDef,
     BatchEnvironmentVariableTypeDef,
     BatchResourceRequirementTypeDef,
-    BatchJobDependencyOutputTypeDef,
     BatchJobDependencyTypeDef,
-    BatchRetryStrategyOutputTypeDef,
     BatchRetryStrategyTypeDef,
-    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ResponseMetadataTypeDef,
-    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeletePipeRequestRequestTypeDef,
     DescribePipeRequestRequestTypeDef,
-    EcsEnvironmentFileOutputTypeDef,
-    EcsEnvironmentVariableOutputTypeDef,
-    EcsResourceRequirementOutputTypeDef,
     EcsEnvironmentFileTypeDef,
     EcsEnvironmentVariableTypeDef,
     EcsResourceRequirementTypeDef,
-    EcsEphemeralStorageOutputTypeDef,
     EcsEphemeralStorageTypeDef,
-    EcsInferenceAcceleratorOverrideOutputTypeDef,
     EcsInferenceAcceleratorOverrideTypeDef,
-    FilterOutputTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
     ListPipesRequestRequestTypeDef,
     PipeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    MQBrokerAccessCredentialsOutputTypeDef,
     MQBrokerAccessCredentialsTypeDef,
-    MSKAccessCredentialsOutputTypeDef,
     MSKAccessCredentialsTypeDef,
     PipeEnrichmentHttpParametersOutputTypeDef,
     PipeEnrichmentHttpParametersTypeDef,
-    PipeSourceSqsQueueParametersOutputTypeDef,
     PipeSourceSqsQueueParametersTypeDef,
-    SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef,
-    SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
+    SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     SelfManagedKafkaAccessConfigurationVpcTypeDef,
-    PipeTargetCloudWatchLogsParametersOutputTypeDef,
     PipeTargetCloudWatchLogsParametersTypeDef,
-    PlacementConstraintOutputTypeDef,
-    PlacementStrategyOutputTypeDef,
-    TagOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     TagTypeDef,
     PipeTargetEventBridgeEventBusParametersOutputTypeDef,
     PipeTargetEventBridgeEventBusParametersTypeDef,
     PipeTargetHttpParametersOutputTypeDef,
     PipeTargetHttpParametersTypeDef,
-    PipeTargetKinesisStreamParametersOutputTypeDef,
     PipeTargetKinesisStreamParametersTypeDef,
-    PipeTargetLambdaFunctionParametersOutputTypeDef,
     PipeTargetLambdaFunctionParametersTypeDef,
     PipeTargetRedshiftDataParametersOutputTypeDef,
-    PipeTargetSqsQueueParametersOutputTypeDef,
-    PipeTargetStateMachineParametersOutputTypeDef,
-    PipeTargetRedshiftDataParametersTypeDef,
     PipeTargetSqsQueueParametersTypeDef,
     PipeTargetStateMachineParametersTypeDef,
-    SageMakerPipelineParameterOutputTypeDef,
+    PipeTargetRedshiftDataParametersTypeDef,
     SageMakerPipelineParameterTypeDef,
     StartPipeRequestRequestTypeDef,
     StopPipeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePipeSourceSqsQueueParametersTypeDef,
     NetworkConfigurationOutputTypeDef,
@@ -422,33 +396,29 @@
     BatchContainerOverridesTypeDef,
     CreatePipeResponseTypeDef,
     DeletePipeResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartPipeResponseTypeDef,
     StopPipeResponseTypeDef,
     UpdatePipeResponseTypeDef,
-    PipeSourceDynamoDBStreamParametersOutputTypeDef,
-    PipeSourceKinesisStreamParametersOutputTypeDef,
     PipeSourceDynamoDBStreamParametersTypeDef,
+    PipeSourceKinesisStreamParametersOutputTypeDef,
     PipeSourceKinesisStreamParametersTypeDef,
     UpdatePipeSourceDynamoDBStreamParametersTypeDef,
     UpdatePipeSourceKinesisStreamParametersTypeDef,
     EcsContainerOverrideOutputTypeDef,
     EcsContainerOverrideTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     ListPipesRequestListPipesPaginateTypeDef,
     ListPipesResponseTypeDef,
-    PipeSourceActiveMQBrokerParametersOutputTypeDef,
-    PipeSourceRabbitMQBrokerParametersOutputTypeDef,
     PipeSourceActiveMQBrokerParametersTypeDef,
     PipeSourceRabbitMQBrokerParametersTypeDef,
     UpdatePipeSourceActiveMQBrokerParametersTypeDef,
     UpdatePipeSourceRabbitMQBrokerParametersTypeDef,
-    PipeSourceManagedStreamingKafkaParametersOutputTypeDef,
     PipeSourceManagedStreamingKafkaParametersTypeDef,
     UpdatePipeSourceManagedStreamingKafkaParametersTypeDef,
     PipeEnrichmentParametersOutputTypeDef,
     PipeEnrichmentParametersTypeDef,
     PipeSourceSelfManagedKafkaParametersOutputTypeDef,
     PipeSourceSelfManagedKafkaParametersTypeDef,
     UpdatePipeSourceSelfManagedKafkaParametersTypeDef,
```

### Comparing `mypy-boto3-pipes-1.28.12/README.md` & `mypy-boto3-pipes-1.28.15/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pipes)](https://pepy.tech/project/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,82 +306,56 @@
 `mypy_boto3_pipes.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pipes.type_defs import (
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
-    BatchArrayPropertiesOutputTypeDef,
     BatchArrayPropertiesTypeDef,
-    BatchEnvironmentVariableOutputTypeDef,
-    BatchResourceRequirementOutputTypeDef,
     BatchEnvironmentVariableTypeDef,
     BatchResourceRequirementTypeDef,
-    BatchJobDependencyOutputTypeDef,
     BatchJobDependencyTypeDef,
-    BatchRetryStrategyOutputTypeDef,
     BatchRetryStrategyTypeDef,
-    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ResponseMetadataTypeDef,
-    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeletePipeRequestRequestTypeDef,
     DescribePipeRequestRequestTypeDef,
-    EcsEnvironmentFileOutputTypeDef,
-    EcsEnvironmentVariableOutputTypeDef,
-    EcsResourceRequirementOutputTypeDef,
     EcsEnvironmentFileTypeDef,
     EcsEnvironmentVariableTypeDef,
     EcsResourceRequirementTypeDef,
-    EcsEphemeralStorageOutputTypeDef,
     EcsEphemeralStorageTypeDef,
-    EcsInferenceAcceleratorOverrideOutputTypeDef,
     EcsInferenceAcceleratorOverrideTypeDef,
-    FilterOutputTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
     ListPipesRequestRequestTypeDef,
     PipeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    MQBrokerAccessCredentialsOutputTypeDef,
     MQBrokerAccessCredentialsTypeDef,
-    MSKAccessCredentialsOutputTypeDef,
     MSKAccessCredentialsTypeDef,
     PipeEnrichmentHttpParametersOutputTypeDef,
     PipeEnrichmentHttpParametersTypeDef,
-    PipeSourceSqsQueueParametersOutputTypeDef,
     PipeSourceSqsQueueParametersTypeDef,
-    SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef,
-    SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
+    SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     SelfManagedKafkaAccessConfigurationVpcTypeDef,
-    PipeTargetCloudWatchLogsParametersOutputTypeDef,
     PipeTargetCloudWatchLogsParametersTypeDef,
-    PlacementConstraintOutputTypeDef,
-    PlacementStrategyOutputTypeDef,
-    TagOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     TagTypeDef,
     PipeTargetEventBridgeEventBusParametersOutputTypeDef,
     PipeTargetEventBridgeEventBusParametersTypeDef,
     PipeTargetHttpParametersOutputTypeDef,
     PipeTargetHttpParametersTypeDef,
-    PipeTargetKinesisStreamParametersOutputTypeDef,
     PipeTargetKinesisStreamParametersTypeDef,
-    PipeTargetLambdaFunctionParametersOutputTypeDef,
     PipeTargetLambdaFunctionParametersTypeDef,
     PipeTargetRedshiftDataParametersOutputTypeDef,
-    PipeTargetSqsQueueParametersOutputTypeDef,
-    PipeTargetStateMachineParametersOutputTypeDef,
-    PipeTargetRedshiftDataParametersTypeDef,
     PipeTargetSqsQueueParametersTypeDef,
     PipeTargetStateMachineParametersTypeDef,
-    SageMakerPipelineParameterOutputTypeDef,
+    PipeTargetRedshiftDataParametersTypeDef,
     SageMakerPipelineParameterTypeDef,
     StartPipeRequestRequestTypeDef,
     StopPipeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePipeSourceSqsQueueParametersTypeDef,
     NetworkConfigurationOutputTypeDef,
@@ -390,33 +364,29 @@
     BatchContainerOverridesTypeDef,
     CreatePipeResponseTypeDef,
     DeletePipeResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartPipeResponseTypeDef,
     StopPipeResponseTypeDef,
     UpdatePipeResponseTypeDef,
-    PipeSourceDynamoDBStreamParametersOutputTypeDef,
-    PipeSourceKinesisStreamParametersOutputTypeDef,
     PipeSourceDynamoDBStreamParametersTypeDef,
+    PipeSourceKinesisStreamParametersOutputTypeDef,
     PipeSourceKinesisStreamParametersTypeDef,
     UpdatePipeSourceDynamoDBStreamParametersTypeDef,
     UpdatePipeSourceKinesisStreamParametersTypeDef,
     EcsContainerOverrideOutputTypeDef,
     EcsContainerOverrideTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     ListPipesRequestListPipesPaginateTypeDef,
     ListPipesResponseTypeDef,
-    PipeSourceActiveMQBrokerParametersOutputTypeDef,
-    PipeSourceRabbitMQBrokerParametersOutputTypeDef,
     PipeSourceActiveMQBrokerParametersTypeDef,
     PipeSourceRabbitMQBrokerParametersTypeDef,
     UpdatePipeSourceActiveMQBrokerParametersTypeDef,
     UpdatePipeSourceRabbitMQBrokerParametersTypeDef,
-    PipeSourceManagedStreamingKafkaParametersOutputTypeDef,
     PipeSourceManagedStreamingKafkaParametersTypeDef,
     UpdatePipeSourceManagedStreamingKafkaParametersTypeDef,
     PipeEnrichmentParametersOutputTypeDef,
     PipeEnrichmentParametersTypeDef,
     PipeSourceSelfManagedKafkaParametersOutputTypeDef,
     PipeSourceSelfManagedKafkaParametersTypeDef,
     UpdatePipeSourceSelfManagedKafkaParametersTypeDef,
```

### Comparing `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/__init__.py` & `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/__init__.pyi` & `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/__main__.py` & `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridgePipes 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.EventBridgePipes 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes\nOther"
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

### Comparing `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/client.py` & `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/client.pyi` & `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/literals.py` & `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/literals.pyi` & `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/paginator.py` & `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/paginator.pyi` & `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/type_defs.py` & `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,82 +42,56 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
-    "BatchArrayPropertiesOutputTypeDef",
     "BatchArrayPropertiesTypeDef",
-    "BatchEnvironmentVariableOutputTypeDef",
-    "BatchResourceRequirementOutputTypeDef",
     "BatchEnvironmentVariableTypeDef",
     "BatchResourceRequirementTypeDef",
-    "BatchJobDependencyOutputTypeDef",
     "BatchJobDependencyTypeDef",
-    "BatchRetryStrategyOutputTypeDef",
     "BatchRetryStrategyTypeDef",
-    "CapacityProviderStrategyItemOutputTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "ResponseMetadataTypeDef",
-    "DeadLetterConfigOutputTypeDef",
     "DeadLetterConfigTypeDef",
     "DeletePipeRequestRequestTypeDef",
     "DescribePipeRequestRequestTypeDef",
-    "EcsEnvironmentFileOutputTypeDef",
-    "EcsEnvironmentVariableOutputTypeDef",
-    "EcsResourceRequirementOutputTypeDef",
     "EcsEnvironmentFileTypeDef",
     "EcsEnvironmentVariableTypeDef",
     "EcsResourceRequirementTypeDef",
-    "EcsEphemeralStorageOutputTypeDef",
     "EcsEphemeralStorageTypeDef",
-    "EcsInferenceAcceleratorOverrideOutputTypeDef",
     "EcsInferenceAcceleratorOverrideTypeDef",
-    "FilterOutputTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
     "ListPipesRequestRequestTypeDef",
     "PipeTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "MQBrokerAccessCredentialsOutputTypeDef",
     "MQBrokerAccessCredentialsTypeDef",
-    "MSKAccessCredentialsOutputTypeDef",
     "MSKAccessCredentialsTypeDef",
     "PipeEnrichmentHttpParametersOutputTypeDef",
     "PipeEnrichmentHttpParametersTypeDef",
-    "PipeSourceSqsQueueParametersOutputTypeDef",
     "PipeSourceSqsQueueParametersTypeDef",
-    "SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef",
-    "SelfManagedKafkaAccessConfigurationVpcOutputTypeDef",
     "SelfManagedKafkaAccessConfigurationCredentialsTypeDef",
+    "SelfManagedKafkaAccessConfigurationVpcOutputTypeDef",
     "SelfManagedKafkaAccessConfigurationVpcTypeDef",
-    "PipeTargetCloudWatchLogsParametersOutputTypeDef",
     "PipeTargetCloudWatchLogsParametersTypeDef",
-    "PlacementConstraintOutputTypeDef",
-    "PlacementStrategyOutputTypeDef",
-    "TagOutputTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "TagTypeDef",
     "PipeTargetEventBridgeEventBusParametersOutputTypeDef",
     "PipeTargetEventBridgeEventBusParametersTypeDef",
     "PipeTargetHttpParametersOutputTypeDef",
     "PipeTargetHttpParametersTypeDef",
-    "PipeTargetKinesisStreamParametersOutputTypeDef",
     "PipeTargetKinesisStreamParametersTypeDef",
-    "PipeTargetLambdaFunctionParametersOutputTypeDef",
     "PipeTargetLambdaFunctionParametersTypeDef",
     "PipeTargetRedshiftDataParametersOutputTypeDef",
-    "PipeTargetSqsQueueParametersOutputTypeDef",
-    "PipeTargetStateMachineParametersOutputTypeDef",
-    "PipeTargetRedshiftDataParametersTypeDef",
     "PipeTargetSqsQueueParametersTypeDef",
     "PipeTargetStateMachineParametersTypeDef",
-    "SageMakerPipelineParameterOutputTypeDef",
+    "PipeTargetRedshiftDataParametersTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "StartPipeRequestRequestTypeDef",
     "StopPipeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePipeSourceSqsQueueParametersTypeDef",
     "NetworkConfigurationOutputTypeDef",
@@ -126,33 +100,29 @@
     "BatchContainerOverridesTypeDef",
     "CreatePipeResponseTypeDef",
     "DeletePipeResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartPipeResponseTypeDef",
     "StopPipeResponseTypeDef",
     "UpdatePipeResponseTypeDef",
-    "PipeSourceDynamoDBStreamParametersOutputTypeDef",
-    "PipeSourceKinesisStreamParametersOutputTypeDef",
     "PipeSourceDynamoDBStreamParametersTypeDef",
+    "PipeSourceKinesisStreamParametersOutputTypeDef",
     "PipeSourceKinesisStreamParametersTypeDef",
     "UpdatePipeSourceDynamoDBStreamParametersTypeDef",
     "UpdatePipeSourceKinesisStreamParametersTypeDef",
     "EcsContainerOverrideOutputTypeDef",
     "EcsContainerOverrideTypeDef",
     "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "ListPipesRequestListPipesPaginateTypeDef",
     "ListPipesResponseTypeDef",
-    "PipeSourceActiveMQBrokerParametersOutputTypeDef",
-    "PipeSourceRabbitMQBrokerParametersOutputTypeDef",
     "PipeSourceActiveMQBrokerParametersTypeDef",
     "PipeSourceRabbitMQBrokerParametersTypeDef",
     "UpdatePipeSourceActiveMQBrokerParametersTypeDef",
     "UpdatePipeSourceRabbitMQBrokerParametersTypeDef",
-    "PipeSourceManagedStreamingKafkaParametersOutputTypeDef",
     "PipeSourceManagedStreamingKafkaParametersTypeDef",
     "UpdatePipeSourceManagedStreamingKafkaParametersTypeDef",
     "PipeEnrichmentParametersOutputTypeDef",
     "PipeEnrichmentParametersTypeDef",
     "PipeSourceSelfManagedKafkaParametersOutputTypeDef",
     "PipeSourceSelfManagedKafkaParametersTypeDef",
     "UpdatePipeSourceSelfManagedKafkaParametersTypeDef",
@@ -214,47 +184,22 @@
 
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
 
-BatchArrayPropertiesOutputTypeDef = TypedDict(
-    "BatchArrayPropertiesOutputTypeDef",
-    {
-        "Size": int,
-    },
-    total=False,
-)
-
 BatchArrayPropertiesTypeDef = TypedDict(
     "BatchArrayPropertiesTypeDef",
     {
         "Size": int,
     },
     total=False,
 )
 
-BatchEnvironmentVariableOutputTypeDef = TypedDict(
-    "BatchEnvironmentVariableOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-BatchResourceRequirementOutputTypeDef = TypedDict(
-    "BatchResourceRequirementOutputTypeDef",
-    {
-        "Type": BatchResourceRequirementTypeType,
-        "Value": str,
-    },
-)
-
 BatchEnvironmentVariableTypeDef = TypedDict(
     "BatchEnvironmentVariableTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -264,71 +209,31 @@
     "BatchResourceRequirementTypeDef",
     {
         "Type": BatchResourceRequirementTypeType,
         "Value": str,
     },
 )
 
-BatchJobDependencyOutputTypeDef = TypedDict(
-    "BatchJobDependencyOutputTypeDef",
-    {
-        "JobId": str,
-        "Type": BatchJobDependencyTypeType,
-    },
-    total=False,
-)
-
 BatchJobDependencyTypeDef = TypedDict(
     "BatchJobDependencyTypeDef",
     {
         "JobId": str,
         "Type": BatchJobDependencyTypeType,
     },
     total=False,
 )
 
-BatchRetryStrategyOutputTypeDef = TypedDict(
-    "BatchRetryStrategyOutputTypeDef",
-    {
-        "Attempts": int,
-    },
-    total=False,
-)
-
 BatchRetryStrategyTypeDef = TypedDict(
     "BatchRetryStrategyTypeDef",
     {
         "Attempts": int,
     },
     total=False,
 )
 
-_RequiredCapacityProviderStrategyItemOutputTypeDef = TypedDict(
-    "_RequiredCapacityProviderStrategyItemOutputTypeDef",
-    {
-        "capacityProvider": str,
-    },
-)
-_OptionalCapacityProviderStrategyItemOutputTypeDef = TypedDict(
-    "_OptionalCapacityProviderStrategyItemOutputTypeDef",
-    {
-        "base": int,
-        "weight": int,
-    },
-    total=False,
-)
-
-
-class CapacityProviderStrategyItemOutputTypeDef(
-    _RequiredCapacityProviderStrategyItemOutputTypeDef,
-    _OptionalCapacityProviderStrategyItemOutputTypeDef,
-):
-    pass
-
-
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -354,22 +259,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-DeadLetterConfigOutputTypeDef = TypedDict(
-    "DeadLetterConfigOutputTypeDef",
-    {
-        "Arn": str,
-    },
-    total=False,
-)
-
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
@@ -384,39 +281,14 @@
 DescribePipeRequestRequestTypeDef = TypedDict(
     "DescribePipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-EcsEnvironmentFileOutputTypeDef = TypedDict(
-    "EcsEnvironmentFileOutputTypeDef",
-    {
-        "type": Literal["s3"],
-        "value": str,
-    },
-)
-
-EcsEnvironmentVariableOutputTypeDef = TypedDict(
-    "EcsEnvironmentVariableOutputTypeDef",
-    {
-        "name": str,
-        "value": str,
-    },
-    total=False,
-)
-
-EcsResourceRequirementOutputTypeDef = TypedDict(
-    "EcsResourceRequirementOutputTypeDef",
-    {
-        "type": EcsResourceRequirementTypeType,
-        "value": str,
-    },
-)
-
 EcsEnvironmentFileTypeDef = TypedDict(
     "EcsEnvironmentFileTypeDef",
     {
         "type": Literal["s3"],
         "value": str,
     },
 )
@@ -434,54 +306,30 @@
     "EcsResourceRequirementTypeDef",
     {
         "type": EcsResourceRequirementTypeType,
         "value": str,
     },
 )
 
-EcsEphemeralStorageOutputTypeDef = TypedDict(
-    "EcsEphemeralStorageOutputTypeDef",
-    {
-        "sizeInGiB": int,
-    },
-)
-
 EcsEphemeralStorageTypeDef = TypedDict(
     "EcsEphemeralStorageTypeDef",
     {
         "sizeInGiB": int,
     },
 )
 
-EcsInferenceAcceleratorOverrideOutputTypeDef = TypedDict(
-    "EcsInferenceAcceleratorOverrideOutputTypeDef",
-    {
-        "deviceName": str,
-        "deviceType": str,
-    },
-    total=False,
-)
-
 EcsInferenceAcceleratorOverrideTypeDef = TypedDict(
     "EcsInferenceAcceleratorOverrideTypeDef",
     {
         "deviceName": str,
         "deviceType": str,
     },
     total=False,
 )
 
-FilterOutputTypeDef = TypedDict(
-    "FilterOutputTypeDef",
-    {
-        "Pattern": str,
-    },
-    total=False,
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Pattern": str,
     },
     total=False,
 )
@@ -530,39 +378,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-MQBrokerAccessCredentialsOutputTypeDef = TypedDict(
-    "MQBrokerAccessCredentialsOutputTypeDef",
-    {
-        "BasicAuth": str,
-    },
-    total=False,
-)
-
 MQBrokerAccessCredentialsTypeDef = TypedDict(
     "MQBrokerAccessCredentialsTypeDef",
     {
         "BasicAuth": str,
     },
     total=False,
 )
 
-MSKAccessCredentialsOutputTypeDef = TypedDict(
-    "MSKAccessCredentialsOutputTypeDef",
-    {
-        "ClientCertificateTlsAuth": str,
-        "SaslScram512Auth": str,
-    },
-    total=False,
-)
-
 MSKAccessCredentialsTypeDef = TypedDict(
     "MSKAccessCredentialsTypeDef",
     {
         "ClientCertificateTlsAuth": str,
         "SaslScram512Auth": str,
     },
     total=False,
@@ -584,34 +415,25 @@
         "HeaderParameters": Mapping[str, str],
         "PathParameterValues": Sequence[str],
         "QueryStringParameters": Mapping[str, str],
     },
     total=False,
 )
 
-PipeSourceSqsQueueParametersOutputTypeDef = TypedDict(
-    "PipeSourceSqsQueueParametersOutputTypeDef",
-    {
-        "BatchSize": int,
-        "MaximumBatchingWindowInSeconds": int,
-    },
-    total=False,
-)
-
 PipeSourceSqsQueueParametersTypeDef = TypedDict(
     "PipeSourceSqsQueueParametersTypeDef",
     {
         "BatchSize": int,
         "MaximumBatchingWindowInSeconds": int,
     },
     total=False,
 )
 
-SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef = TypedDict(
-    "SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef",
+SelfManagedKafkaAccessConfigurationCredentialsTypeDef = TypedDict(
+    "SelfManagedKafkaAccessConfigurationCredentialsTypeDef",
     {
         "BasicAuth": str,
         "ClientCertificateTlsAuth": str,
         "SaslScram256Auth": str,
         "SaslScram512Auth": str,
     },
     total=False,
@@ -622,78 +444,32 @@
     {
         "SecurityGroup": List[str],
         "Subnets": List[str],
     },
     total=False,
 )
 
-SelfManagedKafkaAccessConfigurationCredentialsTypeDef = TypedDict(
-    "SelfManagedKafkaAccessConfigurationCredentialsTypeDef",
-    {
-        "BasicAuth": str,
-        "ClientCertificateTlsAuth": str,
-        "SaslScram256Auth": str,
-        "SaslScram512Auth": str,
-    },
-    total=False,
-)
-
 SelfManagedKafkaAccessConfigurationVpcTypeDef = TypedDict(
     "SelfManagedKafkaAccessConfigurationVpcTypeDef",
     {
         "SecurityGroup": Sequence[str],
         "Subnets": Sequence[str],
     },
     total=False,
 )
 
-PipeTargetCloudWatchLogsParametersOutputTypeDef = TypedDict(
-    "PipeTargetCloudWatchLogsParametersOutputTypeDef",
-    {
-        "LogStreamName": str,
-        "Timestamp": str,
-    },
-    total=False,
-)
-
 PipeTargetCloudWatchLogsParametersTypeDef = TypedDict(
     "PipeTargetCloudWatchLogsParametersTypeDef",
     {
         "LogStreamName": str,
         "Timestamp": str,
     },
     total=False,
 )
 
-PlacementConstraintOutputTypeDef = TypedDict(
-    "PlacementConstraintOutputTypeDef",
-    {
-        "expression": str,
-        "type": PlacementConstraintTypeType,
-    },
-    total=False,
-)
-
-PlacementStrategyOutputTypeDef = TypedDict(
-    "PlacementStrategyOutputTypeDef",
-    {
-        "field": str,
-        "type": PlacementStrategyTypeType,
-    },
-    total=False,
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 PlacementConstraintTypeDef = TypedDict(
     "PlacementConstraintTypeDef",
     {
         "expression": str,
         "type": PlacementConstraintTypeType,
     },
     total=False,
@@ -756,36 +532,21 @@
         "HeaderParameters": Mapping[str, str],
         "PathParameterValues": Sequence[str],
         "QueryStringParameters": Mapping[str, str],
     },
     total=False,
 )
 
-PipeTargetKinesisStreamParametersOutputTypeDef = TypedDict(
-    "PipeTargetKinesisStreamParametersOutputTypeDef",
-    {
-        "PartitionKey": str,
-    },
-)
-
 PipeTargetKinesisStreamParametersTypeDef = TypedDict(
     "PipeTargetKinesisStreamParametersTypeDef",
     {
         "PartitionKey": str,
     },
 )
 
-PipeTargetLambdaFunctionParametersOutputTypeDef = TypedDict(
-    "PipeTargetLambdaFunctionParametersOutputTypeDef",
-    {
-        "InvocationType": PipeTargetInvocationTypeType,
-    },
-    total=False,
-)
-
 PipeTargetLambdaFunctionParametersTypeDef = TypedDict(
     "PipeTargetLambdaFunctionParametersTypeDef",
     {
         "InvocationType": PipeTargetInvocationTypeType,
     },
     total=False,
 )
@@ -812,25 +573,25 @@
 class PipeTargetRedshiftDataParametersOutputTypeDef(
     _RequiredPipeTargetRedshiftDataParametersOutputTypeDef,
     _OptionalPipeTargetRedshiftDataParametersOutputTypeDef,
 ):
     pass
 
 
-PipeTargetSqsQueueParametersOutputTypeDef = TypedDict(
-    "PipeTargetSqsQueueParametersOutputTypeDef",
+PipeTargetSqsQueueParametersTypeDef = TypedDict(
+    "PipeTargetSqsQueueParametersTypeDef",
     {
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
 )
 
-PipeTargetStateMachineParametersOutputTypeDef = TypedDict(
-    "PipeTargetStateMachineParametersOutputTypeDef",
+PipeTargetStateMachineParametersTypeDef = TypedDict(
+    "PipeTargetStateMachineParametersTypeDef",
     {
         "InvocationType": PipeTargetInvocationTypeType,
     },
     total=False,
 )
 
 _RequiredPipeTargetRedshiftDataParametersTypeDef = TypedDict(
@@ -855,39 +616,14 @@
 class PipeTargetRedshiftDataParametersTypeDef(
     _RequiredPipeTargetRedshiftDataParametersTypeDef,
     _OptionalPipeTargetRedshiftDataParametersTypeDef,
 ):
     pass
 
 
-PipeTargetSqsQueueParametersTypeDef = TypedDict(
-    "PipeTargetSqsQueueParametersTypeDef",
-    {
-        "MessageDeduplicationId": str,
-        "MessageGroupId": str,
-    },
-    total=False,
-)
-
-PipeTargetStateMachineParametersTypeDef = TypedDict(
-    "PipeTargetStateMachineParametersTypeDef",
-    {
-        "InvocationType": PipeTargetInvocationTypeType,
-    },
-    total=False,
-)
-
-SageMakerPipelineParameterOutputTypeDef = TypedDict(
-    "SageMakerPipelineParameterOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 SageMakerPipelineParameterTypeDef = TypedDict(
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -947,17 +683,17 @@
     total=False,
 )
 
 BatchContainerOverridesOutputTypeDef = TypedDict(
     "BatchContainerOverridesOutputTypeDef",
     {
         "Command": List[str],
-        "Environment": List[BatchEnvironmentVariableOutputTypeDef],
+        "Environment": List[BatchEnvironmentVariableTypeDef],
         "InstanceType": str,
-        "ResourceRequirements": List[BatchResourceRequirementOutputTypeDef],
+        "ResourceRequirements": List[BatchResourceRequirementTypeDef],
     },
     total=False,
 )
 
 BatchContainerOverridesTypeDef = TypedDict(
     "BatchContainerOverridesTypeDef",
     {
@@ -1038,53 +774,53 @@
         "DesiredState": RequestedPipeStateType,
         "LastModifiedTime": datetime,
         "Name": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPipeSourceDynamoDBStreamParametersOutputTypeDef = TypedDict(
-    "_RequiredPipeSourceDynamoDBStreamParametersOutputTypeDef",
+_RequiredPipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
+    "_RequiredPipeSourceDynamoDBStreamParametersTypeDef",
     {
         "StartingPosition": DynamoDBStreamStartPositionType,
     },
 )
-_OptionalPipeSourceDynamoDBStreamParametersOutputTypeDef = TypedDict(
-    "_OptionalPipeSourceDynamoDBStreamParametersOutputTypeDef",
+_OptionalPipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
+    "_OptionalPipeSourceDynamoDBStreamParametersTypeDef",
     {
         "BatchSize": int,
-        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
         "MaximumBatchingWindowInSeconds": int,
         "MaximumRecordAgeInSeconds": int,
         "MaximumRetryAttempts": int,
         "OnPartialBatchItemFailure": Literal["AUTOMATIC_BISECT"],
         "ParallelizationFactor": int,
     },
     total=False,
 )
 
 
-class PipeSourceDynamoDBStreamParametersOutputTypeDef(
-    _RequiredPipeSourceDynamoDBStreamParametersOutputTypeDef,
-    _OptionalPipeSourceDynamoDBStreamParametersOutputTypeDef,
+class PipeSourceDynamoDBStreamParametersTypeDef(
+    _RequiredPipeSourceDynamoDBStreamParametersTypeDef,
+    _OptionalPipeSourceDynamoDBStreamParametersTypeDef,
 ):
     pass
 
 
 _RequiredPipeSourceKinesisStreamParametersOutputTypeDef = TypedDict(
     "_RequiredPipeSourceKinesisStreamParametersOutputTypeDef",
     {
         "StartingPosition": KinesisStreamStartPositionType,
     },
 )
 _OptionalPipeSourceKinesisStreamParametersOutputTypeDef = TypedDict(
     "_OptionalPipeSourceKinesisStreamParametersOutputTypeDef",
     {
         "BatchSize": int,
-        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
         "MaximumBatchingWindowInSeconds": int,
         "MaximumRecordAgeInSeconds": int,
         "MaximumRetryAttempts": int,
         "OnPartialBatchItemFailure": Literal["AUTOMATIC_BISECT"],
         "ParallelizationFactor": int,
         "StartingPositionTimestamp": datetime,
     },
@@ -1095,42 +831,14 @@
 class PipeSourceKinesisStreamParametersOutputTypeDef(
     _RequiredPipeSourceKinesisStreamParametersOutputTypeDef,
     _OptionalPipeSourceKinesisStreamParametersOutputTypeDef,
 ):
     pass
 
 
-_RequiredPipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
-    "_RequiredPipeSourceDynamoDBStreamParametersTypeDef",
-    {
-        "StartingPosition": DynamoDBStreamStartPositionType,
-    },
-)
-_OptionalPipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
-    "_OptionalPipeSourceDynamoDBStreamParametersTypeDef",
-    {
-        "BatchSize": int,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "MaximumBatchingWindowInSeconds": int,
-        "MaximumRecordAgeInSeconds": int,
-        "MaximumRetryAttempts": int,
-        "OnPartialBatchItemFailure": Literal["AUTOMATIC_BISECT"],
-        "ParallelizationFactor": int,
-    },
-    total=False,
-)
-
-
-class PipeSourceDynamoDBStreamParametersTypeDef(
-    _RequiredPipeSourceDynamoDBStreamParametersTypeDef,
-    _OptionalPipeSourceDynamoDBStreamParametersTypeDef,
-):
-    pass
-
-
 _RequiredPipeSourceKinesisStreamParametersTypeDef = TypedDict(
     "_RequiredPipeSourceKinesisStreamParametersTypeDef",
     {
         "StartingPosition": KinesisStreamStartPositionType,
     },
 )
 _OptionalPipeSourceKinesisStreamParametersTypeDef = TypedDict(
@@ -1185,20 +893,20 @@
 )
 
 EcsContainerOverrideOutputTypeDef = TypedDict(
     "EcsContainerOverrideOutputTypeDef",
     {
         "Command": List[str],
         "Cpu": int,
-        "Environment": List[EcsEnvironmentVariableOutputTypeDef],
-        "EnvironmentFiles": List[EcsEnvironmentFileOutputTypeDef],
+        "Environment": List[EcsEnvironmentVariableTypeDef],
+        "EnvironmentFiles": List[EcsEnvironmentFileTypeDef],
         "Memory": int,
         "MemoryReservation": int,
         "Name": str,
-        "ResourceRequirements": List[EcsResourceRequirementOutputTypeDef],
+        "ResourceRequirements": List[EcsResourceRequirementTypeDef],
     },
     total=False,
 )
 
 EcsContainerOverrideTypeDef = TypedDict(
     "EcsContainerOverrideTypeDef",
     {
@@ -1213,15 +921,15 @@
     },
     total=False,
 )
 
 FilterCriteriaOutputTypeDef = TypedDict(
     "FilterCriteriaOutputTypeDef",
     {
-        "Filters": List[FilterOutputTypeDef],
+        "Filters": List[FilterTypeDef],
     },
     total=False,
 )
 
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
@@ -1248,63 +956,14 @@
     {
         "NextToken": str,
         "Pipes": List[PipeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPipeSourceActiveMQBrokerParametersOutputTypeDef = TypedDict(
-    "_RequiredPipeSourceActiveMQBrokerParametersOutputTypeDef",
-    {
-        "Credentials": MQBrokerAccessCredentialsOutputTypeDef,
-        "QueueName": str,
-    },
-)
-_OptionalPipeSourceActiveMQBrokerParametersOutputTypeDef = TypedDict(
-    "_OptionalPipeSourceActiveMQBrokerParametersOutputTypeDef",
-    {
-        "BatchSize": int,
-        "MaximumBatchingWindowInSeconds": int,
-    },
-    total=False,
-)
-
-
-class PipeSourceActiveMQBrokerParametersOutputTypeDef(
-    _RequiredPipeSourceActiveMQBrokerParametersOutputTypeDef,
-    _OptionalPipeSourceActiveMQBrokerParametersOutputTypeDef,
-):
-    pass
-
-
-_RequiredPipeSourceRabbitMQBrokerParametersOutputTypeDef = TypedDict(
-    "_RequiredPipeSourceRabbitMQBrokerParametersOutputTypeDef",
-    {
-        "Credentials": MQBrokerAccessCredentialsOutputTypeDef,
-        "QueueName": str,
-    },
-)
-_OptionalPipeSourceRabbitMQBrokerParametersOutputTypeDef = TypedDict(
-    "_OptionalPipeSourceRabbitMQBrokerParametersOutputTypeDef",
-    {
-        "BatchSize": int,
-        "MaximumBatchingWindowInSeconds": int,
-        "VirtualHost": str,
-    },
-    total=False,
-)
-
-
-class PipeSourceRabbitMQBrokerParametersOutputTypeDef(
-    _RequiredPipeSourceRabbitMQBrokerParametersOutputTypeDef,
-    _OptionalPipeSourceRabbitMQBrokerParametersOutputTypeDef,
-):
-    pass
-
-
 _RequiredPipeSourceActiveMQBrokerParametersTypeDef = TypedDict(
     "_RequiredPipeSourceActiveMQBrokerParametersTypeDef",
     {
         "Credentials": MQBrokerAccessCredentialsTypeDef,
         "QueueName": str,
     },
 )
@@ -1392,40 +1051,14 @@
 class UpdatePipeSourceRabbitMQBrokerParametersTypeDef(
     _RequiredUpdatePipeSourceRabbitMQBrokerParametersTypeDef,
     _OptionalUpdatePipeSourceRabbitMQBrokerParametersTypeDef,
 ):
     pass
 
 
-_RequiredPipeSourceManagedStreamingKafkaParametersOutputTypeDef = TypedDict(
-    "_RequiredPipeSourceManagedStreamingKafkaParametersOutputTypeDef",
-    {
-        "TopicName": str,
-    },
-)
-_OptionalPipeSourceManagedStreamingKafkaParametersOutputTypeDef = TypedDict(
-    "_OptionalPipeSourceManagedStreamingKafkaParametersOutputTypeDef",
-    {
-        "BatchSize": int,
-        "ConsumerGroupID": str,
-        "Credentials": MSKAccessCredentialsOutputTypeDef,
-        "MaximumBatchingWindowInSeconds": int,
-        "StartingPosition": MSKStartPositionType,
-    },
-    total=False,
-)
-
-
-class PipeSourceManagedStreamingKafkaParametersOutputTypeDef(
-    _RequiredPipeSourceManagedStreamingKafkaParametersOutputTypeDef,
-    _OptionalPipeSourceManagedStreamingKafkaParametersOutputTypeDef,
-):
-    pass
-
-
 _RequiredPipeSourceManagedStreamingKafkaParametersTypeDef = TypedDict(
     "_RequiredPipeSourceManagedStreamingKafkaParametersTypeDef",
     {
         "TopicName": str,
     },
 )
 _OptionalPipeSourceManagedStreamingKafkaParametersTypeDef = TypedDict(
@@ -1484,15 +1117,15 @@
 )
 _OptionalPipeSourceSelfManagedKafkaParametersOutputTypeDef = TypedDict(
     "_OptionalPipeSourceSelfManagedKafkaParametersOutputTypeDef",
     {
         "AdditionalBootstrapServers": List[str],
         "BatchSize": int,
         "ConsumerGroupID": str,
-        "Credentials": SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef,
+        "Credentials": SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
         "MaximumBatchingWindowInSeconds": int,
         "ServerRootCaCertificate": str,
         "StartingPosition": SelfManagedKafkaStartPositionType,
         "Vpc": SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     },
     total=False,
 )
@@ -1545,15 +1178,15 @@
     },
     total=False,
 )
 
 PipeTargetSageMakerPipelineParametersOutputTypeDef = TypedDict(
     "PipeTargetSageMakerPipelineParametersOutputTypeDef",
     {
-        "PipelineParameterList": List[SageMakerPipelineParameterOutputTypeDef],
+        "PipelineParameterList": List[SageMakerPipelineParameterTypeDef],
     },
     total=False,
 )
 
 PipeTargetSageMakerPipelineParametersTypeDef = TypedDict(
     "PipeTargetSageMakerPipelineParametersTypeDef",
     {
@@ -1568,19 +1201,19 @@
         "JobDefinition": str,
         "JobName": str,
     },
 )
 _OptionalPipeTargetBatchJobParametersOutputTypeDef = TypedDict(
     "_OptionalPipeTargetBatchJobParametersOutputTypeDef",
     {
-        "ArrayProperties": BatchArrayPropertiesOutputTypeDef,
+        "ArrayProperties": BatchArrayPropertiesTypeDef,
         "ContainerOverrides": BatchContainerOverridesOutputTypeDef,
-        "DependsOn": List[BatchJobDependencyOutputTypeDef],
+        "DependsOn": List[BatchJobDependencyTypeDef],
         "Parameters": Dict[str, str],
-        "RetryStrategy": BatchRetryStrategyOutputTypeDef,
+        "RetryStrategy": BatchRetryStrategyTypeDef,
     },
     total=False,
 )
 
 
 class PipeTargetBatchJobParametersOutputTypeDef(
     _RequiredPipeTargetBatchJobParametersOutputTypeDef,
@@ -1616,17 +1249,17 @@
 
 
 EcsTaskOverrideOutputTypeDef = TypedDict(
     "EcsTaskOverrideOutputTypeDef",
     {
         "ContainerOverrides": List[EcsContainerOverrideOutputTypeDef],
         "Cpu": str,
-        "EphemeralStorage": EcsEphemeralStorageOutputTypeDef,
+        "EphemeralStorage": EcsEphemeralStorageTypeDef,
         "ExecutionRoleArn": str,
-        "InferenceAcceleratorOverrides": List[EcsInferenceAcceleratorOverrideOutputTypeDef],
+        "InferenceAcceleratorOverrides": List[EcsInferenceAcceleratorOverrideTypeDef],
         "Memory": str,
         "TaskRoleArn": str,
     },
     total=False,
 )
 
 EcsTaskOverrideTypeDef = TypedDict(
@@ -1642,22 +1275,22 @@
     },
     total=False,
 )
 
 PipeSourceParametersOutputTypeDef = TypedDict(
     "PipeSourceParametersOutputTypeDef",
     {
-        "ActiveMQBrokerParameters": PipeSourceActiveMQBrokerParametersOutputTypeDef,
-        "DynamoDBStreamParameters": PipeSourceDynamoDBStreamParametersOutputTypeDef,
+        "ActiveMQBrokerParameters": PipeSourceActiveMQBrokerParametersTypeDef,
+        "DynamoDBStreamParameters": PipeSourceDynamoDBStreamParametersTypeDef,
         "FilterCriteria": FilterCriteriaOutputTypeDef,
         "KinesisStreamParameters": PipeSourceKinesisStreamParametersOutputTypeDef,
-        "ManagedStreamingKafkaParameters": PipeSourceManagedStreamingKafkaParametersOutputTypeDef,
-        "RabbitMQBrokerParameters": PipeSourceRabbitMQBrokerParametersOutputTypeDef,
+        "ManagedStreamingKafkaParameters": PipeSourceManagedStreamingKafkaParametersTypeDef,
+        "RabbitMQBrokerParameters": PipeSourceRabbitMQBrokerParametersTypeDef,
         "SelfManagedKafkaParameters": PipeSourceSelfManagedKafkaParametersOutputTypeDef,
-        "SqsQueueParameters": PipeSourceSqsQueueParametersOutputTypeDef,
+        "SqsQueueParameters": PipeSourceSqsQueueParametersTypeDef,
     },
     total=False,
 )
 
 PipeSourceParametersTypeDef = TypedDict(
     "PipeSourceParametersTypeDef",
     {
@@ -1693,27 +1326,27 @@
     {
         "TaskDefinitionArn": str,
     },
 )
 _OptionalPipeTargetEcsTaskParametersOutputTypeDef = TypedDict(
     "_OptionalPipeTargetEcsTaskParametersOutputTypeDef",
     {
-        "CapacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "CapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "EnableECSManagedTags": bool,
         "EnableExecuteCommand": bool,
         "Group": str,
         "LaunchType": LaunchTypeType,
         "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
         "Overrides": EcsTaskOverrideOutputTypeDef,
-        "PlacementConstraints": List[PlacementConstraintOutputTypeDef],
-        "PlacementStrategy": List[PlacementStrategyOutputTypeDef],
+        "PlacementConstraints": List[PlacementConstraintTypeDef],
+        "PlacementStrategy": List[PlacementStrategyTypeDef],
         "PlatformVersion": str,
         "PropagateTags": Literal["TASK_DEFINITION"],
         "ReferenceId": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "TaskCount": int,
     },
     total=False,
 )
 
 
 class PipeTargetEcsTaskParametersOutputTypeDef(
@@ -1757,25 +1390,25 @@
     pass
 
 
 PipeTargetParametersOutputTypeDef = TypedDict(
     "PipeTargetParametersOutputTypeDef",
     {
         "BatchJobParameters": PipeTargetBatchJobParametersOutputTypeDef,
-        "CloudWatchLogsParameters": PipeTargetCloudWatchLogsParametersOutputTypeDef,
+        "CloudWatchLogsParameters": PipeTargetCloudWatchLogsParametersTypeDef,
         "EcsTaskParameters": PipeTargetEcsTaskParametersOutputTypeDef,
         "EventBridgeEventBusParameters": PipeTargetEventBridgeEventBusParametersOutputTypeDef,
         "HttpParameters": PipeTargetHttpParametersOutputTypeDef,
         "InputTemplate": str,
-        "KinesisStreamParameters": PipeTargetKinesisStreamParametersOutputTypeDef,
-        "LambdaFunctionParameters": PipeTargetLambdaFunctionParametersOutputTypeDef,
+        "KinesisStreamParameters": PipeTargetKinesisStreamParametersTypeDef,
+        "LambdaFunctionParameters": PipeTargetLambdaFunctionParametersTypeDef,
         "RedshiftDataParameters": PipeTargetRedshiftDataParametersOutputTypeDef,
         "SageMakerPipelineParameters": PipeTargetSageMakerPipelineParametersOutputTypeDef,
-        "SqsQueueParameters": PipeTargetSqsQueueParametersOutputTypeDef,
-        "StepFunctionStateMachineParameters": PipeTargetStateMachineParametersOutputTypeDef,
+        "SqsQueueParameters": PipeTargetSqsQueueParametersTypeDef,
+        "StepFunctionStateMachineParameters": PipeTargetStateMachineParametersTypeDef,
     },
     total=False,
 )
 
 PipeTargetParametersTypeDef = TypedDict(
     "PipeTargetParametersTypeDef",
     {
```

### Comparing `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/type_defs.pyi` & `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -41,82 +41,56 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
-    "BatchArrayPropertiesOutputTypeDef",
     "BatchArrayPropertiesTypeDef",
-    "BatchEnvironmentVariableOutputTypeDef",
-    "BatchResourceRequirementOutputTypeDef",
     "BatchEnvironmentVariableTypeDef",
     "BatchResourceRequirementTypeDef",
-    "BatchJobDependencyOutputTypeDef",
     "BatchJobDependencyTypeDef",
-    "BatchRetryStrategyOutputTypeDef",
     "BatchRetryStrategyTypeDef",
-    "CapacityProviderStrategyItemOutputTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "ResponseMetadataTypeDef",
-    "DeadLetterConfigOutputTypeDef",
     "DeadLetterConfigTypeDef",
     "DeletePipeRequestRequestTypeDef",
     "DescribePipeRequestRequestTypeDef",
-    "EcsEnvironmentFileOutputTypeDef",
-    "EcsEnvironmentVariableOutputTypeDef",
-    "EcsResourceRequirementOutputTypeDef",
     "EcsEnvironmentFileTypeDef",
     "EcsEnvironmentVariableTypeDef",
     "EcsResourceRequirementTypeDef",
-    "EcsEphemeralStorageOutputTypeDef",
     "EcsEphemeralStorageTypeDef",
-    "EcsInferenceAcceleratorOverrideOutputTypeDef",
     "EcsInferenceAcceleratorOverrideTypeDef",
-    "FilterOutputTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
     "ListPipesRequestRequestTypeDef",
     "PipeTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "MQBrokerAccessCredentialsOutputTypeDef",
     "MQBrokerAccessCredentialsTypeDef",
-    "MSKAccessCredentialsOutputTypeDef",
     "MSKAccessCredentialsTypeDef",
     "PipeEnrichmentHttpParametersOutputTypeDef",
     "PipeEnrichmentHttpParametersTypeDef",
-    "PipeSourceSqsQueueParametersOutputTypeDef",
     "PipeSourceSqsQueueParametersTypeDef",
-    "SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef",
-    "SelfManagedKafkaAccessConfigurationVpcOutputTypeDef",
     "SelfManagedKafkaAccessConfigurationCredentialsTypeDef",
+    "SelfManagedKafkaAccessConfigurationVpcOutputTypeDef",
     "SelfManagedKafkaAccessConfigurationVpcTypeDef",
-    "PipeTargetCloudWatchLogsParametersOutputTypeDef",
     "PipeTargetCloudWatchLogsParametersTypeDef",
-    "PlacementConstraintOutputTypeDef",
-    "PlacementStrategyOutputTypeDef",
-    "TagOutputTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "TagTypeDef",
     "PipeTargetEventBridgeEventBusParametersOutputTypeDef",
     "PipeTargetEventBridgeEventBusParametersTypeDef",
     "PipeTargetHttpParametersOutputTypeDef",
     "PipeTargetHttpParametersTypeDef",
-    "PipeTargetKinesisStreamParametersOutputTypeDef",
     "PipeTargetKinesisStreamParametersTypeDef",
-    "PipeTargetLambdaFunctionParametersOutputTypeDef",
     "PipeTargetLambdaFunctionParametersTypeDef",
     "PipeTargetRedshiftDataParametersOutputTypeDef",
-    "PipeTargetSqsQueueParametersOutputTypeDef",
-    "PipeTargetStateMachineParametersOutputTypeDef",
-    "PipeTargetRedshiftDataParametersTypeDef",
     "PipeTargetSqsQueueParametersTypeDef",
     "PipeTargetStateMachineParametersTypeDef",
-    "SageMakerPipelineParameterOutputTypeDef",
+    "PipeTargetRedshiftDataParametersTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "StartPipeRequestRequestTypeDef",
     "StopPipeRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePipeSourceSqsQueueParametersTypeDef",
     "NetworkConfigurationOutputTypeDef",
@@ -125,33 +99,29 @@
     "BatchContainerOverridesTypeDef",
     "CreatePipeResponseTypeDef",
     "DeletePipeResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartPipeResponseTypeDef",
     "StopPipeResponseTypeDef",
     "UpdatePipeResponseTypeDef",
-    "PipeSourceDynamoDBStreamParametersOutputTypeDef",
-    "PipeSourceKinesisStreamParametersOutputTypeDef",
     "PipeSourceDynamoDBStreamParametersTypeDef",
+    "PipeSourceKinesisStreamParametersOutputTypeDef",
     "PipeSourceKinesisStreamParametersTypeDef",
     "UpdatePipeSourceDynamoDBStreamParametersTypeDef",
     "UpdatePipeSourceKinesisStreamParametersTypeDef",
     "EcsContainerOverrideOutputTypeDef",
     "EcsContainerOverrideTypeDef",
     "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "ListPipesRequestListPipesPaginateTypeDef",
     "ListPipesResponseTypeDef",
-    "PipeSourceActiveMQBrokerParametersOutputTypeDef",
-    "PipeSourceRabbitMQBrokerParametersOutputTypeDef",
     "PipeSourceActiveMQBrokerParametersTypeDef",
     "PipeSourceRabbitMQBrokerParametersTypeDef",
     "UpdatePipeSourceActiveMQBrokerParametersTypeDef",
     "UpdatePipeSourceRabbitMQBrokerParametersTypeDef",
-    "PipeSourceManagedStreamingKafkaParametersOutputTypeDef",
     "PipeSourceManagedStreamingKafkaParametersTypeDef",
     "UpdatePipeSourceManagedStreamingKafkaParametersTypeDef",
     "PipeEnrichmentParametersOutputTypeDef",
     "PipeEnrichmentParametersTypeDef",
     "PipeSourceSelfManagedKafkaParametersOutputTypeDef",
     "PipeSourceSelfManagedKafkaParametersTypeDef",
     "UpdatePipeSourceSelfManagedKafkaParametersTypeDef",
@@ -209,47 +179,22 @@
 )
 
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
-BatchArrayPropertiesOutputTypeDef = TypedDict(
-    "BatchArrayPropertiesOutputTypeDef",
-    {
-        "Size": int,
-    },
-    total=False,
-)
-
 BatchArrayPropertiesTypeDef = TypedDict(
     "BatchArrayPropertiesTypeDef",
     {
         "Size": int,
     },
     total=False,
 )
 
-BatchEnvironmentVariableOutputTypeDef = TypedDict(
-    "BatchEnvironmentVariableOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-BatchResourceRequirementOutputTypeDef = TypedDict(
-    "BatchResourceRequirementOutputTypeDef",
-    {
-        "Type": BatchResourceRequirementTypeType,
-        "Value": str,
-    },
-)
-
 BatchEnvironmentVariableTypeDef = TypedDict(
     "BatchEnvironmentVariableTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -259,69 +204,31 @@
     "BatchResourceRequirementTypeDef",
     {
         "Type": BatchResourceRequirementTypeType,
         "Value": str,
     },
 )
 
-BatchJobDependencyOutputTypeDef = TypedDict(
-    "BatchJobDependencyOutputTypeDef",
-    {
-        "JobId": str,
-        "Type": BatchJobDependencyTypeType,
-    },
-    total=False,
-)
-
 BatchJobDependencyTypeDef = TypedDict(
     "BatchJobDependencyTypeDef",
     {
         "JobId": str,
         "Type": BatchJobDependencyTypeType,
     },
     total=False,
 )
 
-BatchRetryStrategyOutputTypeDef = TypedDict(
-    "BatchRetryStrategyOutputTypeDef",
-    {
-        "Attempts": int,
-    },
-    total=False,
-)
-
 BatchRetryStrategyTypeDef = TypedDict(
     "BatchRetryStrategyTypeDef",
     {
         "Attempts": int,
     },
     total=False,
 )
 
-_RequiredCapacityProviderStrategyItemOutputTypeDef = TypedDict(
-    "_RequiredCapacityProviderStrategyItemOutputTypeDef",
-    {
-        "capacityProvider": str,
-    },
-)
-_OptionalCapacityProviderStrategyItemOutputTypeDef = TypedDict(
-    "_OptionalCapacityProviderStrategyItemOutputTypeDef",
-    {
-        "base": int,
-        "weight": int,
-    },
-    total=False,
-)
-
-class CapacityProviderStrategyItemOutputTypeDef(
-    _RequiredCapacityProviderStrategyItemOutputTypeDef,
-    _OptionalCapacityProviderStrategyItemOutputTypeDef,
-):
-    pass
-
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -345,22 +252,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-DeadLetterConfigOutputTypeDef = TypedDict(
-    "DeadLetterConfigOutputTypeDef",
-    {
-        "Arn": str,
-    },
-    total=False,
-)
-
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
@@ -375,39 +274,14 @@
 DescribePipeRequestRequestTypeDef = TypedDict(
     "DescribePipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-EcsEnvironmentFileOutputTypeDef = TypedDict(
-    "EcsEnvironmentFileOutputTypeDef",
-    {
-        "type": Literal["s3"],
-        "value": str,
-    },
-)
-
-EcsEnvironmentVariableOutputTypeDef = TypedDict(
-    "EcsEnvironmentVariableOutputTypeDef",
-    {
-        "name": str,
-        "value": str,
-    },
-    total=False,
-)
-
-EcsResourceRequirementOutputTypeDef = TypedDict(
-    "EcsResourceRequirementOutputTypeDef",
-    {
-        "type": EcsResourceRequirementTypeType,
-        "value": str,
-    },
-)
-
 EcsEnvironmentFileTypeDef = TypedDict(
     "EcsEnvironmentFileTypeDef",
     {
         "type": Literal["s3"],
         "value": str,
     },
 )
@@ -425,54 +299,30 @@
     "EcsResourceRequirementTypeDef",
     {
         "type": EcsResourceRequirementTypeType,
         "value": str,
     },
 )
 
-EcsEphemeralStorageOutputTypeDef = TypedDict(
-    "EcsEphemeralStorageOutputTypeDef",
-    {
-        "sizeInGiB": int,
-    },
-)
-
 EcsEphemeralStorageTypeDef = TypedDict(
     "EcsEphemeralStorageTypeDef",
     {
         "sizeInGiB": int,
     },
 )
 
-EcsInferenceAcceleratorOverrideOutputTypeDef = TypedDict(
-    "EcsInferenceAcceleratorOverrideOutputTypeDef",
-    {
-        "deviceName": str,
-        "deviceType": str,
-    },
-    total=False,
-)
-
 EcsInferenceAcceleratorOverrideTypeDef = TypedDict(
     "EcsInferenceAcceleratorOverrideTypeDef",
     {
         "deviceName": str,
         "deviceType": str,
     },
     total=False,
 )
 
-FilterOutputTypeDef = TypedDict(
-    "FilterOutputTypeDef",
-    {
-        "Pattern": str,
-    },
-    total=False,
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Pattern": str,
     },
     total=False,
 )
@@ -521,39 +371,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-MQBrokerAccessCredentialsOutputTypeDef = TypedDict(
-    "MQBrokerAccessCredentialsOutputTypeDef",
-    {
-        "BasicAuth": str,
-    },
-    total=False,
-)
-
 MQBrokerAccessCredentialsTypeDef = TypedDict(
     "MQBrokerAccessCredentialsTypeDef",
     {
         "BasicAuth": str,
     },
     total=False,
 )
 
-MSKAccessCredentialsOutputTypeDef = TypedDict(
-    "MSKAccessCredentialsOutputTypeDef",
-    {
-        "ClientCertificateTlsAuth": str,
-        "SaslScram512Auth": str,
-    },
-    total=False,
-)
-
 MSKAccessCredentialsTypeDef = TypedDict(
     "MSKAccessCredentialsTypeDef",
     {
         "ClientCertificateTlsAuth": str,
         "SaslScram512Auth": str,
     },
     total=False,
@@ -575,34 +408,25 @@
         "HeaderParameters": Mapping[str, str],
         "PathParameterValues": Sequence[str],
         "QueryStringParameters": Mapping[str, str],
     },
     total=False,
 )
 
-PipeSourceSqsQueueParametersOutputTypeDef = TypedDict(
-    "PipeSourceSqsQueueParametersOutputTypeDef",
-    {
-        "BatchSize": int,
-        "MaximumBatchingWindowInSeconds": int,
-    },
-    total=False,
-)
-
 PipeSourceSqsQueueParametersTypeDef = TypedDict(
     "PipeSourceSqsQueueParametersTypeDef",
     {
         "BatchSize": int,
         "MaximumBatchingWindowInSeconds": int,
     },
     total=False,
 )
 
-SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef = TypedDict(
-    "SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef",
+SelfManagedKafkaAccessConfigurationCredentialsTypeDef = TypedDict(
+    "SelfManagedKafkaAccessConfigurationCredentialsTypeDef",
     {
         "BasicAuth": str,
         "ClientCertificateTlsAuth": str,
         "SaslScram256Auth": str,
         "SaslScram512Auth": str,
     },
     total=False,
@@ -613,78 +437,32 @@
     {
         "SecurityGroup": List[str],
         "Subnets": List[str],
     },
     total=False,
 )
 
-SelfManagedKafkaAccessConfigurationCredentialsTypeDef = TypedDict(
-    "SelfManagedKafkaAccessConfigurationCredentialsTypeDef",
-    {
-        "BasicAuth": str,
-        "ClientCertificateTlsAuth": str,
-        "SaslScram256Auth": str,
-        "SaslScram512Auth": str,
-    },
-    total=False,
-)
-
 SelfManagedKafkaAccessConfigurationVpcTypeDef = TypedDict(
     "SelfManagedKafkaAccessConfigurationVpcTypeDef",
     {
         "SecurityGroup": Sequence[str],
         "Subnets": Sequence[str],
     },
     total=False,
 )
 
-PipeTargetCloudWatchLogsParametersOutputTypeDef = TypedDict(
-    "PipeTargetCloudWatchLogsParametersOutputTypeDef",
-    {
-        "LogStreamName": str,
-        "Timestamp": str,
-    },
-    total=False,
-)
-
 PipeTargetCloudWatchLogsParametersTypeDef = TypedDict(
     "PipeTargetCloudWatchLogsParametersTypeDef",
     {
         "LogStreamName": str,
         "Timestamp": str,
     },
     total=False,
 )
 
-PlacementConstraintOutputTypeDef = TypedDict(
-    "PlacementConstraintOutputTypeDef",
-    {
-        "expression": str,
-        "type": PlacementConstraintTypeType,
-    },
-    total=False,
-)
-
-PlacementStrategyOutputTypeDef = TypedDict(
-    "PlacementStrategyOutputTypeDef",
-    {
-        "field": str,
-        "type": PlacementStrategyTypeType,
-    },
-    total=False,
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 PlacementConstraintTypeDef = TypedDict(
     "PlacementConstraintTypeDef",
     {
         "expression": str,
         "type": PlacementConstraintTypeType,
     },
     total=False,
@@ -747,36 +525,21 @@
         "HeaderParameters": Mapping[str, str],
         "PathParameterValues": Sequence[str],
         "QueryStringParameters": Mapping[str, str],
     },
     total=False,
 )
 
-PipeTargetKinesisStreamParametersOutputTypeDef = TypedDict(
-    "PipeTargetKinesisStreamParametersOutputTypeDef",
-    {
-        "PartitionKey": str,
-    },
-)
-
 PipeTargetKinesisStreamParametersTypeDef = TypedDict(
     "PipeTargetKinesisStreamParametersTypeDef",
     {
         "PartitionKey": str,
     },
 )
 
-PipeTargetLambdaFunctionParametersOutputTypeDef = TypedDict(
-    "PipeTargetLambdaFunctionParametersOutputTypeDef",
-    {
-        "InvocationType": PipeTargetInvocationTypeType,
-    },
-    total=False,
-)
-
 PipeTargetLambdaFunctionParametersTypeDef = TypedDict(
     "PipeTargetLambdaFunctionParametersTypeDef",
     {
         "InvocationType": PipeTargetInvocationTypeType,
     },
     total=False,
 )
@@ -801,25 +564,25 @@
 
 class PipeTargetRedshiftDataParametersOutputTypeDef(
     _RequiredPipeTargetRedshiftDataParametersOutputTypeDef,
     _OptionalPipeTargetRedshiftDataParametersOutputTypeDef,
 ):
     pass
 
-PipeTargetSqsQueueParametersOutputTypeDef = TypedDict(
-    "PipeTargetSqsQueueParametersOutputTypeDef",
+PipeTargetSqsQueueParametersTypeDef = TypedDict(
+    "PipeTargetSqsQueueParametersTypeDef",
     {
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
 )
 
-PipeTargetStateMachineParametersOutputTypeDef = TypedDict(
-    "PipeTargetStateMachineParametersOutputTypeDef",
+PipeTargetStateMachineParametersTypeDef = TypedDict(
+    "PipeTargetStateMachineParametersTypeDef",
     {
         "InvocationType": PipeTargetInvocationTypeType,
     },
     total=False,
 )
 
 _RequiredPipeTargetRedshiftDataParametersTypeDef = TypedDict(
@@ -842,39 +605,14 @@
 
 class PipeTargetRedshiftDataParametersTypeDef(
     _RequiredPipeTargetRedshiftDataParametersTypeDef,
     _OptionalPipeTargetRedshiftDataParametersTypeDef,
 ):
     pass
 
-PipeTargetSqsQueueParametersTypeDef = TypedDict(
-    "PipeTargetSqsQueueParametersTypeDef",
-    {
-        "MessageDeduplicationId": str,
-        "MessageGroupId": str,
-    },
-    total=False,
-)
-
-PipeTargetStateMachineParametersTypeDef = TypedDict(
-    "PipeTargetStateMachineParametersTypeDef",
-    {
-        "InvocationType": PipeTargetInvocationTypeType,
-    },
-    total=False,
-)
-
-SageMakerPipelineParameterOutputTypeDef = TypedDict(
-    "SageMakerPipelineParameterOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-)
-
 SageMakerPipelineParameterTypeDef = TypedDict(
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -934,17 +672,17 @@
     total=False,
 )
 
 BatchContainerOverridesOutputTypeDef = TypedDict(
     "BatchContainerOverridesOutputTypeDef",
     {
         "Command": List[str],
-        "Environment": List[BatchEnvironmentVariableOutputTypeDef],
+        "Environment": List[BatchEnvironmentVariableTypeDef],
         "InstanceType": str,
-        "ResourceRequirements": List[BatchResourceRequirementOutputTypeDef],
+        "ResourceRequirements": List[BatchResourceRequirementTypeDef],
     },
     total=False,
 )
 
 BatchContainerOverridesTypeDef = TypedDict(
     "BatchContainerOverridesTypeDef",
     {
@@ -1025,51 +763,51 @@
         "DesiredState": RequestedPipeStateType,
         "LastModifiedTime": datetime,
         "Name": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPipeSourceDynamoDBStreamParametersOutputTypeDef = TypedDict(
-    "_RequiredPipeSourceDynamoDBStreamParametersOutputTypeDef",
+_RequiredPipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
+    "_RequiredPipeSourceDynamoDBStreamParametersTypeDef",
     {
         "StartingPosition": DynamoDBStreamStartPositionType,
     },
 )
-_OptionalPipeSourceDynamoDBStreamParametersOutputTypeDef = TypedDict(
-    "_OptionalPipeSourceDynamoDBStreamParametersOutputTypeDef",
+_OptionalPipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
+    "_OptionalPipeSourceDynamoDBStreamParametersTypeDef",
     {
         "BatchSize": int,
-        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
         "MaximumBatchingWindowInSeconds": int,
         "MaximumRecordAgeInSeconds": int,
         "MaximumRetryAttempts": int,
         "OnPartialBatchItemFailure": Literal["AUTOMATIC_BISECT"],
         "ParallelizationFactor": int,
     },
     total=False,
 )
 
-class PipeSourceDynamoDBStreamParametersOutputTypeDef(
-    _RequiredPipeSourceDynamoDBStreamParametersOutputTypeDef,
-    _OptionalPipeSourceDynamoDBStreamParametersOutputTypeDef,
+class PipeSourceDynamoDBStreamParametersTypeDef(
+    _RequiredPipeSourceDynamoDBStreamParametersTypeDef,
+    _OptionalPipeSourceDynamoDBStreamParametersTypeDef,
 ):
     pass
 
 _RequiredPipeSourceKinesisStreamParametersOutputTypeDef = TypedDict(
     "_RequiredPipeSourceKinesisStreamParametersOutputTypeDef",
     {
         "StartingPosition": KinesisStreamStartPositionType,
     },
 )
 _OptionalPipeSourceKinesisStreamParametersOutputTypeDef = TypedDict(
     "_OptionalPipeSourceKinesisStreamParametersOutputTypeDef",
     {
         "BatchSize": int,
-        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
         "MaximumBatchingWindowInSeconds": int,
         "MaximumRecordAgeInSeconds": int,
         "MaximumRetryAttempts": int,
         "OnPartialBatchItemFailure": Literal["AUTOMATIC_BISECT"],
         "ParallelizationFactor": int,
         "StartingPositionTimestamp": datetime,
     },
@@ -1078,40 +816,14 @@
 
 class PipeSourceKinesisStreamParametersOutputTypeDef(
     _RequiredPipeSourceKinesisStreamParametersOutputTypeDef,
     _OptionalPipeSourceKinesisStreamParametersOutputTypeDef,
 ):
     pass
 
-_RequiredPipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
-    "_RequiredPipeSourceDynamoDBStreamParametersTypeDef",
-    {
-        "StartingPosition": DynamoDBStreamStartPositionType,
-    },
-)
-_OptionalPipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
-    "_OptionalPipeSourceDynamoDBStreamParametersTypeDef",
-    {
-        "BatchSize": int,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "MaximumBatchingWindowInSeconds": int,
-        "MaximumRecordAgeInSeconds": int,
-        "MaximumRetryAttempts": int,
-        "OnPartialBatchItemFailure": Literal["AUTOMATIC_BISECT"],
-        "ParallelizationFactor": int,
-    },
-    total=False,
-)
-
-class PipeSourceDynamoDBStreamParametersTypeDef(
-    _RequiredPipeSourceDynamoDBStreamParametersTypeDef,
-    _OptionalPipeSourceDynamoDBStreamParametersTypeDef,
-):
-    pass
-
 _RequiredPipeSourceKinesisStreamParametersTypeDef = TypedDict(
     "_RequiredPipeSourceKinesisStreamParametersTypeDef",
     {
         "StartingPosition": KinesisStreamStartPositionType,
     },
 )
 _OptionalPipeSourceKinesisStreamParametersTypeDef = TypedDict(
@@ -1164,20 +876,20 @@
 )
 
 EcsContainerOverrideOutputTypeDef = TypedDict(
     "EcsContainerOverrideOutputTypeDef",
     {
         "Command": List[str],
         "Cpu": int,
-        "Environment": List[EcsEnvironmentVariableOutputTypeDef],
-        "EnvironmentFiles": List[EcsEnvironmentFileOutputTypeDef],
+        "Environment": List[EcsEnvironmentVariableTypeDef],
+        "EnvironmentFiles": List[EcsEnvironmentFileTypeDef],
         "Memory": int,
         "MemoryReservation": int,
         "Name": str,
-        "ResourceRequirements": List[EcsResourceRequirementOutputTypeDef],
+        "ResourceRequirements": List[EcsResourceRequirementTypeDef],
     },
     total=False,
 )
 
 EcsContainerOverrideTypeDef = TypedDict(
     "EcsContainerOverrideTypeDef",
     {
@@ -1192,15 +904,15 @@
     },
     total=False,
 )
 
 FilterCriteriaOutputTypeDef = TypedDict(
     "FilterCriteriaOutputTypeDef",
     {
-        "Filters": List[FilterOutputTypeDef],
+        "Filters": List[FilterTypeDef],
     },
     total=False,
 )
 
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
@@ -1227,59 +939,14 @@
     {
         "NextToken": str,
         "Pipes": List[PipeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPipeSourceActiveMQBrokerParametersOutputTypeDef = TypedDict(
-    "_RequiredPipeSourceActiveMQBrokerParametersOutputTypeDef",
-    {
-        "Credentials": MQBrokerAccessCredentialsOutputTypeDef,
-        "QueueName": str,
-    },
-)
-_OptionalPipeSourceActiveMQBrokerParametersOutputTypeDef = TypedDict(
-    "_OptionalPipeSourceActiveMQBrokerParametersOutputTypeDef",
-    {
-        "BatchSize": int,
-        "MaximumBatchingWindowInSeconds": int,
-    },
-    total=False,
-)
-
-class PipeSourceActiveMQBrokerParametersOutputTypeDef(
-    _RequiredPipeSourceActiveMQBrokerParametersOutputTypeDef,
-    _OptionalPipeSourceActiveMQBrokerParametersOutputTypeDef,
-):
-    pass
-
-_RequiredPipeSourceRabbitMQBrokerParametersOutputTypeDef = TypedDict(
-    "_RequiredPipeSourceRabbitMQBrokerParametersOutputTypeDef",
-    {
-        "Credentials": MQBrokerAccessCredentialsOutputTypeDef,
-        "QueueName": str,
-    },
-)
-_OptionalPipeSourceRabbitMQBrokerParametersOutputTypeDef = TypedDict(
-    "_OptionalPipeSourceRabbitMQBrokerParametersOutputTypeDef",
-    {
-        "BatchSize": int,
-        "MaximumBatchingWindowInSeconds": int,
-        "VirtualHost": str,
-    },
-    total=False,
-)
-
-class PipeSourceRabbitMQBrokerParametersOutputTypeDef(
-    _RequiredPipeSourceRabbitMQBrokerParametersOutputTypeDef,
-    _OptionalPipeSourceRabbitMQBrokerParametersOutputTypeDef,
-):
-    pass
-
 _RequiredPipeSourceActiveMQBrokerParametersTypeDef = TypedDict(
     "_RequiredPipeSourceActiveMQBrokerParametersTypeDef",
     {
         "Credentials": MQBrokerAccessCredentialsTypeDef,
         "QueueName": str,
     },
 )
@@ -1359,38 +1026,14 @@
 
 class UpdatePipeSourceRabbitMQBrokerParametersTypeDef(
     _RequiredUpdatePipeSourceRabbitMQBrokerParametersTypeDef,
     _OptionalUpdatePipeSourceRabbitMQBrokerParametersTypeDef,
 ):
     pass
 
-_RequiredPipeSourceManagedStreamingKafkaParametersOutputTypeDef = TypedDict(
-    "_RequiredPipeSourceManagedStreamingKafkaParametersOutputTypeDef",
-    {
-        "TopicName": str,
-    },
-)
-_OptionalPipeSourceManagedStreamingKafkaParametersOutputTypeDef = TypedDict(
-    "_OptionalPipeSourceManagedStreamingKafkaParametersOutputTypeDef",
-    {
-        "BatchSize": int,
-        "ConsumerGroupID": str,
-        "Credentials": MSKAccessCredentialsOutputTypeDef,
-        "MaximumBatchingWindowInSeconds": int,
-        "StartingPosition": MSKStartPositionType,
-    },
-    total=False,
-)
-
-class PipeSourceManagedStreamingKafkaParametersOutputTypeDef(
-    _RequiredPipeSourceManagedStreamingKafkaParametersOutputTypeDef,
-    _OptionalPipeSourceManagedStreamingKafkaParametersOutputTypeDef,
-):
-    pass
-
 _RequiredPipeSourceManagedStreamingKafkaParametersTypeDef = TypedDict(
     "_RequiredPipeSourceManagedStreamingKafkaParametersTypeDef",
     {
         "TopicName": str,
     },
 )
 _OptionalPipeSourceManagedStreamingKafkaParametersTypeDef = TypedDict(
@@ -1447,15 +1090,15 @@
 )
 _OptionalPipeSourceSelfManagedKafkaParametersOutputTypeDef = TypedDict(
     "_OptionalPipeSourceSelfManagedKafkaParametersOutputTypeDef",
     {
         "AdditionalBootstrapServers": List[str],
         "BatchSize": int,
         "ConsumerGroupID": str,
-        "Credentials": SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef,
+        "Credentials": SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
         "MaximumBatchingWindowInSeconds": int,
         "ServerRootCaCertificate": str,
         "StartingPosition": SelfManagedKafkaStartPositionType,
         "Vpc": SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     },
     total=False,
 )
@@ -1504,15 +1147,15 @@
     },
     total=False,
 )
 
 PipeTargetSageMakerPipelineParametersOutputTypeDef = TypedDict(
     "PipeTargetSageMakerPipelineParametersOutputTypeDef",
     {
-        "PipelineParameterList": List[SageMakerPipelineParameterOutputTypeDef],
+        "PipelineParameterList": List[SageMakerPipelineParameterTypeDef],
     },
     total=False,
 )
 
 PipeTargetSageMakerPipelineParametersTypeDef = TypedDict(
     "PipeTargetSageMakerPipelineParametersTypeDef",
     {
@@ -1527,19 +1170,19 @@
         "JobDefinition": str,
         "JobName": str,
     },
 )
 _OptionalPipeTargetBatchJobParametersOutputTypeDef = TypedDict(
     "_OptionalPipeTargetBatchJobParametersOutputTypeDef",
     {
-        "ArrayProperties": BatchArrayPropertiesOutputTypeDef,
+        "ArrayProperties": BatchArrayPropertiesTypeDef,
         "ContainerOverrides": BatchContainerOverridesOutputTypeDef,
-        "DependsOn": List[BatchJobDependencyOutputTypeDef],
+        "DependsOn": List[BatchJobDependencyTypeDef],
         "Parameters": Dict[str, str],
-        "RetryStrategy": BatchRetryStrategyOutputTypeDef,
+        "RetryStrategy": BatchRetryStrategyTypeDef,
     },
     total=False,
 )
 
 class PipeTargetBatchJobParametersOutputTypeDef(
     _RequiredPipeTargetBatchJobParametersOutputTypeDef,
     _OptionalPipeTargetBatchJobParametersOutputTypeDef,
@@ -1571,17 +1214,17 @@
     pass
 
 EcsTaskOverrideOutputTypeDef = TypedDict(
     "EcsTaskOverrideOutputTypeDef",
     {
         "ContainerOverrides": List[EcsContainerOverrideOutputTypeDef],
         "Cpu": str,
-        "EphemeralStorage": EcsEphemeralStorageOutputTypeDef,
+        "EphemeralStorage": EcsEphemeralStorageTypeDef,
         "ExecutionRoleArn": str,
-        "InferenceAcceleratorOverrides": List[EcsInferenceAcceleratorOverrideOutputTypeDef],
+        "InferenceAcceleratorOverrides": List[EcsInferenceAcceleratorOverrideTypeDef],
         "Memory": str,
         "TaskRoleArn": str,
     },
     total=False,
 )
 
 EcsTaskOverrideTypeDef = TypedDict(
@@ -1597,22 +1240,22 @@
     },
     total=False,
 )
 
 PipeSourceParametersOutputTypeDef = TypedDict(
     "PipeSourceParametersOutputTypeDef",
     {
-        "ActiveMQBrokerParameters": PipeSourceActiveMQBrokerParametersOutputTypeDef,
-        "DynamoDBStreamParameters": PipeSourceDynamoDBStreamParametersOutputTypeDef,
+        "ActiveMQBrokerParameters": PipeSourceActiveMQBrokerParametersTypeDef,
+        "DynamoDBStreamParameters": PipeSourceDynamoDBStreamParametersTypeDef,
         "FilterCriteria": FilterCriteriaOutputTypeDef,
         "KinesisStreamParameters": PipeSourceKinesisStreamParametersOutputTypeDef,
-        "ManagedStreamingKafkaParameters": PipeSourceManagedStreamingKafkaParametersOutputTypeDef,
-        "RabbitMQBrokerParameters": PipeSourceRabbitMQBrokerParametersOutputTypeDef,
+        "ManagedStreamingKafkaParameters": PipeSourceManagedStreamingKafkaParametersTypeDef,
+        "RabbitMQBrokerParameters": PipeSourceRabbitMQBrokerParametersTypeDef,
         "SelfManagedKafkaParameters": PipeSourceSelfManagedKafkaParametersOutputTypeDef,
-        "SqsQueueParameters": PipeSourceSqsQueueParametersOutputTypeDef,
+        "SqsQueueParameters": PipeSourceSqsQueueParametersTypeDef,
     },
     total=False,
 )
 
 PipeSourceParametersTypeDef = TypedDict(
     "PipeSourceParametersTypeDef",
     {
@@ -1648,27 +1291,27 @@
     {
         "TaskDefinitionArn": str,
     },
 )
 _OptionalPipeTargetEcsTaskParametersOutputTypeDef = TypedDict(
     "_OptionalPipeTargetEcsTaskParametersOutputTypeDef",
     {
-        "CapacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "CapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "EnableECSManagedTags": bool,
         "EnableExecuteCommand": bool,
         "Group": str,
         "LaunchType": LaunchTypeType,
         "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
         "Overrides": EcsTaskOverrideOutputTypeDef,
-        "PlacementConstraints": List[PlacementConstraintOutputTypeDef],
-        "PlacementStrategy": List[PlacementStrategyOutputTypeDef],
+        "PlacementConstraints": List[PlacementConstraintTypeDef],
+        "PlacementStrategy": List[PlacementStrategyTypeDef],
         "PlatformVersion": str,
         "PropagateTags": Literal["TASK_DEFINITION"],
         "ReferenceId": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "TaskCount": int,
     },
     total=False,
 )
 
 class PipeTargetEcsTaskParametersOutputTypeDef(
     _RequiredPipeTargetEcsTaskParametersOutputTypeDef,
@@ -1708,25 +1351,25 @@
 ):
     pass
 
 PipeTargetParametersOutputTypeDef = TypedDict(
     "PipeTargetParametersOutputTypeDef",
     {
         "BatchJobParameters": PipeTargetBatchJobParametersOutputTypeDef,
-        "CloudWatchLogsParameters": PipeTargetCloudWatchLogsParametersOutputTypeDef,
+        "CloudWatchLogsParameters": PipeTargetCloudWatchLogsParametersTypeDef,
         "EcsTaskParameters": PipeTargetEcsTaskParametersOutputTypeDef,
         "EventBridgeEventBusParameters": PipeTargetEventBridgeEventBusParametersOutputTypeDef,
         "HttpParameters": PipeTargetHttpParametersOutputTypeDef,
         "InputTemplate": str,
-        "KinesisStreamParameters": PipeTargetKinesisStreamParametersOutputTypeDef,
-        "LambdaFunctionParameters": PipeTargetLambdaFunctionParametersOutputTypeDef,
+        "KinesisStreamParameters": PipeTargetKinesisStreamParametersTypeDef,
+        "LambdaFunctionParameters": PipeTargetLambdaFunctionParametersTypeDef,
         "RedshiftDataParameters": PipeTargetRedshiftDataParametersOutputTypeDef,
         "SageMakerPipelineParameters": PipeTargetSageMakerPipelineParametersOutputTypeDef,
-        "SqsQueueParameters": PipeTargetSqsQueueParametersOutputTypeDef,
-        "StepFunctionStateMachineParameters": PipeTargetStateMachineParametersOutputTypeDef,
+        "SqsQueueParameters": PipeTargetSqsQueueParametersTypeDef,
+        "StepFunctionStateMachineParameters": PipeTargetStateMachineParametersTypeDef,
     },
     total=False,
 )
 
 PipeTargetParametersTypeDef = TypedDict(
     "PipeTargetParametersTypeDef",
     {
```

### Comparing `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/PKG-INFO` & `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pipes
-Version: 1.28.12
-Summary: Type annotations for boto3.EventBridgePipes 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.EventBridgePipes 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pipes)](https://pepy.tech/project/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,82 +338,56 @@
 `mypy_boto3_pipes.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pipes.type_defs import (
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
-    BatchArrayPropertiesOutputTypeDef,
     BatchArrayPropertiesTypeDef,
-    BatchEnvironmentVariableOutputTypeDef,
-    BatchResourceRequirementOutputTypeDef,
     BatchEnvironmentVariableTypeDef,
     BatchResourceRequirementTypeDef,
-    BatchJobDependencyOutputTypeDef,
     BatchJobDependencyTypeDef,
-    BatchRetryStrategyOutputTypeDef,
     BatchRetryStrategyTypeDef,
-    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ResponseMetadataTypeDef,
-    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeletePipeRequestRequestTypeDef,
     DescribePipeRequestRequestTypeDef,
-    EcsEnvironmentFileOutputTypeDef,
-    EcsEnvironmentVariableOutputTypeDef,
-    EcsResourceRequirementOutputTypeDef,
     EcsEnvironmentFileTypeDef,
     EcsEnvironmentVariableTypeDef,
     EcsResourceRequirementTypeDef,
-    EcsEphemeralStorageOutputTypeDef,
     EcsEphemeralStorageTypeDef,
-    EcsInferenceAcceleratorOverrideOutputTypeDef,
     EcsInferenceAcceleratorOverrideTypeDef,
-    FilterOutputTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
     ListPipesRequestRequestTypeDef,
     PipeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    MQBrokerAccessCredentialsOutputTypeDef,
     MQBrokerAccessCredentialsTypeDef,
-    MSKAccessCredentialsOutputTypeDef,
     MSKAccessCredentialsTypeDef,
     PipeEnrichmentHttpParametersOutputTypeDef,
     PipeEnrichmentHttpParametersTypeDef,
-    PipeSourceSqsQueueParametersOutputTypeDef,
     PipeSourceSqsQueueParametersTypeDef,
-    SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef,
-    SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
+    SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     SelfManagedKafkaAccessConfigurationVpcTypeDef,
-    PipeTargetCloudWatchLogsParametersOutputTypeDef,
     PipeTargetCloudWatchLogsParametersTypeDef,
-    PlacementConstraintOutputTypeDef,
-    PlacementStrategyOutputTypeDef,
-    TagOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     TagTypeDef,
     PipeTargetEventBridgeEventBusParametersOutputTypeDef,
     PipeTargetEventBridgeEventBusParametersTypeDef,
     PipeTargetHttpParametersOutputTypeDef,
     PipeTargetHttpParametersTypeDef,
-    PipeTargetKinesisStreamParametersOutputTypeDef,
     PipeTargetKinesisStreamParametersTypeDef,
-    PipeTargetLambdaFunctionParametersOutputTypeDef,
     PipeTargetLambdaFunctionParametersTypeDef,
     PipeTargetRedshiftDataParametersOutputTypeDef,
-    PipeTargetSqsQueueParametersOutputTypeDef,
-    PipeTargetStateMachineParametersOutputTypeDef,
-    PipeTargetRedshiftDataParametersTypeDef,
     PipeTargetSqsQueueParametersTypeDef,
     PipeTargetStateMachineParametersTypeDef,
-    SageMakerPipelineParameterOutputTypeDef,
+    PipeTargetRedshiftDataParametersTypeDef,
     SageMakerPipelineParameterTypeDef,
     StartPipeRequestRequestTypeDef,
     StopPipeRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePipeSourceSqsQueueParametersTypeDef,
     NetworkConfigurationOutputTypeDef,
@@ -422,33 +396,29 @@
     BatchContainerOverridesTypeDef,
     CreatePipeResponseTypeDef,
     DeletePipeResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartPipeResponseTypeDef,
     StopPipeResponseTypeDef,
     UpdatePipeResponseTypeDef,
-    PipeSourceDynamoDBStreamParametersOutputTypeDef,
-    PipeSourceKinesisStreamParametersOutputTypeDef,
     PipeSourceDynamoDBStreamParametersTypeDef,
+    PipeSourceKinesisStreamParametersOutputTypeDef,
     PipeSourceKinesisStreamParametersTypeDef,
     UpdatePipeSourceDynamoDBStreamParametersTypeDef,
     UpdatePipeSourceKinesisStreamParametersTypeDef,
     EcsContainerOverrideOutputTypeDef,
     EcsContainerOverrideTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     ListPipesRequestListPipesPaginateTypeDef,
     ListPipesResponseTypeDef,
-    PipeSourceActiveMQBrokerParametersOutputTypeDef,
-    PipeSourceRabbitMQBrokerParametersOutputTypeDef,
     PipeSourceActiveMQBrokerParametersTypeDef,
     PipeSourceRabbitMQBrokerParametersTypeDef,
     UpdatePipeSourceActiveMQBrokerParametersTypeDef,
     UpdatePipeSourceRabbitMQBrokerParametersTypeDef,
-    PipeSourceManagedStreamingKafkaParametersOutputTypeDef,
     PipeSourceManagedStreamingKafkaParametersTypeDef,
     UpdatePipeSourceManagedStreamingKafkaParametersTypeDef,
     PipeEnrichmentParametersOutputTypeDef,
     PipeEnrichmentParametersTypeDef,
     PipeSourceSelfManagedKafkaParametersOutputTypeDef,
     PipeSourceSelfManagedKafkaParametersTypeDef,
     UpdatePipeSourceSelfManagedKafkaParametersTypeDef,
```

### Comparing `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/SOURCES.txt` & `mypy-boto3-pipes-1.28.15/mypy_boto3_pipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.12/setup.py` & `mypy-boto3-pipes-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pipes",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_pipes"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EventBridgePipes 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.EventBridgePipes 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

