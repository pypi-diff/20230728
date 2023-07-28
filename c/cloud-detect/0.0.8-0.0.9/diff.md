# Comparing `tmp/cloud-detect-0.0.8.tar.gz` & `tmp/cloud-detect-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloud-detect-0.0.8.tar", last modified: Mon Apr 25 08:46:22 2022, max compression
+gzip compressed data, was "dist/cloud-detect-0.0.9.tar", last modified: Mon Jul 11 12:47:25 2022, max compression
```

## Comparing `cloud-detect-0.0.8.tar` & `cloud-detect-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 dgzlopes  (1000) dgzlopes  (1000)        0 2022-04-25 08:46:22.895477 cloud-detect-0.0.8/
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     3738 2022-04-25 08:46:22.891477 cloud-detect-0.0.8/PKG-INFO
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     2405 2022-04-25 08:44:20.000000 cloud-detect-0.0.8/README.md
-drwxrwxr-x   0 dgzlopes  (1000) dgzlopes  (1000)        0 2022-04-25 08:46:22.891477 cloud-detect-0.0.8/cloud_detect/
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     3523 2022-04-25 08:45:22.000000 cloud-detect-0.0.8/cloud_detect/__init__.py
-drwxrwxr-x   0 dgzlopes  (1000) dgzlopes  (1000)        0 2022-04-25 08:46:22.891477 cloud-detect-0.0.8/cloud_detect/providers/
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)      445 2022-04-25 08:45:22.000000 cloud-detect-0.0.8/cloud_detect/providers/__init__.py
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1627 2022-04-25 08:45:22.000000 cloud-detect-0.0.8/cloud_detect/providers/alibaba_provider.py
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1777 2022-04-25 08:45:22.000000 cloud-detect-0.0.8/cloud_detect/providers/aws_provider.py
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1642 2022-04-25 08:45:22.000000 cloud-detect-0.0.8/cloud_detect/providers/azure_provider.py
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1563 2022-04-25 08:45:22.000000 cloud-detect-0.0.8/cloud_detect/providers/do_provider.py
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1601 2022-04-25 08:45:22.000000 cloud-detect-0.0.8/cloud_detect/providers/gcp_provider.py
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1085 2022-04-25 08:45:22.000000 cloud-detect-0.0.8/cloud_detect/providers/oci_provider.py
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)      507 2022-04-25 08:45:22.000000 cloud-detect-0.0.8/cloud_detect/providers/provider.py
-drwxrwxr-x   0 dgzlopes  (1000) dgzlopes  (1000)        0 2022-04-25 08:46:22.891477 cloud-detect-0.0.8/cloud_detect.egg-info/
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     3738 2022-04-25 08:46:22.000000 cloud-detect-0.0.8/cloud_detect.egg-info/PKG-INFO
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)      531 2022-04-25 08:46:22.000000 cloud-detect-0.0.8/cloud_detect.egg-info/SOURCES.txt
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)        1 2022-04-25 08:46:22.000000 cloud-detect-0.0.8/cloud_detect.egg-info/dependency_links.txt
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)       13 2022-04-25 08:46:22.000000 cloud-detect-0.0.8/cloud_detect.egg-info/requires.txt
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)       13 2022-04-25 08:46:22.000000 cloud-detect-0.0.8/cloud_detect.egg-info/top_level.txt
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)       38 2022-04-25 08:46:22.895477 cloud-detect-0.0.8/setup.cfg
--rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1429 2022-04-25 08:46:01.000000 cloud-detect-0.0.8/setup.py
+drwxrwxr-x   0 dgzlopes  (1000) dgzlopes  (1000)        0 2022-07-11 12:47:25.044105 cloud-detect-0.0.9/
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     3738 2022-07-11 12:47:25.044105 cloud-detect-0.0.9/PKG-INFO
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     2405 2022-04-25 08:44:20.000000 cloud-detect-0.0.9/README.md
+drwxrwxr-x   0 dgzlopes  (1000) dgzlopes  (1000)        0 2022-07-11 12:47:25.044105 cloud-detect-0.0.9/cloud_detect/
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     3523 2022-04-25 08:45:22.000000 cloud-detect-0.0.9/cloud_detect/__init__.py
+drwxrwxr-x   0 dgzlopes  (1000) dgzlopes  (1000)        0 2022-07-11 12:47:25.044105 cloud-detect-0.0.9/cloud_detect/providers/
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)      445 2022-04-25 08:45:22.000000 cloud-detect-0.0.9/cloud_detect/providers/__init__.py
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1621 2022-07-11 12:46:53.000000 cloud-detect-0.0.9/cloud_detect/providers/alibaba_provider.py
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1768 2022-07-11 12:46:53.000000 cloud-detect-0.0.9/cloud_detect/providers/aws_provider.py
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1632 2022-07-11 12:46:53.000000 cloud-detect-0.0.9/cloud_detect/providers/azure_provider.py
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1553 2022-07-11 12:46:53.000000 cloud-detect-0.0.9/cloud_detect/providers/do_provider.py
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1592 2022-07-11 12:46:53.000000 cloud-detect-0.0.9/cloud_detect/providers/gcp_provider.py
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1076 2022-07-11 12:46:53.000000 cloud-detect-0.0.9/cloud_detect/providers/oci_provider.py
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)      507 2022-04-25 08:45:22.000000 cloud-detect-0.0.9/cloud_detect/providers/provider.py
+drwxrwxr-x   0 dgzlopes  (1000) dgzlopes  (1000)        0 2022-07-11 12:47:25.044105 cloud-detect-0.0.9/cloud_detect.egg-info/
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     3738 2022-07-11 12:47:24.000000 cloud-detect-0.0.9/cloud_detect.egg-info/PKG-INFO
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)      531 2022-07-11 12:47:24.000000 cloud-detect-0.0.9/cloud_detect.egg-info/SOURCES.txt
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)        1 2022-07-11 12:47:24.000000 cloud-detect-0.0.9/cloud_detect.egg-info/dependency_links.txt
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)       13 2022-07-11 12:47:24.000000 cloud-detect-0.0.9/cloud_detect.egg-info/requires.txt
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)       13 2022-07-11 12:47:24.000000 cloud-detect-0.0.9/cloud_detect.egg-info/top_level.txt
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)       38 2022-07-11 12:47:25.044105 cloud-detect-0.0.9/setup.cfg
+-rw-rw-r--   0 dgzlopes  (1000) dgzlopes  (1000)     1429 2022-07-11 12:47:07.000000 cloud-detect-0.0.9/setup.py
```

### Comparing `cloud-detect-0.0.8/PKG-INFO` & `cloud-detect-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-detect
-Version: 0.0.8
+Version: 0.0.9
 Summary: Module that determines a host's cloud provider
 Home-page: https://github.com/dgzlopes/cloud-detect
 Author: Daniel Gonzalez Lopes
 Author-email: danielgonzalezlopes@gmail.com
 License: MIT
 Description: # cloud-detect
         [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cloud-detect.svg)](https://pypi.org/project/cloud-detect/)
```

### Comparing `cloud-detect-0.0.8/README.md` & `cloud-detect-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cloud-detect-0.0.8/cloud_detect/__init__.py` & `cloud-detect-0.0.9/cloud_detect/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-detect-0.0.8/cloud_detect/providers/alibaba_provider.py` & `cloud-detect-0.0.9/cloud_detect/providers/alibaba_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,13 +36,13 @@
         except BaseException:
             return False
 
     def check_vendor_file(self):
         """
             Tries to identify Alibaba provider by reading the /sys/class/dmi/id/product_name
         """
-        self.logger.debug('Checking Aliobaba vendor file')
+        self.logger.debug('Checking Alibaba vendor file')
         alibaba_path = Path(self.vendor_file)
         if alibaba_path.is_file():
-            if 'Alibaba Cloud ECS' in open(self.vendor_file).read():
+            if 'Alibaba Cloud ECS' in alibaba_path.read_text():
                 return True
         return False
```

### Comparing `cloud-detect-0.0.8/cloud_detect/providers/aws_provider.py` & `cloud-detect-0.0.9/cloud_detect/providers/azure_provider.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,54 +2,50 @@
 from pathlib import Path
 
 import aiohttp
 
 from . import AbstractProvider
 
 
-class AWSProvider(AbstractProvider):
+class AzureProvider(AbstractProvider):
     """
-        Concrete implementation of the AWS cloud provider.
+        Concrete implementation of the Azure cloud provider.
     """
-    identifier = 'aws'
+    identifier = 'azure'
 
     def __init__(self, logger=None):
         self.logger = logger or logging.getLogger(__name__)
         self.metadata_url = (
-            'http://169.254.169.254/latest/dynamic/instance-identity/document'
+            'http://169.254.169.254/metadata/instance?api-version=2017-12-01'
         )
-        self.vendor_file = '/sys/class/dmi/id/product_version'
+        self.vendor_file = '/sys/class/dmi/id/sys_vendor'
+        self.headers = {'Metadata': 'true'}
 
     async def identify(self):
         """
-            Tries to identify AWS using all the implemented options
+            Tries to identify Azure using all the implemented options
         """
-        self.logger.info('Try to identify AWS')
+        self.logger.info('Try to identify DO')
         return self.check_vendor_file() or await self.check_metadata_server()
 
     async def check_metadata_server(self):
         """
-            Tries to identify AWS via metadata server
+            Tries to identify Azure via metadata server
         """
-        self.logger.debug('Checking AWS metadata')
+        self.logger.debug('Checking Azure metadata')
         try:
             async with aiohttp.ClientSession() as session:
-                async with session.get(self.metadata_url) as response:
-                    response = await response.json()
-                    if response['imageId'].startswith('ami-',) and response[
-                        'instanceId'
-                    ].startswith('i-'):
-                        return True
-            return False
+                async with session.get(self.metadata_url, headers=self.headers) as response:
+                    return response.status == 200
         except BaseException:
             return False
 
     def check_vendor_file(self):
         """
-            Tries to identify AWS provider by reading the /sys/class/dmi/id/product_version
+            Tries to identify Azure provider by reading the /sys/class/dmi/id/sys_vendor
         """
-        self.logger.debug('Checking AWS vendor file')
-        aws_path = Path(self.vendor_file)
-        if aws_path.is_file():
-            if 'amazon' in open(self.vendor_file).read():
+        self.logger.debug('Checking Azure vendor file')
+        ms_path = Path(self.vendor_file)
+        if ms_path.is_file():
+            if 'Microsoft Corporation' in ms_path.read_text():
                 return True
         return False
```

### Comparing `cloud-detect-0.0.8/cloud_detect/providers/azure_provider.py` & `cloud-detect-0.0.9/cloud_detect/providers/do_provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,50 +2,48 @@
 from pathlib import Path
 
 import aiohttp
 
 from . import AbstractProvider
 
 
-class AzureProvider(AbstractProvider):
+class DOProvider(AbstractProvider):
     """
-        Concrete implementation of the Azure cloud provider.
+        Concrete implementation of the Digital Ocean cloud provider.
     """
-    identifier = 'azure'
+    identifier = 'do'
 
     def __init__(self, logger=None):
         self.logger = logger or logging.getLogger(__name__)
-        self.metadata_url = (
-            'http://169.254.169.254/metadata/instance?api-version=2017-12-01'
-        )
+        self.metadata_url = 'http://169.254.169.254/metadata/v1.json'
         self.vendor_file = '/sys/class/dmi/id/sys_vendor'
-        self.headers = {'Metadata': 'true'}
 
     async def identify(self):
         """
-            Tries to identify Azure using all the implemented options
+            Tries to identify DO using all the implemented options
         """
         self.logger.info('Try to identify DO')
         return self.check_vendor_file() or await self.check_metadata_server()
 
     async def check_metadata_server(self):
         """
-            Tries to identify Azure via metadata server
+            Tries to identify DO via metadata server
         """
-        self.logger.debug('Checking Azure metadata')
+        self.logger.debug('Checking DO metadata')
         try:
             async with aiohttp.ClientSession() as session:
-                async with session.get(self.metadata_url, headers=self.headers) as response:
-                    return response.status == 200
+                async with session.get(self.metadata_url) as response:
+                    response = await response.json()
+                    return response['droplet_id'] > 0
         except BaseException:
             return False
 
     def check_vendor_file(self):
         """
-            Tries to identify Azure provider by reading the /sys/class/dmi/id/sys_vendor
+            Tries to identify DO provider by reading the /sys/class/dmi/id/sys_vendor
         """
-        self.logger.debug('Checking Azure vendor file')
+        self.logger.debug('Checking DO vendor file')
         do_path = Path(self.vendor_file)
         if do_path.is_file():
-            if 'Microsoft Corporation' in open(self.vendor_file).read():
+            if 'DigitalOcean' in do_path.read_text():
                 return True
         return False
```

### Comparing `cloud-detect-0.0.8/cloud_detect/providers/do_provider.py` & `cloud-detect-0.0.9/cloud_detect/providers/gcp_provider.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,48 +2,50 @@
 from pathlib import Path
 
 import aiohttp
 
 from . import AbstractProvider
 
 
-class DOProvider(AbstractProvider):
+class GCPProvider(AbstractProvider):
     """
-        Concrete implementation of the Digital Ocean cloud provider.
+        Concrete implementation of the GCP cloud provider.
     """
-    identifier = 'do'
+    identifier = 'gcp'
 
     def __init__(self, logger=None):
         self.logger = logger or logging.getLogger(__name__)
-        self.metadata_url = 'http://169.254.169.254/metadata/v1.json'
-        self.vendor_file = '/sys/class/dmi/id/sys_vendor'
+        self.metadata_url = (
+            'http://metadata.google.internal/computeMetadata/v1/instance/tags'
+        )
+        self.vendor_file = '/sys/class/dmi/id/product_name'
+        self.headers = {'Metadata-Flavor': 'Google'}
 
     async def identify(self):
         """
-            Tries to identify DO using all the implemented options
+            Tries to identify GCP using all the implemented options
         """
-        self.logger.info('Try to identify DO')
+        self.logger.info('Try to identify GCP')
         return self.check_vendor_file() or await self.check_metadata_server()
 
     async def check_metadata_server(self):
         """
-            Tries to identify DO via metadata server
+            Tries to identify GCP via metadata server
         """
-        self.logger.debug('Checking DO metadata')
+        self.logger.debug('Checking GCP metadata')
         try:
             async with aiohttp.ClientSession() as session:
-                async with session.get(self.metadata_url) as response:
-                    response = await response.json()
-                    return response['droplet_id'] > 0
-        except BaseException:
+                async with session.get(self.metadata_url):
+                    return True
+        except aiohttp.ClientError as e:  # noqa: F841
             return False
 
     def check_vendor_file(self):
         """
-            Tries to identify DO provider by reading the /sys/class/dmi/id/sys_vendor
+            Tries to identify GCP provider by reading the /sys/class/dmi/id/product_name
         """
-        self.logger.debug('Checking DO vendor file')
-        do_path = Path(self.vendor_file)
-        if do_path.is_file():
-            if 'DigitalOcean' in open(self.vendor_file).read():
+        self.logger.debug('Checking GCP vendor file')
+        gcp_path = Path(self.vendor_file)
+        if gcp_path.is_file():
+            if 'Google' in gcp_path.read_text():
                 return True
         return False
```

### Comparing `cloud-detect-0.0.8/cloud_detect/providers/gcp_provider.py` & `cloud-detect-0.0.9/cloud_detect/providers/oci_provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,36 @@
 import logging
 from pathlib import Path
 
-import aiohttp
-
 from . import AbstractProvider
 
 
-class GCPProvider(AbstractProvider):
+class OCIProvider(AbstractProvider):
     """
-        Concrete implementation of the GCP cloud provider.
+        Concrete implementation of the Oracle Cloud Infrastructure cloud provider.
     """
-    identifier = 'gcp'
+    identifier = 'oci'
 
     def __init__(self, logger=None):
         self.logger = logger or logging.getLogger(__name__)
-        self.metadata_url = (
-            'http://metadata.google.internal/computeMetadata/v1/instance/tags'
-        )
-        self.vendor_file = '/sys/class/dmi/id/product_name'
-        self.headers = {'Metadata-Flavor': 'Google'}
+        self.vendor_file = '/sys/class/dmi/id/chassis_asset_tag'
 
     async def identify(self):
         """
-            Tries to identify GCP using all the implemented options
+            Tries to identify OCI using all the implemented options
         """
-        self.logger.info('Try to identify GCP')
-        return self.check_vendor_file() or await self.check_metadata_server()
+        self.logger.info('Try to identify OCI')
+        return self.check_vendor_file()
 
-    async def check_metadata_server(self):
-        """
-            Tries to identify GCP via metadata server
-        """
-        self.logger.debug('Checking GCP metadata')
-        try:
-            async with aiohttp.ClientSession() as session:
-                async with session.get(self.metadata_url):
-                    return True
-        except aiohttp.ClientError as e:  # noqa: F841
-            return False
+    def check_metadata_server(self):
+        raise NotImplementedError
 
     def check_vendor_file(self):
         """
-            Tries to identify GCP provider by reading the /sys/class/dmi/id/product_name
+            Tries to identify OCI provider by reading the file -> /sys/class/dmi/id/chassis_asset_tag # noqa
         """
-        self.logger.debug('Checking GCP vendor file')
-        gcp_path = Path(self.vendor_file)
-        if gcp_path.is_file():
-            if 'Google' in open(self.vendor_file).read():
+        self.logger.debug('Checking OCI vendor file')
+        oci_path = Path(self.vendor_file)
+        if oci_path.is_file():
+            if 'OracleCloud' in oci_path.read_text():
                 return True
         return False
```

### Comparing `cloud-detect-0.0.8/cloud_detect.egg-info/PKG-INFO` & `cloud-detect-0.0.9/cloud_detect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-detect
-Version: 0.0.8
+Version: 0.0.9
 Summary: Module that determines a host's cloud provider
 Home-page: https://github.com/dgzlopes/cloud-detect
 Author: Daniel Gonzalez Lopes
 Author-email: danielgonzalezlopes@gmail.com
 License: MIT
 Description: # cloud-detect
         [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cloud-detect.svg)](https://pypi.org/project/cloud-detect/)
```

### Comparing `cloud-detect-0.0.8/cloud_detect.egg-info/SOURCES.txt` & `cloud-detect-0.0.9/cloud_detect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-detect-0.0.8/setup.py` & `cloud-detect-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 if py_version.minor >= 7:
     install_requires = ['aiohttp>=3.7']
 else:
     install_requires = ['aiohttp>=3.7,<4']
 
 setup(
     name='cloud-detect',
-    version='0.0.8',
+    version='0.0.9',
     description="Module that determines a host's cloud provider",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dgzlopes/cloud-detect',
     license='MIT',
     install_requires=install_requires,
     classifiers=[
```

