# Comparing `tmp/cohere-sagemaker-0.7.1.tar.gz` & `tmp/cohere-sagemaker-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-sagemaker-0.7.1.tar", last modified: Thu Jul 13 11:25:18 2023, max compression
+gzip compressed data, was "cohere-sagemaker-0.7.2.tar", last modified: Fri Jul 28 01:04:38 2023, max compression
```

## Comparing `cohere-sagemaker-0.7.1.tar` & `cohere-sagemaker-0.7.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        0 2023-07-13 11:25:18.970277 cohere-sagemaker-0.7.1/
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1066 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/LICENSE
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1412 2023-07-13 11:25:18.970277 cohere-sagemaker-0.7.1/PKG-INFO
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      948 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/README.md
-drwxr-xr-x   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        0 2023-07-13 11:25:18.966277 cohere-sagemaker-0.7.1/cohere_sagemaker/
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       57 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/__init__.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1222 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/classification.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)    21487 2023-07-13 11:05:48.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/client.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      623 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/embeddings.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      591 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/error.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      796 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/generation.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     2069 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/rerank.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      337 2023-07-11 10:58:17.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/response.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      491 2023-07-13 11:04:25.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/summary.py
-drwxr-xr-x   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        0 2023-07-13 11:25:18.970277 cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1412 2023-07-13 11:25:18.000000 cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      488 2023-07-13 11:25:18.000000 cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        1 2023-07-13 11:25:18.000000 cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       16 2023-07-13 11:25:18.000000 cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/requires.txt
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       17 2023-07-13 11:25:18.000000 cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       38 2023-07-13 11:25:18.970277 cohere-sagemaker-0.7.1/setup.cfg
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1525 2023-07-13 11:25:09.000000 cohere-sagemaker-0.7.1/setup.py
+drwxr-xr-x   0 hemantj    (502) staff       (20)        0 2023-07-28 01:04:38.195476 cohere-sagemaker-0.7.2/
+-rw-r--r--   0 hemantj    (502) staff       (20)     1066 2022-11-23 18:02:25.000000 cohere-sagemaker-0.7.2/LICENSE
+-rw-r--r--   0 hemantj    (502) staff       (20)     1412 2023-07-28 01:04:38.195281 cohere-sagemaker-0.7.2/PKG-INFO
+-rw-r--r--   0 hemantj    (502) staff       (20)      948 2023-07-19 20:01:10.000000 cohere-sagemaker-0.7.2/README.md
+drwxr-xr-x   0 hemantj    (502) staff       (20)        0 2023-07-28 01:04:38.194027 cohere-sagemaker-0.7.2/cohere_sagemaker/
+-rw-r--r--   0 hemantj    (502) staff       (20)       57 2022-11-23 18:02:25.000000 cohere-sagemaker-0.7.2/cohere_sagemaker/__init__.py
+-rw-r--r--   0 hemantj    (502) staff       (20)     1222 2023-07-19 20:01:10.000000 cohere-sagemaker-0.7.2/cohere_sagemaker/classification.py
+-rw-r--r--   0 hemantj    (502) staff       (20)    21451 2023-07-24 18:07:17.000000 cohere-sagemaker-0.7.2/cohere_sagemaker/client.py
+-rw-r--r--   0 hemantj    (502) staff       (20)      623 2023-07-19 20:01:10.000000 cohere-sagemaker-0.7.2/cohere_sagemaker/embeddings.py
+-rw-r--r--   0 hemantj    (502) staff       (20)      591 2022-11-23 18:02:25.000000 cohere-sagemaker-0.7.2/cohere_sagemaker/error.py
+-rw-r--r--   0 hemantj    (502) staff       (20)      796 2023-07-19 20:01:10.000000 cohere-sagemaker-0.7.2/cohere_sagemaker/generation.py
+-rw-r--r--   0 hemantj    (502) staff       (20)     2069 2023-07-19 20:01:10.000000 cohere-sagemaker-0.7.2/cohere_sagemaker/rerank.py
+-rw-r--r--   0 hemantj    (502) staff       (20)      337 2022-11-23 18:02:25.000000 cohere-sagemaker-0.7.2/cohere_sagemaker/response.py
+-rw-r--r--   0 hemantj    (502) staff       (20)      491 2023-07-19 20:01:10.000000 cohere-sagemaker-0.7.2/cohere_sagemaker/summary.py
+drwxr-xr-x   0 hemantj    (502) staff       (20)        0 2023-07-28 01:04:38.194959 cohere-sagemaker-0.7.2/cohere_sagemaker.egg-info/
+-rw-r--r--   0 hemantj    (502) staff       (20)     1412 2023-07-28 01:04:38.000000 cohere-sagemaker-0.7.2/cohere_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 hemantj    (502) staff       (20)      488 2023-07-28 01:04:38.000000 cohere-sagemaker-0.7.2/cohere_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 hemantj    (502) staff       (20)        1 2023-07-28 01:04:38.000000 cohere-sagemaker-0.7.2/cohere_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 hemantj    (502) staff       (20)       16 2023-07-28 01:04:38.000000 cohere-sagemaker-0.7.2/cohere_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 hemantj    (502) staff       (20)       17 2023-07-28 01:04:38.000000 cohere-sagemaker-0.7.2/cohere_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 hemantj    (502) staff       (20)       38 2023-07-28 01:04:38.195532 cohere-sagemaker-0.7.2/setup.cfg
+-rw-r--r--   0 hemantj    (502) staff       (20)     1525 2023-07-24 18:07:03.000000 cohere-sagemaker-0.7.2/setup.py
```

### Comparing `cohere-sagemaker-0.7.1/LICENSE` & `cohere-sagemaker-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.1/PKG-INFO` & `cohere-sagemaker-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere-sagemaker
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker
 Home-page: https://github.com/cohere-ai/cohere-sagemaker
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cohere-sagemaker-0.7.1/README.md` & `cohere-sagemaker-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.1/cohere_sagemaker/classification.py` & `cohere-sagemaker-0.7.2/cohere_sagemaker/classification.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.1/cohere_sagemaker/client.py` & `cohere-sagemaker-0.7.2/cohere_sagemaker/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,33 +405,33 @@
             eval_data (str, optional): An S3 path pointing to the eval data. Defaults to None.
             instance_type (str, optional): The EC2 instance type to use for training. Defaults to "ml.g4dn.xlarge".
             training_parameters (Dict[str, Any], optional): Additional training parameters. Defaults to {}.
             rool (str, optional): The IAM role to use for the endpoint. If not provided, sagemaker.get_execution_role()
                 will be used to get the role. This should work when one uses the client inside SageMaker. If this errors
                 out, the default role "ServiceRoleSagemaker" will be used, which generally works outside of SageMaker.
         """
-        assert len(training_parameters) == 0, "training_parameters not yet supported."
         assert name != "model", "name cannot be 'model'"
         s3_models_dir = s3_models_dir + ("/" if not s3_models_dir.endswith("/") else "")
 
         if role is None:
             try:
                 role = sage.get_execution_role()
             except ValueError:
                 print("Using default role: 'ServiceRoleSagemaker'.")
                 role = "ServiceRoleSagemaker"
 
+        training_parameters.update({"name": name})
         estimator = sage.algorithm.AlgorithmEstimator(
             algorithm_arn=arn,
             role=role,
             instance_count=1,
             instance_type=instance_type,
             sagemaker_session=self._sess,
             output_path=s3_models_dir,
-            hyperparameters={"name": name},
+            hyperparameters=training_parameters,
         )
 
         inputs = {}
         if not train_data.startswith("s3:"):
             raise ValueError("train_data must point to an S3 location.")
         inputs["training"] = train_data
         if eval_data is not None:
@@ -444,15 +444,15 @@
         current_filepath = f"{s3_models_dir}{job_name}/output/model.tar.gz"
 
         s3_resource = boto3.resource("s3")
 
         # Copy new model to root of output_model_dir
         bucket, old_key = parse_s3_url(current_filepath)
         _, new_key = parse_s3_url(f"{s3_models_dir}{name}.tar.gz")
-        s3_resource.Object(bucket, new_key).copy_from(CopySource={"Bucket": bucket, "Key": old_key})
+        s3_resource.Object(bucket, new_key).copy(CopySource={"Bucket": bucket, "Key": old_key})
 
         # Delete old dir
         bucket, old_short_key = parse_s3_url(s3_models_dir + job_name)
         s3_resource.Bucket(bucket).objects.filter(Prefix=old_short_key).delete()
 
     def summarize(
         self,
```

### Comparing `cohere-sagemaker-0.7.1/cohere_sagemaker/embeddings.py` & `cohere-sagemaker-0.7.2/cohere_sagemaker/embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.1/cohere_sagemaker/error.py` & `cohere-sagemaker-0.7.2/cohere_sagemaker/error.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.1/cohere_sagemaker/generation.py` & `cohere-sagemaker-0.7.2/cohere_sagemaker/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.1/cohere_sagemaker/rerank.py` & `cohere-sagemaker-0.7.2/cohere_sagemaker/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/PKG-INFO` & `cohere-sagemaker-0.7.2/cohere_sagemaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere-sagemaker
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker
 Home-page: https://github.com/cohere-ai/cohere-sagemaker
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cohere-sagemaker-0.7.1/setup.py` & `cohere-sagemaker-0.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         return False
 
     def has_ext_modules(foo) -> bool:
         return True
 
 
 setuptools.setup(name='cohere-sagemaker',
-                 version='0.7.1',
+                 version='0.7.2',
                  author='Cohere',
                  author_email='support@cohere.ai',
                  description='A Python library for the Cohere endpoints in AWS Sagemaker',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://github.com/cohere-ai/cohere-sagemaker',
                  packages=setuptools.find_packages(),
```

