# Comparing `tmp/mypy-boto3-kafka-1.28.12.tar.gz` & `tmp/mypy-boto3-kafka-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kafka-1.28.12.tar", last modified: Thu Jul 27 05:34:51 2023, max compression
+gzip compressed data, was "mypy-boto3-kafka-1.28.15.tar", last modified: Fri Jul 28 19:47:31 2023, max compression
```

## Comparing `mypy-boto3-kafka-1.28.12.tar` & `mypy-boto3-kafka-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.796474 mypy-boto3-kafka-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21610 2023-07-27 05:34:51.796474 mypy-boto3-kafka-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20131 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.792474 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34876 2023-07-27 05:24:27.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34814 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-07-27 05:24:27.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-07-27 05:24:27.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-07-27 05:24:27.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11460 2023-07-27 05:24:27.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64069 2023-07-27 05:24:29.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63988 2023-07-27 05:24:27.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.796474 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21610 2023-07-27 05:34:51.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 05:34:51.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:51.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:34:51.000000 mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:51.796474 mypy-boto3-kafka-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:24:26.000000 mypy-boto3-kafka-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.672180 mypy-boto3-kafka-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-07-28 19:47:31.672180 mypy-boto3-kafka-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19749 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.668180 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36588 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36523 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-28 19:47:12.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-07-28 19:47:12.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-07-28 19:47:12.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60653 2023-07-28 19:47:13.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60576 2023-07-28 19:47:12.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.672180 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-07-28 19:47:31.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 19:47:31.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 19:47:31.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 19:47:31.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:47:31.672180 mypy-boto3-kafka-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/setup.py
```

### Comparing `mypy-boto3-kafka-1.28.12/LICENSE` & `mypy-boto3-kafka-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.12/PKG-INFO` & `mypy-boto3-kafka-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafka
-Version: 1.28.12
-Summary: Type annotations for boto3.Kafka 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Kafka 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafka)](https://pepy.tech/project/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,14 +281,15 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kafka import KafkaClient
 from mypy_boto3_kafka.paginator import (
     ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
+    ListClusterOperationsV2Paginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
@@ -301,14 +302,17 @@
 # Types should be correctly discovered by mypy and IDEs
 list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator(
     "list_client_vpc_connections"
 )
 list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator(
     "list_cluster_operations"
 )
+list_cluster_operations_v2_paginator: ListClusterOperationsV2Paginator = client.get_paginator(
+    "list_cluster_operations_v2"
+)
 list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
 list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
 list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator(
     "list_configuration_revisions"
 )
 list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator(
     "list_configurations"
@@ -337,14 +341,15 @@
     ClusterStateType,
     ClusterTypeType,
     ConfigurationStateType,
     EnhancedMonitoringType,
     KafkaVersionStatusType,
     ListClientVpcConnectionsPaginatorName,
     ListClusterOperationsPaginatorName,
+    ListClusterOperationsV2PaginatorName,
     ListClustersPaginatorName,
     ListClustersV2PaginatorName,
     ListConfigurationRevisionsPaginatorName,
     ListConfigurationsPaginatorName,
     ListKafkaVersionsPaginatorName,
     ListNodesPaginatorName,
     ListScramSecretsPaginatorName,
@@ -371,211 +376,190 @@
 
 `mypy_boto3_kafka.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kafka.type_defs import (
     BatchAssociateScramSecretRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedScramSecretTypeDef,
     BatchDisassociateScramSecretRequestRequestTypeDef,
-    ProvisionedThroughputOutputTypeDef,
     ProvisionedThroughputTypeDef,
-    CloudWatchLogsOutputTypeDef,
-    FirehoseOutputTypeDef,
-    S3OutputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
     TlsOutputTypeDef,
-    UnauthenticatedOutputTypeDef,
-    TlsTypeDef,
     UnauthenticatedTypeDef,
+    TlsTypeDef,
     ClientVpcConnectionTypeDef,
     StateInfoTypeDef,
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
+    ClusterOperationV2SummaryTypeDef,
     CompatibleKafkaVersionTypeDef,
-    ConfigurationInfoOutputTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
-    PublicAccessOutputTypeDef,
     PublicAccessTypeDef,
-    CreateClusterResponseTypeDef,
-    CreateClusterV2ResponseTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateVpcConnectionRequestRequestTypeDef,
-    CreateVpcConnectionResponseTypeDef,
     DeleteClusterPolicyRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
-    DeleteClusterResponseTypeDef,
     DeleteConfigurationRequestRequestTypeDef,
-    DeleteConfigurationResponseTypeDef,
     DeleteVpcConnectionRequestRequestTypeDef,
-    DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationRequestRequestTypeDef,
+    DescribeClusterOperationV2RequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeClusterV2RequestRequestTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
-    DescribeConfigurationRevisionResponseTypeDef,
     DescribeVpcConnectionRequestRequestTypeDef,
-    DescribeVpcConnectionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionAtRestOutputTypeDef,
     EncryptionAtRestTypeDef,
-    EncryptionInTransitOutputTypeDef,
     EncryptionInTransitTypeDef,
     GetBootstrapBrokersRequestRequestTypeDef,
-    GetBootstrapBrokersResponseTypeDef,
     GetClusterPolicyRequestRequestTypeDef,
-    GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsRequestRequestTypeDef,
-    IamOutputTypeDef,
     IamTypeDef,
-    JmxExporterInfoOutputTypeDef,
     JmxExporterInfoTypeDef,
     JmxExporterTypeDef,
     KafkaVersionTypeDef,
-    ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListClientVpcConnectionsRequestRequestTypeDef,
-    ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     ListClusterOperationsRequestRequestTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
+    ListClusterOperationsV2RequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersV2RequestListClustersV2PaginateTypeDef,
     ListClustersV2RequestRequestTypeDef,
-    ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
-    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
     ListConfigurationsRequestRequestTypeDef,
-    ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
     ListKafkaVersionsRequestRequestTypeDef,
-    ListNodesRequestListNodesPaginateTypeDef,
     ListNodesRequestRequestTypeDef,
-    ListScramSecretsRequestListScramSecretsPaginateTypeDef,
     ListScramSecretsRequestRequestTypeDef,
-    ListScramSecretsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
     ListVpcConnectionsRequestRequestTypeDef,
     VpcConnectionTypeDef,
-    NodeExporterInfoOutputTypeDef,
     NodeExporterInfoTypeDef,
     NodeExporterTypeDef,
     ZookeeperNodeInfoTypeDef,
-    PaginatorConfigTypeDef,
     PutClusterPolicyRequestRequestTypeDef,
-    PutClusterPolicyResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
-    RebootBrokerResponseTypeDef,
     RejectClientVpcConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ScramOutputTypeDef,
     ScramTypeDef,
     VpcConfigTypeDef,
     VpcConfigOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
+    UpdateBrokerTypeRequestRequestTypeDef,
+    UpdateConfigurationRequestRequestTypeDef,
+    UserIdentityTypeDef,
+    VpcConnectivityTlsTypeDef,
+    VpcConnectivityIamTypeDef,
+    VpcConnectivityScramTypeDef,
+    CreateClusterResponseTypeDef,
+    CreateClusterV2ResponseTypeDef,
+    CreateVpcConnectionResponseTypeDef,
+    DeleteClusterResponseTypeDef,
+    DeleteConfigurationResponseTypeDef,
+    DeleteVpcConnectionResponseTypeDef,
+    DescribeConfigurationRevisionResponseTypeDef,
+    DescribeVpcConnectionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetBootstrapBrokersResponseTypeDef,
+    GetClusterPolicyResponseTypeDef,
+    ListScramSecretsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutClusterPolicyResponseTypeDef,
+    RebootBrokerResponseTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
-    UpdateBrokerTypeRequestRequestTypeDef,
     UpdateBrokerTypeResponseTypeDef,
     UpdateClusterConfigurationResponseTypeDef,
     UpdateClusterKafkaVersionResponseTypeDef,
-    UpdateConfigurationRequestRequestTypeDef,
     UpdateConnectivityResponseTypeDef,
     UpdateMonitoringResponseTypeDef,
     UpdateSecurityResponseTypeDef,
     UpdateStorageResponseTypeDef,
-    UserIdentityTypeDef,
-    VpcConnectivityTlsOutputTypeDef,
-    VpcConnectivityTlsTypeDef,
-    VpcConnectivityIamOutputTypeDef,
-    VpcConnectivityIamTypeDef,
-    VpcConnectivityScramOutputTypeDef,
-    VpcConnectivityScramTypeDef,
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
-    BrokerEBSVolumeInfoOutputTypeDef,
-    EBSStorageInfoOutputTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
-    BrokerLogsOutputTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
     ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
+    ListClusterOperationsV2ResponseTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     UpdateClusterConfigurationRequestRequestTypeDef,
     UpdateClusterKafkaVersionRequestRequestTypeDef,
     ConfigurationTypeDef,
     CreateConfigurationResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
-    EncryptionInfoOutputTypeDef,
     EncryptionInfoTypeDef,
-    ServerlessSaslOutputTypeDef,
     ServerlessSaslTypeDef,
     ListKafkaVersionsResponseTypeDef,
+    ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+    ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
+    ListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListClustersV2RequestListClustersV2PaginateTypeDef,
+    ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
+    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
+    ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
+    ListNodesRequestListNodesPaginateTypeDef,
+    ListScramSecretsRequestListScramSecretsPaginateTypeDef,
+    ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
     ListVpcConnectionsResponseTypeDef,
-    PrometheusInfoOutputTypeDef,
     PrometheusInfoTypeDef,
     PrometheusTypeDef,
-    SaslOutputTypeDef,
     SaslTypeDef,
+    VpcConnectionInfoServerlessTypeDef,
     VpcConnectionInfoTypeDef,
-    VpcConnectivitySaslOutputTypeDef,
     VpcConnectivitySaslTypeDef,
-    StorageInfoOutputTypeDef,
     UpdateBrokerStorageRequestRequestTypeDef,
     StorageInfoTypeDef,
-    LoggingInfoOutputTypeDef,
     LoggingInfoTypeDef,
     NodeInfoTypeDef,
     ListConfigurationsResponseTypeDef,
-    ServerlessClientAuthenticationOutputTypeDef,
     ServerlessClientAuthenticationTypeDef,
-    OpenMonitoringInfoOutputTypeDef,
     OpenMonitoringInfoTypeDef,
     OpenMonitoringTypeDef,
     ClientAuthenticationOutputTypeDef,
     ClientAuthenticationTypeDef,
-    VpcConnectivityClientAuthenticationOutputTypeDef,
+    ClusterOperationV2ServerlessTypeDef,
     VpcConnectivityClientAuthenticationTypeDef,
     ListNodesResponseTypeDef,
-    ServerlessTypeDef,
     ServerlessRequestTypeDef,
+    ServerlessTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
     UpdateSecurityRequestRequestTypeDef,
-    VpcConnectivityOutputTypeDef,
     VpcConnectivityTypeDef,
-    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
     BrokerNodeGroupInfoOutputTypeDef,
-    MutableClusterInfoTypeDef,
     BrokerNodeGroupInfoTypeDef,
+    MutableClusterInfoTypeDef,
     UpdateConnectivityRequestRequestTypeDef,
     ClusterInfoTypeDef,
     ProvisionedTypeDef,
-    ClusterOperationInfoTypeDef,
     CreateClusterRequestRequestTypeDef,
     ProvisionedRequestTypeDef,
+    ClusterOperationInfoTypeDef,
+    ClusterOperationV2ProvisionedTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
     ClusterTypeDef,
+    CreateClusterV2RequestRequestTypeDef,
     DescribeClusterOperationResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
-    CreateClusterV2RequestRequestTypeDef,
+    ClusterOperationV2TypeDef,
     DescribeClusterV2ResponseTypeDef,
     ListClustersV2ResponseTypeDef,
+    DescribeClusterOperationV2ResponseTypeDef,
 )
 
 
 def get_structure() -> BatchAssociateScramSecretRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-kafka-1.28.12/README.md` & `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-kafka
+Version: 1.28.15
+Summary: Type annotations for boto3.Kafka 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 kafka type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-kafka"></a>
 
 # mypy-boto3-kafka
 
 [![PyPI - mypy-boto3-kafka](https://img.shields.io/pypi/v/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafka)](https://pepy.tech/project/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
 
@@ -249,14 +281,15 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kafka import KafkaClient
 from mypy_boto3_kafka.paginator import (
     ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
+    ListClusterOperationsV2Paginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
@@ -269,14 +302,17 @@
 # Types should be correctly discovered by mypy and IDEs
 list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator(
     "list_client_vpc_connections"
 )
 list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator(
     "list_cluster_operations"
 )
+list_cluster_operations_v2_paginator: ListClusterOperationsV2Paginator = client.get_paginator(
+    "list_cluster_operations_v2"
+)
 list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
 list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
 list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator(
     "list_configuration_revisions"
 )
 list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator(
     "list_configurations"
@@ -305,14 +341,15 @@
     ClusterStateType,
     ClusterTypeType,
     ConfigurationStateType,
     EnhancedMonitoringType,
     KafkaVersionStatusType,
     ListClientVpcConnectionsPaginatorName,
     ListClusterOperationsPaginatorName,
+    ListClusterOperationsV2PaginatorName,
     ListClustersPaginatorName,
     ListClustersV2PaginatorName,
     ListConfigurationRevisionsPaginatorName,
     ListConfigurationsPaginatorName,
     ListKafkaVersionsPaginatorName,
     ListNodesPaginatorName,
     ListScramSecretsPaginatorName,
@@ -339,211 +376,190 @@
 
 `mypy_boto3_kafka.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kafka.type_defs import (
     BatchAssociateScramSecretRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedScramSecretTypeDef,
     BatchDisassociateScramSecretRequestRequestTypeDef,
-    ProvisionedThroughputOutputTypeDef,
     ProvisionedThroughputTypeDef,
-    CloudWatchLogsOutputTypeDef,
-    FirehoseOutputTypeDef,
-    S3OutputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
     TlsOutputTypeDef,
-    UnauthenticatedOutputTypeDef,
-    TlsTypeDef,
     UnauthenticatedTypeDef,
+    TlsTypeDef,
     ClientVpcConnectionTypeDef,
     StateInfoTypeDef,
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
+    ClusterOperationV2SummaryTypeDef,
     CompatibleKafkaVersionTypeDef,
-    ConfigurationInfoOutputTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
-    PublicAccessOutputTypeDef,
     PublicAccessTypeDef,
-    CreateClusterResponseTypeDef,
-    CreateClusterV2ResponseTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateVpcConnectionRequestRequestTypeDef,
-    CreateVpcConnectionResponseTypeDef,
     DeleteClusterPolicyRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
-    DeleteClusterResponseTypeDef,
     DeleteConfigurationRequestRequestTypeDef,
-    DeleteConfigurationResponseTypeDef,
     DeleteVpcConnectionRequestRequestTypeDef,
-    DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationRequestRequestTypeDef,
+    DescribeClusterOperationV2RequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeClusterV2RequestRequestTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
-    DescribeConfigurationRevisionResponseTypeDef,
     DescribeVpcConnectionRequestRequestTypeDef,
-    DescribeVpcConnectionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionAtRestOutputTypeDef,
     EncryptionAtRestTypeDef,
-    EncryptionInTransitOutputTypeDef,
     EncryptionInTransitTypeDef,
     GetBootstrapBrokersRequestRequestTypeDef,
-    GetBootstrapBrokersResponseTypeDef,
     GetClusterPolicyRequestRequestTypeDef,
-    GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsRequestRequestTypeDef,
-    IamOutputTypeDef,
     IamTypeDef,
-    JmxExporterInfoOutputTypeDef,
     JmxExporterInfoTypeDef,
     JmxExporterTypeDef,
     KafkaVersionTypeDef,
-    ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListClientVpcConnectionsRequestRequestTypeDef,
-    ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     ListClusterOperationsRequestRequestTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
+    ListClusterOperationsV2RequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersV2RequestListClustersV2PaginateTypeDef,
     ListClustersV2RequestRequestTypeDef,
-    ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
-    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
     ListConfigurationsRequestRequestTypeDef,
-    ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
     ListKafkaVersionsRequestRequestTypeDef,
-    ListNodesRequestListNodesPaginateTypeDef,
     ListNodesRequestRequestTypeDef,
-    ListScramSecretsRequestListScramSecretsPaginateTypeDef,
     ListScramSecretsRequestRequestTypeDef,
-    ListScramSecretsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
     ListVpcConnectionsRequestRequestTypeDef,
     VpcConnectionTypeDef,
-    NodeExporterInfoOutputTypeDef,
     NodeExporterInfoTypeDef,
     NodeExporterTypeDef,
     ZookeeperNodeInfoTypeDef,
-    PaginatorConfigTypeDef,
     PutClusterPolicyRequestRequestTypeDef,
-    PutClusterPolicyResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
-    RebootBrokerResponseTypeDef,
     RejectClientVpcConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ScramOutputTypeDef,
     ScramTypeDef,
     VpcConfigTypeDef,
     VpcConfigOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
+    UpdateBrokerTypeRequestRequestTypeDef,
+    UpdateConfigurationRequestRequestTypeDef,
+    UserIdentityTypeDef,
+    VpcConnectivityTlsTypeDef,
+    VpcConnectivityIamTypeDef,
+    VpcConnectivityScramTypeDef,
+    CreateClusterResponseTypeDef,
+    CreateClusterV2ResponseTypeDef,
+    CreateVpcConnectionResponseTypeDef,
+    DeleteClusterResponseTypeDef,
+    DeleteConfigurationResponseTypeDef,
+    DeleteVpcConnectionResponseTypeDef,
+    DescribeConfigurationRevisionResponseTypeDef,
+    DescribeVpcConnectionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetBootstrapBrokersResponseTypeDef,
+    GetClusterPolicyResponseTypeDef,
+    ListScramSecretsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutClusterPolicyResponseTypeDef,
+    RebootBrokerResponseTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
-    UpdateBrokerTypeRequestRequestTypeDef,
     UpdateBrokerTypeResponseTypeDef,
     UpdateClusterConfigurationResponseTypeDef,
     UpdateClusterKafkaVersionResponseTypeDef,
-    UpdateConfigurationRequestRequestTypeDef,
     UpdateConnectivityResponseTypeDef,
     UpdateMonitoringResponseTypeDef,
     UpdateSecurityResponseTypeDef,
     UpdateStorageResponseTypeDef,
-    UserIdentityTypeDef,
-    VpcConnectivityTlsOutputTypeDef,
-    VpcConnectivityTlsTypeDef,
-    VpcConnectivityIamOutputTypeDef,
-    VpcConnectivityIamTypeDef,
-    VpcConnectivityScramOutputTypeDef,
-    VpcConnectivityScramTypeDef,
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
-    BrokerEBSVolumeInfoOutputTypeDef,
-    EBSStorageInfoOutputTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
-    BrokerLogsOutputTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
     ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
+    ListClusterOperationsV2ResponseTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     UpdateClusterConfigurationRequestRequestTypeDef,
     UpdateClusterKafkaVersionRequestRequestTypeDef,
     ConfigurationTypeDef,
     CreateConfigurationResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
-    EncryptionInfoOutputTypeDef,
     EncryptionInfoTypeDef,
-    ServerlessSaslOutputTypeDef,
     ServerlessSaslTypeDef,
     ListKafkaVersionsResponseTypeDef,
+    ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+    ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
+    ListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListClustersV2RequestListClustersV2PaginateTypeDef,
+    ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
+    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
+    ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
+    ListNodesRequestListNodesPaginateTypeDef,
+    ListScramSecretsRequestListScramSecretsPaginateTypeDef,
+    ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
     ListVpcConnectionsResponseTypeDef,
-    PrometheusInfoOutputTypeDef,
     PrometheusInfoTypeDef,
     PrometheusTypeDef,
-    SaslOutputTypeDef,
     SaslTypeDef,
+    VpcConnectionInfoServerlessTypeDef,
     VpcConnectionInfoTypeDef,
-    VpcConnectivitySaslOutputTypeDef,
     VpcConnectivitySaslTypeDef,
-    StorageInfoOutputTypeDef,
     UpdateBrokerStorageRequestRequestTypeDef,
     StorageInfoTypeDef,
-    LoggingInfoOutputTypeDef,
     LoggingInfoTypeDef,
     NodeInfoTypeDef,
     ListConfigurationsResponseTypeDef,
-    ServerlessClientAuthenticationOutputTypeDef,
     ServerlessClientAuthenticationTypeDef,
-    OpenMonitoringInfoOutputTypeDef,
     OpenMonitoringInfoTypeDef,
     OpenMonitoringTypeDef,
     ClientAuthenticationOutputTypeDef,
     ClientAuthenticationTypeDef,
-    VpcConnectivityClientAuthenticationOutputTypeDef,
+    ClusterOperationV2ServerlessTypeDef,
     VpcConnectivityClientAuthenticationTypeDef,
     ListNodesResponseTypeDef,
-    ServerlessTypeDef,
     ServerlessRequestTypeDef,
+    ServerlessTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
     UpdateSecurityRequestRequestTypeDef,
-    VpcConnectivityOutputTypeDef,
     VpcConnectivityTypeDef,
-    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
     BrokerNodeGroupInfoOutputTypeDef,
-    MutableClusterInfoTypeDef,
     BrokerNodeGroupInfoTypeDef,
+    MutableClusterInfoTypeDef,
     UpdateConnectivityRequestRequestTypeDef,
     ClusterInfoTypeDef,
     ProvisionedTypeDef,
-    ClusterOperationInfoTypeDef,
     CreateClusterRequestRequestTypeDef,
     ProvisionedRequestTypeDef,
+    ClusterOperationInfoTypeDef,
+    ClusterOperationV2ProvisionedTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
     ClusterTypeDef,
+    CreateClusterV2RequestRequestTypeDef,
     DescribeClusterOperationResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
-    CreateClusterV2RequestRequestTypeDef,
+    ClusterOperationV2TypeDef,
     DescribeClusterV2ResponseTypeDef,
     ListClustersV2ResponseTypeDef,
+    DescribeClusterOperationV2ResponseTypeDef,
 )
 
 
 def get_structure() -> BatchAssociateScramSecretRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/__init__.py` & `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     ```python
     from boto3.session import Session
     from mypy_boto3_kafka import (
         Client,
         KafkaClient,
         ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
+        ListClusterOperationsV2Paginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
@@ -21,28 +22,30 @@
     )
 
     session = Session()
     client: KafkaClient = session.client("kafka")
 
     list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
+    list_cluster_operations_v2_paginator: ListClusterOperationsV2Paginator = client.get_paginator("list_cluster_operations_v2")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
     list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator("list_vpc_connections")
     ```
 """
 from .client import KafkaClient
 from .paginator import (
     ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
+    ListClusterOperationsV2Paginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
@@ -53,14 +56,15 @@
 
 
 __all__ = (
     "Client",
     "KafkaClient",
     "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
+    "ListClusterOperationsV2Paginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
```

### Comparing `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/__init__.pyi` & `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/__init__.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     ```python
     from boto3.session import Session
     from mypy_boto3_kafka import (
         Client,
         KafkaClient,
         ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
+        ListClusterOperationsV2Paginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
@@ -21,28 +22,30 @@
     )
 
     session = Session()
     client: KafkaClient = session.client("kafka")
 
     list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
+    list_cluster_operations_v2_paginator: ListClusterOperationsV2Paginator = client.get_paginator("list_cluster_operations_v2")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
     list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator("list_vpc_connections")
     ```
 """
 from .client import KafkaClient
 from .paginator import (
     ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
+    ListClusterOperationsV2Paginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
@@ -52,14 +55,15 @@
 Client = KafkaClient
 
 __all__ = (
     "Client",
     "KafkaClient",
     "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
+    "ListClusterOperationsV2Paginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
```

### Comparing `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/__main__.py` & `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Kafka 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Kafka 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka\nOther"
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

### Comparing `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/client.py` & `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import EnhancedMonitoringType, StorageModeType
 from .paginator import (
     ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
+    ListClusterOperationsV2Paginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
@@ -44,26 +45,28 @@
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
     CreateVpcConnectionResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteConfigurationResponseTypeDef,
     DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationResponseTypeDef,
+    DescribeClusterOperationV2ResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeClusterV2ResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
     DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionInfoTypeDef,
     GetBootstrapBrokersResponseTypeDef,
     GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
+    ListClusterOperationsV2ResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
@@ -291,14 +294,24 @@
         """
         Returns a description of the cluster operation specified by the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_operation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_cluster_operation)
         """
 
+    def describe_cluster_operation_v2(
+        self, *, ClusterOperationArn: str
+    ) -> DescribeClusterOperationV2ResponseTypeDef:
+        """
+        Returns a description of the cluster operation specified by the ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_operation_v2)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_cluster_operation_v2)
+        """
+
     def describe_cluster_v2(self, *, ClusterArn: str) -> DescribeClusterV2ResponseTypeDef:
         """
         Returns a description of the MSK cluster whose Amazon Resource Name (ARN) is
         specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_cluster_v2)
@@ -388,14 +401,25 @@
         Returns a list of all the operations that have been performed on the specified
         MSK cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_cluster_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_cluster_operations)
         """
 
+    def list_cluster_operations_v2(
+        self, *, ClusterArn: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListClusterOperationsV2ResponseTypeDef:
+        """
+        Returns a list of all the operations that have been performed on the specified
+        MSK cluster.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_cluster_operations_v2)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_cluster_operations_v2)
+        """
+
     def list_clusters(
         self, *, ClusterNameFilter: str = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> ListClustersResponseTypeDef:
         """
         Returns a list of all the MSK clusters in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_clusters)
@@ -682,14 +706,23 @@
     ) -> ListClusterOperationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_cluster_operations_v2"]
+    ) -> ListClusterOperationsV2Paginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_clusters"]) -> ListClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
         """
 
     @overload
```

### Comparing `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/client.pyi` & `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import EnhancedMonitoringType, StorageModeType
 from .paginator import (
     ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
+    ListClusterOperationsV2Paginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
@@ -44,26 +45,28 @@
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
     CreateVpcConnectionResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteConfigurationResponseTypeDef,
     DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationResponseTypeDef,
+    DescribeClusterOperationV2ResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeClusterV2ResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
     DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionInfoTypeDef,
     GetBootstrapBrokersResponseTypeDef,
     GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
+    ListClusterOperationsV2ResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
@@ -272,14 +275,23 @@
     ) -> DescribeClusterOperationResponseTypeDef:
         """
         Returns a description of the cluster operation specified by the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_operation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_cluster_operation)
         """
+    def describe_cluster_operation_v2(
+        self, *, ClusterOperationArn: str
+    ) -> DescribeClusterOperationV2ResponseTypeDef:
+        """
+        Returns a description of the cluster operation specified by the ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_operation_v2)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_cluster_operation_v2)
+        """
     def describe_cluster_v2(self, *, ClusterArn: str) -> DescribeClusterV2ResponseTypeDef:
         """
         Returns a description of the MSK cluster whose Amazon Resource Name (ARN) is
         specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_cluster_v2)
@@ -359,14 +371,24 @@
         """
         Returns a list of all the operations that have been performed on the specified
         MSK cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_cluster_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_cluster_operations)
         """
+    def list_cluster_operations_v2(
+        self, *, ClusterArn: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListClusterOperationsV2ResponseTypeDef:
+        """
+        Returns a list of all the operations that have been performed on the specified
+        MSK cluster.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_cluster_operations_v2)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_cluster_operations_v2)
+        """
     def list_clusters(
         self, *, ClusterNameFilter: str = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> ListClustersResponseTypeDef:
         """
         Returns a list of all the MSK clusters in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_clusters)
@@ -627,14 +649,22 @@
         self, operation_name: Literal["list_cluster_operations"]
     ) -> ListClusterOperationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
         """
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_cluster_operations_v2"]
+    ) -> ListClusterOperationsV2Paginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
+        """
+    @overload
     def get_paginator(self, operation_name: Literal["list_clusters"]) -> ListClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
         """
     @overload
     def get_paginator(self, operation_name: Literal["list_clusters_v2"]) -> ListClustersV2Paginator:
```

### Comparing `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/literals.py` & `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "ClusterStateType",
     "ClusterTypeType",
     "ConfigurationStateType",
     "EnhancedMonitoringType",
     "KafkaVersionStatusType",
     "ListClientVpcConnectionsPaginatorName",
     "ListClusterOperationsPaginatorName",
+    "ListClusterOperationsV2PaginatorName",
     "ListClustersPaginatorName",
     "ListClustersV2PaginatorName",
     "ListConfigurationRevisionsPaginatorName",
     "ListConfigurationsPaginatorName",
     "ListKafkaVersionsPaginatorName",
     "ListNodesPaginatorName",
     "ListScramSecretsPaginatorName",
@@ -65,14 +66,15 @@
 ConfigurationStateType = Literal["ACTIVE", "DELETE_FAILED", "DELETING"]
 EnhancedMonitoringType = Literal[
     "DEFAULT", "PER_BROKER", "PER_TOPIC_PER_BROKER", "PER_TOPIC_PER_PARTITION"
 ]
 KafkaVersionStatusType = Literal["ACTIVE", "DEPRECATED"]
 ListClientVpcConnectionsPaginatorName = Literal["list_client_vpc_connections"]
 ListClusterOperationsPaginatorName = Literal["list_cluster_operations"]
+ListClusterOperationsV2PaginatorName = Literal["list_cluster_operations_v2"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListClustersV2PaginatorName = Literal["list_clusters_v2"]
 ListConfigurationRevisionsPaginatorName = Literal["list_configuration_revisions"]
 ListConfigurationsPaginatorName = Literal["list_configurations"]
 ListKafkaVersionsPaginatorName = Literal["list_kafka_versions"]
 ListNodesPaginatorName = Literal["list_nodes"]
 ListScramSecretsPaginatorName = Literal["list_scram_secrets"]
@@ -457,14 +459,15 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_client_vpc_connections",
     "list_cluster_operations",
+    "list_cluster_operations_v2",
     "list_clusters",
     "list_clusters_v2",
     "list_configuration_revisions",
     "list_configurations",
     "list_kafka_versions",
     "list_nodes",
     "list_scram_secrets",
```

### Comparing `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/literals.pyi` & `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "ClusterStateType",
     "ClusterTypeType",
     "ConfigurationStateType",
     "EnhancedMonitoringType",
     "KafkaVersionStatusType",
     "ListClientVpcConnectionsPaginatorName",
     "ListClusterOperationsPaginatorName",
+    "ListClusterOperationsV2PaginatorName",
     "ListClustersPaginatorName",
     "ListClustersV2PaginatorName",
     "ListConfigurationRevisionsPaginatorName",
     "ListConfigurationsPaginatorName",
     "ListKafkaVersionsPaginatorName",
     "ListNodesPaginatorName",
     "ListScramSecretsPaginatorName",
@@ -63,14 +64,15 @@
 ConfigurationStateType = Literal["ACTIVE", "DELETE_FAILED", "DELETING"]
 EnhancedMonitoringType = Literal[
     "DEFAULT", "PER_BROKER", "PER_TOPIC_PER_BROKER", "PER_TOPIC_PER_PARTITION"
 ]
 KafkaVersionStatusType = Literal["ACTIVE", "DEPRECATED"]
 ListClientVpcConnectionsPaginatorName = Literal["list_client_vpc_connections"]
 ListClusterOperationsPaginatorName = Literal["list_cluster_operations"]
+ListClusterOperationsV2PaginatorName = Literal["list_cluster_operations_v2"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListClustersV2PaginatorName = Literal["list_clusters_v2"]
 ListConfigurationRevisionsPaginatorName = Literal["list_configuration_revisions"]
 ListConfigurationsPaginatorName = Literal["list_configurations"]
 ListKafkaVersionsPaginatorName = Literal["list_kafka_versions"]
 ListNodesPaginatorName = Literal["list_nodes"]
 ListScramSecretsPaginatorName = Literal["list_scram_secrets"]
@@ -455,14 +457,15 @@
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_client_vpc_connections",
     "list_cluster_operations",
+    "list_cluster_operations_v2",
     "list_clusters",
     "list_clusters_v2",
     "list_configuration_revisions",
     "list_configurations",
     "list_kafka_versions",
     "list_nodes",
     "list_scram_secrets",
```

### Comparing `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/paginator.py` & `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ```python
     from boto3.session import Session
 
     from mypy_boto3_kafka.client import KafkaClient
     from mypy_boto3_kafka.paginator import (
         ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
+        ListClusterOperationsV2Paginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
@@ -23,14 +24,15 @@
     )
 
     session = Session()
     client: KafkaClient = session.client("kafka")
 
     list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
+    list_cluster_operations_v2_paginator: ListClusterOperationsV2Paginator = client.get_paginator("list_cluster_operations_v2")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
@@ -40,28 +42,30 @@
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
+    ListClusterOperationsV2ResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
     ListVpcConnectionsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
+    "ListClusterOperationsV2Paginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
@@ -82,45 +86,60 @@
 class ListClientVpcConnectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClientVpcConnections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclientvpcconnectionspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClientVpcConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClientVpcConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclientvpcconnectionspaginator)
         """
 
 
 class ListClusterOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClusterOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
         """
 
 
+class ListClusterOperationsV2Paginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperationsV2)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationsv2paginator)
+    """
+
+    def paginate(
+        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListClusterOperationsV2ResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperationsV2.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationsv2paginator)
+        """
+
+
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, ClusterNameFilter: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterNameFilter: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusterspaginator)
         """
 
 
@@ -131,103 +150,103 @@
     """
 
     def paginate(
         self,
         *,
         ClusterNameFilter: str = ...,
         ClusterTypeFilter: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersV2ResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClustersV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclustersv2paginator)
         """
 
 
 class ListConfigurationRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurationRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationrevisionspaginator)
     """
 
     def paginate(
-        self, *, Arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfigurationRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurationRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationrevisionspaginator)
         """
 
 
 class ListConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationspaginator)
         """
 
 
 class ListKafkaVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListKafkaVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listkafkaversionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKafkaVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListKafkaVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listkafkaversionspaginator)
         """
 
 
 class ListNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listnodespaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listnodespaginator)
         """
 
 
 class ListScramSecretsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListScramSecrets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listscramsecretspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListScramSecretsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListScramSecrets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listscramsecretspaginator)
         """
 
 
 class ListVpcConnectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListVpcConnections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listvpcconnectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVpcConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListVpcConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listvpcconnectionspaginator)
         """
```

### Comparing `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/paginator.pyi` & `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ```python
     from boto3.session import Session
 
     from mypy_boto3_kafka.client import KafkaClient
     from mypy_boto3_kafka.paginator import (
         ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
+        ListClusterOperationsV2Paginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
@@ -23,14 +24,15 @@
     )
 
     session = Session()
     client: KafkaClient = session.client("kafka")
 
     list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
+    list_cluster_operations_v2_paginator: ListClusterOperationsV2Paginator = client.get_paginator("list_cluster_operations_v2")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
@@ -40,28 +42,30 @@
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
+    ListClusterOperationsV2ResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
     ListVpcConnectionsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
+    "ListClusterOperationsV2Paginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
@@ -79,43 +83,57 @@
 class ListClientVpcConnectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClientVpcConnections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclientvpcconnectionspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClientVpcConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClientVpcConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclientvpcconnectionspaginator)
         """
 
 class ListClusterOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClusterOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
         """
 
+class ListClusterOperationsV2Paginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperationsV2)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationsv2paginator)
+    """
+
+    def paginate(
+        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListClusterOperationsV2ResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperationsV2.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationsv2paginator)
+        """
+
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, ClusterNameFilter: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterNameFilter: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusterspaginator)
         """
 
 class ListClustersV2Paginator(Paginator):
@@ -125,97 +143,97 @@
     """
 
     def paginate(
         self,
         *,
         ClusterNameFilter: str = ...,
         ClusterTypeFilter: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersV2ResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClustersV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclustersv2paginator)
         """
 
 class ListConfigurationRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurationRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationrevisionspaginator)
     """
 
     def paginate(
-        self, *, Arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfigurationRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurationRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationrevisionspaginator)
         """
 
 class ListConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationspaginator)
         """
 
 class ListKafkaVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListKafkaVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listkafkaversionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKafkaVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListKafkaVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listkafkaversionspaginator)
         """
 
 class ListNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listnodespaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listnodespaginator)
         """
 
 class ListScramSecretsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListScramSecrets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listscramsecretspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListScramSecretsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListScramSecrets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listscramsecretspaginator)
         """
 
 class ListVpcConnectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListVpcConnections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listvpcconnectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVpcConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListVpcConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listvpcconnectionspaginator)
         """
```

### Comparing `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/type_defs.py` & `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -34,224 +34,213 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchAssociateScramSecretRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedScramSecretTypeDef",
     "BatchDisassociateScramSecretRequestRequestTypeDef",
-    "ProvisionedThroughputOutputTypeDef",
     "ProvisionedThroughputTypeDef",
-    "CloudWatchLogsOutputTypeDef",
-    "FirehoseOutputTypeDef",
-    "S3OutputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
     "TlsOutputTypeDef",
-    "UnauthenticatedOutputTypeDef",
-    "TlsTypeDef",
     "UnauthenticatedTypeDef",
+    "TlsTypeDef",
     "ClientVpcConnectionTypeDef",
     "StateInfoTypeDef",
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
+    "ClusterOperationV2SummaryTypeDef",
     "CompatibleKafkaVersionTypeDef",
-    "ConfigurationInfoOutputTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
-    "PublicAccessOutputTypeDef",
     "PublicAccessTypeDef",
-    "CreateClusterResponseTypeDef",
-    "CreateClusterV2ResponseTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
     "CreateVpcConnectionRequestRequestTypeDef",
-    "CreateVpcConnectionResponseTypeDef",
     "DeleteClusterPolicyRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
-    "DeleteClusterResponseTypeDef",
     "DeleteConfigurationRequestRequestTypeDef",
-    "DeleteConfigurationResponseTypeDef",
     "DeleteVpcConnectionRequestRequestTypeDef",
-    "DeleteVpcConnectionResponseTypeDef",
     "DescribeClusterOperationRequestRequestTypeDef",
+    "DescribeClusterOperationV2RequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeClusterV2RequestRequestTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
-    "DescribeConfigurationRevisionResponseTypeDef",
     "DescribeVpcConnectionRequestRequestTypeDef",
-    "DescribeVpcConnectionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EncryptionAtRestOutputTypeDef",
     "EncryptionAtRestTypeDef",
-    "EncryptionInTransitOutputTypeDef",
     "EncryptionInTransitTypeDef",
     "GetBootstrapBrokersRequestRequestTypeDef",
-    "GetBootstrapBrokersResponseTypeDef",
     "GetClusterPolicyRequestRequestTypeDef",
-    "GetClusterPolicyResponseTypeDef",
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
-    "IamOutputTypeDef",
     "IamTypeDef",
-    "JmxExporterInfoOutputTypeDef",
     "JmxExporterInfoTypeDef",
     "JmxExporterTypeDef",
     "KafkaVersionTypeDef",
-    "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListClientVpcConnectionsRequestRequestTypeDef",
-    "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     "ListClusterOperationsRequestRequestTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListClusterOperationsV2RequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListClustersV2RequestListClustersV2PaginateTypeDef",
     "ListClustersV2RequestRequestTypeDef",
-    "ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
-    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
-    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
     "ListKafkaVersionsRequestRequestTypeDef",
-    "ListNodesRequestListNodesPaginateTypeDef",
     "ListNodesRequestRequestTypeDef",
-    "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
     "ListScramSecretsRequestRequestTypeDef",
-    "ListScramSecretsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     "ListVpcConnectionsRequestRequestTypeDef",
     "VpcConnectionTypeDef",
-    "NodeExporterInfoOutputTypeDef",
     "NodeExporterInfoTypeDef",
     "NodeExporterTypeDef",
     "ZookeeperNodeInfoTypeDef",
-    "PaginatorConfigTypeDef",
     "PutClusterPolicyRequestRequestTypeDef",
-    "PutClusterPolicyResponseTypeDef",
     "RebootBrokerRequestRequestTypeDef",
-    "RebootBrokerResponseTypeDef",
     "RejectClientVpcConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "ScramOutputTypeDef",
     "ScramTypeDef",
     "VpcConfigTypeDef",
     "VpcConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
+    "UpdateBrokerTypeRequestRequestTypeDef",
+    "UpdateConfigurationRequestRequestTypeDef",
+    "UserIdentityTypeDef",
+    "VpcConnectivityTlsTypeDef",
+    "VpcConnectivityIamTypeDef",
+    "VpcConnectivityScramTypeDef",
+    "CreateClusterResponseTypeDef",
+    "CreateClusterV2ResponseTypeDef",
+    "CreateVpcConnectionResponseTypeDef",
+    "DeleteClusterResponseTypeDef",
+    "DeleteConfigurationResponseTypeDef",
+    "DeleteVpcConnectionResponseTypeDef",
+    "DescribeConfigurationRevisionResponseTypeDef",
+    "DescribeVpcConnectionResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetBootstrapBrokersResponseTypeDef",
+    "GetClusterPolicyResponseTypeDef",
+    "ListScramSecretsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutClusterPolicyResponseTypeDef",
+    "RebootBrokerResponseTypeDef",
     "UpdateBrokerCountResponseTypeDef",
     "UpdateBrokerStorageResponseTypeDef",
-    "UpdateBrokerTypeRequestRequestTypeDef",
     "UpdateBrokerTypeResponseTypeDef",
     "UpdateClusterConfigurationResponseTypeDef",
     "UpdateClusterKafkaVersionResponseTypeDef",
-    "UpdateConfigurationRequestRequestTypeDef",
     "UpdateConnectivityResponseTypeDef",
     "UpdateMonitoringResponseTypeDef",
     "UpdateSecurityResponseTypeDef",
     "UpdateStorageResponseTypeDef",
-    "UserIdentityTypeDef",
-    "VpcConnectivityTlsOutputTypeDef",
-    "VpcConnectivityTlsTypeDef",
-    "VpcConnectivityIamOutputTypeDef",
-    "VpcConnectivityIamTypeDef",
-    "VpcConnectivityScramOutputTypeDef",
-    "VpcConnectivityScramTypeDef",
     "BatchAssociateScramSecretResponseTypeDef",
     "BatchDisassociateScramSecretResponseTypeDef",
-    "BrokerEBSVolumeInfoOutputTypeDef",
-    "EBSStorageInfoOutputTypeDef",
     "BrokerEBSVolumeInfoTypeDef",
     "EBSStorageInfoTypeDef",
     "UpdateStorageRequestRequestTypeDef",
-    "BrokerLogsOutputTypeDef",
     "BrokerLogsTypeDef",
     "BrokerNodeInfoTypeDef",
     "ListClientVpcConnectionsResponseTypeDef",
     "ClusterOperationStepTypeDef",
+    "ListClusterOperationsV2ResponseTypeDef",
     "GetCompatibleKafkaVersionsResponseTypeDef",
     "UpdateClusterConfigurationRequestRequestTypeDef",
     "UpdateClusterKafkaVersionRequestRequestTypeDef",
     "ConfigurationTypeDef",
     "CreateConfigurationResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
     "UpdateConfigurationResponseTypeDef",
-    "EncryptionInfoOutputTypeDef",
     "EncryptionInfoTypeDef",
-    "ServerlessSaslOutputTypeDef",
     "ServerlessSaslTypeDef",
     "ListKafkaVersionsResponseTypeDef",
+    "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
+    "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
+    "ListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListClustersV2RequestListClustersV2PaginateTypeDef",
+    "ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
+    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
+    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
+    "ListNodesRequestListNodesPaginateTypeDef",
+    "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
+    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     "ListVpcConnectionsResponseTypeDef",
-    "PrometheusInfoOutputTypeDef",
     "PrometheusInfoTypeDef",
     "PrometheusTypeDef",
-    "SaslOutputTypeDef",
     "SaslTypeDef",
+    "VpcConnectionInfoServerlessTypeDef",
     "VpcConnectionInfoTypeDef",
-    "VpcConnectivitySaslOutputTypeDef",
     "VpcConnectivitySaslTypeDef",
-    "StorageInfoOutputTypeDef",
     "UpdateBrokerStorageRequestRequestTypeDef",
     "StorageInfoTypeDef",
-    "LoggingInfoOutputTypeDef",
     "LoggingInfoTypeDef",
     "NodeInfoTypeDef",
     "ListConfigurationsResponseTypeDef",
-    "ServerlessClientAuthenticationOutputTypeDef",
     "ServerlessClientAuthenticationTypeDef",
-    "OpenMonitoringInfoOutputTypeDef",
     "OpenMonitoringInfoTypeDef",
     "OpenMonitoringTypeDef",
     "ClientAuthenticationOutputTypeDef",
     "ClientAuthenticationTypeDef",
-    "VpcConnectivityClientAuthenticationOutputTypeDef",
+    "ClusterOperationV2ServerlessTypeDef",
     "VpcConnectivityClientAuthenticationTypeDef",
     "ListNodesResponseTypeDef",
-    "ServerlessTypeDef",
     "ServerlessRequestTypeDef",
+    "ServerlessTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
     "UpdateSecurityRequestRequestTypeDef",
-    "VpcConnectivityOutputTypeDef",
     "VpcConnectivityTypeDef",
-    "ConnectivityInfoOutputTypeDef",
     "ConnectivityInfoTypeDef",
     "BrokerNodeGroupInfoOutputTypeDef",
-    "MutableClusterInfoTypeDef",
     "BrokerNodeGroupInfoTypeDef",
+    "MutableClusterInfoTypeDef",
     "UpdateConnectivityRequestRequestTypeDef",
     "ClusterInfoTypeDef",
     "ProvisionedTypeDef",
-    "ClusterOperationInfoTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ProvisionedRequestTypeDef",
+    "ClusterOperationInfoTypeDef",
+    "ClusterOperationV2ProvisionedTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
     "ClusterTypeDef",
+    "CreateClusterV2RequestRequestTypeDef",
     "DescribeClusterOperationResponseTypeDef",
     "ListClusterOperationsResponseTypeDef",
-    "CreateClusterV2RequestRequestTypeDef",
+    "ClusterOperationV2TypeDef",
     "DescribeClusterV2ResponseTypeDef",
     "ListClustersV2ResponseTypeDef",
+    "DescribeClusterOperationV2ResponseTypeDef",
 )
 
 BatchAssociateScramSecretRequestRequestTypeDef = TypedDict(
     "BatchAssociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 UnprocessedScramSecretTypeDef = TypedDict(
     "UnprocessedScramSecretTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "SecretArn": str,
     },
@@ -262,130 +251,57 @@
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
     },
 )
 
-ProvisionedThroughputOutputTypeDef = TypedDict(
-    "ProvisionedThroughputOutputTypeDef",
-    {
-        "Enabled": bool,
-        "VolumeThroughput": int,
-    },
-    total=False,
-)
-
 ProvisionedThroughputTypeDef = TypedDict(
     "ProvisionedThroughputTypeDef",
     {
         "Enabled": bool,
         "VolumeThroughput": int,
     },
     total=False,
 )
 
-_RequiredCloudWatchLogsOutputTypeDef = TypedDict(
-    "_RequiredCloudWatchLogsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalCloudWatchLogsOutputTypeDef = TypedDict(
-    "_OptionalCloudWatchLogsOutputTypeDef",
-    {
-        "LogGroup": str,
-    },
-    total=False,
-)
-
-
-class CloudWatchLogsOutputTypeDef(
-    _RequiredCloudWatchLogsOutputTypeDef, _OptionalCloudWatchLogsOutputTypeDef
-):
-    pass
-
-
-_RequiredFirehoseOutputTypeDef = TypedDict(
-    "_RequiredFirehoseOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalFirehoseOutputTypeDef = TypedDict(
-    "_OptionalFirehoseOutputTypeDef",
-    {
-        "DeliveryStream": str,
-    },
-    total=False,
-)
-
-
-class FirehoseOutputTypeDef(_RequiredFirehoseOutputTypeDef, _OptionalFirehoseOutputTypeDef):
-    pass
-
-
-_RequiredS3OutputTypeDef = TypedDict(
-    "_RequiredS3OutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalS3OutputTypeDef = TypedDict(
-    "_OptionalS3OutputTypeDef",
-    {
-        "Bucket": str,
-        "Prefix": str,
-    },
-    total=False,
-)
-
-
-class S3OutputTypeDef(_RequiredS3OutputTypeDef, _OptionalS3OutputTypeDef):
-    pass
-
-
 _RequiredCloudWatchLogsTypeDef = TypedDict(
     "_RequiredCloudWatchLogsTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalCloudWatchLogsTypeDef = TypedDict(
     "_OptionalCloudWatchLogsTypeDef",
     {
         "LogGroup": str,
     },
     total=False,
 )
 
-
 class CloudWatchLogsTypeDef(_RequiredCloudWatchLogsTypeDef, _OptionalCloudWatchLogsTypeDef):
     pass
 
-
 _RequiredFirehoseTypeDef = TypedDict(
     "_RequiredFirehoseTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalFirehoseTypeDef = TypedDict(
     "_OptionalFirehoseTypeDef",
     {
         "DeliveryStream": str,
     },
     total=False,
 )
 
-
 class FirehoseTypeDef(_RequiredFirehoseTypeDef, _OptionalFirehoseTypeDef):
     pass
 
-
 _RequiredS3TypeDef = TypedDict(
     "_RequiredS3TypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalS3TypeDef = TypedDict(
@@ -393,19 +309,17 @@
     {
         "Bucket": str,
         "Prefix": str,
     },
     total=False,
 )
 
-
 class S3TypeDef(_RequiredS3TypeDef, _OptionalS3TypeDef):
     pass
 
-
 BrokerSoftwareInfoTypeDef = TypedDict(
     "BrokerSoftwareInfoTypeDef",
     {
         "ConfigurationArn": str,
         "ConfigurationRevision": int,
         "KafkaVersion": str,
     },
@@ -417,16 +331,16 @@
     {
         "CertificateAuthorityArnList": List[str],
         "Enabled": bool,
     },
     total=False,
 )
 
-UnauthenticatedOutputTypeDef = TypedDict(
-    "UnauthenticatedOutputTypeDef",
+UnauthenticatedTypeDef = TypedDict(
+    "UnauthenticatedTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
 TlsTypeDef = TypedDict(
@@ -434,22 +348,14 @@
     {
         "CertificateAuthorityArnList": Sequence[str],
         "Enabled": bool,
     },
     total=False,
 )
 
-UnauthenticatedTypeDef = TypedDict(
-    "UnauthenticatedTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 _RequiredClientVpcConnectionTypeDef = TypedDict(
     "_RequiredClientVpcConnectionTypeDef",
     {
         "VpcConnectionArn": str,
     },
 )
 _OptionalClientVpcConnectionTypeDef = TypedDict(
@@ -459,21 +365,19 @@
         "CreationTime": datetime,
         "State": VpcConnectionStateType,
         "Owner": str,
     },
     total=False,
 )
 
-
 class ClientVpcConnectionTypeDef(
     _RequiredClientVpcConnectionTypeDef, _OptionalClientVpcConnectionTypeDef
 ):
     pass
 
-
 StateInfoTypeDef = TypedDict(
     "StateInfoTypeDef",
     {
         "Code": str,
         "Message": str,
     },
     total=False,
@@ -492,29 +396,35 @@
     "ClusterOperationStepInfoTypeDef",
     {
         "StepStatus": str,
     },
     total=False,
 )
 
-CompatibleKafkaVersionTypeDef = TypedDict(
-    "CompatibleKafkaVersionTypeDef",
+ClusterOperationV2SummaryTypeDef = TypedDict(
+    "ClusterOperationV2SummaryTypeDef",
     {
-        "SourceVersion": str,
-        "TargetVersions": List[str],
+        "ClusterArn": str,
+        "ClusterType": ClusterTypeType,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "OperationArn": str,
+        "OperationState": str,
+        "OperationType": str,
     },
     total=False,
 )
 
-ConfigurationInfoOutputTypeDef = TypedDict(
-    "ConfigurationInfoOutputTypeDef",
+CompatibleKafkaVersionTypeDef = TypedDict(
+    "CompatibleKafkaVersionTypeDef",
     {
-        "Arn": str,
-        "Revision": int,
+        "SourceVersion": str,
+        "TargetVersions": List[str],
     },
+    total=False,
 )
 
 ConfigurationInfoTypeDef = TypedDict(
     "ConfigurationInfoTypeDef",
     {
         "Arn": str,
         "Revision": int,
@@ -532,58 +442,27 @@
     "_OptionalConfigurationRevisionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class ConfigurationRevisionTypeDef(
     _RequiredConfigurationRevisionTypeDef, _OptionalConfigurationRevisionTypeDef
 ):
     pass
 
-
-PublicAccessOutputTypeDef = TypedDict(
-    "PublicAccessOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
 PublicAccessTypeDef = TypedDict(
     "PublicAccessTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-CreateClusterResponseTypeDef = TypedDict(
-    "CreateClusterResponseTypeDef",
-    {
-        "ClusterArn": str,
-        "ClusterName": str,
-        "State": ClusterStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateClusterV2ResponseTypeDef = TypedDict(
-    "CreateClusterV2ResponseTypeDef",
-    {
-        "ClusterArn": str,
-        "ClusterName": str,
-        "State": ClusterStateType,
-        "ClusterType": ClusterTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationRequestRequestTypeDef",
     {
         "Name": str,
         "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
@@ -592,22 +471,20 @@
     {
         "Description": str,
         "KafkaVersions": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateConfigurationRequestRequestTypeDef(
     _RequiredCreateConfigurationRequestRequestTypeDef,
     _OptionalCreateConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateVpcConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcConnectionRequestRequestTypeDef",
     {
         "TargetClusterArn": str,
         "Authentication": str,
         "VpcId": str,
         "ClientSubnets": Sequence[str],
@@ -618,37 +495,20 @@
     "_OptionalCreateVpcConnectionRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateVpcConnectionRequestRequestTypeDef(
     _RequiredCreateVpcConnectionRequestRequestTypeDef,
     _OptionalCreateVpcConnectionRequestRequestTypeDef,
 ):
     pass
 
-
-CreateVpcConnectionResponseTypeDef = TypedDict(
-    "CreateVpcConnectionResponseTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "State": VpcConnectionStateType,
-        "Authentication": str,
-        "VpcId": str,
-        "ClientSubnets": List[str],
-        "SecurityGroups": List[str],
-        "CreationTime": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteClusterPolicyRequestRequestTypeDef = TypedDict(
     "DeleteClusterPolicyRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 
@@ -662,64 +522,42 @@
     "_OptionalDeleteClusterRequestRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
-
 class DeleteClusterRequestRequestTypeDef(
     _RequiredDeleteClusterRequestRequestTypeDef, _OptionalDeleteClusterRequestRequestTypeDef
 ):
     pass
 
-
-DeleteClusterResponseTypeDef = TypedDict(
-    "DeleteClusterResponseTypeDef",
-    {
-        "ClusterArn": str,
-        "State": ClusterStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteConfigurationResponseTypeDef = TypedDict(
-    "DeleteConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "State": ConfigurationStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVpcConnectionRequestRequestTypeDef = TypedDict(
     "DeleteVpcConnectionRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteVpcConnectionResponseTypeDef = TypedDict(
-    "DeleteVpcConnectionResponseTypeDef",
+DescribeClusterOperationRequestRequestTypeDef = TypedDict(
+    "DescribeClusterOperationRequestRequestTypeDef",
     {
-        "VpcConnectionArn": str,
-        "State": VpcConnectionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterOperationArn": str,
     },
 )
 
-DescribeClusterOperationRequestRequestTypeDef = TypedDict(
-    "DescribeClusterOperationRequestRequestTypeDef",
+DescribeClusterOperationV2RequestRequestTypeDef = TypedDict(
+    "DescribeClusterOperationV2RequestRequestTypeDef",
     {
         "ClusterOperationArn": str,
     },
 )
 
 DescribeClusterRequestRequestTypeDef = TypedDict(
     "DescribeClusterRequestRequestTypeDef",
@@ -746,79 +584,28 @@
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     {
         "Arn": str,
         "Revision": int,
     },
 )
 
-DescribeConfigurationRevisionResponseTypeDef = TypedDict(
-    "DescribeConfigurationRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "Description": str,
-        "Revision": int,
-        "ServerProperties": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeVpcConnectionRequestRequestTypeDef = TypedDict(
     "DescribeVpcConnectionRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DescribeVpcConnectionResponseTypeDef = TypedDict(
-    "DescribeVpcConnectionResponseTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "TargetClusterArn": str,
-        "State": VpcConnectionStateType,
-        "Authentication": str,
-        "VpcId": str,
-        "Subnets": List[str],
-        "SecurityGroups": List[str],
-        "CreationTime": datetime,
-        "Tags": Dict[str, str],
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
-EncryptionAtRestOutputTypeDef = TypedDict(
-    "EncryptionAtRestOutputTypeDef",
-    {
-        "DataVolumeKMSKeyId": str,
-    },
-)
-
 EncryptionAtRestTypeDef = TypedDict(
     "EncryptionAtRestTypeDef",
     {
         "DataVolumeKMSKeyId": str,
     },
 )
 
-EncryptionInTransitOutputTypeDef = TypedDict(
-    "EncryptionInTransitOutputTypeDef",
-    {
-        "ClientBroker": ClientBrokerType,
-        "InCluster": bool,
-    },
-    total=False,
-)
-
 EncryptionInTransitTypeDef = TypedDict(
     "EncryptionInTransitTypeDef",
     {
         "ClientBroker": ClientBrokerType,
         "InCluster": bool,
     },
     total=False,
@@ -827,78 +614,37 @@
 GetBootstrapBrokersRequestRequestTypeDef = TypedDict(
     "GetBootstrapBrokersRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 
-GetBootstrapBrokersResponseTypeDef = TypedDict(
-    "GetBootstrapBrokersResponseTypeDef",
-    {
-        "BootstrapBrokerString": str,
-        "BootstrapBrokerStringTls": str,
-        "BootstrapBrokerStringSaslScram": str,
-        "BootstrapBrokerStringSaslIam": str,
-        "BootstrapBrokerStringPublicTls": str,
-        "BootstrapBrokerStringPublicSaslScram": str,
-        "BootstrapBrokerStringPublicSaslIam": str,
-        "BootstrapBrokerStringVpcConnectivityTls": str,
-        "BootstrapBrokerStringVpcConnectivitySaslScram": str,
-        "BootstrapBrokerStringVpcConnectivitySaslIam": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetClusterPolicyRequestRequestTypeDef = TypedDict(
     "GetClusterPolicyRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 
-GetClusterPolicyResponseTypeDef = TypedDict(
-    "GetClusterPolicyResponseTypeDef",
-    {
-        "CurrentVersion": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCompatibleKafkaVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
     total=False,
 )
 
-IamOutputTypeDef = TypedDict(
-    "IamOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 IamTypeDef = TypedDict(
     "IamTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-JmxExporterInfoOutputTypeDef = TypedDict(
-    "JmxExporterInfoOutputTypeDef",
-    {
-        "EnabledInBroker": bool,
-    },
-)
-
 JmxExporterInfoTypeDef = TypedDict(
     "JmxExporterInfoTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
 
@@ -914,36 +660,24 @@
     {
         "Version": str,
         "Status": KafkaVersionStatusType,
     },
     total=False,
 )
 
-_RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
-    "_RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
-    "_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
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
-class ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef(
-    _RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
-    _OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListClientVpcConnectionsRequestRequestTypeDef = TypedDict(
     "_RequiredListClientVpcConnectionsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClientVpcConnectionsRequestRequestTypeDef = TypedDict(
@@ -951,44 +685,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListClientVpcConnectionsRequestRequestTypeDef(
     _RequiredListClientVpcConnectionsRequestRequestTypeDef,
     _OptionalListClientVpcConnectionsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListClusterOperationsRequestListClusterOperationsPaginateTypeDef(
-    _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
-    _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListClusterOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterOperationsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsRequestRequestTypeDef = TypedDict(
@@ -996,47 +706,47 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListClusterOperationsRequestRequestTypeDef(
     _RequiredListClusterOperationsRequestRequestTypeDef,
     _OptionalListClusterOperationsRequestRequestTypeDef,
 ):
     pass
 
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
+_RequiredListClusterOperationsV2RequestRequestTypeDef = TypedDict(
+    "_RequiredListClusterOperationsV2RequestRequestTypeDef",
     {
-        "ClusterNameFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ClusterArn": str,
     },
-    total=False,
 )
-
-ListClustersRequestRequestTypeDef = TypedDict(
-    "ListClustersRequestRequestTypeDef",
+_OptionalListClusterOperationsV2RequestRequestTypeDef = TypedDict(
+    "_OptionalListClusterOperationsV2RequestRequestTypeDef",
     {
-        "ClusterNameFilter": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListClustersV2RequestListClustersV2PaginateTypeDef = TypedDict(
-    "ListClustersV2RequestListClustersV2PaginateTypeDef",
+class ListClusterOperationsV2RequestRequestTypeDef(
+    _RequiredListClusterOperationsV2RequestRequestTypeDef,
+    _OptionalListClusterOperationsV2RequestRequestTypeDef,
+):
+    pass
+
+ListClustersRequestRequestTypeDef = TypedDict(
+    "ListClustersRequestRequestTypeDef",
     {
         "ClusterNameFilter": str,
-        "ClusterTypeFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
 ListClustersV2RequestRequestTypeDef = TypedDict(
     "ListClustersV2RequestRequestTypeDef",
     {
@@ -1044,36 +754,14 @@
         "ClusterTypeFilter": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef(
-    _RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
-    _OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListConfigurationRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredListConfigurationRevisionsRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListConfigurationRevisionsRequestRequestTypeDef = TypedDict(
@@ -1081,78 +769,38 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListConfigurationRevisionsRequestRequestTypeDef(
     _RequiredListConfigurationRevisionsRequestRequestTypeDef,
     _OptionalListConfigurationRevisionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
-    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListConfigurationsRequestRequestTypeDef = TypedDict(
     "ListConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef = TypedDict(
-    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKafkaVersionsRequestRequestTypeDef = TypedDict(
     "ListKafkaVersionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListNodesRequestListNodesPaginateTypeDef = TypedDict(
-    "_RequiredListNodesRequestListNodesPaginateTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-_OptionalListNodesRequestListNodesPaginateTypeDef = TypedDict(
-    "_OptionalListNodesRequestListNodesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListNodesRequestListNodesPaginateTypeDef(
-    _RequiredListNodesRequestListNodesPaginateTypeDef,
-    _OptionalListNodesRequestListNodesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListNodesRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListNodesRequestRequestTypeDef = TypedDict(
@@ -1160,43 +808,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListNodesRequestRequestTypeDef(
     _RequiredListNodesRequestRequestTypeDef, _OptionalListNodesRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
-    "_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
-    "_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListScramSecretsRequestListScramSecretsPaginateTypeDef(
-    _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef,
-    _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListScramSecretsRequestRequestTypeDef = TypedDict(
     "_RequiredListScramSecretsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListScramSecretsRequestRequestTypeDef = TypedDict(
@@ -1204,53 +828,26 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListScramSecretsRequestRequestTypeDef(
     _RequiredListScramSecretsRequestRequestTypeDef, _OptionalListScramSecretsRequestRequestTypeDef
 ):
     pass
 
-
-ListScramSecretsResponseTypeDef = TypedDict(
-    "ListScramSecretsResponseTypeDef",
-    {
-        "NextToken": str,
-        "SecretArnList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef = TypedDict(
-    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVpcConnectionsRequestRequestTypeDef = TypedDict(
     "ListVpcConnectionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1270,26 +867,17 @@
         "Authentication": str,
         "VpcId": str,
         "State": VpcConnectionStateType,
     },
     total=False,
 )
 
-
 class VpcConnectionTypeDef(_RequiredVpcConnectionTypeDef, _OptionalVpcConnectionTypeDef):
     pass
 
-
-NodeExporterInfoOutputTypeDef = TypedDict(
-    "NodeExporterInfoOutputTypeDef",
-    {
-        "EnabledInBroker": bool,
-    },
-)
-
 NodeExporterInfoTypeDef = TypedDict(
     "NodeExporterInfoTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
 
@@ -1308,24 +896,14 @@
         "Endpoints": List[str],
         "ZookeeperId": float,
         "ZookeeperVersion": str,
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
 _RequiredPutClusterPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutClusterPolicyRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "Policy": str,
     },
 )
@@ -1333,73 +911,35 @@
     "_OptionalPutClusterPolicyRequestRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
-
 class PutClusterPolicyRequestRequestTypeDef(
     _RequiredPutClusterPolicyRequestRequestTypeDef, _OptionalPutClusterPolicyRequestRequestTypeDef
 ):
     pass
 
-
-PutClusterPolicyResponseTypeDef = TypedDict(
-    "PutClusterPolicyResponseTypeDef",
-    {
-        "CurrentVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RebootBrokerRequestRequestTypeDef = TypedDict(
     "RebootBrokerRequestRequestTypeDef",
     {
         "BrokerIds": Sequence[str],
         "ClusterArn": str,
     },
 )
 
-RebootBrokerResponseTypeDef = TypedDict(
-    "RebootBrokerResponseTypeDef",
-    {
-        "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RejectClientVpcConnectionRequestRequestTypeDef = TypedDict(
     "RejectClientVpcConnectionRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "VpcConnectionArn": str,
     },
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
-ScramOutputTypeDef = TypedDict(
-    "ScramOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 ScramTypeDef = TypedDict(
     "ScramTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1414,38 +954,34 @@
     "_OptionalVpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class VpcConfigTypeDef(_RequiredVpcConfigTypeDef, _OptionalVpcConfigTypeDef):
     pass
 
-
 _RequiredVpcConfigOutputTypeDef = TypedDict(
     "_RequiredVpcConfigOutputTypeDef",
     {
         "SubnetIds": List[str],
     },
 )
 _OptionalVpcConfigOutputTypeDef = TypedDict(
     "_OptionalVpcConfigOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
-
 class VpcConfigOutputTypeDef(_RequiredVpcConfigOutputTypeDef, _OptionalVpcConfigOutputTypeDef):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1463,231 +999,332 @@
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "TargetNumberOfBrokerNodes": int,
     },
 )
 
-UpdateBrokerCountResponseTypeDef = TypedDict(
-    "UpdateBrokerCountResponseTypeDef",
+UpdateBrokerTypeRequestRequestTypeDef = TypedDict(
+    "UpdateBrokerTypeRequestRequestTypeDef",
     {
         "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CurrentVersion": str,
+        "TargetInstanceType": str,
     },
 )
 
-UpdateBrokerStorageResponseTypeDef = TypedDict(
-    "UpdateBrokerStorageResponseTypeDef",
+_RequiredUpdateConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConfigurationRequestRequestTypeDef",
     {
-        "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Arn": str,
+        "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
+    },
+)
+_OptionalUpdateConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class UpdateConfigurationRequestRequestTypeDef(
+    _RequiredUpdateConfigurationRequestRequestTypeDef,
+    _OptionalUpdateConfigurationRequestRequestTypeDef,
+):
+    pass
+
+UserIdentityTypeDef = TypedDict(
+    "UserIdentityTypeDef",
+    {
+        "Type": UserIdentityTypeType,
+        "PrincipalId": str,
     },
+    total=False,
 )
 
-UpdateBrokerTypeRequestRequestTypeDef = TypedDict(
-    "UpdateBrokerTypeRequestRequestTypeDef",
+VpcConnectivityTlsTypeDef = TypedDict(
+    "VpcConnectivityTlsTypeDef",
     {
-        "ClusterArn": str,
-        "CurrentVersion": str,
-        "TargetInstanceType": str,
+        "Enabled": bool,
     },
+    total=False,
 )
 
-UpdateBrokerTypeResponseTypeDef = TypedDict(
-    "UpdateBrokerTypeResponseTypeDef",
+VpcConnectivityIamTypeDef = TypedDict(
+    "VpcConnectivityIamTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+VpcConnectivityScramTypeDef = TypedDict(
+    "VpcConnectivityScramTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+CreateClusterResponseTypeDef = TypedDict(
+    "CreateClusterResponseTypeDef",
     {
         "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterName": str,
+        "State": ClusterStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateClusterConfigurationResponseTypeDef = TypedDict(
-    "UpdateClusterConfigurationResponseTypeDef",
+CreateClusterV2ResponseTypeDef = TypedDict(
+    "CreateClusterV2ResponseTypeDef",
     {
         "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterName": str,
+        "State": ClusterStateType,
+        "ClusterType": ClusterTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateClusterKafkaVersionResponseTypeDef = TypedDict(
-    "UpdateClusterKafkaVersionResponseTypeDef",
+CreateVpcConnectionResponseTypeDef = TypedDict(
+    "CreateVpcConnectionResponseTypeDef",
+    {
+        "VpcConnectionArn": str,
+        "State": VpcConnectionStateType,
+        "Authentication": str,
+        "VpcId": str,
+        "ClientSubnets": List[str],
+        "SecurityGroups": List[str],
+        "CreationTime": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteClusterResponseTypeDef = TypedDict(
+    "DeleteClusterResponseTypeDef",
     {
         "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "State": ClusterStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConfigurationRequestRequestTypeDef",
+DeleteConfigurationResponseTypeDef = TypedDict(
+    "DeleteConfigurationResponseTypeDef",
     {
         "Arn": str,
-        "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
+        "State": ConfigurationStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConfigurationRequestRequestTypeDef",
+
+DeleteVpcConnectionResponseTypeDef = TypedDict(
+    "DeleteVpcConnectionResponseTypeDef",
     {
+        "VpcConnectionArn": str,
+        "State": VpcConnectionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeConfigurationRevisionResponseTypeDef = TypedDict(
+    "DescribeConfigurationRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
         "Description": str,
+        "Revision": int,
+        "ServerProperties": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+DescribeVpcConnectionResponseTypeDef = TypedDict(
+    "DescribeVpcConnectionResponseTypeDef",
+    {
+        "VpcConnectionArn": str,
+        "TargetClusterArn": str,
+        "State": VpcConnectionStateType,
+        "Authentication": str,
+        "VpcId": str,
+        "Subnets": List[str],
+        "SecurityGroups": List[str],
+        "CreationTime": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateConfigurationRequestRequestTypeDef(
-    _RequiredUpdateConfigurationRequestRequestTypeDef,
-    _OptionalUpdateConfigurationRequestRequestTypeDef,
-):
-    pass
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GetBootstrapBrokersResponseTypeDef = TypedDict(
+    "GetBootstrapBrokersResponseTypeDef",
+    {
+        "BootstrapBrokerString": str,
+        "BootstrapBrokerStringTls": str,
+        "BootstrapBrokerStringSaslScram": str,
+        "BootstrapBrokerStringSaslIam": str,
+        "BootstrapBrokerStringPublicTls": str,
+        "BootstrapBrokerStringPublicSaslScram": str,
+        "BootstrapBrokerStringPublicSaslIam": str,
+        "BootstrapBrokerStringVpcConnectivityTls": str,
+        "BootstrapBrokerStringVpcConnectivitySaslScram": str,
+        "BootstrapBrokerStringVpcConnectivitySaslIam": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateConnectivityResponseTypeDef = TypedDict(
-    "UpdateConnectivityResponseTypeDef",
+GetClusterPolicyResponseTypeDef = TypedDict(
+    "GetClusterPolicyResponseTypeDef",
     {
-        "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CurrentVersion": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateMonitoringResponseTypeDef = TypedDict(
-    "UpdateMonitoringResponseTypeDef",
+ListScramSecretsResponseTypeDef = TypedDict(
+    "ListScramSecretsResponseTypeDef",
+    {
+        "NextToken": str,
+        "SecretArnList": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutClusterPolicyResponseTypeDef = TypedDict(
+    "PutClusterPolicyResponseTypeDef",
+    {
+        "CurrentVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RebootBrokerResponseTypeDef = TypedDict(
+    "RebootBrokerResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSecurityResponseTypeDef = TypedDict(
-    "UpdateSecurityResponseTypeDef",
+UpdateBrokerCountResponseTypeDef = TypedDict(
+    "UpdateBrokerCountResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateStorageResponseTypeDef = TypedDict(
-    "UpdateStorageResponseTypeDef",
+UpdateBrokerStorageResponseTypeDef = TypedDict(
+    "UpdateBrokerStorageResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserIdentityTypeDef = TypedDict(
-    "UserIdentityTypeDef",
+UpdateBrokerTypeResponseTypeDef = TypedDict(
+    "UpdateBrokerTypeResponseTypeDef",
     {
-        "Type": UserIdentityTypeType,
-        "PrincipalId": str,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VpcConnectivityTlsOutputTypeDef = TypedDict(
-    "VpcConnectivityTlsOutputTypeDef",
+UpdateClusterConfigurationResponseTypeDef = TypedDict(
+    "UpdateClusterConfigurationResponseTypeDef",
     {
-        "Enabled": bool,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VpcConnectivityTlsTypeDef = TypedDict(
-    "VpcConnectivityTlsTypeDef",
+UpdateClusterKafkaVersionResponseTypeDef = TypedDict(
+    "UpdateClusterKafkaVersionResponseTypeDef",
     {
-        "Enabled": bool,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VpcConnectivityIamOutputTypeDef = TypedDict(
-    "VpcConnectivityIamOutputTypeDef",
+UpdateConnectivityResponseTypeDef = TypedDict(
+    "UpdateConnectivityResponseTypeDef",
     {
-        "Enabled": bool,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VpcConnectivityIamTypeDef = TypedDict(
-    "VpcConnectivityIamTypeDef",
+UpdateMonitoringResponseTypeDef = TypedDict(
+    "UpdateMonitoringResponseTypeDef",
     {
-        "Enabled": bool,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VpcConnectivityScramOutputTypeDef = TypedDict(
-    "VpcConnectivityScramOutputTypeDef",
+UpdateSecurityResponseTypeDef = TypedDict(
+    "UpdateSecurityResponseTypeDef",
     {
-        "Enabled": bool,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VpcConnectivityScramTypeDef = TypedDict(
-    "VpcConnectivityScramTypeDef",
+UpdateStorageResponseTypeDef = TypedDict(
+    "UpdateStorageResponseTypeDef",
     {
-        "Enabled": bool,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 BatchAssociateScramSecretResponseTypeDef = TypedDict(
     "BatchAssociateScramSecretResponseTypeDef",
     {
         "ClusterArn": str,
         "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateScramSecretResponseTypeDef = TypedDict(
     "BatchDisassociateScramSecretResponseTypeDef",
     {
         "ClusterArn": str,
         "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredBrokerEBSVolumeInfoOutputTypeDef = TypedDict(
-    "_RequiredBrokerEBSVolumeInfoOutputTypeDef",
-    {
-        "KafkaBrokerNodeId": str,
-    },
-)
-_OptionalBrokerEBSVolumeInfoOutputTypeDef = TypedDict(
-    "_OptionalBrokerEBSVolumeInfoOutputTypeDef",
-    {
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
-        "VolumeSizeGB": int,
-    },
-    total=False,
-)
-
-
-class BrokerEBSVolumeInfoOutputTypeDef(
-    _RequiredBrokerEBSVolumeInfoOutputTypeDef, _OptionalBrokerEBSVolumeInfoOutputTypeDef
-):
-    pass
-
-
-EBSStorageInfoOutputTypeDef = TypedDict(
-    "EBSStorageInfoOutputTypeDef",
-    {
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
-        "VolumeSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredBrokerEBSVolumeInfoTypeDef = TypedDict(
     "_RequiredBrokerEBSVolumeInfoTypeDef",
     {
         "KafkaBrokerNodeId": str,
     },
@@ -1697,21 +1334,19 @@
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "VolumeSizeGB": int,
     },
     total=False,
 )
 
-
 class BrokerEBSVolumeInfoTypeDef(
     _RequiredBrokerEBSVolumeInfoTypeDef, _OptionalBrokerEBSVolumeInfoTypeDef
 ):
     pass
 
-
 EBSStorageInfoTypeDef = TypedDict(
     "EBSStorageInfoTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "VolumeSize": int,
     },
     total=False,
@@ -1730,31 +1365,19 @@
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "StorageMode": StorageModeType,
         "VolumeSizeGB": int,
     },
     total=False,
 )
 
-
 class UpdateStorageRequestRequestTypeDef(
     _RequiredUpdateStorageRequestRequestTypeDef, _OptionalUpdateStorageRequestRequestTypeDef
 ):
     pass
 
-
-BrokerLogsOutputTypeDef = TypedDict(
-    "BrokerLogsOutputTypeDef",
-    {
-        "CloudWatchLogs": CloudWatchLogsOutputTypeDef,
-        "Firehose": FirehoseOutputTypeDef,
-        "S3": S3OutputTypeDef,
-    },
-    total=False,
-)
-
 BrokerLogsTypeDef = TypedDict(
     "BrokerLogsTypeDef",
     {
         "CloudWatchLogs": CloudWatchLogsTypeDef,
         "Firehose": FirehoseTypeDef,
         "S3": S3TypeDef,
     },
@@ -1775,32 +1398,41 @@
 )
 
 ListClientVpcConnectionsResponseTypeDef = TypedDict(
     "ListClientVpcConnectionsResponseTypeDef",
     {
         "ClientVpcConnections": List[ClientVpcConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterOperationStepTypeDef = TypedDict(
     "ClusterOperationStepTypeDef",
     {
         "StepInfo": ClusterOperationStepInfoTypeDef,
         "StepName": str,
     },
     total=False,
 )
 
+ListClusterOperationsV2ResponseTypeDef = TypedDict(
+    "ListClusterOperationsV2ResponseTypeDef",
+    {
+        "ClusterOperationInfoList": List[ClusterOperationV2SummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetCompatibleKafkaVersionsResponseTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsResponseTypeDef",
     {
         "CompatibleKafkaVersions": List[CompatibleKafkaVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateClusterConfigurationRequestRequestTypeDef",
     {
         "ClusterArn": str,
@@ -1821,22 +1453,20 @@
     "_OptionalUpdateClusterKafkaVersionRequestRequestTypeDef",
     {
         "ConfigurationInfo": ConfigurationInfoTypeDef,
     },
     total=False,
 )
 
-
 class UpdateClusterKafkaVersionRequestRequestTypeDef(
     _RequiredUpdateClusterKafkaVersionRequestRequestTypeDef,
     _OptionalUpdateClusterKafkaVersionRequestRequestTypeDef,
 ):
     pass
 
-
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "Description": str,
         "KafkaVersions": List[str],
@@ -1850,111 +1480,248 @@
     "CreateConfigurationResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "LatestRevision": ConfigurationRevisionTypeDef,
         "Name": str,
         "State": ConfigurationStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConfigurationResponseTypeDef = TypedDict(
     "DescribeConfigurationResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "Description": str,
         "KafkaVersions": List[str],
         "LatestRevision": ConfigurationRevisionTypeDef,
         "Name": str,
         "State": ConfigurationStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfigurationRevisionsResponseTypeDef = TypedDict(
     "ListConfigurationRevisionsResponseTypeDef",
     {
         "NextToken": str,
         "Revisions": List[ConfigurationRevisionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfigurationResponseTypeDef = TypedDict(
     "UpdateConfigurationResponseTypeDef",
     {
         "Arn": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EncryptionInfoOutputTypeDef = TypedDict(
-    "EncryptionInfoOutputTypeDef",
-    {
-        "EncryptionAtRest": EncryptionAtRestOutputTypeDef,
-        "EncryptionInTransit": EncryptionInTransitOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 EncryptionInfoTypeDef = TypedDict(
     "EncryptionInfoTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "EncryptionInTransit": EncryptionInTransitTypeDef,
     },
     total=False,
 )
 
-ServerlessSaslOutputTypeDef = TypedDict(
-    "ServerlessSaslOutputTypeDef",
-    {
-        "Iam": IamOutputTypeDef,
-    },
-    total=False,
-)
-
 ServerlessSaslTypeDef = TypedDict(
     "ServerlessSaslTypeDef",
     {
         "Iam": IamTypeDef,
     },
     total=False,
 )
 
 ListKafkaVersionsResponseTypeDef = TypedDict(
     "ListKafkaVersionsResponseTypeDef",
     {
         "KafkaVersions": List[KafkaVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListVpcConnectionsResponseTypeDef = TypedDict(
-    "ListVpcConnectionsResponseTypeDef",
+_RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
+    "_RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     {
-        "VpcConnections": List[VpcConnectionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterArn": str,
+    },
+)
+_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
+    "_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef(
+    _RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+    _OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListClusterOperationsRequestListClusterOperationsPaginateTypeDef(
+    _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
+    _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
+):
+    pass
+
+_RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef = TypedDict(
+    "_RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef = TypedDict(
+    "_OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef(
+    _RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
+    _OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
+):
+    pass
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "ClusterNameFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListClustersV2RequestListClustersV2PaginateTypeDef = TypedDict(
+    "ListClustersV2RequestListClustersV2PaginateTypeDef",
+    {
+        "ClusterNameFilter": str,
+        "ClusterTypeFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-PrometheusInfoOutputTypeDef = TypedDict(
-    "PrometheusInfoOutputTypeDef",
+_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
     {
-        "JmxExporter": JmxExporterInfoOutputTypeDef,
-        "NodeExporter": NodeExporterInfoOutputTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef(
+    _RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
+    _OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
+):
+    pass
+
+ListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
+    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef = TypedDict(
+    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListNodesRequestListNodesPaginateTypeDef = TypedDict(
+    "_RequiredListNodesRequestListNodesPaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListNodesRequestListNodesPaginateTypeDef = TypedDict(
+    "_OptionalListNodesRequestListNodesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListNodesRequestListNodesPaginateTypeDef(
+    _RequiredListNodesRequestListNodesPaginateTypeDef,
+    _OptionalListNodesRequestListNodesPaginateTypeDef,
+):
+    pass
+
+_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
+    "_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
+    "_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListScramSecretsRequestListScramSecretsPaginateTypeDef(
+    _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef,
+    _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef,
+):
+    pass
+
+ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef = TypedDict(
+    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListVpcConnectionsResponseTypeDef = TypedDict(
+    "ListVpcConnectionsResponseTypeDef",
+    {
+        "VpcConnections": List[VpcConnectionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PrometheusInfoTypeDef = TypedDict(
     "PrometheusInfoTypeDef",
     {
         "JmxExporter": JmxExporterInfoTypeDef,
         "NodeExporter": NodeExporterInfoTypeDef,
     },
     total=False,
@@ -1965,69 +1732,54 @@
     {
         "JmxExporter": JmxExporterTypeDef,
         "NodeExporter": NodeExporterTypeDef,
     },
     total=False,
 )
 
-SaslOutputTypeDef = TypedDict(
-    "SaslOutputTypeDef",
-    {
-        "Scram": ScramOutputTypeDef,
-        "Iam": IamOutputTypeDef,
-    },
-    total=False,
-)
-
 SaslTypeDef = TypedDict(
     "SaslTypeDef",
     {
         "Scram": ScramTypeDef,
         "Iam": IamTypeDef,
     },
     total=False,
 )
 
-VpcConnectionInfoTypeDef = TypedDict(
-    "VpcConnectionInfoTypeDef",
+VpcConnectionInfoServerlessTypeDef = TypedDict(
+    "VpcConnectionInfoServerlessTypeDef",
     {
-        "VpcConnectionArn": str,
+        "CreationTime": datetime,
         "Owner": str,
         "UserIdentity": UserIdentityTypeDef,
-        "CreationTime": datetime,
+        "VpcConnectionArn": str,
     },
     total=False,
 )
 
-VpcConnectivitySaslOutputTypeDef = TypedDict(
-    "VpcConnectivitySaslOutputTypeDef",
+VpcConnectionInfoTypeDef = TypedDict(
+    "VpcConnectionInfoTypeDef",
     {
-        "Scram": VpcConnectivityScramOutputTypeDef,
-        "Iam": VpcConnectivityIamOutputTypeDef,
+        "VpcConnectionArn": str,
+        "Owner": str,
+        "UserIdentity": UserIdentityTypeDef,
+        "CreationTime": datetime,
     },
     total=False,
 )
 
 VpcConnectivitySaslTypeDef = TypedDict(
     "VpcConnectivitySaslTypeDef",
     {
         "Scram": VpcConnectivityScramTypeDef,
         "Iam": VpcConnectivityIamTypeDef,
     },
     total=False,
 )
 
-StorageInfoOutputTypeDef = TypedDict(
-    "StorageInfoOutputTypeDef",
-    {
-        "EbsStorageInfo": EBSStorageInfoOutputTypeDef,
-    },
-    total=False,
-)
-
 UpdateBrokerStorageRequestRequestTypeDef = TypedDict(
     "UpdateBrokerStorageRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "TargetBrokerEBSVolumeInfo": Sequence[BrokerEBSVolumeInfoTypeDef],
     },
@@ -2037,21 +1789,14 @@
     "StorageInfoTypeDef",
     {
         "EbsStorageInfo": EBSStorageInfoTypeDef,
     },
     total=False,
 )
 
-LoggingInfoOutputTypeDef = TypedDict(
-    "LoggingInfoOutputTypeDef",
-    {
-        "BrokerLogs": BrokerLogsOutputTypeDef,
-    },
-)
-
 LoggingInfoTypeDef = TypedDict(
     "LoggingInfoTypeDef",
     {
         "BrokerLogs": BrokerLogsTypeDef,
     },
 )
 
@@ -2069,41 +1814,26 @@
 )
 
 ListConfigurationsResponseTypeDef = TypedDict(
     "ListConfigurationsResponseTypeDef",
     {
         "Configurations": List[ConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ServerlessClientAuthenticationOutputTypeDef = TypedDict(
-    "ServerlessClientAuthenticationOutputTypeDef",
-    {
-        "Sasl": ServerlessSaslOutputTypeDef,
-    },
-    total=False,
-)
-
 ServerlessClientAuthenticationTypeDef = TypedDict(
     "ServerlessClientAuthenticationTypeDef",
     {
         "Sasl": ServerlessSaslTypeDef,
     },
     total=False,
 )
 
-OpenMonitoringInfoOutputTypeDef = TypedDict(
-    "OpenMonitoringInfoOutputTypeDef",
-    {
-        "Prometheus": PrometheusInfoOutputTypeDef,
-    },
-)
-
 OpenMonitoringInfoTypeDef = TypedDict(
     "OpenMonitoringInfoTypeDef",
     {
         "Prometheus": PrometheusInfoTypeDef,
     },
 )
 
@@ -2113,36 +1843,35 @@
         "Prometheus": PrometheusTypeDef,
     },
 )
 
 ClientAuthenticationOutputTypeDef = TypedDict(
     "ClientAuthenticationOutputTypeDef",
     {
-        "Sasl": SaslOutputTypeDef,
+        "Sasl": SaslTypeDef,
         "Tls": TlsOutputTypeDef,
-        "Unauthenticated": UnauthenticatedOutputTypeDef,
+        "Unauthenticated": UnauthenticatedTypeDef,
     },
     total=False,
 )
 
 ClientAuthenticationTypeDef = TypedDict(
     "ClientAuthenticationTypeDef",
     {
         "Sasl": SaslTypeDef,
         "Tls": TlsTypeDef,
         "Unauthenticated": UnauthenticatedTypeDef,
     },
     total=False,
 )
 
-VpcConnectivityClientAuthenticationOutputTypeDef = TypedDict(
-    "VpcConnectivityClientAuthenticationOutputTypeDef",
+ClusterOperationV2ServerlessTypeDef = TypedDict(
+    "ClusterOperationV2ServerlessTypeDef",
     {
-        "Sasl": VpcConnectivitySaslOutputTypeDef,
-        "Tls": VpcConnectivityTlsOutputTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoServerlessTypeDef,
     },
     total=False,
 )
 
 VpcConnectivityClientAuthenticationTypeDef = TypedDict(
     "VpcConnectivityClientAuthenticationTypeDef",
     {
@@ -2153,58 +1882,54 @@
 )
 
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
         "NextToken": str,
         "NodeInfoList": List[NodeInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredServerlessTypeDef = TypedDict(
-    "_RequiredServerlessTypeDef",
+_RequiredServerlessRequestTypeDef = TypedDict(
+    "_RequiredServerlessRequestTypeDef",
     {
-        "VpcConfigs": List[VpcConfigOutputTypeDef],
+        "VpcConfigs": Sequence[VpcConfigTypeDef],
     },
 )
-_OptionalServerlessTypeDef = TypedDict(
-    "_OptionalServerlessTypeDef",
+_OptionalServerlessRequestTypeDef = TypedDict(
+    "_OptionalServerlessRequestTypeDef",
     {
-        "ClientAuthentication": ServerlessClientAuthenticationOutputTypeDef,
+        "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
     },
     total=False,
 )
 
-
-class ServerlessTypeDef(_RequiredServerlessTypeDef, _OptionalServerlessTypeDef):
+class ServerlessRequestTypeDef(
+    _RequiredServerlessRequestTypeDef, _OptionalServerlessRequestTypeDef
+):
     pass
 
-
-_RequiredServerlessRequestTypeDef = TypedDict(
-    "_RequiredServerlessRequestTypeDef",
+_RequiredServerlessTypeDef = TypedDict(
+    "_RequiredServerlessTypeDef",
     {
-        "VpcConfigs": Sequence[VpcConfigTypeDef],
+        "VpcConfigs": List[VpcConfigOutputTypeDef],
     },
 )
-_OptionalServerlessRequestTypeDef = TypedDict(
-    "_OptionalServerlessRequestTypeDef",
+_OptionalServerlessTypeDef = TypedDict(
+    "_OptionalServerlessTypeDef",
     {
         "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
     },
     total=False,
 )
 
-
-class ServerlessRequestTypeDef(
-    _RequiredServerlessRequestTypeDef, _OptionalServerlessRequestTypeDef
-):
+class ServerlessTypeDef(_RequiredServerlessTypeDef, _OptionalServerlessTypeDef):
     pass
 
-
 _RequiredUpdateMonitoringRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitoringRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
     },
 )
@@ -2214,21 +1939,19 @@
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringInfoTypeDef,
         "LoggingInfo": LoggingInfoTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMonitoringRequestRequestTypeDef(
     _RequiredUpdateMonitoringRequestRequestTypeDef, _OptionalUpdateMonitoringRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
     },
 )
@@ -2237,46 +1960,27 @@
     {
         "ClientAuthentication": ClientAuthenticationTypeDef,
         "EncryptionInfo": EncryptionInfoTypeDef,
     },
     total=False,
 )
 
-
 class UpdateSecurityRequestRequestTypeDef(
     _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
 ):
     pass
 
-
-VpcConnectivityOutputTypeDef = TypedDict(
-    "VpcConnectivityOutputTypeDef",
-    {
-        "ClientAuthentication": VpcConnectivityClientAuthenticationOutputTypeDef,
-    },
-    total=False,
-)
-
 VpcConnectivityTypeDef = TypedDict(
     "VpcConnectivityTypeDef",
     {
         "ClientAuthentication": VpcConnectivityClientAuthenticationTypeDef,
     },
     total=False,
 )
 
-ConnectivityInfoOutputTypeDef = TypedDict(
-    "ConnectivityInfoOutputTypeDef",
-    {
-        "PublicAccess": PublicAccessOutputTypeDef,
-        "VpcConnectivity": VpcConnectivityOutputTypeDef,
-    },
-    total=False,
-)
-
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "PublicAccess": PublicAccessTypeDef,
         "VpcConnectivity": VpcConnectivityTypeDef,
     },
     total=False,
@@ -2290,47 +1994,26 @@
     },
 )
 _OptionalBrokerNodeGroupInfoOutputTypeDef = TypedDict(
     "_OptionalBrokerNodeGroupInfoOutputTypeDef",
     {
         "BrokerAZDistribution": Literal["DEFAULT"],
         "SecurityGroups": List[str],
-        "StorageInfo": StorageInfoOutputTypeDef,
-        "ConnectivityInfo": ConnectivityInfoOutputTypeDef,
+        "StorageInfo": StorageInfoTypeDef,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
         "ZoneIds": List[str],
     },
     total=False,
 )
 
-
 class BrokerNodeGroupInfoOutputTypeDef(
     _RequiredBrokerNodeGroupInfoOutputTypeDef, _OptionalBrokerNodeGroupInfoOutputTypeDef
 ):
     pass
 
-
-MutableClusterInfoTypeDef = TypedDict(
-    "MutableClusterInfoTypeDef",
-    {
-        "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoOutputTypeDef],
-        "ConfigurationInfo": ConfigurationInfoOutputTypeDef,
-        "NumberOfBrokerNodes": int,
-        "EnhancedMonitoring": EnhancedMonitoringType,
-        "OpenMonitoring": OpenMonitoringTypeDef,
-        "KafkaVersion": str,
-        "LoggingInfo": LoggingInfoOutputTypeDef,
-        "InstanceType": str,
-        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
-        "EncryptionInfo": EncryptionInfoOutputTypeDef,
-        "ConnectivityInfo": ConnectivityInfoOutputTypeDef,
-        "StorageMode": StorageModeType,
-    },
-    total=False,
-)
-
 _RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
     "_RequiredBrokerNodeGroupInfoTypeDef",
     {
         "ClientSubnets": Sequence[str],
         "InstanceType": str,
     },
 )
@@ -2342,20 +2025,37 @@
         "StorageInfo": StorageInfoTypeDef,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "ZoneIds": Sequence[str],
     },
     total=False,
 )
 
-
 class BrokerNodeGroupInfoTypeDef(
     _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
 ):
     pass
 
+MutableClusterInfoTypeDef = TypedDict(
+    "MutableClusterInfoTypeDef",
+    {
+        "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoTypeDef],
+        "ConfigurationInfo": ConfigurationInfoTypeDef,
+        "NumberOfBrokerNodes": int,
+        "EnhancedMonitoring": EnhancedMonitoringType,
+        "OpenMonitoring": OpenMonitoringTypeDef,
+        "KafkaVersion": str,
+        "LoggingInfo": LoggingInfoTypeDef,
+        "InstanceType": str,
+        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
+        "EncryptionInfo": EncryptionInfoTypeDef,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
+        "StorageMode": StorageModeType,
+    },
+    total=False,
+)
 
 UpdateConnectivityRequestRequestTypeDef = TypedDict(
     "UpdateConnectivityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "CurrentVersion": str,
@@ -2369,18 +2069,18 @@
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoOutputTypeDef,
         "ClientAuthentication": ClientAuthenticationOutputTypeDef,
         "ClusterArn": str,
         "ClusterName": str,
         "CreationTime": datetime,
         "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
         "CurrentVersion": str,
-        "EncryptionInfo": EncryptionInfoOutputTypeDef,
+        "EncryptionInfo": EncryptionInfoTypeDef,
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringTypeDef,
-        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "LoggingInfo": LoggingInfoTypeDef,
         "NumberOfBrokerNodes": int,
         "State": ClusterStateType,
         "StateInfo": StateInfoTypeDef,
         "Tags": Dict[str, str],
         "ZookeeperConnectString": str,
         "ZookeeperConnectStringTls": str,
         "StorageMode": StorageModeType,
@@ -2396,49 +2096,28 @@
     },
 )
 _OptionalProvisionedTypeDef = TypedDict(
     "_OptionalProvisionedTypeDef",
     {
         "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
         "ClientAuthentication": ClientAuthenticationOutputTypeDef,
-        "EncryptionInfo": EncryptionInfoOutputTypeDef,
+        "EncryptionInfo": EncryptionInfoTypeDef,
         "EnhancedMonitoring": EnhancedMonitoringType,
-        "OpenMonitoring": OpenMonitoringInfoOutputTypeDef,
-        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "OpenMonitoring": OpenMonitoringInfoTypeDef,
+        "LoggingInfo": LoggingInfoTypeDef,
         "ZookeeperConnectString": str,
         "ZookeeperConnectStringTls": str,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
-
 class ProvisionedTypeDef(_RequiredProvisionedTypeDef, _OptionalProvisionedTypeDef):
     pass
 
-
-ClusterOperationInfoTypeDef = TypedDict(
-    "ClusterOperationInfoTypeDef",
-    {
-        "ClientRequestId": str,
-        "ClusterArn": str,
-        "CreationTime": datetime,
-        "EndTime": datetime,
-        "ErrorInfo": ErrorInfoTypeDef,
-        "OperationArn": str,
-        "OperationState": str,
-        "OperationSteps": List[ClusterOperationStepTypeDef],
-        "OperationType": str,
-        "SourceClusterInfo": MutableClusterInfoTypeDef,
-        "TargetClusterInfo": MutableClusterInfoTypeDef,
-        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "ClusterName": str,
         "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
@@ -2455,21 +2134,19 @@
         "LoggingInfo": LoggingInfoTypeDef,
         "Tags": Mapping[str, str],
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
-
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredProvisionedRequestTypeDef = TypedDict(
     "_RequiredProvisionedRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
     },
@@ -2484,35 +2161,63 @@
         "OpenMonitoring": OpenMonitoringInfoTypeDef,
         "LoggingInfo": LoggingInfoTypeDef,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
-
 class ProvisionedRequestTypeDef(
     _RequiredProvisionedRequestTypeDef, _OptionalProvisionedRequestTypeDef
 ):
     pass
 
+ClusterOperationInfoTypeDef = TypedDict(
+    "ClusterOperationInfoTypeDef",
+    {
+        "ClientRequestId": str,
+        "ClusterArn": str,
+        "CreationTime": datetime,
+        "EndTime": datetime,
+        "ErrorInfo": ErrorInfoTypeDef,
+        "OperationArn": str,
+        "OperationState": str,
+        "OperationSteps": List[ClusterOperationStepTypeDef],
+        "OperationType": str,
+        "SourceClusterInfo": MutableClusterInfoTypeDef,
+        "TargetClusterInfo": MutableClusterInfoTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
+    },
+    total=False,
+)
+
+ClusterOperationV2ProvisionedTypeDef = TypedDict(
+    "ClusterOperationV2ProvisionedTypeDef",
+    {
+        "OperationSteps": List[ClusterOperationStepTypeDef],
+        "SourceClusterInfo": MutableClusterInfoTypeDef,
+        "TargetClusterInfo": MutableClusterInfoTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
+    },
+    total=False,
+)
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "ClusterInfo": ClusterInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListClustersResponseTypeDef = TypedDict(
     "ListClustersResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ActiveOperationArn": str,
@@ -2526,31 +2231,14 @@
         "Tags": Dict[str, str],
         "Provisioned": ProvisionedTypeDef,
         "Serverless": ServerlessTypeDef,
     },
     total=False,
 )
 
-DescribeClusterOperationResponseTypeDef = TypedDict(
-    "DescribeClusterOperationResponseTypeDef",
-    {
-        "ClusterOperationInfo": ClusterOperationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListClusterOperationsResponseTypeDef = TypedDict(
-    "ListClusterOperationsResponseTypeDef",
-    {
-        "ClusterOperationInfoList": List[ClusterOperationInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateClusterV2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterV2RequestRequestTypeDef",
     {
         "ClusterName": str,
     },
 )
 _OptionalCreateClusterV2RequestRequestTypeDef = TypedDict(
@@ -2559,30 +2247,70 @@
         "Tags": Mapping[str, str],
         "Provisioned": ProvisionedRequestTypeDef,
         "Serverless": ServerlessRequestTypeDef,
     },
     total=False,
 )
 
-
 class CreateClusterV2RequestRequestTypeDef(
     _RequiredCreateClusterV2RequestRequestTypeDef, _OptionalCreateClusterV2RequestRequestTypeDef
 ):
     pass
 
+DescribeClusterOperationResponseTypeDef = TypedDict(
+    "DescribeClusterOperationResponseTypeDef",
+    {
+        "ClusterOperationInfo": ClusterOperationInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClusterOperationsResponseTypeDef = TypedDict(
+    "ListClusterOperationsResponseTypeDef",
+    {
+        "ClusterOperationInfoList": List[ClusterOperationInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterOperationV2TypeDef = TypedDict(
+    "ClusterOperationV2TypeDef",
+    {
+        "ClusterArn": str,
+        "ClusterType": ClusterTypeType,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ErrorInfo": ErrorInfoTypeDef,
+        "OperationArn": str,
+        "OperationState": str,
+        "OperationType": str,
+        "Provisioned": ClusterOperationV2ProvisionedTypeDef,
+        "Serverless": ClusterOperationV2ServerlessTypeDef,
+    },
+    total=False,
+)
 
 DescribeClusterV2ResponseTypeDef = TypedDict(
     "DescribeClusterV2ResponseTypeDef",
     {
         "ClusterInfo": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListClustersV2ResponseTypeDef = TypedDict(
     "ListClustersV2ResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeClusterOperationV2ResponseTypeDef = TypedDict(
+    "DescribeClusterOperationV2ResponseTypeDef",
+    {
+        "ClusterOperationInfo": ClusterOperationV2TypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka/type_defs.pyi` & `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,223 +34,214 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BatchAssociateScramSecretRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedScramSecretTypeDef",
     "BatchDisassociateScramSecretRequestRequestTypeDef",
-    "ProvisionedThroughputOutputTypeDef",
     "ProvisionedThroughputTypeDef",
-    "CloudWatchLogsOutputTypeDef",
-    "FirehoseOutputTypeDef",
-    "S3OutputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
     "TlsOutputTypeDef",
-    "UnauthenticatedOutputTypeDef",
-    "TlsTypeDef",
     "UnauthenticatedTypeDef",
+    "TlsTypeDef",
     "ClientVpcConnectionTypeDef",
     "StateInfoTypeDef",
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
+    "ClusterOperationV2SummaryTypeDef",
     "CompatibleKafkaVersionTypeDef",
-    "ConfigurationInfoOutputTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
-    "PublicAccessOutputTypeDef",
     "PublicAccessTypeDef",
-    "CreateClusterResponseTypeDef",
-    "CreateClusterV2ResponseTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
     "CreateVpcConnectionRequestRequestTypeDef",
-    "CreateVpcConnectionResponseTypeDef",
     "DeleteClusterPolicyRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
-    "DeleteClusterResponseTypeDef",
     "DeleteConfigurationRequestRequestTypeDef",
-    "DeleteConfigurationResponseTypeDef",
     "DeleteVpcConnectionRequestRequestTypeDef",
-    "DeleteVpcConnectionResponseTypeDef",
     "DescribeClusterOperationRequestRequestTypeDef",
+    "DescribeClusterOperationV2RequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeClusterV2RequestRequestTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
-    "DescribeConfigurationRevisionResponseTypeDef",
     "DescribeVpcConnectionRequestRequestTypeDef",
-    "DescribeVpcConnectionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EncryptionAtRestOutputTypeDef",
     "EncryptionAtRestTypeDef",
-    "EncryptionInTransitOutputTypeDef",
     "EncryptionInTransitTypeDef",
     "GetBootstrapBrokersRequestRequestTypeDef",
-    "GetBootstrapBrokersResponseTypeDef",
     "GetClusterPolicyRequestRequestTypeDef",
-    "GetClusterPolicyResponseTypeDef",
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
-    "IamOutputTypeDef",
     "IamTypeDef",
-    "JmxExporterInfoOutputTypeDef",
     "JmxExporterInfoTypeDef",
     "JmxExporterTypeDef",
     "KafkaVersionTypeDef",
-    "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListClientVpcConnectionsRequestRequestTypeDef",
-    "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     "ListClusterOperationsRequestRequestTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListClusterOperationsV2RequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListClustersV2RequestListClustersV2PaginateTypeDef",
     "ListClustersV2RequestRequestTypeDef",
-    "ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
-    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
-    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
     "ListKafkaVersionsRequestRequestTypeDef",
-    "ListNodesRequestListNodesPaginateTypeDef",
     "ListNodesRequestRequestTypeDef",
-    "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
     "ListScramSecretsRequestRequestTypeDef",
-    "ListScramSecretsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     "ListVpcConnectionsRequestRequestTypeDef",
     "VpcConnectionTypeDef",
-    "NodeExporterInfoOutputTypeDef",
     "NodeExporterInfoTypeDef",
     "NodeExporterTypeDef",
     "ZookeeperNodeInfoTypeDef",
-    "PaginatorConfigTypeDef",
     "PutClusterPolicyRequestRequestTypeDef",
-    "PutClusterPolicyResponseTypeDef",
     "RebootBrokerRequestRequestTypeDef",
-    "RebootBrokerResponseTypeDef",
     "RejectClientVpcConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "ScramOutputTypeDef",
     "ScramTypeDef",
     "VpcConfigTypeDef",
     "VpcConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
+    "UpdateBrokerTypeRequestRequestTypeDef",
+    "UpdateConfigurationRequestRequestTypeDef",
+    "UserIdentityTypeDef",
+    "VpcConnectivityTlsTypeDef",
+    "VpcConnectivityIamTypeDef",
+    "VpcConnectivityScramTypeDef",
+    "CreateClusterResponseTypeDef",
+    "CreateClusterV2ResponseTypeDef",
+    "CreateVpcConnectionResponseTypeDef",
+    "DeleteClusterResponseTypeDef",
+    "DeleteConfigurationResponseTypeDef",
+    "DeleteVpcConnectionResponseTypeDef",
+    "DescribeConfigurationRevisionResponseTypeDef",
+    "DescribeVpcConnectionResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetBootstrapBrokersResponseTypeDef",
+    "GetClusterPolicyResponseTypeDef",
+    "ListScramSecretsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutClusterPolicyResponseTypeDef",
+    "RebootBrokerResponseTypeDef",
     "UpdateBrokerCountResponseTypeDef",
     "UpdateBrokerStorageResponseTypeDef",
-    "UpdateBrokerTypeRequestRequestTypeDef",
     "UpdateBrokerTypeResponseTypeDef",
     "UpdateClusterConfigurationResponseTypeDef",
     "UpdateClusterKafkaVersionResponseTypeDef",
-    "UpdateConfigurationRequestRequestTypeDef",
     "UpdateConnectivityResponseTypeDef",
     "UpdateMonitoringResponseTypeDef",
     "UpdateSecurityResponseTypeDef",
     "UpdateStorageResponseTypeDef",
-    "UserIdentityTypeDef",
-    "VpcConnectivityTlsOutputTypeDef",
-    "VpcConnectivityTlsTypeDef",
-    "VpcConnectivityIamOutputTypeDef",
-    "VpcConnectivityIamTypeDef",
-    "VpcConnectivityScramOutputTypeDef",
-    "VpcConnectivityScramTypeDef",
     "BatchAssociateScramSecretResponseTypeDef",
     "BatchDisassociateScramSecretResponseTypeDef",
-    "BrokerEBSVolumeInfoOutputTypeDef",
-    "EBSStorageInfoOutputTypeDef",
     "BrokerEBSVolumeInfoTypeDef",
     "EBSStorageInfoTypeDef",
     "UpdateStorageRequestRequestTypeDef",
-    "BrokerLogsOutputTypeDef",
     "BrokerLogsTypeDef",
     "BrokerNodeInfoTypeDef",
     "ListClientVpcConnectionsResponseTypeDef",
     "ClusterOperationStepTypeDef",
+    "ListClusterOperationsV2ResponseTypeDef",
     "GetCompatibleKafkaVersionsResponseTypeDef",
     "UpdateClusterConfigurationRequestRequestTypeDef",
     "UpdateClusterKafkaVersionRequestRequestTypeDef",
     "ConfigurationTypeDef",
     "CreateConfigurationResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
     "UpdateConfigurationResponseTypeDef",
-    "EncryptionInfoOutputTypeDef",
     "EncryptionInfoTypeDef",
-    "ServerlessSaslOutputTypeDef",
     "ServerlessSaslTypeDef",
     "ListKafkaVersionsResponseTypeDef",
+    "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
+    "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
+    "ListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListClustersV2RequestListClustersV2PaginateTypeDef",
+    "ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
+    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
+    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
+    "ListNodesRequestListNodesPaginateTypeDef",
+    "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
+    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     "ListVpcConnectionsResponseTypeDef",
-    "PrometheusInfoOutputTypeDef",
     "PrometheusInfoTypeDef",
     "PrometheusTypeDef",
-    "SaslOutputTypeDef",
     "SaslTypeDef",
+    "VpcConnectionInfoServerlessTypeDef",
     "VpcConnectionInfoTypeDef",
-    "VpcConnectivitySaslOutputTypeDef",
     "VpcConnectivitySaslTypeDef",
-    "StorageInfoOutputTypeDef",
     "UpdateBrokerStorageRequestRequestTypeDef",
     "StorageInfoTypeDef",
-    "LoggingInfoOutputTypeDef",
     "LoggingInfoTypeDef",
     "NodeInfoTypeDef",
     "ListConfigurationsResponseTypeDef",
-    "ServerlessClientAuthenticationOutputTypeDef",
     "ServerlessClientAuthenticationTypeDef",
-    "OpenMonitoringInfoOutputTypeDef",
     "OpenMonitoringInfoTypeDef",
     "OpenMonitoringTypeDef",
     "ClientAuthenticationOutputTypeDef",
     "ClientAuthenticationTypeDef",
-    "VpcConnectivityClientAuthenticationOutputTypeDef",
+    "ClusterOperationV2ServerlessTypeDef",
     "VpcConnectivityClientAuthenticationTypeDef",
     "ListNodesResponseTypeDef",
-    "ServerlessTypeDef",
     "ServerlessRequestTypeDef",
+    "ServerlessTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
     "UpdateSecurityRequestRequestTypeDef",
-    "VpcConnectivityOutputTypeDef",
     "VpcConnectivityTypeDef",
-    "ConnectivityInfoOutputTypeDef",
     "ConnectivityInfoTypeDef",
     "BrokerNodeGroupInfoOutputTypeDef",
-    "MutableClusterInfoTypeDef",
     "BrokerNodeGroupInfoTypeDef",
+    "MutableClusterInfoTypeDef",
     "UpdateConnectivityRequestRequestTypeDef",
     "ClusterInfoTypeDef",
     "ProvisionedTypeDef",
-    "ClusterOperationInfoTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ProvisionedRequestTypeDef",
+    "ClusterOperationInfoTypeDef",
+    "ClusterOperationV2ProvisionedTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
     "ClusterTypeDef",
+    "CreateClusterV2RequestRequestTypeDef",
     "DescribeClusterOperationResponseTypeDef",
     "ListClusterOperationsResponseTypeDef",
-    "CreateClusterV2RequestRequestTypeDef",
+    "ClusterOperationV2TypeDef",
     "DescribeClusterV2ResponseTypeDef",
     "ListClustersV2ResponseTypeDef",
+    "DescribeClusterOperationV2ResponseTypeDef",
 )
 
 BatchAssociateScramSecretRequestRequestTypeDef = TypedDict(
     "BatchAssociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 UnprocessedScramSecretTypeDef = TypedDict(
     "UnprocessedScramSecretTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "SecretArn": str,
     },
@@ -261,120 +252,61 @@
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
     },
 )
 
-ProvisionedThroughputOutputTypeDef = TypedDict(
-    "ProvisionedThroughputOutputTypeDef",
-    {
-        "Enabled": bool,
-        "VolumeThroughput": int,
-    },
-    total=False,
-)
-
 ProvisionedThroughputTypeDef = TypedDict(
     "ProvisionedThroughputTypeDef",
     {
         "Enabled": bool,
         "VolumeThroughput": int,
     },
     total=False,
 )
 
-_RequiredCloudWatchLogsOutputTypeDef = TypedDict(
-    "_RequiredCloudWatchLogsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalCloudWatchLogsOutputTypeDef = TypedDict(
-    "_OptionalCloudWatchLogsOutputTypeDef",
-    {
-        "LogGroup": str,
-    },
-    total=False,
-)
-
-class CloudWatchLogsOutputTypeDef(
-    _RequiredCloudWatchLogsOutputTypeDef, _OptionalCloudWatchLogsOutputTypeDef
-):
-    pass
-
-_RequiredFirehoseOutputTypeDef = TypedDict(
-    "_RequiredFirehoseOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalFirehoseOutputTypeDef = TypedDict(
-    "_OptionalFirehoseOutputTypeDef",
-    {
-        "DeliveryStream": str,
-    },
-    total=False,
-)
-
-class FirehoseOutputTypeDef(_RequiredFirehoseOutputTypeDef, _OptionalFirehoseOutputTypeDef):
-    pass
-
-_RequiredS3OutputTypeDef = TypedDict(
-    "_RequiredS3OutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalS3OutputTypeDef = TypedDict(
-    "_OptionalS3OutputTypeDef",
-    {
-        "Bucket": str,
-        "Prefix": str,
-    },
-    total=False,
-)
-
-class S3OutputTypeDef(_RequiredS3OutputTypeDef, _OptionalS3OutputTypeDef):
-    pass
-
 _RequiredCloudWatchLogsTypeDef = TypedDict(
     "_RequiredCloudWatchLogsTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalCloudWatchLogsTypeDef = TypedDict(
     "_OptionalCloudWatchLogsTypeDef",
     {
         "LogGroup": str,
     },
     total=False,
 )
 
+
 class CloudWatchLogsTypeDef(_RequiredCloudWatchLogsTypeDef, _OptionalCloudWatchLogsTypeDef):
     pass
 
+
 _RequiredFirehoseTypeDef = TypedDict(
     "_RequiredFirehoseTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalFirehoseTypeDef = TypedDict(
     "_OptionalFirehoseTypeDef",
     {
         "DeliveryStream": str,
     },
     total=False,
 )
 
+
 class FirehoseTypeDef(_RequiredFirehoseTypeDef, _OptionalFirehoseTypeDef):
     pass
 
+
 _RequiredS3TypeDef = TypedDict(
     "_RequiredS3TypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalS3TypeDef = TypedDict(
@@ -382,17 +314,19 @@
     {
         "Bucket": str,
         "Prefix": str,
     },
     total=False,
 )
 
+
 class S3TypeDef(_RequiredS3TypeDef, _OptionalS3TypeDef):
     pass
 
+
 BrokerSoftwareInfoTypeDef = TypedDict(
     "BrokerSoftwareInfoTypeDef",
     {
         "ConfigurationArn": str,
         "ConfigurationRevision": int,
         "KafkaVersion": str,
     },
@@ -404,16 +338,16 @@
     {
         "CertificateAuthorityArnList": List[str],
         "Enabled": bool,
     },
     total=False,
 )
 
-UnauthenticatedOutputTypeDef = TypedDict(
-    "UnauthenticatedOutputTypeDef",
+UnauthenticatedTypeDef = TypedDict(
+    "UnauthenticatedTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
 TlsTypeDef = TypedDict(
@@ -421,22 +355,14 @@
     {
         "CertificateAuthorityArnList": Sequence[str],
         "Enabled": bool,
     },
     total=False,
 )
 
-UnauthenticatedTypeDef = TypedDict(
-    "UnauthenticatedTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 _RequiredClientVpcConnectionTypeDef = TypedDict(
     "_RequiredClientVpcConnectionTypeDef",
     {
         "VpcConnectionArn": str,
     },
 )
 _OptionalClientVpcConnectionTypeDef = TypedDict(
@@ -446,19 +372,21 @@
         "CreationTime": datetime,
         "State": VpcConnectionStateType,
         "Owner": str,
     },
     total=False,
 )
 
+
 class ClientVpcConnectionTypeDef(
     _RequiredClientVpcConnectionTypeDef, _OptionalClientVpcConnectionTypeDef
 ):
     pass
 
+
 StateInfoTypeDef = TypedDict(
     "StateInfoTypeDef",
     {
         "Code": str,
         "Message": str,
     },
     total=False,
@@ -477,29 +405,35 @@
     "ClusterOperationStepInfoTypeDef",
     {
         "StepStatus": str,
     },
     total=False,
 )
 
-CompatibleKafkaVersionTypeDef = TypedDict(
-    "CompatibleKafkaVersionTypeDef",
+ClusterOperationV2SummaryTypeDef = TypedDict(
+    "ClusterOperationV2SummaryTypeDef",
     {
-        "SourceVersion": str,
-        "TargetVersions": List[str],
+        "ClusterArn": str,
+        "ClusterType": ClusterTypeType,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "OperationArn": str,
+        "OperationState": str,
+        "OperationType": str,
     },
     total=False,
 )
 
-ConfigurationInfoOutputTypeDef = TypedDict(
-    "ConfigurationInfoOutputTypeDef",
+CompatibleKafkaVersionTypeDef = TypedDict(
+    "CompatibleKafkaVersionTypeDef",
     {
-        "Arn": str,
-        "Revision": int,
+        "SourceVersion": str,
+        "TargetVersions": List[str],
     },
+    total=False,
 )
 
 ConfigurationInfoTypeDef = TypedDict(
     "ConfigurationInfoTypeDef",
     {
         "Arn": str,
         "Revision": int,
@@ -517,56 +451,29 @@
     "_OptionalConfigurationRevisionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class ConfigurationRevisionTypeDef(
     _RequiredConfigurationRevisionTypeDef, _OptionalConfigurationRevisionTypeDef
 ):
     pass
 
-PublicAccessOutputTypeDef = TypedDict(
-    "PublicAccessOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
 
 PublicAccessTypeDef = TypedDict(
     "PublicAccessTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-CreateClusterResponseTypeDef = TypedDict(
-    "CreateClusterResponseTypeDef",
-    {
-        "ClusterArn": str,
-        "ClusterName": str,
-        "State": ClusterStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateClusterV2ResponseTypeDef = TypedDict(
-    "CreateClusterV2ResponseTypeDef",
-    {
-        "ClusterArn": str,
-        "ClusterName": str,
-        "State": ClusterStateType,
-        "ClusterType": ClusterTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationRequestRequestTypeDef",
     {
         "Name": str,
         "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
@@ -575,20 +482,22 @@
     {
         "Description": str,
         "KafkaVersions": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateConfigurationRequestRequestTypeDef(
     _RequiredCreateConfigurationRequestRequestTypeDef,
     _OptionalCreateConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateVpcConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcConnectionRequestRequestTypeDef",
     {
         "TargetClusterArn": str,
         "Authentication": str,
         "VpcId": str,
         "ClientSubnets": Sequence[str],
@@ -599,34 +508,21 @@
     "_OptionalCreateVpcConnectionRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateVpcConnectionRequestRequestTypeDef(
     _RequiredCreateVpcConnectionRequestRequestTypeDef,
     _OptionalCreateVpcConnectionRequestRequestTypeDef,
 ):
     pass
 
-CreateVpcConnectionResponseTypeDef = TypedDict(
-    "CreateVpcConnectionResponseTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "State": VpcConnectionStateType,
-        "Authentication": str,
-        "VpcId": str,
-        "ClientSubnets": List[str],
-        "SecurityGroups": List[str],
-        "CreationTime": datetime,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteClusterPolicyRequestRequestTypeDef = TypedDict(
     "DeleteClusterPolicyRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
@@ -641,62 +537,44 @@
     "_OptionalDeleteClusterRequestRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
+
 class DeleteClusterRequestRequestTypeDef(
     _RequiredDeleteClusterRequestRequestTypeDef, _OptionalDeleteClusterRequestRequestTypeDef
 ):
     pass
 
-DeleteClusterResponseTypeDef = TypedDict(
-    "DeleteClusterResponseTypeDef",
-    {
-        "ClusterArn": str,
-        "State": ClusterStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteConfigurationResponseTypeDef = TypedDict(
-    "DeleteConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "State": ConfigurationStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVpcConnectionRequestRequestTypeDef = TypedDict(
     "DeleteVpcConnectionRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteVpcConnectionResponseTypeDef = TypedDict(
-    "DeleteVpcConnectionResponseTypeDef",
+DescribeClusterOperationRequestRequestTypeDef = TypedDict(
+    "DescribeClusterOperationRequestRequestTypeDef",
     {
-        "VpcConnectionArn": str,
-        "State": VpcConnectionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterOperationArn": str,
     },
 )
 
-DescribeClusterOperationRequestRequestTypeDef = TypedDict(
-    "DescribeClusterOperationRequestRequestTypeDef",
+DescribeClusterOperationV2RequestRequestTypeDef = TypedDict(
+    "DescribeClusterOperationV2RequestRequestTypeDef",
     {
         "ClusterOperationArn": str,
     },
 )
 
 DescribeClusterRequestRequestTypeDef = TypedDict(
     "DescribeClusterRequestRequestTypeDef",
@@ -723,79 +601,28 @@
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     {
         "Arn": str,
         "Revision": int,
     },
 )
 
-DescribeConfigurationRevisionResponseTypeDef = TypedDict(
-    "DescribeConfigurationRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "Description": str,
-        "Revision": int,
-        "ServerProperties": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeVpcConnectionRequestRequestTypeDef = TypedDict(
     "DescribeVpcConnectionRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DescribeVpcConnectionResponseTypeDef = TypedDict(
-    "DescribeVpcConnectionResponseTypeDef",
-    {
-        "VpcConnectionArn": str,
-        "TargetClusterArn": str,
-        "State": VpcConnectionStateType,
-        "Authentication": str,
-        "VpcId": str,
-        "Subnets": List[str],
-        "SecurityGroups": List[str],
-        "CreationTime": datetime,
-        "Tags": Dict[str, str],
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
-EncryptionAtRestOutputTypeDef = TypedDict(
-    "EncryptionAtRestOutputTypeDef",
-    {
-        "DataVolumeKMSKeyId": str,
-    },
-)
-
 EncryptionAtRestTypeDef = TypedDict(
     "EncryptionAtRestTypeDef",
     {
         "DataVolumeKMSKeyId": str,
     },
 )
 
-EncryptionInTransitOutputTypeDef = TypedDict(
-    "EncryptionInTransitOutputTypeDef",
-    {
-        "ClientBroker": ClientBrokerType,
-        "InCluster": bool,
-    },
-    total=False,
-)
-
 EncryptionInTransitTypeDef = TypedDict(
     "EncryptionInTransitTypeDef",
     {
         "ClientBroker": ClientBrokerType,
         "InCluster": bool,
     },
     total=False,
@@ -804,78 +631,37 @@
 GetBootstrapBrokersRequestRequestTypeDef = TypedDict(
     "GetBootstrapBrokersRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 
-GetBootstrapBrokersResponseTypeDef = TypedDict(
-    "GetBootstrapBrokersResponseTypeDef",
-    {
-        "BootstrapBrokerString": str,
-        "BootstrapBrokerStringTls": str,
-        "BootstrapBrokerStringSaslScram": str,
-        "BootstrapBrokerStringSaslIam": str,
-        "BootstrapBrokerStringPublicTls": str,
-        "BootstrapBrokerStringPublicSaslScram": str,
-        "BootstrapBrokerStringPublicSaslIam": str,
-        "BootstrapBrokerStringVpcConnectivityTls": str,
-        "BootstrapBrokerStringVpcConnectivitySaslScram": str,
-        "BootstrapBrokerStringVpcConnectivitySaslIam": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetClusterPolicyRequestRequestTypeDef = TypedDict(
     "GetClusterPolicyRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 
-GetClusterPolicyResponseTypeDef = TypedDict(
-    "GetClusterPolicyResponseTypeDef",
-    {
-        "CurrentVersion": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCompatibleKafkaVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
     total=False,
 )
 
-IamOutputTypeDef = TypedDict(
-    "IamOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 IamTypeDef = TypedDict(
     "IamTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-JmxExporterInfoOutputTypeDef = TypedDict(
-    "JmxExporterInfoOutputTypeDef",
-    {
-        "EnabledInBroker": bool,
-    },
-)
-
 JmxExporterInfoTypeDef = TypedDict(
     "JmxExporterInfoTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
 
@@ -891,34 +677,24 @@
     {
         "Version": str,
         "Status": KafkaVersionStatusType,
     },
     total=False,
 )
 
-_RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
-    "_RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
-    "_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
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
 
-class ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef(
-    _RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
-    _OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListClientVpcConnectionsRequestRequestTypeDef = TypedDict(
     "_RequiredListClientVpcConnectionsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClientVpcConnectionsRequestRequestTypeDef = TypedDict(
@@ -926,39 +702,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListClientVpcConnectionsRequestRequestTypeDef(
     _RequiredListClientVpcConnectionsRequestRequestTypeDef,
     _OptionalListClientVpcConnectionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListClusterOperationsRequestListClusterOperationsPaginateTypeDef(
-    _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
-    _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
-):
-    pass
 
 _RequiredListClusterOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterOperationsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
@@ -967,45 +725,51 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListClusterOperationsRequestRequestTypeDef(
     _RequiredListClusterOperationsRequestRequestTypeDef,
     _OptionalListClusterOperationsRequestRequestTypeDef,
 ):
     pass
 
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
+
+_RequiredListClusterOperationsV2RequestRequestTypeDef = TypedDict(
+    "_RequiredListClusterOperationsV2RequestRequestTypeDef",
     {
-        "ClusterNameFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ClusterArn": str,
     },
-    total=False,
 )
-
-ListClustersRequestRequestTypeDef = TypedDict(
-    "ListClustersRequestRequestTypeDef",
+_OptionalListClusterOperationsV2RequestRequestTypeDef = TypedDict(
+    "_OptionalListClusterOperationsV2RequestRequestTypeDef",
     {
-        "ClusterNameFilter": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListClustersV2RequestListClustersV2PaginateTypeDef = TypedDict(
-    "ListClustersV2RequestListClustersV2PaginateTypeDef",
+
+class ListClusterOperationsV2RequestRequestTypeDef(
+    _RequiredListClusterOperationsV2RequestRequestTypeDef,
+    _OptionalListClusterOperationsV2RequestRequestTypeDef,
+):
+    pass
+
+
+ListClustersRequestRequestTypeDef = TypedDict(
+    "ListClustersRequestRequestTypeDef",
     {
         "ClusterNameFilter": str,
-        "ClusterTypeFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
 ListClustersV2RequestRequestTypeDef = TypedDict(
     "ListClustersV2RequestRequestTypeDef",
     {
@@ -1013,34 +777,14 @@
         "ClusterTypeFilter": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef(
-    _RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
-    _OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListConfigurationRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredListConfigurationRevisionsRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListConfigurationRevisionsRequestRequestTypeDef = TypedDict(
@@ -1048,74 +792,40 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListConfigurationRevisionsRequestRequestTypeDef(
     _RequiredListConfigurationRevisionsRequestRequestTypeDef,
     _OptionalListConfigurationRevisionsRequestRequestTypeDef,
 ):
     pass
 
-ListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
-    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListConfigurationsRequestRequestTypeDef = TypedDict(
     "ListConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef = TypedDict(
-    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKafkaVersionsRequestRequestTypeDef = TypedDict(
     "ListKafkaVersionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListNodesRequestListNodesPaginateTypeDef = TypedDict(
-    "_RequiredListNodesRequestListNodesPaginateTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-_OptionalListNodesRequestListNodesPaginateTypeDef = TypedDict(
-    "_OptionalListNodesRequestListNodesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListNodesRequestListNodesPaginateTypeDef(
-    _RequiredListNodesRequestListNodesPaginateTypeDef,
-    _OptionalListNodesRequestListNodesPaginateTypeDef,
-):
-    pass
-
 _RequiredListNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListNodesRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListNodesRequestRequestTypeDef = TypedDict(
@@ -1123,38 +833,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListNodesRequestRequestTypeDef(
     _RequiredListNodesRequestRequestTypeDef, _OptionalListNodesRequestRequestTypeDef
 ):
     pass
 
-_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
-    "_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
-    "_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListScramSecretsRequestListScramSecretsPaginateTypeDef(
-    _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef,
-    _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef,
-):
-    pass
 
 _RequiredListScramSecretsRequestRequestTypeDef = TypedDict(
     "_RequiredListScramSecretsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
@@ -1163,51 +855,28 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListScramSecretsRequestRequestTypeDef(
     _RequiredListScramSecretsRequestRequestTypeDef, _OptionalListScramSecretsRequestRequestTypeDef
 ):
     pass
 
-ListScramSecretsResponseTypeDef = TypedDict(
-    "ListScramSecretsResponseTypeDef",
-    {
-        "NextToken": str,
-        "SecretArnList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef = TypedDict(
-    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVpcConnectionsRequestRequestTypeDef = TypedDict(
     "ListVpcConnectionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1227,23 +896,18 @@
         "Authentication": str,
         "VpcId": str,
         "State": VpcConnectionStateType,
     },
     total=False,
 )
 
+
 class VpcConnectionTypeDef(_RequiredVpcConnectionTypeDef, _OptionalVpcConnectionTypeDef):
     pass
 
-NodeExporterInfoOutputTypeDef = TypedDict(
-    "NodeExporterInfoOutputTypeDef",
-    {
-        "EnabledInBroker": bool,
-    },
-)
 
 NodeExporterInfoTypeDef = TypedDict(
     "NodeExporterInfoTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
@@ -1263,24 +927,14 @@
         "Endpoints": List[str],
         "ZookeeperId": float,
         "ZookeeperVersion": str,
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
 _RequiredPutClusterPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutClusterPolicyRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "Policy": str,
     },
 )
@@ -1288,71 +942,37 @@
     "_OptionalPutClusterPolicyRequestRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
+
 class PutClusterPolicyRequestRequestTypeDef(
     _RequiredPutClusterPolicyRequestRequestTypeDef, _OptionalPutClusterPolicyRequestRequestTypeDef
 ):
     pass
 
-PutClusterPolicyResponseTypeDef = TypedDict(
-    "PutClusterPolicyResponseTypeDef",
-    {
-        "CurrentVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 RebootBrokerRequestRequestTypeDef = TypedDict(
     "RebootBrokerRequestRequestTypeDef",
     {
         "BrokerIds": Sequence[str],
         "ClusterArn": str,
     },
 )
 
-RebootBrokerResponseTypeDef = TypedDict(
-    "RebootBrokerResponseTypeDef",
-    {
-        "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RejectClientVpcConnectionRequestRequestTypeDef = TypedDict(
     "RejectClientVpcConnectionRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "VpcConnectionArn": str,
     },
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
-ScramOutputTypeDef = TypedDict(
-    "ScramOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 ScramTypeDef = TypedDict(
     "ScramTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1367,34 +987,38 @@
     "_OptionalVpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class VpcConfigTypeDef(_RequiredVpcConfigTypeDef, _OptionalVpcConfigTypeDef):
     pass
 
+
 _RequiredVpcConfigOutputTypeDef = TypedDict(
     "_RequiredVpcConfigOutputTypeDef",
     {
         "SubnetIds": List[str],
     },
 )
 _OptionalVpcConfigOutputTypeDef = TypedDict(
     "_OptionalVpcConfigOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
+
 class VpcConfigOutputTypeDef(_RequiredVpcConfigOutputTypeDef, _OptionalVpcConfigOutputTypeDef):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1412,227 +1036,334 @@
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "TargetNumberOfBrokerNodes": int,
     },
 )
 
-UpdateBrokerCountResponseTypeDef = TypedDict(
-    "UpdateBrokerCountResponseTypeDef",
+UpdateBrokerTypeRequestRequestTypeDef = TypedDict(
+    "UpdateBrokerTypeRequestRequestTypeDef",
     {
         "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CurrentVersion": str,
+        "TargetInstanceType": str,
     },
 )
 
-UpdateBrokerStorageResponseTypeDef = TypedDict(
-    "UpdateBrokerStorageResponseTypeDef",
+_RequiredUpdateConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConfigurationRequestRequestTypeDef",
     {
-        "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Arn": str,
+        "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
+_OptionalUpdateConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
 
-UpdateBrokerTypeRequestRequestTypeDef = TypedDict(
-    "UpdateBrokerTypeRequestRequestTypeDef",
+
+class UpdateConfigurationRequestRequestTypeDef(
+    _RequiredUpdateConfigurationRequestRequestTypeDef,
+    _OptionalUpdateConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+UserIdentityTypeDef = TypedDict(
+    "UserIdentityTypeDef",
     {
-        "ClusterArn": str,
-        "CurrentVersion": str,
-        "TargetInstanceType": str,
+        "Type": UserIdentityTypeType,
+        "PrincipalId": str,
     },
+    total=False,
 )
 
-UpdateBrokerTypeResponseTypeDef = TypedDict(
-    "UpdateBrokerTypeResponseTypeDef",
+VpcConnectivityTlsTypeDef = TypedDict(
+    "VpcConnectivityTlsTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+VpcConnectivityIamTypeDef = TypedDict(
+    "VpcConnectivityIamTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+VpcConnectivityScramTypeDef = TypedDict(
+    "VpcConnectivityScramTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+CreateClusterResponseTypeDef = TypedDict(
+    "CreateClusterResponseTypeDef",
     {
         "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterName": str,
+        "State": ClusterStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateClusterConfigurationResponseTypeDef = TypedDict(
-    "UpdateClusterConfigurationResponseTypeDef",
+CreateClusterV2ResponseTypeDef = TypedDict(
+    "CreateClusterV2ResponseTypeDef",
     {
         "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterName": str,
+        "State": ClusterStateType,
+        "ClusterType": ClusterTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateClusterKafkaVersionResponseTypeDef = TypedDict(
-    "UpdateClusterKafkaVersionResponseTypeDef",
+CreateVpcConnectionResponseTypeDef = TypedDict(
+    "CreateVpcConnectionResponseTypeDef",
+    {
+        "VpcConnectionArn": str,
+        "State": VpcConnectionStateType,
+        "Authentication": str,
+        "VpcId": str,
+        "ClientSubnets": List[str],
+        "SecurityGroups": List[str],
+        "CreationTime": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteClusterResponseTypeDef = TypedDict(
+    "DeleteClusterResponseTypeDef",
     {
         "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "State": ClusterStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConfigurationRequestRequestTypeDef",
+DeleteConfigurationResponseTypeDef = TypedDict(
+    "DeleteConfigurationResponseTypeDef",
     {
         "Arn": str,
-        "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
+        "State": ConfigurationStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConfigurationRequestRequestTypeDef",
+
+DeleteVpcConnectionResponseTypeDef = TypedDict(
+    "DeleteVpcConnectionResponseTypeDef",
     {
+        "VpcConnectionArn": str,
+        "State": VpcConnectionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeConfigurationRevisionResponseTypeDef = TypedDict(
+    "DescribeConfigurationRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
         "Description": str,
+        "Revision": int,
+        "ServerProperties": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateConfigurationRequestRequestTypeDef(
-    _RequiredUpdateConfigurationRequestRequestTypeDef,
-    _OptionalUpdateConfigurationRequestRequestTypeDef,
-):
-    pass
+DescribeVpcConnectionResponseTypeDef = TypedDict(
+    "DescribeVpcConnectionResponseTypeDef",
+    {
+        "VpcConnectionArn": str,
+        "TargetClusterArn": str,
+        "State": VpcConnectionStateType,
+        "Authentication": str,
+        "VpcId": str,
+        "Subnets": List[str],
+        "SecurityGroups": List[str],
+        "CreationTime": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateConnectivityResponseTypeDef = TypedDict(
-    "UpdateConnectivityResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateMonitoringResponseTypeDef = TypedDict(
-    "UpdateMonitoringResponseTypeDef",
+GetBootstrapBrokersResponseTypeDef = TypedDict(
+    "GetBootstrapBrokersResponseTypeDef",
     {
-        "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BootstrapBrokerString": str,
+        "BootstrapBrokerStringTls": str,
+        "BootstrapBrokerStringSaslScram": str,
+        "BootstrapBrokerStringSaslIam": str,
+        "BootstrapBrokerStringPublicTls": str,
+        "BootstrapBrokerStringPublicSaslScram": str,
+        "BootstrapBrokerStringPublicSaslIam": str,
+        "BootstrapBrokerStringVpcConnectivityTls": str,
+        "BootstrapBrokerStringVpcConnectivitySaslScram": str,
+        "BootstrapBrokerStringVpcConnectivitySaslIam": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSecurityResponseTypeDef = TypedDict(
-    "UpdateSecurityResponseTypeDef",
+GetClusterPolicyResponseTypeDef = TypedDict(
+    "GetClusterPolicyResponseTypeDef",
     {
-        "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CurrentVersion": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateStorageResponseTypeDef = TypedDict(
-    "UpdateStorageResponseTypeDef",
+ListScramSecretsResponseTypeDef = TypedDict(
+    "ListScramSecretsResponseTypeDef",
     {
-        "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NextToken": str,
+        "SecretArnList": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserIdentityTypeDef = TypedDict(
-    "UserIdentityTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "Type": UserIdentityTypeType,
-        "PrincipalId": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VpcConnectivityTlsOutputTypeDef = TypedDict(
-    "VpcConnectivityTlsOutputTypeDef",
+PutClusterPolicyResponseTypeDef = TypedDict(
+    "PutClusterPolicyResponseTypeDef",
     {
-        "Enabled": bool,
+        "CurrentVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VpcConnectivityTlsTypeDef = TypedDict(
-    "VpcConnectivityTlsTypeDef",
+RebootBrokerResponseTypeDef = TypedDict(
+    "RebootBrokerResponseTypeDef",
     {
-        "Enabled": bool,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VpcConnectivityIamOutputTypeDef = TypedDict(
-    "VpcConnectivityIamOutputTypeDef",
+UpdateBrokerCountResponseTypeDef = TypedDict(
+    "UpdateBrokerCountResponseTypeDef",
     {
-        "Enabled": bool,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VpcConnectivityIamTypeDef = TypedDict(
-    "VpcConnectivityIamTypeDef",
+UpdateBrokerStorageResponseTypeDef = TypedDict(
+    "UpdateBrokerStorageResponseTypeDef",
     {
-        "Enabled": bool,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VpcConnectivityScramOutputTypeDef = TypedDict(
-    "VpcConnectivityScramOutputTypeDef",
+UpdateBrokerTypeResponseTypeDef = TypedDict(
+    "UpdateBrokerTypeResponseTypeDef",
     {
-        "Enabled": bool,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-VpcConnectivityScramTypeDef = TypedDict(
-    "VpcConnectivityScramTypeDef",
+UpdateClusterConfigurationResponseTypeDef = TypedDict(
+    "UpdateClusterConfigurationResponseTypeDef",
     {
-        "Enabled": bool,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-BatchAssociateScramSecretResponseTypeDef = TypedDict(
-    "BatchAssociateScramSecretResponseTypeDef",
+UpdateClusterKafkaVersionResponseTypeDef = TypedDict(
+    "UpdateClusterKafkaVersionResponseTypeDef",
     {
         "ClusterArn": str,
-        "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDisassociateScramSecretResponseTypeDef = TypedDict(
-    "BatchDisassociateScramSecretResponseTypeDef",
+UpdateConnectivityResponseTypeDef = TypedDict(
+    "UpdateConnectivityResponseTypeDef",
     {
         "ClusterArn": str,
-        "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBrokerEBSVolumeInfoOutputTypeDef = TypedDict(
-    "_RequiredBrokerEBSVolumeInfoOutputTypeDef",
+UpdateMonitoringResponseTypeDef = TypedDict(
+    "UpdateMonitoringResponseTypeDef",
     {
-        "KafkaBrokerNodeId": str,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBrokerEBSVolumeInfoOutputTypeDef = TypedDict(
-    "_OptionalBrokerEBSVolumeInfoOutputTypeDef",
+
+UpdateSecurityResponseTypeDef = TypedDict(
+    "UpdateSecurityResponseTypeDef",
     {
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
-        "VolumeSizeGB": int,
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class BrokerEBSVolumeInfoOutputTypeDef(
-    _RequiredBrokerEBSVolumeInfoOutputTypeDef, _OptionalBrokerEBSVolumeInfoOutputTypeDef
-):
-    pass
+UpdateStorageResponseTypeDef = TypedDict(
+    "UpdateStorageResponseTypeDef",
+    {
+        "ClusterArn": str,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-EBSStorageInfoOutputTypeDef = TypedDict(
-    "EBSStorageInfoOutputTypeDef",
+BatchAssociateScramSecretResponseTypeDef = TypedDict(
+    "BatchAssociateScramSecretResponseTypeDef",
     {
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
-        "VolumeSize": int,
+        "ClusterArn": str,
+        "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchDisassociateScramSecretResponseTypeDef = TypedDict(
+    "BatchDisassociateScramSecretResponseTypeDef",
+    {
+        "ClusterArn": str,
+        "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredBrokerEBSVolumeInfoTypeDef = TypedDict(
     "_RequiredBrokerEBSVolumeInfoTypeDef",
     {
         "KafkaBrokerNodeId": str,
     },
@@ -1642,19 +1373,21 @@
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "VolumeSizeGB": int,
     },
     total=False,
 )
 
+
 class BrokerEBSVolumeInfoTypeDef(
     _RequiredBrokerEBSVolumeInfoTypeDef, _OptionalBrokerEBSVolumeInfoTypeDef
 ):
     pass
 
+
 EBSStorageInfoTypeDef = TypedDict(
     "EBSStorageInfoTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "VolumeSize": int,
     },
     total=False,
@@ -1673,28 +1406,20 @@
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "StorageMode": StorageModeType,
         "VolumeSizeGB": int,
     },
     total=False,
 )
 
+
 class UpdateStorageRequestRequestTypeDef(
     _RequiredUpdateStorageRequestRequestTypeDef, _OptionalUpdateStorageRequestRequestTypeDef
 ):
     pass
 
-BrokerLogsOutputTypeDef = TypedDict(
-    "BrokerLogsOutputTypeDef",
-    {
-        "CloudWatchLogs": CloudWatchLogsOutputTypeDef,
-        "Firehose": FirehoseOutputTypeDef,
-        "S3": S3OutputTypeDef,
-    },
-    total=False,
-)
 
 BrokerLogsTypeDef = TypedDict(
     "BrokerLogsTypeDef",
     {
         "CloudWatchLogs": CloudWatchLogsTypeDef,
         "Firehose": FirehoseTypeDef,
         "S3": S3TypeDef,
@@ -1716,32 +1441,41 @@
 )
 
 ListClientVpcConnectionsResponseTypeDef = TypedDict(
     "ListClientVpcConnectionsResponseTypeDef",
     {
         "ClientVpcConnections": List[ClientVpcConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterOperationStepTypeDef = TypedDict(
     "ClusterOperationStepTypeDef",
     {
         "StepInfo": ClusterOperationStepInfoTypeDef,
         "StepName": str,
     },
     total=False,
 )
 
+ListClusterOperationsV2ResponseTypeDef = TypedDict(
+    "ListClusterOperationsV2ResponseTypeDef",
+    {
+        "ClusterOperationInfoList": List[ClusterOperationV2SummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetCompatibleKafkaVersionsResponseTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsResponseTypeDef",
     {
         "CompatibleKafkaVersions": List[CompatibleKafkaVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateClusterConfigurationRequestRequestTypeDef",
     {
         "ClusterArn": str,
@@ -1762,20 +1496,22 @@
     "_OptionalUpdateClusterKafkaVersionRequestRequestTypeDef",
     {
         "ConfigurationInfo": ConfigurationInfoTypeDef,
     },
     total=False,
 )
 
+
 class UpdateClusterKafkaVersionRequestRequestTypeDef(
     _RequiredUpdateClusterKafkaVersionRequestRequestTypeDef,
     _OptionalUpdateClusterKafkaVersionRequestRequestTypeDef,
 ):
     pass
 
+
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "Description": str,
         "KafkaVersions": List[str],
@@ -1789,111 +1525,260 @@
     "CreateConfigurationResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "LatestRevision": ConfigurationRevisionTypeDef,
         "Name": str,
         "State": ConfigurationStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConfigurationResponseTypeDef = TypedDict(
     "DescribeConfigurationResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "Description": str,
         "KafkaVersions": List[str],
         "LatestRevision": ConfigurationRevisionTypeDef,
         "Name": str,
         "State": ConfigurationStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfigurationRevisionsResponseTypeDef = TypedDict(
     "ListConfigurationRevisionsResponseTypeDef",
     {
         "NextToken": str,
         "Revisions": List[ConfigurationRevisionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfigurationResponseTypeDef = TypedDict(
     "UpdateConfigurationResponseTypeDef",
     {
         "Arn": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EncryptionInfoOutputTypeDef = TypedDict(
-    "EncryptionInfoOutputTypeDef",
-    {
-        "EncryptionAtRest": EncryptionAtRestOutputTypeDef,
-        "EncryptionInTransit": EncryptionInTransitOutputTypeDef,
-    },
-    total=False,
-)
-
 EncryptionInfoTypeDef = TypedDict(
     "EncryptionInfoTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "EncryptionInTransit": EncryptionInTransitTypeDef,
     },
     total=False,
 )
 
-ServerlessSaslOutputTypeDef = TypedDict(
-    "ServerlessSaslOutputTypeDef",
-    {
-        "Iam": IamOutputTypeDef,
-    },
-    total=False,
-)
-
 ServerlessSaslTypeDef = TypedDict(
     "ServerlessSaslTypeDef",
     {
         "Iam": IamTypeDef,
     },
     total=False,
 )
 
 ListKafkaVersionsResponseTypeDef = TypedDict(
     "ListKafkaVersionsResponseTypeDef",
     {
         "KafkaVersions": List[KafkaVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListVpcConnectionsResponseTypeDef = TypedDict(
-    "ListVpcConnectionsResponseTypeDef",
+_RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
+    "_RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     {
-        "VpcConnections": List[VpcConnectionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterArn": str,
+    },
+)
+_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
+    "_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef(
+    _RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+    _OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListClusterOperationsRequestListClusterOperationsPaginateTypeDef(
+    _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
+    _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef = TypedDict(
+    "_RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef = TypedDict(
+    "_OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef(
+    _RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
+    _OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
+):
+    pass
+
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "ClusterNameFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListClustersV2RequestListClustersV2PaginateTypeDef = TypedDict(
+    "ListClustersV2RequestListClustersV2PaginateTypeDef",
+    {
+        "ClusterNameFilter": str,
+        "ClusterTypeFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef(
+    _RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
+    _OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
+):
+    pass
+
+
+ListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
+    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef = TypedDict(
+    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-PrometheusInfoOutputTypeDef = TypedDict(
-    "PrometheusInfoOutputTypeDef",
+_RequiredListNodesRequestListNodesPaginateTypeDef = TypedDict(
+    "_RequiredListNodesRequestListNodesPaginateTypeDef",
     {
-        "JmxExporter": JmxExporterInfoOutputTypeDef,
-        "NodeExporter": NodeExporterInfoOutputTypeDef,
+        "ClusterArn": str,
+    },
+)
+_OptionalListNodesRequestListNodesPaginateTypeDef = TypedDict(
+    "_OptionalListNodesRequestListNodesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
+class ListNodesRequestListNodesPaginateTypeDef(
+    _RequiredListNodesRequestListNodesPaginateTypeDef,
+    _OptionalListNodesRequestListNodesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
+    "_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
+    "_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListScramSecretsRequestListScramSecretsPaginateTypeDef(
+    _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef,
+    _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef,
+):
+    pass
+
+
+ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef = TypedDict(
+    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListVpcConnectionsResponseTypeDef = TypedDict(
+    "ListVpcConnectionsResponseTypeDef",
+    {
+        "VpcConnections": List[VpcConnectionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PrometheusInfoTypeDef = TypedDict(
     "PrometheusInfoTypeDef",
     {
         "JmxExporter": JmxExporterInfoTypeDef,
         "NodeExporter": NodeExporterInfoTypeDef,
     },
     total=False,
@@ -1904,69 +1789,54 @@
     {
         "JmxExporter": JmxExporterTypeDef,
         "NodeExporter": NodeExporterTypeDef,
     },
     total=False,
 )
 
-SaslOutputTypeDef = TypedDict(
-    "SaslOutputTypeDef",
-    {
-        "Scram": ScramOutputTypeDef,
-        "Iam": IamOutputTypeDef,
-    },
-    total=False,
-)
-
 SaslTypeDef = TypedDict(
     "SaslTypeDef",
     {
         "Scram": ScramTypeDef,
         "Iam": IamTypeDef,
     },
     total=False,
 )
 
-VpcConnectionInfoTypeDef = TypedDict(
-    "VpcConnectionInfoTypeDef",
+VpcConnectionInfoServerlessTypeDef = TypedDict(
+    "VpcConnectionInfoServerlessTypeDef",
     {
-        "VpcConnectionArn": str,
+        "CreationTime": datetime,
         "Owner": str,
         "UserIdentity": UserIdentityTypeDef,
-        "CreationTime": datetime,
+        "VpcConnectionArn": str,
     },
     total=False,
 )
 
-VpcConnectivitySaslOutputTypeDef = TypedDict(
-    "VpcConnectivitySaslOutputTypeDef",
+VpcConnectionInfoTypeDef = TypedDict(
+    "VpcConnectionInfoTypeDef",
     {
-        "Scram": VpcConnectivityScramOutputTypeDef,
-        "Iam": VpcConnectivityIamOutputTypeDef,
+        "VpcConnectionArn": str,
+        "Owner": str,
+        "UserIdentity": UserIdentityTypeDef,
+        "CreationTime": datetime,
     },
     total=False,
 )
 
 VpcConnectivitySaslTypeDef = TypedDict(
     "VpcConnectivitySaslTypeDef",
     {
         "Scram": VpcConnectivityScramTypeDef,
         "Iam": VpcConnectivityIamTypeDef,
     },
     total=False,
 )
 
-StorageInfoOutputTypeDef = TypedDict(
-    "StorageInfoOutputTypeDef",
-    {
-        "EbsStorageInfo": EBSStorageInfoOutputTypeDef,
-    },
-    total=False,
-)
-
 UpdateBrokerStorageRequestRequestTypeDef = TypedDict(
     "UpdateBrokerStorageRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "TargetBrokerEBSVolumeInfo": Sequence[BrokerEBSVolumeInfoTypeDef],
     },
@@ -1976,21 +1846,14 @@
     "StorageInfoTypeDef",
     {
         "EbsStorageInfo": EBSStorageInfoTypeDef,
     },
     total=False,
 )
 
-LoggingInfoOutputTypeDef = TypedDict(
-    "LoggingInfoOutputTypeDef",
-    {
-        "BrokerLogs": BrokerLogsOutputTypeDef,
-    },
-)
-
 LoggingInfoTypeDef = TypedDict(
     "LoggingInfoTypeDef",
     {
         "BrokerLogs": BrokerLogsTypeDef,
     },
 )
 
@@ -2008,41 +1871,26 @@
 )
 
 ListConfigurationsResponseTypeDef = TypedDict(
     "ListConfigurationsResponseTypeDef",
     {
         "Configurations": List[ConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ServerlessClientAuthenticationOutputTypeDef = TypedDict(
-    "ServerlessClientAuthenticationOutputTypeDef",
-    {
-        "Sasl": ServerlessSaslOutputTypeDef,
-    },
-    total=False,
-)
-
 ServerlessClientAuthenticationTypeDef = TypedDict(
     "ServerlessClientAuthenticationTypeDef",
     {
         "Sasl": ServerlessSaslTypeDef,
     },
     total=False,
 )
 
-OpenMonitoringInfoOutputTypeDef = TypedDict(
-    "OpenMonitoringInfoOutputTypeDef",
-    {
-        "Prometheus": PrometheusInfoOutputTypeDef,
-    },
-)
-
 OpenMonitoringInfoTypeDef = TypedDict(
     "OpenMonitoringInfoTypeDef",
     {
         "Prometheus": PrometheusInfoTypeDef,
     },
 )
 
@@ -2052,36 +1900,35 @@
         "Prometheus": PrometheusTypeDef,
     },
 )
 
 ClientAuthenticationOutputTypeDef = TypedDict(
     "ClientAuthenticationOutputTypeDef",
     {
-        "Sasl": SaslOutputTypeDef,
+        "Sasl": SaslTypeDef,
         "Tls": TlsOutputTypeDef,
-        "Unauthenticated": UnauthenticatedOutputTypeDef,
+        "Unauthenticated": UnauthenticatedTypeDef,
     },
     total=False,
 )
 
 ClientAuthenticationTypeDef = TypedDict(
     "ClientAuthenticationTypeDef",
     {
         "Sasl": SaslTypeDef,
         "Tls": TlsTypeDef,
         "Unauthenticated": UnauthenticatedTypeDef,
     },
     total=False,
 )
 
-VpcConnectivityClientAuthenticationOutputTypeDef = TypedDict(
-    "VpcConnectivityClientAuthenticationOutputTypeDef",
+ClusterOperationV2ServerlessTypeDef = TypedDict(
+    "ClusterOperationV2ServerlessTypeDef",
     {
-        "Sasl": VpcConnectivitySaslOutputTypeDef,
-        "Tls": VpcConnectivityTlsOutputTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoServerlessTypeDef,
     },
     total=False,
 )
 
 VpcConnectivityClientAuthenticationTypeDef = TypedDict(
     "VpcConnectivityClientAuthenticationTypeDef",
     {
@@ -2092,54 +1939,58 @@
 )
 
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
         "NextToken": str,
         "NodeInfoList": List[NodeInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredServerlessTypeDef = TypedDict(
-    "_RequiredServerlessTypeDef",
+_RequiredServerlessRequestTypeDef = TypedDict(
+    "_RequiredServerlessRequestTypeDef",
     {
-        "VpcConfigs": List[VpcConfigOutputTypeDef],
+        "VpcConfigs": Sequence[VpcConfigTypeDef],
     },
 )
-_OptionalServerlessTypeDef = TypedDict(
-    "_OptionalServerlessTypeDef",
+_OptionalServerlessRequestTypeDef = TypedDict(
+    "_OptionalServerlessRequestTypeDef",
     {
-        "ClientAuthentication": ServerlessClientAuthenticationOutputTypeDef,
+        "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
     },
     total=False,
 )
 
-class ServerlessTypeDef(_RequiredServerlessTypeDef, _OptionalServerlessTypeDef):
+
+class ServerlessRequestTypeDef(
+    _RequiredServerlessRequestTypeDef, _OptionalServerlessRequestTypeDef
+):
     pass
 
-_RequiredServerlessRequestTypeDef = TypedDict(
-    "_RequiredServerlessRequestTypeDef",
+
+_RequiredServerlessTypeDef = TypedDict(
+    "_RequiredServerlessTypeDef",
     {
-        "VpcConfigs": Sequence[VpcConfigTypeDef],
+        "VpcConfigs": List[VpcConfigOutputTypeDef],
     },
 )
-_OptionalServerlessRequestTypeDef = TypedDict(
-    "_OptionalServerlessRequestTypeDef",
+_OptionalServerlessTypeDef = TypedDict(
+    "_OptionalServerlessTypeDef",
     {
         "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
     },
     total=False,
 )
 
-class ServerlessRequestTypeDef(
-    _RequiredServerlessRequestTypeDef, _OptionalServerlessRequestTypeDef
-):
+
+class ServerlessTypeDef(_RequiredServerlessTypeDef, _OptionalServerlessTypeDef):
     pass
 
+
 _RequiredUpdateMonitoringRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitoringRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
     },
 )
@@ -2149,19 +2000,21 @@
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringInfoTypeDef,
         "LoggingInfo": LoggingInfoTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMonitoringRequestRequestTypeDef(
     _RequiredUpdateMonitoringRequestRequestTypeDef, _OptionalUpdateMonitoringRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
     },
 )
@@ -2170,44 +2023,29 @@
     {
         "ClientAuthentication": ClientAuthenticationTypeDef,
         "EncryptionInfo": EncryptionInfoTypeDef,
     },
     total=False,
 )
 
+
 class UpdateSecurityRequestRequestTypeDef(
     _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
 ):
     pass
 
-VpcConnectivityOutputTypeDef = TypedDict(
-    "VpcConnectivityOutputTypeDef",
-    {
-        "ClientAuthentication": VpcConnectivityClientAuthenticationOutputTypeDef,
-    },
-    total=False,
-)
 
 VpcConnectivityTypeDef = TypedDict(
     "VpcConnectivityTypeDef",
     {
         "ClientAuthentication": VpcConnectivityClientAuthenticationTypeDef,
     },
     total=False,
 )
 
-ConnectivityInfoOutputTypeDef = TypedDict(
-    "ConnectivityInfoOutputTypeDef",
-    {
-        "PublicAccess": PublicAccessOutputTypeDef,
-        "VpcConnectivity": VpcConnectivityOutputTypeDef,
-    },
-    total=False,
-)
-
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "PublicAccess": PublicAccessTypeDef,
         "VpcConnectivity": VpcConnectivityTypeDef,
     },
     total=False,
@@ -2221,44 +2059,27 @@
     },
 )
 _OptionalBrokerNodeGroupInfoOutputTypeDef = TypedDict(
     "_OptionalBrokerNodeGroupInfoOutputTypeDef",
     {
         "BrokerAZDistribution": Literal["DEFAULT"],
         "SecurityGroups": List[str],
-        "StorageInfo": StorageInfoOutputTypeDef,
-        "ConnectivityInfo": ConnectivityInfoOutputTypeDef,
+        "StorageInfo": StorageInfoTypeDef,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
         "ZoneIds": List[str],
     },
     total=False,
 )
 
+
 class BrokerNodeGroupInfoOutputTypeDef(
     _RequiredBrokerNodeGroupInfoOutputTypeDef, _OptionalBrokerNodeGroupInfoOutputTypeDef
 ):
     pass
 
-MutableClusterInfoTypeDef = TypedDict(
-    "MutableClusterInfoTypeDef",
-    {
-        "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoOutputTypeDef],
-        "ConfigurationInfo": ConfigurationInfoOutputTypeDef,
-        "NumberOfBrokerNodes": int,
-        "EnhancedMonitoring": EnhancedMonitoringType,
-        "OpenMonitoring": OpenMonitoringTypeDef,
-        "KafkaVersion": str,
-        "LoggingInfo": LoggingInfoOutputTypeDef,
-        "InstanceType": str,
-        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
-        "EncryptionInfo": EncryptionInfoOutputTypeDef,
-        "ConnectivityInfo": ConnectivityInfoOutputTypeDef,
-        "StorageMode": StorageModeType,
-    },
-    total=False,
-)
 
 _RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
     "_RequiredBrokerNodeGroupInfoTypeDef",
     {
         "ClientSubnets": Sequence[str],
         "InstanceType": str,
     },
@@ -2271,19 +2092,40 @@
         "StorageInfo": StorageInfoTypeDef,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "ZoneIds": Sequence[str],
     },
     total=False,
 )
 
+
 class BrokerNodeGroupInfoTypeDef(
     _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
 ):
     pass
 
+
+MutableClusterInfoTypeDef = TypedDict(
+    "MutableClusterInfoTypeDef",
+    {
+        "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoTypeDef],
+        "ConfigurationInfo": ConfigurationInfoTypeDef,
+        "NumberOfBrokerNodes": int,
+        "EnhancedMonitoring": EnhancedMonitoringType,
+        "OpenMonitoring": OpenMonitoringTypeDef,
+        "KafkaVersion": str,
+        "LoggingInfo": LoggingInfoTypeDef,
+        "InstanceType": str,
+        "ClientAuthentication": ClientAuthenticationOutputTypeDef,
+        "EncryptionInfo": EncryptionInfoTypeDef,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
+        "StorageMode": StorageModeType,
+    },
+    total=False,
+)
+
 UpdateConnectivityRequestRequestTypeDef = TypedDict(
     "UpdateConnectivityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "CurrentVersion": str,
     },
@@ -2296,18 +2138,18 @@
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoOutputTypeDef,
         "ClientAuthentication": ClientAuthenticationOutputTypeDef,
         "ClusterArn": str,
         "ClusterName": str,
         "CreationTime": datetime,
         "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
         "CurrentVersion": str,
-        "EncryptionInfo": EncryptionInfoOutputTypeDef,
+        "EncryptionInfo": EncryptionInfoTypeDef,
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringTypeDef,
-        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "LoggingInfo": LoggingInfoTypeDef,
         "NumberOfBrokerNodes": int,
         "State": ClusterStateType,
         "StateInfo": StateInfoTypeDef,
         "Tags": Dict[str, str],
         "ZookeeperConnectString": str,
         "ZookeeperConnectStringTls": str,
         "StorageMode": StorageModeType,
@@ -2323,46 +2165,29 @@
     },
 )
 _OptionalProvisionedTypeDef = TypedDict(
     "_OptionalProvisionedTypeDef",
     {
         "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
         "ClientAuthentication": ClientAuthenticationOutputTypeDef,
-        "EncryptionInfo": EncryptionInfoOutputTypeDef,
+        "EncryptionInfo": EncryptionInfoTypeDef,
         "EnhancedMonitoring": EnhancedMonitoringType,
-        "OpenMonitoring": OpenMonitoringInfoOutputTypeDef,
-        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "OpenMonitoring": OpenMonitoringInfoTypeDef,
+        "LoggingInfo": LoggingInfoTypeDef,
         "ZookeeperConnectString": str,
         "ZookeeperConnectStringTls": str,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
+
 class ProvisionedTypeDef(_RequiredProvisionedTypeDef, _OptionalProvisionedTypeDef):
     pass
 
-ClusterOperationInfoTypeDef = TypedDict(
-    "ClusterOperationInfoTypeDef",
-    {
-        "ClientRequestId": str,
-        "ClusterArn": str,
-        "CreationTime": datetime,
-        "EndTime": datetime,
-        "ErrorInfo": ErrorInfoTypeDef,
-        "OperationArn": str,
-        "OperationState": str,
-        "OperationSteps": List[ClusterOperationStepTypeDef],
-        "OperationType": str,
-        "SourceClusterInfo": MutableClusterInfoTypeDef,
-        "TargetClusterInfo": MutableClusterInfoTypeDef,
-        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
-    },
-    total=False,
-)
 
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "ClusterName": str,
         "KafkaVersion": str,
@@ -2380,19 +2205,21 @@
         "LoggingInfo": LoggingInfoTypeDef,
         "Tags": Mapping[str, str],
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
+
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredProvisionedRequestTypeDef = TypedDict(
     "_RequiredProvisionedRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
     },
@@ -2407,33 +2234,65 @@
         "OpenMonitoring": OpenMonitoringInfoTypeDef,
         "LoggingInfo": LoggingInfoTypeDef,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
+
 class ProvisionedRequestTypeDef(
     _RequiredProvisionedRequestTypeDef, _OptionalProvisionedRequestTypeDef
 ):
     pass
 
+
+ClusterOperationInfoTypeDef = TypedDict(
+    "ClusterOperationInfoTypeDef",
+    {
+        "ClientRequestId": str,
+        "ClusterArn": str,
+        "CreationTime": datetime,
+        "EndTime": datetime,
+        "ErrorInfo": ErrorInfoTypeDef,
+        "OperationArn": str,
+        "OperationState": str,
+        "OperationSteps": List[ClusterOperationStepTypeDef],
+        "OperationType": str,
+        "SourceClusterInfo": MutableClusterInfoTypeDef,
+        "TargetClusterInfo": MutableClusterInfoTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
+    },
+    total=False,
+)
+
+ClusterOperationV2ProvisionedTypeDef = TypedDict(
+    "ClusterOperationV2ProvisionedTypeDef",
+    {
+        "OperationSteps": List[ClusterOperationStepTypeDef],
+        "SourceClusterInfo": MutableClusterInfoTypeDef,
+        "TargetClusterInfo": MutableClusterInfoTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
+    },
+    total=False,
+)
+
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "ClusterInfo": ClusterInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListClustersResponseTypeDef = TypedDict(
     "ListClustersResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ActiveOperationArn": str,
@@ -2447,31 +2306,14 @@
         "Tags": Dict[str, str],
         "Provisioned": ProvisionedTypeDef,
         "Serverless": ServerlessTypeDef,
     },
     total=False,
 )
 
-DescribeClusterOperationResponseTypeDef = TypedDict(
-    "DescribeClusterOperationResponseTypeDef",
-    {
-        "ClusterOperationInfo": ClusterOperationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListClusterOperationsResponseTypeDef = TypedDict(
-    "ListClusterOperationsResponseTypeDef",
-    {
-        "ClusterOperationInfoList": List[ClusterOperationInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateClusterV2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterV2RequestRequestTypeDef",
     {
         "ClusterName": str,
     },
 )
 _OptionalCreateClusterV2RequestRequestTypeDef = TypedDict(
@@ -2480,28 +2322,72 @@
         "Tags": Mapping[str, str],
         "Provisioned": ProvisionedRequestTypeDef,
         "Serverless": ServerlessRequestTypeDef,
     },
     total=False,
 )
 
+
 class CreateClusterV2RequestRequestTypeDef(
     _RequiredCreateClusterV2RequestRequestTypeDef, _OptionalCreateClusterV2RequestRequestTypeDef
 ):
     pass
 
+
+DescribeClusterOperationResponseTypeDef = TypedDict(
+    "DescribeClusterOperationResponseTypeDef",
+    {
+        "ClusterOperationInfo": ClusterOperationInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClusterOperationsResponseTypeDef = TypedDict(
+    "ListClusterOperationsResponseTypeDef",
+    {
+        "ClusterOperationInfoList": List[ClusterOperationInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterOperationV2TypeDef = TypedDict(
+    "ClusterOperationV2TypeDef",
+    {
+        "ClusterArn": str,
+        "ClusterType": ClusterTypeType,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ErrorInfo": ErrorInfoTypeDef,
+        "OperationArn": str,
+        "OperationState": str,
+        "OperationType": str,
+        "Provisioned": ClusterOperationV2ProvisionedTypeDef,
+        "Serverless": ClusterOperationV2ServerlessTypeDef,
+    },
+    total=False,
+)
+
 DescribeClusterV2ResponseTypeDef = TypedDict(
     "DescribeClusterV2ResponseTypeDef",
     {
         "ClusterInfo": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListClustersV2ResponseTypeDef = TypedDict(
     "ListClustersV2ResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeClusterOperationV2ResponseTypeDef = TypedDict(
+    "DescribeClusterOperationV2ResponseTypeDef",
+    {
+        "ClusterOperationInfo": ClusterOperationV2TypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/PKG-INFO` & `mypy-boto3-kafka-1.28.15/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-kafka
-Version: 1.28.12
-Summary: Type annotations for boto3.Kafka 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kafka type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-kafka"></a>
 
 # mypy-boto3-kafka
 
 [![PyPI - mypy-boto3-kafka](https://img.shields.io/pypi/v/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafka)](https://pepy.tech/project/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,14 +249,15 @@
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kafka import KafkaClient
 from mypy_boto3_kafka.paginator import (
     ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
+    ListClusterOperationsV2Paginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
@@ -301,14 +270,17 @@
 # Types should be correctly discovered by mypy and IDEs
 list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator(
     "list_client_vpc_connections"
 )
 list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator(
     "list_cluster_operations"
 )
+list_cluster_operations_v2_paginator: ListClusterOperationsV2Paginator = client.get_paginator(
+    "list_cluster_operations_v2"
+)
 list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
 list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
 list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator(
     "list_configuration_revisions"
 )
 list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator(
     "list_configurations"
@@ -337,14 +309,15 @@
     ClusterStateType,
     ClusterTypeType,
     ConfigurationStateType,
     EnhancedMonitoringType,
     KafkaVersionStatusType,
     ListClientVpcConnectionsPaginatorName,
     ListClusterOperationsPaginatorName,
+    ListClusterOperationsV2PaginatorName,
     ListClustersPaginatorName,
     ListClustersV2PaginatorName,
     ListConfigurationRevisionsPaginatorName,
     ListConfigurationsPaginatorName,
     ListKafkaVersionsPaginatorName,
     ListNodesPaginatorName,
     ListScramSecretsPaginatorName,
@@ -371,211 +344,190 @@
 
 `mypy_boto3_kafka.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kafka.type_defs import (
     BatchAssociateScramSecretRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedScramSecretTypeDef,
     BatchDisassociateScramSecretRequestRequestTypeDef,
-    ProvisionedThroughputOutputTypeDef,
     ProvisionedThroughputTypeDef,
-    CloudWatchLogsOutputTypeDef,
-    FirehoseOutputTypeDef,
-    S3OutputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
     TlsOutputTypeDef,
-    UnauthenticatedOutputTypeDef,
-    TlsTypeDef,
     UnauthenticatedTypeDef,
+    TlsTypeDef,
     ClientVpcConnectionTypeDef,
     StateInfoTypeDef,
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
+    ClusterOperationV2SummaryTypeDef,
     CompatibleKafkaVersionTypeDef,
-    ConfigurationInfoOutputTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
-    PublicAccessOutputTypeDef,
     PublicAccessTypeDef,
-    CreateClusterResponseTypeDef,
-    CreateClusterV2ResponseTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateVpcConnectionRequestRequestTypeDef,
-    CreateVpcConnectionResponseTypeDef,
     DeleteClusterPolicyRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
-    DeleteClusterResponseTypeDef,
     DeleteConfigurationRequestRequestTypeDef,
-    DeleteConfigurationResponseTypeDef,
     DeleteVpcConnectionRequestRequestTypeDef,
-    DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationRequestRequestTypeDef,
+    DescribeClusterOperationV2RequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeClusterV2RequestRequestTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
-    DescribeConfigurationRevisionResponseTypeDef,
     DescribeVpcConnectionRequestRequestTypeDef,
-    DescribeVpcConnectionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionAtRestOutputTypeDef,
     EncryptionAtRestTypeDef,
-    EncryptionInTransitOutputTypeDef,
     EncryptionInTransitTypeDef,
     GetBootstrapBrokersRequestRequestTypeDef,
-    GetBootstrapBrokersResponseTypeDef,
     GetClusterPolicyRequestRequestTypeDef,
-    GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsRequestRequestTypeDef,
-    IamOutputTypeDef,
     IamTypeDef,
-    JmxExporterInfoOutputTypeDef,
     JmxExporterInfoTypeDef,
     JmxExporterTypeDef,
     KafkaVersionTypeDef,
-    ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListClientVpcConnectionsRequestRequestTypeDef,
-    ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     ListClusterOperationsRequestRequestTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
+    ListClusterOperationsV2RequestRequestTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersV2RequestListClustersV2PaginateTypeDef,
     ListClustersV2RequestRequestTypeDef,
-    ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
-    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
     ListConfigurationsRequestRequestTypeDef,
-    ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
     ListKafkaVersionsRequestRequestTypeDef,
-    ListNodesRequestListNodesPaginateTypeDef,
     ListNodesRequestRequestTypeDef,
-    ListScramSecretsRequestListScramSecretsPaginateTypeDef,
     ListScramSecretsRequestRequestTypeDef,
-    ListScramSecretsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
     ListVpcConnectionsRequestRequestTypeDef,
     VpcConnectionTypeDef,
-    NodeExporterInfoOutputTypeDef,
     NodeExporterInfoTypeDef,
     NodeExporterTypeDef,
     ZookeeperNodeInfoTypeDef,
-    PaginatorConfigTypeDef,
     PutClusterPolicyRequestRequestTypeDef,
-    PutClusterPolicyResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
-    RebootBrokerResponseTypeDef,
     RejectClientVpcConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ScramOutputTypeDef,
     ScramTypeDef,
     VpcConfigTypeDef,
     VpcConfigOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
+    UpdateBrokerTypeRequestRequestTypeDef,
+    UpdateConfigurationRequestRequestTypeDef,
+    UserIdentityTypeDef,
+    VpcConnectivityTlsTypeDef,
+    VpcConnectivityIamTypeDef,
+    VpcConnectivityScramTypeDef,
+    CreateClusterResponseTypeDef,
+    CreateClusterV2ResponseTypeDef,
+    CreateVpcConnectionResponseTypeDef,
+    DeleteClusterResponseTypeDef,
+    DeleteConfigurationResponseTypeDef,
+    DeleteVpcConnectionResponseTypeDef,
+    DescribeConfigurationRevisionResponseTypeDef,
+    DescribeVpcConnectionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetBootstrapBrokersResponseTypeDef,
+    GetClusterPolicyResponseTypeDef,
+    ListScramSecretsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutClusterPolicyResponseTypeDef,
+    RebootBrokerResponseTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
-    UpdateBrokerTypeRequestRequestTypeDef,
     UpdateBrokerTypeResponseTypeDef,
     UpdateClusterConfigurationResponseTypeDef,
     UpdateClusterKafkaVersionResponseTypeDef,
-    UpdateConfigurationRequestRequestTypeDef,
     UpdateConnectivityResponseTypeDef,
     UpdateMonitoringResponseTypeDef,
     UpdateSecurityResponseTypeDef,
     UpdateStorageResponseTypeDef,
-    UserIdentityTypeDef,
-    VpcConnectivityTlsOutputTypeDef,
-    VpcConnectivityTlsTypeDef,
-    VpcConnectivityIamOutputTypeDef,
-    VpcConnectivityIamTypeDef,
-    VpcConnectivityScramOutputTypeDef,
-    VpcConnectivityScramTypeDef,
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
-    BrokerEBSVolumeInfoOutputTypeDef,
-    EBSStorageInfoOutputTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
-    BrokerLogsOutputTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
     ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
+    ListClusterOperationsV2ResponseTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     UpdateClusterConfigurationRequestRequestTypeDef,
     UpdateClusterKafkaVersionRequestRequestTypeDef,
     ConfigurationTypeDef,
     CreateConfigurationResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
-    EncryptionInfoOutputTypeDef,
     EncryptionInfoTypeDef,
-    ServerlessSaslOutputTypeDef,
     ServerlessSaslTypeDef,
     ListKafkaVersionsResponseTypeDef,
+    ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+    ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
+    ListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListClustersV2RequestListClustersV2PaginateTypeDef,
+    ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
+    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
+    ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
+    ListNodesRequestListNodesPaginateTypeDef,
+    ListScramSecretsRequestListScramSecretsPaginateTypeDef,
+    ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
     ListVpcConnectionsResponseTypeDef,
-    PrometheusInfoOutputTypeDef,
     PrometheusInfoTypeDef,
     PrometheusTypeDef,
-    SaslOutputTypeDef,
     SaslTypeDef,
+    VpcConnectionInfoServerlessTypeDef,
     VpcConnectionInfoTypeDef,
-    VpcConnectivitySaslOutputTypeDef,
     VpcConnectivitySaslTypeDef,
-    StorageInfoOutputTypeDef,
     UpdateBrokerStorageRequestRequestTypeDef,
     StorageInfoTypeDef,
-    LoggingInfoOutputTypeDef,
     LoggingInfoTypeDef,
     NodeInfoTypeDef,
     ListConfigurationsResponseTypeDef,
-    ServerlessClientAuthenticationOutputTypeDef,
     ServerlessClientAuthenticationTypeDef,
-    OpenMonitoringInfoOutputTypeDef,
     OpenMonitoringInfoTypeDef,
     OpenMonitoringTypeDef,
     ClientAuthenticationOutputTypeDef,
     ClientAuthenticationTypeDef,
-    VpcConnectivityClientAuthenticationOutputTypeDef,
+    ClusterOperationV2ServerlessTypeDef,
     VpcConnectivityClientAuthenticationTypeDef,
     ListNodesResponseTypeDef,
-    ServerlessTypeDef,
     ServerlessRequestTypeDef,
+    ServerlessTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
     UpdateSecurityRequestRequestTypeDef,
-    VpcConnectivityOutputTypeDef,
     VpcConnectivityTypeDef,
-    ConnectivityInfoOutputTypeDef,
     ConnectivityInfoTypeDef,
     BrokerNodeGroupInfoOutputTypeDef,
-    MutableClusterInfoTypeDef,
     BrokerNodeGroupInfoTypeDef,
+    MutableClusterInfoTypeDef,
     UpdateConnectivityRequestRequestTypeDef,
     ClusterInfoTypeDef,
     ProvisionedTypeDef,
-    ClusterOperationInfoTypeDef,
     CreateClusterRequestRequestTypeDef,
     ProvisionedRequestTypeDef,
+    ClusterOperationInfoTypeDef,
+    ClusterOperationV2ProvisionedTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
     ClusterTypeDef,
+    CreateClusterV2RequestRequestTypeDef,
     DescribeClusterOperationResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
-    CreateClusterV2RequestRequestTypeDef,
+    ClusterOperationV2TypeDef,
     DescribeClusterV2ResponseTypeDef,
     ListClustersV2ResponseTypeDef,
+    DescribeClusterOperationV2ResponseTypeDef,
 )
 
 
 def get_structure() -> BatchAssociateScramSecretRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-kafka-1.28.12/mypy_boto3_kafka.egg-info/SOURCES.txt` & `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.12/setup.py` & `mypy-boto3-kafka-1.28.15/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kafka",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_kafka"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Kafka 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Kafka 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

