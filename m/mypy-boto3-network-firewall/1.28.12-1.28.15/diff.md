# Comparing `tmp/mypy-boto3-network-firewall-1.28.12.tar.gz` & `tmp/mypy-boto3-network-firewall-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-network-firewall-1.28.12.tar", last modified: Thu Jul 27 05:35:05 2023, max compression
+gzip compressed data, was "mypy-boto3-network-firewall-1.28.15.tar", last modified: Fri Jul 28 20:43:21 2023, max compression
```

## Comparing `mypy-boto3-network-firewall-1.28.12.tar` & `mypy-boto3-network-firewall-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:05.136426 mypy-boto3-network-firewall-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-07-27 05:35:05.136426 mypy-boto3-network-firewall-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:05.132426 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32089 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32041 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59450 2023-07-27 05:26:58.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59378 2023-07-27 05:26:56.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:05.136426 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-07-27 05:35:04.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:35:04.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:04.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:35:04.000000 mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:05.136426 mypy-boto3-network-firewall-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-27 05:26:55.000000 mypy-boto3-network-firewall-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.797563 mypy-boto3-network-firewall-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-07-28 20:43:21.793563 mypy-boto3-network-firewall-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18743 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.793563 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32089 2023-07-28 20:32:24.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32041 2023-07-28 20:32:24.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-07-28 20:32:24.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-28 20:32:24.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-28 20:32:24.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-28 20:32:24.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55242 2023-07-28 20:32:28.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55176 2023-07-28 20:32:27.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.793563 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-07-28 20:43:21.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-28 20:43:21.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:21.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:43:21.000000 mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:21.797563 mypy-boto3-network-firewall-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-28 20:32:23.000000 mypy-boto3-network-firewall-1.28.15/setup.py
```

### Comparing `mypy-boto3-network-firewall-1.28.12/LICENSE` & `mypy-boto3-network-firewall-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.12/PKG-INFO` & `mypy-boto3-network-firewall-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-network-firewall
-Version: 1.28.12
-Summary: Type annotations for boto3.NetworkFirewall 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.NetworkFirewall 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-network-firewall)](https://pepy.tech/project/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,187 +361,172 @@
 ### Typed dictionaries
 
 `mypy_boto3_network_firewall.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_network_firewall.type_defs import (
-    AddressOutputTypeDef,
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
-    AssociateFirewallPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     SubnetMappingTypeDef,
-    SubnetMappingOutputTypeDef,
     AttachmentTypeDef,
     IPSetMetadataTypeDef,
     EncryptionConfigurationTypeDef,
     TagTypeDef,
     SourceMetadataTypeDef,
     DeleteFirewallPolicyRequestRequestTypeDef,
     DeleteFirewallRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallRequestRequestTypeDef,
     DescribeLoggingConfigurationRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataRequestRequestTypeDef,
-    StatefulRuleOptionsOutputTypeDef,
+    StatefulRuleOptionsTypeDef,
     DescribeRuleGroupRequestRequestTypeDef,
     DescribeTLSInspectionConfigurationRequestRequestTypeDef,
-    DimensionOutputTypeDef,
     DimensionTypeDef,
     DisassociateSubnetsRequestRequestTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     FirewallMetadataTypeDef,
     FirewallPolicyMetadataTypeDef,
-    StatefulEngineOptionsOutputTypeDef,
-    StatelessRuleGroupReferenceOutputTypeDef,
-    TagOutputTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupReferenceTypeDef,
-    HeaderOutputTypeDef,
     HeaderTypeDef,
     IPSetOutputTypeDef,
-    IPSetReferenceOutputTypeDef,
     IPSetReferenceTypeDef,
     IPSetTypeDef,
-    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListFirewallPoliciesRequestRequestTypeDef,
-    ListFirewallsRequestListFirewallsPaginateTypeDef,
     ListFirewallsRequestRequestTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupMetadataTypeDef,
-    ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
     ListTLSInspectionConfigurationsRequestRequestTypeDef,
     TLSInspectionConfigurationMetadataTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     LogDestinationConfigOutputTypeDef,
     LogDestinationConfigTypeDef,
-    PortRangeOutputTypeDef,
-    TCPFlagFieldOutputTypeDef,
     PortRangeTypeDef,
+    TCPFlagFieldOutputTypeDef,
     TCPFlagFieldTypeDef,
-    PaginatorConfigTypeDef,
     PerObjectStatusTypeDef,
     PortSetOutputTypeDef,
     PortSetTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SourceMetadataOutputTypeDef,
-    StatefulRuleOptionsTypeDef,
     RuleOptionOutputTypeDef,
     RuleOptionTypeDef,
     RulesSourceListOutputTypeDef,
     RulesSourceListTypeDef,
-    ServerCertificateOutputTypeDef,
     ServerCertificateTypeDef,
-    StatefulRuleGroupOverrideOutputTypeDef,
     StatefulRuleGroupOverrideTypeDef,
     TlsCertificateDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionRequestRequestTypeDef,
-    UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionRequestRequestTypeDef,
-    UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
-    UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateSubnetChangeProtectionRequestRequestTypeDef,
+    AssociateFirewallPolicyResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    UpdateFirewallDeleteProtectionResponseTypeDef,
+    UpdateFirewallDescriptionResponseTypeDef,
+    UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateSubnetChangeProtectionResponseTypeDef,
     AssociateSubnetsRequestRequestTypeDef,
     AssociateSubnetsResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     CIDRSummaryTypeDef,
     UpdateFirewallEncryptionConfigurationRequestRequestTypeDef,
+    UpdateFirewallEncryptionConfigurationResponseTypeDef,
     CreateFirewallRequestRequestTypeDef,
+    FirewallPolicyResponseTypeDef,
+    FirewallTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    RuleGroupResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     PublishMetricActionOutputTypeDef,
     PublishMetricActionTypeDef,
-    UpdateFirewallEncryptionConfigurationResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListFirewallPoliciesResponseTypeDef,
-    FirewallPolicyResponseTypeDef,
-    FirewallTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PolicyVariablesOutputTypeDef,
     ReferenceSetsOutputTypeDef,
     ReferenceSetsTypeDef,
     PolicyVariablesTypeDef,
+    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
+    ListFirewallsRequestListFirewallsPaginateTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
+    ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     ServerCertificateScopeOutputTypeDef,
-    MatchAttributesOutputTypeDef,
     ServerCertificateScopeTypeDef,
+    MatchAttributesOutputTypeDef,
     MatchAttributesTypeDef,
     SyncStateTypeDef,
     RuleVariablesOutputTypeDef,
     RuleVariablesTypeDef,
-    RuleGroupResponseTypeDef,
     StatefulRuleOutputTypeDef,
     StatefulRuleTypeDef,
-    StatefulRuleGroupReferenceOutputTypeDef,
     StatefulRuleGroupReferenceTypeDef,
     TLSInspectionConfigurationResponseTypeDef,
     CapacityUsageSummaryTypeDef,
-    ActionDefinitionOutputTypeDef,
-    ActionDefinitionTypeDef,
     CreateFirewallPolicyResponseTypeDef,
     DeleteFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
+    CreateRuleGroupResponseTypeDef,
+    DeleteRuleGroupResponseTypeDef,
+    UpdateRuleGroupResponseTypeDef,
+    ActionDefinitionOutputTypeDef,
+    ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
     ServerCertificateConfigurationOutputTypeDef,
-    RuleDefinitionOutputTypeDef,
     ServerCertificateConfigurationTypeDef,
+    RuleDefinitionOutputTypeDef,
     RuleDefinitionTypeDef,
-    CreateRuleGroupResponseTypeDef,
-    DeleteRuleGroupResponseTypeDef,
-    UpdateRuleGroupResponseTypeDef,
     CreateTLSInspectionConfigurationResponseTypeDef,
     DeleteTLSInspectionConfigurationResponseTypeDef,
     UpdateTLSInspectionConfigurationResponseTypeDef,
     FirewallStatusTypeDef,
     CustomActionOutputTypeDef,
     CustomActionTypeDef,
     TLSInspectionConfigurationOutputTypeDef,
-    StatelessRuleOutputTypeDef,
     TLSInspectionConfigurationTypeDef,
+    StatelessRuleOutputTypeDef,
     StatelessRuleTypeDef,
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
     FirewallPolicyOutputTypeDef,
     FirewallPolicyTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
-    StatelessRulesAndCustomActionsOutputTypeDef,
     CreateTLSInspectionConfigurationRequestRequestTypeDef,
     UpdateTLSInspectionConfigurationRequestRequestTypeDef,
+    StatelessRulesAndCustomActionsOutputTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
     CreateFirewallPolicyRequestRequestTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
     RulesSourceOutputTypeDef,
     RulesSourceTypeDef,
     RuleGroupOutputTypeDef,
     RuleGroupTypeDef,
     DescribeRuleGroupResponseTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddressOutputTypeDef:
+def get_structure() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-network-firewall-1.28.12/README.md` & `mypy-boto3-network-firewall-1.28.15/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-network-firewall)](https://pepy.tech/project/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,187 +329,172 @@
 ### Typed dictionaries
 
 `mypy_boto3_network_firewall.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_network_firewall.type_defs import (
-    AddressOutputTypeDef,
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
-    AssociateFirewallPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     SubnetMappingTypeDef,
-    SubnetMappingOutputTypeDef,
     AttachmentTypeDef,
     IPSetMetadataTypeDef,
     EncryptionConfigurationTypeDef,
     TagTypeDef,
     SourceMetadataTypeDef,
     DeleteFirewallPolicyRequestRequestTypeDef,
     DeleteFirewallRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallRequestRequestTypeDef,
     DescribeLoggingConfigurationRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataRequestRequestTypeDef,
-    StatefulRuleOptionsOutputTypeDef,
+    StatefulRuleOptionsTypeDef,
     DescribeRuleGroupRequestRequestTypeDef,
     DescribeTLSInspectionConfigurationRequestRequestTypeDef,
-    DimensionOutputTypeDef,
     DimensionTypeDef,
     DisassociateSubnetsRequestRequestTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     FirewallMetadataTypeDef,
     FirewallPolicyMetadataTypeDef,
-    StatefulEngineOptionsOutputTypeDef,
-    StatelessRuleGroupReferenceOutputTypeDef,
-    TagOutputTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupReferenceTypeDef,
-    HeaderOutputTypeDef,
     HeaderTypeDef,
     IPSetOutputTypeDef,
-    IPSetReferenceOutputTypeDef,
     IPSetReferenceTypeDef,
     IPSetTypeDef,
-    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListFirewallPoliciesRequestRequestTypeDef,
-    ListFirewallsRequestListFirewallsPaginateTypeDef,
     ListFirewallsRequestRequestTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupMetadataTypeDef,
-    ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
     ListTLSInspectionConfigurationsRequestRequestTypeDef,
     TLSInspectionConfigurationMetadataTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     LogDestinationConfigOutputTypeDef,
     LogDestinationConfigTypeDef,
-    PortRangeOutputTypeDef,
-    TCPFlagFieldOutputTypeDef,
     PortRangeTypeDef,
+    TCPFlagFieldOutputTypeDef,
     TCPFlagFieldTypeDef,
-    PaginatorConfigTypeDef,
     PerObjectStatusTypeDef,
     PortSetOutputTypeDef,
     PortSetTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SourceMetadataOutputTypeDef,
-    StatefulRuleOptionsTypeDef,
     RuleOptionOutputTypeDef,
     RuleOptionTypeDef,
     RulesSourceListOutputTypeDef,
     RulesSourceListTypeDef,
-    ServerCertificateOutputTypeDef,
     ServerCertificateTypeDef,
-    StatefulRuleGroupOverrideOutputTypeDef,
     StatefulRuleGroupOverrideTypeDef,
     TlsCertificateDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionRequestRequestTypeDef,
-    UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionRequestRequestTypeDef,
-    UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
-    UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateSubnetChangeProtectionRequestRequestTypeDef,
+    AssociateFirewallPolicyResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    UpdateFirewallDeleteProtectionResponseTypeDef,
+    UpdateFirewallDescriptionResponseTypeDef,
+    UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateSubnetChangeProtectionResponseTypeDef,
     AssociateSubnetsRequestRequestTypeDef,
     AssociateSubnetsResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     CIDRSummaryTypeDef,
     UpdateFirewallEncryptionConfigurationRequestRequestTypeDef,
+    UpdateFirewallEncryptionConfigurationResponseTypeDef,
     CreateFirewallRequestRequestTypeDef,
+    FirewallPolicyResponseTypeDef,
+    FirewallTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    RuleGroupResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     PublishMetricActionOutputTypeDef,
     PublishMetricActionTypeDef,
-    UpdateFirewallEncryptionConfigurationResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListFirewallPoliciesResponseTypeDef,
-    FirewallPolicyResponseTypeDef,
-    FirewallTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PolicyVariablesOutputTypeDef,
     ReferenceSetsOutputTypeDef,
     ReferenceSetsTypeDef,
     PolicyVariablesTypeDef,
+    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
+    ListFirewallsRequestListFirewallsPaginateTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
+    ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     ServerCertificateScopeOutputTypeDef,
-    MatchAttributesOutputTypeDef,
     ServerCertificateScopeTypeDef,
+    MatchAttributesOutputTypeDef,
     MatchAttributesTypeDef,
     SyncStateTypeDef,
     RuleVariablesOutputTypeDef,
     RuleVariablesTypeDef,
-    RuleGroupResponseTypeDef,
     StatefulRuleOutputTypeDef,
     StatefulRuleTypeDef,
-    StatefulRuleGroupReferenceOutputTypeDef,
     StatefulRuleGroupReferenceTypeDef,
     TLSInspectionConfigurationResponseTypeDef,
     CapacityUsageSummaryTypeDef,
-    ActionDefinitionOutputTypeDef,
-    ActionDefinitionTypeDef,
     CreateFirewallPolicyResponseTypeDef,
     DeleteFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
+    CreateRuleGroupResponseTypeDef,
+    DeleteRuleGroupResponseTypeDef,
+    UpdateRuleGroupResponseTypeDef,
+    ActionDefinitionOutputTypeDef,
+    ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
     ServerCertificateConfigurationOutputTypeDef,
-    RuleDefinitionOutputTypeDef,
     ServerCertificateConfigurationTypeDef,
+    RuleDefinitionOutputTypeDef,
     RuleDefinitionTypeDef,
-    CreateRuleGroupResponseTypeDef,
-    DeleteRuleGroupResponseTypeDef,
-    UpdateRuleGroupResponseTypeDef,
     CreateTLSInspectionConfigurationResponseTypeDef,
     DeleteTLSInspectionConfigurationResponseTypeDef,
     UpdateTLSInspectionConfigurationResponseTypeDef,
     FirewallStatusTypeDef,
     CustomActionOutputTypeDef,
     CustomActionTypeDef,
     TLSInspectionConfigurationOutputTypeDef,
-    StatelessRuleOutputTypeDef,
     TLSInspectionConfigurationTypeDef,
+    StatelessRuleOutputTypeDef,
     StatelessRuleTypeDef,
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
     FirewallPolicyOutputTypeDef,
     FirewallPolicyTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
-    StatelessRulesAndCustomActionsOutputTypeDef,
     CreateTLSInspectionConfigurationRequestRequestTypeDef,
     UpdateTLSInspectionConfigurationRequestRequestTypeDef,
+    StatelessRulesAndCustomActionsOutputTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
     CreateFirewallPolicyRequestRequestTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
     RulesSourceOutputTypeDef,
     RulesSourceTypeDef,
     RuleGroupOutputTypeDef,
     RuleGroupTypeDef,
     DescribeRuleGroupResponseTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddressOutputTypeDef:
+def get_structure() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/__init__.py` & `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/__init__.pyi` & `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/__main__.py` & `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.NetworkFirewall 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.NetworkFirewall 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall\nOther"
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

### Comparing `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/client.py` & `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/client.pyi` & `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/literals.py` & `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/literals.pyi` & `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/paginator.py` & `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,96 +45,89 @@
     "ListFirewallPoliciesPaginator",
     "ListFirewallsPaginator",
     "ListRuleGroupsPaginator",
     "ListTLSInspectionConfigurationsPaginator",
     "ListTagsForResourcePaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListFirewallPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewallPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewallPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallpoliciespaginator)
         """
 
-
 class ListFirewallsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewalls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallspaginator)
     """
 
     def paginate(
-        self, *, VpcIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, VpcIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewalls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallspaginator)
         """
 
-
 class ListRuleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListRuleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listrulegroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
         Type: RuleGroupTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListRuleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listrulegroupspaginator)
         """
 
-
 class ListTLSInspectionConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTLSInspectionConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtlsinspectionconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTLSInspectionConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTLSInspectionConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtlsinspectionconfigurationspaginator)
         """
 
-
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/paginator.pyi` & `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,89 +45,96 @@
     "ListFirewallPoliciesPaginator",
     "ListFirewallsPaginator",
     "ListRuleGroupsPaginator",
     "ListTLSInspectionConfigurationsPaginator",
     "ListTagsForResourcePaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListFirewallPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewallPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewallPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallpoliciespaginator)
         """
 
+
 class ListFirewallsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewalls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallspaginator)
     """
 
     def paginate(
-        self, *, VpcIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, VpcIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewalls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listfirewallspaginator)
         """
 
+
 class ListRuleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListRuleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listrulegroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Scope: ResourceManagedStatusType = ...,
         ManagedType: ResourceManagedTypeType = ...,
         Type: RuleGroupTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListRuleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listrulegroupspaginator)
         """
 
+
 class ListTLSInspectionConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTLSInspectionConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtlsinspectionconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTLSInspectionConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTLSInspectionConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtlsinspectionconfigurationspaginator)
         """
 
+
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/type_defs.py` & `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for network-firewall service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_network_firewall.type_defs import AddressOutputTypeDef
+    from mypy_boto3_network_firewall.type_defs import AddressTypeDef
 
-    data: AddressOutputTypeDef = {...}
+    data: AddressTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -45,192 +45,170 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AddressOutputTypeDef",
     "AddressTypeDef",
     "AssociateFirewallPolicyRequestRequestTypeDef",
-    "AssociateFirewallPolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SubnetMappingTypeDef",
-    "SubnetMappingOutputTypeDef",
     "AttachmentTypeDef",
     "IPSetMetadataTypeDef",
     "EncryptionConfigurationTypeDef",
     "TagTypeDef",
     "SourceMetadataTypeDef",
     "DeleteFirewallPolicyRequestRequestTypeDef",
     "DeleteFirewallRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteTLSInspectionConfigurationRequestRequestTypeDef",
     "DescribeFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallRequestRequestTypeDef",
     "DescribeLoggingConfigurationRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
-    "StatefulRuleOptionsOutputTypeDef",
+    "StatefulRuleOptionsTypeDef",
     "DescribeRuleGroupRequestRequestTypeDef",
     "DescribeTLSInspectionConfigurationRequestRequestTypeDef",
-    "DimensionOutputTypeDef",
     "DimensionTypeDef",
     "DisassociateSubnetsRequestRequestTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "FirewallMetadataTypeDef",
     "FirewallPolicyMetadataTypeDef",
-    "StatefulEngineOptionsOutputTypeDef",
-    "StatelessRuleGroupReferenceOutputTypeDef",
-    "TagOutputTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupReferenceTypeDef",
-    "HeaderOutputTypeDef",
     "HeaderTypeDef",
     "IPSetOutputTypeDef",
-    "IPSetReferenceOutputTypeDef",
     "IPSetReferenceTypeDef",
     "IPSetTypeDef",
-    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListFirewallPoliciesRequestRequestTypeDef",
-    "ListFirewallsRequestListFirewallsPaginateTypeDef",
     "ListFirewallsRequestRequestTypeDef",
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupMetadataTypeDef",
-    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
     "ListTLSInspectionConfigurationsRequestRequestTypeDef",
     "TLSInspectionConfigurationMetadataTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "LogDestinationConfigOutputTypeDef",
     "LogDestinationConfigTypeDef",
-    "PortRangeOutputTypeDef",
-    "TCPFlagFieldOutputTypeDef",
     "PortRangeTypeDef",
+    "TCPFlagFieldOutputTypeDef",
     "TCPFlagFieldTypeDef",
-    "PaginatorConfigTypeDef",
     "PerObjectStatusTypeDef",
     "PortSetOutputTypeDef",
     "PortSetTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SourceMetadataOutputTypeDef",
-    "StatefulRuleOptionsTypeDef",
     "RuleOptionOutputTypeDef",
     "RuleOptionTypeDef",
     "RulesSourceListOutputTypeDef",
     "RulesSourceListTypeDef",
-    "ServerCertificateOutputTypeDef",
     "ServerCertificateTypeDef",
-    "StatefulRuleGroupOverrideOutputTypeDef",
     "StatefulRuleGroupOverrideTypeDef",
     "TlsCertificateDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallDeleteProtectionRequestRequestTypeDef",
-    "UpdateFirewallDeleteProtectionResponseTypeDef",
     "UpdateFirewallDescriptionRequestRequestTypeDef",
-    "UpdateFirewallDescriptionResponseTypeDef",
     "UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
-    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
     "UpdateSubnetChangeProtectionRequestRequestTypeDef",
+    "AssociateFirewallPolicyResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
+    "UpdateFirewallDeleteProtectionResponseTypeDef",
+    "UpdateFirewallDescriptionResponseTypeDef",
+    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
     "UpdateSubnetChangeProtectionResponseTypeDef",
     "AssociateSubnetsRequestRequestTypeDef",
     "AssociateSubnetsResponseTypeDef",
     "DisassociateSubnetsResponseTypeDef",
     "CIDRSummaryTypeDef",
     "UpdateFirewallEncryptionConfigurationRequestRequestTypeDef",
+    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     "CreateFirewallRequestRequestTypeDef",
+    "FirewallPolicyResponseTypeDef",
+    "FirewallTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "RuleGroupResponseTypeDef",
     "DescribeRuleGroupMetadataResponseTypeDef",
     "PublishMetricActionOutputTypeDef",
     "PublishMetricActionTypeDef",
-    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     "ListFirewallsResponseTypeDef",
     "ListFirewallPoliciesResponseTypeDef",
-    "FirewallPolicyResponseTypeDef",
-    "FirewallTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PolicyVariablesOutputTypeDef",
     "ReferenceSetsOutputTypeDef",
     "ReferenceSetsTypeDef",
     "PolicyVariablesTypeDef",
+    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
+    "ListFirewallsRequestListFirewallsPaginateTypeDef",
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "ListTLSInspectionConfigurationsResponseTypeDef",
     "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "ServerCertificateScopeOutputTypeDef",
-    "MatchAttributesOutputTypeDef",
     "ServerCertificateScopeTypeDef",
+    "MatchAttributesOutputTypeDef",
     "MatchAttributesTypeDef",
     "SyncStateTypeDef",
     "RuleVariablesOutputTypeDef",
     "RuleVariablesTypeDef",
-    "RuleGroupResponseTypeDef",
     "StatefulRuleOutputTypeDef",
     "StatefulRuleTypeDef",
-    "StatefulRuleGroupReferenceOutputTypeDef",
     "StatefulRuleGroupReferenceTypeDef",
     "TLSInspectionConfigurationResponseTypeDef",
     "CapacityUsageSummaryTypeDef",
-    "ActionDefinitionOutputTypeDef",
-    "ActionDefinitionTypeDef",
     "CreateFirewallPolicyResponseTypeDef",
     "DeleteFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyResponseTypeDef",
+    "CreateRuleGroupResponseTypeDef",
+    "DeleteRuleGroupResponseTypeDef",
+    "UpdateRuleGroupResponseTypeDef",
+    "ActionDefinitionOutputTypeDef",
+    "ActionDefinitionTypeDef",
     "DescribeLoggingConfigurationResponseTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     "ServerCertificateConfigurationOutputTypeDef",
-    "RuleDefinitionOutputTypeDef",
     "ServerCertificateConfigurationTypeDef",
+    "RuleDefinitionOutputTypeDef",
     "RuleDefinitionTypeDef",
-    "CreateRuleGroupResponseTypeDef",
-    "DeleteRuleGroupResponseTypeDef",
-    "UpdateRuleGroupResponseTypeDef",
     "CreateTLSInspectionConfigurationResponseTypeDef",
     "DeleteTLSInspectionConfigurationResponseTypeDef",
     "UpdateTLSInspectionConfigurationResponseTypeDef",
     "FirewallStatusTypeDef",
     "CustomActionOutputTypeDef",
     "CustomActionTypeDef",
     "TLSInspectionConfigurationOutputTypeDef",
-    "StatelessRuleOutputTypeDef",
     "TLSInspectionConfigurationTypeDef",
+    "StatelessRuleOutputTypeDef",
     "StatelessRuleTypeDef",
     "CreateFirewallResponseTypeDef",
     "DeleteFirewallResponseTypeDef",
     "DescribeFirewallResponseTypeDef",
     "FirewallPolicyOutputTypeDef",
     "FirewallPolicyTypeDef",
     "DescribeTLSInspectionConfigurationResponseTypeDef",
-    "StatelessRulesAndCustomActionsOutputTypeDef",
     "CreateTLSInspectionConfigurationRequestRequestTypeDef",
     "UpdateTLSInspectionConfigurationRequestRequestTypeDef",
+    "StatelessRulesAndCustomActionsOutputTypeDef",
     "StatelessRulesAndCustomActionsTypeDef",
     "DescribeFirewallPolicyResponseTypeDef",
     "CreateFirewallPolicyRequestRequestTypeDef",
     "UpdateFirewallPolicyRequestRequestTypeDef",
     "RulesSourceOutputTypeDef",
     "RulesSourceTypeDef",
     "RuleGroupOutputTypeDef",
     "RuleGroupTypeDef",
     "DescribeRuleGroupResponseTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
 )
 
-AddressOutputTypeDef = TypedDict(
-    "AddressOutputTypeDef",
-    {
-        "AddressDefinition": str,
-    },
-)
-
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressDefinition": str,
     },
 )
 
@@ -254,22 +232,22 @@
 class AssociateFirewallPolicyRequestRequestTypeDef(
     _RequiredAssociateFirewallPolicyRequestRequestTypeDef,
     _OptionalAssociateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateFirewallPolicyResponseTypeDef = TypedDict(
-    "AssociateFirewallPolicyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "FirewallPolicyArn": str,
-        "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredSubnetMappingTypeDef = TypedDict(
     "_RequiredSubnetMappingTypeDef",
     {
         "SubnetId": str,
@@ -284,35 +262,14 @@
 )
 
 
 class SubnetMappingTypeDef(_RequiredSubnetMappingTypeDef, _OptionalSubnetMappingTypeDef):
     pass
 
 
-_RequiredSubnetMappingOutputTypeDef = TypedDict(
-    "_RequiredSubnetMappingOutputTypeDef",
-    {
-        "SubnetId": str,
-    },
-)
-_OptionalSubnetMappingOutputTypeDef = TypedDict(
-    "_OptionalSubnetMappingOutputTypeDef",
-    {
-        "IPAddressType": IPAddressTypeType,
-    },
-    total=False,
-)
-
-
-class SubnetMappingOutputTypeDef(
-    _RequiredSubnetMappingOutputTypeDef, _OptionalSubnetMappingOutputTypeDef
-):
-    pass
-
-
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "SubnetId": str,
         "EndpointId": str,
         "Status": AttachmentStatusType,
         "StatusMessage": str,
@@ -440,34 +397,26 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRuleGroupMetadataRequestRequestTypeDef = TypedDict(
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
     {
         "RuleGroupName": str,
         "RuleGroupArn": str,
         "Type": RuleGroupTypeType,
     },
     total=False,
 )
 
-StatefulRuleOptionsOutputTypeDef = TypedDict(
-    "StatefulRuleOptionsOutputTypeDef",
+StatefulRuleOptionsTypeDef = TypedDict(
+    "StatefulRuleOptionsTypeDef",
     {
         "RuleOrder": RuleOrderType,
     },
     total=False,
 )
 
 DescribeRuleGroupRequestRequestTypeDef = TypedDict(
@@ -485,21 +434,14 @@
     {
         "TLSInspectionConfigurationArn": str,
         "TLSInspectionConfigurationName": str,
     },
     total=False,
 )
 
-DimensionOutputTypeDef = TypedDict(
-    "DimensionOutputTypeDef",
-    {
-        "Value": str,
-    },
-)
-
 DimensionTypeDef = TypedDict(
     "DimensionTypeDef",
     {
         "Value": str,
     },
 )
 
@@ -523,35 +465,14 @@
 class DisassociateSubnetsRequestRequestTypeDef(
     _RequiredDisassociateSubnetsRequestRequestTypeDef,
     _OptionalDisassociateSubnetsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEncryptionConfigurationOutputTypeDef",
-    {
-        "Type": EncryptionTypeType,
-    },
-)
-_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEncryptionConfigurationOutputTypeDef",
-    {
-        "KeyId": str,
-    },
-    total=False,
-)
-
-
-class EncryptionConfigurationOutputTypeDef(
-    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
-):
-    pass
-
-
 FirewallMetadataTypeDef = TypedDict(
     "FirewallMetadataTypeDef",
     {
         "FirewallName": str,
         "FirewallArn": str,
     },
     total=False,
@@ -562,39 +483,14 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
-StatefulEngineOptionsOutputTypeDef = TypedDict(
-    "StatefulEngineOptionsOutputTypeDef",
-    {
-        "RuleOrder": RuleOrderType,
-        "StreamExceptionPolicy": StreamExceptionPolicyType,
-    },
-    total=False,
-)
-
-StatelessRuleGroupReferenceOutputTypeDef = TypedDict(
-    "StatelessRuleGroupReferenceOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "Priority": int,
-    },
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
 StatefulEngineOptionsTypeDef = TypedDict(
     "StatefulEngineOptionsTypeDef",
     {
         "RuleOrder": RuleOrderType,
         "StreamExceptionPolicy": StreamExceptionPolicyType,
     },
     total=False,
@@ -604,26 +500,14 @@
     "StatelessRuleGroupReferenceTypeDef",
     {
         "ResourceArn": str,
         "Priority": int,
     },
 )
 
-HeaderOutputTypeDef = TypedDict(
-    "HeaderOutputTypeDef",
-    {
-        "Protocol": StatefulRuleProtocolType,
-        "Source": str,
-        "SourcePort": str,
-        "Direction": StatefulRuleDirectionType,
-        "Destination": str,
-        "DestinationPort": str,
-    },
-)
-
 HeaderTypeDef = TypedDict(
     "HeaderTypeDef",
     {
         "Protocol": StatefulRuleProtocolType,
         "Source": str,
         "SourcePort": str,
         "Direction": StatefulRuleDirectionType,
@@ -635,22 +519,14 @@
 IPSetOutputTypeDef = TypedDict(
     "IPSetOutputTypeDef",
     {
         "Definition": List[str],
     },
 )
 
-IPSetReferenceOutputTypeDef = TypedDict(
-    "IPSetReferenceOutputTypeDef",
-    {
-        "ReferenceArn": str,
-    },
-    total=False,
-)
-
 IPSetReferenceTypeDef = TypedDict(
     "IPSetReferenceTypeDef",
     {
         "ReferenceArn": str,
     },
     total=False,
 )
@@ -658,61 +534,43 @@
 IPSetTypeDef = TypedDict(
     "IPSetTypeDef",
     {
         "Definition": Sequence[str],
     },
 )
 
-ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef = TypedDict(
-    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
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
 
 ListFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "ListFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListFirewallsRequestListFirewallsPaginateTypeDef = TypedDict(
-    "ListFirewallsRequestListFirewallsPaginateTypeDef",
-    {
-        "VpcIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFirewallsRequestRequestTypeDef = TypedDict(
     "ListFirewallsRequestRequestTypeDef",
     {
         "NextToken": str,
         "VpcIds": Sequence[str],
         "MaxResults": int,
     },
     total=False,
 )
 
-ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
-    {
-        "Scope": ResourceManagedStatusType,
-        "ManagedType": ResourceManagedTypeType,
-        "Type": RuleGroupTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Scope": ResourceManagedStatusType,
         "ManagedType": ResourceManagedTypeType,
@@ -726,22 +584,14 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
-ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef = TypedDict(
-    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTLSInspectionConfigurationsRequestRequestTypeDef = TypedDict(
     "ListTLSInspectionConfigurationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -752,36 +602,14 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
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
@@ -815,16 +643,16 @@
     {
         "LogType": LogTypeType,
         "LogDestinationType": LogDestinationTypeType,
         "LogDestination": Mapping[str, str],
     },
 )
 
-PortRangeOutputTypeDef = TypedDict(
-    "PortRangeOutputTypeDef",
+PortRangeTypeDef = TypedDict(
+    "PortRangeTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
 )
 
 _RequiredTCPFlagFieldOutputTypeDef = TypedDict(
@@ -844,22 +672,14 @@
 
 class TCPFlagFieldOutputTypeDef(
     _RequiredTCPFlagFieldOutputTypeDef, _OptionalTCPFlagFieldOutputTypeDef
 ):
     pass
 
 
-PortRangeTypeDef = TypedDict(
-    "PortRangeTypeDef",
-    {
-        "FromPort": int,
-        "ToPort": int,
-    },
-)
-
 _RequiredTCPFlagFieldTypeDef = TypedDict(
     "_RequiredTCPFlagFieldTypeDef",
     {
         "Flags": Sequence[TCPFlagType],
     },
 )
 _OptionalTCPFlagFieldTypeDef = TypedDict(
@@ -871,24 +691,14 @@
 )
 
 
 class TCPFlagFieldTypeDef(_RequiredTCPFlagFieldTypeDef, _OptionalTCPFlagFieldTypeDef):
     pass
 
 
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
 PerObjectStatusTypeDef = TypedDict(
     "PerObjectStatusTypeDef",
     {
         "SyncStatus": PerObjectSyncStatusType,
         "UpdateToken": str,
     },
     total=False,
@@ -914,42 +724,14 @@
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
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
-SourceMetadataOutputTypeDef = TypedDict(
-    "SourceMetadataOutputTypeDef",
-    {
-        "SourceArn": str,
-        "SourceUpdateToken": str,
-    },
-    total=False,
-)
-
-StatefulRuleOptionsTypeDef = TypedDict(
-    "StatefulRuleOptionsTypeDef",
-    {
-        "RuleOrder": RuleOrderType,
-    },
-    total=False,
-)
-
 _RequiredRuleOptionOutputTypeDef = TypedDict(
     "_RequiredRuleOptionOutputTypeDef",
     {
         "Keyword": str,
     },
 )
 _OptionalRuleOptionOutputTypeDef = TypedDict(
@@ -998,38 +780,22 @@
     {
         "Targets": Sequence[str],
         "TargetTypes": Sequence[TargetTypeType],
         "GeneratedRulesType": GeneratedRulesTypeType,
     },
 )
 
-ServerCertificateOutputTypeDef = TypedDict(
-    "ServerCertificateOutputTypeDef",
-    {
-        "ResourceArn": str,
-    },
-    total=False,
-)
-
 ServerCertificateTypeDef = TypedDict(
     "ServerCertificateTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
 
-StatefulRuleGroupOverrideOutputTypeDef = TypedDict(
-    "StatefulRuleGroupOverrideOutputTypeDef",
-    {
-        "Action": Literal["DROP_TO_ALERT"],
-    },
-    total=False,
-)
-
 StatefulRuleGroupOverrideTypeDef = TypedDict(
     "StatefulRuleGroupOverrideTypeDef",
     {
         "Action": Literal["DROP_TO_ALERT"],
     },
     total=False,
 )
@@ -1073,47 +839,25 @@
 class UpdateFirewallDeleteProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallDeleteProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallDeleteProtectionRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateFirewallDeleteProtectionResponseTypeDef = TypedDict(
-    "UpdateFirewallDeleteProtectionResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "DeleteProtection": bool,
-        "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateFirewallDescriptionRequestRequestTypeDef = TypedDict(
     "UpdateFirewallDescriptionRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "Description": str,
     },
     total=False,
 )
 
-UpdateFirewallDescriptionResponseTypeDef = TypedDict(
-    "UpdateFirewallDescriptionResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "Description": str,
-        "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
     {
         "FirewallPolicyChangeProtection": bool,
     },
 )
 _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -1130,25 +874,14 @@
 class UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateFirewallPolicyChangeProtectionResponseTypeDef = TypedDict(
-    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "FirewallArn": str,
-        "FirewallName": str,
-        "FirewallPolicyChangeProtection": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef",
     {
         "SubnetChangeProtection": bool,
     },
 )
 _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -1165,22 +898,74 @@
 class UpdateSubnetChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
 
+AssociateFirewallPolicyResponseTypeDef = TypedDict(
+    "AssociateFirewallPolicyResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "FirewallPolicyArn": str,
+        "UpdateToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallDeleteProtectionResponseTypeDef = TypedDict(
+    "UpdateFirewallDeleteProtectionResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "DeleteProtection": bool,
+        "UpdateToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallDescriptionResponseTypeDef = TypedDict(
+    "UpdateFirewallDescriptionResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "Description": str,
+        "UpdateToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallPolicyChangeProtectionResponseTypeDef = TypedDict(
+    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "FirewallArn": str,
+        "FirewallName": str,
+        "FirewallPolicyChangeProtection": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSubnetChangeProtectionResponseTypeDef = TypedDict(
     "UpdateSubnetChangeProtectionResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetChangeProtection": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssociateSubnetsRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateSubnetsRequestRequestTypeDef",
     {
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
@@ -1204,28 +989,28 @@
 
 
 AssociateSubnetsResponseTypeDef = TypedDict(
     "AssociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
-        "SubnetMappings": List[SubnetMappingOutputTypeDef],
+        "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateSubnetsResponseTypeDef = TypedDict(
     "DisassociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
-        "SubnetMappings": List[SubnetMappingOutputTypeDef],
+        "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CIDRSummaryTypeDef = TypedDict(
     "CIDRSummaryTypeDef",
     {
         "AvailableCIDRCount": int,
@@ -1242,14 +1027,25 @@
         "FirewallArn": str,
         "FirewallName": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+UpdateFirewallEncryptionConfigurationResponseTypeDef = TypedDict(
+    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "UpdateToken": str,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateFirewallRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRequestRequestTypeDef",
     {
         "FirewallName": str,
         "FirewallPolicyArn": str,
         "VpcId": str,
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
@@ -1271,97 +1067,32 @@
 
 class CreateFirewallRequestRequestTypeDef(
     _RequiredCreateFirewallRequestRequestTypeDef, _OptionalCreateFirewallRequestRequestTypeDef
 ):
     pass
 
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-DescribeRuleGroupMetadataResponseTypeDef = TypedDict(
-    "DescribeRuleGroupMetadataResponseTypeDef",
-    {
-        "RuleGroupArn": str,
-        "RuleGroupName": str,
-        "Description": str,
-        "Type": RuleGroupTypeType,
-        "Capacity": int,
-        "StatefulRuleOptions": StatefulRuleOptionsOutputTypeDef,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PublishMetricActionOutputTypeDef = TypedDict(
-    "PublishMetricActionOutputTypeDef",
-    {
-        "Dimensions": List[DimensionOutputTypeDef],
-    },
-)
-
-PublishMetricActionTypeDef = TypedDict(
-    "PublishMetricActionTypeDef",
-    {
-        "Dimensions": Sequence[DimensionTypeDef],
-    },
-)
-
-UpdateFirewallEncryptionConfigurationResponseTypeDef = TypedDict(
-    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "UpdateToken": str,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFirewallsResponseTypeDef = TypedDict(
-    "ListFirewallsResponseTypeDef",
-    {
-        "NextToken": str,
-        "Firewalls": List[FirewallMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFirewallPoliciesResponseTypeDef = TypedDict(
-    "ListFirewallPoliciesResponseTypeDef",
-    {
-        "NextToken": str,
-        "FirewallPolicies": List[FirewallPolicyMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredFirewallPolicyResponseTypeDef = TypedDict(
     "_RequiredFirewallPolicyResponseTypeDef",
     {
         "FirewallPolicyName": str,
         "FirewallPolicyArn": str,
         "FirewallPolicyId": str,
     },
 )
 _OptionalFirewallPolicyResponseTypeDef = TypedDict(
     "_OptionalFirewallPolicyResponseTypeDef",
     {
         "Description": str,
         "FirewallPolicyStatus": ResourceStatusType,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ConsumedStatelessRuleCapacity": int,
         "ConsumedStatefulRuleCapacity": int,
         "NumberOfAssociations": int,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
 
 class FirewallPolicyResponseTypeDef(
@@ -1371,59 +1102,146 @@
 
 
 _RequiredFirewallTypeDef = TypedDict(
     "_RequiredFirewallTypeDef",
     {
         "FirewallPolicyArn": str,
         "VpcId": str,
-        "SubnetMappings": List[SubnetMappingOutputTypeDef],
+        "SubnetMappings": List[SubnetMappingTypeDef],
         "FirewallId": str,
     },
 )
 _OptionalFirewallTypeDef = TypedDict(
     "_OptionalFirewallTypeDef",
     {
         "FirewallName": str,
         "FirewallArn": str,
         "DeleteProtection": bool,
         "SubnetChangeProtection": bool,
         "FirewallPolicyChangeProtection": bool,
         "Description": str,
-        "Tags": List[TagOutputTypeDef],
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "Tags": List[TagTypeDef],
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class FirewallTypeDef(_RequiredFirewallTypeDef, _OptionalFirewallTypeDef):
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "NextToken": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+_RequiredRuleGroupResponseTypeDef = TypedDict(
+    "_RequiredRuleGroupResponseTypeDef",
+    {
+        "RuleGroupArn": str,
+        "RuleGroupName": str,
+        "RuleGroupId": str,
+    },
+)
+_OptionalRuleGroupResponseTypeDef = TypedDict(
+    "_OptionalRuleGroupResponseTypeDef",
+    {
+        "Description": str,
+        "Type": RuleGroupTypeType,
+        "Capacity": int,
+        "RuleGroupStatus": ResourceStatusType,
+        "Tags": List[TagTypeDef],
+        "ConsumedCapacity": int,
+        "NumberOfAssociations": int,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "SourceMetadata": SourceMetadataTypeDef,
+        "SnsTopic": str,
+        "LastModifiedTime": datetime,
+    },
+    total=False,
+)
+
+
+class RuleGroupResponseTypeDef(
+    _RequiredRuleGroupResponseTypeDef, _OptionalRuleGroupResponseTypeDef
+):
+    pass
+
+
+DescribeRuleGroupMetadataResponseTypeDef = TypedDict(
+    "DescribeRuleGroupMetadataResponseTypeDef",
+    {
+        "RuleGroupArn": str,
+        "RuleGroupName": str,
+        "Description": str,
+        "Type": RuleGroupTypeType,
+        "Capacity": int,
+        "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishMetricActionOutputTypeDef = TypedDict(
+    "PublishMetricActionOutputTypeDef",
+    {
+        "Dimensions": List[DimensionTypeDef],
+    },
+)
+
+PublishMetricActionTypeDef = TypedDict(
+    "PublishMetricActionTypeDef",
+    {
+        "Dimensions": Sequence[DimensionTypeDef],
+    },
+)
+
+ListFirewallsResponseTypeDef = TypedDict(
+    "ListFirewallsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Firewalls": List[FirewallMetadataTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFirewallPoliciesResponseTypeDef = TypedDict(
+    "ListFirewallPoliciesResponseTypeDef",
+    {
+        "NextToken": str,
+        "FirewallPolicies": List[FirewallPolicyMetadataTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyVariablesOutputTypeDef = TypedDict(
     "PolicyVariablesOutputTypeDef",
     {
         "RuleVariables": Dict[str, IPSetOutputTypeDef],
     },
     total=False,
 )
 
 ReferenceSetsOutputTypeDef = TypedDict(
     "ReferenceSetsOutputTypeDef",
     {
-        "IPSetReferences": Dict[str, IPSetReferenceOutputTypeDef],
+        "IPSetReferences": Dict[str, IPSetReferenceTypeDef],
     },
     total=False,
 )
 
 ReferenceSetsTypeDef = TypedDict(
     "ReferenceSetsTypeDef",
     {
@@ -1436,29 +1254,87 @@
     "PolicyVariablesTypeDef",
     {
         "RuleVariables": Mapping[str, IPSetTypeDef],
     },
     total=False,
 )
 
+ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef = TypedDict(
+    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFirewallsRequestListFirewallsPaginateTypeDef = TypedDict(
+    "ListFirewallsRequestListFirewallsPaginateTypeDef",
+    {
+        "VpcIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    {
+        "Scope": ResourceManagedStatusType,
+        "ManagedType": ResourceManagedTypeType,
+        "Type": RuleGroupTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef = TypedDict(
+    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
+    {
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
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextToken": str,
         "RuleGroups": List[RuleGroupMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTLSInspectionConfigurationsResponseTypeDef = TypedDict(
     "ListTLSInspectionConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "TLSInspectionConfigurations": List[TLSInspectionConfigurationMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoggingConfigurationOutputTypeDef = TypedDict(
     "LoggingConfigurationOutputTypeDef",
     {
         "LogDestinationConfigs": List[LogDestinationConfigOutputTypeDef],
@@ -1471,32 +1347,19 @@
         "LogDestinationConfigs": Sequence[LogDestinationConfigTypeDef],
     },
 )
 
 ServerCertificateScopeOutputTypeDef = TypedDict(
     "ServerCertificateScopeOutputTypeDef",
     {
-        "Sources": List[AddressOutputTypeDef],
-        "Destinations": List[AddressOutputTypeDef],
-        "SourcePorts": List[PortRangeOutputTypeDef],
-        "DestinationPorts": List[PortRangeOutputTypeDef],
-        "Protocols": List[int],
-    },
-    total=False,
-)
-
-MatchAttributesOutputTypeDef = TypedDict(
-    "MatchAttributesOutputTypeDef",
-    {
-        "Sources": List[AddressOutputTypeDef],
-        "Destinations": List[AddressOutputTypeDef],
-        "SourcePorts": List[PortRangeOutputTypeDef],
-        "DestinationPorts": List[PortRangeOutputTypeDef],
+        "Sources": List[AddressTypeDef],
+        "Destinations": List[AddressTypeDef],
+        "SourcePorts": List[PortRangeTypeDef],
+        "DestinationPorts": List[PortRangeTypeDef],
         "Protocols": List[int],
-        "TCPFlags": List[TCPFlagFieldOutputTypeDef],
     },
     total=False,
 )
 
 ServerCertificateScopeTypeDef = TypedDict(
     "ServerCertificateScopeTypeDef",
     {
@@ -1505,14 +1368,27 @@
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
         "Protocols": Sequence[int],
     },
     total=False,
 )
 
+MatchAttributesOutputTypeDef = TypedDict(
+    "MatchAttributesOutputTypeDef",
+    {
+        "Sources": List[AddressTypeDef],
+        "Destinations": List[AddressTypeDef],
+        "SourcePorts": List[PortRangeTypeDef],
+        "DestinationPorts": List[PortRangeTypeDef],
+        "Protocols": List[int],
+        "TCPFlags": List[TCPFlagFieldOutputTypeDef],
+    },
+    total=False,
+)
+
 MatchAttributesTypeDef = TypedDict(
     "MatchAttributesTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
@@ -1545,88 +1421,32 @@
     {
         "IPSets": Mapping[str, IPSetTypeDef],
         "PortSets": Mapping[str, PortSetTypeDef],
     },
     total=False,
 )
 
-_RequiredRuleGroupResponseTypeDef = TypedDict(
-    "_RequiredRuleGroupResponseTypeDef",
-    {
-        "RuleGroupArn": str,
-        "RuleGroupName": str,
-        "RuleGroupId": str,
-    },
-)
-_OptionalRuleGroupResponseTypeDef = TypedDict(
-    "_OptionalRuleGroupResponseTypeDef",
-    {
-        "Description": str,
-        "Type": RuleGroupTypeType,
-        "Capacity": int,
-        "RuleGroupStatus": ResourceStatusType,
-        "Tags": List[TagOutputTypeDef],
-        "ConsumedCapacity": int,
-        "NumberOfAssociations": int,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-        "SourceMetadata": SourceMetadataOutputTypeDef,
-        "SnsTopic": str,
-        "LastModifiedTime": datetime,
-    },
-    total=False,
-)
-
-
-class RuleGroupResponseTypeDef(
-    _RequiredRuleGroupResponseTypeDef, _OptionalRuleGroupResponseTypeDef
-):
-    pass
-
-
 StatefulRuleOutputTypeDef = TypedDict(
     "StatefulRuleOutputTypeDef",
     {
         "Action": StatefulActionType,
-        "Header": HeaderOutputTypeDef,
+        "Header": HeaderTypeDef,
         "RuleOptions": List[RuleOptionOutputTypeDef],
     },
 )
 
 StatefulRuleTypeDef = TypedDict(
     "StatefulRuleTypeDef",
     {
         "Action": StatefulActionType,
         "Header": HeaderTypeDef,
         "RuleOptions": Sequence[RuleOptionTypeDef],
     },
 )
 
-_RequiredStatefulRuleGroupReferenceOutputTypeDef = TypedDict(
-    "_RequiredStatefulRuleGroupReferenceOutputTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalStatefulRuleGroupReferenceOutputTypeDef = TypedDict(
-    "_OptionalStatefulRuleGroupReferenceOutputTypeDef",
-    {
-        "Priority": int,
-        "Override": StatefulRuleGroupOverrideOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class StatefulRuleGroupReferenceOutputTypeDef(
-    _RequiredStatefulRuleGroupReferenceOutputTypeDef,
-    _OptionalStatefulRuleGroupReferenceOutputTypeDef,
-):
-    pass
-
-
 _RequiredStatefulRuleGroupReferenceTypeDef = TypedDict(
     "_RequiredStatefulRuleGroupReferenceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalStatefulRuleGroupReferenceTypeDef = TypedDict(
@@ -1654,18 +1474,18 @@
     },
 )
 _OptionalTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "_OptionalTLSInspectionConfigurationResponseTypeDef",
     {
         "TLSInspectionConfigurationStatus": ResourceStatusType,
         "Description": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "LastModifiedTime": datetime,
         "NumberOfAssociations": int,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "Certificates": List[TlsCertificateDataTypeDef],
     },
     total=False,
 )
 
 
 class TLSInspectionConfigurationResponseTypeDef(
@@ -1679,72 +1499,98 @@
     "CapacityUsageSummaryTypeDef",
     {
         "CIDRs": CIDRSummaryTypeDef,
     },
     total=False,
 )
 
-ActionDefinitionOutputTypeDef = TypedDict(
-    "ActionDefinitionOutputTypeDef",
-    {
-        "PublishMetricAction": PublishMetricActionOutputTypeDef,
-    },
-    total=False,
-)
-
-ActionDefinitionTypeDef = TypedDict(
-    "ActionDefinitionTypeDef",
-    {
-        "PublishMetricAction": PublishMetricActionTypeDef,
-    },
-    total=False,
-)
-
 CreateFirewallPolicyResponseTypeDef = TypedDict(
     "CreateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallPolicyResponseTypeDef = TypedDict(
     "DeleteFirewallPolicyResponseTypeDef",
     {
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallPolicyResponseTypeDef = TypedDict(
     "UpdateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRuleGroupResponseTypeDef = TypedDict(
+    "CreateRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRuleGroupResponseTypeDef = TypedDict(
+    "DeleteRuleGroupResponseTypeDef",
+    {
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ActionDefinitionOutputTypeDef = TypedDict(
+    "ActionDefinitionOutputTypeDef",
+    {
+        "PublishMetricAction": PublishMetricActionOutputTypeDef,
+    },
+    total=False,
+)
+
+ActionDefinitionTypeDef = TypedDict(
+    "ActionDefinitionTypeDef",
+    {
+        "PublishMetricAction": PublishMetricActionTypeDef,
     },
+    total=False,
 )
 
 DescribeLoggingConfigurationResponseTypeDef = TypedDict(
     "DescribeLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
         "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLoggingConfigurationResponseTypeDef = TypedDict(
     "UpdateLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "FirewallArn": str,
@@ -1753,94 +1599,68 @@
     },
     total=False,
 )
 
 ServerCertificateConfigurationOutputTypeDef = TypedDict(
     "ServerCertificateConfigurationOutputTypeDef",
     {
-        "ServerCertificates": List[ServerCertificateOutputTypeDef],
+        "ServerCertificates": List[ServerCertificateTypeDef],
         "Scopes": List[ServerCertificateScopeOutputTypeDef],
     },
     total=False,
 )
 
-RuleDefinitionOutputTypeDef = TypedDict(
-    "RuleDefinitionOutputTypeDef",
-    {
-        "MatchAttributes": MatchAttributesOutputTypeDef,
-        "Actions": List[str],
-    },
-)
-
 ServerCertificateConfigurationTypeDef = TypedDict(
     "ServerCertificateConfigurationTypeDef",
     {
         "ServerCertificates": Sequence[ServerCertificateTypeDef],
         "Scopes": Sequence[ServerCertificateScopeTypeDef],
     },
     total=False,
 )
 
-RuleDefinitionTypeDef = TypedDict(
-    "RuleDefinitionTypeDef",
-    {
-        "MatchAttributes": MatchAttributesTypeDef,
-        "Actions": Sequence[str],
-    },
-)
-
-CreateRuleGroupResponseTypeDef = TypedDict(
-    "CreateRuleGroupResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteRuleGroupResponseTypeDef = TypedDict(
-    "DeleteRuleGroupResponseTypeDef",
+RuleDefinitionOutputTypeDef = TypedDict(
+    "RuleDefinitionOutputTypeDef",
     {
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MatchAttributes": MatchAttributesOutputTypeDef,
+        "Actions": List[str],
     },
 )
 
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+RuleDefinitionTypeDef = TypedDict(
+    "RuleDefinitionTypeDef",
     {
-        "UpdateToken": str,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MatchAttributes": MatchAttributesTypeDef,
+        "Actions": Sequence[str],
     },
 )
 
 CreateTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "CreateTLSInspectionConfigurationResponseTypeDef",
     {
         "UpdateToken": str,
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "DeleteTLSInspectionConfigurationResponseTypeDef",
     {
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "UpdateTLSInspectionConfigurationResponseTypeDef",
     {
         "UpdateToken": str,
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFirewallStatusTypeDef = TypedDict(
     "_RequiredFirewallStatusTypeDef",
     {
         "Status": FirewallStatusValueType,
@@ -1881,81 +1701,81 @@
     "TLSInspectionConfigurationOutputTypeDef",
     {
         "ServerCertificateConfigurations": List[ServerCertificateConfigurationOutputTypeDef],
     },
     total=False,
 )
 
-StatelessRuleOutputTypeDef = TypedDict(
-    "StatelessRuleOutputTypeDef",
-    {
-        "RuleDefinition": RuleDefinitionOutputTypeDef,
-        "Priority": int,
-    },
-)
-
 TLSInspectionConfigurationTypeDef = TypedDict(
     "TLSInspectionConfigurationTypeDef",
     {
         "ServerCertificateConfigurations": Sequence[ServerCertificateConfigurationTypeDef],
     },
     total=False,
 )
 
+StatelessRuleOutputTypeDef = TypedDict(
+    "StatelessRuleOutputTypeDef",
+    {
+        "RuleDefinition": RuleDefinitionOutputTypeDef,
+        "Priority": int,
+    },
+)
+
 StatelessRuleTypeDef = TypedDict(
     "StatelessRuleTypeDef",
     {
         "RuleDefinition": RuleDefinitionTypeDef,
         "Priority": int,
     },
 )
 
 CreateFirewallResponseTypeDef = TypedDict(
     "CreateFirewallResponseTypeDef",
     {
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallResponseTypeDef = TypedDict(
     "DeleteFirewallResponseTypeDef",
     {
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFirewallResponseTypeDef = TypedDict(
     "DescribeFirewallResponseTypeDef",
     {
         "UpdateToken": str,
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFirewallPolicyOutputTypeDef = TypedDict(
     "_RequiredFirewallPolicyOutputTypeDef",
     {
         "StatelessDefaultActions": List[str],
         "StatelessFragmentDefaultActions": List[str],
     },
 )
 _OptionalFirewallPolicyOutputTypeDef = TypedDict(
     "_OptionalFirewallPolicyOutputTypeDef",
     {
-        "StatelessRuleGroupReferences": List[StatelessRuleGroupReferenceOutputTypeDef],
+        "StatelessRuleGroupReferences": List[StatelessRuleGroupReferenceTypeDef],
         "StatelessCustomActions": List[CustomActionOutputTypeDef],
-        "StatefulRuleGroupReferences": List[StatefulRuleGroupReferenceOutputTypeDef],
+        "StatefulRuleGroupReferences": List[StatefulRuleGroupReferenceTypeDef],
         "StatefulDefaultActions": List[str],
-        "StatefulEngineOptions": StatefulEngineOptionsOutputTypeDef,
+        "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
         "TLSInspectionConfigurationArn": str,
         "PolicyVariables": PolicyVariablesOutputTypeDef,
     },
     total=False,
 )
 
 
@@ -1993,40 +1813,18 @@
 
 DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "DescribeTLSInspectionConfigurationResponseTypeDef",
     {
         "UpdateToken": str,
         "TLSInspectionConfiguration": TLSInspectionConfigurationOutputTypeDef,
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
-    "_RequiredStatelessRulesAndCustomActionsOutputTypeDef",
-    {
-        "StatelessRules": List[StatelessRuleOutputTypeDef],
-    },
-)
-_OptionalStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
-    "_OptionalStatelessRulesAndCustomActionsOutputTypeDef",
-    {
-        "CustomActions": List[CustomActionOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class StatelessRulesAndCustomActionsOutputTypeDef(
-    _RequiredStatelessRulesAndCustomActionsOutputTypeDef,
-    _OptionalStatelessRulesAndCustomActionsOutputTypeDef,
-):
-    pass
-
-
 _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfigurationName": str,
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
     },
 )
@@ -2070,14 +1868,36 @@
 class UpdateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalUpdateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
+    "_RequiredStatelessRulesAndCustomActionsOutputTypeDef",
+    {
+        "StatelessRules": List[StatelessRuleOutputTypeDef],
+    },
+)
+_OptionalStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
+    "_OptionalStatelessRulesAndCustomActionsOutputTypeDef",
+    {
+        "CustomActions": List[CustomActionOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class StatelessRulesAndCustomActionsOutputTypeDef(
+    _RequiredStatelessRulesAndCustomActionsOutputTypeDef,
+    _OptionalStatelessRulesAndCustomActionsOutputTypeDef,
+):
+    pass
+
+
 _RequiredStatelessRulesAndCustomActionsTypeDef = TypedDict(
     "_RequiredStatelessRulesAndCustomActionsTypeDef",
     {
         "StatelessRules": Sequence[StatelessRuleTypeDef],
     },
 )
 _OptionalStatelessRulesAndCustomActionsTypeDef = TypedDict(
@@ -2097,15 +1917,15 @@
 
 DescribeFirewallPolicyResponseTypeDef = TypedDict(
     "DescribeFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
         "FirewallPolicy": FirewallPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallPolicyRequestRequestTypeDef",
     {
         "FirewallPolicyName": str,
@@ -2187,15 +2007,15 @@
     },
 )
 _OptionalRuleGroupOutputTypeDef = TypedDict(
     "_OptionalRuleGroupOutputTypeDef",
     {
         "RuleVariables": RuleVariablesOutputTypeDef,
         "ReferenceSets": ReferenceSetsOutputTypeDef,
-        "StatefulRuleOptions": StatefulRuleOptionsOutputTypeDef,
+        "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
     },
     total=False,
 )
 
 
 class RuleGroupOutputTypeDef(_RequiredRuleGroupOutputTypeDef, _OptionalRuleGroupOutputTypeDef):
     pass
@@ -2224,15 +2044,15 @@
 
 DescribeRuleGroupResponseTypeDef = TypedDict(
     "DescribeRuleGroupResponseTypeDef",
     {
         "UpdateToken": str,
         "RuleGroup": RuleGroupOutputTypeDef,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupName": str,
```

### Comparing `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall/type_defs.pyi` & `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for network-firewall service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_network_firewall.type_defs import AddressOutputTypeDef
+    from mypy_boto3_network_firewall.type_defs import AddressTypeDef
 
-    data: AddressOutputTypeDef = {...}
+    data: AddressTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -44,192 +44,170 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AddressOutputTypeDef",
     "AddressTypeDef",
     "AssociateFirewallPolicyRequestRequestTypeDef",
-    "AssociateFirewallPolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SubnetMappingTypeDef",
-    "SubnetMappingOutputTypeDef",
     "AttachmentTypeDef",
     "IPSetMetadataTypeDef",
     "EncryptionConfigurationTypeDef",
     "TagTypeDef",
     "SourceMetadataTypeDef",
     "DeleteFirewallPolicyRequestRequestTypeDef",
     "DeleteFirewallRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteTLSInspectionConfigurationRequestRequestTypeDef",
     "DescribeFirewallPolicyRequestRequestTypeDef",
     "DescribeFirewallRequestRequestTypeDef",
     "DescribeLoggingConfigurationRequestRequestTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
-    "StatefulRuleOptionsOutputTypeDef",
+    "StatefulRuleOptionsTypeDef",
     "DescribeRuleGroupRequestRequestTypeDef",
     "DescribeTLSInspectionConfigurationRequestRequestTypeDef",
-    "DimensionOutputTypeDef",
     "DimensionTypeDef",
     "DisassociateSubnetsRequestRequestTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "FirewallMetadataTypeDef",
     "FirewallPolicyMetadataTypeDef",
-    "StatefulEngineOptionsOutputTypeDef",
-    "StatelessRuleGroupReferenceOutputTypeDef",
-    "TagOutputTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupReferenceTypeDef",
-    "HeaderOutputTypeDef",
     "HeaderTypeDef",
     "IPSetOutputTypeDef",
-    "IPSetReferenceOutputTypeDef",
     "IPSetReferenceTypeDef",
     "IPSetTypeDef",
-    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListFirewallPoliciesRequestRequestTypeDef",
-    "ListFirewallsRequestListFirewallsPaginateTypeDef",
     "ListFirewallsRequestRequestTypeDef",
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupMetadataTypeDef",
-    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
     "ListTLSInspectionConfigurationsRequestRequestTypeDef",
     "TLSInspectionConfigurationMetadataTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "LogDestinationConfigOutputTypeDef",
     "LogDestinationConfigTypeDef",
-    "PortRangeOutputTypeDef",
-    "TCPFlagFieldOutputTypeDef",
     "PortRangeTypeDef",
+    "TCPFlagFieldOutputTypeDef",
     "TCPFlagFieldTypeDef",
-    "PaginatorConfigTypeDef",
     "PerObjectStatusTypeDef",
     "PortSetOutputTypeDef",
     "PortSetTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SourceMetadataOutputTypeDef",
-    "StatefulRuleOptionsTypeDef",
     "RuleOptionOutputTypeDef",
     "RuleOptionTypeDef",
     "RulesSourceListOutputTypeDef",
     "RulesSourceListTypeDef",
-    "ServerCertificateOutputTypeDef",
     "ServerCertificateTypeDef",
-    "StatefulRuleGroupOverrideOutputTypeDef",
     "StatefulRuleGroupOverrideTypeDef",
     "TlsCertificateDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallDeleteProtectionRequestRequestTypeDef",
-    "UpdateFirewallDeleteProtectionResponseTypeDef",
     "UpdateFirewallDescriptionRequestRequestTypeDef",
-    "UpdateFirewallDescriptionResponseTypeDef",
     "UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
-    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
     "UpdateSubnetChangeProtectionRequestRequestTypeDef",
+    "AssociateFirewallPolicyResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
+    "UpdateFirewallDeleteProtectionResponseTypeDef",
+    "UpdateFirewallDescriptionResponseTypeDef",
+    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
     "UpdateSubnetChangeProtectionResponseTypeDef",
     "AssociateSubnetsRequestRequestTypeDef",
     "AssociateSubnetsResponseTypeDef",
     "DisassociateSubnetsResponseTypeDef",
     "CIDRSummaryTypeDef",
     "UpdateFirewallEncryptionConfigurationRequestRequestTypeDef",
+    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     "CreateFirewallRequestRequestTypeDef",
+    "FirewallPolicyResponseTypeDef",
+    "FirewallTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "RuleGroupResponseTypeDef",
     "DescribeRuleGroupMetadataResponseTypeDef",
     "PublishMetricActionOutputTypeDef",
     "PublishMetricActionTypeDef",
-    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
     "ListFirewallsResponseTypeDef",
     "ListFirewallPoliciesResponseTypeDef",
-    "FirewallPolicyResponseTypeDef",
-    "FirewallTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PolicyVariablesOutputTypeDef",
     "ReferenceSetsOutputTypeDef",
     "ReferenceSetsTypeDef",
     "PolicyVariablesTypeDef",
+    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
+    "ListFirewallsRequestListFirewallsPaginateTypeDef",
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "ListTLSInspectionConfigurationsResponseTypeDef",
     "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "ServerCertificateScopeOutputTypeDef",
-    "MatchAttributesOutputTypeDef",
     "ServerCertificateScopeTypeDef",
+    "MatchAttributesOutputTypeDef",
     "MatchAttributesTypeDef",
     "SyncStateTypeDef",
     "RuleVariablesOutputTypeDef",
     "RuleVariablesTypeDef",
-    "RuleGroupResponseTypeDef",
     "StatefulRuleOutputTypeDef",
     "StatefulRuleTypeDef",
-    "StatefulRuleGroupReferenceOutputTypeDef",
     "StatefulRuleGroupReferenceTypeDef",
     "TLSInspectionConfigurationResponseTypeDef",
     "CapacityUsageSummaryTypeDef",
-    "ActionDefinitionOutputTypeDef",
-    "ActionDefinitionTypeDef",
     "CreateFirewallPolicyResponseTypeDef",
     "DeleteFirewallPolicyResponseTypeDef",
     "UpdateFirewallPolicyResponseTypeDef",
+    "CreateRuleGroupResponseTypeDef",
+    "DeleteRuleGroupResponseTypeDef",
+    "UpdateRuleGroupResponseTypeDef",
+    "ActionDefinitionOutputTypeDef",
+    "ActionDefinitionTypeDef",
     "DescribeLoggingConfigurationResponseTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     "ServerCertificateConfigurationOutputTypeDef",
-    "RuleDefinitionOutputTypeDef",
     "ServerCertificateConfigurationTypeDef",
+    "RuleDefinitionOutputTypeDef",
     "RuleDefinitionTypeDef",
-    "CreateRuleGroupResponseTypeDef",
-    "DeleteRuleGroupResponseTypeDef",
-    "UpdateRuleGroupResponseTypeDef",
     "CreateTLSInspectionConfigurationResponseTypeDef",
     "DeleteTLSInspectionConfigurationResponseTypeDef",
     "UpdateTLSInspectionConfigurationResponseTypeDef",
     "FirewallStatusTypeDef",
     "CustomActionOutputTypeDef",
     "CustomActionTypeDef",
     "TLSInspectionConfigurationOutputTypeDef",
-    "StatelessRuleOutputTypeDef",
     "TLSInspectionConfigurationTypeDef",
+    "StatelessRuleOutputTypeDef",
     "StatelessRuleTypeDef",
     "CreateFirewallResponseTypeDef",
     "DeleteFirewallResponseTypeDef",
     "DescribeFirewallResponseTypeDef",
     "FirewallPolicyOutputTypeDef",
     "FirewallPolicyTypeDef",
     "DescribeTLSInspectionConfigurationResponseTypeDef",
-    "StatelessRulesAndCustomActionsOutputTypeDef",
     "CreateTLSInspectionConfigurationRequestRequestTypeDef",
     "UpdateTLSInspectionConfigurationRequestRequestTypeDef",
+    "StatelessRulesAndCustomActionsOutputTypeDef",
     "StatelessRulesAndCustomActionsTypeDef",
     "DescribeFirewallPolicyResponseTypeDef",
     "CreateFirewallPolicyRequestRequestTypeDef",
     "UpdateFirewallPolicyRequestRequestTypeDef",
     "RulesSourceOutputTypeDef",
     "RulesSourceTypeDef",
     "RuleGroupOutputTypeDef",
     "RuleGroupTypeDef",
     "DescribeRuleGroupResponseTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
 )
 
-AddressOutputTypeDef = TypedDict(
-    "AddressOutputTypeDef",
-    {
-        "AddressDefinition": str,
-    },
-)
-
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressDefinition": str,
     },
 )
 
@@ -251,22 +229,22 @@
 
 class AssociateFirewallPolicyRequestRequestTypeDef(
     _RequiredAssociateFirewallPolicyRequestRequestTypeDef,
     _OptionalAssociateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
-AssociateFirewallPolicyResponseTypeDef = TypedDict(
-    "AssociateFirewallPolicyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "FirewallPolicyArn": str,
-        "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredSubnetMappingTypeDef = TypedDict(
     "_RequiredSubnetMappingTypeDef",
     {
         "SubnetId": str,
@@ -279,33 +257,14 @@
     },
     total=False,
 )
 
 class SubnetMappingTypeDef(_RequiredSubnetMappingTypeDef, _OptionalSubnetMappingTypeDef):
     pass
 
-_RequiredSubnetMappingOutputTypeDef = TypedDict(
-    "_RequiredSubnetMappingOutputTypeDef",
-    {
-        "SubnetId": str,
-    },
-)
-_OptionalSubnetMappingOutputTypeDef = TypedDict(
-    "_OptionalSubnetMappingOutputTypeDef",
-    {
-        "IPAddressType": IPAddressTypeType,
-    },
-    total=False,
-)
-
-class SubnetMappingOutputTypeDef(
-    _RequiredSubnetMappingOutputTypeDef, _OptionalSubnetMappingOutputTypeDef
-):
-    pass
-
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "SubnetId": str,
         "EndpointId": str,
         "Status": AttachmentStatusType,
         "StatusMessage": str,
@@ -431,34 +390,26 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRuleGroupMetadataRequestRequestTypeDef = TypedDict(
     "DescribeRuleGroupMetadataRequestRequestTypeDef",
     {
         "RuleGroupName": str,
         "RuleGroupArn": str,
         "Type": RuleGroupTypeType,
     },
     total=False,
 )
 
-StatefulRuleOptionsOutputTypeDef = TypedDict(
-    "StatefulRuleOptionsOutputTypeDef",
+StatefulRuleOptionsTypeDef = TypedDict(
+    "StatefulRuleOptionsTypeDef",
     {
         "RuleOrder": RuleOrderType,
     },
     total=False,
 )
 
 DescribeRuleGroupRequestRequestTypeDef = TypedDict(
@@ -476,21 +427,14 @@
     {
         "TLSInspectionConfigurationArn": str,
         "TLSInspectionConfigurationName": str,
     },
     total=False,
 )
 
-DimensionOutputTypeDef = TypedDict(
-    "DimensionOutputTypeDef",
-    {
-        "Value": str,
-    },
-)
-
 DimensionTypeDef = TypedDict(
     "DimensionTypeDef",
     {
         "Value": str,
     },
 )
 
@@ -512,33 +456,14 @@
 
 class DisassociateSubnetsRequestRequestTypeDef(
     _RequiredDisassociateSubnetsRequestRequestTypeDef,
     _OptionalDisassociateSubnetsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEncryptionConfigurationOutputTypeDef",
-    {
-        "Type": EncryptionTypeType,
-    },
-)
-_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEncryptionConfigurationOutputTypeDef",
-    {
-        "KeyId": str,
-    },
-    total=False,
-)
-
-class EncryptionConfigurationOutputTypeDef(
-    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
-):
-    pass
-
 FirewallMetadataTypeDef = TypedDict(
     "FirewallMetadataTypeDef",
     {
         "FirewallName": str,
         "FirewallArn": str,
     },
     total=False,
@@ -549,39 +474,14 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
-StatefulEngineOptionsOutputTypeDef = TypedDict(
-    "StatefulEngineOptionsOutputTypeDef",
-    {
-        "RuleOrder": RuleOrderType,
-        "StreamExceptionPolicy": StreamExceptionPolicyType,
-    },
-    total=False,
-)
-
-StatelessRuleGroupReferenceOutputTypeDef = TypedDict(
-    "StatelessRuleGroupReferenceOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "Priority": int,
-    },
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
 StatefulEngineOptionsTypeDef = TypedDict(
     "StatefulEngineOptionsTypeDef",
     {
         "RuleOrder": RuleOrderType,
         "StreamExceptionPolicy": StreamExceptionPolicyType,
     },
     total=False,
@@ -591,26 +491,14 @@
     "StatelessRuleGroupReferenceTypeDef",
     {
         "ResourceArn": str,
         "Priority": int,
     },
 )
 
-HeaderOutputTypeDef = TypedDict(
-    "HeaderOutputTypeDef",
-    {
-        "Protocol": StatefulRuleProtocolType,
-        "Source": str,
-        "SourcePort": str,
-        "Direction": StatefulRuleDirectionType,
-        "Destination": str,
-        "DestinationPort": str,
-    },
-)
-
 HeaderTypeDef = TypedDict(
     "HeaderTypeDef",
     {
         "Protocol": StatefulRuleProtocolType,
         "Source": str,
         "SourcePort": str,
         "Direction": StatefulRuleDirectionType,
@@ -622,22 +510,14 @@
 IPSetOutputTypeDef = TypedDict(
     "IPSetOutputTypeDef",
     {
         "Definition": List[str],
     },
 )
 
-IPSetReferenceOutputTypeDef = TypedDict(
-    "IPSetReferenceOutputTypeDef",
-    {
-        "ReferenceArn": str,
-    },
-    total=False,
-)
-
 IPSetReferenceTypeDef = TypedDict(
     "IPSetReferenceTypeDef",
     {
         "ReferenceArn": str,
     },
     total=False,
 )
@@ -645,61 +525,43 @@
 IPSetTypeDef = TypedDict(
     "IPSetTypeDef",
     {
         "Definition": Sequence[str],
     },
 )
 
-ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef = TypedDict(
-    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
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
 
 ListFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "ListFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListFirewallsRequestListFirewallsPaginateTypeDef = TypedDict(
-    "ListFirewallsRequestListFirewallsPaginateTypeDef",
-    {
-        "VpcIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFirewallsRequestRequestTypeDef = TypedDict(
     "ListFirewallsRequestRequestTypeDef",
     {
         "NextToken": str,
         "VpcIds": Sequence[str],
         "MaxResults": int,
     },
     total=False,
 )
 
-ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
-    {
-        "Scope": ResourceManagedStatusType,
-        "ManagedType": ResourceManagedTypeType,
-        "Type": RuleGroupTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Scope": ResourceManagedStatusType,
         "ManagedType": ResourceManagedTypeType,
@@ -713,22 +575,14 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
-ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef = TypedDict(
-    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTLSInspectionConfigurationsRequestRequestTypeDef = TypedDict(
     "ListTLSInspectionConfigurationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -739,34 +593,14 @@
     {
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
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
@@ -798,16 +632,16 @@
     {
         "LogType": LogTypeType,
         "LogDestinationType": LogDestinationTypeType,
         "LogDestination": Mapping[str, str],
     },
 )
 
-PortRangeOutputTypeDef = TypedDict(
-    "PortRangeOutputTypeDef",
+PortRangeTypeDef = TypedDict(
+    "PortRangeTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
 )
 
 _RequiredTCPFlagFieldOutputTypeDef = TypedDict(
@@ -825,22 +659,14 @@
 )
 
 class TCPFlagFieldOutputTypeDef(
     _RequiredTCPFlagFieldOutputTypeDef, _OptionalTCPFlagFieldOutputTypeDef
 ):
     pass
 
-PortRangeTypeDef = TypedDict(
-    "PortRangeTypeDef",
-    {
-        "FromPort": int,
-        "ToPort": int,
-    },
-)
-
 _RequiredTCPFlagFieldTypeDef = TypedDict(
     "_RequiredTCPFlagFieldTypeDef",
     {
         "Flags": Sequence[TCPFlagType],
     },
 )
 _OptionalTCPFlagFieldTypeDef = TypedDict(
@@ -850,24 +676,14 @@
     },
     total=False,
 )
 
 class TCPFlagFieldTypeDef(_RequiredTCPFlagFieldTypeDef, _OptionalTCPFlagFieldTypeDef):
     pass
 
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
 PerObjectStatusTypeDef = TypedDict(
     "PerObjectStatusTypeDef",
     {
         "SyncStatus": PerObjectSyncStatusType,
         "UpdateToken": str,
     },
     total=False,
@@ -893,42 +709,14 @@
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
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
-SourceMetadataOutputTypeDef = TypedDict(
-    "SourceMetadataOutputTypeDef",
-    {
-        "SourceArn": str,
-        "SourceUpdateToken": str,
-    },
-    total=False,
-)
-
-StatefulRuleOptionsTypeDef = TypedDict(
-    "StatefulRuleOptionsTypeDef",
-    {
-        "RuleOrder": RuleOrderType,
-    },
-    total=False,
-)
-
 _RequiredRuleOptionOutputTypeDef = TypedDict(
     "_RequiredRuleOptionOutputTypeDef",
     {
         "Keyword": str,
     },
 )
 _OptionalRuleOptionOutputTypeDef = TypedDict(
@@ -973,38 +761,22 @@
     {
         "Targets": Sequence[str],
         "TargetTypes": Sequence[TargetTypeType],
         "GeneratedRulesType": GeneratedRulesTypeType,
     },
 )
 
-ServerCertificateOutputTypeDef = TypedDict(
-    "ServerCertificateOutputTypeDef",
-    {
-        "ResourceArn": str,
-    },
-    total=False,
-)
-
 ServerCertificateTypeDef = TypedDict(
     "ServerCertificateTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
 
-StatefulRuleGroupOverrideOutputTypeDef = TypedDict(
-    "StatefulRuleGroupOverrideOutputTypeDef",
-    {
-        "Action": Literal["DROP_TO_ALERT"],
-    },
-    total=False,
-)
-
 StatefulRuleGroupOverrideTypeDef = TypedDict(
     "StatefulRuleGroupOverrideTypeDef",
     {
         "Action": Literal["DROP_TO_ALERT"],
     },
     total=False,
 )
@@ -1046,47 +818,25 @@
 
 class UpdateFirewallDeleteProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallDeleteProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallDeleteProtectionRequestRequestTypeDef,
 ):
     pass
 
-UpdateFirewallDeleteProtectionResponseTypeDef = TypedDict(
-    "UpdateFirewallDeleteProtectionResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "DeleteProtection": bool,
-        "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateFirewallDescriptionRequestRequestTypeDef = TypedDict(
     "UpdateFirewallDescriptionRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "Description": str,
     },
     total=False,
 )
 
-UpdateFirewallDescriptionResponseTypeDef = TypedDict(
-    "UpdateFirewallDescriptionResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "Description": str,
-        "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef",
     {
         "FirewallPolicyChangeProtection": bool,
     },
 )
 _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -1101,25 +851,14 @@
 
 class UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
-UpdateFirewallPolicyChangeProtectionResponseTypeDef = TypedDict(
-    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "FirewallArn": str,
-        "FirewallName": str,
-        "FirewallPolicyChangeProtection": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef",
     {
         "SubnetChangeProtection": bool,
     },
 )
 _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef = TypedDict(
@@ -1134,22 +873,74 @@
 
 class UpdateSubnetChangeProtectionRequestRequestTypeDef(
     _RequiredUpdateSubnetChangeProtectionRequestRequestTypeDef,
     _OptionalUpdateSubnetChangeProtectionRequestRequestTypeDef,
 ):
     pass
 
+AssociateFirewallPolicyResponseTypeDef = TypedDict(
+    "AssociateFirewallPolicyResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "FirewallPolicyArn": str,
+        "UpdateToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallDeleteProtectionResponseTypeDef = TypedDict(
+    "UpdateFirewallDeleteProtectionResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "DeleteProtection": bool,
+        "UpdateToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallDescriptionResponseTypeDef = TypedDict(
+    "UpdateFirewallDescriptionResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "Description": str,
+        "UpdateToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallPolicyChangeProtectionResponseTypeDef = TypedDict(
+    "UpdateFirewallPolicyChangeProtectionResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "FirewallArn": str,
+        "FirewallName": str,
+        "FirewallPolicyChangeProtection": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSubnetChangeProtectionResponseTypeDef = TypedDict(
     "UpdateSubnetChangeProtectionResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallArn": str,
         "FirewallName": str,
         "SubnetChangeProtection": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssociateSubnetsRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateSubnetsRequestRequestTypeDef",
     {
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
@@ -1171,28 +962,28 @@
     pass
 
 AssociateSubnetsResponseTypeDef = TypedDict(
     "AssociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
-        "SubnetMappings": List[SubnetMappingOutputTypeDef],
+        "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateSubnetsResponseTypeDef = TypedDict(
     "DisassociateSubnetsResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
-        "SubnetMappings": List[SubnetMappingOutputTypeDef],
+        "SubnetMappings": List[SubnetMappingTypeDef],
         "UpdateToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CIDRSummaryTypeDef = TypedDict(
     "CIDRSummaryTypeDef",
     {
         "AvailableCIDRCount": int,
@@ -1209,14 +1000,25 @@
         "FirewallArn": str,
         "FirewallName": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+UpdateFirewallEncryptionConfigurationResponseTypeDef = TypedDict(
+    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
+    {
+        "FirewallArn": str,
+        "FirewallName": str,
+        "UpdateToken": str,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateFirewallRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRequestRequestTypeDef",
     {
         "FirewallName": str,
         "FirewallPolicyArn": str,
         "VpcId": str,
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
@@ -1236,190 +1038,266 @@
 )
 
 class CreateFirewallRequestRequestTypeDef(
     _RequiredCreateFirewallRequestRequestTypeDef, _OptionalCreateFirewallRequestRequestTypeDef
 ):
     pass
 
+_RequiredFirewallPolicyResponseTypeDef = TypedDict(
+    "_RequiredFirewallPolicyResponseTypeDef",
+    {
+        "FirewallPolicyName": str,
+        "FirewallPolicyArn": str,
+        "FirewallPolicyId": str,
+    },
+)
+_OptionalFirewallPolicyResponseTypeDef = TypedDict(
+    "_OptionalFirewallPolicyResponseTypeDef",
+    {
+        "Description": str,
+        "FirewallPolicyStatus": ResourceStatusType,
+        "Tags": List[TagTypeDef],
+        "ConsumedStatelessRuleCapacity": int,
+        "ConsumedStatefulRuleCapacity": int,
+        "NumberOfAssociations": int,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "LastModifiedTime": datetime,
+    },
+    total=False,
+)
+
+class FirewallPolicyResponseTypeDef(
+    _RequiredFirewallPolicyResponseTypeDef, _OptionalFirewallPolicyResponseTypeDef
+):
+    pass
+
+_RequiredFirewallTypeDef = TypedDict(
+    "_RequiredFirewallTypeDef",
+    {
+        "FirewallPolicyArn": str,
+        "VpcId": str,
+        "SubnetMappings": List[SubnetMappingTypeDef],
+        "FirewallId": str,
+    },
+)
+_OptionalFirewallTypeDef = TypedDict(
+    "_OptionalFirewallTypeDef",
+    {
+        "FirewallName": str,
+        "FirewallArn": str,
+        "DeleteProtection": bool,
+        "SubnetChangeProtection": bool,
+        "FirewallPolicyChangeProtection": bool,
+        "Description": str,
+        "Tags": List[TagTypeDef],
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class FirewallTypeDef(_RequiredFirewallTypeDef, _OptionalFirewallTypeDef):
+    pass
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "NextToken": str,
+        "Tags": List[TagTypeDef],
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
 
+_RequiredRuleGroupResponseTypeDef = TypedDict(
+    "_RequiredRuleGroupResponseTypeDef",
+    {
+        "RuleGroupArn": str,
+        "RuleGroupName": str,
+        "RuleGroupId": str,
+    },
+)
+_OptionalRuleGroupResponseTypeDef = TypedDict(
+    "_OptionalRuleGroupResponseTypeDef",
+    {
+        "Description": str,
+        "Type": RuleGroupTypeType,
+        "Capacity": int,
+        "RuleGroupStatus": ResourceStatusType,
+        "Tags": List[TagTypeDef],
+        "ConsumedCapacity": int,
+        "NumberOfAssociations": int,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "SourceMetadata": SourceMetadataTypeDef,
+        "SnsTopic": str,
+        "LastModifiedTime": datetime,
+    },
+    total=False,
+)
+
+class RuleGroupResponseTypeDef(
+    _RequiredRuleGroupResponseTypeDef, _OptionalRuleGroupResponseTypeDef
+):
+    pass
+
 DescribeRuleGroupMetadataResponseTypeDef = TypedDict(
     "DescribeRuleGroupMetadataResponseTypeDef",
     {
         "RuleGroupArn": str,
         "RuleGroupName": str,
         "Description": str,
         "Type": RuleGroupTypeType,
         "Capacity": int,
-        "StatefulRuleOptions": StatefulRuleOptionsOutputTypeDef,
+        "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
         "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PublishMetricActionOutputTypeDef = TypedDict(
     "PublishMetricActionOutputTypeDef",
     {
-        "Dimensions": List[DimensionOutputTypeDef],
+        "Dimensions": List[DimensionTypeDef],
     },
 )
 
 PublishMetricActionTypeDef = TypedDict(
     "PublishMetricActionTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
     },
 )
 
-UpdateFirewallEncryptionConfigurationResponseTypeDef = TypedDict(
-    "UpdateFirewallEncryptionConfigurationResponseTypeDef",
-    {
-        "FirewallArn": str,
-        "FirewallName": str,
-        "UpdateToken": str,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListFirewallsResponseTypeDef = TypedDict(
     "ListFirewallsResponseTypeDef",
     {
         "NextToken": str,
         "Firewalls": List[FirewallMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallPoliciesResponseTypeDef = TypedDict(
     "ListFirewallPoliciesResponseTypeDef",
     {
         "NextToken": str,
         "FirewallPolicies": List[FirewallPolicyMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFirewallPolicyResponseTypeDef = TypedDict(
-    "_RequiredFirewallPolicyResponseTypeDef",
+PolicyVariablesOutputTypeDef = TypedDict(
+    "PolicyVariablesOutputTypeDef",
     {
-        "FirewallPolicyName": str,
-        "FirewallPolicyArn": str,
-        "FirewallPolicyId": str,
+        "RuleVariables": Dict[str, IPSetOutputTypeDef],
     },
+    total=False,
 )
-_OptionalFirewallPolicyResponseTypeDef = TypedDict(
-    "_OptionalFirewallPolicyResponseTypeDef",
+
+ReferenceSetsOutputTypeDef = TypedDict(
+    "ReferenceSetsOutputTypeDef",
     {
-        "Description": str,
-        "FirewallPolicyStatus": ResourceStatusType,
-        "Tags": List[TagOutputTypeDef],
-        "ConsumedStatelessRuleCapacity": int,
-        "ConsumedStatefulRuleCapacity": int,
-        "NumberOfAssociations": int,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-        "LastModifiedTime": datetime,
+        "IPSetReferences": Dict[str, IPSetReferenceTypeDef],
     },
     total=False,
 )
 
-class FirewallPolicyResponseTypeDef(
-    _RequiredFirewallPolicyResponseTypeDef, _OptionalFirewallPolicyResponseTypeDef
-):
-    pass
-
-_RequiredFirewallTypeDef = TypedDict(
-    "_RequiredFirewallTypeDef",
+ReferenceSetsTypeDef = TypedDict(
+    "ReferenceSetsTypeDef",
     {
-        "FirewallPolicyArn": str,
-        "VpcId": str,
-        "SubnetMappings": List[SubnetMappingOutputTypeDef],
-        "FirewallId": str,
+        "IPSetReferences": Mapping[str, IPSetReferenceTypeDef],
     },
+    total=False,
 )
-_OptionalFirewallTypeDef = TypedDict(
-    "_OptionalFirewallTypeDef",
+
+PolicyVariablesTypeDef = TypedDict(
+    "PolicyVariablesTypeDef",
     {
-        "FirewallName": str,
-        "FirewallArn": str,
-        "DeleteProtection": bool,
-        "SubnetChangeProtection": bool,
-        "FirewallPolicyChangeProtection": bool,
-        "Description": str,
-        "Tags": List[TagOutputTypeDef],
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "RuleVariables": Mapping[str, IPSetTypeDef],
     },
     total=False,
 )
 
-class FirewallTypeDef(_RequiredFirewallTypeDef, _OptionalFirewallTypeDef):
-    pass
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef = TypedDict(
+    "ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef",
     {
-        "NextToken": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-PolicyVariablesOutputTypeDef = TypedDict(
-    "PolicyVariablesOutputTypeDef",
+ListFirewallsRequestListFirewallsPaginateTypeDef = TypedDict(
+    "ListFirewallsRequestListFirewallsPaginateTypeDef",
     {
-        "RuleVariables": Dict[str, IPSetOutputTypeDef],
+        "VpcIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ReferenceSetsOutputTypeDef = TypedDict(
-    "ReferenceSetsOutputTypeDef",
+ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     {
-        "IPSetReferences": Dict[str, IPSetReferenceOutputTypeDef],
+        "Scope": ResourceManagedStatusType,
+        "ManagedType": ResourceManagedTypeType,
+        "Type": RuleGroupTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ReferenceSetsTypeDef = TypedDict(
-    "ReferenceSetsTypeDef",
+ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef = TypedDict(
+    "ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef",
     {
-        "IPSetReferences": Mapping[str, IPSetReferenceTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-PolicyVariablesTypeDef = TypedDict(
-    "PolicyVariablesTypeDef",
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
-        "RuleVariables": Mapping[str, IPSetTypeDef],
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextToken": str,
         "RuleGroups": List[RuleGroupMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTLSInspectionConfigurationsResponseTypeDef = TypedDict(
     "ListTLSInspectionConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "TLSInspectionConfigurations": List[TLSInspectionConfigurationMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoggingConfigurationOutputTypeDef = TypedDict(
     "LoggingConfigurationOutputTypeDef",
     {
         "LogDestinationConfigs": List[LogDestinationConfigOutputTypeDef],
@@ -1432,32 +1310,19 @@
         "LogDestinationConfigs": Sequence[LogDestinationConfigTypeDef],
     },
 )
 
 ServerCertificateScopeOutputTypeDef = TypedDict(
     "ServerCertificateScopeOutputTypeDef",
     {
-        "Sources": List[AddressOutputTypeDef],
-        "Destinations": List[AddressOutputTypeDef],
-        "SourcePorts": List[PortRangeOutputTypeDef],
-        "DestinationPorts": List[PortRangeOutputTypeDef],
-        "Protocols": List[int],
-    },
-    total=False,
-)
-
-MatchAttributesOutputTypeDef = TypedDict(
-    "MatchAttributesOutputTypeDef",
-    {
-        "Sources": List[AddressOutputTypeDef],
-        "Destinations": List[AddressOutputTypeDef],
-        "SourcePorts": List[PortRangeOutputTypeDef],
-        "DestinationPorts": List[PortRangeOutputTypeDef],
+        "Sources": List[AddressTypeDef],
+        "Destinations": List[AddressTypeDef],
+        "SourcePorts": List[PortRangeTypeDef],
+        "DestinationPorts": List[PortRangeTypeDef],
         "Protocols": List[int],
-        "TCPFlags": List[TCPFlagFieldOutputTypeDef],
     },
     total=False,
 )
 
 ServerCertificateScopeTypeDef = TypedDict(
     "ServerCertificateScopeTypeDef",
     {
@@ -1466,14 +1331,27 @@
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
         "Protocols": Sequence[int],
     },
     total=False,
 )
 
+MatchAttributesOutputTypeDef = TypedDict(
+    "MatchAttributesOutputTypeDef",
+    {
+        "Sources": List[AddressTypeDef],
+        "Destinations": List[AddressTypeDef],
+        "SourcePorts": List[PortRangeTypeDef],
+        "DestinationPorts": List[PortRangeTypeDef],
+        "Protocols": List[int],
+        "TCPFlags": List[TCPFlagFieldOutputTypeDef],
+    },
+    total=False,
+)
+
 MatchAttributesTypeDef = TypedDict(
     "MatchAttributesTypeDef",
     {
         "Sources": Sequence[AddressTypeDef],
         "Destinations": Sequence[AddressTypeDef],
         "SourcePorts": Sequence[PortRangeTypeDef],
         "DestinationPorts": Sequence[PortRangeTypeDef],
@@ -1506,84 +1384,32 @@
     {
         "IPSets": Mapping[str, IPSetTypeDef],
         "PortSets": Mapping[str, PortSetTypeDef],
     },
     total=False,
 )
 
-_RequiredRuleGroupResponseTypeDef = TypedDict(
-    "_RequiredRuleGroupResponseTypeDef",
-    {
-        "RuleGroupArn": str,
-        "RuleGroupName": str,
-        "RuleGroupId": str,
-    },
-)
-_OptionalRuleGroupResponseTypeDef = TypedDict(
-    "_OptionalRuleGroupResponseTypeDef",
-    {
-        "Description": str,
-        "Type": RuleGroupTypeType,
-        "Capacity": int,
-        "RuleGroupStatus": ResourceStatusType,
-        "Tags": List[TagOutputTypeDef],
-        "ConsumedCapacity": int,
-        "NumberOfAssociations": int,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-        "SourceMetadata": SourceMetadataOutputTypeDef,
-        "SnsTopic": str,
-        "LastModifiedTime": datetime,
-    },
-    total=False,
-)
-
-class RuleGroupResponseTypeDef(
-    _RequiredRuleGroupResponseTypeDef, _OptionalRuleGroupResponseTypeDef
-):
-    pass
-
 StatefulRuleOutputTypeDef = TypedDict(
     "StatefulRuleOutputTypeDef",
     {
         "Action": StatefulActionType,
-        "Header": HeaderOutputTypeDef,
+        "Header": HeaderTypeDef,
         "RuleOptions": List[RuleOptionOutputTypeDef],
     },
 )
 
 StatefulRuleTypeDef = TypedDict(
     "StatefulRuleTypeDef",
     {
         "Action": StatefulActionType,
         "Header": HeaderTypeDef,
         "RuleOptions": Sequence[RuleOptionTypeDef],
     },
 )
 
-_RequiredStatefulRuleGroupReferenceOutputTypeDef = TypedDict(
-    "_RequiredStatefulRuleGroupReferenceOutputTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalStatefulRuleGroupReferenceOutputTypeDef = TypedDict(
-    "_OptionalStatefulRuleGroupReferenceOutputTypeDef",
-    {
-        "Priority": int,
-        "Override": StatefulRuleGroupOverrideOutputTypeDef,
-    },
-    total=False,
-)
-
-class StatefulRuleGroupReferenceOutputTypeDef(
-    _RequiredStatefulRuleGroupReferenceOutputTypeDef,
-    _OptionalStatefulRuleGroupReferenceOutputTypeDef,
-):
-    pass
-
 _RequiredStatefulRuleGroupReferenceTypeDef = TypedDict(
     "_RequiredStatefulRuleGroupReferenceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalStatefulRuleGroupReferenceTypeDef = TypedDict(
@@ -1609,18 +1435,18 @@
     },
 )
 _OptionalTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "_OptionalTLSInspectionConfigurationResponseTypeDef",
     {
         "TLSInspectionConfigurationStatus": ResourceStatusType,
         "Description": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "LastModifiedTime": datetime,
         "NumberOfAssociations": int,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "Certificates": List[TlsCertificateDataTypeDef],
     },
     total=False,
 )
 
 class TLSInspectionConfigurationResponseTypeDef(
     _RequiredTLSInspectionConfigurationResponseTypeDef,
@@ -1632,72 +1458,98 @@
     "CapacityUsageSummaryTypeDef",
     {
         "CIDRs": CIDRSummaryTypeDef,
     },
     total=False,
 )
 
-ActionDefinitionOutputTypeDef = TypedDict(
-    "ActionDefinitionOutputTypeDef",
-    {
-        "PublishMetricAction": PublishMetricActionOutputTypeDef,
-    },
-    total=False,
-)
-
-ActionDefinitionTypeDef = TypedDict(
-    "ActionDefinitionTypeDef",
-    {
-        "PublishMetricAction": PublishMetricActionTypeDef,
-    },
-    total=False,
-)
-
 CreateFirewallPolicyResponseTypeDef = TypedDict(
     "CreateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallPolicyResponseTypeDef = TypedDict(
     "DeleteFirewallPolicyResponseTypeDef",
     {
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallPolicyResponseTypeDef = TypedDict(
     "UpdateFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRuleGroupResponseTypeDef = TypedDict(
+    "CreateRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRuleGroupResponseTypeDef = TypedDict(
+    "DeleteRuleGroupResponseTypeDef",
+    {
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
+    {
+        "UpdateToken": str,
+        "RuleGroupResponse": RuleGroupResponseTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ActionDefinitionOutputTypeDef = TypedDict(
+    "ActionDefinitionOutputTypeDef",
+    {
+        "PublishMetricAction": PublishMetricActionOutputTypeDef,
     },
+    total=False,
+)
+
+ActionDefinitionTypeDef = TypedDict(
+    "ActionDefinitionTypeDef",
+    {
+        "PublishMetricAction": PublishMetricActionTypeDef,
+    },
+    total=False,
 )
 
 DescribeLoggingConfigurationResponseTypeDef = TypedDict(
     "DescribeLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
         "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLoggingConfigurationResponseTypeDef = TypedDict(
     "UpdateLoggingConfigurationResponseTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "FirewallArn": str,
@@ -1706,94 +1558,68 @@
     },
     total=False,
 )
 
 ServerCertificateConfigurationOutputTypeDef = TypedDict(
     "ServerCertificateConfigurationOutputTypeDef",
     {
-        "ServerCertificates": List[ServerCertificateOutputTypeDef],
+        "ServerCertificates": List[ServerCertificateTypeDef],
         "Scopes": List[ServerCertificateScopeOutputTypeDef],
     },
     total=False,
 )
 
-RuleDefinitionOutputTypeDef = TypedDict(
-    "RuleDefinitionOutputTypeDef",
-    {
-        "MatchAttributes": MatchAttributesOutputTypeDef,
-        "Actions": List[str],
-    },
-)
-
 ServerCertificateConfigurationTypeDef = TypedDict(
     "ServerCertificateConfigurationTypeDef",
     {
         "ServerCertificates": Sequence[ServerCertificateTypeDef],
         "Scopes": Sequence[ServerCertificateScopeTypeDef],
     },
     total=False,
 )
 
-RuleDefinitionTypeDef = TypedDict(
-    "RuleDefinitionTypeDef",
-    {
-        "MatchAttributes": MatchAttributesTypeDef,
-        "Actions": Sequence[str],
-    },
-)
-
-CreateRuleGroupResponseTypeDef = TypedDict(
-    "CreateRuleGroupResponseTypeDef",
-    {
-        "UpdateToken": str,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteRuleGroupResponseTypeDef = TypedDict(
-    "DeleteRuleGroupResponseTypeDef",
+RuleDefinitionOutputTypeDef = TypedDict(
+    "RuleDefinitionOutputTypeDef",
     {
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MatchAttributes": MatchAttributesOutputTypeDef,
+        "Actions": List[str],
     },
 )
 
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+RuleDefinitionTypeDef = TypedDict(
+    "RuleDefinitionTypeDef",
     {
-        "UpdateToken": str,
-        "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MatchAttributes": MatchAttributesTypeDef,
+        "Actions": Sequence[str],
     },
 )
 
 CreateTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "CreateTLSInspectionConfigurationResponseTypeDef",
     {
         "UpdateToken": str,
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "DeleteTLSInspectionConfigurationResponseTypeDef",
     {
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "UpdateTLSInspectionConfigurationResponseTypeDef",
     {
         "UpdateToken": str,
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFirewallStatusTypeDef = TypedDict(
     "_RequiredFirewallStatusTypeDef",
     {
         "Status": FirewallStatusValueType,
@@ -1832,81 +1658,81 @@
     "TLSInspectionConfigurationOutputTypeDef",
     {
         "ServerCertificateConfigurations": List[ServerCertificateConfigurationOutputTypeDef],
     },
     total=False,
 )
 
-StatelessRuleOutputTypeDef = TypedDict(
-    "StatelessRuleOutputTypeDef",
-    {
-        "RuleDefinition": RuleDefinitionOutputTypeDef,
-        "Priority": int,
-    },
-)
-
 TLSInspectionConfigurationTypeDef = TypedDict(
     "TLSInspectionConfigurationTypeDef",
     {
         "ServerCertificateConfigurations": Sequence[ServerCertificateConfigurationTypeDef],
     },
     total=False,
 )
 
+StatelessRuleOutputTypeDef = TypedDict(
+    "StatelessRuleOutputTypeDef",
+    {
+        "RuleDefinition": RuleDefinitionOutputTypeDef,
+        "Priority": int,
+    },
+)
+
 StatelessRuleTypeDef = TypedDict(
     "StatelessRuleTypeDef",
     {
         "RuleDefinition": RuleDefinitionTypeDef,
         "Priority": int,
     },
 )
 
 CreateFirewallResponseTypeDef = TypedDict(
     "CreateFirewallResponseTypeDef",
     {
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallResponseTypeDef = TypedDict(
     "DeleteFirewallResponseTypeDef",
     {
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFirewallResponseTypeDef = TypedDict(
     "DescribeFirewallResponseTypeDef",
     {
         "UpdateToken": str,
         "Firewall": FirewallTypeDef,
         "FirewallStatus": FirewallStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFirewallPolicyOutputTypeDef = TypedDict(
     "_RequiredFirewallPolicyOutputTypeDef",
     {
         "StatelessDefaultActions": List[str],
         "StatelessFragmentDefaultActions": List[str],
     },
 )
 _OptionalFirewallPolicyOutputTypeDef = TypedDict(
     "_OptionalFirewallPolicyOutputTypeDef",
     {
-        "StatelessRuleGroupReferences": List[StatelessRuleGroupReferenceOutputTypeDef],
+        "StatelessRuleGroupReferences": List[StatelessRuleGroupReferenceTypeDef],
         "StatelessCustomActions": List[CustomActionOutputTypeDef],
-        "StatefulRuleGroupReferences": List[StatefulRuleGroupReferenceOutputTypeDef],
+        "StatefulRuleGroupReferences": List[StatefulRuleGroupReferenceTypeDef],
         "StatefulDefaultActions": List[str],
-        "StatefulEngineOptions": StatefulEngineOptionsOutputTypeDef,
+        "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
         "TLSInspectionConfigurationArn": str,
         "PolicyVariables": PolicyVariablesOutputTypeDef,
     },
     total=False,
 )
 
 class FirewallPolicyOutputTypeDef(
@@ -1940,37 +1766,17 @@
 
 DescribeTLSInspectionConfigurationResponseTypeDef = TypedDict(
     "DescribeTLSInspectionConfigurationResponseTypeDef",
     {
         "UpdateToken": str,
         "TLSInspectionConfiguration": TLSInspectionConfigurationOutputTypeDef,
         "TLSInspectionConfigurationResponse": TLSInspectionConfigurationResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
-    "_RequiredStatelessRulesAndCustomActionsOutputTypeDef",
-    {
-        "StatelessRules": List[StatelessRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
-    "_OptionalStatelessRulesAndCustomActionsOutputTypeDef",
-    {
-        "CustomActions": List[CustomActionOutputTypeDef],
-    },
-    total=False,
-)
-
-class StatelessRulesAndCustomActionsOutputTypeDef(
-    _RequiredStatelessRulesAndCustomActionsOutputTypeDef,
-    _OptionalStatelessRulesAndCustomActionsOutputTypeDef,
-):
-    pass
 
 _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfigurationName": str,
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
     },
@@ -2011,14 +1817,34 @@
 
 class UpdateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalUpdateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
+_RequiredStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
+    "_RequiredStatelessRulesAndCustomActionsOutputTypeDef",
+    {
+        "StatelessRules": List[StatelessRuleOutputTypeDef],
+    },
+)
+_OptionalStatelessRulesAndCustomActionsOutputTypeDef = TypedDict(
+    "_OptionalStatelessRulesAndCustomActionsOutputTypeDef",
+    {
+        "CustomActions": List[CustomActionOutputTypeDef],
+    },
+    total=False,
+)
+
+class StatelessRulesAndCustomActionsOutputTypeDef(
+    _RequiredStatelessRulesAndCustomActionsOutputTypeDef,
+    _OptionalStatelessRulesAndCustomActionsOutputTypeDef,
+):
+    pass
+
 _RequiredStatelessRulesAndCustomActionsTypeDef = TypedDict(
     "_RequiredStatelessRulesAndCustomActionsTypeDef",
     {
         "StatelessRules": Sequence[StatelessRuleTypeDef],
     },
 )
 _OptionalStatelessRulesAndCustomActionsTypeDef = TypedDict(
@@ -2036,15 +1862,15 @@
 
 DescribeFirewallPolicyResponseTypeDef = TypedDict(
     "DescribeFirewallPolicyResponseTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicyResponse": FirewallPolicyResponseTypeDef,
         "FirewallPolicy": FirewallPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallPolicyRequestRequestTypeDef",
     {
         "FirewallPolicyName": str,
@@ -2122,15 +1948,15 @@
     },
 )
 _OptionalRuleGroupOutputTypeDef = TypedDict(
     "_OptionalRuleGroupOutputTypeDef",
     {
         "RuleVariables": RuleVariablesOutputTypeDef,
         "ReferenceSets": ReferenceSetsOutputTypeDef,
-        "StatefulRuleOptions": StatefulRuleOptionsOutputTypeDef,
+        "StatefulRuleOptions": StatefulRuleOptionsTypeDef,
     },
     total=False,
 )
 
 class RuleGroupOutputTypeDef(_RequiredRuleGroupOutputTypeDef, _OptionalRuleGroupOutputTypeDef):
     pass
 
@@ -2155,15 +1981,15 @@
 
 DescribeRuleGroupResponseTypeDef = TypedDict(
     "DescribeRuleGroupResponseTypeDef",
     {
         "UpdateToken": str,
         "RuleGroup": RuleGroupOutputTypeDef,
         "RuleGroupResponse": RuleGroupResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupName": str,
```

### Comparing `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/PKG-INFO` & `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-network-firewall
-Version: 1.28.12
-Summary: Type annotations for boto3.NetworkFirewall 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.NetworkFirewall 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-network-firewall)](https://pepy.tech/project/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,187 +361,172 @@
 ### Typed dictionaries
 
 `mypy_boto3_network_firewall.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_network_firewall.type_defs import (
-    AddressOutputTypeDef,
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
-    AssociateFirewallPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     SubnetMappingTypeDef,
-    SubnetMappingOutputTypeDef,
     AttachmentTypeDef,
     IPSetMetadataTypeDef,
     EncryptionConfigurationTypeDef,
     TagTypeDef,
     SourceMetadataTypeDef,
     DeleteFirewallPolicyRequestRequestTypeDef,
     DeleteFirewallRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteTLSInspectionConfigurationRequestRequestTypeDef,
     DescribeFirewallPolicyRequestRequestTypeDef,
     DescribeFirewallRequestRequestTypeDef,
     DescribeLoggingConfigurationRequestRequestTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataRequestRequestTypeDef,
-    StatefulRuleOptionsOutputTypeDef,
+    StatefulRuleOptionsTypeDef,
     DescribeRuleGroupRequestRequestTypeDef,
     DescribeTLSInspectionConfigurationRequestRequestTypeDef,
-    DimensionOutputTypeDef,
     DimensionTypeDef,
     DisassociateSubnetsRequestRequestTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     FirewallMetadataTypeDef,
     FirewallPolicyMetadataTypeDef,
-    StatefulEngineOptionsOutputTypeDef,
-    StatelessRuleGroupReferenceOutputTypeDef,
-    TagOutputTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupReferenceTypeDef,
-    HeaderOutputTypeDef,
     HeaderTypeDef,
     IPSetOutputTypeDef,
-    IPSetReferenceOutputTypeDef,
     IPSetReferenceTypeDef,
     IPSetTypeDef,
-    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListFirewallPoliciesRequestRequestTypeDef,
-    ListFirewallsRequestListFirewallsPaginateTypeDef,
     ListFirewallsRequestRequestTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupMetadataTypeDef,
-    ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
     ListTLSInspectionConfigurationsRequestRequestTypeDef,
     TLSInspectionConfigurationMetadataTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     LogDestinationConfigOutputTypeDef,
     LogDestinationConfigTypeDef,
-    PortRangeOutputTypeDef,
-    TCPFlagFieldOutputTypeDef,
     PortRangeTypeDef,
+    TCPFlagFieldOutputTypeDef,
     TCPFlagFieldTypeDef,
-    PaginatorConfigTypeDef,
     PerObjectStatusTypeDef,
     PortSetOutputTypeDef,
     PortSetTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SourceMetadataOutputTypeDef,
-    StatefulRuleOptionsTypeDef,
     RuleOptionOutputTypeDef,
     RuleOptionTypeDef,
     RulesSourceListOutputTypeDef,
     RulesSourceListTypeDef,
-    ServerCertificateOutputTypeDef,
     ServerCertificateTypeDef,
-    StatefulRuleGroupOverrideOutputTypeDef,
     StatefulRuleGroupOverrideTypeDef,
     TlsCertificateDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallDeleteProtectionRequestRequestTypeDef,
-    UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionRequestRequestTypeDef,
-    UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef,
-    UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateSubnetChangeProtectionRequestRequestTypeDef,
+    AssociateFirewallPolicyResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    UpdateFirewallDeleteProtectionResponseTypeDef,
+    UpdateFirewallDescriptionResponseTypeDef,
+    UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateSubnetChangeProtectionResponseTypeDef,
     AssociateSubnetsRequestRequestTypeDef,
     AssociateSubnetsResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     CIDRSummaryTypeDef,
     UpdateFirewallEncryptionConfigurationRequestRequestTypeDef,
+    UpdateFirewallEncryptionConfigurationResponseTypeDef,
     CreateFirewallRequestRequestTypeDef,
+    FirewallPolicyResponseTypeDef,
+    FirewallTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    RuleGroupResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     PublishMetricActionOutputTypeDef,
     PublishMetricActionTypeDef,
-    UpdateFirewallEncryptionConfigurationResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListFirewallPoliciesResponseTypeDef,
-    FirewallPolicyResponseTypeDef,
-    FirewallTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PolicyVariablesOutputTypeDef,
     ReferenceSetsOutputTypeDef,
     ReferenceSetsTypeDef,
     PolicyVariablesTypeDef,
+    ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef,
+    ListFirewallsRequestListFirewallsPaginateTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
+    ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     ServerCertificateScopeOutputTypeDef,
-    MatchAttributesOutputTypeDef,
     ServerCertificateScopeTypeDef,
+    MatchAttributesOutputTypeDef,
     MatchAttributesTypeDef,
     SyncStateTypeDef,
     RuleVariablesOutputTypeDef,
     RuleVariablesTypeDef,
-    RuleGroupResponseTypeDef,
     StatefulRuleOutputTypeDef,
     StatefulRuleTypeDef,
-    StatefulRuleGroupReferenceOutputTypeDef,
     StatefulRuleGroupReferenceTypeDef,
     TLSInspectionConfigurationResponseTypeDef,
     CapacityUsageSummaryTypeDef,
-    ActionDefinitionOutputTypeDef,
-    ActionDefinitionTypeDef,
     CreateFirewallPolicyResponseTypeDef,
     DeleteFirewallPolicyResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
+    CreateRuleGroupResponseTypeDef,
+    DeleteRuleGroupResponseTypeDef,
+    UpdateRuleGroupResponseTypeDef,
+    ActionDefinitionOutputTypeDef,
+    ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
     ServerCertificateConfigurationOutputTypeDef,
-    RuleDefinitionOutputTypeDef,
     ServerCertificateConfigurationTypeDef,
+    RuleDefinitionOutputTypeDef,
     RuleDefinitionTypeDef,
-    CreateRuleGroupResponseTypeDef,
-    DeleteRuleGroupResponseTypeDef,
-    UpdateRuleGroupResponseTypeDef,
     CreateTLSInspectionConfigurationResponseTypeDef,
     DeleteTLSInspectionConfigurationResponseTypeDef,
     UpdateTLSInspectionConfigurationResponseTypeDef,
     FirewallStatusTypeDef,
     CustomActionOutputTypeDef,
     CustomActionTypeDef,
     TLSInspectionConfigurationOutputTypeDef,
-    StatelessRuleOutputTypeDef,
     TLSInspectionConfigurationTypeDef,
+    StatelessRuleOutputTypeDef,
     StatelessRuleTypeDef,
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
     FirewallPolicyOutputTypeDef,
     FirewallPolicyTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
-    StatelessRulesAndCustomActionsOutputTypeDef,
     CreateTLSInspectionConfigurationRequestRequestTypeDef,
     UpdateTLSInspectionConfigurationRequestRequestTypeDef,
+    StatelessRulesAndCustomActionsOutputTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
     CreateFirewallPolicyRequestRequestTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
     RulesSourceOutputTypeDef,
     RulesSourceTypeDef,
     RuleGroupOutputTypeDef,
     RuleGroupTypeDef,
     DescribeRuleGroupResponseTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddressOutputTypeDef:
+def get_structure() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-network-firewall-1.28.12/mypy_boto3_network_firewall.egg-info/SOURCES.txt` & `mypy-boto3-network-firewall-1.28.15/mypy_boto3_network_firewall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.12/setup.py` & `mypy-boto3-network-firewall-1.28.15/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-network-firewall",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_network_firewall"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.NetworkFirewall 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.NetworkFirewall 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

