# Comparing `tmp/mypy-boto3-apigatewayv2-1.28.12.tar.gz` & `tmp/mypy-boto3-apigatewayv2-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apigatewayv2-1.28.12.tar", last modified: Thu Jul 27 05:34:16 2023, max compression
+gzip compressed data, was "mypy-boto3-apigatewayv2-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
```

## Comparing `mypy-boto3-apigatewayv2-1.28.12.tar` & `mypy-boto3-apigatewayv2-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.252584 mypy-boto3-apigatewayv2-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:12.000000 mypy-boto3-apigatewayv2-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20692 2023-07-27 05:34:16.252584 mypy-boto3-apigatewayv2-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19185 2023-07-27 05:17:12.000000 mypy-boto3-apigatewayv2-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.248584 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-27 05:17:12.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-27 05:17:12.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:17:12.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51692 2023-07-27 05:17:13.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51603 2023-07-27 05:17:13.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-07-27 05:17:13.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-27 05:17:13.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-27 05:17:13.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-07-27 05:17:13.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:12.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    77301 2023-07-27 05:17:15.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    77190 2023-07-27 05:17:14.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:12.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.248584 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20692 2023-07-27 05:34:16.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:16.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:16.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:16.000000 mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:16.252584 mypy-boto3-apigatewayv2-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:17:12.000000 mypy-boto3-apigatewayv2-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.256654 mypy-boto3-apigatewayv2-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-07-28 20:42:16.252654 mypy-boto3-apigatewayv2-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19072 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.248654 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51692 2023-07-28 20:19:08.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51603 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-07-28 20:19:08.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-28 20:19:08.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-28 20:19:08.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-07-28 20:19:08.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    76314 2023-07-28 20:19:11.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76203 2023-07-28 20:19:10.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.252654 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-07-28 20:42:16.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:16.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:16.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:16.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.256654 mypy-boto3-apigatewayv2-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/setup.py
```

### Comparing `mypy-boto3-apigatewayv2-1.28.12/LICENSE` & `mypy-boto3-apigatewayv2-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.12/PKG-INFO` & `mypy-boto3-apigatewayv2-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewayv2
-Version: 1.28.12
-Summary: Type annotations for boto3.ApiGatewayV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ApiGatewayV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewayv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigatewayv2)](https://pepy.tech/project/mypy-boto3-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[boto3.ApiGatewayV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
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
 [mypy-boto3-apigatewayv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,41 +368,34 @@
 ### Typed dictionaries
 
 `mypy_boto3_apigatewayv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigatewayv2.type_defs import (
-    AccessLogSettingsOutputTypeDef,
     AccessLogSettingsTypeDef,
     ApiMappingTypeDef,
     CorsOutputTypeDef,
     JWTConfigurationOutputTypeDef,
     CorsTypeDef,
     CreateApiMappingRequestRequestTypeDef,
-    CreateApiMappingResponseTypeDef,
+    ResponseMetadataTypeDef,
     JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
     DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
     DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
-    CreateIntegrationResponseResponseTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
-    CreateModelResponseTypeDef,
     ParameterConstraintsTypeDef,
-    ParameterConstraintsOutputTypeDef,
     RouteSettingsTypeDef,
-    RouteSettingsOutputTypeDef,
     CreateVpcLinkRequestRequestTypeDef,
-    CreateVpcLinkResponseTypeDef,
     DeleteAccessLogSettingsRequestRequestTypeDef,
     DeleteApiMappingRequestRequestTypeDef,
     DeleteApiRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteCorsConfigurationRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
     DeleteDomainNameRequestRequestTypeDef,
@@ -412,93 +405,87 @@
     DeleteRouteRequestParameterRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseRequestRequestTypeDef,
     DeleteRouteSettingsRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     DeploymentTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportApiRequestRequestTypeDef,
-    ExportApiResponseTypeDef,
     GetApiMappingRequestRequestTypeDef,
-    GetApiMappingResponseTypeDef,
     GetApiMappingsRequestRequestTypeDef,
     GetApiRequestRequestTypeDef,
-    GetApisRequestGetApisPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetApisRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
-    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetAuthorizersRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetDeploymentResponseTypeDef,
-    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
-    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetDomainNamesRequestRequestTypeDef,
     GetIntegrationRequestRequestTypeDef,
     GetIntegrationResponseRequestRequestTypeDef,
-    GetIntegrationResponseResponseTypeDef,
-    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
     GetIntegrationResponsesRequestRequestTypeDef,
     IntegrationResponseTypeDef,
-    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
     GetIntegrationsRequestRequestTypeDef,
     GetModelRequestRequestTypeDef,
-    GetModelResponseTypeDef,
     GetModelTemplateRequestRequestTypeDef,
-    GetModelTemplateResponseTypeDef,
-    GetModelsRequestGetModelsPaginateTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetRouteRequestRequestTypeDef,
     GetRouteResponseRequestRequestTypeDef,
-    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
     GetRouteResponsesRequestRequestTypeDef,
-    GetRoutesRequestGetRoutesPaginateTypeDef,
     GetRoutesRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    GetStagesRequestGetStagesPaginateTypeDef,
     GetStagesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
-    GetTagsResponseTypeDef,
     GetVpcLinkRequestRequestTypeDef,
-    GetVpcLinkResponseTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     VpcLinkTypeDef,
     ImportApiRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ReimportApiRequestRequestTypeDef,
     ResetAuthorizersCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiMappingRequestRequestTypeDef,
-    UpdateApiMappingResponseTypeDef,
     UpdateDeploymentRequestRequestTypeDef,
-    UpdateDeploymentResponseTypeDef,
     UpdateIntegrationResponseRequestRequestTypeDef,
-    UpdateIntegrationResponseResponseTypeDef,
     UpdateModelRequestRequestTypeDef,
-    UpdateModelResponseTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
-    UpdateVpcLinkResponseTypeDef,
-    GetApiMappingsResponseTypeDef,
     ApiTypeDef,
+    AuthorizerTypeDef,
+    CreateApiRequestRequestTypeDef,
+    UpdateApiRequestRequestTypeDef,
+    CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateIntegrationResponseResponseTypeDef,
+    CreateModelResponseTypeDef,
+    CreateVpcLinkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportApiResponseTypeDef,
+    GetApiMappingResponseTypeDef,
+    GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
+    GetAuthorizerResponseTypeDef,
+    GetDeploymentResponseTypeDef,
+    GetIntegrationResponseResponseTypeDef,
+    GetModelResponseTypeDef,
+    GetModelTemplateResponseTypeDef,
+    GetTagsResponseTypeDef,
+    GetVpcLinkResponseTypeDef,
     ImportApiResponseTypeDef,
     ReimportApiResponseTypeDef,
+    UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
-    AuthorizerTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    GetAuthorizerResponseTypeDef,
     UpdateAuthorizerResponseTypeDef,
-    CreateApiRequestRequestTypeDef,
-    UpdateApiRequestRequestTypeDef,
+    UpdateDeploymentResponseTypeDef,
+    UpdateIntegrationResponseResponseTypeDef,
+    UpdateModelResponseTypeDef,
+    UpdateVpcLinkResponseTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
     CreateDomainNameRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     CreateDomainNameResponseTypeDef,
     DomainNameTypeDef,
     GetDomainNameResponseTypeDef,
@@ -507,45 +494,55 @@
     UpdateIntegrationRequestRequestTypeDef,
     CreateIntegrationResultTypeDef,
     GetIntegrationResultTypeDef,
     IntegrationTypeDef,
     UpdateIntegrationResultTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseRequestRequestTypeDef,
-    UpdateRouteRequestRequestTypeDef,
-    UpdateRouteResponseRequestRequestTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     GetRouteResponseResponseTypeDef,
     GetRouteResultTypeDef,
     RouteResponseTypeDef,
     RouteTypeDef,
+    UpdateRouteRequestRequestTypeDef,
+    UpdateRouteResponseRequestRequestTypeDef,
     UpdateRouteResponseResponseTypeDef,
     UpdateRouteResultTypeDef,
     CreateStageRequestRequestTypeDef,
-    UpdateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     StageTypeDef,
+    UpdateStageRequestRequestTypeDef,
     UpdateStageResponseTypeDef,
     GetDeploymentsResponseTypeDef,
+    GetApisRequestGetApisPaginateTypeDef,
+    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
+    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    GetModelsRequestGetModelsPaginateTypeDef,
+    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    GetRoutesRequestGetRoutesPaginateTypeDef,
+    GetStagesRequestGetStagesPaginateTypeDef,
     GetIntegrationResponsesResponseTypeDef,
     GetModelsResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizersResponseTypeDef,
     GetDomainNamesResponseTypeDef,
     GetIntegrationsResponseTypeDef,
     GetRouteResponsesResponseTypeDef,
     GetRoutesResponseTypeDef,
     GetStagesResponseTypeDef,
 )
 
 
-def get_structure() -> AccessLogSettingsOutputTypeDef:
+def get_structure() -> AccessLogSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apigatewayv2-1.28.12/README.md` & `mypy-boto3-apigatewayv2-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewayv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigatewayv2)](https://pepy.tech/project/mypy-boto3-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[boto3.ApiGatewayV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
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
 [mypy-boto3-apigatewayv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,41 +336,34 @@
 ### Typed dictionaries
 
 `mypy_boto3_apigatewayv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigatewayv2.type_defs import (
-    AccessLogSettingsOutputTypeDef,
     AccessLogSettingsTypeDef,
     ApiMappingTypeDef,
     CorsOutputTypeDef,
     JWTConfigurationOutputTypeDef,
     CorsTypeDef,
     CreateApiMappingRequestRequestTypeDef,
-    CreateApiMappingResponseTypeDef,
+    ResponseMetadataTypeDef,
     JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
     DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
     DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
-    CreateIntegrationResponseResponseTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
-    CreateModelResponseTypeDef,
     ParameterConstraintsTypeDef,
-    ParameterConstraintsOutputTypeDef,
     RouteSettingsTypeDef,
-    RouteSettingsOutputTypeDef,
     CreateVpcLinkRequestRequestTypeDef,
-    CreateVpcLinkResponseTypeDef,
     DeleteAccessLogSettingsRequestRequestTypeDef,
     DeleteApiMappingRequestRequestTypeDef,
     DeleteApiRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteCorsConfigurationRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
     DeleteDomainNameRequestRequestTypeDef,
@@ -380,93 +373,87 @@
     DeleteRouteRequestParameterRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseRequestRequestTypeDef,
     DeleteRouteSettingsRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     DeploymentTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportApiRequestRequestTypeDef,
-    ExportApiResponseTypeDef,
     GetApiMappingRequestRequestTypeDef,
-    GetApiMappingResponseTypeDef,
     GetApiMappingsRequestRequestTypeDef,
     GetApiRequestRequestTypeDef,
-    GetApisRequestGetApisPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetApisRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
-    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetAuthorizersRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetDeploymentResponseTypeDef,
-    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
-    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetDomainNamesRequestRequestTypeDef,
     GetIntegrationRequestRequestTypeDef,
     GetIntegrationResponseRequestRequestTypeDef,
-    GetIntegrationResponseResponseTypeDef,
-    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
     GetIntegrationResponsesRequestRequestTypeDef,
     IntegrationResponseTypeDef,
-    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
     GetIntegrationsRequestRequestTypeDef,
     GetModelRequestRequestTypeDef,
-    GetModelResponseTypeDef,
     GetModelTemplateRequestRequestTypeDef,
-    GetModelTemplateResponseTypeDef,
-    GetModelsRequestGetModelsPaginateTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetRouteRequestRequestTypeDef,
     GetRouteResponseRequestRequestTypeDef,
-    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
     GetRouteResponsesRequestRequestTypeDef,
-    GetRoutesRequestGetRoutesPaginateTypeDef,
     GetRoutesRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    GetStagesRequestGetStagesPaginateTypeDef,
     GetStagesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
-    GetTagsResponseTypeDef,
     GetVpcLinkRequestRequestTypeDef,
-    GetVpcLinkResponseTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     VpcLinkTypeDef,
     ImportApiRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ReimportApiRequestRequestTypeDef,
     ResetAuthorizersCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiMappingRequestRequestTypeDef,
-    UpdateApiMappingResponseTypeDef,
     UpdateDeploymentRequestRequestTypeDef,
-    UpdateDeploymentResponseTypeDef,
     UpdateIntegrationResponseRequestRequestTypeDef,
-    UpdateIntegrationResponseResponseTypeDef,
     UpdateModelRequestRequestTypeDef,
-    UpdateModelResponseTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
-    UpdateVpcLinkResponseTypeDef,
-    GetApiMappingsResponseTypeDef,
     ApiTypeDef,
+    AuthorizerTypeDef,
+    CreateApiRequestRequestTypeDef,
+    UpdateApiRequestRequestTypeDef,
+    CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateIntegrationResponseResponseTypeDef,
+    CreateModelResponseTypeDef,
+    CreateVpcLinkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportApiResponseTypeDef,
+    GetApiMappingResponseTypeDef,
+    GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
+    GetAuthorizerResponseTypeDef,
+    GetDeploymentResponseTypeDef,
+    GetIntegrationResponseResponseTypeDef,
+    GetModelResponseTypeDef,
+    GetModelTemplateResponseTypeDef,
+    GetTagsResponseTypeDef,
+    GetVpcLinkResponseTypeDef,
     ImportApiResponseTypeDef,
     ReimportApiResponseTypeDef,
+    UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
-    AuthorizerTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    GetAuthorizerResponseTypeDef,
     UpdateAuthorizerResponseTypeDef,
-    CreateApiRequestRequestTypeDef,
-    UpdateApiRequestRequestTypeDef,
+    UpdateDeploymentResponseTypeDef,
+    UpdateIntegrationResponseResponseTypeDef,
+    UpdateModelResponseTypeDef,
+    UpdateVpcLinkResponseTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
     CreateDomainNameRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     CreateDomainNameResponseTypeDef,
     DomainNameTypeDef,
     GetDomainNameResponseTypeDef,
@@ -475,45 +462,55 @@
     UpdateIntegrationRequestRequestTypeDef,
     CreateIntegrationResultTypeDef,
     GetIntegrationResultTypeDef,
     IntegrationTypeDef,
     UpdateIntegrationResultTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseRequestRequestTypeDef,
-    UpdateRouteRequestRequestTypeDef,
-    UpdateRouteResponseRequestRequestTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     GetRouteResponseResponseTypeDef,
     GetRouteResultTypeDef,
     RouteResponseTypeDef,
     RouteTypeDef,
+    UpdateRouteRequestRequestTypeDef,
+    UpdateRouteResponseRequestRequestTypeDef,
     UpdateRouteResponseResponseTypeDef,
     UpdateRouteResultTypeDef,
     CreateStageRequestRequestTypeDef,
-    UpdateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     StageTypeDef,
+    UpdateStageRequestRequestTypeDef,
     UpdateStageResponseTypeDef,
     GetDeploymentsResponseTypeDef,
+    GetApisRequestGetApisPaginateTypeDef,
+    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
+    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    GetModelsRequestGetModelsPaginateTypeDef,
+    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    GetRoutesRequestGetRoutesPaginateTypeDef,
+    GetStagesRequestGetStagesPaginateTypeDef,
     GetIntegrationResponsesResponseTypeDef,
     GetModelsResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizersResponseTypeDef,
     GetDomainNamesResponseTypeDef,
     GetIntegrationsResponseTypeDef,
     GetRouteResponsesResponseTypeDef,
     GetRoutesResponseTypeDef,
     GetStagesResponseTypeDef,
 )
 
 
-def get_structure() -> AccessLogSettingsOutputTypeDef:
+def get_structure() -> AccessLogSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/__init__.py` & `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/__init__.pyi` & `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/__main__.py` & `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApiGatewayV2 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ApiGatewayV2 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2\nOther"
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

### Comparing `mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/client.py` & `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/client.pyi` & `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/literals.py` & `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/literals.pyi` & `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/paginator.py` & `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,148 +82,148 @@
 class GetApisPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetApis)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getapispaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetApisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetApis.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getapispaginator)
         """
 
 
 class GetAuthorizersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetAuthorizers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getauthorizerspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAuthorizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetAuthorizers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getauthorizerspaginator)
         """
 
 
 class GetDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdeploymentspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdeploymentspaginator)
         """
 
 
 class GetDomainNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDomainNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdomainnamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDomainNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDomainNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdomainnamespaginator)
         """
 
 
 class GetIntegrationResponsesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrationResponses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationresponsespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, IntegrationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, IntegrationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetIntegrationResponsesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrationResponses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationresponsespaginator)
         """
 
 
 class GetIntegrationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetIntegrationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationspaginator)
         """
 
 
 class GetModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getmodelspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getmodelspaginator)
         """
 
 
 class GetRouteResponsesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRouteResponses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getrouteresponsespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, RouteId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, RouteId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRouteResponsesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRouteResponses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getrouteresponsespaginator)
         """
 
 
 class GetRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getroutespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRoutesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getroutespaginator)
         """
 
 
 class GetStagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetStages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getstagespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetStagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetStages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getstagespaginator)
         """
```

### Comparing `mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/paginator.pyi` & `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -79,139 +79,139 @@
 class GetApisPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetApis)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getapispaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetApisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetApis.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getapispaginator)
         """
 
 class GetAuthorizersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetAuthorizers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getauthorizerspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetAuthorizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetAuthorizers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getauthorizerspaginator)
         """
 
 class GetDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdeploymentspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdeploymentspaginator)
         """
 
 class GetDomainNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDomainNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdomainnamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDomainNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDomainNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getdomainnamespaginator)
         """
 
 class GetIntegrationResponsesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrationResponses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationresponsespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, IntegrationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, IntegrationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetIntegrationResponsesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrationResponses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationresponsespaginator)
         """
 
 class GetIntegrationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetIntegrationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getintegrationspaginator)
         """
 
 class GetModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getmodelspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getmodelspaginator)
         """
 
 class GetRouteResponsesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRouteResponses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getrouteresponsespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, RouteId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, RouteId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRouteResponsesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRouteResponses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getrouteresponsespaginator)
         """
 
 class GetRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getroutespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRoutesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getroutespaginator)
         """
 
 class GetStagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetStages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getstagespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetStagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetStages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/paginators/#getstagespaginator)
         """
```

### Comparing `mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/type_defs.py` & `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for apigatewayv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_apigatewayv2.type_defs import AccessLogSettingsOutputTypeDef
+    from mypy_boto3_apigatewayv2.type_defs import AccessLogSettingsTypeDef
 
-    data: AccessLogSettingsOutputTypeDef = {...}
+    data: AccessLogSettingsTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -41,41 +41,34 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AccessLogSettingsOutputTypeDef",
     "AccessLogSettingsTypeDef",
     "ApiMappingTypeDef",
     "CorsOutputTypeDef",
     "JWTConfigurationOutputTypeDef",
     "CorsTypeDef",
     "CreateApiMappingRequestRequestTypeDef",
-    "CreateApiMappingResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "JWTConfigurationTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "CreateDeploymentResponseTypeDef",
     "DomainNameConfigurationTypeDef",
     "MutualTlsAuthenticationInputTypeDef",
     "DomainNameConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "TlsConfigInputTypeDef",
     "CreateIntegrationResponseRequestRequestTypeDef",
-    "CreateIntegrationResponseResponseTypeDef",
     "TlsConfigTypeDef",
     "CreateModelRequestRequestTypeDef",
-    "CreateModelResponseTypeDef",
     "ParameterConstraintsTypeDef",
-    "ParameterConstraintsOutputTypeDef",
     "RouteSettingsTypeDef",
-    "RouteSettingsOutputTypeDef",
     "CreateVpcLinkRequestRequestTypeDef",
-    "CreateVpcLinkResponseTypeDef",
     "DeleteAccessLogSettingsRequestRequestTypeDef",
     "DeleteApiMappingRequestRequestTypeDef",
     "DeleteApiRequestRequestTypeDef",
     "DeleteAuthorizerRequestRequestTypeDef",
     "DeleteCorsConfigurationRequestRequestTypeDef",
     "DeleteDeploymentRequestRequestTypeDef",
     "DeleteDomainNameRequestRequestTypeDef",
@@ -85,93 +78,87 @@
     "DeleteRouteRequestParameterRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
     "DeleteRouteResponseRequestRequestTypeDef",
     "DeleteRouteSettingsRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeleteVpcLinkRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportApiRequestRequestTypeDef",
-    "ExportApiResponseTypeDef",
     "GetApiMappingRequestRequestTypeDef",
-    "GetApiMappingResponseTypeDef",
     "GetApiMappingsRequestRequestTypeDef",
     "GetApiRequestRequestTypeDef",
-    "GetApisRequestGetApisPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetApisRequestRequestTypeDef",
     "GetAuthorizerRequestRequestTypeDef",
-    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
     "GetAuthorizersRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
-    "GetDeploymentResponseTypeDef",
-    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDomainNameRequestRequestTypeDef",
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
     "GetDomainNamesRequestRequestTypeDef",
     "GetIntegrationRequestRequestTypeDef",
     "GetIntegrationResponseRequestRequestTypeDef",
-    "GetIntegrationResponseResponseTypeDef",
-    "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
     "GetIntegrationResponsesRequestRequestTypeDef",
     "IntegrationResponseTypeDef",
-    "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
     "GetIntegrationsRequestRequestTypeDef",
     "GetModelRequestRequestTypeDef",
-    "GetModelResponseTypeDef",
     "GetModelTemplateRequestRequestTypeDef",
-    "GetModelTemplateResponseTypeDef",
-    "GetModelsRequestGetModelsPaginateTypeDef",
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetRouteRequestRequestTypeDef",
     "GetRouteResponseRequestRequestTypeDef",
-    "GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
     "GetRouteResponsesRequestRequestTypeDef",
-    "GetRoutesRequestGetRoutesPaginateTypeDef",
     "GetRoutesRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
-    "GetStagesRequestGetStagesPaginateTypeDef",
     "GetStagesRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
-    "GetTagsResponseTypeDef",
     "GetVpcLinkRequestRequestTypeDef",
-    "GetVpcLinkResponseTypeDef",
     "GetVpcLinksRequestRequestTypeDef",
     "VpcLinkTypeDef",
     "ImportApiRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ReimportApiRequestRequestTypeDef",
     "ResetAuthorizersCacheRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiMappingRequestRequestTypeDef",
-    "UpdateApiMappingResponseTypeDef",
     "UpdateDeploymentRequestRequestTypeDef",
-    "UpdateDeploymentResponseTypeDef",
     "UpdateIntegrationResponseRequestRequestTypeDef",
-    "UpdateIntegrationResponseResponseTypeDef",
     "UpdateModelRequestRequestTypeDef",
-    "UpdateModelResponseTypeDef",
     "UpdateVpcLinkRequestRequestTypeDef",
-    "UpdateVpcLinkResponseTypeDef",
-    "GetApiMappingsResponseTypeDef",
     "ApiTypeDef",
+    "AuthorizerTypeDef",
+    "CreateApiRequestRequestTypeDef",
+    "UpdateApiRequestRequestTypeDef",
+    "CreateApiMappingResponseTypeDef",
     "CreateApiResponseTypeDef",
+    "CreateAuthorizerResponseTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "CreateIntegrationResponseResponseTypeDef",
+    "CreateModelResponseTypeDef",
+    "CreateVpcLinkResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportApiResponseTypeDef",
+    "GetApiMappingResponseTypeDef",
+    "GetApiMappingsResponseTypeDef",
     "GetApiResponseTypeDef",
+    "GetAuthorizerResponseTypeDef",
+    "GetDeploymentResponseTypeDef",
+    "GetIntegrationResponseResponseTypeDef",
+    "GetModelResponseTypeDef",
+    "GetModelTemplateResponseTypeDef",
+    "GetTagsResponseTypeDef",
+    "GetVpcLinkResponseTypeDef",
     "ImportApiResponseTypeDef",
     "ReimportApiResponseTypeDef",
+    "UpdateApiMappingResponseTypeDef",
     "UpdateApiResponseTypeDef",
-    "AuthorizerTypeDef",
-    "CreateAuthorizerResponseTypeDef",
-    "GetAuthorizerResponseTypeDef",
     "UpdateAuthorizerResponseTypeDef",
-    "CreateApiRequestRequestTypeDef",
-    "UpdateApiRequestRequestTypeDef",
+    "UpdateDeploymentResponseTypeDef",
+    "UpdateIntegrationResponseResponseTypeDef",
+    "UpdateModelResponseTypeDef",
+    "UpdateVpcLinkResponseTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
     "CreateDomainNameRequestRequestTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
     "CreateDomainNameResponseTypeDef",
     "DomainNameTypeDef",
     "GetDomainNameResponseTypeDef",
@@ -180,52 +167,53 @@
     "UpdateIntegrationRequestRequestTypeDef",
     "CreateIntegrationResultTypeDef",
     "GetIntegrationResultTypeDef",
     "IntegrationTypeDef",
     "UpdateIntegrationResultTypeDef",
     "CreateRouteRequestRequestTypeDef",
     "CreateRouteResponseRequestRequestTypeDef",
-    "UpdateRouteRequestRequestTypeDef",
-    "UpdateRouteResponseRequestRequestTypeDef",
     "CreateRouteResponseResponseTypeDef",
     "CreateRouteResultTypeDef",
     "GetRouteResponseResponseTypeDef",
     "GetRouteResultTypeDef",
     "RouteResponseTypeDef",
     "RouteTypeDef",
+    "UpdateRouteRequestRequestTypeDef",
+    "UpdateRouteResponseRequestRequestTypeDef",
     "UpdateRouteResponseResponseTypeDef",
     "UpdateRouteResultTypeDef",
     "CreateStageRequestRequestTypeDef",
-    "UpdateStageRequestRequestTypeDef",
     "CreateStageResponseTypeDef",
     "GetStageResponseTypeDef",
     "StageTypeDef",
+    "UpdateStageRequestRequestTypeDef",
     "UpdateStageResponseTypeDef",
     "GetDeploymentsResponseTypeDef",
+    "GetApisRequestGetApisPaginateTypeDef",
+    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
+    "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    "GetModelsRequestGetModelsPaginateTypeDef",
+    "GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    "GetRoutesRequestGetRoutesPaginateTypeDef",
+    "GetStagesRequestGetStagesPaginateTypeDef",
     "GetIntegrationResponsesResponseTypeDef",
     "GetModelsResponseTypeDef",
     "GetVpcLinksResponseTypeDef",
     "GetApisResponseTypeDef",
     "GetAuthorizersResponseTypeDef",
     "GetDomainNamesResponseTypeDef",
     "GetIntegrationsResponseTypeDef",
     "GetRouteResponsesResponseTypeDef",
     "GetRoutesResponseTypeDef",
     "GetStagesResponseTypeDef",
 )
 
-AccessLogSettingsOutputTypeDef = TypedDict(
-    "AccessLogSettingsOutputTypeDef",
-    {
-        "DestinationArn": str,
-        "Format": str,
-    },
-    total=False,
-)
-
 AccessLogSettingsTypeDef = TypedDict(
     "AccessLogSettingsTypeDef",
     {
         "DestinationArn": str,
         "Format": str,
     },
     total=False,
@@ -306,22 +294,22 @@
 
 class CreateApiMappingRequestRequestTypeDef(
     _RequiredCreateApiMappingRequestRequestTypeDef, _OptionalCreateApiMappingRequestRequestTypeDef
 ):
     pass
 
 
-CreateApiMappingResponseTypeDef = TypedDict(
-    "CreateApiMappingResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 JWTConfigurationTypeDef = TypedDict(
     "JWTConfigurationTypeDef",
     {
         "Audience": Sequence[str],
@@ -348,27 +336,14 @@
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DomainNameConfigurationTypeDef = TypedDict(
     "DomainNameConfigurationTypeDef",
     {
         "ApiGatewayDomainName": str,
         "CertificateArn": str,
         "CertificateName": str,
         "CertificateUploadDate": Union[datetime, str],
@@ -449,27 +424,14 @@
 class CreateIntegrationResponseRequestRequestTypeDef(
     _RequiredCreateIntegrationResponseRequestRequestTypeDef,
     _OptionalCreateIntegrationResponseRequestRequestTypeDef,
 ):
     pass
 
 
-CreateIntegrationResponseResponseTypeDef = TypedDict(
-    "CreateIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TlsConfigTypeDef = TypedDict(
     "TlsConfigTypeDef",
     {
         "ServerNameToVerify": str,
     },
     total=False,
 )
@@ -494,66 +456,34 @@
 
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
 
-CreateModelResponseTypeDef = TypedDict(
-    "CreateModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "Required": bool,
     },
     total=False,
 )
 
-ParameterConstraintsOutputTypeDef = TypedDict(
-    "ParameterConstraintsOutputTypeDef",
-    {
-        "Required": bool,
-    },
-    total=False,
-)
-
 RouteSettingsTypeDef = TypedDict(
     "RouteSettingsTypeDef",
     {
         "DataTraceEnabled": bool,
         "DetailedMetricsEnabled": bool,
         "LoggingLevel": LoggingLevelType,
         "ThrottlingBurstLimit": int,
         "ThrottlingRateLimit": float,
     },
     total=False,
 )
 
-RouteSettingsOutputTypeDef = TypedDict(
-    "RouteSettingsOutputTypeDef",
-    {
-        "DataTraceEnabled": bool,
-        "DetailedMetricsEnabled": bool,
-        "LoggingLevel": LoggingLevelType,
-        "ThrottlingBurstLimit": int,
-        "ThrottlingRateLimit": float,
-    },
-    total=False,
-)
-
 _RequiredCreateVpcLinkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcLinkRequestRequestTypeDef",
     {
         "Name": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -569,30 +499,14 @@
 
 class CreateVpcLinkRequestRequestTypeDef(
     _RequiredCreateVpcLinkRequestRequestTypeDef, _OptionalCreateVpcLinkRequestRequestTypeDef
 ):
     pass
 
 
-CreateVpcLinkResponseTypeDef = TypedDict(
-    "CreateVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccessLogSettingsRequestRequestTypeDef = TypedDict(
     "DeleteAccessLogSettingsRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
@@ -726,21 +640,14 @@
         "DeploymentStatus": DeploymentStatusType,
         "DeploymentStatusMessage": str,
         "Description": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExportApiRequestRequestTypeDef = TypedDict(
     "_RequiredExportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "OutputType": JSONYAMLType,
         "Specification": Literal["OAS30"],
     },
@@ -758,41 +665,22 @@
 
 class ExportApiRequestRequestTypeDef(
     _RequiredExportApiRequestRequestTypeDef, _OptionalExportApiRequestRequestTypeDef
 ):
     pass
 
 
-ExportApiResponseTypeDef = TypedDict(
-    "ExportApiResponseTypeDef",
-    {
-        "body": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApiMappingRequestRequestTypeDef = TypedDict(
     "GetApiMappingRequestRequestTypeDef",
     {
         "ApiMappingId": str,
         "DomainName": str,
     },
 )
 
-GetApiMappingResponseTypeDef = TypedDict(
-    "GetApiMappingResponseTypeDef",
-    {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetApiMappingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetApiMappingsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetApiMappingsRequestRequestTypeDef = TypedDict(
@@ -814,18 +702,20 @@
 GetApiRequestRequestTypeDef = TypedDict(
     "GetApiRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 
-GetApisRequestGetApisPaginateTypeDef = TypedDict(
-    "GetApisRequestGetApisPaginateTypeDef",
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
 
 GetApisRequestRequestTypeDef = TypedDict(
     "GetApisRequestRequestTypeDef",
     {
@@ -839,36 +729,14 @@
     "GetAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerId": str,
     },
 )
 
-_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
-    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetAuthorizersRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizersRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetAuthorizersRequestRequestTypeDef = TypedDict(
@@ -891,49 +759,14 @@
     "GetDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
         "DeploymentId": str,
     },
 )
 
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
-    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeploymentsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetDeploymentsRequestRequestTypeDef = TypedDict(
@@ -955,22 +788,14 @@
 GetDomainNameRequestRequestTypeDef = TypedDict(
     "GetDomainNameRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetDomainNamesRequestRequestTypeDef = TypedDict(
     "GetDomainNamesRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -989,50 +814,14 @@
     {
         "ApiId": str,
         "IntegrationId": str,
         "IntegrationResponseId": str,
     },
 )
 
-GetIntegrationResponseResponseTypeDef = TypedDict(
-    "GetIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
-    {
-        "ApiId": str,
-        "IntegrationId": str,
-    },
-)
-_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef(
-    _RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
-    _OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetIntegrationResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntegrationResponsesRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
     },
 )
@@ -1074,36 +863,14 @@
 
 class IntegrationResponseTypeDef(
     _RequiredIntegrationResponseTypeDef, _OptionalIntegrationResponseTypeDef
 ):
     pass
 
 
-_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
-    "_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
-    "_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetIntegrationsRequestGetIntegrationsPaginateTypeDef(
-    _RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
-    _OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetIntegrationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntegrationsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetIntegrationsRequestRequestTypeDef = TypedDict(
@@ -1126,64 +893,22 @@
     "GetModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
 
-GetModelResponseTypeDef = TypedDict(
-    "GetModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetModelTemplateRequestRequestTypeDef = TypedDict(
     "GetModelTemplateRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
 
-GetModelTemplateResponseTypeDef = TypedDict(
-    "GetModelTemplateResponseTypeDef",
-    {
-        "Value": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetModelsRequestGetModelsPaginateTypeDef(
-    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
-    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetModelsRequestRequestTypeDef = TypedDict(
     "_RequiredGetModelsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetModelsRequestRequestTypeDef = TypedDict(
@@ -1237,37 +962,14 @@
     {
         "ApiId": str,
         "RouteId": str,
         "RouteResponseId": str,
     },
 )
 
-_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-    },
-)
-_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef(
-    _RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
-    _OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetRouteResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRouteResponsesRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
     },
 )
@@ -1283,36 +985,14 @@
 
 class GetRouteResponsesRequestRequestTypeDef(
     _RequiredGetRouteResponsesRequestRequestTypeDef, _OptionalGetRouteResponsesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
-    "_RequiredGetRoutesRequestGetRoutesPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
-    "_OptionalGetRoutesRequestGetRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetRoutesRequestGetRoutesPaginateTypeDef(
-    _RequiredGetRoutesRequestGetRoutesPaginateTypeDef,
-    _OptionalGetRoutesRequestGetRoutesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRoutesRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetRoutesRequestRequestTypeDef = TypedDict(
@@ -1335,36 +1015,14 @@
     "GetStageRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
 
-_RequiredGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
-    "_RequiredGetStagesRequestGetStagesPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
-    "_OptionalGetStagesRequestGetStagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetStagesRequestGetStagesPaginateTypeDef(
-    _RequiredGetStagesRequestGetStagesPaginateTypeDef,
-    _OptionalGetStagesRequestGetStagesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetStagesRequestRequestTypeDef = TypedDict(
     "_RequiredGetStagesRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetStagesRequestRequestTypeDef = TypedDict(
@@ -1386,45 +1044,21 @@
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVpcLinkRequestRequestTypeDef = TypedDict(
     "GetVpcLinkRequestRequestTypeDef",
     {
         "VpcLinkId": str,
     },
 )
 
-GetVpcLinkResponseTypeDef = TypedDict(
-    "GetVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVpcLinksRequestRequestTypeDef = TypedDict(
     "GetVpcLinksRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1474,24 +1108,14 @@
 
 class ImportApiRequestRequestTypeDef(
     _RequiredImportApiRequestRequestTypeDef, _OptionalImportApiRequestRequestTypeDef
 ):
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
 _RequiredReimportApiRequestRequestTypeDef = TypedDict(
     "_RequiredReimportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "Body": str,
     },
 )
@@ -1515,25 +1139,14 @@
     "ResetAuthorizersCacheRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
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
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
@@ -1579,25 +1192,14 @@
 
 class UpdateApiMappingRequestRequestTypeDef(
     _RequiredUpdateApiMappingRequestRequestTypeDef, _OptionalUpdateApiMappingRequestRequestTypeDef
 ):
     pass
 
 
-UpdateApiMappingResponseTypeDef = TypedDict(
-    "UpdateApiMappingResponseTypeDef",
-    {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
         "DeploymentId": str,
     },
 )
@@ -1612,27 +1214,14 @@
 
 class UpdateDeploymentRequestRequestTypeDef(
     _RequiredUpdateDeploymentRequestRequestTypeDef, _OptionalUpdateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
-UpdateDeploymentResponseTypeDef = TypedDict(
-    "UpdateDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateIntegrationResponseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIntegrationResponseRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
         "IntegrationResponseId": str,
     },
@@ -1653,27 +1242,14 @@
 class UpdateIntegrationResponseRequestRequestTypeDef(
     _RequiredUpdateIntegrationResponseRequestRequestTypeDef,
     _OptionalUpdateIntegrationResponseRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateIntegrationResponseResponseTypeDef = TypedDict(
-    "UpdateIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
@@ -1691,26 +1267,14 @@
 
 class UpdateModelRequestRequestTypeDef(
     _RequiredUpdateModelRequestRequestTypeDef, _OptionalUpdateModelRequestRequestTypeDef
 ):
     pass
 
 
-UpdateModelResponseTypeDef = TypedDict(
-    "UpdateModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVpcLinkRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVpcLinkRequestRequestTypeDef",
     {
         "VpcLinkId": str,
     },
 )
 _OptionalUpdateVpcLinkRequestRequestTypeDef = TypedDict(
@@ -1724,39 +1288,14 @@
 
 class UpdateVpcLinkRequestRequestTypeDef(
     _RequiredUpdateVpcLinkRequestRequestTypeDef, _OptionalUpdateVpcLinkRequestRequestTypeDef
 ):
     pass
 
 
-UpdateVpcLinkResponseTypeDef = TypedDict(
-    "UpdateVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetApiMappingsResponseTypeDef = TypedDict(
-    "GetApiMappingsResponseTypeDef",
-    {
-        "Items": List[ApiMappingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredApiTypeDef = TypedDict(
     "_RequiredApiTypeDef",
     {
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
     },
@@ -1782,14 +1321,116 @@
 )
 
 
 class ApiTypeDef(_RequiredApiTypeDef, _OptionalApiTypeDef):
     pass
 
 
+_RequiredAuthorizerTypeDef = TypedDict(
+    "_RequiredAuthorizerTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAuthorizerTypeDef = TypedDict(
+    "_OptionalAuthorizerTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
+    pass
+
+
+_RequiredCreateApiRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateApiRequestRequestTypeDef",
+    {
+        "Name": str,
+        "ProtocolType": ProtocolTypeType,
+    },
+)
+_OptionalCreateApiRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateApiRequestRequestTypeDef",
+    {
+        "ApiKeySelectionExpression": str,
+        "CorsConfiguration": CorsTypeDef,
+        "CredentialsArn": str,
+        "Description": str,
+        "DisableSchemaValidation": bool,
+        "DisableExecuteApiEndpoint": bool,
+        "RouteKey": str,
+        "RouteSelectionExpression": str,
+        "Tags": Mapping[str, str],
+        "Target": str,
+        "Version": str,
+    },
+    total=False,
+)
+
+
+class CreateApiRequestRequestTypeDef(
+    _RequiredCreateApiRequestRequestTypeDef, _OptionalCreateApiRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateApiRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateApiRequestRequestTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalUpdateApiRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateApiRequestRequestTypeDef",
+    {
+        "ApiKeySelectionExpression": str,
+        "CorsConfiguration": CorsTypeDef,
+        "CredentialsArn": str,
+        "Description": str,
+        "DisableSchemaValidation": bool,
+        "DisableExecuteApiEndpoint": bool,
+        "Name": str,
+        "RouteKey": str,
+        "RouteSelectionExpression": str,
+        "Target": str,
+        "Version": str,
+    },
+    total=False,
+)
+
+
+class UpdateApiRequestRequestTypeDef(
+    _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
+):
+    pass
+
+
+CreateApiMappingResponseTypeDef = TypedDict(
+    "CreateApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateApiResponseTypeDef = TypedDict(
     "CreateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
@@ -1801,15 +1442,122 @@
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthorizerResponseTypeDef = TypedDict(
+    "CreateAuthorizerResponseTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIntegrationResponseResponseTypeDef = TypedDict(
+    "CreateIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelResponseTypeDef = TypedDict(
+    "CreateModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVpcLinkResponseTypeDef = TypedDict(
+    "CreateVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
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
+ExportApiResponseTypeDef = TypedDict(
+    "ExportApiResponseTypeDef",
+    {
+        "body": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiMappingResponseTypeDef = TypedDict(
+    "GetApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiMappingsResponseTypeDef = TypedDict(
+    "GetApiMappingsResponseTypeDef",
+    {
+        "Items": List[ApiMappingTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApiResponseTypeDef = TypedDict(
     "GetApiResponseTypeDef",
     {
         "ApiEndpoint": str,
@@ -1824,15 +1572,103 @@
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAuthorizerResponseTypeDef = TypedDict(
+    "GetAuthorizerResponseTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIntegrationResponseResponseTypeDef = TypedDict(
+    "GetIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelResponseTypeDef = TypedDict(
+    "GetModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelTemplateResponseTypeDef = TypedDict(
+    "GetModelTemplateResponseTypeDef",
+    {
+        "Value": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVpcLinkResponseTypeDef = TypedDict(
+    "GetVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportApiResponseTypeDef = TypedDict(
     "ImportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
@@ -1847,15 +1683,15 @@
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReimportApiResponseTypeDef = TypedDict(
     "ReimportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
@@ -1870,15 +1706,26 @@
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApiMappingResponseTypeDef = TypedDict(
+    "UpdateApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApiResponseTypeDef = TypedDict(
     "UpdateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
@@ -1893,163 +1740,90 @@
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredAuthorizerTypeDef = TypedDict(
-    "_RequiredAuthorizerTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAuthorizerTypeDef = TypedDict(
-    "_OptionalAuthorizerTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
-    pass
-
-
-CreateAuthorizerResponseTypeDef = TypedDict(
-    "CreateAuthorizerResponseTypeDef",
+UpdateAuthorizerResponseTypeDef = TypedDict(
+    "UpdateAuthorizerResponseTypeDef",
     {
         "AuthorizerCredentialsArn": str,
         "AuthorizerId": str,
         "AuthorizerPayloadFormatVersion": str,
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerType": AuthorizerTypeType,
         "AuthorizerUri": str,
         "EnableSimpleResponses": bool,
         "IdentitySource": List[str],
         "IdentityValidationExpression": str,
         "JwtConfiguration": JWTConfigurationOutputTypeDef,
         "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAuthorizerResponseTypeDef = TypedDict(
-    "GetAuthorizerResponseTypeDef",
+UpdateDeploymentResponseTypeDef = TypedDict(
+    "UpdateDeploymentResponseTypeDef",
     {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAuthorizerResponseTypeDef = TypedDict(
-    "UpdateAuthorizerResponseTypeDef",
+UpdateIntegrationResponseResponseTypeDef = TypedDict(
+    "UpdateIntegrationResponseResponseTypeDef",
     {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateApiRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateApiRequestRequestTypeDef",
-    {
-        "Name": str,
-        "ProtocolType": ProtocolTypeType,
-    },
-)
-_OptionalCreateApiRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateApiRequestRequestTypeDef",
+UpdateModelResponseTypeDef = TypedDict(
+    "UpdateModelResponseTypeDef",
     {
-        "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
-        "CredentialsArn": str,
+        "ContentType": str,
         "Description": str,
-        "DisableSchemaValidation": bool,
-        "DisableExecuteApiEndpoint": bool,
-        "RouteKey": str,
-        "RouteSelectionExpression": str,
-        "Tags": Mapping[str, str],
-        "Target": str,
-        "Version": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateApiRequestRequestTypeDef(
-    _RequiredCreateApiRequestRequestTypeDef, _OptionalCreateApiRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateApiRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateApiRequestRequestTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalUpdateApiRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateApiRequestRequestTypeDef",
+UpdateVpcLinkResponseTypeDef = TypedDict(
+    "UpdateVpcLinkResponseTypeDef",
     {
-        "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
-        "CredentialsArn": str,
-        "Description": str,
-        "DisableSchemaValidation": bool,
-        "DisableExecuteApiEndpoint": bool,
+        "CreatedDate": datetime,
         "Name": str,
-        "RouteKey": str,
-        "RouteSelectionExpression": str,
-        "Target": str,
-        "Version": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateApiRequestRequestTypeDef(
-    _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerType": AuthorizerTypeType,
         "IdentitySource": Sequence[str],
         "Name": str,
@@ -2156,15 +1930,15 @@
     "CreateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
         "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDomainNameTypeDef = TypedDict(
     "_RequiredDomainNameTypeDef",
     {
         "DomainName": str,
@@ -2190,27 +1964,27 @@
     "GetDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
         "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainNameResponseTypeDef = TypedDict(
     "UpdateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
         "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntegrationRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2304,15 +2078,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntegrationResultTypeDef = TypedDict(
     "GetIntegrationResultTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2331,15 +2105,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2385,15 +2159,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRouteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2446,149 +2220,90 @@
 class CreateRouteResponseRequestRequestTypeDef(
     _RequiredCreateRouteResponseRequestRequestTypeDef,
     _OptionalCreateRouteResponseRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredUpdateRouteRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRouteRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-    },
-)
-_OptionalUpdateRouteRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRouteRequestRequestTypeDef",
-    {
-        "ApiKeyRequired": bool,
-        "AuthorizationScopes": Sequence[str],
-        "AuthorizationType": AuthorizationTypeType,
-        "AuthorizerId": str,
-        "ModelSelectionExpression": str,
-        "OperationName": str,
-        "RequestModels": Mapping[str, str],
-        "RequestParameters": Mapping[str, ParameterConstraintsTypeDef],
-        "RouteKey": str,
-        "RouteResponseSelectionExpression": str,
-        "Target": str,
-    },
-    total=False,
-)
-
-
-class UpdateRouteRequestRequestTypeDef(
-    _RequiredUpdateRouteRequestRequestTypeDef, _OptionalUpdateRouteRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateRouteResponseRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRouteResponseRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-        "RouteResponseId": str,
-    },
-)
-_OptionalUpdateRouteResponseRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRouteResponseRequestRequestTypeDef",
-    {
-        "ModelSelectionExpression": str,
-        "ResponseModels": Mapping[str, str],
-        "ResponseParameters": Mapping[str, ParameterConstraintsTypeDef],
-        "RouteResponseKey": str,
-    },
-    total=False,
-)
-
-
-class UpdateRouteResponseRequestRequestTypeDef(
-    _RequiredUpdateRouteResponseRequestRequestTypeDef,
-    _OptionalUpdateRouteResponseRequestRequestTypeDef,
-):
-    pass
-
-
 CreateRouteResponseResponseTypeDef = TypedDict(
     "CreateRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRouteResultTypeDef = TypedDict(
     "CreateRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponseResponseTypeDef = TypedDict(
     "GetRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResultTypeDef = TypedDict(
     "GetRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRouteResponseTypeDef = TypedDict(
     "_RequiredRouteResponseTypeDef",
     {
         "RouteResponseKey": str,
     },
 )
 _OptionalRouteResponseTypeDef = TypedDict(
     "_OptionalRouteResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
     },
     total=False,
 )
 
 
 class RouteResponseTypeDef(_RequiredRouteResponseTypeDef, _OptionalRouteResponseTypeDef):
@@ -2608,56 +2323,115 @@
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
     },
     total=False,
 )
 
 
 class RouteTypeDef(_RequiredRouteTypeDef, _OptionalRouteTypeDef):
     pass
 
 
+_RequiredUpdateRouteRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRouteRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+    },
+)
+_OptionalUpdateRouteRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRouteRequestRequestTypeDef",
+    {
+        "ApiKeyRequired": bool,
+        "AuthorizationScopes": Sequence[str],
+        "AuthorizationType": AuthorizationTypeType,
+        "AuthorizerId": str,
+        "ModelSelectionExpression": str,
+        "OperationName": str,
+        "RequestModels": Mapping[str, str],
+        "RequestParameters": Mapping[str, ParameterConstraintsTypeDef],
+        "RouteKey": str,
+        "RouteResponseSelectionExpression": str,
+        "Target": str,
+    },
+    total=False,
+)
+
+
+class UpdateRouteRequestRequestTypeDef(
+    _RequiredUpdateRouteRequestRequestTypeDef, _OptionalUpdateRouteRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateRouteResponseRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRouteResponseRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+        "RouteResponseId": str,
+    },
+)
+_OptionalUpdateRouteResponseRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRouteResponseRequestRequestTypeDef",
+    {
+        "ModelSelectionExpression": str,
+        "ResponseModels": Mapping[str, str],
+        "ResponseParameters": Mapping[str, ParameterConstraintsTypeDef],
+        "RouteResponseKey": str,
+    },
+    total=False,
+)
+
+
+class UpdateRouteResponseRequestRequestTypeDef(
+    _RequiredUpdateRouteResponseRequestRequestTypeDef,
+    _OptionalUpdateRouteResponseRequestRequestTypeDef,
+):
+    pass
+
+
 UpdateRouteResponseResponseTypeDef = TypedDict(
     "UpdateRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRouteResultTypeDef = TypedDict(
     "UpdateRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2683,228 +2457,422 @@
 
 class CreateStageRequestRequestTypeDef(
     _RequiredCreateStageRequestRequestTypeDef, _OptionalCreateStageRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateStageRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStageRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "StageName": str,
-    },
-)
-_OptionalUpdateStageRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStageRequestRequestTypeDef",
-    {
-        "AccessLogSettings": AccessLogSettingsTypeDef,
-        "AutoDeploy": bool,
-        "ClientCertificateId": str,
-        "DefaultRouteSettings": RouteSettingsTypeDef,
-        "DeploymentId": str,
-        "Description": str,
-        "RouteSettings": Mapping[str, RouteSettingsTypeDef],
-        "StageVariables": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class UpdateStageRequestRequestTypeDef(
-    _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
-):
-    pass
-
-
 CreateStageResponseTypeDef = TypedDict(
     "CreateStageResponseTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
+        "AccessLogSettings": AccessLogSettingsTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
+        "DefaultRouteSettings": RouteSettingsTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageResponseTypeDef = TypedDict(
     "GetStageResponseTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
+        "AccessLogSettings": AccessLogSettingsTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
+        "DefaultRouteSettings": RouteSettingsTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStageTypeDef = TypedDict(
     "_RequiredStageTypeDef",
     {
         "StageName": str,
     },
 )
 _OptionalStageTypeDef = TypedDict(
     "_OptionalStageTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
+        "AccessLogSettings": AccessLogSettingsTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
+        "DefaultRouteSettings": RouteSettingsTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
 
 class StageTypeDef(_RequiredStageTypeDef, _OptionalStageTypeDef):
     pass
 
 
+_RequiredUpdateStageRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStageRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "StageName": str,
+    },
+)
+_OptionalUpdateStageRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStageRequestRequestTypeDef",
+    {
+        "AccessLogSettings": AccessLogSettingsTypeDef,
+        "AutoDeploy": bool,
+        "ClientCertificateId": str,
+        "DefaultRouteSettings": RouteSettingsTypeDef,
+        "DeploymentId": str,
+        "Description": str,
+        "RouteSettings": Mapping[str, RouteSettingsTypeDef],
+        "StageVariables": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class UpdateStageRequestRequestTypeDef(
+    _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
+):
+    pass
+
+
 UpdateStageResponseTypeDef = TypedDict(
     "UpdateStageResponseTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
+        "AccessLogSettings": AccessLogSettingsTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
+        "DefaultRouteSettings": RouteSettingsTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentsResponseTypeDef = TypedDict(
     "GetDeploymentsResponseTypeDef",
     {
         "Items": List[DeploymentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApisRequestGetApisPaginateTypeDef = TypedDict(
+    "GetApisRequestGetApisPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "ApiId": str,
     },
 )
+_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
+    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
+    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+):
+    pass
+
+
+GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    {
+        "ApiId": str,
+        "IntegrationId": str,
+    },
+)
+_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef(
+    _RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    _OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
+    "_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
+    "_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetIntegrationsRequestGetIntegrationsPaginateTypeDef(
+    _RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    _OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetModelsRequestGetModelsPaginateTypeDef(
+    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
+    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+    },
+)
+_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef(
+    _RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    _OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
+    "_RequiredGetRoutesRequestGetRoutesPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
+    "_OptionalGetRoutesRequestGetRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetRoutesRequestGetRoutesPaginateTypeDef(
+    _RequiredGetRoutesRequestGetRoutesPaginateTypeDef,
+    _OptionalGetRoutesRequestGetRoutesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
+    "_RequiredGetStagesRequestGetStagesPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
+    "_OptionalGetStagesRequestGetStagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetStagesRequestGetStagesPaginateTypeDef(
+    _RequiredGetStagesRequestGetStagesPaginateTypeDef,
+    _OptionalGetStagesRequestGetStagesPaginateTypeDef,
+):
+    pass
+
 
 GetIntegrationResponsesResponseTypeDef = TypedDict(
     "GetIntegrationResponsesResponseTypeDef",
     {
         "Items": List[IntegrationResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetModelsResponseTypeDef = TypedDict(
     "GetModelsResponseTypeDef",
     {
         "Items": List[ModelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVpcLinksResponseTypeDef = TypedDict(
     "GetVpcLinksResponseTypeDef",
     {
         "Items": List[VpcLinkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApisResponseTypeDef = TypedDict(
     "GetApisResponseTypeDef",
     {
         "Items": List[ApiTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAuthorizersResponseTypeDef = TypedDict(
     "GetAuthorizersResponseTypeDef",
     {
         "Items": List[AuthorizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainNamesResponseTypeDef = TypedDict(
     "GetDomainNamesResponseTypeDef",
     {
         "Items": List[DomainNameTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntegrationsResponseTypeDef = TypedDict(
     "GetIntegrationsResponseTypeDef",
     {
         "Items": List[IntegrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponsesResponseTypeDef = TypedDict(
     "GetRouteResponsesResponseTypeDef",
     {
         "Items": List[RouteResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoutesResponseTypeDef = TypedDict(
     "GetRoutesResponseTypeDef",
     {
         "Items": List[RouteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStagesResponseTypeDef = TypedDict(
     "GetStagesResponseTypeDef",
     {
         "Items": List[StageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2/type_defs.pyi` & `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for apigatewayv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_apigatewayv2.type_defs import AccessLogSettingsOutputTypeDef
+    from mypy_boto3_apigatewayv2.type_defs import AccessLogSettingsTypeDef
 
-    data: AccessLogSettingsOutputTypeDef = {...}
+    data: AccessLogSettingsTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -40,41 +40,34 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AccessLogSettingsOutputTypeDef",
     "AccessLogSettingsTypeDef",
     "ApiMappingTypeDef",
     "CorsOutputTypeDef",
     "JWTConfigurationOutputTypeDef",
     "CorsTypeDef",
     "CreateApiMappingRequestRequestTypeDef",
-    "CreateApiMappingResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "JWTConfigurationTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "CreateDeploymentResponseTypeDef",
     "DomainNameConfigurationTypeDef",
     "MutualTlsAuthenticationInputTypeDef",
     "DomainNameConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "TlsConfigInputTypeDef",
     "CreateIntegrationResponseRequestRequestTypeDef",
-    "CreateIntegrationResponseResponseTypeDef",
     "TlsConfigTypeDef",
     "CreateModelRequestRequestTypeDef",
-    "CreateModelResponseTypeDef",
     "ParameterConstraintsTypeDef",
-    "ParameterConstraintsOutputTypeDef",
     "RouteSettingsTypeDef",
-    "RouteSettingsOutputTypeDef",
     "CreateVpcLinkRequestRequestTypeDef",
-    "CreateVpcLinkResponseTypeDef",
     "DeleteAccessLogSettingsRequestRequestTypeDef",
     "DeleteApiMappingRequestRequestTypeDef",
     "DeleteApiRequestRequestTypeDef",
     "DeleteAuthorizerRequestRequestTypeDef",
     "DeleteCorsConfigurationRequestRequestTypeDef",
     "DeleteDeploymentRequestRequestTypeDef",
     "DeleteDomainNameRequestRequestTypeDef",
@@ -84,93 +77,87 @@
     "DeleteRouteRequestParameterRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
     "DeleteRouteResponseRequestRequestTypeDef",
     "DeleteRouteSettingsRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeleteVpcLinkRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportApiRequestRequestTypeDef",
-    "ExportApiResponseTypeDef",
     "GetApiMappingRequestRequestTypeDef",
-    "GetApiMappingResponseTypeDef",
     "GetApiMappingsRequestRequestTypeDef",
     "GetApiRequestRequestTypeDef",
-    "GetApisRequestGetApisPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetApisRequestRequestTypeDef",
     "GetAuthorizerRequestRequestTypeDef",
-    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
     "GetAuthorizersRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
-    "GetDeploymentResponseTypeDef",
-    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDomainNameRequestRequestTypeDef",
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
     "GetDomainNamesRequestRequestTypeDef",
     "GetIntegrationRequestRequestTypeDef",
     "GetIntegrationResponseRequestRequestTypeDef",
-    "GetIntegrationResponseResponseTypeDef",
-    "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
     "GetIntegrationResponsesRequestRequestTypeDef",
     "IntegrationResponseTypeDef",
-    "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
     "GetIntegrationsRequestRequestTypeDef",
     "GetModelRequestRequestTypeDef",
-    "GetModelResponseTypeDef",
     "GetModelTemplateRequestRequestTypeDef",
-    "GetModelTemplateResponseTypeDef",
-    "GetModelsRequestGetModelsPaginateTypeDef",
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetRouteRequestRequestTypeDef",
     "GetRouteResponseRequestRequestTypeDef",
-    "GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
     "GetRouteResponsesRequestRequestTypeDef",
-    "GetRoutesRequestGetRoutesPaginateTypeDef",
     "GetRoutesRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
-    "GetStagesRequestGetStagesPaginateTypeDef",
     "GetStagesRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
-    "GetTagsResponseTypeDef",
     "GetVpcLinkRequestRequestTypeDef",
-    "GetVpcLinkResponseTypeDef",
     "GetVpcLinksRequestRequestTypeDef",
     "VpcLinkTypeDef",
     "ImportApiRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ReimportApiRequestRequestTypeDef",
     "ResetAuthorizersCacheRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiMappingRequestRequestTypeDef",
-    "UpdateApiMappingResponseTypeDef",
     "UpdateDeploymentRequestRequestTypeDef",
-    "UpdateDeploymentResponseTypeDef",
     "UpdateIntegrationResponseRequestRequestTypeDef",
-    "UpdateIntegrationResponseResponseTypeDef",
     "UpdateModelRequestRequestTypeDef",
-    "UpdateModelResponseTypeDef",
     "UpdateVpcLinkRequestRequestTypeDef",
-    "UpdateVpcLinkResponseTypeDef",
-    "GetApiMappingsResponseTypeDef",
     "ApiTypeDef",
+    "AuthorizerTypeDef",
+    "CreateApiRequestRequestTypeDef",
+    "UpdateApiRequestRequestTypeDef",
+    "CreateApiMappingResponseTypeDef",
     "CreateApiResponseTypeDef",
+    "CreateAuthorizerResponseTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "CreateIntegrationResponseResponseTypeDef",
+    "CreateModelResponseTypeDef",
+    "CreateVpcLinkResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportApiResponseTypeDef",
+    "GetApiMappingResponseTypeDef",
+    "GetApiMappingsResponseTypeDef",
     "GetApiResponseTypeDef",
+    "GetAuthorizerResponseTypeDef",
+    "GetDeploymentResponseTypeDef",
+    "GetIntegrationResponseResponseTypeDef",
+    "GetModelResponseTypeDef",
+    "GetModelTemplateResponseTypeDef",
+    "GetTagsResponseTypeDef",
+    "GetVpcLinkResponseTypeDef",
     "ImportApiResponseTypeDef",
     "ReimportApiResponseTypeDef",
+    "UpdateApiMappingResponseTypeDef",
     "UpdateApiResponseTypeDef",
-    "AuthorizerTypeDef",
-    "CreateAuthorizerResponseTypeDef",
-    "GetAuthorizerResponseTypeDef",
     "UpdateAuthorizerResponseTypeDef",
-    "CreateApiRequestRequestTypeDef",
-    "UpdateApiRequestRequestTypeDef",
+    "UpdateDeploymentResponseTypeDef",
+    "UpdateIntegrationResponseResponseTypeDef",
+    "UpdateModelResponseTypeDef",
+    "UpdateVpcLinkResponseTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
     "CreateDomainNameRequestRequestTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
     "CreateDomainNameResponseTypeDef",
     "DomainNameTypeDef",
     "GetDomainNameResponseTypeDef",
@@ -179,52 +166,53 @@
     "UpdateIntegrationRequestRequestTypeDef",
     "CreateIntegrationResultTypeDef",
     "GetIntegrationResultTypeDef",
     "IntegrationTypeDef",
     "UpdateIntegrationResultTypeDef",
     "CreateRouteRequestRequestTypeDef",
     "CreateRouteResponseRequestRequestTypeDef",
-    "UpdateRouteRequestRequestTypeDef",
-    "UpdateRouteResponseRequestRequestTypeDef",
     "CreateRouteResponseResponseTypeDef",
     "CreateRouteResultTypeDef",
     "GetRouteResponseResponseTypeDef",
     "GetRouteResultTypeDef",
     "RouteResponseTypeDef",
     "RouteTypeDef",
+    "UpdateRouteRequestRequestTypeDef",
+    "UpdateRouteResponseRequestRequestTypeDef",
     "UpdateRouteResponseResponseTypeDef",
     "UpdateRouteResultTypeDef",
     "CreateStageRequestRequestTypeDef",
-    "UpdateStageRequestRequestTypeDef",
     "CreateStageResponseTypeDef",
     "GetStageResponseTypeDef",
     "StageTypeDef",
+    "UpdateStageRequestRequestTypeDef",
     "UpdateStageResponseTypeDef",
     "GetDeploymentsResponseTypeDef",
+    "GetApisRequestGetApisPaginateTypeDef",
+    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
+    "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    "GetModelsRequestGetModelsPaginateTypeDef",
+    "GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    "GetRoutesRequestGetRoutesPaginateTypeDef",
+    "GetStagesRequestGetStagesPaginateTypeDef",
     "GetIntegrationResponsesResponseTypeDef",
     "GetModelsResponseTypeDef",
     "GetVpcLinksResponseTypeDef",
     "GetApisResponseTypeDef",
     "GetAuthorizersResponseTypeDef",
     "GetDomainNamesResponseTypeDef",
     "GetIntegrationsResponseTypeDef",
     "GetRouteResponsesResponseTypeDef",
     "GetRoutesResponseTypeDef",
     "GetStagesResponseTypeDef",
 )
 
-AccessLogSettingsOutputTypeDef = TypedDict(
-    "AccessLogSettingsOutputTypeDef",
-    {
-        "DestinationArn": str,
-        "Format": str,
-    },
-    total=False,
-)
-
 AccessLogSettingsTypeDef = TypedDict(
     "AccessLogSettingsTypeDef",
     {
         "DestinationArn": str,
         "Format": str,
     },
     total=False,
@@ -301,22 +289,22 @@
 )
 
 class CreateApiMappingRequestRequestTypeDef(
     _RequiredCreateApiMappingRequestRequestTypeDef, _OptionalCreateApiMappingRequestRequestTypeDef
 ):
     pass
 
-CreateApiMappingResponseTypeDef = TypedDict(
-    "CreateApiMappingResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 JWTConfigurationTypeDef = TypedDict(
     "JWTConfigurationTypeDef",
     {
         "Audience": Sequence[str],
@@ -341,27 +329,14 @@
 )
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DomainNameConfigurationTypeDef = TypedDict(
     "DomainNameConfigurationTypeDef",
     {
         "ApiGatewayDomainName": str,
         "CertificateArn": str,
         "CertificateName": str,
         "CertificateUploadDate": Union[datetime, str],
@@ -440,27 +415,14 @@
 
 class CreateIntegrationResponseRequestRequestTypeDef(
     _RequiredCreateIntegrationResponseRequestRequestTypeDef,
     _OptionalCreateIntegrationResponseRequestRequestTypeDef,
 ):
     pass
 
-CreateIntegrationResponseResponseTypeDef = TypedDict(
-    "CreateIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TlsConfigTypeDef = TypedDict(
     "TlsConfigTypeDef",
     {
         "ServerNameToVerify": str,
     },
     total=False,
 )
@@ -483,66 +445,34 @@
 )
 
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
-CreateModelResponseTypeDef = TypedDict(
-    "CreateModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "Required": bool,
     },
     total=False,
 )
 
-ParameterConstraintsOutputTypeDef = TypedDict(
-    "ParameterConstraintsOutputTypeDef",
-    {
-        "Required": bool,
-    },
-    total=False,
-)
-
 RouteSettingsTypeDef = TypedDict(
     "RouteSettingsTypeDef",
     {
         "DataTraceEnabled": bool,
         "DetailedMetricsEnabled": bool,
         "LoggingLevel": LoggingLevelType,
         "ThrottlingBurstLimit": int,
         "ThrottlingRateLimit": float,
     },
     total=False,
 )
 
-RouteSettingsOutputTypeDef = TypedDict(
-    "RouteSettingsOutputTypeDef",
-    {
-        "DataTraceEnabled": bool,
-        "DetailedMetricsEnabled": bool,
-        "LoggingLevel": LoggingLevelType,
-        "ThrottlingBurstLimit": int,
-        "ThrottlingRateLimit": float,
-    },
-    total=False,
-)
-
 _RequiredCreateVpcLinkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcLinkRequestRequestTypeDef",
     {
         "Name": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -556,30 +486,14 @@
 )
 
 class CreateVpcLinkRequestRequestTypeDef(
     _RequiredCreateVpcLinkRequestRequestTypeDef, _OptionalCreateVpcLinkRequestRequestTypeDef
 ):
     pass
 
-CreateVpcLinkResponseTypeDef = TypedDict(
-    "CreateVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccessLogSettingsRequestRequestTypeDef = TypedDict(
     "DeleteAccessLogSettingsRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
@@ -713,21 +627,14 @@
         "DeploymentStatus": DeploymentStatusType,
         "DeploymentStatusMessage": str,
         "Description": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExportApiRequestRequestTypeDef = TypedDict(
     "_RequiredExportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "OutputType": JSONYAMLType,
         "Specification": Literal["OAS30"],
     },
@@ -743,41 +650,22 @@
 )
 
 class ExportApiRequestRequestTypeDef(
     _RequiredExportApiRequestRequestTypeDef, _OptionalExportApiRequestRequestTypeDef
 ):
     pass
 
-ExportApiResponseTypeDef = TypedDict(
-    "ExportApiResponseTypeDef",
-    {
-        "body": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApiMappingRequestRequestTypeDef = TypedDict(
     "GetApiMappingRequestRequestTypeDef",
     {
         "ApiMappingId": str,
         "DomainName": str,
     },
 )
 
-GetApiMappingResponseTypeDef = TypedDict(
-    "GetApiMappingResponseTypeDef",
-    {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetApiMappingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetApiMappingsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetApiMappingsRequestRequestTypeDef = TypedDict(
@@ -797,18 +685,20 @@
 GetApiRequestRequestTypeDef = TypedDict(
     "GetApiRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 
-GetApisRequestGetApisPaginateTypeDef = TypedDict(
-    "GetApisRequestGetApisPaginateTypeDef",
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
 
 GetApisRequestRequestTypeDef = TypedDict(
     "GetApisRequestRequestTypeDef",
     {
@@ -822,34 +712,14 @@
     "GetAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerId": str,
     },
 )
 
-_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
-    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-):
-    pass
-
 _RequiredGetAuthorizersRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizersRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetAuthorizersRequestRequestTypeDef = TypedDict(
@@ -870,47 +740,14 @@
     "GetDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
         "DeploymentId": str,
     },
 )
 
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
-    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeploymentsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetDeploymentsRequestRequestTypeDef = TypedDict(
@@ -930,22 +767,14 @@
 GetDomainNameRequestRequestTypeDef = TypedDict(
     "GetDomainNameRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetDomainNamesRequestRequestTypeDef = TypedDict(
     "GetDomainNamesRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -964,48 +793,14 @@
     {
         "ApiId": str,
         "IntegrationId": str,
         "IntegrationResponseId": str,
     },
 )
 
-GetIntegrationResponseResponseTypeDef = TypedDict(
-    "GetIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
-    {
-        "ApiId": str,
-        "IntegrationId": str,
-    },
-)
-_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef(
-    _RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
-    _OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetIntegrationResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntegrationResponsesRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
     },
 )
@@ -1043,34 +838,14 @@
 )
 
 class IntegrationResponseTypeDef(
     _RequiredIntegrationResponseTypeDef, _OptionalIntegrationResponseTypeDef
 ):
     pass
 
-_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
-    "_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
-    "_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetIntegrationsRequestGetIntegrationsPaginateTypeDef(
-    _RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
-    _OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetIntegrationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntegrationsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetIntegrationsRequestRequestTypeDef = TypedDict(
@@ -1091,62 +866,22 @@
     "GetModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
 
-GetModelResponseTypeDef = TypedDict(
-    "GetModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetModelTemplateRequestRequestTypeDef = TypedDict(
     "GetModelTemplateRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
 
-GetModelTemplateResponseTypeDef = TypedDict(
-    "GetModelTemplateResponseTypeDef",
-    {
-        "Value": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetModelsRequestGetModelsPaginateTypeDef(
-    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
-    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetModelsRequestRequestTypeDef = TypedDict(
     "_RequiredGetModelsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetModelsRequestRequestTypeDef = TypedDict(
@@ -1196,35 +931,14 @@
     {
         "ApiId": str,
         "RouteId": str,
         "RouteResponseId": str,
     },
 )
 
-_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-    },
-)
-_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef(
-    _RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
-    _OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetRouteResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRouteResponsesRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
     },
 )
@@ -1238,34 +952,14 @@
 )
 
 class GetRouteResponsesRequestRequestTypeDef(
     _RequiredGetRouteResponsesRequestRequestTypeDef, _OptionalGetRouteResponsesRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
-    "_RequiredGetRoutesRequestGetRoutesPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
-    "_OptionalGetRoutesRequestGetRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetRoutesRequestGetRoutesPaginateTypeDef(
-    _RequiredGetRoutesRequestGetRoutesPaginateTypeDef,
-    _OptionalGetRoutesRequestGetRoutesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRoutesRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetRoutesRequestRequestTypeDef = TypedDict(
@@ -1286,34 +980,14 @@
     "GetStageRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
 
-_RequiredGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
-    "_RequiredGetStagesRequestGetStagesPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
-    "_OptionalGetStagesRequestGetStagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetStagesRequestGetStagesPaginateTypeDef(
-    _RequiredGetStagesRequestGetStagesPaginateTypeDef,
-    _OptionalGetStagesRequestGetStagesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetStagesRequestRequestTypeDef = TypedDict(
     "_RequiredGetStagesRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetStagesRequestRequestTypeDef = TypedDict(
@@ -1333,45 +1007,21 @@
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVpcLinkRequestRequestTypeDef = TypedDict(
     "GetVpcLinkRequestRequestTypeDef",
     {
         "VpcLinkId": str,
     },
 )
 
-GetVpcLinkResponseTypeDef = TypedDict(
-    "GetVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVpcLinksRequestRequestTypeDef = TypedDict(
     "GetVpcLinksRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1417,24 +1067,14 @@
 )
 
 class ImportApiRequestRequestTypeDef(
     _RequiredImportApiRequestRequestTypeDef, _OptionalImportApiRequestRequestTypeDef
 ):
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
 _RequiredReimportApiRequestRequestTypeDef = TypedDict(
     "_RequiredReimportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "Body": str,
     },
 )
@@ -1456,25 +1096,14 @@
     "ResetAuthorizersCacheRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
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
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
@@ -1516,25 +1145,14 @@
 )
 
 class UpdateApiMappingRequestRequestTypeDef(
     _RequiredUpdateApiMappingRequestRequestTypeDef, _OptionalUpdateApiMappingRequestRequestTypeDef
 ):
     pass
 
-UpdateApiMappingResponseTypeDef = TypedDict(
-    "UpdateApiMappingResponseTypeDef",
-    {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
         "DeploymentId": str,
     },
 )
@@ -1547,27 +1165,14 @@
 )
 
 class UpdateDeploymentRequestRequestTypeDef(
     _RequiredUpdateDeploymentRequestRequestTypeDef, _OptionalUpdateDeploymentRequestRequestTypeDef
 ):
     pass
 
-UpdateDeploymentResponseTypeDef = TypedDict(
-    "UpdateDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateIntegrationResponseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIntegrationResponseRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
         "IntegrationResponseId": str,
     },
@@ -1586,27 +1191,14 @@
 
 class UpdateIntegrationResponseRequestRequestTypeDef(
     _RequiredUpdateIntegrationResponseRequestRequestTypeDef,
     _OptionalUpdateIntegrationResponseRequestRequestTypeDef,
 ):
     pass
 
-UpdateIntegrationResponseResponseTypeDef = TypedDict(
-    "UpdateIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
@@ -1622,26 +1214,14 @@
 )
 
 class UpdateModelRequestRequestTypeDef(
     _RequiredUpdateModelRequestRequestTypeDef, _OptionalUpdateModelRequestRequestTypeDef
 ):
     pass
 
-UpdateModelResponseTypeDef = TypedDict(
-    "UpdateModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVpcLinkRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVpcLinkRequestRequestTypeDef",
     {
         "VpcLinkId": str,
     },
 )
 _OptionalUpdateVpcLinkRequestRequestTypeDef = TypedDict(
@@ -1653,39 +1233,14 @@
 )
 
 class UpdateVpcLinkRequestRequestTypeDef(
     _RequiredUpdateVpcLinkRequestRequestTypeDef, _OptionalUpdateVpcLinkRequestRequestTypeDef
 ):
     pass
 
-UpdateVpcLinkResponseTypeDef = TypedDict(
-    "UpdateVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetApiMappingsResponseTypeDef = TypedDict(
-    "GetApiMappingsResponseTypeDef",
-    {
-        "Items": List[ApiMappingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredApiTypeDef = TypedDict(
     "_RequiredApiTypeDef",
     {
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
     },
@@ -1709,14 +1264,110 @@
     },
     total=False,
 )
 
 class ApiTypeDef(_RequiredApiTypeDef, _OptionalApiTypeDef):
     pass
 
+_RequiredAuthorizerTypeDef = TypedDict(
+    "_RequiredAuthorizerTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAuthorizerTypeDef = TypedDict(
+    "_OptionalAuthorizerTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
+    pass
+
+_RequiredCreateApiRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateApiRequestRequestTypeDef",
+    {
+        "Name": str,
+        "ProtocolType": ProtocolTypeType,
+    },
+)
+_OptionalCreateApiRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateApiRequestRequestTypeDef",
+    {
+        "ApiKeySelectionExpression": str,
+        "CorsConfiguration": CorsTypeDef,
+        "CredentialsArn": str,
+        "Description": str,
+        "DisableSchemaValidation": bool,
+        "DisableExecuteApiEndpoint": bool,
+        "RouteKey": str,
+        "RouteSelectionExpression": str,
+        "Tags": Mapping[str, str],
+        "Target": str,
+        "Version": str,
+    },
+    total=False,
+)
+
+class CreateApiRequestRequestTypeDef(
+    _RequiredCreateApiRequestRequestTypeDef, _OptionalCreateApiRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateApiRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateApiRequestRequestTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalUpdateApiRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateApiRequestRequestTypeDef",
+    {
+        "ApiKeySelectionExpression": str,
+        "CorsConfiguration": CorsTypeDef,
+        "CredentialsArn": str,
+        "Description": str,
+        "DisableSchemaValidation": bool,
+        "DisableExecuteApiEndpoint": bool,
+        "Name": str,
+        "RouteKey": str,
+        "RouteSelectionExpression": str,
+        "Target": str,
+        "Version": str,
+    },
+    total=False,
+)
+
+class UpdateApiRequestRequestTypeDef(
+    _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
+):
+    pass
+
+CreateApiMappingResponseTypeDef = TypedDict(
+    "CreateApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateApiResponseTypeDef = TypedDict(
     "CreateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
@@ -1728,15 +1379,122 @@
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthorizerResponseTypeDef = TypedDict(
+    "CreateAuthorizerResponseTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIntegrationResponseResponseTypeDef = TypedDict(
+    "CreateIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelResponseTypeDef = TypedDict(
+    "CreateModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVpcLinkResponseTypeDef = TypedDict(
+    "CreateVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
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
+ExportApiResponseTypeDef = TypedDict(
+    "ExportApiResponseTypeDef",
+    {
+        "body": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiMappingResponseTypeDef = TypedDict(
+    "GetApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiMappingsResponseTypeDef = TypedDict(
+    "GetApiMappingsResponseTypeDef",
+    {
+        "Items": List[ApiMappingTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApiResponseTypeDef = TypedDict(
     "GetApiResponseTypeDef",
     {
         "ApiEndpoint": str,
@@ -1751,15 +1509,103 @@
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAuthorizerResponseTypeDef = TypedDict(
+    "GetAuthorizerResponseTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIntegrationResponseResponseTypeDef = TypedDict(
+    "GetIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelResponseTypeDef = TypedDict(
+    "GetModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelTemplateResponseTypeDef = TypedDict(
+    "GetModelTemplateResponseTypeDef",
+    {
+        "Value": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVpcLinkResponseTypeDef = TypedDict(
+    "GetVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportApiResponseTypeDef = TypedDict(
     "ImportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
@@ -1774,15 +1620,15 @@
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReimportApiResponseTypeDef = TypedDict(
     "ReimportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
@@ -1797,15 +1643,26 @@
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApiMappingResponseTypeDef = TypedDict(
+    "UpdateApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApiResponseTypeDef = TypedDict(
     "UpdateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
@@ -1820,157 +1677,90 @@
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredAuthorizerTypeDef = TypedDict(
-    "_RequiredAuthorizerTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAuthorizerTypeDef = TypedDict(
-    "_OptionalAuthorizerTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
-    pass
-
-CreateAuthorizerResponseTypeDef = TypedDict(
-    "CreateAuthorizerResponseTypeDef",
+UpdateAuthorizerResponseTypeDef = TypedDict(
+    "UpdateAuthorizerResponseTypeDef",
     {
         "AuthorizerCredentialsArn": str,
         "AuthorizerId": str,
         "AuthorizerPayloadFormatVersion": str,
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerType": AuthorizerTypeType,
         "AuthorizerUri": str,
         "EnableSimpleResponses": bool,
         "IdentitySource": List[str],
         "IdentityValidationExpression": str,
         "JwtConfiguration": JWTConfigurationOutputTypeDef,
         "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAuthorizerResponseTypeDef = TypedDict(
-    "GetAuthorizerResponseTypeDef",
+UpdateDeploymentResponseTypeDef = TypedDict(
+    "UpdateDeploymentResponseTypeDef",
     {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAuthorizerResponseTypeDef = TypedDict(
-    "UpdateAuthorizerResponseTypeDef",
+UpdateIntegrationResponseResponseTypeDef = TypedDict(
+    "UpdateIntegrationResponseResponseTypeDef",
     {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateApiRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateApiRequestRequestTypeDef",
-    {
-        "Name": str,
-        "ProtocolType": ProtocolTypeType,
-    },
-)
-_OptionalCreateApiRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateApiRequestRequestTypeDef",
+UpdateModelResponseTypeDef = TypedDict(
+    "UpdateModelResponseTypeDef",
     {
-        "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
-        "CredentialsArn": str,
+        "ContentType": str,
         "Description": str,
-        "DisableSchemaValidation": bool,
-        "DisableExecuteApiEndpoint": bool,
-        "RouteKey": str,
-        "RouteSelectionExpression": str,
-        "Tags": Mapping[str, str],
-        "Target": str,
-        "Version": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateApiRequestRequestTypeDef(
-    _RequiredCreateApiRequestRequestTypeDef, _OptionalCreateApiRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateApiRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateApiRequestRequestTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalUpdateApiRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateApiRequestRequestTypeDef",
+UpdateVpcLinkResponseTypeDef = TypedDict(
+    "UpdateVpcLinkResponseTypeDef",
     {
-        "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
-        "CredentialsArn": str,
-        "Description": str,
-        "DisableSchemaValidation": bool,
-        "DisableExecuteApiEndpoint": bool,
+        "CreatedDate": datetime,
         "Name": str,
-        "RouteKey": str,
-        "RouteSelectionExpression": str,
-        "Target": str,
-        "Version": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateApiRequestRequestTypeDef(
-    _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
-):
-    pass
-
 _RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerType": AuthorizerTypeType,
         "IdentitySource": Sequence[str],
         "Name": str,
@@ -2069,15 +1859,15 @@
     "CreateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
         "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDomainNameTypeDef = TypedDict(
     "_RequiredDomainNameTypeDef",
     {
         "DomainName": str,
@@ -2101,27 +1891,27 @@
     "GetDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
         "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainNameResponseTypeDef = TypedDict(
     "UpdateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
         "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntegrationRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2211,15 +2001,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntegrationResultTypeDef = TypedDict(
     "GetIntegrationResultTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2238,15 +2028,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2292,15 +2082,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRouteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2349,145 +2139,90 @@
 
 class CreateRouteResponseRequestRequestTypeDef(
     _RequiredCreateRouteResponseRequestRequestTypeDef,
     _OptionalCreateRouteResponseRequestRequestTypeDef,
 ):
     pass
 
-_RequiredUpdateRouteRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRouteRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-    },
-)
-_OptionalUpdateRouteRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRouteRequestRequestTypeDef",
-    {
-        "ApiKeyRequired": bool,
-        "AuthorizationScopes": Sequence[str],
-        "AuthorizationType": AuthorizationTypeType,
-        "AuthorizerId": str,
-        "ModelSelectionExpression": str,
-        "OperationName": str,
-        "RequestModels": Mapping[str, str],
-        "RequestParameters": Mapping[str, ParameterConstraintsTypeDef],
-        "RouteKey": str,
-        "RouteResponseSelectionExpression": str,
-        "Target": str,
-    },
-    total=False,
-)
-
-class UpdateRouteRequestRequestTypeDef(
-    _RequiredUpdateRouteRequestRequestTypeDef, _OptionalUpdateRouteRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateRouteResponseRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRouteResponseRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-        "RouteResponseId": str,
-    },
-)
-_OptionalUpdateRouteResponseRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRouteResponseRequestRequestTypeDef",
-    {
-        "ModelSelectionExpression": str,
-        "ResponseModels": Mapping[str, str],
-        "ResponseParameters": Mapping[str, ParameterConstraintsTypeDef],
-        "RouteResponseKey": str,
-    },
-    total=False,
-)
-
-class UpdateRouteResponseRequestRequestTypeDef(
-    _RequiredUpdateRouteResponseRequestRequestTypeDef,
-    _OptionalUpdateRouteResponseRequestRequestTypeDef,
-):
-    pass
-
 CreateRouteResponseResponseTypeDef = TypedDict(
     "CreateRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRouteResultTypeDef = TypedDict(
     "CreateRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponseResponseTypeDef = TypedDict(
     "GetRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResultTypeDef = TypedDict(
     "GetRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRouteResponseTypeDef = TypedDict(
     "_RequiredRouteResponseTypeDef",
     {
         "RouteResponseKey": str,
     },
 )
 _OptionalRouteResponseTypeDef = TypedDict(
     "_OptionalRouteResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
     },
     total=False,
 )
 
 class RouteResponseTypeDef(_RequiredRouteResponseTypeDef, _OptionalRouteResponseTypeDef):
     pass
@@ -2505,54 +2240,109 @@
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
     },
     total=False,
 )
 
 class RouteTypeDef(_RequiredRouteTypeDef, _OptionalRouteTypeDef):
     pass
 
+_RequiredUpdateRouteRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRouteRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+    },
+)
+_OptionalUpdateRouteRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRouteRequestRequestTypeDef",
+    {
+        "ApiKeyRequired": bool,
+        "AuthorizationScopes": Sequence[str],
+        "AuthorizationType": AuthorizationTypeType,
+        "AuthorizerId": str,
+        "ModelSelectionExpression": str,
+        "OperationName": str,
+        "RequestModels": Mapping[str, str],
+        "RequestParameters": Mapping[str, ParameterConstraintsTypeDef],
+        "RouteKey": str,
+        "RouteResponseSelectionExpression": str,
+        "Target": str,
+    },
+    total=False,
+)
+
+class UpdateRouteRequestRequestTypeDef(
+    _RequiredUpdateRouteRequestRequestTypeDef, _OptionalUpdateRouteRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateRouteResponseRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRouteResponseRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+        "RouteResponseId": str,
+    },
+)
+_OptionalUpdateRouteResponseRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRouteResponseRequestRequestTypeDef",
+    {
+        "ModelSelectionExpression": str,
+        "ResponseModels": Mapping[str, str],
+        "ResponseParameters": Mapping[str, ParameterConstraintsTypeDef],
+        "RouteResponseKey": str,
+    },
+    total=False,
+)
+
+class UpdateRouteResponseRequestRequestTypeDef(
+    _RequiredUpdateRouteResponseRequestRequestTypeDef,
+    _OptionalUpdateRouteResponseRequestRequestTypeDef,
+):
+    pass
+
 UpdateRouteResponseResponseTypeDef = TypedDict(
     "UpdateRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
-        "ResponseParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRouteResultTypeDef = TypedDict(
     "UpdateRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ApiKeyRequired": bool,
         "AuthorizationScopes": List[str],
         "AuthorizationType": AuthorizationTypeType,
         "AuthorizerId": str,
         "ModelSelectionExpression": str,
         "OperationName": str,
         "RequestModels": Dict[str, str],
-        "RequestParameters": Dict[str, ParameterConstraintsOutputTypeDef],
+        "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2576,224 +2366,402 @@
 )
 
 class CreateStageRequestRequestTypeDef(
     _RequiredCreateStageRequestRequestTypeDef, _OptionalCreateStageRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateStageRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStageRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "StageName": str,
-    },
-)
-_OptionalUpdateStageRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStageRequestRequestTypeDef",
-    {
-        "AccessLogSettings": AccessLogSettingsTypeDef,
-        "AutoDeploy": bool,
-        "ClientCertificateId": str,
-        "DefaultRouteSettings": RouteSettingsTypeDef,
-        "DeploymentId": str,
-        "Description": str,
-        "RouteSettings": Mapping[str, RouteSettingsTypeDef],
-        "StageVariables": Mapping[str, str],
-    },
-    total=False,
-)
-
-class UpdateStageRequestRequestTypeDef(
-    _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
-):
-    pass
-
 CreateStageResponseTypeDef = TypedDict(
     "CreateStageResponseTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
+        "AccessLogSettings": AccessLogSettingsTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
+        "DefaultRouteSettings": RouteSettingsTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageResponseTypeDef = TypedDict(
     "GetStageResponseTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
+        "AccessLogSettings": AccessLogSettingsTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
+        "DefaultRouteSettings": RouteSettingsTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStageTypeDef = TypedDict(
     "_RequiredStageTypeDef",
     {
         "StageName": str,
     },
 )
 _OptionalStageTypeDef = TypedDict(
     "_OptionalStageTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
+        "AccessLogSettings": AccessLogSettingsTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
+        "DefaultRouteSettings": RouteSettingsTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
 class StageTypeDef(_RequiredStageTypeDef, _OptionalStageTypeDef):
     pass
 
+_RequiredUpdateStageRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStageRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "StageName": str,
+    },
+)
+_OptionalUpdateStageRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStageRequestRequestTypeDef",
+    {
+        "AccessLogSettings": AccessLogSettingsTypeDef,
+        "AutoDeploy": bool,
+        "ClientCertificateId": str,
+        "DefaultRouteSettings": RouteSettingsTypeDef,
+        "DeploymentId": str,
+        "Description": str,
+        "RouteSettings": Mapping[str, RouteSettingsTypeDef],
+        "StageVariables": Mapping[str, str],
+    },
+    total=False,
+)
+
+class UpdateStageRequestRequestTypeDef(
+    _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
+):
+    pass
+
 UpdateStageResponseTypeDef = TypedDict(
     "UpdateStageResponseTypeDef",
     {
-        "AccessLogSettings": AccessLogSettingsOutputTypeDef,
+        "AccessLogSettings": AccessLogSettingsTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
         "CreatedDate": datetime,
-        "DefaultRouteSettings": RouteSettingsOutputTypeDef,
+        "DefaultRouteSettings": RouteSettingsTypeDef,
         "DeploymentId": str,
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
-        "RouteSettings": Dict[str, RouteSettingsOutputTypeDef],
+        "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentsResponseTypeDef = TypedDict(
     "GetDeploymentsResponseTypeDef",
     {
         "Items": List[DeploymentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetApisRequestGetApisPaginateTypeDef = TypedDict(
+    "GetApisRequestGetApisPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
+    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+):
+    pass
+
+_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
+    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+):
+    pass
+
+GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    {
+        "ApiId": str,
+        "IntegrationId": str,
+    },
+)
+_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef(
+    _RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    _OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+):
+    pass
+
+_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
+    "_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
+    "_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetIntegrationsRequestGetIntegrationsPaginateTypeDef(
+    _RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    _OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetModelsRequestGetModelsPaginateTypeDef(
+    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
+    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+    },
+)
+_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef(
+    _RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    _OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+):
+    pass
+
+_RequiredGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
+    "_RequiredGetRoutesRequestGetRoutesPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
+    "_OptionalGetRoutesRequestGetRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetRoutesRequestGetRoutesPaginateTypeDef(
+    _RequiredGetRoutesRequestGetRoutesPaginateTypeDef,
+    _OptionalGetRoutesRequestGetRoutesPaginateTypeDef,
+):
+    pass
+
+_RequiredGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
+    "_RequiredGetStagesRequestGetStagesPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
+    "_OptionalGetStagesRequestGetStagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetStagesRequestGetStagesPaginateTypeDef(
+    _RequiredGetStagesRequestGetStagesPaginateTypeDef,
+    _OptionalGetStagesRequestGetStagesPaginateTypeDef,
+):
+    pass
+
 GetIntegrationResponsesResponseTypeDef = TypedDict(
     "GetIntegrationResponsesResponseTypeDef",
     {
         "Items": List[IntegrationResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetModelsResponseTypeDef = TypedDict(
     "GetModelsResponseTypeDef",
     {
         "Items": List[ModelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVpcLinksResponseTypeDef = TypedDict(
     "GetVpcLinksResponseTypeDef",
     {
         "Items": List[VpcLinkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApisResponseTypeDef = TypedDict(
     "GetApisResponseTypeDef",
     {
         "Items": List[ApiTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAuthorizersResponseTypeDef = TypedDict(
     "GetAuthorizersResponseTypeDef",
     {
         "Items": List[AuthorizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainNamesResponseTypeDef = TypedDict(
     "GetDomainNamesResponseTypeDef",
     {
         "Items": List[DomainNameTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntegrationsResponseTypeDef = TypedDict(
     "GetIntegrationsResponseTypeDef",
     {
         "Items": List[IntegrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponsesResponseTypeDef = TypedDict(
     "GetRouteResponsesResponseTypeDef",
     {
         "Items": List[RouteResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoutesResponseTypeDef = TypedDict(
     "GetRoutesResponseTypeDef",
     {
         "Items": List[RouteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStagesResponseTypeDef = TypedDict(
     "GetStagesResponseTypeDef",
     {
         "Items": List[StageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2.egg-info/PKG-INFO` & `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewayv2
-Version: 1.28.12
-Summary: Type annotations for boto3.ApiGatewayV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ApiGatewayV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewayv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigatewayv2)](https://pepy.tech/project/mypy-boto3-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[boto3.ApiGatewayV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
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
 [mypy-boto3-apigatewayv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,41 +368,34 @@
 ### Typed dictionaries
 
 `mypy_boto3_apigatewayv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigatewayv2.type_defs import (
-    AccessLogSettingsOutputTypeDef,
     AccessLogSettingsTypeDef,
     ApiMappingTypeDef,
     CorsOutputTypeDef,
     JWTConfigurationOutputTypeDef,
     CorsTypeDef,
     CreateApiMappingRequestRequestTypeDef,
-    CreateApiMappingResponseTypeDef,
+    ResponseMetadataTypeDef,
     JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
     DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
     DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
-    CreateIntegrationResponseResponseTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
-    CreateModelResponseTypeDef,
     ParameterConstraintsTypeDef,
-    ParameterConstraintsOutputTypeDef,
     RouteSettingsTypeDef,
-    RouteSettingsOutputTypeDef,
     CreateVpcLinkRequestRequestTypeDef,
-    CreateVpcLinkResponseTypeDef,
     DeleteAccessLogSettingsRequestRequestTypeDef,
     DeleteApiMappingRequestRequestTypeDef,
     DeleteApiRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteCorsConfigurationRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
     DeleteDomainNameRequestRequestTypeDef,
@@ -412,93 +405,87 @@
     DeleteRouteRequestParameterRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseRequestRequestTypeDef,
     DeleteRouteSettingsRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     DeploymentTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportApiRequestRequestTypeDef,
-    ExportApiResponseTypeDef,
     GetApiMappingRequestRequestTypeDef,
-    GetApiMappingResponseTypeDef,
     GetApiMappingsRequestRequestTypeDef,
     GetApiRequestRequestTypeDef,
-    GetApisRequestGetApisPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetApisRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
-    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetAuthorizersRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetDeploymentResponseTypeDef,
-    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
-    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetDomainNamesRequestRequestTypeDef,
     GetIntegrationRequestRequestTypeDef,
     GetIntegrationResponseRequestRequestTypeDef,
-    GetIntegrationResponseResponseTypeDef,
-    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
     GetIntegrationResponsesRequestRequestTypeDef,
     IntegrationResponseTypeDef,
-    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
     GetIntegrationsRequestRequestTypeDef,
     GetModelRequestRequestTypeDef,
-    GetModelResponseTypeDef,
     GetModelTemplateRequestRequestTypeDef,
-    GetModelTemplateResponseTypeDef,
-    GetModelsRequestGetModelsPaginateTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetRouteRequestRequestTypeDef,
     GetRouteResponseRequestRequestTypeDef,
-    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
     GetRouteResponsesRequestRequestTypeDef,
-    GetRoutesRequestGetRoutesPaginateTypeDef,
     GetRoutesRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    GetStagesRequestGetStagesPaginateTypeDef,
     GetStagesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
-    GetTagsResponseTypeDef,
     GetVpcLinkRequestRequestTypeDef,
-    GetVpcLinkResponseTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     VpcLinkTypeDef,
     ImportApiRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ReimportApiRequestRequestTypeDef,
     ResetAuthorizersCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiMappingRequestRequestTypeDef,
-    UpdateApiMappingResponseTypeDef,
     UpdateDeploymentRequestRequestTypeDef,
-    UpdateDeploymentResponseTypeDef,
     UpdateIntegrationResponseRequestRequestTypeDef,
-    UpdateIntegrationResponseResponseTypeDef,
     UpdateModelRequestRequestTypeDef,
-    UpdateModelResponseTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
-    UpdateVpcLinkResponseTypeDef,
-    GetApiMappingsResponseTypeDef,
     ApiTypeDef,
+    AuthorizerTypeDef,
+    CreateApiRequestRequestTypeDef,
+    UpdateApiRequestRequestTypeDef,
+    CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateIntegrationResponseResponseTypeDef,
+    CreateModelResponseTypeDef,
+    CreateVpcLinkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportApiResponseTypeDef,
+    GetApiMappingResponseTypeDef,
+    GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
+    GetAuthorizerResponseTypeDef,
+    GetDeploymentResponseTypeDef,
+    GetIntegrationResponseResponseTypeDef,
+    GetModelResponseTypeDef,
+    GetModelTemplateResponseTypeDef,
+    GetTagsResponseTypeDef,
+    GetVpcLinkResponseTypeDef,
     ImportApiResponseTypeDef,
     ReimportApiResponseTypeDef,
+    UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
-    AuthorizerTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    GetAuthorizerResponseTypeDef,
     UpdateAuthorizerResponseTypeDef,
-    CreateApiRequestRequestTypeDef,
-    UpdateApiRequestRequestTypeDef,
+    UpdateDeploymentResponseTypeDef,
+    UpdateIntegrationResponseResponseTypeDef,
+    UpdateModelResponseTypeDef,
+    UpdateVpcLinkResponseTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
     CreateDomainNameRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     CreateDomainNameResponseTypeDef,
     DomainNameTypeDef,
     GetDomainNameResponseTypeDef,
@@ -507,45 +494,55 @@
     UpdateIntegrationRequestRequestTypeDef,
     CreateIntegrationResultTypeDef,
     GetIntegrationResultTypeDef,
     IntegrationTypeDef,
     UpdateIntegrationResultTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseRequestRequestTypeDef,
-    UpdateRouteRequestRequestTypeDef,
-    UpdateRouteResponseRequestRequestTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     GetRouteResponseResponseTypeDef,
     GetRouteResultTypeDef,
     RouteResponseTypeDef,
     RouteTypeDef,
+    UpdateRouteRequestRequestTypeDef,
+    UpdateRouteResponseRequestRequestTypeDef,
     UpdateRouteResponseResponseTypeDef,
     UpdateRouteResultTypeDef,
     CreateStageRequestRequestTypeDef,
-    UpdateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     StageTypeDef,
+    UpdateStageRequestRequestTypeDef,
     UpdateStageResponseTypeDef,
     GetDeploymentsResponseTypeDef,
+    GetApisRequestGetApisPaginateTypeDef,
+    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
+    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    GetModelsRequestGetModelsPaginateTypeDef,
+    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    GetRoutesRequestGetRoutesPaginateTypeDef,
+    GetStagesRequestGetStagesPaginateTypeDef,
     GetIntegrationResponsesResponseTypeDef,
     GetModelsResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizersResponseTypeDef,
     GetDomainNamesResponseTypeDef,
     GetIntegrationsResponseTypeDef,
     GetRouteResponsesResponseTypeDef,
     GetRoutesResponseTypeDef,
     GetStagesResponseTypeDef,
 )
 
 
-def get_structure() -> AccessLogSettingsOutputTypeDef:
+def get_structure() -> AccessLogSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apigatewayv2-1.28.12/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt` & `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.12/setup.py` & `mypy-boto3-apigatewayv2-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apigatewayv2",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_apigatewayv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApiGatewayV2 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.ApiGatewayV2 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

