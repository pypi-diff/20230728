# Comparing `tmp/mypy-boto3-panorama-1.28.12.tar.gz` & `tmp/mypy-boto3-panorama-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-panorama-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
+gzip compressed data, was "mypy-boto3-panorama-1.28.15.tar", last modified: Fri Jul 28 20:43:26 2023, max compression
```

## Comparing `mypy-boto3-panorama-1.28.12.tar` & `mypy-boto3-panorama-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.793132 mypy-boto3-panorama-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:10.000000 mypy-boto3-panorama-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16866 2023-07-27 11:49:21.793132 mypy-boto3-panorama-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15375 2023-07-27 11:41:10.000000 mypy-boto3-panorama-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.793132 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 11:41:10.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 11:41:10.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23775 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23734 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40902 2023-07-27 11:41:12.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40856 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:10.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.793132 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16866 2023-07-27 11:49:21.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-27 11:49:21.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:21.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.793132 mypy-boto3-panorama-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:41:10.000000 mypy-boto3-panorama-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:26.165623 mypy-boto3-panorama-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16578 2023-07-28 20:43:26.153623 mypy-boto3-panorama-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15087 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:26.145623 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23775 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23734 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-28 20:33:10.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-28 20:33:10.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38744 2023-07-28 20:33:11.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38701 2023-07-28 20:33:10.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:26.153623 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16578 2023-07-28 20:43:25.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-28 20:43:25.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:25.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:25.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:25.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:25.000000 mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:26.165623 mypy-boto3-panorama-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:33:09.000000 mypy-boto3-panorama-1.28.15/setup.py
```

### Comparing `mypy-boto3-panorama-1.28.12/LICENSE` & `mypy-boto3-panorama-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.12/PKG-INFO` & `mypy-boto3-panorama-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-panorama
-Version: 1.28.12
-Summary: Type annotations for boto3.Panorama 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Panorama 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-panorama)](https://pepy.tech/project/mypy-boto3-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Panorama 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[boto3.Panorama 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,16 +333,14 @@
     JobResourceTagsTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
-    ManifestOverridesPayloadOutputTypeDef,
-    ManifestPayloadOutputTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
     JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
@@ -373,41 +371,39 @@
     NtpPayloadOutputTypeDef,
     NtpPayloadTypeDef,
     NtpStatusTypeDef,
     NodeInputPortTypeDef,
     NodeOutputPortTypeDef,
     NodeSignalTypeDef,
     OutPutS3LocationTypeDef,
-    PackageVersionOutputConfigOutputTypeDef,
     PackageVersionOutputConfigTypeDef,
-    S3LocationOutputTypeDef,
     S3LocationTypeDef,
     RegisterPackageVersionRequestRequestTypeDef,
     RemoveApplicationInstanceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceMetadataRequestRequestTypeDef,
     ApplicationInstanceTypeDef,
     CreateApplicationInstanceRequestRequestTypeDef,
     CreateApplicationInstanceResponseTypeDef,
     CreateNodeFromTemplateJobResponseTypeDef,
     CreatePackageImportJobResponseTypeDef,
     DeleteDeviceResponseTypeDef,
+    DescribeApplicationInstanceDetailsResponseTypeDef,
     DescribeApplicationInstanceResponseTypeDef,
     DescribeDeviceJobResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
     CreateNodeFromTemplateJobRequestRequestTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
-    DescribeApplicationInstanceDetailsResponseTypeDef,
     DeviceTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
     EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
@@ -416,30 +412,27 @@
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     NetworkStatusTypeDef,
     NodeInterfaceTypeDef,
     SignalApplicationInstanceNodeInstancesRequestRequestTypeDef,
     PackageImportJobOutputTypeDef,
-    PackageImportJobOutputConfigOutputTypeDef,
     PackageImportJobOutputConfigTypeDef,
-    PackageVersionInputConfigOutputTypeDef,
     PackageVersionInputConfigTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesResponseTypeDef,
     CreateJobForDevicesRequestRequestTypeDef,
     NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
     DescribeNodeResponseTypeDef,
-    PackageImportJobInputConfigOutputTypeDef,
     PackageImportJobInputConfigTypeDef,
     DescribeDeviceResponseTypeDef,
     ProvisionDeviceRequestRequestTypeDef,
-    DescribePackageImportJobResponseTypeDef,
     CreatePackageImportJobRequestRequestTypeDef,
+    DescribePackageImportJobResponseTypeDef,
 )
 
 
 def get_structure() -> AlternateSoftwareMetadataTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-panorama-1.28.12/README.md` & `mypy-boto3-panorama-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-panorama)](https://pepy.tech/project/mypy-boto3-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Panorama 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[boto3.Panorama 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,16 +301,14 @@
     JobResourceTagsTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
-    ManifestOverridesPayloadOutputTypeDef,
-    ManifestPayloadOutputTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
     JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
@@ -341,41 +339,39 @@
     NtpPayloadOutputTypeDef,
     NtpPayloadTypeDef,
     NtpStatusTypeDef,
     NodeInputPortTypeDef,
     NodeOutputPortTypeDef,
     NodeSignalTypeDef,
     OutPutS3LocationTypeDef,
-    PackageVersionOutputConfigOutputTypeDef,
     PackageVersionOutputConfigTypeDef,
-    S3LocationOutputTypeDef,
     S3LocationTypeDef,
     RegisterPackageVersionRequestRequestTypeDef,
     RemoveApplicationInstanceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceMetadataRequestRequestTypeDef,
     ApplicationInstanceTypeDef,
     CreateApplicationInstanceRequestRequestTypeDef,
     CreateApplicationInstanceResponseTypeDef,
     CreateNodeFromTemplateJobResponseTypeDef,
     CreatePackageImportJobResponseTypeDef,
     DeleteDeviceResponseTypeDef,
+    DescribeApplicationInstanceDetailsResponseTypeDef,
     DescribeApplicationInstanceResponseTypeDef,
     DescribeDeviceJobResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
     CreateNodeFromTemplateJobRequestRequestTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
-    DescribeApplicationInstanceDetailsResponseTypeDef,
     DeviceTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
     EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
@@ -384,30 +380,27 @@
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     NetworkStatusTypeDef,
     NodeInterfaceTypeDef,
     SignalApplicationInstanceNodeInstancesRequestRequestTypeDef,
     PackageImportJobOutputTypeDef,
-    PackageImportJobOutputConfigOutputTypeDef,
     PackageImportJobOutputConfigTypeDef,
-    PackageVersionInputConfigOutputTypeDef,
     PackageVersionInputConfigTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesResponseTypeDef,
     CreateJobForDevicesRequestRequestTypeDef,
     NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
     DescribeNodeResponseTypeDef,
-    PackageImportJobInputConfigOutputTypeDef,
     PackageImportJobInputConfigTypeDef,
     DescribeDeviceResponseTypeDef,
     ProvisionDeviceRequestRequestTypeDef,
-    DescribePackageImportJobResponseTypeDef,
     CreatePackageImportJobRequestRequestTypeDef,
+    DescribePackageImportJobResponseTypeDef,
 )
 
 
 def get_structure() -> AlternateSoftwareMetadataTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/__main__.py` & `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Panorama 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Panorama 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama\nOther"
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

### Comparing `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/client.py` & `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/client.pyi` & `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/literals.py` & `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/literals.pyi` & `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/type_defs.py` & `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,31 +47,28 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
     "ResponseMetadataTypeDef",
     "JobTypeDef",
     "JobResourceTagsTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
-    "ManifestOverridesPayloadOutputTypeDef",
-    "ManifestPayloadOutputTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     "JobResourceTagsOutputTypeDef",
     "DescribeNodeRequestRequestTypeDef",
@@ -102,41 +99,39 @@
     "NtpPayloadOutputTypeDef",
     "NtpPayloadTypeDef",
     "NtpStatusTypeDef",
     "NodeInputPortTypeDef",
     "NodeOutputPortTypeDef",
     "NodeSignalTypeDef",
     "OutPutS3LocationTypeDef",
-    "PackageVersionOutputConfigOutputTypeDef",
     "PackageVersionOutputConfigTypeDef",
-    "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
     "RegisterPackageVersionRequestRequestTypeDef",
     "RemoveApplicationInstanceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceMetadataRequestRequestTypeDef",
     "ApplicationInstanceTypeDef",
     "CreateApplicationInstanceRequestRequestTypeDef",
     "CreateApplicationInstanceResponseTypeDef",
     "CreateNodeFromTemplateJobResponseTypeDef",
     "CreatePackageImportJobResponseTypeDef",
     "DeleteDeviceResponseTypeDef",
+    "DescribeApplicationInstanceDetailsResponseTypeDef",
     "DescribeApplicationInstanceResponseTypeDef",
     "DescribeDeviceJobResponseTypeDef",
     "DescribePackageVersionResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ProvisionDeviceResponseTypeDef",
     "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
     "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
-    "DescribeApplicationInstanceDetailsResponseTypeDef",
     "DeviceTypeDef",
     "DescribeNodeFromTemplateJobResponseTypeDef",
     "DeviceJobConfigTypeDef",
     "ListDevicesJobsResponseTypeDef",
     "EthernetPayloadOutputTypeDef",
     "EthernetPayloadTypeDef",
     "ListApplicationInstanceDependenciesResponseTypeDef",
@@ -145,30 +140,27 @@
     "ListNodesResponseTypeDef",
     "ListPackageImportJobsResponseTypeDef",
     "ListPackagesResponseTypeDef",
     "NetworkStatusTypeDef",
     "NodeInterfaceTypeDef",
     "SignalApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "PackageImportJobOutputTypeDef",
-    "PackageImportJobOutputConfigOutputTypeDef",
     "PackageImportJobOutputConfigTypeDef",
-    "PackageVersionInputConfigOutputTypeDef",
     "PackageVersionInputConfigTypeDef",
     "ListApplicationInstancesResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "CreateJobForDevicesRequestRequestTypeDef",
     "NetworkPayloadOutputTypeDef",
     "NetworkPayloadTypeDef",
     "DescribeNodeResponseTypeDef",
-    "PackageImportJobInputConfigOutputTypeDef",
     "PackageImportJobInputConfigTypeDef",
     "DescribeDeviceResponseTypeDef",
     "ProvisionDeviceRequestRequestTypeDef",
-    "DescribePackageImportJobResponseTypeDef",
     "CreatePackageImportJobRequestRequestTypeDef",
+    "DescribePackageImportJobResponseTypeDef",
 )
 
 AlternateSoftwareMetadataTypeDef = TypedDict(
     "AlternateSoftwareMetadataTypeDef",
     {
         "Version": str,
     },
@@ -239,21 +231,19 @@
     "_OptionalCreatePackageRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreatePackageRequestRequestTypeDef(
     _RequiredCreatePackageRequestRequestTypeDef, _OptionalCreatePackageRequestRequestTypeDef
 ):
     pass
 
-
 StorageLocationTypeDef = TypedDict(
     "StorageLocationTypeDef",
     {
         "BinaryPrefixLocation": str,
         "Bucket": str,
         "GeneratedPrefixLocation": str,
         "ManifestPrefixLocation": str,
@@ -278,21 +268,19 @@
     "_OptionalDeletePackageRequestRequestTypeDef",
     {
         "ForceDelete": bool,
     },
     total=False,
 )
 
-
 class DeletePackageRequestRequestTypeDef(
     _RequiredDeletePackageRequestRequestTypeDef, _OptionalDeletePackageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeregisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -302,45 +290,27 @@
     {
         "OwnerAccount": str,
         "UpdatedLatestPatchVersion": str,
     },
     total=False,
 )
 
-
 class DeregisterPackageVersionRequestRequestTypeDef(
     _RequiredDeregisterPackageVersionRequestRequestTypeDef,
     _OptionalDeregisterPackageVersionRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeApplicationInstanceDetailsRequestRequestTypeDef = TypedDict(
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
-ManifestOverridesPayloadOutputTypeDef = TypedDict(
-    "ManifestOverridesPayloadOutputTypeDef",
-    {
-        "PayloadData": str,
-    },
-    total=False,
-)
-
-ManifestPayloadOutputTypeDef = TypedDict(
-    "ManifestPayloadOutputTypeDef",
-    {
-        "PayloadData": str,
-    },
-    total=False,
-)
-
 DescribeApplicationInstanceRequestRequestTypeDef = TypedDict(
     "DescribeApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
@@ -393,21 +363,19 @@
     "_OptionalDescribeNodeRequestRequestTypeDef",
     {
         "OwnerAccount": str,
     },
     total=False,
 )
 
-
 class DescribeNodeRequestRequestTypeDef(
     _RequiredDescribeNodeRequestRequestTypeDef, _OptionalDescribeNodeRequestRequestTypeDef
 ):
     pass
 
-
 DescribePackageImportJobRequestRequestTypeDef = TypedDict(
     "DescribePackageImportJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -430,41 +398,37 @@
     {
         "OwnerAccount": str,
         "PatchVersion": str,
     },
     total=False,
 )
 
-
 class DescribePackageVersionRequestRequestTypeDef(
     _RequiredDescribePackageVersionRequestRequestTypeDef,
     _OptionalDescribePackageVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredOTAJobConfigTypeDef = TypedDict(
     "_RequiredOTAJobConfigTypeDef",
     {
         "ImageVersion": str,
     },
 )
 _OptionalOTAJobConfigTypeDef = TypedDict(
     "_OptionalOTAJobConfigTypeDef",
     {
         "AllowMajorVersionUpdate": bool,
     },
     total=False,
 )
 
-
 class OTAJobConfigTypeDef(_RequiredOTAJobConfigTypeDef, _OptionalOTAJobConfigTypeDef):
     pass
 
-
 DeviceJobTypeDef = TypedDict(
     "DeviceJobTypeDef",
     {
         "CreatedTime": datetime,
         "DeviceId": str,
         "DeviceName": str,
         "JobId": str,
@@ -514,22 +478,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListApplicationInstanceDependenciesRequestRequestTypeDef(
     _RequiredListApplicationInstanceDependenciesRequestRequestTypeDef,
     _OptionalListApplicationInstanceDependenciesRequestRequestTypeDef,
 ):
     pass
 
-
 PackageObjectTypeDef = TypedDict(
     "PackageObjectTypeDef",
     {
         "Name": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -546,22 +508,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListApplicationInstanceNodeInstancesRequestRequestTypeDef(
     _RequiredListApplicationInstanceNodeInstancesRequestRequestTypeDef,
     _OptionalListApplicationInstanceNodeInstancesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredNodeInstanceTypeDef = TypedDict(
     "_RequiredNodeInstanceTypeDef",
     {
         "CurrentStatus": NodeInstanceStatusType,
         "NodeInstanceId": str,
     },
 )
@@ -573,19 +533,17 @@
         "PackageName": str,
         "PackagePatchVersion": str,
         "PackageVersion": str,
     },
     total=False,
 )
 
-
 class NodeInstanceTypeDef(_RequiredNodeInstanceTypeDef, _OptionalNodeInstanceTypeDef):
     pass
 
-
 ListApplicationInstancesRequestRequestTypeDef = TypedDict(
     "ListApplicationInstancesRequestRequestTypeDef",
     {
         "DeviceId": str,
         "MaxResults": int,
         "NextToken": str,
         "StatusFilter": StatusFilterType,
@@ -671,19 +629,17 @@
         "Description": str,
         "OwnerAccount": str,
         "PackageArn": str,
     },
     total=False,
 )
 
-
 class NodeTypeDef(_RequiredNodeTypeDef, _OptionalNodeTypeDef):
     pass
 
-
 ListPackageImportJobsRequestRequestTypeDef = TypedDict(
     "ListPackageImportJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -788,37 +744,14 @@
     "OutPutS3LocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
 )
 
-_RequiredPackageVersionOutputConfigOutputTypeDef = TypedDict(
-    "_RequiredPackageVersionOutputConfigOutputTypeDef",
-    {
-        "PackageName": str,
-        "PackageVersion": str,
-    },
-)
-_OptionalPackageVersionOutputConfigOutputTypeDef = TypedDict(
-    "_OptionalPackageVersionOutputConfigOutputTypeDef",
-    {
-        "MarkLatest": bool,
-    },
-    total=False,
-)
-
-
-class PackageVersionOutputConfigOutputTypeDef(
-    _RequiredPackageVersionOutputConfigOutputTypeDef,
-    _OptionalPackageVersionOutputConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredPackageVersionOutputConfigTypeDef = TypedDict(
     "_RequiredPackageVersionOutputConfigTypeDef",
     {
         "PackageName": str,
         "PackageVersion": str,
     },
 )
@@ -826,41 +759,19 @@
     "_OptionalPackageVersionOutputConfigTypeDef",
     {
         "MarkLatest": bool,
     },
     total=False,
 )
 
-
 class PackageVersionOutputConfigTypeDef(
     _RequiredPackageVersionOutputConfigTypeDef, _OptionalPackageVersionOutputConfigTypeDef
 ):
     pass
 
-
-_RequiredS3LocationOutputTypeDef = TypedDict(
-    "_RequiredS3LocationOutputTypeDef",
-    {
-        "BucketName": str,
-        "ObjectKey": str,
-    },
-)
-_OptionalS3LocationOutputTypeDef = TypedDict(
-    "_OptionalS3LocationOutputTypeDef",
-    {
-        "Region": str,
-    },
-    total=False,
-)
-
-
-class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
-    pass
-
-
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
 )
@@ -868,19 +779,17 @@
     "_OptionalS3LocationTypeDef",
     {
         "Region": str,
     },
     total=False,
 )
 
-
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-
 _RequiredRegisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -890,22 +799,20 @@
     {
         "MarkLatest": bool,
         "OwnerAccount": str,
     },
     total=False,
 )
 
-
 class RegisterPackageVersionRequestRequestTypeDef(
     _RequiredRegisterPackageVersionRequestRequestTypeDef,
     _OptionalRegisterPackageVersionRequestRequestTypeDef,
 ):
     pass
 
-
 RemoveApplicationInstanceRequestRequestTypeDef = TypedDict(
     "RemoveApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
@@ -935,22 +842,20 @@
     "_OptionalUpdateDeviceMetadataRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateDeviceMetadataRequestRequestTypeDef(
     _RequiredUpdateDeviceMetadataRequestRequestTypeDef,
     _OptionalUpdateDeviceMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 ApplicationInstanceTypeDef = TypedDict(
     "ApplicationInstanceTypeDef",
     {
         "ApplicationInstanceId": str,
         "Arn": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
@@ -982,22 +887,20 @@
         "Name": str,
         "RuntimeRoleArn": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateApplicationInstanceRequestRequestTypeDef(
     _RequiredCreateApplicationInstanceRequestRequestTypeDef,
     _OptionalCreateApplicationInstanceRequestRequestTypeDef,
 ):
     pass
 
-
 CreateApplicationInstanceResponseTypeDef = TypedDict(
     "CreateApplicationInstanceResponseTypeDef",
     {
         "ApplicationInstanceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1022,14 +925,29 @@
     "DeleteDeviceResponseTypeDef",
     {
         "DeviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeApplicationInstanceDetailsResponseTypeDef = TypedDict(
+    "DescribeApplicationInstanceDetailsResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ApplicationInstanceIdToReplace": str,
+        "CreatedTime": datetime,
+        "DefaultRuntimeContextDevice": str,
+        "Description": str,
+        "ManifestOverridesPayload": ManifestOverridesPayloadTypeDef,
+        "ManifestPayload": ManifestPayloadTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeApplicationInstanceResponseTypeDef = TypedDict(
     "DescribeApplicationInstanceResponseTypeDef",
     {
         "ApplicationInstanceId": str,
         "ApplicationInstanceIdToReplace": str,
         "Arn": str,
         "CreatedTime": datetime,
@@ -1140,22 +1058,20 @@
     {
         "JobTags": Sequence[JobResourceTagsTypeDef],
         "NodeDescription": str,
     },
     total=False,
 )
 
-
 class CreateNodeFromTemplateJobRequestRequestTypeDef(
     _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
     _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
 ):
     pass
 
-
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "Arn": str,
         "PackageId": str,
         "StorageLocation": StorageLocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1173,29 +1089,14 @@
         "StorageLocation": StorageLocationTypeDef,
         "Tags": Dict[str, str],
         "WriteAccessPrincipalArns": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeApplicationInstanceDetailsResponseTypeDef = TypedDict(
-    "DescribeApplicationInstanceDetailsResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ApplicationInstanceIdToReplace": str,
-        "CreatedTime": datetime,
-        "DefaultRuntimeContextDevice": str,
-        "Description": str,
-        "ManifestOverridesPayload": ManifestOverridesPayloadOutputTypeDef,
-        "ManifestPayload": ManifestPayloadOutputTypeDef,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "Brand": DeviceBrandType,
         "CreatedTime": datetime,
         "CurrentSoftware": str,
         "Description": str,
@@ -1258,40 +1159,36 @@
     "_OptionalEthernetPayloadOutputTypeDef",
     {
         "StaticIpConnectionInfo": StaticIpConnectionInfoOutputTypeDef,
     },
     total=False,
 )
 
-
 class EthernetPayloadOutputTypeDef(
     _RequiredEthernetPayloadOutputTypeDef, _OptionalEthernetPayloadOutputTypeDef
 ):
     pass
 
-
 _RequiredEthernetPayloadTypeDef = TypedDict(
     "_RequiredEthernetPayloadTypeDef",
     {
         "ConnectionType": ConnectionTypeType,
     },
 )
 _OptionalEthernetPayloadTypeDef = TypedDict(
     "_OptionalEthernetPayloadTypeDef",
     {
         "StaticIpConnectionInfo": StaticIpConnectionInfoTypeDef,
     },
     total=False,
 )
 
-
 class EthernetPayloadTypeDef(_RequiredEthernetPayloadTypeDef, _OptionalEthernetPayloadTypeDef):
     pass
 
-
 ListApplicationInstanceDependenciesResponseTypeDef = TypedDict(
     "ListApplicationInstanceDependenciesResponseTypeDef",
     {
         "NextToken": str,
         "PackageObjects": List[PackageObjectTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1375,37 +1272,22 @@
         "OutputS3Location": OutPutS3LocationTypeDef,
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
 )
 
-PackageImportJobOutputConfigOutputTypeDef = TypedDict(
-    "PackageImportJobOutputConfigOutputTypeDef",
-    {
-        "PackageVersionOutputConfig": PackageVersionOutputConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 PackageImportJobOutputConfigTypeDef = TypedDict(
     "PackageImportJobOutputConfigTypeDef",
     {
         "PackageVersionOutputConfig": PackageVersionOutputConfigTypeDef,
     },
     total=False,
 )
 
-PackageVersionInputConfigOutputTypeDef = TypedDict(
-    "PackageVersionInputConfigOutputTypeDef",
-    {
-        "S3Location": S3LocationOutputTypeDef,
-    },
-)
-
 PackageVersionInputConfigTypeDef = TypedDict(
     "PackageVersionInputConfigTypeDef",
     {
         "S3Location": S3LocationTypeDef,
     },
 )
 
@@ -1438,22 +1320,20 @@
     "_OptionalCreateJobForDevicesRequestRequestTypeDef",
     {
         "DeviceJobConfig": DeviceJobConfigTypeDef,
     },
     total=False,
 )
 
-
 class CreateJobForDevicesRequestRequestTypeDef(
     _RequiredCreateJobForDevicesRequestRequestTypeDef,
     _OptionalCreateJobForDevicesRequestRequestTypeDef,
 ):
     pass
 
-
 NetworkPayloadOutputTypeDef = TypedDict(
     "NetworkPayloadOutputTypeDef",
     {
         "Ethernet0": EthernetPayloadOutputTypeDef,
         "Ethernet1": EthernetPayloadOutputTypeDef,
         "Ntp": NtpPayloadOutputTypeDef,
     },
@@ -1487,22 +1367,14 @@
         "PackageName": str,
         "PackageVersion": str,
         "PatchVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PackageImportJobInputConfigOutputTypeDef = TypedDict(
-    "PackageImportJobInputConfigOutputTypeDef",
-    {
-        "PackageVersionInputConfig": PackageVersionInputConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 PackageImportJobInputConfigTypeDef = TypedDict(
     "PackageImportJobInputConfigTypeDef",
     {
         "PackageVersionInputConfig": PackageVersionInputConfigTypeDef,
     },
     total=False,
 )
@@ -1546,39 +1418,19 @@
         "Description": str,
         "NetworkingConfiguration": NetworkPayloadTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ProvisionDeviceRequestRequestTypeDef(
     _RequiredProvisionDeviceRequestRequestTypeDef, _OptionalProvisionDeviceRequestRequestTypeDef
 ):
     pass
 
-
-DescribePackageImportJobResponseTypeDef = TypedDict(
-    "DescribePackageImportJobResponseTypeDef",
-    {
-        "ClientToken": str,
-        "CreatedTime": datetime,
-        "InputConfig": PackageImportJobInputConfigOutputTypeDef,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsOutputTypeDef],
-        "JobType": PackageImportJobTypeType,
-        "LastUpdatedTime": datetime,
-        "Output": PackageImportJobOutputTypeDef,
-        "OutputConfig": PackageImportJobOutputConfigOutputTypeDef,
-        "Status": PackageImportJobStatusType,
-        "StatusMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageImportJobRequestRequestTypeDef",
     {
         "ClientToken": str,
         "InputConfig": PackageImportJobInputConfigTypeDef,
         "JobType": PackageImportJobTypeType,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
@@ -1588,13 +1440,30 @@
     "_OptionalCreatePackageImportJobRequestRequestTypeDef",
     {
         "JobTags": Sequence[JobResourceTagsTypeDef],
     },
     total=False,
 )
 
-
 class CreatePackageImportJobRequestRequestTypeDef(
     _RequiredCreatePackageImportJobRequestRequestTypeDef,
     _OptionalCreatePackageImportJobRequestRequestTypeDef,
 ):
     pass
+
+DescribePackageImportJobResponseTypeDef = TypedDict(
+    "DescribePackageImportJobResponseTypeDef",
+    {
+        "ClientToken": str,
+        "CreatedTime": datetime,
+        "InputConfig": PackageImportJobInputConfigTypeDef,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "JobType": PackageImportJobTypeType,
+        "LastUpdatedTime": datetime,
+        "Output": PackageImportJobOutputTypeDef,
+        "OutputConfig": PackageImportJobOutputConfigTypeDef,
+        "Status": PackageImportJobStatusType,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/type_defs.pyi` & `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,30 +47,29 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
     "ResponseMetadataTypeDef",
     "JobTypeDef",
     "JobResourceTagsTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
-    "ManifestOverridesPayloadOutputTypeDef",
-    "ManifestPayloadOutputTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     "JobResourceTagsOutputTypeDef",
     "DescribeNodeRequestRequestTypeDef",
@@ -101,41 +100,39 @@
     "NtpPayloadOutputTypeDef",
     "NtpPayloadTypeDef",
     "NtpStatusTypeDef",
     "NodeInputPortTypeDef",
     "NodeOutputPortTypeDef",
     "NodeSignalTypeDef",
     "OutPutS3LocationTypeDef",
-    "PackageVersionOutputConfigOutputTypeDef",
     "PackageVersionOutputConfigTypeDef",
-    "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
     "RegisterPackageVersionRequestRequestTypeDef",
     "RemoveApplicationInstanceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceMetadataRequestRequestTypeDef",
     "ApplicationInstanceTypeDef",
     "CreateApplicationInstanceRequestRequestTypeDef",
     "CreateApplicationInstanceResponseTypeDef",
     "CreateNodeFromTemplateJobResponseTypeDef",
     "CreatePackageImportJobResponseTypeDef",
     "DeleteDeviceResponseTypeDef",
+    "DescribeApplicationInstanceDetailsResponseTypeDef",
     "DescribeApplicationInstanceResponseTypeDef",
     "DescribeDeviceJobResponseTypeDef",
     "DescribePackageVersionResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ProvisionDeviceResponseTypeDef",
     "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
     "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
-    "DescribeApplicationInstanceDetailsResponseTypeDef",
     "DeviceTypeDef",
     "DescribeNodeFromTemplateJobResponseTypeDef",
     "DeviceJobConfigTypeDef",
     "ListDevicesJobsResponseTypeDef",
     "EthernetPayloadOutputTypeDef",
     "EthernetPayloadTypeDef",
     "ListApplicationInstanceDependenciesResponseTypeDef",
@@ -144,30 +141,27 @@
     "ListNodesResponseTypeDef",
     "ListPackageImportJobsResponseTypeDef",
     "ListPackagesResponseTypeDef",
     "NetworkStatusTypeDef",
     "NodeInterfaceTypeDef",
     "SignalApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "PackageImportJobOutputTypeDef",
-    "PackageImportJobOutputConfigOutputTypeDef",
     "PackageImportJobOutputConfigTypeDef",
-    "PackageVersionInputConfigOutputTypeDef",
     "PackageVersionInputConfigTypeDef",
     "ListApplicationInstancesResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "CreateJobForDevicesRequestRequestTypeDef",
     "NetworkPayloadOutputTypeDef",
     "NetworkPayloadTypeDef",
     "DescribeNodeResponseTypeDef",
-    "PackageImportJobInputConfigOutputTypeDef",
     "PackageImportJobInputConfigTypeDef",
     "DescribeDeviceResponseTypeDef",
     "ProvisionDeviceRequestRequestTypeDef",
-    "DescribePackageImportJobResponseTypeDef",
     "CreatePackageImportJobRequestRequestTypeDef",
+    "DescribePackageImportJobResponseTypeDef",
 )
 
 AlternateSoftwareMetadataTypeDef = TypedDict(
     "AlternateSoftwareMetadataTypeDef",
     {
         "Version": str,
     },
@@ -238,19 +232,21 @@
     "_OptionalCreatePackageRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreatePackageRequestRequestTypeDef(
     _RequiredCreatePackageRequestRequestTypeDef, _OptionalCreatePackageRequestRequestTypeDef
 ):
     pass
 
+
 StorageLocationTypeDef = TypedDict(
     "StorageLocationTypeDef",
     {
         "BinaryPrefixLocation": str,
         "Bucket": str,
         "GeneratedPrefixLocation": str,
         "ManifestPrefixLocation": str,
@@ -275,19 +271,21 @@
     "_OptionalDeletePackageRequestRequestTypeDef",
     {
         "ForceDelete": bool,
     },
     total=False,
 )
 
+
 class DeletePackageRequestRequestTypeDef(
     _RequiredDeletePackageRequestRequestTypeDef, _OptionalDeletePackageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeregisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -297,43 +295,29 @@
     {
         "OwnerAccount": str,
         "UpdatedLatestPatchVersion": str,
     },
     total=False,
 )
 
+
 class DeregisterPackageVersionRequestRequestTypeDef(
     _RequiredDeregisterPackageVersionRequestRequestTypeDef,
     _OptionalDeregisterPackageVersionRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeApplicationInstanceDetailsRequestRequestTypeDef = TypedDict(
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
-ManifestOverridesPayloadOutputTypeDef = TypedDict(
-    "ManifestOverridesPayloadOutputTypeDef",
-    {
-        "PayloadData": str,
-    },
-    total=False,
-)
-
-ManifestPayloadOutputTypeDef = TypedDict(
-    "ManifestPayloadOutputTypeDef",
-    {
-        "PayloadData": str,
-    },
-    total=False,
-)
-
 DescribeApplicationInstanceRequestRequestTypeDef = TypedDict(
     "DescribeApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
@@ -386,19 +370,21 @@
     "_OptionalDescribeNodeRequestRequestTypeDef",
     {
         "OwnerAccount": str,
     },
     total=False,
 )
 
+
 class DescribeNodeRequestRequestTypeDef(
     _RequiredDescribeNodeRequestRequestTypeDef, _OptionalDescribeNodeRequestRequestTypeDef
 ):
     pass
 
+
 DescribePackageImportJobRequestRequestTypeDef = TypedDict(
     "DescribePackageImportJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -421,37 +407,41 @@
     {
         "OwnerAccount": str,
         "PatchVersion": str,
     },
     total=False,
 )
 
+
 class DescribePackageVersionRequestRequestTypeDef(
     _RequiredDescribePackageVersionRequestRequestTypeDef,
     _OptionalDescribePackageVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredOTAJobConfigTypeDef = TypedDict(
     "_RequiredOTAJobConfigTypeDef",
     {
         "ImageVersion": str,
     },
 )
 _OptionalOTAJobConfigTypeDef = TypedDict(
     "_OptionalOTAJobConfigTypeDef",
     {
         "AllowMajorVersionUpdate": bool,
     },
     total=False,
 )
 
+
 class OTAJobConfigTypeDef(_RequiredOTAJobConfigTypeDef, _OptionalOTAJobConfigTypeDef):
     pass
 
+
 DeviceJobTypeDef = TypedDict(
     "DeviceJobTypeDef",
     {
         "CreatedTime": datetime,
         "DeviceId": str,
         "DeviceName": str,
         "JobId": str,
@@ -501,20 +491,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListApplicationInstanceDependenciesRequestRequestTypeDef(
     _RequiredListApplicationInstanceDependenciesRequestRequestTypeDef,
     _OptionalListApplicationInstanceDependenciesRequestRequestTypeDef,
 ):
     pass
 
+
 PackageObjectTypeDef = TypedDict(
     "PackageObjectTypeDef",
     {
         "Name": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -531,20 +523,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListApplicationInstanceNodeInstancesRequestRequestTypeDef(
     _RequiredListApplicationInstanceNodeInstancesRequestRequestTypeDef,
     _OptionalListApplicationInstanceNodeInstancesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredNodeInstanceTypeDef = TypedDict(
     "_RequiredNodeInstanceTypeDef",
     {
         "CurrentStatus": NodeInstanceStatusType,
         "NodeInstanceId": str,
     },
 )
@@ -556,17 +550,19 @@
         "PackageName": str,
         "PackagePatchVersion": str,
         "PackageVersion": str,
     },
     total=False,
 )
 
+
 class NodeInstanceTypeDef(_RequiredNodeInstanceTypeDef, _OptionalNodeInstanceTypeDef):
     pass
 
+
 ListApplicationInstancesRequestRequestTypeDef = TypedDict(
     "ListApplicationInstancesRequestRequestTypeDef",
     {
         "DeviceId": str,
         "MaxResults": int,
         "NextToken": str,
         "StatusFilter": StatusFilterType,
@@ -652,17 +648,19 @@
         "Description": str,
         "OwnerAccount": str,
         "PackageArn": str,
     },
     total=False,
 )
 
+
 class NodeTypeDef(_RequiredNodeTypeDef, _OptionalNodeTypeDef):
     pass
 
+
 ListPackageImportJobsRequestRequestTypeDef = TypedDict(
     "ListPackageImportJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -767,35 +765,14 @@
     "OutPutS3LocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
 )
 
-_RequiredPackageVersionOutputConfigOutputTypeDef = TypedDict(
-    "_RequiredPackageVersionOutputConfigOutputTypeDef",
-    {
-        "PackageName": str,
-        "PackageVersion": str,
-    },
-)
-_OptionalPackageVersionOutputConfigOutputTypeDef = TypedDict(
-    "_OptionalPackageVersionOutputConfigOutputTypeDef",
-    {
-        "MarkLatest": bool,
-    },
-    total=False,
-)
-
-class PackageVersionOutputConfigOutputTypeDef(
-    _RequiredPackageVersionOutputConfigOutputTypeDef,
-    _OptionalPackageVersionOutputConfigOutputTypeDef,
-):
-    pass
-
 _RequiredPackageVersionOutputConfigTypeDef = TypedDict(
     "_RequiredPackageVersionOutputConfigTypeDef",
     {
         "PackageName": str,
         "PackageVersion": str,
     },
 )
@@ -803,36 +780,20 @@
     "_OptionalPackageVersionOutputConfigTypeDef",
     {
         "MarkLatest": bool,
     },
     total=False,
 )
 
+
 class PackageVersionOutputConfigTypeDef(
     _RequiredPackageVersionOutputConfigTypeDef, _OptionalPackageVersionOutputConfigTypeDef
 ):
     pass
 
-_RequiredS3LocationOutputTypeDef = TypedDict(
-    "_RequiredS3LocationOutputTypeDef",
-    {
-        "BucketName": str,
-        "ObjectKey": str,
-    },
-)
-_OptionalS3LocationOutputTypeDef = TypedDict(
-    "_OptionalS3LocationOutputTypeDef",
-    {
-        "Region": str,
-    },
-    total=False,
-)
-
-class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
-    pass
 
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
@@ -841,17 +802,19 @@
     "_OptionalS3LocationTypeDef",
     {
         "Region": str,
     },
     total=False,
 )
 
+
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
+
 _RequiredRegisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -861,20 +824,22 @@
     {
         "MarkLatest": bool,
         "OwnerAccount": str,
     },
     total=False,
 )
 
+
 class RegisterPackageVersionRequestRequestTypeDef(
     _RequiredRegisterPackageVersionRequestRequestTypeDef,
     _OptionalRegisterPackageVersionRequestRequestTypeDef,
 ):
     pass
 
+
 RemoveApplicationInstanceRequestRequestTypeDef = TypedDict(
     "RemoveApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
@@ -904,20 +869,22 @@
     "_OptionalUpdateDeviceMetadataRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateDeviceMetadataRequestRequestTypeDef(
     _RequiredUpdateDeviceMetadataRequestRequestTypeDef,
     _OptionalUpdateDeviceMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 ApplicationInstanceTypeDef = TypedDict(
     "ApplicationInstanceTypeDef",
     {
         "ApplicationInstanceId": str,
         "Arn": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
@@ -949,20 +916,22 @@
         "Name": str,
         "RuntimeRoleArn": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateApplicationInstanceRequestRequestTypeDef(
     _RequiredCreateApplicationInstanceRequestRequestTypeDef,
     _OptionalCreateApplicationInstanceRequestRequestTypeDef,
 ):
     pass
 
+
 CreateApplicationInstanceResponseTypeDef = TypedDict(
     "CreateApplicationInstanceResponseTypeDef",
     {
         "ApplicationInstanceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -987,14 +956,29 @@
     "DeleteDeviceResponseTypeDef",
     {
         "DeviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeApplicationInstanceDetailsResponseTypeDef = TypedDict(
+    "DescribeApplicationInstanceDetailsResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ApplicationInstanceIdToReplace": str,
+        "CreatedTime": datetime,
+        "DefaultRuntimeContextDevice": str,
+        "Description": str,
+        "ManifestOverridesPayload": ManifestOverridesPayloadTypeDef,
+        "ManifestPayload": ManifestPayloadTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeApplicationInstanceResponseTypeDef = TypedDict(
     "DescribeApplicationInstanceResponseTypeDef",
     {
         "ApplicationInstanceId": str,
         "ApplicationInstanceIdToReplace": str,
         "Arn": str,
         "CreatedTime": datetime,
@@ -1105,20 +1089,22 @@
     {
         "JobTags": Sequence[JobResourceTagsTypeDef],
         "NodeDescription": str,
     },
     total=False,
 )
 
+
 class CreateNodeFromTemplateJobRequestRequestTypeDef(
     _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
     _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
 ):
     pass
 
+
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "Arn": str,
         "PackageId": str,
         "StorageLocation": StorageLocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1136,29 +1122,14 @@
         "StorageLocation": StorageLocationTypeDef,
         "Tags": Dict[str, str],
         "WriteAccessPrincipalArns": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeApplicationInstanceDetailsResponseTypeDef = TypedDict(
-    "DescribeApplicationInstanceDetailsResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ApplicationInstanceIdToReplace": str,
-        "CreatedTime": datetime,
-        "DefaultRuntimeContextDevice": str,
-        "Description": str,
-        "ManifestOverridesPayload": ManifestOverridesPayloadOutputTypeDef,
-        "ManifestPayload": ManifestPayloadOutputTypeDef,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "Brand": DeviceBrandType,
         "CreatedTime": datetime,
         "CurrentSoftware": str,
         "Description": str,
@@ -1221,36 +1192,40 @@
     "_OptionalEthernetPayloadOutputTypeDef",
     {
         "StaticIpConnectionInfo": StaticIpConnectionInfoOutputTypeDef,
     },
     total=False,
 )
 
+
 class EthernetPayloadOutputTypeDef(
     _RequiredEthernetPayloadOutputTypeDef, _OptionalEthernetPayloadOutputTypeDef
 ):
     pass
 
+
 _RequiredEthernetPayloadTypeDef = TypedDict(
     "_RequiredEthernetPayloadTypeDef",
     {
         "ConnectionType": ConnectionTypeType,
     },
 )
 _OptionalEthernetPayloadTypeDef = TypedDict(
     "_OptionalEthernetPayloadTypeDef",
     {
         "StaticIpConnectionInfo": StaticIpConnectionInfoTypeDef,
     },
     total=False,
 )
 
+
 class EthernetPayloadTypeDef(_RequiredEthernetPayloadTypeDef, _OptionalEthernetPayloadTypeDef):
     pass
 
+
 ListApplicationInstanceDependenciesResponseTypeDef = TypedDict(
     "ListApplicationInstanceDependenciesResponseTypeDef",
     {
         "NextToken": str,
         "PackageObjects": List[PackageObjectTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1334,37 +1309,22 @@
         "OutputS3Location": OutPutS3LocationTypeDef,
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
 )
 
-PackageImportJobOutputConfigOutputTypeDef = TypedDict(
-    "PackageImportJobOutputConfigOutputTypeDef",
-    {
-        "PackageVersionOutputConfig": PackageVersionOutputConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 PackageImportJobOutputConfigTypeDef = TypedDict(
     "PackageImportJobOutputConfigTypeDef",
     {
         "PackageVersionOutputConfig": PackageVersionOutputConfigTypeDef,
     },
     total=False,
 )
 
-PackageVersionInputConfigOutputTypeDef = TypedDict(
-    "PackageVersionInputConfigOutputTypeDef",
-    {
-        "S3Location": S3LocationOutputTypeDef,
-    },
-)
-
 PackageVersionInputConfigTypeDef = TypedDict(
     "PackageVersionInputConfigTypeDef",
     {
         "S3Location": S3LocationTypeDef,
     },
 )
 
@@ -1397,20 +1357,22 @@
     "_OptionalCreateJobForDevicesRequestRequestTypeDef",
     {
         "DeviceJobConfig": DeviceJobConfigTypeDef,
     },
     total=False,
 )
 
+
 class CreateJobForDevicesRequestRequestTypeDef(
     _RequiredCreateJobForDevicesRequestRequestTypeDef,
     _OptionalCreateJobForDevicesRequestRequestTypeDef,
 ):
     pass
 
+
 NetworkPayloadOutputTypeDef = TypedDict(
     "NetworkPayloadOutputTypeDef",
     {
         "Ethernet0": EthernetPayloadOutputTypeDef,
         "Ethernet1": EthernetPayloadOutputTypeDef,
         "Ntp": NtpPayloadOutputTypeDef,
     },
@@ -1444,22 +1406,14 @@
         "PackageName": str,
         "PackageVersion": str,
         "PatchVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PackageImportJobInputConfigOutputTypeDef = TypedDict(
-    "PackageImportJobInputConfigOutputTypeDef",
-    {
-        "PackageVersionInputConfig": PackageVersionInputConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 PackageImportJobInputConfigTypeDef = TypedDict(
     "PackageImportJobInputConfigTypeDef",
     {
         "PackageVersionInputConfig": PackageVersionInputConfigTypeDef,
     },
     total=False,
 )
@@ -1503,36 +1457,20 @@
         "Description": str,
         "NetworkingConfiguration": NetworkPayloadTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ProvisionDeviceRequestRequestTypeDef(
     _RequiredProvisionDeviceRequestRequestTypeDef, _OptionalProvisionDeviceRequestRequestTypeDef
 ):
     pass
 
-DescribePackageImportJobResponseTypeDef = TypedDict(
-    "DescribePackageImportJobResponseTypeDef",
-    {
-        "ClientToken": str,
-        "CreatedTime": datetime,
-        "InputConfig": PackageImportJobInputConfigOutputTypeDef,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsOutputTypeDef],
-        "JobType": PackageImportJobTypeType,
-        "LastUpdatedTime": datetime,
-        "Output": PackageImportJobOutputTypeDef,
-        "OutputConfig": PackageImportJobOutputConfigOutputTypeDef,
-        "Status": PackageImportJobStatusType,
-        "StatusMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageImportJobRequestRequestTypeDef",
     {
         "ClientToken": str,
         "InputConfig": PackageImportJobInputConfigTypeDef,
         "JobType": PackageImportJobTypeType,
@@ -1543,12 +1481,32 @@
     "_OptionalCreatePackageImportJobRequestRequestTypeDef",
     {
         "JobTags": Sequence[JobResourceTagsTypeDef],
     },
     total=False,
 )
 
+
 class CreatePackageImportJobRequestRequestTypeDef(
     _RequiredCreatePackageImportJobRequestRequestTypeDef,
     _OptionalCreatePackageImportJobRequestRequestTypeDef,
 ):
     pass
+
+
+DescribePackageImportJobResponseTypeDef = TypedDict(
+    "DescribePackageImportJobResponseTypeDef",
+    {
+        "ClientToken": str,
+        "CreatedTime": datetime,
+        "InputConfig": PackageImportJobInputConfigTypeDef,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "JobType": PackageImportJobTypeType,
+        "LastUpdatedTime": datetime,
+        "Output": PackageImportJobOutputTypeDef,
+        "OutputConfig": PackageImportJobOutputConfigTypeDef,
+        "Status": PackageImportJobStatusType,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/PKG-INFO` & `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-panorama
-Version: 1.28.12
-Summary: Type annotations for boto3.Panorama 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Panorama 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-panorama)](https://pepy.tech/project/mypy-boto3-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Panorama 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[boto3.Panorama 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,16 +333,14 @@
     JobResourceTagsTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
-    ManifestOverridesPayloadOutputTypeDef,
-    ManifestPayloadOutputTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
     JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
@@ -373,41 +371,39 @@
     NtpPayloadOutputTypeDef,
     NtpPayloadTypeDef,
     NtpStatusTypeDef,
     NodeInputPortTypeDef,
     NodeOutputPortTypeDef,
     NodeSignalTypeDef,
     OutPutS3LocationTypeDef,
-    PackageVersionOutputConfigOutputTypeDef,
     PackageVersionOutputConfigTypeDef,
-    S3LocationOutputTypeDef,
     S3LocationTypeDef,
     RegisterPackageVersionRequestRequestTypeDef,
     RemoveApplicationInstanceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceMetadataRequestRequestTypeDef,
     ApplicationInstanceTypeDef,
     CreateApplicationInstanceRequestRequestTypeDef,
     CreateApplicationInstanceResponseTypeDef,
     CreateNodeFromTemplateJobResponseTypeDef,
     CreatePackageImportJobResponseTypeDef,
     DeleteDeviceResponseTypeDef,
+    DescribeApplicationInstanceDetailsResponseTypeDef,
     DescribeApplicationInstanceResponseTypeDef,
     DescribeDeviceJobResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
     CreateNodeFromTemplateJobRequestRequestTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
-    DescribeApplicationInstanceDetailsResponseTypeDef,
     DeviceTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
     EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
@@ -416,30 +412,27 @@
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     NetworkStatusTypeDef,
     NodeInterfaceTypeDef,
     SignalApplicationInstanceNodeInstancesRequestRequestTypeDef,
     PackageImportJobOutputTypeDef,
-    PackageImportJobOutputConfigOutputTypeDef,
     PackageImportJobOutputConfigTypeDef,
-    PackageVersionInputConfigOutputTypeDef,
     PackageVersionInputConfigTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesResponseTypeDef,
     CreateJobForDevicesRequestRequestTypeDef,
     NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
     DescribeNodeResponseTypeDef,
-    PackageImportJobInputConfigOutputTypeDef,
     PackageImportJobInputConfigTypeDef,
     DescribeDeviceResponseTypeDef,
     ProvisionDeviceRequestRequestTypeDef,
-    DescribePackageImportJobResponseTypeDef,
     CreatePackageImportJobRequestRequestTypeDef,
+    DescribePackageImportJobResponseTypeDef,
 )
 
 
 def get_structure() -> AlternateSoftwareMetadataTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/SOURCES.txt` & `mypy-boto3-panorama-1.28.15/mypy_boto3_panorama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.12/setup.py` & `mypy-boto3-panorama-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-panorama",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_panorama"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Panorama 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Panorama 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

