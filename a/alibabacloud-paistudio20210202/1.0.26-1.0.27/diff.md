# Comparing `tmp/alibabacloud_paistudio20210202-1.0.26.tar.gz` & `tmp/alibabacloud_paistudio20210202-1.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_paistudio20210202-1.0.26.tar", last modified: Thu Jun 30 07:36:18 2022, max compression
+gzip compressed data, was "dist/alibabacloud_paistudio20210202-1.0.27.tar", last modified: Fri Jul 28 02:02:46 2023, max compression
```

## Comparing `alibabacloud_paistudio20210202-1.0.26.tar` & `alibabacloud_paistudio20210202-1.0.27.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/
--rw-r--r--   0 root         (0) root         (0)      213 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2365 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/alibabacloud_paistudio20210202/
--rw-r--r--   0 root         (0) root         (0)       22 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/alibabacloud_paistudio20210202/__init__.py
--rw-r--r--   0 root         (0) root         (0)   172312 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/alibabacloud_paistudio20210202/client.py
--rw-r--r--   0 root         (0) root         (0)   230017 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/alibabacloud_paistudio20210202/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/alibabacloud_paistudio20210202.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2365 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/alibabacloud_paistudio20210202.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/alibabacloud_paistudio20210202.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/alibabacloud_paistudio20210202.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/alibabacloud_paistudio20210202.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/alibabacloud_paistudio20210202.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2022-06-30 07:36:18.000000 alibabacloud_paistudio20210202-1.0.26/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/alibabacloud_paistudio20210202/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/alibabacloud_paistudio20210202/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161052 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/alibabacloud_paistudio20210202/client.py
+-rw-r--r--   0 root         (0) root         (0)   217843 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/alibabacloud_paistudio20210202/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/alibabacloud_paistudio20210202.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/alibabacloud_paistudio20210202.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/alibabacloud_paistudio20210202.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/alibabacloud_paistudio20210202.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/alibabacloud_paistudio20210202.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/alibabacloud_paistudio20210202.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-07-28 02:02:46.000000 alibabacloud_paistudio20210202-1.0.27/setup.py
```

### Comparing `alibabacloud_paistudio20210202-1.0.26/LICENSE` & `alibabacloud_paistudio20210202-1.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_paistudio20210202-1.0.26/PKG-INFO` & `alibabacloud_paistudio20210202-1.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_paistudio20210202
-Version: 1.0.26
+Version: 1.0.27
 Summary: Alibaba Cloud PaiStudio (20210202) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_paistudio20210202-1.0.26/README-CN.md` & `alibabacloud_paistudio20210202-1.0.27/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_paistudio20210202-1.0.26/README.md` & `alibabacloud_paistudio20210202-1.0.27/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_paistudio20210202-1.0.26/alibabacloud_paistudio20210202/client.py` & `alibabacloud_paistudio20210202-1.0.27/alibabacloud_paistudio20210202/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,30 +55,14 @@
     ) -> str:
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
-    def add_image(
-        self,
-        request: pai_studio_20210202_models.AddImageRequest,
-    ) -> pai_studio_20210202_models.AddImageResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.add_image_with_options(request, headers, runtime)
-
-    async def add_image_async(
-        self,
-        request: pai_studio_20210202_models.AddImageRequest,
-    ) -> pai_studio_20210202_models.AddImageResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.add_image_with_options_async(request, headers, runtime)
-
     def add_image_with_options(
         self,
         request: pai_studio_20210202_models.AddImageRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.AddImageResponse:
         UtilClient.validate_model(request)
@@ -143,53 +127,50 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.AddImageResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def add_image_labels(
+    def add_image(
         self,
-        image_id: str,
-        request: pai_studio_20210202_models.AddImageLabelsRequest,
-    ) -> pai_studio_20210202_models.AddImageLabelsResponse:
+        request: pai_studio_20210202_models.AddImageRequest,
+    ) -> pai_studio_20210202_models.AddImageResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.add_image_labels_with_options(image_id, request, headers, runtime)
+        return self.add_image_with_options(request, headers, runtime)
 
-    async def add_image_labels_async(
+    async def add_image_async(
         self,
-        image_id: str,
-        request: pai_studio_20210202_models.AddImageLabelsRequest,
-    ) -> pai_studio_20210202_models.AddImageLabelsResponse:
+        request: pai_studio_20210202_models.AddImageRequest,
+    ) -> pai_studio_20210202_models.AddImageResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.add_image_labels_with_options_async(image_id, request, headers, runtime)
+        return await self.add_image_with_options_async(request, headers, runtime)
 
     def add_image_labels_with_options(
         self,
         image_id: str,
         request: pai_studio_20210202_models.AddImageLabelsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.AddImageLabelsResponse:
         UtilClient.validate_model(request)
-        image_id = OpenApiUtilClient.get_encode_param(image_id)
         body = {}
         if not UtilClient.is_unset(request.labels):
             body['Labels'] = request.labels
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='AddImageLabels',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/images/{image_id}/labels',
+            pathname=f'/api/v1/images/{OpenApiUtilClient.get_encode_param(image_id)}/labels',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -201,65 +182,63 @@
         self,
         image_id: str,
         request: pai_studio_20210202_models.AddImageLabelsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.AddImageLabelsResponse:
         UtilClient.validate_model(request)
-        image_id = OpenApiUtilClient.get_encode_param(image_id)
         body = {}
         if not UtilClient.is_unset(request.labels):
             body['Labels'] = request.labels
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='AddImageLabels',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/images/{image_id}/labels',
+            pathname=f'/api/v1/images/{OpenApiUtilClient.get_encode_param(image_id)}/labels',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.AddImageLabelsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def copy_experiment(
+    def add_image_labels(
         self,
-        experiment_id: str,
-        request: pai_studio_20210202_models.CopyExperimentRequest,
-    ) -> pai_studio_20210202_models.CopyExperimentResponse:
+        image_id: str,
+        request: pai_studio_20210202_models.AddImageLabelsRequest,
+    ) -> pai_studio_20210202_models.AddImageLabelsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.copy_experiment_with_options(experiment_id, request, headers, runtime)
+        return self.add_image_labels_with_options(image_id, request, headers, runtime)
 
-    async def copy_experiment_async(
+    async def add_image_labels_async(
         self,
-        experiment_id: str,
-        request: pai_studio_20210202_models.CopyExperimentRequest,
-    ) -> pai_studio_20210202_models.CopyExperimentResponse:
+        image_id: str,
+        request: pai_studio_20210202_models.AddImageLabelsRequest,
+    ) -> pai_studio_20210202_models.AddImageLabelsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.copy_experiment_with_options_async(experiment_id, request, headers, runtime)
+        return await self.add_image_labels_with_options_async(image_id, request, headers, runtime)
 
     def copy_experiment_with_options(
         self,
         experiment_id: str,
         request: pai_studio_20210202_models.CopyExperimentRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.CopyExperimentResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         body = {}
         if not UtilClient.is_unset(request.accessibility):
             body['Accessibility'] = request.accessibility
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.folder_id):
             body['FolderId'] = request.folder_id
@@ -273,15 +252,15 @@
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CopyExperiment',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/[ExperimentId]/copy',
+            pathname=f'/api/v1/experiments/%5BExperimentId%5D/copy',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -293,15 +272,14 @@
         self,
         experiment_id: str,
         request: pai_studio_20210202_models.CopyExperimentRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.CopyExperimentResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         body = {}
         if not UtilClient.is_unset(request.accessibility):
             body['Accessibility'] = request.accessibility
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.folder_id):
             body['FolderId'] = request.folder_id
@@ -315,41 +293,43 @@
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CopyExperiment',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/[ExperimentId]/copy',
+            pathname=f'/api/v1/experiments/%5BExperimentId%5D/copy',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.CopyExperimentResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def create_experiment(
+    def copy_experiment(
         self,
-        request: pai_studio_20210202_models.CreateExperimentRequest,
-    ) -> pai_studio_20210202_models.CreateExperimentResponse:
+        experiment_id: str,
+        request: pai_studio_20210202_models.CopyExperimentRequest,
+    ) -> pai_studio_20210202_models.CopyExperimentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.create_experiment_with_options(request, headers, runtime)
+        return self.copy_experiment_with_options(experiment_id, request, headers, runtime)
 
-    async def create_experiment_async(
+    async def copy_experiment_async(
         self,
-        request: pai_studio_20210202_models.CreateExperimentRequest,
-    ) -> pai_studio_20210202_models.CreateExperimentResponse:
+        experiment_id: str,
+        request: pai_studio_20210202_models.CopyExperimentRequest,
+    ) -> pai_studio_20210202_models.CopyExperimentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.create_experiment_with_options_async(request, headers, runtime)
+        return await self.copy_experiment_with_options_async(experiment_id, request, headers, runtime)
 
     def create_experiment_with_options(
         self,
         request: pai_studio_20210202_models.CreateExperimentRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.CreateExperimentResponse:
@@ -431,29 +411,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.CreateExperimentResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def create_experiment_folder(
+    def create_experiment(
         self,
-        request: pai_studio_20210202_models.CreateExperimentFolderRequest,
-    ) -> pai_studio_20210202_models.CreateExperimentFolderResponse:
+        request: pai_studio_20210202_models.CreateExperimentRequest,
+    ) -> pai_studio_20210202_models.CreateExperimentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.create_experiment_folder_with_options(request, headers, runtime)
+        return self.create_experiment_with_options(request, headers, runtime)
 
-    async def create_experiment_folder_async(
+    async def create_experiment_async(
         self,
-        request: pai_studio_20210202_models.CreateExperimentFolderRequest,
-    ) -> pai_studio_20210202_models.CreateExperimentFolderResponse:
+        request: pai_studio_20210202_models.CreateExperimentRequest,
+    ) -> pai_studio_20210202_models.CreateExperimentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.create_experiment_folder_with_options_async(request, headers, runtime)
+        return await self.create_experiment_with_options_async(request, headers, runtime)
 
     def create_experiment_folder_with_options(
         self,
         request: pai_studio_20210202_models.CreateExperimentFolderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.CreateExperimentFolderResponse:
@@ -523,29 +503,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.CreateExperimentFolderResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def create_experiment_migrate_validation(
+    def create_experiment_folder(
         self,
-        request: pai_studio_20210202_models.CreateExperimentMigrateValidationRequest,
-    ) -> pai_studio_20210202_models.CreateExperimentMigrateValidationResponse:
+        request: pai_studio_20210202_models.CreateExperimentFolderRequest,
+    ) -> pai_studio_20210202_models.CreateExperimentFolderResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.create_experiment_migrate_validation_with_options(request, headers, runtime)
+        return self.create_experiment_folder_with_options(request, headers, runtime)
 
-    async def create_experiment_migrate_validation_async(
+    async def create_experiment_folder_async(
         self,
-        request: pai_studio_20210202_models.CreateExperimentMigrateValidationRequest,
-    ) -> pai_studio_20210202_models.CreateExperimentMigrateValidationResponse:
+        request: pai_studio_20210202_models.CreateExperimentFolderRequest,
+    ) -> pai_studio_20210202_models.CreateExperimentFolderResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.create_experiment_migrate_validation_with_options_async(request, headers, runtime)
+        return await self.create_experiment_folder_with_options_async(request, headers, runtime)
 
     def create_experiment_migrate_validation_with_options(
         self,
         request: pai_studio_20210202_models.CreateExperimentMigrateValidationRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.CreateExperimentMigrateValidationResponse:
@@ -599,29 +579,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.CreateExperimentMigrateValidationResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def create_job(
+    def create_experiment_migrate_validation(
         self,
-        request: pai_studio_20210202_models.CreateJobRequest,
-    ) -> pai_studio_20210202_models.CreateJobResponse:
+        request: pai_studio_20210202_models.CreateExperimentMigrateValidationRequest,
+    ) -> pai_studio_20210202_models.CreateExperimentMigrateValidationResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.create_job_with_options(request, headers, runtime)
+        return self.create_experiment_migrate_validation_with_options(request, headers, runtime)
 
-    async def create_job_async(
+    async def create_experiment_migrate_validation_async(
         self,
-        request: pai_studio_20210202_models.CreateJobRequest,
-    ) -> pai_studio_20210202_models.CreateJobResponse:
+        request: pai_studio_20210202_models.CreateExperimentMigrateValidationRequest,
+    ) -> pai_studio_20210202_models.CreateExperimentMigrateValidationResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.create_job_with_options_async(request, headers, runtime)
+        return await self.create_experiment_migrate_validation_with_options_async(request, headers, runtime)
 
     def create_job_with_options(
         self,
         request: pai_studio_20210202_models.CreateJobRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.CreateJobResponse:
@@ -687,125 +667,44 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.CreateJobResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def create_service(
-        self,
-        request: pai_studio_20210202_models.CreateServiceRequest,
-    ) -> pai_studio_20210202_models.CreateServiceResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.create_service_with_options(request, headers, runtime)
-
-    async def create_service_async(
-        self,
-        request: pai_studio_20210202_models.CreateServiceRequest,
-    ) -> pai_studio_20210202_models.CreateServiceResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.create_service_with_options_async(request, headers, runtime)
-
-    def create_service_with_options(
-        self,
-        request: pai_studio_20210202_models.CreateServiceRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> pai_studio_20210202_models.CreateServiceResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.config):
-            body['Config'] = request.config
-        if not UtilClient.is_unset(request.service_type):
-            body['ServiceType'] = request.service_type
-        req = open_api_models.OpenApiRequest(
-            headers=headers,
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='CreateService',
-            version='2021-02-02',
-            protocol='HTTPS',
-            pathname=f'/api/v1/services',
-            method='POST',
-            auth_type='AK',
-            style='ROA',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            pai_studio_20210202_models.CreateServiceResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def create_service_with_options_async(
-        self,
-        request: pai_studio_20210202_models.CreateServiceRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> pai_studio_20210202_models.CreateServiceResponse:
-        UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.config):
-            body['Config'] = request.config
-        if not UtilClient.is_unset(request.service_type):
-            body['ServiceType'] = request.service_type
-        req = open_api_models.OpenApiRequest(
-            headers=headers,
-            body=OpenApiUtilClient.parse_to_map(body)
-        )
-        params = open_api_models.Params(
-            action='CreateService',
-            version='2021-02-02',
-            protocol='HTTPS',
-            pathname=f'/api/v1/services',
-            method='POST',
-            auth_type='AK',
-            style='ROA',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            pai_studio_20210202_models.CreateServiceResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def delete_experiment(
+    def create_job(
         self,
-        experiment_id: str,
-    ) -> pai_studio_20210202_models.DeleteExperimentResponse:
+        request: pai_studio_20210202_models.CreateJobRequest,
+    ) -> pai_studio_20210202_models.CreateJobResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.delete_experiment_with_options(experiment_id, headers, runtime)
+        return self.create_job_with_options(request, headers, runtime)
 
-    async def delete_experiment_async(
+    async def create_job_async(
         self,
-        experiment_id: str,
-    ) -> pai_studio_20210202_models.DeleteExperimentResponse:
+        request: pai_studio_20210202_models.CreateJobRequest,
+    ) -> pai_studio_20210202_models.CreateJobResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.delete_experiment_with_options_async(experiment_id, headers, runtime)
+        return await self.create_job_with_options_async(request, headers, runtime)
 
     def delete_experiment_with_options(
         self,
         experiment_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.DeleteExperimentResponse:
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteExperiment',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}',
             method='DELETE',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -815,65 +714,63 @@
 
     async def delete_experiment_with_options_async(
         self,
         experiment_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.DeleteExperimentResponse:
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteExperiment',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}',
             method='DELETE',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.DeleteExperimentResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def delete_experiment_folder(
+    def delete_experiment(
         self,
-        folder_id: str,
-    ) -> pai_studio_20210202_models.DeleteExperimentFolderResponse:
+        experiment_id: str,
+    ) -> pai_studio_20210202_models.DeleteExperimentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.delete_experiment_folder_with_options(folder_id, headers, runtime)
+        return self.delete_experiment_with_options(experiment_id, headers, runtime)
 
-    async def delete_experiment_folder_async(
+    async def delete_experiment_async(
         self,
-        folder_id: str,
-    ) -> pai_studio_20210202_models.DeleteExperimentFolderResponse:
+        experiment_id: str,
+    ) -> pai_studio_20210202_models.DeleteExperimentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.delete_experiment_folder_with_options_async(folder_id, headers, runtime)
+        return await self.delete_experiment_with_options_async(experiment_id, headers, runtime)
 
     def delete_experiment_folder_with_options(
         self,
         folder_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.DeleteExperimentFolderResponse:
-        folder_id = OpenApiUtilClient.get_encode_param(folder_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteExperimentFolder',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experimentfolders/{folder_id}',
+            pathname=f'/api/v1/experimentfolders/{OpenApiUtilClient.get_encode_param(folder_id)}',
             method='DELETE',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -883,117 +780,48 @@
 
     async def delete_experiment_folder_with_options_async(
         self,
         folder_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.DeleteExperimentFolderResponse:
-        folder_id = OpenApiUtilClient.get_encode_param(folder_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteExperimentFolder',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experimentfolders/{folder_id}',
+            pathname=f'/api/v1/experimentfolders/{OpenApiUtilClient.get_encode_param(folder_id)}',
             method='DELETE',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.DeleteExperimentFolderResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def delete_service(
-        self,
-        service_id: str,
-    ) -> pai_studio_20210202_models.DeleteServiceResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.delete_service_with_options(service_id, headers, runtime)
-
-    async def delete_service_async(
-        self,
-        service_id: str,
-    ) -> pai_studio_20210202_models.DeleteServiceResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.delete_service_with_options_async(service_id, headers, runtime)
-
-    def delete_service_with_options(
-        self,
-        service_id: str,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> pai_studio_20210202_models.DeleteServiceResponse:
-        service_id = OpenApiUtilClient.get_encode_param(service_id)
-        req = open_api_models.OpenApiRequest(
-            headers=headers
-        )
-        params = open_api_models.Params(
-            action='DeleteService',
-            version='2021-02-02',
-            protocol='HTTPS',
-            pathname=f'/api/v1/services/{service_id}',
-            method='DELETE',
-            auth_type='AK',
-            style='ROA',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            pai_studio_20210202_models.DeleteServiceResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def delete_service_with_options_async(
-        self,
-        service_id: str,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> pai_studio_20210202_models.DeleteServiceResponse:
-        service_id = OpenApiUtilClient.get_encode_param(service_id)
-        req = open_api_models.OpenApiRequest(
-            headers=headers
-        )
-        params = open_api_models.Params(
-            action='DeleteService',
-            version='2021-02-02',
-            protocol='HTTPS',
-            pathname=f'/api/v1/services/{service_id}',
-            method='DELETE',
-            auth_type='AK',
-            style='ROA',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            pai_studio_20210202_models.DeleteServiceResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def get_algo_tree(
+    def delete_experiment_folder(
         self,
-        request: pai_studio_20210202_models.GetAlgoTreeRequest,
-    ) -> pai_studio_20210202_models.GetAlgoTreeResponse:
+        folder_id: str,
+    ) -> pai_studio_20210202_models.DeleteExperimentFolderResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_algo_tree_with_options(request, headers, runtime)
+        return self.delete_experiment_folder_with_options(folder_id, headers, runtime)
 
-    async def get_algo_tree_async(
+    async def delete_experiment_folder_async(
         self,
-        request: pai_studio_20210202_models.GetAlgoTreeRequest,
-    ) -> pai_studio_20210202_models.GetAlgoTreeResponse:
+        folder_id: str,
+    ) -> pai_studio_20210202_models.DeleteExperimentFolderResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_algo_tree_with_options_async(request, headers, runtime)
+        return await self.delete_experiment_folder_with_options_async(folder_id, headers, runtime)
 
     def get_algo_tree_with_options(
         self,
         request: pai_studio_20210202_models.GetAlgoTreeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetAlgoTreeResponse:
@@ -1047,29 +875,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetAlgoTreeResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_algorithm_def(
+    def get_algo_tree(
         self,
-        request: pai_studio_20210202_models.GetAlgorithmDefRequest,
-    ) -> pai_studio_20210202_models.GetAlgorithmDefResponse:
+        request: pai_studio_20210202_models.GetAlgoTreeRequest,
+    ) -> pai_studio_20210202_models.GetAlgoTreeResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_algorithm_def_with_options(request, headers, runtime)
+        return self.get_algo_tree_with_options(request, headers, runtime)
 
-    async def get_algorithm_def_async(
+    async def get_algo_tree_async(
         self,
-        request: pai_studio_20210202_models.GetAlgorithmDefRequest,
-    ) -> pai_studio_20210202_models.GetAlgorithmDefResponse:
+        request: pai_studio_20210202_models.GetAlgoTreeRequest,
+    ) -> pai_studio_20210202_models.GetAlgoTreeResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_algorithm_def_with_options_async(request, headers, runtime)
+        return await self.get_algo_tree_with_options_async(request, headers, runtime)
 
     def get_algorithm_def_with_options(
         self,
         request: pai_studio_20210202_models.GetAlgorithmDefRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetAlgorithmDefResponse:
@@ -1135,29 +963,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetAlgorithmDefResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_algorithm_defs(
+    def get_algorithm_def(
         self,
-        request: pai_studio_20210202_models.GetAlgorithmDefsRequest,
-    ) -> pai_studio_20210202_models.GetAlgorithmDefsResponse:
+        request: pai_studio_20210202_models.GetAlgorithmDefRequest,
+    ) -> pai_studio_20210202_models.GetAlgorithmDefResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_algorithm_defs_with_options(request, headers, runtime)
+        return self.get_algorithm_def_with_options(request, headers, runtime)
 
-    async def get_algorithm_defs_async(
+    async def get_algorithm_def_async(
         self,
-        request: pai_studio_20210202_models.GetAlgorithmDefsRequest,
-    ) -> pai_studio_20210202_models.GetAlgorithmDefsResponse:
+        request: pai_studio_20210202_models.GetAlgorithmDefRequest,
+    ) -> pai_studio_20210202_models.GetAlgorithmDefResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_algorithm_defs_with_options_async(request, headers, runtime)
+        return await self.get_algorithm_def_with_options_async(request, headers, runtime)
 
     def get_algorithm_defs_with_options(
         self,
         request: pai_studio_20210202_models.GetAlgorithmDefsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetAlgorithmDefsResponse:
@@ -1223,40 +1051,42 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetAlgorithmDefsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_algorithm_tree(
+    def get_algorithm_defs(
         self,
-        request: pai_studio_20210202_models.GetAlgorithmTreeRequest,
-    ) -> pai_studio_20210202_models.GetAlgorithmTreeResponse:
+        request: pai_studio_20210202_models.GetAlgorithmDefsRequest,
+    ) -> pai_studio_20210202_models.GetAlgorithmDefsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_algorithm_tree_with_options(request, headers, runtime)
+        return self.get_algorithm_defs_with_options(request, headers, runtime)
 
-    async def get_algorithm_tree_async(
+    async def get_algorithm_defs_async(
         self,
-        request: pai_studio_20210202_models.GetAlgorithmTreeRequest,
-    ) -> pai_studio_20210202_models.GetAlgorithmTreeResponse:
+        request: pai_studio_20210202_models.GetAlgorithmDefsRequest,
+    ) -> pai_studio_20210202_models.GetAlgorithmDefsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_algorithm_tree_with_options_async(request, headers, runtime)
+        return await self.get_algorithm_defs_with_options_async(request, headers, runtime)
 
     def get_algorithm_tree_with_options(
         self,
         request: pai_studio_20210202_models.GetAlgorithmTreeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetAlgorithmTreeResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.source):
             query['Source'] = request.source
+        if not UtilClient.is_unset(request.workspace_id):
+            query['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAlgorithmTree',
             version='2021-02-02',
@@ -1279,14 +1109,16 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetAlgorithmTreeResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.source):
             query['Source'] = request.source
+        if not UtilClient.is_unset(request.workspace_id):
+            query['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetAlgorithmTree',
             version='2021-02-02',
@@ -1299,45 +1131,44 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetAlgorithmTreeResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_experiment(
+    def get_algorithm_tree(
         self,
-        experiment_id: str,
-    ) -> pai_studio_20210202_models.GetExperimentResponse:
+        request: pai_studio_20210202_models.GetAlgorithmTreeRequest,
+    ) -> pai_studio_20210202_models.GetAlgorithmTreeResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_experiment_with_options(experiment_id, headers, runtime)
+        return self.get_algorithm_tree_with_options(request, headers, runtime)
 
-    async def get_experiment_async(
+    async def get_algorithm_tree_async(
         self,
-        experiment_id: str,
-    ) -> pai_studio_20210202_models.GetExperimentResponse:
+        request: pai_studio_20210202_models.GetAlgorithmTreeRequest,
+    ) -> pai_studio_20210202_models.GetAlgorithmTreeResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_experiment_with_options_async(experiment_id, headers, runtime)
+        return await self.get_algorithm_tree_with_options_async(request, headers, runtime)
 
     def get_experiment_with_options(
         self,
         experiment_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetExperimentResponse:
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetExperiment',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -1347,61 +1178,57 @@
 
     async def get_experiment_with_options_async(
         self,
         experiment_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetExperimentResponse:
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetExperiment',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetExperimentResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_experiment_folder_children(
+    def get_experiment(
         self,
-        folder_id: str,
-        request: pai_studio_20210202_models.GetExperimentFolderChildrenRequest,
-    ) -> pai_studio_20210202_models.GetExperimentFolderChildrenResponse:
+        experiment_id: str,
+    ) -> pai_studio_20210202_models.GetExperimentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_experiment_folder_children_with_options(folder_id, request, headers, runtime)
+        return self.get_experiment_with_options(experiment_id, headers, runtime)
 
-    async def get_experiment_folder_children_async(
+    async def get_experiment_async(
         self,
-        folder_id: str,
-        request: pai_studio_20210202_models.GetExperimentFolderChildrenRequest,
-    ) -> pai_studio_20210202_models.GetExperimentFolderChildrenResponse:
+        experiment_id: str,
+    ) -> pai_studio_20210202_models.GetExperimentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_experiment_folder_children_with_options_async(folder_id, request, headers, runtime)
+        return await self.get_experiment_with_options_async(experiment_id, headers, runtime)
 
     def get_experiment_folder_children_with_options(
         self,
         folder_id: str,
         request: pai_studio_20210202_models.GetExperimentFolderChildrenRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetExperimentFolderChildrenResponse:
         UtilClient.validate_model(request)
-        folder_id = OpenApiUtilClient.get_encode_param(folder_id)
         query = {}
         if not UtilClient.is_unset(request.accessibility):
             query['Accessibility'] = request.accessibility
         if not UtilClient.is_unset(request.only_folder):
             query['OnlyFolder'] = request.only_folder
         if not UtilClient.is_unset(request.source):
             query['Source'] = request.source
@@ -1413,15 +1240,15 @@
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetExperimentFolderChildren',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experimentfolders/{folder_id}/children',
+            pathname=f'/api/v1/experimentfolders/{OpenApiUtilClient.get_encode_param(folder_id)}/children',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -1433,15 +1260,14 @@
         self,
         folder_id: str,
         request: pai_studio_20210202_models.GetExperimentFolderChildrenRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetExperimentFolderChildrenResponse:
         UtilClient.validate_model(request)
-        folder_id = OpenApiUtilClient.get_encode_param(folder_id)
         query = {}
         if not UtilClient.is_unset(request.accessibility):
             query['Accessibility'] = request.accessibility
         if not UtilClient.is_unset(request.only_folder):
             query['OnlyFolder'] = request.only_folder
         if not UtilClient.is_unset(request.source):
             query['Source'] = request.source
@@ -1453,57 +1279,58 @@
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetExperimentFolderChildren',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experimentfolders/{folder_id}/children',
+            pathname=f'/api/v1/experimentfolders/{OpenApiUtilClient.get_encode_param(folder_id)}/children',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetExperimentFolderChildrenResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_experiment_meta(
+    def get_experiment_folder_children(
         self,
-        experiment_id: str,
-    ) -> pai_studio_20210202_models.GetExperimentMetaResponse:
+        folder_id: str,
+        request: pai_studio_20210202_models.GetExperimentFolderChildrenRequest,
+    ) -> pai_studio_20210202_models.GetExperimentFolderChildrenResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_experiment_meta_with_options(experiment_id, headers, runtime)
+        return self.get_experiment_folder_children_with_options(folder_id, request, headers, runtime)
 
-    async def get_experiment_meta_async(
+    async def get_experiment_folder_children_async(
         self,
-        experiment_id: str,
-    ) -> pai_studio_20210202_models.GetExperimentMetaResponse:
+        folder_id: str,
+        request: pai_studio_20210202_models.GetExperimentFolderChildrenRequest,
+    ) -> pai_studio_20210202_models.GetExperimentFolderChildrenResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_experiment_meta_with_options_async(experiment_id, headers, runtime)
+        return await self.get_experiment_folder_children_with_options_async(folder_id, request, headers, runtime)
 
     def get_experiment_meta_with_options(
         self,
         experiment_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetExperimentMetaResponse:
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetExperimentMeta',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/meta',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/meta',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -1513,65 +1340,63 @@
 
     async def get_experiment_meta_with_options_async(
         self,
         experiment_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetExperimentMetaResponse:
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetExperimentMeta',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/meta',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/meta',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetExperimentMetaResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_experiment_status(
+    def get_experiment_meta(
         self,
         experiment_id: str,
-    ) -> pai_studio_20210202_models.GetExperimentStatusResponse:
+    ) -> pai_studio_20210202_models.GetExperimentMetaResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_experiment_status_with_options(experiment_id, headers, runtime)
+        return self.get_experiment_meta_with_options(experiment_id, headers, runtime)
 
-    async def get_experiment_status_async(
+    async def get_experiment_meta_async(
         self,
         experiment_id: str,
-    ) -> pai_studio_20210202_models.GetExperimentStatusResponse:
+    ) -> pai_studio_20210202_models.GetExperimentMetaResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_experiment_status_with_options_async(experiment_id, headers, runtime)
+        return await self.get_experiment_meta_with_options_async(experiment_id, headers, runtime)
 
     def get_experiment_status_with_options(
         self,
         experiment_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetExperimentStatusResponse:
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetExperimentStatus',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/status',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/status',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -1581,73 +1406,69 @@
 
     async def get_experiment_status_with_options_async(
         self,
         experiment_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetExperimentStatusResponse:
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetExperimentStatus',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/status',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/status',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetExperimentStatusResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_experiment_visualization_meta(
+    def get_experiment_status(
         self,
         experiment_id: str,
-        request: pai_studio_20210202_models.GetExperimentVisualizationMetaRequest,
-    ) -> pai_studio_20210202_models.GetExperimentVisualizationMetaResponse:
+    ) -> pai_studio_20210202_models.GetExperimentStatusResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_experiment_visualization_meta_with_options(experiment_id, request, headers, runtime)
+        return self.get_experiment_status_with_options(experiment_id, headers, runtime)
 
-    async def get_experiment_visualization_meta_async(
+    async def get_experiment_status_async(
         self,
         experiment_id: str,
-        request: pai_studio_20210202_models.GetExperimentVisualizationMetaRequest,
-    ) -> pai_studio_20210202_models.GetExperimentVisualizationMetaResponse:
+    ) -> pai_studio_20210202_models.GetExperimentStatusResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_experiment_visualization_meta_with_options_async(experiment_id, request, headers, runtime)
+        return await self.get_experiment_status_with_options_async(experiment_id, headers, runtime)
 
     def get_experiment_visualization_meta_with_options(
         self,
         experiment_id: str,
         request: pai_studio_20210202_models.GetExperimentVisualizationMetaRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetExperimentVisualizationMetaResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         query = {}
         if not UtilClient.is_unset(request.node_ids):
             query['NodeIds'] = request.node_ids
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetExperimentVisualizationMeta',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/visualizationMeta',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/visualizationMeta',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -1659,53 +1480,54 @@
         self,
         experiment_id: str,
         request: pai_studio_20210202_models.GetExperimentVisualizationMetaRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetExperimentVisualizationMetaResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         query = {}
         if not UtilClient.is_unset(request.node_ids):
             query['NodeIds'] = request.node_ids
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetExperimentVisualizationMeta',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/visualizationMeta',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/visualizationMeta',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetExperimentVisualizationMetaResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_experiments_statistics(
+    def get_experiment_visualization_meta(
         self,
-        request: pai_studio_20210202_models.GetExperimentsStatisticsRequest,
-    ) -> pai_studio_20210202_models.GetExperimentsStatisticsResponse:
+        experiment_id: str,
+        request: pai_studio_20210202_models.GetExperimentVisualizationMetaRequest,
+    ) -> pai_studio_20210202_models.GetExperimentVisualizationMetaResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_experiments_statistics_with_options(request, headers, runtime)
+        return self.get_experiment_visualization_meta_with_options(experiment_id, request, headers, runtime)
 
-    async def get_experiments_statistics_async(
+    async def get_experiment_visualization_meta_async(
         self,
-        request: pai_studio_20210202_models.GetExperimentsStatisticsRequest,
-    ) -> pai_studio_20210202_models.GetExperimentsStatisticsResponse:
+        experiment_id: str,
+        request: pai_studio_20210202_models.GetExperimentVisualizationMetaRequest,
+    ) -> pai_studio_20210202_models.GetExperimentVisualizationMetaResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_experiments_statistics_with_options_async(request, headers, runtime)
+        return await self.get_experiment_visualization_meta_with_options_async(experiment_id, request, headers, runtime)
 
     def get_experiments_statistics_with_options(
         self,
         request: pai_studio_20210202_models.GetExperimentsStatisticsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetExperimentsStatisticsResponse:
@@ -1763,29 +1585,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetExperimentsStatisticsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_experiments_users_statistics(
+    def get_experiments_statistics(
         self,
-        request: pai_studio_20210202_models.GetExperimentsUsersStatisticsRequest,
-    ) -> pai_studio_20210202_models.GetExperimentsUsersStatisticsResponse:
+        request: pai_studio_20210202_models.GetExperimentsStatisticsRequest,
+    ) -> pai_studio_20210202_models.GetExperimentsStatisticsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_experiments_users_statistics_with_options(request, headers, runtime)
+        return self.get_experiments_statistics_with_options(request, headers, runtime)
 
-    async def get_experiments_users_statistics_async(
+    async def get_experiments_statistics_async(
         self,
-        request: pai_studio_20210202_models.GetExperimentsUsersStatisticsRequest,
-    ) -> pai_studio_20210202_models.GetExperimentsUsersStatisticsResponse:
+        request: pai_studio_20210202_models.GetExperimentsStatisticsRequest,
+    ) -> pai_studio_20210202_models.GetExperimentsStatisticsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_experiments_users_statistics_with_options_async(request, headers, runtime)
+        return await self.get_experiments_statistics_with_options_async(request, headers, runtime)
 
     def get_experiments_users_statistics_with_options(
         self,
         request: pai_studio_20210202_models.GetExperimentsUsersStatisticsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetExperimentsUsersStatisticsResponse:
@@ -1843,53 +1665,50 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetExperimentsUsersStatisticsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_image(
+    def get_experiments_users_statistics(
         self,
-        image_id: str,
-        request: pai_studio_20210202_models.GetImageRequest,
-    ) -> pai_studio_20210202_models.GetImageResponse:
+        request: pai_studio_20210202_models.GetExperimentsUsersStatisticsRequest,
+    ) -> pai_studio_20210202_models.GetExperimentsUsersStatisticsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_image_with_options(image_id, request, headers, runtime)
+        return self.get_experiments_users_statistics_with_options(request, headers, runtime)
 
-    async def get_image_async(
+    async def get_experiments_users_statistics_async(
         self,
-        image_id: str,
-        request: pai_studio_20210202_models.GetImageRequest,
-    ) -> pai_studio_20210202_models.GetImageResponse:
+        request: pai_studio_20210202_models.GetExperimentsUsersStatisticsRequest,
+    ) -> pai_studio_20210202_models.GetExperimentsUsersStatisticsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_image_with_options_async(image_id, request, headers, runtime)
+        return await self.get_experiments_users_statistics_with_options_async(request, headers, runtime)
 
     def get_image_with_options(
         self,
         image_id: str,
         request: pai_studio_20210202_models.GetImageRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetImageResponse:
         UtilClient.validate_model(request)
-        image_id = OpenApiUtilClient.get_encode_param(image_id)
         query = {}
         if not UtilClient.is_unset(request.verbose):
             query['Verbose'] = request.verbose
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetImage',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/images/{image_id}',
+            pathname=f'/api/v1/images/{OpenApiUtilClient.get_encode_param(image_id)}',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -1901,77 +1720,75 @@
         self,
         image_id: str,
         request: pai_studio_20210202_models.GetImageRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetImageResponse:
         UtilClient.validate_model(request)
-        image_id = OpenApiUtilClient.get_encode_param(image_id)
         query = {}
         if not UtilClient.is_unset(request.verbose):
             query['Verbose'] = request.verbose
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetImage',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/images/{image_id}',
+            pathname=f'/api/v1/images/{OpenApiUtilClient.get_encode_param(image_id)}',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetImageResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_job(
+    def get_image(
         self,
-        job_id: str,
-        request: pai_studio_20210202_models.GetJobRequest,
-    ) -> pai_studio_20210202_models.GetJobResponse:
+        image_id: str,
+        request: pai_studio_20210202_models.GetImageRequest,
+    ) -> pai_studio_20210202_models.GetImageResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_job_with_options(job_id, request, headers, runtime)
+        return self.get_image_with_options(image_id, request, headers, runtime)
 
-    async def get_job_async(
+    async def get_image_async(
         self,
-        job_id: str,
-        request: pai_studio_20210202_models.GetJobRequest,
-    ) -> pai_studio_20210202_models.GetJobResponse:
+        image_id: str,
+        request: pai_studio_20210202_models.GetImageRequest,
+    ) -> pai_studio_20210202_models.GetImageResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_job_with_options_async(job_id, request, headers, runtime)
+        return await self.get_image_with_options_async(image_id, request, headers, runtime)
 
     def get_job_with_options(
         self,
         job_id: str,
         request: pai_studio_20210202_models.GetJobRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetJobResponse:
         UtilClient.validate_model(request)
-        job_id = OpenApiUtilClient.get_encode_param(job_id)
         query = {}
         if not UtilClient.is_unset(request.verbose):
             query['Verbose'] = request.verbose
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetJob',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/jobs/{job_id}',
+            pathname=f'/api/v1/jobs/{OpenApiUtilClient.get_encode_param(job_id)}',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -1983,77 +1800,75 @@
         self,
         job_id: str,
         request: pai_studio_20210202_models.GetJobRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetJobResponse:
         UtilClient.validate_model(request)
-        job_id = OpenApiUtilClient.get_encode_param(job_id)
         query = {}
         if not UtilClient.is_unset(request.verbose):
             query['Verbose'] = request.verbose
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetJob',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/jobs/{job_id}',
+            pathname=f'/api/v1/jobs/{OpenApiUtilClient.get_encode_param(job_id)}',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetJobResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_mctable_schema(
+    def get_job(
         self,
-        table_name: str,
-        request: pai_studio_20210202_models.GetMCTableSchemaRequest,
-    ) -> pai_studio_20210202_models.GetMCTableSchemaResponse:
+        job_id: str,
+        request: pai_studio_20210202_models.GetJobRequest,
+    ) -> pai_studio_20210202_models.GetJobResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_mctable_schema_with_options(table_name, request, headers, runtime)
+        return self.get_job_with_options(job_id, request, headers, runtime)
 
-    async def get_mctable_schema_async(
+    async def get_job_async(
         self,
-        table_name: str,
-        request: pai_studio_20210202_models.GetMCTableSchemaRequest,
-    ) -> pai_studio_20210202_models.GetMCTableSchemaResponse:
+        job_id: str,
+        request: pai_studio_20210202_models.GetJobRequest,
+    ) -> pai_studio_20210202_models.GetJobResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_mctable_schema_with_options_async(table_name, request, headers, runtime)
+        return await self.get_job_with_options_async(job_id, request, headers, runtime)
 
     def get_mctable_schema_with_options(
         self,
         table_name: str,
         request: pai_studio_20210202_models.GetMCTableSchemaRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetMCTableSchemaResponse:
         UtilClient.validate_model(request)
-        table_name = OpenApiUtilClient.get_encode_param(table_name)
         query = {}
         if not UtilClient.is_unset(request.workspace_id):
             query['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetMCTableSchema',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/datasources/maxcompute/tables/{table_name}/schema',
+            pathname=f'/api/v1/datasources/maxcompute/tables/{OpenApiUtilClient.get_encode_param(table_name)}/schema',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -2065,83 +1880,78 @@
         self,
         table_name: str,
         request: pai_studio_20210202_models.GetMCTableSchemaRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetMCTableSchemaResponse:
         UtilClient.validate_model(request)
-        table_name = OpenApiUtilClient.get_encode_param(table_name)
         query = {}
         if not UtilClient.is_unset(request.workspace_id):
             query['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetMCTableSchema',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/datasources/maxcompute/tables/{table_name}/schema',
+            pathname=f'/api/v1/datasources/maxcompute/tables/{OpenApiUtilClient.get_encode_param(table_name)}/schema',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetMCTableSchemaResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_node_input_schema(
+    def get_mctable_schema(
         self,
-        experiment_id: str,
-        node_id: str,
-        request: pai_studio_20210202_models.GetNodeInputSchemaRequest,
-    ) -> pai_studio_20210202_models.GetNodeInputSchemaResponse:
+        table_name: str,
+        request: pai_studio_20210202_models.GetMCTableSchemaRequest,
+    ) -> pai_studio_20210202_models.GetMCTableSchemaResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_node_input_schema_with_options(experiment_id, node_id, request, headers, runtime)
+        return self.get_mctable_schema_with_options(table_name, request, headers, runtime)
 
-    async def get_node_input_schema_async(
+    async def get_mctable_schema_async(
         self,
-        experiment_id: str,
-        node_id: str,
-        request: pai_studio_20210202_models.GetNodeInputSchemaRequest,
-    ) -> pai_studio_20210202_models.GetNodeInputSchemaResponse:
+        table_name: str,
+        request: pai_studio_20210202_models.GetMCTableSchemaRequest,
+    ) -> pai_studio_20210202_models.GetMCTableSchemaResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_node_input_schema_with_options_async(experiment_id, node_id, request, headers, runtime)
+        return await self.get_mctable_schema_with_options_async(table_name, request, headers, runtime)
 
     def get_node_input_schema_with_options(
         self,
         experiment_id: str,
         node_id: str,
         request: pai_studio_20210202_models.GetNodeInputSchemaRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetNodeInputSchemaResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
-        node_id = OpenApiUtilClient.get_encode_param(node_id)
         query = {}
         if not UtilClient.is_unset(request.input_id):
             query['InputId'] = request.input_id
         if not UtilClient.is_unset(request.input_index):
             query['InputIndex'] = request.input_index
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetNodeInputSchema',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/nodes/{node_id}/schema',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/nodes/{OpenApiUtilClient.get_encode_param(node_id)}/schema',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -2154,88 +1964,81 @@
         experiment_id: str,
         node_id: str,
         request: pai_studio_20210202_models.GetNodeInputSchemaRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetNodeInputSchemaResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
-        node_id = OpenApiUtilClient.get_encode_param(node_id)
         query = {}
         if not UtilClient.is_unset(request.input_id):
             query['InputId'] = request.input_id
         if not UtilClient.is_unset(request.input_index):
             query['InputIndex'] = request.input_index
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetNodeInputSchema',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/nodes/{node_id}/schema',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/nodes/{OpenApiUtilClient.get_encode_param(node_id)}/schema',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetNodeInputSchemaResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_node_output(
+    def get_node_input_schema(
         self,
         experiment_id: str,
         node_id: str,
-        output_id: str,
-        request: pai_studio_20210202_models.GetNodeOutputRequest,
-    ) -> pai_studio_20210202_models.GetNodeOutputResponse:
+        request: pai_studio_20210202_models.GetNodeInputSchemaRequest,
+    ) -> pai_studio_20210202_models.GetNodeInputSchemaResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_node_output_with_options(experiment_id, node_id, output_id, request, headers, runtime)
+        return self.get_node_input_schema_with_options(experiment_id, node_id, request, headers, runtime)
 
-    async def get_node_output_async(
+    async def get_node_input_schema_async(
         self,
         experiment_id: str,
         node_id: str,
-        output_id: str,
-        request: pai_studio_20210202_models.GetNodeOutputRequest,
-    ) -> pai_studio_20210202_models.GetNodeOutputResponse:
+        request: pai_studio_20210202_models.GetNodeInputSchemaRequest,
+    ) -> pai_studio_20210202_models.GetNodeInputSchemaResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_node_output_with_options_async(experiment_id, node_id, output_id, request, headers, runtime)
+        return await self.get_node_input_schema_with_options_async(experiment_id, node_id, request, headers, runtime)
 
     def get_node_output_with_options(
         self,
         experiment_id: str,
         node_id: str,
         output_id: str,
         request: pai_studio_20210202_models.GetNodeOutputRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetNodeOutputResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
-        node_id = OpenApiUtilClient.get_encode_param(node_id)
-        output_id = OpenApiUtilClient.get_encode_param(output_id)
         query = {}
         if not UtilClient.is_unset(request.output_index):
             query['OutputIndex'] = request.output_index
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetNodeOutput',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/nodes/{node_id}/outputs/{output_id}',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/nodes/{OpenApiUtilClient.get_encode_param(node_id)}/outputs/{OpenApiUtilClient.get_encode_param(output_id)}',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -2249,87 +2052,81 @@
         node_id: str,
         output_id: str,
         request: pai_studio_20210202_models.GetNodeOutputRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetNodeOutputResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
-        node_id = OpenApiUtilClient.get_encode_param(node_id)
-        output_id = OpenApiUtilClient.get_encode_param(output_id)
         query = {}
         if not UtilClient.is_unset(request.output_index):
             query['OutputIndex'] = request.output_index
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetNodeOutput',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/nodes/{node_id}/outputs/{output_id}',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/nodes/{OpenApiUtilClient.get_encode_param(node_id)}/outputs/{OpenApiUtilClient.get_encode_param(output_id)}',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetNodeOutputResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_node_visualization(
+    def get_node_output(
         self,
         experiment_id: str,
         node_id: str,
-        visualization_id: str,
-        request: pai_studio_20210202_models.GetNodeVisualizationRequest,
-    ) -> pai_studio_20210202_models.GetNodeVisualizationResponse:
+        output_id: str,
+        request: pai_studio_20210202_models.GetNodeOutputRequest,
+    ) -> pai_studio_20210202_models.GetNodeOutputResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_node_visualization_with_options(experiment_id, node_id, visualization_id, request, headers, runtime)
+        return self.get_node_output_with_options(experiment_id, node_id, output_id, request, headers, runtime)
 
-    async def get_node_visualization_async(
+    async def get_node_output_async(
         self,
         experiment_id: str,
         node_id: str,
-        visualization_id: str,
-        request: pai_studio_20210202_models.GetNodeVisualizationRequest,
-    ) -> pai_studio_20210202_models.GetNodeVisualizationResponse:
+        output_id: str,
+        request: pai_studio_20210202_models.GetNodeOutputRequest,
+    ) -> pai_studio_20210202_models.GetNodeOutputResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_node_visualization_with_options_async(experiment_id, node_id, visualization_id, request, headers, runtime)
+        return await self.get_node_output_with_options_async(experiment_id, node_id, output_id, request, headers, runtime)
 
     def get_node_visualization_with_options(
         self,
         experiment_id: str,
         node_id: str,
         visualization_id: str,
         request: pai_studio_20210202_models.GetNodeVisualizationRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetNodeVisualizationResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
-        node_id = OpenApiUtilClient.get_encode_param(node_id)
-        visualization_id = OpenApiUtilClient.get_encode_param(visualization_id)
         query = {}
         if not UtilClient.is_unset(request.config):
             query['Config'] = request.config
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetNodeVisualization',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/nodes/{node_id}/visualizations/{visualization_id}',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/nodes/{OpenApiUtilClient.get_encode_param(node_id)}/visualizations/{OpenApiUtilClient.get_encode_param(visualization_id)}',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -2343,205 +2140,138 @@
         node_id: str,
         visualization_id: str,
         request: pai_studio_20210202_models.GetNodeVisualizationRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.GetNodeVisualizationResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
-        node_id = OpenApiUtilClient.get_encode_param(node_id)
-        visualization_id = OpenApiUtilClient.get_encode_param(visualization_id)
         query = {}
         if not UtilClient.is_unset(request.config):
             query['Config'] = request.config
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetNodeVisualization',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/nodes/{node_id}/visualizations/{visualization_id}',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/nodes/{OpenApiUtilClient.get_encode_param(node_id)}/visualizations/{OpenApiUtilClient.get_encode_param(visualization_id)}',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.GetNodeVisualizationResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_service(
+    def get_node_visualization(
         self,
-        service_id: str,
-        request: pai_studio_20210202_models.GetServiceRequest,
-    ) -> pai_studio_20210202_models.GetServiceResponse:
+        experiment_id: str,
+        node_id: str,
+        visualization_id: str,
+        request: pai_studio_20210202_models.GetNodeVisualizationRequest,
+    ) -> pai_studio_20210202_models.GetNodeVisualizationResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_service_with_options(service_id, request, headers, runtime)
+        return self.get_node_visualization_with_options(experiment_id, node_id, visualization_id, request, headers, runtime)
 
-    async def get_service_async(
+    async def get_node_visualization_async(
         self,
-        service_id: str,
-        request: pai_studio_20210202_models.GetServiceRequest,
-    ) -> pai_studio_20210202_models.GetServiceResponse:
+        experiment_id: str,
+        node_id: str,
+        visualization_id: str,
+        request: pai_studio_20210202_models.GetNodeVisualizationRequest,
+    ) -> pai_studio_20210202_models.GetNodeVisualizationResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_service_with_options_async(service_id, request, headers, runtime)
+        return await self.get_node_visualization_with_options_async(experiment_id, node_id, visualization_id, request, headers, runtime)
 
-    def get_service_with_options(
+    def get_template_with_options(
         self,
-        service_id: str,
-        request: pai_studio_20210202_models.GetServiceRequest,
+        template_id: str,
+        request: pai_studio_20210202_models.GetTemplateRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> pai_studio_20210202_models.GetServiceResponse:
+    ) -> pai_studio_20210202_models.GetTemplateResponse:
         UtilClient.validate_model(request)
-        service_id = OpenApiUtilClient.get_encode_param(service_id)
         query = {}
-        if not UtilClient.is_unset(request.service_type):
-            query['ServiceType'] = request.service_type
+        if not UtilClient.is_unset(request.verbose):
+            query['Verbose'] = request.verbose
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='GetService',
+            action='GetTemplate',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/services/{service_id}',
+            pathname=f'/api/v1/templates/{OpenApiUtilClient.get_encode_param(template_id)}',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
-            pai_studio_20210202_models.GetServiceResponse(),
+            pai_studio_20210202_models.GetTemplateResponse(),
             self.call_api(params, req, runtime)
         )
 
-    async def get_service_with_options_async(
+    async def get_template_with_options_async(
         self,
-        service_id: str,
-        request: pai_studio_20210202_models.GetServiceRequest,
+        template_id: str,
+        request: pai_studio_20210202_models.GetTemplateRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> pai_studio_20210202_models.GetServiceResponse:
+    ) -> pai_studio_20210202_models.GetTemplateResponse:
         UtilClient.validate_model(request)
-        service_id = OpenApiUtilClient.get_encode_param(service_id)
         query = {}
-        if not UtilClient.is_unset(request.service_type):
-            query['ServiceType'] = request.service_type
+        if not UtilClient.is_unset(request.verbose):
+            query['Verbose'] = request.verbose
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='GetService',
+            action='GetTemplate',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/services/{service_id}',
+            pathname=f'/api/v1/templates/{OpenApiUtilClient.get_encode_param(template_id)}',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
-            pai_studio_20210202_models.GetServiceResponse(),
+            pai_studio_20210202_models.GetTemplateResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def get_template(
         self,
         template_id: str,
+        request: pai_studio_20210202_models.GetTemplateRequest,
     ) -> pai_studio_20210202_models.GetTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_template_with_options(template_id, headers, runtime)
+        return self.get_template_with_options(template_id, request, headers, runtime)
 
     async def get_template_async(
         self,
         template_id: str,
+        request: pai_studio_20210202_models.GetTemplateRequest,
     ) -> pai_studio_20210202_models.GetTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_template_with_options_async(template_id, headers, runtime)
-
-    def get_template_with_options(
-        self,
-        template_id: str,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> pai_studio_20210202_models.GetTemplateResponse:
-        template_id = OpenApiUtilClient.get_encode_param(template_id)
-        req = open_api_models.OpenApiRequest(
-            headers=headers
-        )
-        params = open_api_models.Params(
-            action='GetTemplate',
-            version='2021-02-02',
-            protocol='HTTPS',
-            pathname=f'/api/v1/templates/{template_id}',
-            method='GET',
-            auth_type='AK',
-            style='ROA',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            pai_studio_20210202_models.GetTemplateResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def get_template_with_options_async(
-        self,
-        template_id: str,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> pai_studio_20210202_models.GetTemplateResponse:
-        template_id = OpenApiUtilClient.get_encode_param(template_id)
-        req = open_api_models.OpenApiRequest(
-            headers=headers
-        )
-        params = open_api_models.Params(
-            action='GetTemplate',
-            version='2021-02-02',
-            protocol='HTTPS',
-            pathname=f'/api/v1/templates/{template_id}',
-            method='GET',
-            auth_type='AK',
-            style='ROA',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            pai_studio_20210202_models.GetTemplateResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def list_algo_defs(
-        self,
-        request: pai_studio_20210202_models.ListAlgoDefsRequest,
-    ) -> pai_studio_20210202_models.ListAlgoDefsResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.list_algo_defs_with_options(request, headers, runtime)
-
-    async def list_algo_defs_async(
-        self,
-        request: pai_studio_20210202_models.ListAlgoDefsRequest,
-    ) -> pai_studio_20210202_models.ListAlgoDefsResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.list_algo_defs_with_options_async(request, headers, runtime)
+        return await self.get_template_with_options_async(template_id, request, headers, runtime)
 
     def list_algo_defs_with_options(
         self,
         request: pai_studio_20210202_models.ListAlgoDefsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.ListAlgoDefsResponse:
@@ -2589,29 +2319,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.ListAlgoDefsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_auth_roles(
+    def list_algo_defs(
         self,
-        request: pai_studio_20210202_models.ListAuthRolesRequest,
-    ) -> pai_studio_20210202_models.ListAuthRolesResponse:
+        request: pai_studio_20210202_models.ListAlgoDefsRequest,
+    ) -> pai_studio_20210202_models.ListAlgoDefsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_auth_roles_with_options(request, headers, runtime)
+        return self.list_algo_defs_with_options(request, headers, runtime)
 
-    async def list_auth_roles_async(
+    async def list_algo_defs_async(
         self,
-        request: pai_studio_20210202_models.ListAuthRolesRequest,
-    ) -> pai_studio_20210202_models.ListAuthRolesResponse:
+        request: pai_studio_20210202_models.ListAlgoDefsRequest,
+    ) -> pai_studio_20210202_models.ListAlgoDefsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_auth_roles_with_options_async(request, headers, runtime)
+        return await self.list_algo_defs_with_options_async(request, headers, runtime)
 
     def list_auth_roles_with_options(
         self,
         request: pai_studio_20210202_models.ListAuthRolesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.ListAuthRolesResponse:
@@ -2669,29 +2399,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.ListAuthRolesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_experiments(
+    def list_auth_roles(
         self,
-        request: pai_studio_20210202_models.ListExperimentsRequest,
-    ) -> pai_studio_20210202_models.ListExperimentsResponse:
+        request: pai_studio_20210202_models.ListAuthRolesRequest,
+    ) -> pai_studio_20210202_models.ListAuthRolesResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_experiments_with_options(request, headers, runtime)
+        return self.list_auth_roles_with_options(request, headers, runtime)
 
-    async def list_experiments_async(
+    async def list_auth_roles_async(
         self,
-        request: pai_studio_20210202_models.ListExperimentsRequest,
-    ) -> pai_studio_20210202_models.ListExperimentsResponse:
+        request: pai_studio_20210202_models.ListAuthRolesRequest,
+    ) -> pai_studio_20210202_models.ListAuthRolesResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_experiments_with_options_async(request, headers, runtime)
+        return await self.list_auth_roles_with_options_async(request, headers, runtime)
 
     def list_experiments_with_options(
         self,
         request: pai_studio_20210202_models.ListExperimentsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.ListExperimentsResponse:
@@ -2777,29 +2507,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.ListExperimentsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_image_labels(
+    def list_experiments(
         self,
-        request: pai_studio_20210202_models.ListImageLabelsRequest,
-    ) -> pai_studio_20210202_models.ListImageLabelsResponse:
+        request: pai_studio_20210202_models.ListExperimentsRequest,
+    ) -> pai_studio_20210202_models.ListExperimentsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_image_labels_with_options(request, headers, runtime)
+        return self.list_experiments_with_options(request, headers, runtime)
 
-    async def list_image_labels_async(
+    async def list_experiments_async(
         self,
-        request: pai_studio_20210202_models.ListImageLabelsRequest,
-    ) -> pai_studio_20210202_models.ListImageLabelsResponse:
+        request: pai_studio_20210202_models.ListExperimentsRequest,
+    ) -> pai_studio_20210202_models.ListExperimentsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_image_labels_with_options_async(request, headers, runtime)
+        return await self.list_experiments_with_options_async(request, headers, runtime)
 
     def list_image_labels_with_options(
         self,
         request: pai_studio_20210202_models.ListImageLabelsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.ListImageLabelsResponse:
@@ -2861,29 +2591,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.ListImageLabelsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_images(
+    def list_image_labels(
         self,
-        request: pai_studio_20210202_models.ListImagesRequest,
-    ) -> pai_studio_20210202_models.ListImagesResponse:
+        request: pai_studio_20210202_models.ListImageLabelsRequest,
+    ) -> pai_studio_20210202_models.ListImageLabelsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_images_with_options(request, headers, runtime)
+        return self.list_image_labels_with_options(request, headers, runtime)
 
-    async def list_images_async(
+    async def list_image_labels_async(
         self,
-        request: pai_studio_20210202_models.ListImagesRequest,
-    ) -> pai_studio_20210202_models.ListImagesResponse:
+        request: pai_studio_20210202_models.ListImageLabelsRequest,
+    ) -> pai_studio_20210202_models.ListImageLabelsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_images_with_options_async(request, headers, runtime)
+        return await self.list_image_labels_with_options_async(request, headers, runtime)
 
     def list_images_with_options(
         self,
         request: pai_studio_20210202_models.ListImagesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.ListImagesResponse:
@@ -2961,29 +2691,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.ListImagesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_jobs(
+    def list_images(
         self,
-        request: pai_studio_20210202_models.ListJobsRequest,
-    ) -> pai_studio_20210202_models.ListJobsResponse:
+        request: pai_studio_20210202_models.ListImagesRequest,
+    ) -> pai_studio_20210202_models.ListImagesResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_jobs_with_options(request, headers, runtime)
+        return self.list_images_with_options(request, headers, runtime)
 
-    async def list_jobs_async(
+    async def list_images_async(
         self,
-        request: pai_studio_20210202_models.ListJobsRequest,
-    ) -> pai_studio_20210202_models.ListJobsResponse:
+        request: pai_studio_20210202_models.ListImagesRequest,
+    ) -> pai_studio_20210202_models.ListImagesResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_jobs_with_options_async(request, headers, runtime)
+        return await self.list_images_with_options_async(request, headers, runtime)
 
     def list_jobs_with_options(
         self,
         request: pai_studio_20210202_models.ListJobsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.ListJobsResponse:
@@ -3053,49 +2783,45 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.ListJobsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_node_outputs(
+    def list_jobs(
         self,
-        experiment_id: str,
-        node_id: str,
-    ) -> pai_studio_20210202_models.ListNodeOutputsResponse:
+        request: pai_studio_20210202_models.ListJobsRequest,
+    ) -> pai_studio_20210202_models.ListJobsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_node_outputs_with_options(experiment_id, node_id, headers, runtime)
+        return self.list_jobs_with_options(request, headers, runtime)
 
-    async def list_node_outputs_async(
+    async def list_jobs_async(
         self,
-        experiment_id: str,
-        node_id: str,
-    ) -> pai_studio_20210202_models.ListNodeOutputsResponse:
+        request: pai_studio_20210202_models.ListJobsRequest,
+    ) -> pai_studio_20210202_models.ListJobsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_node_outputs_with_options_async(experiment_id, node_id, headers, runtime)
+        return await self.list_jobs_with_options_async(request, headers, runtime)
 
     def list_node_outputs_with_options(
         self,
         experiment_id: str,
         node_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.ListNodeOutputsResponse:
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
-        node_id = OpenApiUtilClient.get_encode_param(node_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListNodeOutputs',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/nodes/{node_id}/outputs',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/nodes/{OpenApiUtilClient.get_encode_param(node_id)}/outputs',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -3106,50 +2832,50 @@
     async def list_node_outputs_with_options_async(
         self,
         experiment_id: str,
         node_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.ListNodeOutputsResponse:
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
-        node_id = OpenApiUtilClient.get_encode_param(node_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListNodeOutputs',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/nodes/{node_id}/outputs',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/nodes/{OpenApiUtilClient.get_encode_param(node_id)}/outputs',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.ListNodeOutputsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_recent_experiments(
+    def list_node_outputs(
         self,
-        request: pai_studio_20210202_models.ListRecentExperimentsRequest,
-    ) -> pai_studio_20210202_models.ListRecentExperimentsResponse:
+        experiment_id: str,
+        node_id: str,
+    ) -> pai_studio_20210202_models.ListNodeOutputsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_recent_experiments_with_options(request, headers, runtime)
+        return self.list_node_outputs_with_options(experiment_id, node_id, headers, runtime)
 
-    async def list_recent_experiments_async(
+    async def list_node_outputs_async(
         self,
-        request: pai_studio_20210202_models.ListRecentExperimentsRequest,
-    ) -> pai_studio_20210202_models.ListRecentExperimentsResponse:
+        experiment_id: str,
+        node_id: str,
+    ) -> pai_studio_20210202_models.ListNodeOutputsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_recent_experiments_with_options_async(request, headers, runtime)
+        return await self.list_node_outputs_with_options_async(experiment_id, node_id, headers, runtime)
 
     def list_recent_experiments_with_options(
         self,
         request: pai_studio_20210202_models.ListRecentExperimentsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.ListRecentExperimentsResponse:
@@ -3223,132 +2949,64 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.ListRecentExperimentsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_services(
-        self,
-        request: pai_studio_20210202_models.ListServicesRequest,
-    ) -> pai_studio_20210202_models.ListServicesResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.list_services_with_options(request, headers, runtime)
-
-    async def list_services_async(
-        self,
-        request: pai_studio_20210202_models.ListServicesRequest,
-    ) -> pai_studio_20210202_models.ListServicesResponse:
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.list_services_with_options_async(request, headers, runtime)
-
-    def list_services_with_options(
-        self,
-        request: pai_studio_20210202_models.ListServicesRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> pai_studio_20210202_models.ListServicesResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.service_type):
-            query['ServiceType'] = request.service_type
-        if not UtilClient.is_unset(request.workspace_id):
-            query['WorkspaceId'] = request.workspace_id
-        req = open_api_models.OpenApiRequest(
-            headers=headers,
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ListServices',
-            version='2021-02-02',
-            protocol='HTTPS',
-            pathname=f'/api/v1/services',
-            method='GET',
-            auth_type='AK',
-            style='ROA',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            pai_studio_20210202_models.ListServicesResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    async def list_services_with_options_async(
-        self,
-        request: pai_studio_20210202_models.ListServicesRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> pai_studio_20210202_models.ListServicesResponse:
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.service_type):
-            query['ServiceType'] = request.service_type
-        if not UtilClient.is_unset(request.workspace_id):
-            query['WorkspaceId'] = request.workspace_id
-        req = open_api_models.OpenApiRequest(
-            headers=headers,
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='ListServices',
-            version='2021-02-02',
-            protocol='HTTPS',
-            pathname=f'/api/v1/services',
-            method='GET',
-            auth_type='AK',
-            style='ROA',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            pai_studio_20210202_models.ListServicesResponse(),
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def list_templates(
+    def list_recent_experiments(
         self,
-        request: pai_studio_20210202_models.ListTemplatesRequest,
-    ) -> pai_studio_20210202_models.ListTemplatesResponse:
+        request: pai_studio_20210202_models.ListRecentExperimentsRequest,
+    ) -> pai_studio_20210202_models.ListRecentExperimentsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_templates_with_options(request, headers, runtime)
+        return self.list_recent_experiments_with_options(request, headers, runtime)
 
-    async def list_templates_async(
+    async def list_recent_experiments_async(
         self,
-        request: pai_studio_20210202_models.ListTemplatesRequest,
-    ) -> pai_studio_20210202_models.ListTemplatesResponse:
+        request: pai_studio_20210202_models.ListRecentExperimentsRequest,
+    ) -> pai_studio_20210202_models.ListRecentExperimentsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_templates_with_options_async(request, headers, runtime)
+        return await self.list_recent_experiments_with_options_async(request, headers, runtime)
 
     def list_templates_with_options(
         self,
         request: pai_studio_20210202_models.ListTemplatesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.ListTemplatesResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.label):
+            query['Label'] = request.label
         if not UtilClient.is_unset(request.list):
             query['List'] = request.list
+        if not UtilClient.is_unset(request.name):
+            query['Name'] = request.name
         if not UtilClient.is_unset(request.order):
             query['Order'] = request.order
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.sort_by):
+            query['SortBy'] = request.sort_by
         if not UtilClient.is_unset(request.source):
             query['Source'] = request.source
         if not UtilClient.is_unset(request.tag_id):
             query['TagId'] = request.tag_id
+        if not UtilClient.is_unset(request.template_type):
+            query['TemplateType'] = request.template_type
         if not UtilClient.is_unset(request.type_id):
             query['TypeId'] = request.type_id
+        if not UtilClient.is_unset(request.verbose):
+            query['Verbose'] = request.verbose
+        if not UtilClient.is_unset(request.workspace_id):
+            query['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTemplates',
             version='2021-02-02',
@@ -3369,28 +3027,40 @@
         self,
         request: pai_studio_20210202_models.ListTemplatesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.ListTemplatesResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.label):
+            query['Label'] = request.label
         if not UtilClient.is_unset(request.list):
             query['List'] = request.list
+        if not UtilClient.is_unset(request.name):
+            query['Name'] = request.name
         if not UtilClient.is_unset(request.order):
             query['Order'] = request.order
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.sort_by):
+            query['SortBy'] = request.sort_by
         if not UtilClient.is_unset(request.source):
             query['Source'] = request.source
         if not UtilClient.is_unset(request.tag_id):
             query['TagId'] = request.tag_id
+        if not UtilClient.is_unset(request.template_type):
+            query['TemplateType'] = request.template_type
         if not UtilClient.is_unset(request.type_id):
             query['TypeId'] = request.type_id
+        if not UtilClient.is_unset(request.verbose):
+            query['Verbose'] = request.verbose
+        if not UtilClient.is_unset(request.workspace_id):
+            query['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTemplates',
             version='2021-02-02',
@@ -3403,29 +3073,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.ListTemplatesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def migrate_experiment_folders(
+    def list_templates(
         self,
-        request: pai_studio_20210202_models.MigrateExperimentFoldersRequest,
-    ) -> pai_studio_20210202_models.MigrateExperimentFoldersResponse:
+        request: pai_studio_20210202_models.ListTemplatesRequest,
+    ) -> pai_studio_20210202_models.ListTemplatesResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.migrate_experiment_folders_with_options(request, headers, runtime)
+        return self.list_templates_with_options(request, headers, runtime)
 
-    async def migrate_experiment_folders_async(
+    async def list_templates_async(
         self,
-        request: pai_studio_20210202_models.MigrateExperimentFoldersRequest,
-    ) -> pai_studio_20210202_models.MigrateExperimentFoldersResponse:
+        request: pai_studio_20210202_models.ListTemplatesRequest,
+    ) -> pai_studio_20210202_models.ListTemplatesResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.migrate_experiment_folders_with_options_async(request, headers, runtime)
+        return await self.list_templates_with_options_async(request, headers, runtime)
 
     def migrate_experiment_folders_with_options(
         self,
         request: pai_studio_20210202_models.MigrateExperimentFoldersRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.MigrateExperimentFoldersResponse:
@@ -3487,29 +3157,29 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.MigrateExperimentFoldersResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def migrate_experiments(
+    def migrate_experiment_folders(
         self,
-        request: pai_studio_20210202_models.MigrateExperimentsRequest,
-    ) -> pai_studio_20210202_models.MigrateExperimentsResponse:
+        request: pai_studio_20210202_models.MigrateExperimentFoldersRequest,
+    ) -> pai_studio_20210202_models.MigrateExperimentFoldersResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.migrate_experiments_with_options(request, headers, runtime)
+        return self.migrate_experiment_folders_with_options(request, headers, runtime)
 
-    async def migrate_experiments_async(
+    async def migrate_experiment_folders_async(
         self,
-        request: pai_studio_20210202_models.MigrateExperimentsRequest,
-    ) -> pai_studio_20210202_models.MigrateExperimentsResponse:
+        request: pai_studio_20210202_models.MigrateExperimentFoldersRequest,
+    ) -> pai_studio_20210202_models.MigrateExperimentFoldersResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.migrate_experiments_with_options_async(request, headers, runtime)
+        return await self.migrate_experiment_folders_with_options_async(request, headers, runtime)
 
     def migrate_experiments_with_options(
         self,
         request: pai_studio_20210202_models.MigrateExperimentsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.MigrateExperimentsResponse:
@@ -3583,57 +3253,56 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.MigrateExperimentsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def preview_mctable(
+    def migrate_experiments(
         self,
-        table_name: str,
-        request: pai_studio_20210202_models.PreviewMCTableRequest,
-    ) -> pai_studio_20210202_models.PreviewMCTableResponse:
+        request: pai_studio_20210202_models.MigrateExperimentsRequest,
+    ) -> pai_studio_20210202_models.MigrateExperimentsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.preview_mctable_with_options(table_name, request, headers, runtime)
+        return self.migrate_experiments_with_options(request, headers, runtime)
 
-    async def preview_mctable_async(
+    async def migrate_experiments_async(
         self,
-        table_name: str,
-        request: pai_studio_20210202_models.PreviewMCTableRequest,
-    ) -> pai_studio_20210202_models.PreviewMCTableResponse:
+        request: pai_studio_20210202_models.MigrateExperimentsRequest,
+    ) -> pai_studio_20210202_models.MigrateExperimentsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.preview_mctable_with_options_async(table_name, request, headers, runtime)
+        return await self.migrate_experiments_with_options_async(request, headers, runtime)
 
     def preview_mctable_with_options(
         self,
         table_name: str,
         request: pai_studio_20210202_models.PreviewMCTableRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.PreviewMCTableResponse:
         UtilClient.validate_model(request)
-        table_name = OpenApiUtilClient.get_encode_param(table_name)
         query = {}
         if not UtilClient.is_unset(request.endpoint):
             query['Endpoint'] = request.endpoint
+        if not UtilClient.is_unset(request.limit):
+            query['Limit'] = request.limit
         if not UtilClient.is_unset(request.partition):
             query['Partition'] = request.partition
         if not UtilClient.is_unset(request.workspace_id):
             query['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='PreviewMCTable',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/datasources/maxcompute/tables/{table_name}/preview',
+            pathname=f'/api/v1/datasources/maxcompute/tables/{OpenApiUtilClient.get_encode_param(table_name)}/preview',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -3645,81 +3314,81 @@
         self,
         table_name: str,
         request: pai_studio_20210202_models.PreviewMCTableRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.PreviewMCTableResponse:
         UtilClient.validate_model(request)
-        table_name = OpenApiUtilClient.get_encode_param(table_name)
         query = {}
         if not UtilClient.is_unset(request.endpoint):
             query['Endpoint'] = request.endpoint
+        if not UtilClient.is_unset(request.limit):
+            query['Limit'] = request.limit
         if not UtilClient.is_unset(request.partition):
             query['Partition'] = request.partition
         if not UtilClient.is_unset(request.workspace_id):
             query['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='PreviewMCTable',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/datasources/maxcompute/tables/{table_name}/preview',
+            pathname=f'/api/v1/datasources/maxcompute/tables/{OpenApiUtilClient.get_encode_param(table_name)}/preview',
             method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.PreviewMCTableResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def publish_experiment(
+    def preview_mctable(
         self,
-        experiment_id: str,
-        request: pai_studio_20210202_models.PublishExperimentRequest,
-    ) -> pai_studio_20210202_models.PublishExperimentResponse:
+        table_name: str,
+        request: pai_studio_20210202_models.PreviewMCTableRequest,
+    ) -> pai_studio_20210202_models.PreviewMCTableResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.publish_experiment_with_options(experiment_id, request, headers, runtime)
+        return self.preview_mctable_with_options(table_name, request, headers, runtime)
 
-    async def publish_experiment_async(
+    async def preview_mctable_async(
         self,
-        experiment_id: str,
-        request: pai_studio_20210202_models.PublishExperimentRequest,
-    ) -> pai_studio_20210202_models.PublishExperimentResponse:
+        table_name: str,
+        request: pai_studio_20210202_models.PreviewMCTableRequest,
+    ) -> pai_studio_20210202_models.PreviewMCTableResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.publish_experiment_with_options_async(experiment_id, request, headers, runtime)
+        return await self.preview_mctable_with_options_async(table_name, request, headers, runtime)
 
     def publish_experiment_with_options(
         self,
         experiment_id: str,
         request: pai_studio_20210202_models.PublishExperimentRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.PublishExperimentResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         body = {}
         if not UtilClient.is_unset(request.folder_id):
             body['FolderId'] = request.folder_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PublishExperiment',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/publish',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/publish',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -3731,74 +3400,72 @@
         self,
         experiment_id: str,
         request: pai_studio_20210202_models.PublishExperimentRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.PublishExperimentResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         body = {}
         if not UtilClient.is_unset(request.folder_id):
             body['FolderId'] = request.folder_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PublishExperiment',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/publish',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/publish',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.PublishExperimentResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def query_experiment_visualization_data(
+    def publish_experiment(
         self,
         experiment_id: str,
-        request: pai_studio_20210202_models.QueryExperimentVisualizationDataRequest,
-    ) -> pai_studio_20210202_models.QueryExperimentVisualizationDataResponse:
+        request: pai_studio_20210202_models.PublishExperimentRequest,
+    ) -> pai_studio_20210202_models.PublishExperimentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.query_experiment_visualization_data_with_options(experiment_id, request, headers, runtime)
+        return self.publish_experiment_with_options(experiment_id, request, headers, runtime)
 
-    async def query_experiment_visualization_data_async(
+    async def publish_experiment_async(
         self,
         experiment_id: str,
-        request: pai_studio_20210202_models.QueryExperimentVisualizationDataRequest,
-    ) -> pai_studio_20210202_models.QueryExperimentVisualizationDataResponse:
+        request: pai_studio_20210202_models.PublishExperimentRequest,
+    ) -> pai_studio_20210202_models.PublishExperimentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.query_experiment_visualization_data_with_options_async(experiment_id, request, headers, runtime)
+        return await self.publish_experiment_with_options_async(experiment_id, request, headers, runtime)
 
     def query_experiment_visualization_data_with_options(
         self,
         experiment_id: str,
         request: pai_studio_20210202_models.QueryExperimentVisualizationDataRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.QueryExperimentVisualizationDataResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=UtilClient.to_array(request.body)
         )
         params = open_api_models.Params(
             action='QueryExperimentVisualizationData',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/visualizationDataQuery',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/visualizationDataQuery',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -3810,66 +3477,66 @@
         self,
         experiment_id: str,
         request: pai_studio_20210202_models.QueryExperimentVisualizationDataRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.QueryExperimentVisualizationDataResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=UtilClient.to_array(request.body)
         )
         params = open_api_models.Params(
             action='QueryExperimentVisualizationData',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/visualizationDataQuery',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/visualizationDataQuery',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.QueryExperimentVisualizationDataResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def remove_image(
+    def query_experiment_visualization_data(
         self,
-        image_id: str,
-    ) -> pai_studio_20210202_models.RemoveImageResponse:
+        experiment_id: str,
+        request: pai_studio_20210202_models.QueryExperimentVisualizationDataRequest,
+    ) -> pai_studio_20210202_models.QueryExperimentVisualizationDataResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.remove_image_with_options(image_id, headers, runtime)
+        return self.query_experiment_visualization_data_with_options(experiment_id, request, headers, runtime)
 
-    async def remove_image_async(
+    async def query_experiment_visualization_data_async(
         self,
-        image_id: str,
-    ) -> pai_studio_20210202_models.RemoveImageResponse:
+        experiment_id: str,
+        request: pai_studio_20210202_models.QueryExperimentVisualizationDataRequest,
+    ) -> pai_studio_20210202_models.QueryExperimentVisualizationDataResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.remove_image_with_options_async(image_id, headers, runtime)
+        return await self.query_experiment_visualization_data_with_options_async(experiment_id, request, headers, runtime)
 
     def remove_image_with_options(
         self,
         image_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.RemoveImageResponse:
-        image_id = OpenApiUtilClient.get_encode_param(image_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='RemoveImage',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/images/{image_id}',
+            pathname=f'/api/v1/images/{OpenApiUtilClient.get_encode_param(image_id)}',
             method='DELETE',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -3879,69 +3546,64 @@
 
     async def remove_image_with_options_async(
         self,
         image_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.RemoveImageResponse:
-        image_id = OpenApiUtilClient.get_encode_param(image_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='RemoveImage',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/images/{image_id}',
+            pathname=f'/api/v1/images/{OpenApiUtilClient.get_encode_param(image_id)}',
             method='DELETE',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.RemoveImageResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def remove_image_labels(
+    def remove_image(
         self,
         image_id: str,
-        label_key: str,
-    ) -> pai_studio_20210202_models.RemoveImageLabelsResponse:
+    ) -> pai_studio_20210202_models.RemoveImageResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.remove_image_labels_with_options(image_id, label_key, headers, runtime)
+        return self.remove_image_with_options(image_id, headers, runtime)
 
-    async def remove_image_labels_async(
+    async def remove_image_async(
         self,
         image_id: str,
-        label_key: str,
-    ) -> pai_studio_20210202_models.RemoveImageLabelsResponse:
+    ) -> pai_studio_20210202_models.RemoveImageResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.remove_image_labels_with_options_async(image_id, label_key, headers, runtime)
+        return await self.remove_image_with_options_async(image_id, headers, runtime)
 
     def remove_image_labels_with_options(
         self,
         image_id: str,
         label_key: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.RemoveImageLabelsResponse:
-        image_id = OpenApiUtilClient.get_encode_param(image_id)
-        label_key = OpenApiUtilClient.get_encode_param(label_key)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='RemoveImageLabels',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/images/{image_id}/labels/{label_key}',
+            pathname=f'/api/v1/images/{OpenApiUtilClient.get_encode_param(image_id)}/labels/{OpenApiUtilClient.get_encode_param(label_key)}',
             method='DELETE',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -3952,50 +3614,50 @@
     async def remove_image_labels_with_options_async(
         self,
         image_id: str,
         label_key: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.RemoveImageLabelsResponse:
-        image_id = OpenApiUtilClient.get_encode_param(image_id)
-        label_key = OpenApiUtilClient.get_encode_param(label_key)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='RemoveImageLabels',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/images/{image_id}/labels/{label_key}',
+            pathname=f'/api/v1/images/{OpenApiUtilClient.get_encode_param(image_id)}/labels/{OpenApiUtilClient.get_encode_param(label_key)}',
             method='DELETE',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.RemoveImageLabelsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def search_mctables(
+    def remove_image_labels(
         self,
-        request: pai_studio_20210202_models.SearchMCTablesRequest,
-    ) -> pai_studio_20210202_models.SearchMCTablesResponse:
+        image_id: str,
+        label_key: str,
+    ) -> pai_studio_20210202_models.RemoveImageLabelsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.search_mctables_with_options(request, headers, runtime)
+        return self.remove_image_labels_with_options(image_id, label_key, headers, runtime)
 
-    async def search_mctables_async(
+    async def remove_image_labels_async(
         self,
-        request: pai_studio_20210202_models.SearchMCTablesRequest,
-    ) -> pai_studio_20210202_models.SearchMCTablesResponse:
+        image_id: str,
+        label_key: str,
+    ) -> pai_studio_20210202_models.RemoveImageLabelsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.search_mctables_with_options_async(request, headers, runtime)
+        return await self.remove_image_labels_with_options_async(image_id, label_key, headers, runtime)
 
     def search_mctables_with_options(
         self,
         request: pai_studio_20210202_models.SearchMCTablesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.SearchMCTablesResponse:
@@ -4053,45 +3715,44 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.SearchMCTablesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def stop_experiment(
+    def search_mctables(
         self,
-        experiment_id: str,
-    ) -> pai_studio_20210202_models.StopExperimentResponse:
+        request: pai_studio_20210202_models.SearchMCTablesRequest,
+    ) -> pai_studio_20210202_models.SearchMCTablesResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.stop_experiment_with_options(experiment_id, headers, runtime)
+        return self.search_mctables_with_options(request, headers, runtime)
 
-    async def stop_experiment_async(
+    async def search_mctables_async(
         self,
-        experiment_id: str,
-    ) -> pai_studio_20210202_models.StopExperimentResponse:
+        request: pai_studio_20210202_models.SearchMCTablesRequest,
+    ) -> pai_studio_20210202_models.SearchMCTablesResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.stop_experiment_with_options_async(experiment_id, headers, runtime)
+        return await self.search_mctables_with_options_async(request, headers, runtime)
 
     def stop_experiment_with_options(
         self,
         experiment_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.StopExperimentResponse:
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='StopExperiment',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/stop',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/stop',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -4101,65 +3762,63 @@
 
     async def stop_experiment_with_options_async(
         self,
         experiment_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.StopExperimentResponse:
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='StopExperiment',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/stop',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/stop',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.StopExperimentResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def stop_job(
+    def stop_experiment(
         self,
-        job_id: str,
-    ) -> pai_studio_20210202_models.StopJobResponse:
+        experiment_id: str,
+    ) -> pai_studio_20210202_models.StopExperimentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.stop_job_with_options(job_id, headers, runtime)
+        return self.stop_experiment_with_options(experiment_id, headers, runtime)
 
-    async def stop_job_async(
+    async def stop_experiment_async(
         self,
-        job_id: str,
-    ) -> pai_studio_20210202_models.StopJobResponse:
+        experiment_id: str,
+    ) -> pai_studio_20210202_models.StopExperimentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.stop_job_with_options_async(job_id, headers, runtime)
+        return await self.stop_experiment_with_options_async(experiment_id, headers, runtime)
 
     def stop_job_with_options(
         self,
         job_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.StopJobResponse:
-        job_id = OpenApiUtilClient.get_encode_param(job_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='StopJob',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/jobs/{job_id}/stop',
+            pathname=f'/api/v1/jobs/{OpenApiUtilClient.get_encode_param(job_id)}/stop',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -4169,75 +3828,71 @@
 
     async def stop_job_with_options_async(
         self,
         job_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.StopJobResponse:
-        job_id = OpenApiUtilClient.get_encode_param(job_id)
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='StopJob',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/jobs/{job_id}/stop',
+            pathname=f'/api/v1/jobs/{OpenApiUtilClient.get_encode_param(job_id)}/stop',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.StopJobResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def update_experiment_content(
+    def stop_job(
         self,
-        experiment_id: str,
-        request: pai_studio_20210202_models.UpdateExperimentContentRequest,
-    ) -> pai_studio_20210202_models.UpdateExperimentContentResponse:
+        job_id: str,
+    ) -> pai_studio_20210202_models.StopJobResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.update_experiment_content_with_options(experiment_id, request, headers, runtime)
+        return self.stop_job_with_options(job_id, headers, runtime)
 
-    async def update_experiment_content_async(
+    async def stop_job_async(
         self,
-        experiment_id: str,
-        request: pai_studio_20210202_models.UpdateExperimentContentRequest,
-    ) -> pai_studio_20210202_models.UpdateExperimentContentResponse:
+        job_id: str,
+    ) -> pai_studio_20210202_models.StopJobResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.update_experiment_content_with_options_async(experiment_id, request, headers, runtime)
+        return await self.stop_job_with_options_async(job_id, headers, runtime)
 
     def update_experiment_content_with_options(
         self,
         experiment_id: str,
         request: pai_studio_20210202_models.UpdateExperimentContentRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.UpdateExperimentContentResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         body = {}
         if not UtilClient.is_unset(request.content):
             body['Content'] = request.content
         if not UtilClient.is_unset(request.version):
             body['Version'] = request.version
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateExperimentContent',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/content',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/content',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -4249,81 +3904,79 @@
         self,
         experiment_id: str,
         request: pai_studio_20210202_models.UpdateExperimentContentRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.UpdateExperimentContentResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         body = {}
         if not UtilClient.is_unset(request.content):
             body['Content'] = request.content
         if not UtilClient.is_unset(request.version):
             body['Version'] = request.version
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateExperimentContent',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/content',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/content',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.UpdateExperimentContentResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def update_experiment_folder(
+    def update_experiment_content(
         self,
-        folder_id: str,
-        request: pai_studio_20210202_models.UpdateExperimentFolderRequest,
-    ) -> pai_studio_20210202_models.UpdateExperimentFolderResponse:
+        experiment_id: str,
+        request: pai_studio_20210202_models.UpdateExperimentContentRequest,
+    ) -> pai_studio_20210202_models.UpdateExperimentContentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.update_experiment_folder_with_options(folder_id, request, headers, runtime)
+        return self.update_experiment_content_with_options(experiment_id, request, headers, runtime)
 
-    async def update_experiment_folder_async(
+    async def update_experiment_content_async(
         self,
-        folder_id: str,
-        request: pai_studio_20210202_models.UpdateExperimentFolderRequest,
-    ) -> pai_studio_20210202_models.UpdateExperimentFolderResponse:
+        experiment_id: str,
+        request: pai_studio_20210202_models.UpdateExperimentContentRequest,
+    ) -> pai_studio_20210202_models.UpdateExperimentContentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.update_experiment_folder_with_options_async(folder_id, request, headers, runtime)
+        return await self.update_experiment_content_with_options_async(experiment_id, request, headers, runtime)
 
     def update_experiment_folder_with_options(
         self,
         folder_id: str,
         request: pai_studio_20210202_models.UpdateExperimentFolderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.UpdateExperimentFolderResponse:
         UtilClient.validate_model(request)
-        folder_id = OpenApiUtilClient.get_encode_param(folder_id)
         body = {}
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.parent_folder_id):
             body['ParentFolderId'] = request.parent_folder_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateExperimentFolder',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experimentfolders/{folder_id}',
+            pathname=f'/api/v1/experimentfolders/{OpenApiUtilClient.get_encode_param(folder_id)}',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -4335,67 +3988,65 @@
         self,
         folder_id: str,
         request: pai_studio_20210202_models.UpdateExperimentFolderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.UpdateExperimentFolderResponse:
         UtilClient.validate_model(request)
-        folder_id = OpenApiUtilClient.get_encode_param(folder_id)
         body = {}
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.parent_folder_id):
             body['ParentFolderId'] = request.parent_folder_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateExperimentFolder',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experimentfolders/{folder_id}',
+            pathname=f'/api/v1/experimentfolders/{OpenApiUtilClient.get_encode_param(folder_id)}',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.UpdateExperimentFolderResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def update_experiment_meta(
+    def update_experiment_folder(
         self,
-        experiment_id: str,
-        request: pai_studio_20210202_models.UpdateExperimentMetaRequest,
-    ) -> pai_studio_20210202_models.UpdateExperimentMetaResponse:
+        folder_id: str,
+        request: pai_studio_20210202_models.UpdateExperimentFolderRequest,
+    ) -> pai_studio_20210202_models.UpdateExperimentFolderResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.update_experiment_meta_with_options(experiment_id, request, headers, runtime)
+        return self.update_experiment_folder_with_options(folder_id, request, headers, runtime)
 
-    async def update_experiment_meta_async(
+    async def update_experiment_folder_async(
         self,
-        experiment_id: str,
-        request: pai_studio_20210202_models.UpdateExperimentMetaRequest,
-    ) -> pai_studio_20210202_models.UpdateExperimentMetaResponse:
+        folder_id: str,
+        request: pai_studio_20210202_models.UpdateExperimentFolderRequest,
+    ) -> pai_studio_20210202_models.UpdateExperimentFolderResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.update_experiment_meta_with_options_async(experiment_id, request, headers, runtime)
+        return await self.update_experiment_folder_with_options_async(folder_id, request, headers, runtime)
 
     def update_experiment_meta_with_options(
         self,
         experiment_id: str,
         request: pai_studio_20210202_models.UpdateExperimentMetaRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.UpdateExperimentMetaResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         body = {}
         if not UtilClient.is_unset(request.accessibility):
             body['Accessibility'] = request.accessibility
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.folder_id):
             body['FolderId'] = request.folder_id
@@ -4407,15 +4058,15 @@
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateExperimentMeta',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/meta',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/meta',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -4427,15 +4078,14 @@
         self,
         experiment_id: str,
         request: pai_studio_20210202_models.UpdateExperimentMetaRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_studio_20210202_models.UpdateExperimentMetaResponse:
         UtilClient.validate_model(request)
-        experiment_id = OpenApiUtilClient.get_encode_param(experiment_id)
         body = {}
         if not UtilClient.is_unset(request.accessibility):
             body['Accessibility'] = request.accessibility
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.folder_id):
             body['FolderId'] = request.folder_id
@@ -4447,18 +4097,36 @@
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateExperimentMeta',
             version='2021-02-02',
             protocol='HTTPS',
-            pathname=f'/api/v1/experiments/{experiment_id}/meta',
+            pathname=f'/api/v1/experiments/{OpenApiUtilClient.get_encode_param(experiment_id)}/meta',
             method='PUT',
             auth_type='AK',
             style='ROA',
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             pai_studio_20210202_models.UpdateExperimentMetaResponse(),
             await self.call_api_async(params, req, runtime)
         )
+
+    def update_experiment_meta(
+        self,
+        experiment_id: str,
+        request: pai_studio_20210202_models.UpdateExperimentMetaRequest,
+    ) -> pai_studio_20210202_models.UpdateExperimentMetaResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_experiment_meta_with_options(experiment_id, request, headers, runtime)
+
+    async def update_experiment_meta_async(
+        self,
+        experiment_id: str,
+        request: pai_studio_20210202_models.UpdateExperimentMetaRequest,
+    ) -> pai_studio_20210202_models.UpdateExperimentMetaResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_experiment_meta_with_options_async(experiment_id, request, headers, runtime)
```

### Comparing `alibabacloud_paistudio20210202-1.0.26/alibabacloud_paistudio20210202/models.py` & `alibabacloud_paistudio20210202-1.0.27/alibabacloud_paistudio20210202/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 class AddImageRequestLabels(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # Key
         self.key = key
-        # Value
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -43,21 +41,17 @@
     def __init__(
         self,
         description: str = None,
         image_uri: str = None,
         labels: List[AddImageRequestLabels] = None,
         name: str = None,
     ):
-        # 镜像描述
         self.description = description
-        # 镜像地址
         self.image_uri = image_uri
-        # 镜像标签，是个数组
         self.labels = labels
-        # 镜像名称
         self.name = name
 
     def validate(self):
         if self.labels:
             for k in self.labels:
                 if k:
                     k.validate()
@@ -98,17 +92,15 @@
 
 class AddImageResponseBody(TeaModel):
     def __init__(
         self,
         image_id: str = None,
         request_id: str = None,
     ):
-        # 镜像 id
         self.image_id = image_id
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -177,17 +169,15 @@
 
 class AddImageLabelsRequestLabels(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # Key
         self.key = key
-        # Value
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -211,15 +201,14 @@
 
 
 class AddImageLabelsRequest(TeaModel):
     def __init__(
         self,
         labels: List[AddImageLabelsRequestLabels] = None,
     ):
-        # 标签
         self.labels = labels
 
     def validate(self):
         if self.labels:
             for k in self.labels:
                 if k:
                     k.validate()
@@ -247,15 +236,14 @@
 
 
 class AddImageLabelsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -324,25 +312,19 @@
         accessibility: str = None,
         description: str = None,
         folder_id: str = None,
         name: str = None,
         source: str = None,
         workspace_id: str = None,
     ):
-        # 工作空间内可见性 PUBLIC; PRIVATE 默认PUBLIC
         self.accessibility = accessibility
-        # 实验描述
         self.description = description
-        # 实验创建的目录 id
         self.folder_id = folder_id
-        # 实验名称，最大长度 128，可包含中英文
         self.name = name
-        # 实验来源，目前 PaiStudio，data-airec（推荐白盒）
         self.source = source
-        # 实验创建的Workspace
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -384,15 +366,14 @@
 class CopyExperimentResponseBody(TeaModel):
     def __init__(
         self,
         experiment_id: str = None,
         request_id: str = None,
     ):
         self.experiment_id = experiment_id
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -467,15 +448,14 @@
         folder_id: str = None,
         name: str = None,
         options: str = None,
         source: str = None,
         template_id: str = None,
         workspace_id: str = None,
     ):
-        # 工作空间内可见性 PUBLIC; PRIVATE 默认PUBLIC
         self.accessibility = accessibility
         self.description = description
         self.folder_id = folder_id
         self.name = name
         self.options = options
         self.source = source
         self.template_id = template_id
@@ -532,15 +512,14 @@
 class CreateExperimentResponseBody(TeaModel):
     def __init__(
         self,
         experiment_id: str = None,
         request_id: str = None,
     ):
         self.experiment_id = experiment_id
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -612,15 +591,14 @@
         self,
         accessibility: str = None,
         name: str = None,
         parent_folder_id: str = None,
         source: str = None,
         workspace_id: str = None,
     ):
-        # 工作空间内可见性 PUBLIC; PRIVATE 默认PUBLIC
         self.accessibility = accessibility
         self.name = name
         self.parent_folder_id = parent_folder_id
         self.source = source
         self.workspace_id = workspace_id
 
     def validate(self):
@@ -662,15 +640,14 @@
 class CreateExperimentFolderResponseBody(TeaModel):
     def __init__(
         self,
         folder_id: str = None,
         request_id: str = None,
     ):
         self.folder_id = folder_id
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -765,15 +742,14 @@
 
 
 class CreateExperimentMigrateValidationResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -884,15 +860,14 @@
 class CreateJobResponseBody(TeaModel):
     def __init__(
         self,
         job_id: str = None,
         request_id: str = None,
     ):
         self.job_id = job_id
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -955,166 +930,19 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateJobResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CreateServiceRequestConfig(TeaModel):
-    def __init__(
-        self,
-        log_directory: str = None,
-    ):
-        self.log_directory = log_directory
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.log_directory is not None:
-            result['LogDirectory'] = self.log_directory
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('LogDirectory') is not None:
-            self.log_directory = m.get('LogDirectory')
-        return self
-
-
-class CreateServiceRequest(TeaModel):
-    def __init__(
-        self,
-        config: CreateServiceRequestConfig = None,
-        service_type: str = None,
-    ):
-        self.config = config
-        self.service_type = service_type
-
-    def validate(self):
-        if self.config:
-            self.config.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.config is not None:
-            result['Config'] = self.config.to_map()
-        if self.service_type is not None:
-            result['ServiceType'] = self.service_type
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Config') is not None:
-            temp_model = CreateServiceRequestConfig()
-            self.config = temp_model.from_map(m['Config'])
-        if m.get('ServiceType') is not None:
-            self.service_type = m.get('ServiceType')
-        return self
-
-
-class CreateServiceResponseBody(TeaModel):
-    def __init__(
-        self,
-        request_id: str = None,
-        service_id: str = None,
-        url: str = None,
-    ):
-        # Id of the request
-        self.request_id = request_id
-        self.service_id = service_id
-        self.url = url
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.service_id is not None:
-            result['ServiceId'] = self.service_id
-        if self.url is not None:
-            result['Url'] = self.url
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('ServiceId') is not None:
-            self.service_id = m.get('ServiceId')
-        if m.get('Url') is not None:
-            self.url = m.get('Url')
-        return self
-
-
-class CreateServiceResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: CreateServiceResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = CreateServiceResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DeleteExperimentResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1178,15 +1006,14 @@
 
 
 class DeleteExperimentFolderResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1245,86 +1072,14 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteExperimentFolderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DeleteServiceResponseBody(TeaModel):
-    def __init__(
-        self,
-        request_id: str = None,
-    ):
-        # Id of the request
-        self.request_id = request_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        return self
-
-
-class DeleteServiceResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: DeleteServiceResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = DeleteServiceResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class GetAlgoTreeRequest(TeaModel):
     def __init__(
         self,
         source: str = None,
     ):
         self.source = source
 
@@ -1351,15 +1106,14 @@
 class GetAlgoTreeResponseBody(TeaModel):
     def __init__(
         self,
         data: Dict[str, Any] = None,
         request_id: str = None,
     ):
         self.data = data
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1473,15 +1227,14 @@
 
 class GetAlgorithmDefResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         spec: Dict[str, Any] = None,
     ):
-        # Id of the request
         self.request_id = request_id
         self.spec = spec
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1596,15 +1349,14 @@
 
 class GetAlgorithmDefsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         specs: List[Dict[str, Any]] = None,
     ):
-        # Id of the request
         self.request_id = request_id
         self.specs = specs
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1672,45 +1424,50 @@
         return self
 
 
 class GetAlgorithmTreeRequest(TeaModel):
     def __init__(
         self,
         source: str = None,
+        workspace_id: str = None,
     ):
         self.source = source
+        self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.source is not None:
             result['Source'] = self.source
+        if self.workspace_id is not None:
+            result['WorkspaceId'] = self.workspace_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Source') is not None:
             self.source = m.get('Source')
+        if m.get('WorkspaceId') is not None:
+            self.workspace_id = m.get('WorkspaceId')
         return self
 
 
 class GetAlgorithmTreeResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         timestamp: str = None,
         tree: List[Dict[str, Any]] = None,
     ):
-        # Id of the request
         self.request_id = request_id
         self.timestamp = timestamp
         self.tree = tree
 
     def validate(self):
         pass
 
@@ -1805,15 +1562,14 @@
         self.creator = creator
         self.description = description
         self.experiment_id = experiment_id
         self.gmt_create_time = gmt_create_time
         self.gmt_modified_time = gmt_modified_time
         self.name = name
         self.options = options
-        # Id of the request
         self.request_id = request_id
         self.source = source
         self.version = version
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
@@ -1932,19 +1688,17 @@
         self,
         accessibility: str = None,
         only_folder: bool = None,
         source: str = None,
         user_id: str = None,
         workspace_id: str = None,
     ):
-        # 工作空间内可见性 PUBLIC; PRIVATE 默认PUBLIC
         self.accessibility = accessibility
         self.only_folder = only_folder
         self.source = source
-        # 若FolderId为root，Accessibility为PRIVATE，这里代表私有根路径的所有者，默认为访问者自己
         self.user_id = user_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1980,20 +1734,24 @@
         return self
 
 
 class GetExperimentFolderChildrenResponseBodyItems(TeaModel):
     def __init__(
         self,
         empty: bool = None,
+        gmt_create_time: str = None,
+        gmt_modified_time: str = None,
         icon: str = None,
         id: str = None,
         name: str = None,
         type: str = None,
     ):
         self.empty = empty
+        self.gmt_create_time = gmt_create_time
+        self.gmt_modified_time = gmt_modified_time
         self.icon = icon
         self.id = id
         self.name = name
         self.type = type
 
     def validate(self):
         pass
@@ -2002,28 +1760,36 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.empty is not None:
             result['Empty'] = self.empty
+        if self.gmt_create_time is not None:
+            result['GmtCreateTime'] = self.gmt_create_time
+        if self.gmt_modified_time is not None:
+            result['GmtModifiedTime'] = self.gmt_modified_time
         if self.icon is not None:
             result['Icon'] = self.icon
         if self.id is not None:
             result['Id'] = self.id
         if self.name is not None:
             result['Name'] = self.name
         if self.type is not None:
             result['Type'] = self.type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Empty') is not None:
             self.empty = m.get('Empty')
+        if m.get('GmtCreateTime') is not None:
+            self.gmt_create_time = m.get('GmtCreateTime')
+        if m.get('GmtModifiedTime') is not None:
+            self.gmt_modified_time = m.get('GmtModifiedTime')
         if m.get('Icon') is not None:
             self.icon = m.get('Icon')
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Type') is not None:
@@ -2035,15 +1801,14 @@
     def __init__(
         self,
         items: List[GetExperimentFolderChildrenResponseBodyItems] = None,
         request_id: str = None,
         total_count: int = None,
     ):
         self.items = items
-        # Id of the request
         self.request_id = request_id
         self.total_count = total_count
 
     def validate(self):
         if self.items:
             for k in self.items:
                 if k:
@@ -2143,15 +1908,14 @@
         self.creator = creator
         self.description = description
         self.experiment_id = experiment_id
         self.gmt_create_time = gmt_create_time
         self.gmt_modified_time = gmt_modified_time
         self.name = name
         self.options = options
-        # Id of the request
         self.request_id = request_id
         self.source = source
         self.version = version
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
@@ -2328,15 +2092,14 @@
     def __init__(
         self,
         nodes: List[GetExperimentStatusResponseBodyNodes] = None,
         request_id: str = None,
         status: str = None,
     ):
         self.nodes = nodes
-        # Id of the request
         self.request_id = request_id
         self.status = status
 
     def validate(self):
         if self.nodes:
             for k in self.nodes:
                 if k:
@@ -2485,15 +2248,14 @@
 class GetExperimentVisualizationMetaResponseBody(TeaModel):
     def __init__(
         self,
         visualization_meta: List[GetExperimentVisualizationMetaResponseBodyVisualizationMeta] = None,
         request_id: str = None,
     ):
         self.visualization_meta = visualization_meta
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         if self.visualization_meta:
             for k in self.visualization_meta:
                 if k:
                     k.validate()
@@ -2643,15 +2405,14 @@
 class GetExperimentsStatisticsResponseBody(TeaModel):
     def __init__(
         self,
         data: List[GetExperimentsStatisticsResponseBodyData] = None,
         request_id: str = None,
     ):
         self.data = data
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
@@ -2788,15 +2549,14 @@
 
 class GetExperimentsUsersStatisticsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         users: List[GetExperimentsUsersStatisticsResponseBodyUsers] = None,
     ):
-        # Id of the request
         self.request_id = request_id
         self.users = users
 
     def validate(self):
         if self.users:
             for k in self.users:
                 if k:
@@ -2873,15 +2633,14 @@
 
 
 class GetImageRequest(TeaModel):
     def __init__(
         self,
         verbose: bool = None,
     ):
-        # 是否显示非必要信息：Labels
         self.verbose = verbose
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2902,17 +2661,15 @@
 
 class GetImageResponseBodyLabels(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # Key
         self.key = key
-        # Value
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2944,31 +2701,22 @@
         image_uri: str = None,
         labels: List[GetImageResponseBodyLabels] = None,
         name: str = None,
         operator_create: str = None,
         parent_operator_create: str = None,
         request_id: str = None,
     ):
-        # 描述
         self.description = description
-        # 创建 UTC 时间，日期格式 iso8601
         self.gmt_create_time = gmt_create_time
-        # 创建 UTC 时间，日期格式 iso8601
         self.gmt_modified_time = gmt_modified_time
-        # 镜像地址，包含版本号
         self.image_uri = image_uri
-        # 镜像标签
         self.labels = labels
-        # 镜像名称
         self.name = name
-        # 创建人
         self.operator_create = operator_create
-        # 创建人父账户
         self.parent_operator_create = parent_operator_create
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         if self.labels:
             for k in self.labels:
                 if k:
                     k.validate()
@@ -3120,15 +2868,14 @@
         self.creator = creator
         self.execute_type = execute_type
         self.experiment_id = experiment_id
         self.gmt_create_time = gmt_create_time
         self.job_id = job_id
         self.node_id = node_id
         self.paiflow_node_id = paiflow_node_id
-        # Id of the request
         self.request_id = request_id
         self.run_id = run_id
         self.run_info = run_info
         self.snapshot = snapshot
         self.status = status
         self.workspace_id = workspace_id
 
@@ -3319,15 +3066,14 @@
         self,
         columns: List[GetMCTableSchemaResponseBodyColumns] = None,
         partition_columns: List[str] = None,
         request_id: str = None,
     ):
         self.columns = columns
         self.partition_columns = partition_columns
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         if self.columns:
             for k in self.columns:
                 if k:
                     k.validate()
@@ -3444,15 +3190,14 @@
         self,
         col_names: List[str] = None,
         col_types: List[str] = None,
         request_id: str = None,
     ):
         self.col_names = col_names
         self.col_types = col_types
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3561,15 +3306,14 @@
         type: str = None,
         value: Dict[str, Any] = None,
     ):
         self.algo_name = algo_name
         self.display_name = display_name
         self.location_type = location_type
         self.node_name = node_name
-        # Id of the request
         self.request_id = request_id
         self.type = type
         self.value = value
 
     def validate(self):
         pass
 
@@ -3689,15 +3433,14 @@
     def __init__(
         self,
         content: str = None,
         request_id: str = None,
         visualization_type: str = None,
     ):
         self.content = content
-        # Id of the request
         self.request_id = request_id
         self.visualization_type = visualization_type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3765,146 +3508,69 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetNodeVisualizationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetServiceRequest(TeaModel):
+class GetTemplateRequest(TeaModel):
     def __init__(
         self,
-        service_type: str = None,
-    ):
-        self.service_type = service_type
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.service_type is not None:
-            result['ServiceType'] = self.service_type
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('ServiceType') is not None:
-            self.service_type = m.get('ServiceType')
-        return self
-
-
-class GetServiceResponseBody(TeaModel):
-    def __init__(
-        self,
-        request_id: str = None,
-        service_id: str = None,
-        url: str = None,
+        verbose: bool = None,
     ):
-        # Id of the request
-        self.request_id = request_id
-        self.service_id = service_id
-        self.url = url
+        self.verbose = verbose
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.service_id is not None:
-            result['ServiceId'] = self.service_id
-        if self.url is not None:
-            result['Url'] = self.url
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('ServiceId') is not None:
-            self.service_id = m.get('ServiceId')
-        if m.get('Url') is not None:
-            self.url = m.get('Url')
-        return self
-
-
-class GetServiceResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: GetServiceResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        if self.verbose is not None:
+            result['Verbose'] = self.verbose
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = GetServiceResponseBody()
-            self.body = temp_model.from_map(m['body'])
+        if m.get('Verbose') is not None:
+            self.verbose = m.get('Verbose')
         return self
 
 
 class GetTemplateResponseBody(TeaModel):
     def __init__(
         self,
         content: str = None,
         description: str = None,
         detail: str = None,
         doc_link: str = None,
         image_link: str = None,
+        labels: List[Dict[str, Any]] = None,
         name: str = None,
         request_id: str = None,
+        source_id: str = None,
+        source_type: str = None,
         template_id: str = None,
+        template_type: str = None,
     ):
         self.content = content
         self.description = description
         self.detail = detail
         self.doc_link = doc_link
         self.image_link = image_link
+        self.labels = labels
         self.name = name
-        # Id of the request
         self.request_id = request_id
+        self.source_id = source_id
+        self.source_type = source_type
         self.template_id = template_id
+        self.template_type = template_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -3917,40 +3583,56 @@
             result['Description'] = self.description
         if self.detail is not None:
             result['Detail'] = self.detail
         if self.doc_link is not None:
             result['DocLink'] = self.doc_link
         if self.image_link is not None:
             result['ImageLink'] = self.image_link
+        if self.labels is not None:
+            result['Labels'] = self.labels
         if self.name is not None:
             result['Name'] = self.name
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        if self.source_id is not None:
+            result['SourceId'] = self.source_id
+        if self.source_type is not None:
+            result['SourceType'] = self.source_type
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
+        if self.template_type is not None:
+            result['TemplateType'] = self.template_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Content') is not None:
             self.content = m.get('Content')
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('Detail') is not None:
             self.detail = m.get('Detail')
         if m.get('DocLink') is not None:
             self.doc_link = m.get('DocLink')
         if m.get('ImageLink') is not None:
             self.image_link = m.get('ImageLink')
+        if m.get('Labels') is not None:
+            self.labels = m.get('Labels')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('SourceId') is not None:
+            self.source_id = m.get('SourceId')
+        if m.get('SourceType') is not None:
+            self.source_type = m.get('SourceType')
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
+        if m.get('TemplateType') is not None:
+            self.template_type = m.get('TemplateType')
         return self
 
 
 class GetTemplateResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -4077,15 +3759,14 @@
 class ListAlgoDefsResponseBody(TeaModel):
     def __init__(
         self,
         data: List[Dict[str, Any]] = None,
         request_id: str = None,
     ):
         self.data = data
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4285,15 +3966,14 @@
 
 class ListAuthRolesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         roles: List[ListAuthRolesResponseBodyRoles] = None,
     ):
-        # Id of the request
         self.request_id = request_id
         self.roles = roles
 
     def validate(self):
         if self.roles:
             for k in self.roles:
                 if k:
@@ -4529,15 +4209,14 @@
     def __init__(
         self,
         experiments: List[ListExperimentsResponseBodyExperiments] = None,
         request_id: str = None,
         total_count: int = None,
     ):
         self.experiments = experiments
-        # Id of the request
         self.request_id = request_id
         self.total_count = total_count
 
     def validate(self):
         if self.experiments:
             for k in self.experiments:
                 if k:
@@ -4620,19 +4299,16 @@
 class ListImageLabelsRequest(TeaModel):
     def __init__(
         self,
         image_id: str = None,
         label_filter: str = None,
         label_keys: str = None,
     ):
-        # 镜像id
         self.image_id = image_id
-        # image过滤条件，获取满足条件的image的所有label
         self.label_filter = label_filter
-        # 标签列表，以逗号分隔
         self.label_keys = label_keys
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4661,17 +4337,15 @@
 
 class ListImageLabelsResponseBodyLabels(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # 键
         self.key = key
-        # 值
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4697,19 +4371,16 @@
 class ListImageLabelsResponseBody(TeaModel):
     def __init__(
         self,
         labels: List[ListImageLabelsResponseBodyLabels] = None,
         total_count: int = None,
         request_id: str = None,
     ):
-        # 镜像标签
         self.labels = labels
-        # 符合过滤条件的数量
         self.total_count = total_count
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         if self.labels:
             for k in self.labels:
                 if k:
                     k.validate()
@@ -4795,27 +4466,20 @@
         name: str = None,
         order: str = None,
         page_number: int = None,
         page_size: int = None,
         sort_by: str = None,
         verbose: bool = None,
     ):
-        # 过滤值 以逗号分隔
         self.labels = labels
-        # 镜像名称，支持模糊搜索
         self.name = name
-        # 排序方向： ASC - 升序 DESC - 降序
         self.order = order
-        # 分页，从1开始，默认1
         self.page_number = page_number
-        # 页大小，默认20
         self.page_size = page_size
-        # 排序字段
         self.sort_by = sort_by
-        # 是否显示非必要信息：Labels
         self.verbose = verbose
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4860,17 +4524,15 @@
 
 class ListImagesResponseBodyImagesLabels(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # Key
         self.key = key
-        # Value
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4899,25 +4561,19 @@
         description: str = None,
         gmt_create_time: str = None,
         image_id: str = None,
         image_uri: str = None,
         labels: List[ListImagesResponseBodyImagesLabels] = None,
         name: str = None,
     ):
-        # 镜像描述
         self.description = description
-        # 创建 UTC 时间，日期格式 iso8601
         self.gmt_create_time = gmt_create_time
-        # 镜像id
         self.image_id = image_id
-        # 镜像地址，包含版本号
         self.image_uri = image_uri
-        # 镜像标签，是个map
         self.labels = labels
-        # 镜像名称
         self.name = name
 
     def validate(self):
         if self.labels:
             for k in self.labels:
                 if k:
                     k.validate()
@@ -4967,19 +4623,16 @@
 class ListImagesResponseBody(TeaModel):
     def __init__(
         self,
         images: List[ListImagesResponseBodyImages] = None,
         total_count: int = None,
         request_id: str = None,
     ):
-        # 镜像列表
         self.images = images
-        # 总数
         self.total_count = total_count
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         if self.images:
             for k in self.images:
                 if k:
                     k.validate()
@@ -5193,15 +4846,14 @@
 class ListJobsResponseBody(TeaModel):
     def __init__(
         self,
         jobs: List[ListJobsResponseBodyJobs] = None,
         request_id: str = None,
     ):
         self.jobs = jobs
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         if self.jobs:
             for k in self.jobs:
                 if k:
                     k.validate()
@@ -5348,15 +5000,14 @@
 class ListNodeOutputsResponseBody(TeaModel):
     def __init__(
         self,
         outputs: List[ListNodeOutputsResponseBodyOutputs] = None,
         request_id: str = None,
     ):
         self.outputs = outputs
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         if self.outputs:
             for k in self.outputs:
                 if k:
                     k.validate()
@@ -5561,15 +5212,14 @@
     def __init__(
         self,
         experiments: List[ListRecentExperimentsResponseBodyExperiments] = None,
         request_id: str = None,
         total_count: int = None,
     ):
         self.experiments = experiments
-        # Id of the request
         self.request_id = request_id
         self.total_count = total_count
 
     def validate(self):
         if self.experiments:
             for k in self.experiments:
                 if k:
@@ -5645,291 +5295,193 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListRecentExperimentsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListServicesRequest(TeaModel):
-    def __init__(
-        self,
-        service_type: str = None,
-        workspace_id: str = None,
-    ):
-        self.service_type = service_type
-        self.workspace_id = workspace_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.service_type is not None:
-            result['ServiceType'] = self.service_type
-        if self.workspace_id is not None:
-            result['WorkspaceId'] = self.workspace_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('ServiceType') is not None:
-            self.service_type = m.get('ServiceType')
-        if m.get('WorkspaceId') is not None:
-            self.workspace_id = m.get('WorkspaceId')
-        return self
-
-
-class ListServicesResponseBodyServices(TeaModel):
-    def __init__(
-        self,
-        service_id: str = None,
-        url: str = None,
-    ):
-        self.service_id = service_id
-        self.url = url
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.service_id is not None:
-            result['ServiceId'] = self.service_id
-        if self.url is not None:
-            result['Url'] = self.url
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('ServiceId') is not None:
-            self.service_id = m.get('ServiceId')
-        if m.get('Url') is not None:
-            self.url = m.get('Url')
-        return self
-
-
-class ListServicesResponseBody(TeaModel):
-    def __init__(
-        self,
-        request_id: str = None,
-        services: List[ListServicesResponseBodyServices] = None,
-        total_count: int = None,
-    ):
-        # Id of the request
-        self.request_id = request_id
-        self.services = services
-        self.total_count = total_count
-
-    def validate(self):
-        if self.services:
-            for k in self.services:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        result['Services'] = []
-        if self.services is not None:
-            for k in self.services:
-                result['Services'].append(k.to_map() if k else None)
-        if self.total_count is not None:
-            result['TotalCount'] = self.total_count
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        self.services = []
-        if m.get('Services') is not None:
-            for k in m.get('Services'):
-                temp_model = ListServicesResponseBodyServices()
-                self.services.append(temp_model.from_map(k))
-        if m.get('TotalCount') is not None:
-            self.total_count = m.get('TotalCount')
-        return self
-
-
-class ListServicesResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: ListServicesResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = ListServicesResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class ListTemplatesRequest(TeaModel):
     def __init__(
         self,
+        label: str = None,
         list: str = None,
+        name: str = None,
         order: str = None,
         page_number: int = None,
         page_size: int = None,
+        sort_by: str = None,
         source: str = None,
         tag_id: str = None,
+        template_type: str = None,
         type_id: str = None,
+        verbose: bool = None,
+        workspace_id: str = None,
     ):
+        self.label = label
         self.list = list
+        self.name = name
         self.order = order
         self.page_number = page_number
         self.page_size = page_size
+        self.sort_by = sort_by
         self.source = source
         self.tag_id = tag_id
+        self.template_type = template_type
         self.type_id = type_id
+        self.verbose = verbose
+        self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.label is not None:
+            result['Label'] = self.label
         if self.list is not None:
             result['List'] = self.list
+        if self.name is not None:
+            result['Name'] = self.name
         if self.order is not None:
             result['Order'] = self.order
         if self.page_number is not None:
             result['PageNumber'] = self.page_number
         if self.page_size is not None:
             result['PageSize'] = self.page_size
+        if self.sort_by is not None:
+            result['SortBy'] = self.sort_by
         if self.source is not None:
             result['Source'] = self.source
         if self.tag_id is not None:
             result['TagId'] = self.tag_id
+        if self.template_type is not None:
+            result['TemplateType'] = self.template_type
         if self.type_id is not None:
             result['TypeId'] = self.type_id
+        if self.verbose is not None:
+            result['Verbose'] = self.verbose
+        if self.workspace_id is not None:
+            result['WorkspaceId'] = self.workspace_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Label') is not None:
+            self.label = m.get('Label')
         if m.get('List') is not None:
             self.list = m.get('List')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
         if m.get('Order') is not None:
             self.order = m.get('Order')
         if m.get('PageNumber') is not None:
             self.page_number = m.get('PageNumber')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
+        if m.get('SortBy') is not None:
+            self.sort_by = m.get('SortBy')
         if m.get('Source') is not None:
             self.source = m.get('Source')
         if m.get('TagId') is not None:
             self.tag_id = m.get('TagId')
+        if m.get('TemplateType') is not None:
+            self.template_type = m.get('TemplateType')
         if m.get('TypeId') is not None:
             self.type_id = m.get('TypeId')
+        if m.get('Verbose') is not None:
+            self.verbose = m.get('Verbose')
+        if m.get('WorkspaceId') is not None:
+            self.workspace_id = m.get('WorkspaceId')
         return self
 
 
 class ListTemplatesResponseBodyTemplateDataTemplate(TeaModel):
     def __init__(
         self,
         content: str = None,
+        creator: str = None,
         description: str = None,
         detail: str = None,
         doc_link: str = None,
+        gmt_create_time: str = None,
+        gmt_modified_time: str = None,
         image_link: str = None,
+        labels: List[Dict[str, Any]] = None,
         name: str = None,
         template_id: str = None,
     ):
         self.content = content
+        self.creator = creator
         self.description = description
         self.detail = detail
         self.doc_link = doc_link
+        self.gmt_create_time = gmt_create_time
+        self.gmt_modified_time = gmt_modified_time
         self.image_link = image_link
+        self.labels = labels
         self.name = name
         self.template_id = template_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.content is not None:
             result['Content'] = self.content
+        if self.creator is not None:
+            result['Creator'] = self.creator
         if self.description is not None:
             result['Description'] = self.description
         if self.detail is not None:
             result['Detail'] = self.detail
         if self.doc_link is not None:
             result['DocLink'] = self.doc_link
+        if self.gmt_create_time is not None:
+            result['GmtCreateTime'] = self.gmt_create_time
+        if self.gmt_modified_time is not None:
+            result['GmtModifiedTime'] = self.gmt_modified_time
         if self.image_link is not None:
             result['ImageLink'] = self.image_link
+        if self.labels is not None:
+            result['Labels'] = self.labels
         if self.name is not None:
             result['Name'] = self.name
         if self.template_id is not None:
             result['TemplateId'] = self.template_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Content') is not None:
             self.content = m.get('Content')
+        if m.get('Creator') is not None:
+            self.creator = m.get('Creator')
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('Detail') is not None:
             self.detail = m.get('Detail')
         if m.get('DocLink') is not None:
             self.doc_link = m.get('DocLink')
+        if m.get('GmtCreateTime') is not None:
+            self.gmt_create_time = m.get('GmtCreateTime')
+        if m.get('GmtModifiedTime') is not None:
+            self.gmt_modified_time = m.get('GmtModifiedTime')
         if m.get('ImageLink') is not None:
             self.image_link = m.get('ImageLink')
+        if m.get('Labels') is not None:
+            self.labels = m.get('Labels')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         return self
 
 
@@ -6055,15 +5607,14 @@
 class ListTemplatesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         template_data: List[ListTemplatesResponseBodyTemplateData] = None,
         total_count: int = None,
     ):
-        # Id of the request
         self.request_id = request_id
         self.template_data = template_data
         self.total_count = total_count
 
     def validate(self):
         if self.template_data:
             for k in self.template_data:
@@ -6190,15 +5741,14 @@
         folder_id_mapping: Dict[str, dict] = None,
         message: str = None,
         request_id: str = None,
     ):
         self.code = code
         self.folder_id_mapping = folder_id_mapping
         self.message = message
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6376,15 +5926,14 @@
         data: MigrateExperimentsResponseBodyData = None,
         message: str = None,
         request_id: str = None,
     ):
         self.code = code
         self.data = data
         self.message = message
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -6461,57 +6010,62 @@
         return self
 
 
 class PreviewMCTableRequest(TeaModel):
     def __init__(
         self,
         endpoint: str = None,
+        limit: int = None,
         partition: str = None,
         workspace_id: str = None,
     ):
         self.endpoint = endpoint
+        self.limit = limit
         self.partition = partition
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.endpoint is not None:
             result['Endpoint'] = self.endpoint
+        if self.limit is not None:
+            result['Limit'] = self.limit
         if self.partition is not None:
             result['Partition'] = self.partition
         if self.workspace_id is not None:
             result['WorkspaceId'] = self.workspace_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Endpoint') is not None:
             self.endpoint = m.get('Endpoint')
+        if m.get('Limit') is not None:
+            self.limit = m.get('Limit')
         if m.get('Partition') is not None:
             self.partition = m.get('Partition')
         if m.get('WorkspaceId') is not None:
             self.workspace_id = m.get('WorkspaceId')
         return self
 
 
 class PreviewMCTableResponseBody(TeaModel):
     def __init__(
         self,
         content: List[List[str]] = None,
         request_id: str = None,
     ):
         self.content = content
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6579,15 +6133,14 @@
 
 
 class PublishExperimentRequest(TeaModel):
     def __init__(
         self,
         folder_id: str = None,
     ):
-        # 公共目录Id
         self.folder_id = folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6607,15 +6160,14 @@
 
 
 class PublishExperimentResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6682,21 +6234,17 @@
     def __init__(
         self,
         end_time: str = None,
         node_id: str = None,
         start_time: str = None,
         visualization_data_ids: List[str] = None,
     ):
-        # 结束时间，UTC 时间，日期格式 iso8601，闭区间，对流算法必填
         self.end_time = end_time
-        # node id
         self.node_id = node_id
-        # 开始时间，UTC 时间，日期格式 iso8601，闭区间，对流算法必选
         self.start_time = start_time
-        # dataId列表
         self.visualization_data_ids = visualization_data_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6810,15 +6358,14 @@
 class QueryExperimentVisualizationDataResponseBody(TeaModel):
     def __init__(
         self,
         visualization_data: List[QueryExperimentVisualizationDataResponseBodyVisualizationData] = None,
         request_id: str = None,
     ):
         self.visualization_data = visualization_data
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         if self.visualization_data:
             for k in self.visualization_data:
                 if k:
                     k.validate()
@@ -6894,15 +6441,14 @@
 
 
 class RemoveImageResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6966,15 +6512,14 @@
 
 
 class RemoveImageLabelsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7072,15 +6617,14 @@
 
 class SearchMCTablesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tables: List[str] = None,
     ):
-        # Id of the request
         self.request_id = request_id
         self.tables = tables
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -7149,15 +6693,14 @@
 
 
 class StopExperimentResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7221,15 +6764,14 @@
 
 
 class StopJobResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7327,15 +6869,14 @@
 
 class UpdateExperimentContentResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         version: int = None,
     ):
-        # Id of the request
         self.request_id = request_id
         self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -7437,15 +6978,14 @@
 
 
 class UpdateExperimentFolderResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7513,15 +7053,14 @@
         self,
         accessibility: str = None,
         description: str = None,
         folder_id: str = None,
         name: str = None,
         options: str = None,
     ):
-        # 工作空间内可见性 PUBLIC; PRIVATE 默认PUBLIC
         self.accessibility = accessibility
         self.description = description
         self.folder_id = folder_id
         self.name = name
         self.options = options
 
     def validate(self):
@@ -7561,15 +7100,14 @@
 
 
 class UpdateExperimentMetaResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alibabacloud_paistudio20210202-1.0.26/alibabacloud_paistudio20210202.egg-info/PKG-INFO` & `alibabacloud_paistudio20210202-1.0.27/alibabacloud_paistudio20210202.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-paistudio20210202
-Version: 1.0.26
+Version: 1.0.27
 Summary: Alibaba Cloud PaiStudio (20210202) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_paistudio20210202-1.0.26/setup.py` & `alibabacloud_paistudio20210202-1.0.27/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_paistudio20210202.
 
-Created on 30/06/2022
+Created on 28/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_paistudio20210202"
 NAME = "alibabacloud_paistudio20210202" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud PaiStudio (20210202) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

