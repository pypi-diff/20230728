# Comparing `tmp/audioshake_job_manager-0.0.4.tar.gz` & `tmp/audioshake_job_manager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioshake_job_manager-0.0.4.tar", last modified: Wed Jul 26 17:55:22 2023, max compression
+gzip compressed data, was "audioshake_job_manager-0.0.5.tar", last modified: Fri Jul 28 15:03:50 2023, max compression
```

## Comparing `audioshake_job_manager-0.0.4.tar` & `audioshake_job_manager-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 17:55:22.605971 audioshake_job_manager-0.0.4/
--rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 17:55:22.605543 audioshake_job_manager-0.0.4/PKG-INFO
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 17:55:22.602424 audioshake_job_manager-0.0.4/audioshake_job_manager/
--rw-r--r--   0 theslyguy   (501) staff       (20)     3680 2023-07-26 17:54:58.000000 audioshake_job_manager-0.0.4/audioshake_job_manager/__init__.py
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 17:55:22.604960 audioshake_job_manager-0.0.4/audioshake_job_manager.egg-info/
--rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 17:55:22.000000 audioshake_job_manager-0.0.4/audioshake_job_manager.egg-info/PKG-INFO
--rw-r--r--   0 theslyguy   (501) staff       (20)      278 2023-07-26 17:55:22.000000 audioshake_job_manager-0.0.4/audioshake_job_manager.egg-info/SOURCES.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)        1 2023-07-26 17:55:22.000000 audioshake_job_manager-0.0.4/audioshake_job_manager.egg-info/dependency_links.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)        6 2023-07-26 17:55:22.000000 audioshake_job_manager-0.0.4/audioshake_job_manager.egg-info/requires.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)       23 2023-07-26 17:55:22.000000 audioshake_job_manager-0.0.4/audioshake_job_manager.egg-info/top_level.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)      395 2023-07-26 17:55:11.000000 audioshake_job_manager-0.0.4/pyproject.toml
--rw-r--r--   0 theslyguy   (501) staff       (20)       38 2023-07-26 17:55:22.606117 audioshake_job_manager-0.0.4/setup.cfg
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-28 15:03:50.718555 audioshake_job_manager-0.0.5/
+-rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-28 15:03:50.718163 audioshake_job_manager-0.0.5/PKG-INFO
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-28 15:03:50.716057 audioshake_job_manager-0.0.5/audioshake_job_manager/
+-rw-r--r--   0 theslyguy   (501) staff       (20)     3783 2023-07-28 15:01:47.000000 audioshake_job_manager-0.0.5/audioshake_job_manager/__init__.py
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-28 15:03:50.717666 audioshake_job_manager-0.0.5/audioshake_job_manager.egg-info/
+-rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-28 15:03:50.000000 audioshake_job_manager-0.0.5/audioshake_job_manager.egg-info/PKG-INFO
+-rw-r--r--   0 theslyguy   (501) staff       (20)      278 2023-07-28 15:03:50.000000 audioshake_job_manager-0.0.5/audioshake_job_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)        1 2023-07-28 15:03:50.000000 audioshake_job_manager-0.0.5/audioshake_job_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)        6 2023-07-28 15:03:50.000000 audioshake_job_manager-0.0.5/audioshake_job_manager.egg-info/requires.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)       23 2023-07-28 15:03:50.000000 audioshake_job_manager-0.0.5/audioshake_job_manager.egg-info/top_level.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)      395 2023-07-28 15:03:31.000000 audioshake_job_manager-0.0.5/pyproject.toml
+-rw-r--r--   0 theslyguy   (501) staff       (20)       38 2023-07-28 15:03:50.718662 audioshake_job_manager-0.0.5/setup.cfg
```

### Comparing `audioshake_job_manager-0.0.4/audioshake_job_manager/__init__.py` & `audioshake_job_manager-0.0.5/audioshake_job_manager/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 import os
 import abc
 
 import boto3
 
 AWS_REGION = os.environ.get("AWS_REGION", "us-east-1")
 AWS_ENDPOINT_URL = os.environ.get("AWS_ENDPOINT_URL", None)
+QUEUE_URL = os.environ.get("QUEUE_URL", "")
 
 JOB_TIMEOUT = int(os.environ.get("JOB_TIMEOUT", "60"))
 
 logger = logging.getLogger(__name__)
 
 
 class JobManager:
     __metaclass__ = abc.ABCMeta
 
     def __init__(
-        self, queue_url: str, max_number_of_message: int = 10, batch_size: int = 1
+        self,
+        queue_url: str = None,
+        max_number_of_message: int = 10,
+        batch_size: int = 1,
     ):
         self.max_number_of_message = max_number_of_message
-        self.queue_url = queue_url
+        self.queue_url = queue_url or QUEUE_URL
         # NOTE to be used for batching messages read from the queue.
         self.batch_size = batch_size
 
         self.sqs_client = boto3.client(
             "sqs", region_name=AWS_REGION, endpoint_url=AWS_ENDPOINT_URL
         )
         self.step_function_client = boto3.client(
@@ -95,15 +99,15 @@
                 logger.exception(error_message)
             finally:
                 self.sqs_client.delete_message(
                     QueueUrl=self.queue_url, ReceiptHandle=cache[future._id]["job_id"]
                 )
                 self.step_function_client.send_task_success(
                     taskToken=cache[future._id]["task_token"],
-                    output=json.dumps(response),
+                    output=json.dumps(response, default=vars),
                 )
 
     @abc.abstractmethod
     def process(self, payload: str) -> Future:
         raise NotImplementedError("")
 
     @abc.abstractmethod
```

