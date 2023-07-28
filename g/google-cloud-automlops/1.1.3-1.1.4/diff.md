# Comparing `tmp/google-cloud-automlops-1.1.3.tar.gz` & `tmp/google-cloud-automlops-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-automlops-1.1.3.tar", last modified: Fri Jul  7 16:21:21 2023, max compression
+gzip compressed data, was "google-cloud-automlops-1.1.4.tar", last modified: Fri Jul 28 18:40:58 2023, max compression
```

## Comparing `google-cloud-automlops-1.1.3.tar` & `google-cloud-automlops-1.1.4.tar`

### file list

```diff
@@ -1,54 +1,62 @@
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.187656 google-cloud-automlops-1.1.3/
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.180937 google-cloud-automlops-1.1.3/AutoMLOps/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    16076 2023-07-07 16:05:45.000000 google-cloud-automlops-1.1.3/AutoMLOps/AutoMLOps.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2023-07-07 16:21:06.000000 google-cloud-automlops-1.1.3/AutoMLOps/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.181115 google-cloud-automlops-1.1.3/AutoMLOps/deployments/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/deployments/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.181450 google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2258 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/builder.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.181774 google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/constructs/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)        0 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/constructs/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9302 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/constructs/scripts.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.182131 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2271 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/base.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.182642 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11141 2023-06-06 12:45:38.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/builder.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.183957 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    20750 2023-07-07 16:05:45.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/cloudrun.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3711 2023-07-07 01:44:52.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/component.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8842 2023-07-07 01:45:27.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/pipeline.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    25214 2023-07-07 16:05:45.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/scripts.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8731 2023-06-06 12:45:38.000000 google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/scaffold.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.184651 google-cloud-automlops-1.1.3/AutoMLOps/utils/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/AutoMLOps/utils/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3229 2023-07-07 16:05:45.000000 google-cloud-automlops-1.1.3/AutoMLOps/utils/constants.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9886 2023-07-07 01:45:42.000000 google-cloud-automlops-1.1.3/AutoMLOps/utils/utils.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google-cloud-automlops-1.1.3/LICENSE
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14008 2023-07-07 16:21:21.187439 google-cloud-automlops-1.1.3/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13140 2023-07-07 16:05:45.000000 google-cloud-automlops-1.1.3/README.md
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.185561 google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14008 2023-07-07 16:21:21.000000 google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1265 2023-07-07 16:21:21.000000 google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/SOURCES.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2023-07-07 16:21:21.000000 google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/dependency_links.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       79 2023-07-07 16:21:21.000000 google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/requires.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       16 2023-07-07 16:21:21.000000 google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/top_level.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2023-07-07 16:21:21.187703 google-cloud-automlops-1.1.3/setup.cfg
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1949 2023-07-07 16:20:51.000000 google-cloud-automlops-1.1.3/setup.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.185735 google-cloud-automlops-1.1.3/tests/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.186102 google-cloud-automlops-1.1.3/tests/unit/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      702 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/unit/AutoMLOps_test.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/unit/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.186501 google-cloud-automlops-1.1.3/tests/unit/deployments/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/unit/deployments/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.186674 google-cloud-automlops-1.1.3/tests/unit/frameworks/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/unit/frameworks/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.186851 google-cloud-automlops-1.1.3/tests/unit/frameworks/kfp/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/unit/frameworks/kfp/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-07 16:21:21.187204 google-cloud-automlops-1.1.3/tests/unit/utils/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-05-18 17:07:03.000000 google-cloud-automlops-1.1.3/tests/unit/utils/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11523 2023-06-06 12:45:38.000000 google-cloud-automlops-1.1.3/tests/unit/utils/utils_test.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.580439 google-cloud-automlops-1.1.4/
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.571569 google-cloud-automlops-1.1.4/AutoMLOps/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    15964 2023-07-28 15:38:11.000000 google-cloud-automlops-1.1.4/AutoMLOps/AutoMLOps.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2023-07-25 21:27:56.000000 google-cloud-automlops-1.1.4/AutoMLOps/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.571734 google-cloud-automlops-1.1.4/AutoMLOps/deployments/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/deployments/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.572271 google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2258 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/builder.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.572606 google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/constructs/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)        0 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/constructs/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9302 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/constructs/scripts.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.573140 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2271 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/base.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.573652 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11384 2023-07-28 15:31:24.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/builder.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.574841 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    20732 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/cloudrun.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3711 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/component.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9207 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/pipeline.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    29657 2023-07-28 15:37:31.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/scripts.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8714 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/scaffold.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.575471 google-cloud-automlops-1.1.4/AutoMLOps/utils/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/utils/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3229 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/utils/constants.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    10106 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/utils/utils.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google-cloud-automlops-1.1.4/LICENSE
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14825 2023-07-28 18:40:58.580250 google-cloud-automlops-1.1.4/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13957 2023-07-28 15:52:25.000000 google-cloud-automlops-1.1.4/README.md
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.576433 google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14825 2023-07-28 18:40:58.000000 google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1621 2023-07-28 18:40:58.000000 google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/SOURCES.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2023-07-28 18:40:58.000000 google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/dependency_links.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       79 2023-07-28 18:40:58.000000 google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/requires.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       16 2023-07-28 18:40:58.000000 google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/top_level.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2023-07-28 18:40:58.580486 google-cloud-automlops-1.1.4/setup.cfg
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1949 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/setup.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.576676 google-cloud-automlops-1.1.4/tests/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/tests/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.576835 google-cloud-automlops-1.1.4/tests/unit/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/tests/unit/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.577162 google-cloud-automlops-1.1.4/tests/unit/deployments/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/tests/unit/deployments/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.577504 google-cloud-automlops-1.1.4/tests/unit/frameworks/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     4438 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/base_test.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.578240 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    12725 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/builder_test.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.579456 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:59.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    21114 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/cloudrun_test.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     5358 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/component_test.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9119 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/pipeline_test.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    24644 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/scripts_test.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9008 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/scaffold_test.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.579989 google-cloud-automlops-1.1.4/tests/unit/utils/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/tests/unit/utils/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    18039 2023-07-28 16:03:01.000000 google-cloud-automlops-1.1.4/tests/unit/utils/utils_test.py
```

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/AutoMLOps.py` & `google-cloud-automlops-1.1.4/AutoMLOps/AutoMLOps.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,14 @@
 
     # Check for remote origin url mismatch
     actual_remote = subprocess.check_output(['git config --get remote.origin.url'], shell=True, stderr=subprocess.STDOUT).decode('utf-8').strip('\n')
     if actual_remote != csr_remote_origin_url:
         raise RuntimeError(f'Expected remote origin url {csr_remote_origin_url} but found {actual_remote}. Reset your remote origin url to continue.')
 
     # Add, commit, and push changes to CSR
-    execute_process(f'touch {BASE_DIR}scripts/pipeline_spec/.gitkeep', to_null=False) # needed to keep dir here
     execute_process('git add .', to_null=False)
     execute_process('''git commit -m 'Run AutoMLOps' ''', to_null=False)
     execute_process(f'''git push origin {defaults['gcp']['cloud_source_repository_branch']} --force''', to_null=False)
     # pylint: disable=logging-fstring-interpolation
     logging.info(f'''Pushing code to {defaults['gcp']['cloud_source_repository_branch']} branch, triggering cloudbuild...''')
     logging.info(f'''Cloudbuild job running at: https://console.cloud.google.com/cloud-build/builds;region={defaults['gcp']['cb_trigger_location']}''')
```

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/__init__.py` & `google-cloud-automlops-1.1.4/AutoMLOps/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 import, with the end goal of becoming a Jupyter plugin to Vertex
 Workbench managed notebooks. The tool will generate yaml-component
 definitions, complete with Dockerfiles and requirements.txts for all
 Kubeflow components defined in a notebook. It will also generate a
 series of directories to support the creation of Vertex Pipelines.
 """
 # pylint: disable=invalid-name
-__version__ = '1.1.3'
+__version__ = '1.1.4'
 __author__ = 'Sean Rastatter'
 __credits__ = 'Google'
```

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/deployments/__init__.py` & `google-cloud-automlops-1.1.4/AutoMLOps/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/__init__.py` & `google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/builder.py` & `google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/builder.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/deployments/cloudbuild/constructs/scripts.py` & `google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/constructs/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,24 +86,24 @@
             f'# ==============================================================================\n'
             f'\n'
             f'''  # build the component_base image\n'''
             f'''  - name: "gcr.io/cloud-builders/docker"\n'''
             f'''    args: [ "build", "-t", "{self.__af_registry_location}-docker.pkg.dev/{self.__project_id}/{self.__af_registry_name}/components/component_base:latest", "." ]\n'''
             f'''    dir: "{self.__base_dir}components/component_base"\n'''
             f'''    id: "build_component_base"\n'''
-            f'''    waitFor: ["-"]\n'''
+            f'''    waitFor: ["-"]\n''')
+
+        cloudbuild_cloudrun_config = (
             f'\n'
             f'''  # build the run_pipeline image\n'''
             f'''  - name: 'gcr.io/cloud-builders/docker'\n'''
             f'''    args: [ "build", "-t", "{self.__af_registry_location}-docker.pkg.dev/{self.__project_id}/{self.__af_registry_name}/run_pipeline:latest", "-f", "cloud_run/run_pipeline/Dockerfile", "." ]\n'''
             f'''    dir: "{self.__base_dir}"\n'''
             f'''    id: "build_pipeline_runner_svc"\n'''
-            f'''    waitFor: ['build_component_base']\n''')
-
-        cloudbuild_cloudrun_config = (
+            f'''    waitFor: ['build_component_base']\n'''
             f'\n'
             f'# ==============================================================================\n'
             f'# PUSH & DEPLOY CUSTOM IMAGES\n'
             f'# ==============================================================================\n'
             f'\n'
             f'''  # push the component_base image\n'''
             f'''  - name: "gcr.io/cloud-builders/docker"\n'''
```

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/__init__.py` & `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/base.py` & `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # pylint: disable=C0103
 # pylint: disable=line-too-long
 
 from typing import Dict, List
 from AutoMLOps.utils.utils import read_yaml_file
 
 class Component():
-    """Parent class that defined a general abstraction of a Component."""
+    """Parent class that defines a general abstraction of a Component."""
     def __init__(self, component_spec: dict, defaults_file: str):
         """Instantiate Component scripts object with all necessary attributes.
 
         Args:
             component_spec (dict): Dictionary of component specs including details
                 of component image, startup command, and args.
             defaults_file (str): Path to the default config variables yaml.
@@ -35,15 +35,15 @@
         # Parse defaults file for hidden class attributes
         defaults = read_yaml_file(defaults_file)
         self._af_registry_location = defaults['gcp']['af_registry_location']
         self._project_id = defaults['gcp']['project_id']
         self._af_registry_name = defaults['gcp']['af_registry_name']
 
 class Pipeline():
-    """Parent class that defined a general abstraction of a Pipeline """
+    """Parent class that defines a general abstraction of a Pipeline """
     def __init__(self, custom_training_job_specs: List[Dict], defaults_file: str):
         """Instantiate Pipeline scripts object with all necessary attributes.
 
         Args:
             custom_training_job_specs (List[Dict]): Specifies the specs to run the training job with.
             defaults_file (str): Path to the default config variables yaml.
         """
```

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/__init__.py` & `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/builder.py` & `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,20 @@
 
     # Create components and pipelines
     components_path_list = get_components_list()
     for path in components_path_list:
         build_component(path)
     build_pipeline(custom_training_job_specs, pipeline_params)
 
+    # Write empty .gitkeep to pipeline_spec directory
+    write_file(f'{BASE_DIR}scripts/pipeline_spec/.gitkeep', '', 'w')
+
+    # Write empty .gitkeep to pipeline_spec directory
+    write_file(f'{BASE_DIR}README.md', kfp_scripts.readme, 'w')
+
     # Write dockerfile to the component base directory
     write_file(f'{GENERATED_COMPONENT_BASE}/Dockerfile', kfp_scripts.dockerfile, 'w')
 
     # Write requirements.txt to the component base directory
     write_file(f'{GENERATED_COMPONENT_BASE}/requirements.txt', kfp_scripts.requirements, 'w')
 
     # Build the cloud run files
```

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/__init__.py` & `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/cloudrun.py` & `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/cloudrun.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,23 +32,23 @@
 
         Args:
             defaults_file (str): Path to the default config variables yaml.
         """
 
         # Parse defaults file for hidden class attributes
         defaults = read_yaml_file(defaults_file)
-        self.__project_id = defaults['gcp']['project_id']
-        self.__pipeline_runner_service_account = defaults['gcp']['pipeline_runner_service_account']
-        self.__cloud_tasks_queue_location = defaults['gcp']['cloud_tasks_queue_location']
-        self.__cloud_tasks_queue_name = defaults['gcp']['cloud_tasks_queue_name']
-        self.__cloud_run_name = defaults['gcp']['cloud_run_name']
-        self.__cloud_run_location = defaults['gcp']['cloud_run_location']
-        self.__cloud_schedule_pattern = defaults['gcp']['cloud_schedule_pattern']
-        self.__cloud_schedule_location = defaults['gcp']['cloud_schedule_location']
-        self.__cloud_schedule_name = defaults['gcp']['cloud_schedule_name']
+        self._project_id = defaults['gcp']['project_id']
+        self._pipeline_runner_service_account = defaults['gcp']['pipeline_runner_service_account']
+        self._cloud_tasks_queue_location = defaults['gcp']['cloud_tasks_queue_location']
+        self._cloud_tasks_queue_name = defaults['gcp']['cloud_tasks_queue_name']
+        self._cloud_run_name = defaults['gcp']['cloud_run_name']
+        self._cloud_run_location = defaults['gcp']['cloud_run_location']
+        self._cloud_schedule_pattern = defaults['gcp']['cloud_schedule_pattern']
+        self._cloud_schedule_location = defaults['gcp']['cloud_schedule_location']
+        self._cloud_schedule_name = defaults['gcp']['cloud_schedule_name']
 
         # Set generated scripts as public attributes
         self.dockerfile = self._create_dockerfile()
         self.cloudrun_base_reqs = self._create_cloudrun_base_reqs()
         self.queueing_svc_reqs = self._create_queuing_svc_reqs()
         self.cloudrun_base = self._create_cloudrun_base()
         self.queueing_svc = self._create_queueing_svc()
@@ -228,24 +228,24 @@
             f'''import argparse\n'''
             f'''import json\n'''
             f'\n'
             f'''from google.cloud import run_v2\n'''
             f'''from google.cloud import scheduler_v1\n'''
             f'''from google.cloud import tasks_v2\n'''
             f'\n'
-            f'''CLOUD_RUN_LOCATION = '{self.__cloud_run_location}'\n'''
-            f'''CLOUD_RUN_NAME = '{self.__cloud_run_name}'\n'''
-            f'''CLOUD_TASKS_QUEUE_LOCATION = '{self.__cloud_tasks_queue_location}'\n'''
-            f'''CLOUD_TASKS_QUEUE_NAME = '{self.__cloud_tasks_queue_name}'\n'''
+            f'''CLOUD_RUN_LOCATION = '{self._cloud_run_location}'\n'''
+            f'''CLOUD_RUN_NAME = '{self._cloud_run_name}'\n'''
+            f'''CLOUD_TASKS_QUEUE_LOCATION = '{self._cloud_tasks_queue_location}'\n'''
+            f'''CLOUD_TASKS_QUEUE_NAME = '{self._cloud_tasks_queue_name}'\n'''
             f'''PARAMETER_VALUES_PATH = 'queueing_svc/pipeline_parameter_values.json'\n'''
-            f'''PIPELINE_RUNNER_SA = '{self.__pipeline_runner_service_account}'\n'''
-            f'''PROJECT_ID = '{self.__project_id}'\n'''
-            f'''SCHEDULE_LOCATION = '{self.__cloud_schedule_location}'\n'''
-            f'''SCHEDULE_PATTERN = '{self.__cloud_schedule_pattern}'\n'''
-            f'''SCHEDULE_NAME = '{self.__cloud_schedule_name}'\n'''
+            f'''PIPELINE_RUNNER_SA = '{self._pipeline_runner_service_account}'\n'''
+            f'''PROJECT_ID = '{self._project_id}'\n'''
+            f'''SCHEDULE_LOCATION = '{self._cloud_schedule_location}'\n'''
+            f'''SCHEDULE_PATTERN = '{self._cloud_schedule_pattern}'\n'''
+            f'''SCHEDULE_NAME = '{self._cloud_schedule_name}'\n'''
             f'\n'
             f'''def get_runner_svc_uri(\n'''
             f'''    cloud_run_location: str,\n'''
             f'''    cloud_run_name: str,\n'''
             f'''    project_id: str):\n'''
             f'''    """Fetches the uri for the given cloud run instance.\n'''
             f'\n'
```

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/component.py` & `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/component.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
     def _create_task(self):
         """Creates the content of the cell python code to be written to a file with required imports.
 
         Returns:
             str: Contents of component base source code.
         """
-        custom_code = self._component_spec['implementation']['container']['command'][-1]
         default_imports = (GENERATED_LICENSE +
             'import argparse\n'
             'import json\n'
             'from kfp.v2.components import executor\n')
         if not is_using_kfp_spec(self._component_spec['implementation']['container']['image']):
             custom_imports = ('\n'
             'import kfp\n'
             'from kfp.v2 import dsl\n'
             'from kfp.v2.dsl import *\n'
             'from typing import *\n'
             '\n')
         else:
             custom_imports = '' # the above is already included as part of the kfp spec
+        custom_code = self._component_spec['implementation']['container']['command'][-1]
         main_func = (
             '\n'
             '''def main():\n'''
             '''    """Main executor."""\n'''
             '''    parser = argparse.ArgumentParser()\n'''
             '''    parser.add_argument('--executor_input', type=str)\n'''
             '''    parser.add_argument('--function_to_execute', type=str)\n'''
```

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/pipeline.py` & `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,38 +32,52 @@
             defaults_file (str): Path to the default config variables yaml.
         """
         super().__init__(custom_training_job_specs, defaults_file)
         self.pipeline_imports = self._get_pipeline_imports()
         self.pipeline_argparse = self._get_pipeline_argparse()
         self.pipeline_runner = self._get_pipeline_runner()
 
+    def custom_specs_helper(self, custom_training_job_specs):
+        """Helper function that generates custom specs string.
+
+        Returns:
+            str: Custom specs pulled from custom_training_job_specs.
+        """
+        newline_tab = '\n    '
+        quote = '\''
+
+        if not custom_training_job_specs:
+            custom_specs = ''
+        else:
+            custom_specs = (
+                f'''    {newline_tab.join(f'{spec["component_spec"]}_custom_training_job_specs = {format_spec_dict(spec)}' for spec in custom_training_job_specs)}'''
+                f'\n'
+                f'''    {newline_tab.join(f'{spec["component_spec"]}_job_op = create_custom_training_job_op_from_component(**{spec["component_spec"]}_custom_training_job_specs)' for spec in custom_training_job_specs)}'''
+                f'\n'
+                f'''    {newline_tab.join(f'{spec["component_spec"]} = partial({spec["component_spec"]}_job_op, project={quote}{self._project_id}{quote})' for spec in custom_training_job_specs)}'''        
+                f'\n')
+        return custom_specs
+
+
     def _get_pipeline_imports(self):
         """Generates python code that imports modules and loads all custom components.
 
         Returns:
             str: Python pipeline_imports code.
         """
         components_list = get_components_list(full_path=False)
         gcpc_imports = (
             'from functools import partial\n'
             'from google_cloud_pipeline_components.v1.custom_job import create_custom_training_job_op_from_component\n')
         quote = '\''
         newline_tab = '\n    '
 
+
         # If there is a custom training job specified, write those to feed to pipeline imports
-        if not self._custom_training_job_specs:
-            custom_specs = ''
-        else:
-            custom_specs = (
-                f'''    {newline_tab.join(f'{spec["component_spec"]}_custom_training_job_specs = {format_spec_dict(spec)}' for spec in self._custom_training_job_specs)}'''
-                f'\n'
-                f'''    {newline_tab.join(f'{spec["component_spec"]}_job_op = create_custom_training_job_op_from_component(**{spec["component_spec"]}_custom_training_job_specs)' for spec in self._custom_training_job_specs)}'''
-                f'\n'
-                f'''    {newline_tab.join(f'{spec["component_spec"]} = partial({spec["component_spec"]}_job_op, project={quote}{self._project_id}{quote})' for spec in self._custom_training_job_specs)}'''        
-                f'\n')
+        custom_specs = self.custom_specs_helper(self._custom_training_job_specs)
 
         # Return standard code and customized specs
         return (
             f'''import argparse\n'''
             f'''import os\n'''
             f'''{gcpc_imports if self._custom_training_job_specs else ''}'''
             f'''import kfp\n'''
```

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/constructs/scripts.py` & `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/scripts.py`

 * *Files 12% similar despite different names*

```diff
@@ -82,59 +82,58 @@
             schedule_location: The location of the scheduler resource.
             schedule_name: The name of the scheduler resource.
             schedule_pattern: Cron formatted value used to create a Scheduled retrain job.
             base_dir: Top directory name.
             vpc_connector: The name of the vpc connector to use.
         """
         # Set passed variables as hidden attributes
-        self.__base_dir = base_dir
-        self.__run_local = run_local
-
-        # Parse defaults file for hidden class attributes
-        self.__af_registry_name = af_registry_name
-        self.__af_registry_location = af_registry_location
-        self.__project_id = project_id
-        self.__gs_bucket_name = gs_bucket_name
-        self.__gs_bucket_location = gs_bucket_location
-        self.__pipeline_region = gs_bucket_location
-        self.__pipeline_runner_service_account = pipeline_runner_sa
-        self.__cloud_source_repository = csr_name
-        self.__cloud_source_repository_branch = csr_branch_name
-        self.__cb_trigger_location = cb_trigger_location
-        self.__cb_trigger_name = cb_trigger_name
-        self.__cloud_tasks_queue_location = cloud_tasks_queue_location
-        self.__cloud_tasks_queue_name = cloud_tasks_queue_name
-        self.__vpc_connector = vpc_connector
-        self.__cloud_run_name = cloud_run_name
-        self.__cloud_run_location = cloud_run_location
-        self.__cloud_schedule_location = schedule_location
-        self.__cloud_schedule_name = schedule_name
-        self.__cloud_schedule_pattern = schedule_pattern
-        self.__base_image = base_image
+        self._base_dir = base_dir
+        self._run_local = run_local
+        self._af_registry_name = af_registry_name
+        self._af_registry_location = af_registry_location
+        self._project_id = project_id
+        self._gs_bucket_name = gs_bucket_name
+        self._gs_bucket_location = gs_bucket_location
+        self._pipeline_region = gs_bucket_location
+        self._pipeline_runner_service_account = pipeline_runner_sa
+        self._cloud_source_repository = csr_name
+        self._cloud_source_repository_branch = csr_branch_name
+        self._cb_trigger_location = cb_trigger_location
+        self._cb_trigger_name = cb_trigger_name
+        self._cloud_tasks_queue_location = cloud_tasks_queue_location
+        self._cloud_tasks_queue_name = cloud_tasks_queue_name
+        self._vpc_connector = vpc_connector
+        self._cloud_run_name = cloud_run_name
+        self._cloud_run_location = cloud_run_location
+        self._cloud_schedule_location = schedule_location
+        self._cloud_schedule_name = schedule_name
+        self._cloud_schedule_pattern = schedule_pattern
+        self._base_image = base_image
 
         # Set generated scripts as public attributes
         self.build_pipeline_spec = self._build_pipeline_spec()
         self.build_components = self._build_components()
         self.run_pipeline = self._run_pipeline()
         self.run_all = self._run_all()
         self.create_resources_script = self._create_resources_script()
         self.dockerfile = self._create_dockerfile()
         self.defaults = self._create_default_config()
         self.requirements = self._create_requirements()
+        self.readme = self._create_generated_readme()
 
     def _build_pipeline_spec(self):
         """Builds content of a shell script to build the pipeline specs.
 
         Returns:
             str: Text of script to build pipeline specs.
         """
         return (
             '#!/bin/bash\n' + GENERATED_LICENSE +
             '# Builds the pipeline specs\n'
-            f'# This script should run from the {self.__base_dir} directory\n'
+            f'# This script should run from the {self._base_dir} directory\n'
             '# Change directory in case this is not the script root.\n'
             '\n'
             'CONFIG_FILE=configs/defaults.yaml\n'
             '\n'
             'python3 -m pipelines.pipeline --config $CONFIG_FILE\n')
 
     def _build_components(self):
@@ -142,29 +141,29 @@
 
         Returns:
             str: Text of script to build components.
         """
         return (
             '#!/bin/bash\n' + GENERATED_LICENSE +
             '# Submits a Cloud Build job that builds and deploys the components\n'
-            f'# This script should run from the {self.__base_dir} directory\n'
+            f'# This script should run from the {self._base_dir} directory\n'
             '# Change directory in case this is not the script root.\n'
             '\n'
             'gcloud builds submit .. --config cloudbuild.yaml --timeout=3600\n')
 
     def _run_pipeline(self):
         """Builds content of a shell script to run the pipeline.
 
         Returns:
             str: Text of script to run pipeline.
         """
         return (
             '#!/bin/bash\n' + GENERATED_LICENSE +
             '# Submits the PipelineJob to Vertex AI\n'
-            f'# This script should run from the {self.__base_dir} directory\n'
+            f'# This script should run from the {self._base_dir} directory\n'
             '# Change directory in case this is not the script root.\n'
             '\n'
             'CONFIG_FILE=configs/defaults.yaml\n'
             '\n'
             'python3 -m pipelines.pipeline_runner --config $CONFIG_FILE\n')
 
     def _run_all(self):
@@ -172,15 +171,15 @@
 
         Returns:
             str: Text of script to run all other scripts.
         """
         return (
             '#!/bin/bash\n' + GENERATED_LICENSE +
             '# Builds components, pipeline specs, and submits the PipelineJob.\n'
-            f'# This script should run from the {self.__base_dir} directory\n'
+            f'# This script should run from the {self._base_dir} directory\n'
             '# Change directory in case this is not the script root.\n'
             '\n'
             '''GREEN='\033[0;32m'\n'''
             '''NC='\033[0m'\n'''
             '\n'
             'echo -e "${GREEN} BUILDING COMPONENTS ${NC}"\n'
             'gcloud builds submit .. --config cloudbuild.yaml --timeout=3600\n'
@@ -201,28 +200,28 @@
         """
         create_resources_script = (
             '#!/bin/bash\n' + GENERATED_LICENSE +
             f'# This script will create an artifact registry and gs bucket if they do not already exist.\n'
             f'\n'
             f'''GREEN='\033[0;32m'\n'''
             f'''NC='\033[0m'\n'''
-            f'''AF_REGISTRY_NAME={self.__af_registry_name}\n'''
-            f'''AF_REGISTRY_LOCATION={self.__af_registry_location}\n'''
-            f'''PROJECT_ID={self.__project_id}\n'''
-            f'''PROJECT_NUMBER=`gcloud projects describe {self.__project_id} --format 'value(projectNumber)'`\n'''
-            f'''BUCKET_NAME={self.__gs_bucket_name}\n'''
-            f'''BUCKET_LOCATION={self.__pipeline_region}\n'''
-            f'''SERVICE_ACCOUNT_NAME={self.__pipeline_runner_service_account.split('@')[0]}\n'''
-            f'''SERVICE_ACCOUNT_FULL={self.__pipeline_runner_service_account}\n'''
-            f'''CLOUD_SOURCE_REPO={self.__cloud_source_repository}\n'''
-            f'''CLOUD_SOURCE_REPO_BRANCH={self.__cloud_source_repository_branch}\n'''
-            f'''CB_TRIGGER_LOCATION={self.__cb_trigger_location}\n'''
-            f'''CB_TRIGGER_NAME={self.__cb_trigger_name}\n'''
-            f'''CLOUD_TASKS_QUEUE_LOCATION={self.__cloud_tasks_queue_location}\n'''
-            f'''CLOUD_TASKS_QUEUE_NAME={self.__cloud_tasks_queue_name}\n'''
+            f'''AF_REGISTRY_NAME={self._af_registry_name}\n'''
+            f'''AF_REGISTRY_LOCATION={self._af_registry_location}\n'''
+            f'''PROJECT_ID={self._project_id}\n'''
+            f'''PROJECT_NUMBER=`gcloud projects describe {self._project_id} --format 'value(projectNumber)'`\n'''
+            f'''BUCKET_NAME={self._gs_bucket_name}\n'''
+            f'''BUCKET_LOCATION={self._pipeline_region}\n'''
+            f'''SERVICE_ACCOUNT_NAME={self._pipeline_runner_service_account.split('@')[0]}\n'''
+            f'''SERVICE_ACCOUNT_FULL={self._pipeline_runner_service_account}\n'''
+            f'''CLOUD_SOURCE_REPO={self._cloud_source_repository}\n'''
+            f'''CLOUD_SOURCE_REPO_BRANCH={self._cloud_source_repository_branch}\n'''
+            f'''CB_TRIGGER_LOCATION={self._cb_trigger_location}\n'''
+            f'''CB_TRIGGER_NAME={self._cb_trigger_name}\n'''
+            f'''CLOUD_TASKS_QUEUE_LOCATION={self._cloud_tasks_queue_location}\n'''
+            f'''CLOUD_TASKS_QUEUE_NAME={self._cloud_tasks_queue_name}\n'''
             f'\n'
             f'echo -e "$GREEN Updating required API services in project $PROJECT_ID $NC"\n'
             f'gcloud services enable cloudresourcemanager.googleapis.com \{NEWLINE}'
             f'  aiplatform.googleapis.com \{NEWLINE}'
             f'  artifactregistry.googleapis.com \{NEWLINE}'
             f'  cloudbuild.googleapis.com \{NEWLINE}'
             f'  cloudscheduler.googleapis.com \{NEWLINE}'
@@ -341,15 +340,15 @@
             f'\n'
             f'else\n'
             f'\n'
             f'  echo "Cloud Source Repository: ${LEFT_BRACKET}CLOUD_SOURCE_REPO{RIGHT_BRACKET} already exists in project $PROJECT_ID"\n'
             f'\n'
             f'fi\n')
 
-        if not self.__run_local:
+        if not self._run_local:
             create_resources_script += (
                 f'\n'
                 f'# Create cloud tasks queue\n'
                 f'echo -e "$GREEN Checking for Cloud Tasks Queue: $CLOUD_TASKS_QUEUE_NAME in project $PROJECT_ID $NC"\n'
                 f'if ! (gcloud tasks queues list --location $CLOUD_TASKS_QUEUE_LOCATION | grep -E "(^|[[:blank:]])$CLOUD_TASKS_QUEUE_NAME($|[[:blank:]])"); then\n'
                 f'\n'
                 f'  echo "Creating Cloud Tasks Queue: ${LEFT_BRACKET}CLOUD_TASKS_QUEUE_NAME{RIGHT_BRACKET} in project $PROJECT_ID"\n'
@@ -368,15 +367,15 @@
                 f'\n'
                 f'  echo "Creating Cloudbuild Trigger on branch $CLOUD_SOURCE_REPO_BRANCH in project $PROJECT_ID for repo ${LEFT_BRACKET}CLOUD_SOURCE_REPO{RIGHT_BRACKET}"\n'
                 f'  gcloud beta builds triggers create cloud-source-repositories \{NEWLINE}'
                 f'  --region=$CB_TRIGGER_LOCATION \{NEWLINE}'
                 f'  --name=$CB_TRIGGER_NAME \{NEWLINE}'
                 f'  --repo=$CLOUD_SOURCE_REPO \{NEWLINE}'
                 f'  --branch-pattern="$CLOUD_SOURCE_REPO_BRANCH" \{NEWLINE}'
-                f'  --build-config={self.__base_dir}cloudbuild.yaml\n'
+                f'  --build-config={self._base_dir}cloudbuild.yaml\n'
                 f'\n'
                 f'else\n'
                 f'\n'
                 f'  echo "Cloudbuild Trigger already exists in project $PROJECT_ID for repo ${LEFT_BRACKET}CLOUD_SOURCE_REPO{RIGHT_BRACKET}"\n'
                 f'\n'
                 f'fi\n')
 
@@ -386,61 +385,61 @@
         """Creates the content of a Dockerfile to be written to the component_base directory.
 
         Returns:
             str: Text content of dockerfile.
         """
         return (
             GENERATED_LICENSE +
-            f'FROM {self.__base_image}\n'
+            f'FROM {self._base_image}\n'
             f'RUN python -m pip install --upgrade pip\n'
             f'COPY requirements.txt .\n'
             f'RUN python -m pip install -r \ \n'
             f'    requirements.txt --quiet --no-cache-dir \ \n'
             f'    && rm -f requirements.txt\n'
             f'COPY ./src /pipelines/component/src\n'
             f'ENTRYPOINT ["/bin/bash"]\n')
 
     def _create_default_config(self):
-        """Creates default defaults.yaml file contents. This defaults
+        """Creates defaults.yaml file contents. This defaults
         file is used by subsequent functions and by the pipeline
         files themselves.
 
         Returns:
             str: Defaults yaml file content
         """
         return (
             GENERATED_LICENSE +
             f'# These values are descriptive only - do not change.\n'
             f'# Rerun AutoMLOps.generate() to change these values.\n'
             f'gcp:\n'
-            f'  af_registry_location: {self.__af_registry_location}\n'
-            f'  af_registry_name: {self.__af_registry_name}\n'
-            f'  base_image: {self.__base_image}\n'
-            f'  cb_trigger_location: {self.__cb_trigger_location}\n'
-            f'  cb_trigger_name: {self.__cb_trigger_name}\n'
-            f'  cloud_run_location: {self.__cloud_run_location}\n'
-            f'  cloud_run_name: {self.__cloud_run_name}\n'
-            f'  cloud_tasks_queue_location: {self.__cloud_tasks_queue_location}\n'
-            f'  cloud_tasks_queue_name: {self.__cloud_tasks_queue_name}\n'
-            f'  cloud_schedule_location: {self.__cloud_schedule_location}\n'
-            f'  cloud_schedule_name: {self.__cloud_schedule_name}\n'
-            f'  cloud_schedule_pattern: {self.__cloud_schedule_pattern}\n'
-            f'  cloud_source_repository: {self.__cloud_source_repository}\n'
-            f'  cloud_source_repository_branch: {self.__cloud_source_repository_branch}\n'
-            f'  gs_bucket_name: {self.__gs_bucket_name}\n'
-            f'  pipeline_runner_service_account: {self.__pipeline_runner_service_account}\n'
-            f'  project_id: {self.__project_id}\n'
-            f'  vpc_connector: {self.__vpc_connector}\n'
+            f'  af_registry_location: {self._af_registry_location}\n'
+            f'  af_registry_name: {self._af_registry_name}\n'
+            f'  base_image: {self._base_image}\n'
+            f'  cb_trigger_location: {self._cb_trigger_location}\n'
+            f'  cb_trigger_name: {self._cb_trigger_name}\n'
+            f'  cloud_run_location: {self._cloud_run_location}\n'
+            f'  cloud_run_name: {self._cloud_run_name}\n'
+            f'  cloud_tasks_queue_location: {self._cloud_tasks_queue_location}\n'
+            f'  cloud_tasks_queue_name: {self._cloud_tasks_queue_name}\n'
+            f'  cloud_schedule_location: {self._cloud_schedule_location}\n'
+            f'  cloud_schedule_name: {self._cloud_schedule_name}\n'
+            f'  cloud_schedule_pattern: {self._cloud_schedule_pattern}\n'
+            f'  cloud_source_repository: {self._cloud_source_repository}\n'
+            f'  cloud_source_repository_branch: {self._cloud_source_repository_branch}\n'
+            f'  gs_bucket_name: {self._gs_bucket_name}\n'
+            f'  pipeline_runner_service_account: {self._pipeline_runner_service_account}\n'
+            f'  project_id: {self._project_id}\n'
+            f'  vpc_connector: {self._vpc_connector}\n'
             f'\n'
             f'pipelines:\n'
             f'  parameter_values_path: {GENERATED_PARAMETER_VALUES_PATH}\n'
             f'  pipeline_component_directory: components\n'
             f'  pipeline_job_spec_path: {GENERATED_PIPELINE_JOB_SPEC_PATH}\n'
-            f'  pipeline_region: {self.__gs_bucket_location}\n'
-            f'  pipeline_storage_path: gs://{self.__gs_bucket_name}/pipeline_root\n')
+            f'  pipeline_region: {self._gs_bucket_location}\n'
+            f'  pipeline_storage_path: gs://{self._gs_bucket_name}/pipeline_root\n')
 
     def _create_requirements(self):
         """Writes a requirements.txt to the component_base directory.
         Infers pip requirements from the python srcfiles using 
         pipreqs. Takes user-inputted requirements, and addes some 
         default gcp packages as well as packages that are often missing
         in setup.py files (e.g db_types, pyarrow, gcsfs, fsspec).
@@ -499,7 +498,59 @@
         # Pin kfp version
         if 'kfp' in set_of_requirements:
             set_of_requirements.remove('kfp')
         set_of_requirements.add(PINNED_KFP_VERSION)
         # Stringify and sort
         reqs_str = ''.join(r+'\n' for r in sorted(set_of_requirements))
         return reqs_str
+
+    def _create_generated_readme(self):
+        """Creates a readme markdown file to describe the contents of the
+        generated AutoMLOps code repo.
+
+        Returns:
+            str: readme.md file content
+        """
+        cloud_run_dirs = ''
+        if not self._run_local:
+            cloud_run_dirs = (
+                '├── cloud_run                                      : Cloud Runner service for submitting PipelineJobs.\n'
+                '    ├──run_pipeline                                : Contains main.py file, Dockerfile and requirements.txt\n'
+                '    ├──queueing_svc                                : Contains files for scheduling and queueing jobs to runner service\n'
+            )
+
+        return (
+            '# AutoMLOps - Generated Code Directory\n'
+            '\n'
+            '**Note: This directory contains code generated using AutoMLOps**\n'
+            '\n'
+            'AutoMLOps is a service that generates a production ready MLOps pipeline from Jupyter Notebooks, bridging the gap between Data Science and DevOps and accelerating the adoption and use of Vertex AI. The service generates an MLOps codebase for users to customize, and provides a way to build and manage a CI/CD integrated MLOps pipeline from the notebook. AutoMLOps automatically builds a source repo for versioning, cloudbuild configs and triggers, an artifact registry for storing custom components, gs buckets, service accounts and updated IAM privs for running pipelines, enables APIs (cloud Run, Cloud Build, Artifact Registry, etc.), creates a runner service API in Cloud Run for submitting PipelineJobs to Vertex AI, and a Cloud Scheduler job for submitting PipelineJobs on a recurring basis. These automatic integrations empower data scientists to take their experiments to production more quickly, allowing them to focus on what they do best: providing actionable insights through data.\n'
+            '\n'
+            '# User Guide\n'
+            '\n'
+            'For a user-guide, please view these [slides](https://github.com/GoogleCloudPlatform/automlops/blob/main/AutoMLOps_Implementation_Guide_External.pdf).\n'
+            '\n'
+            '# Layout\n'
+            '\n'
+            '```bash\n'
+            '.\n'
+            f'{cloud_run_dirs}'
+            '├── components                                     : Custom vertex pipeline components.\n'
+            '    ├──component_base                              : Contains all the python files, Dockerfile and requirements.txt\n'
+            '    ├──component_a                                 : Components generated using AutoMLOps\n'
+            '    ├──...\n'
+            '├── images                                         : Custom container images for training models.\n'
+            '├── pipelines                                      : Vertex ai pipeline definitions.\n'
+            '    ├── pipeline.py                                : Full pipeline definition.\n'
+            '    ├── pipeline_runner.py                         : Sends a PipelineJob to Vertex AI.\n'
+            '    ├── runtime_parameters                         : Variables to be used in a PipelineJob.\n'
+            '        ├── pipeline_parameter_values.json         : Json containing pipeline parameters.\n'  
+            '├── configs                                        : Configurations for defining vertex ai pipeline.\n'
+            '    ├── defaults.yaml                              : PipelineJob configuration variables.\n'
+            '├── scripts                                        : Scripts for manually triggering the cloud run service.\n'
+            '    ├── build_components.sh                        : Submits a Cloud Build job that builds and deploys the components.\n'
+            '    ├── build_pipeline_spec.sh                     : Builds the pipeline specs.\n'
+            '    ├── create_resources.sh                        : Creates an artifact registry and gs bucket if they do not already exist.\n'
+            '    ├── run_pipeline.sh                            : Submit the PipelineJob to Vertex AI.\n'
+            '    ├── run_all.sh                                 : Builds components, pipeline specs, and submits the PipelineJob.\n'
+            '└── cloudbuild.yaml                                : Cloudbuild configuration file for building custom components.\n'
+            '```\n')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/frameworks/kfp/scaffold.py` & `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/scaffold.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Builds temporary component scaffold yaml files."""
 
+# pylint: disable=anomalous-backslash-in-string
 # pylint: disable=C0103
 # pylint: disable=line-too-long
 
 import inspect
 from typing import Callable, List, Optional, TypeVar, Union
 
 import docstring_parser
@@ -37,17 +38,16 @@
 )
 
 T = TypeVar('T')
 
 def create_component_scaffold(func: Optional[Callable] = None,
                               *,
                               packages_to_install: Optional[List[str]] = None):
-    """Creates a tmp component scaffold which will be used by
-       the formalize function. Code is temporarily stored in
-       component_spec['implementation']['container']['command'].
+    """Creates a tmp component scaffold which will be used by the formalize function.
+    Code is temporarily stored in component_spec['implementation']['container']['command'].
 
     Args:
         func: The python function to create a component from. The function
             should have type annotations for all its arguments, indicating how
             it is intended to be used (e.g. as an input/output Artifact object,
             a plain parameter, or a path to a file).
         packages_to_install: A list of optional packages to install before
@@ -85,15 +85,14 @@
         func: The python function to create a component from. The function
             should have type annotations for all its arguments, indicating how
             it is intended to be used (e.g. as an input/output Artifact object,
             a plain parameter, or a path to a file).
         packages_to_install: A list of optional packages to install before
             executing func. These will always be installed at component runtime.
     """
-    # pylint: disable=anomalous-backslash-in-string
     newline = '\n'
     if not packages_to_install:
         packages_to_install = []
     concat_package_list = ' '.join([repr(str(package)) for package in packages_to_install])
     install_python_packages_script = (
         f'''if ! [ -x "$(command -v pip)" ]; then{newline}'''
         f'''    python3 -m ensurepip || python3 -m ensurepip --user || apt-get install python3-pip{newline}'''
@@ -155,15 +154,15 @@
         return annotation
 
 def create_pipeline_scaffold(func: Optional[Callable] = None,
                              *,
                              name: Optional[str] = None,
                              description: Optional[str] = None):
     """Creates a temporary pipeline scaffold which will
-       be used by the formalize function.
+    be used by the formalize function.
 
     Args:
         func: The python function to create a pipeline from. The function
             should have type annotations for all its arguments, indicating how
             it is intended to be used (e.g. as an input/output Artifact object,
             a plain parameter, or a path to a file).
         name: The name of the pipeline.
```

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/utils/__init__.py` & `google-cloud-automlops-1.1.4/AutoMLOps/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/utils/constants.py` & `google-cloud-automlops-1.1.4/AutoMLOps/utils/constants.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/AutoMLOps/utils/utils.py` & `google-cloud-automlops-1.1.4/AutoMLOps/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,16 +193,18 @@
                        check=True,
                        stdout=stdout,
                        stderr=subprocess.STDOUT)
     except subprocess.CalledProcessError as err:
         raise RuntimeError(f'Error executing process. {err}') from err
 
 def validate_schedule(schedule_pattern: str, run_local: str):
-    """Validates that the inputted schedule parameter.
-
+    """Validates that the inputted schedule parameter aligns with the run_local configuration.
+    Note: this function does not validate that schedule_pattern is a properly formatted cron value.
+    Cron format validation is done in the backend by GCP.
+    
     Args:
         schedule_pattern: Cron formatted value used to create a Scheduled retrain job.
         run_local: Flag that determines whether to use Cloud Run CI/CD.
     Raises:
         Exception: If schedule is not cron formatted or run_local validation fails.
     """
     if schedule_pattern != 'No Schedule Specified' and run_local:
@@ -225,27 +227,27 @@
         Exception: If an inputted type is not a primitive.
     """
     python_kfp_types_mapper = {
         int: 'Integer',
         str: 'String',
         float: 'Float',
         bool: 'Bool',
-        list: 'List',
-        dict: 'Dict'
+        list: 'JsonArray',
+        dict: 'JsonObject'
     }
     for param in params:
         try:
             param['type'] = python_kfp_types_mapper[param['type']]
         except KeyError as err:
             raise ValueError(f'Unsupported python type - we only support '
                              f'primitive types at this time. {err}') from err
     return params
 
 def get_function_source_definition(func: Callable) -> str:
-    """Returns a formatted list of parameters.
+    """Returns a formatted string of the source code.
 
     Args:
         func: The python function to create a component from. The function
             should have type annotations for all its arguments, indicating how
             it is intended to be used (e.g. as an input/output Artifact object,
             a plain parameter, or a path to a file).
     Returns:
```

### Comparing `google-cloud-automlops-1.1.3/LICENSE` & `google-cloud-automlops-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/PKG-INFO` & `google-cloud-automlops-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.1.3
+Version: 1.1.4
 Summary: AutoMLOps is a service that generates a production-style         MLOps pipeline from Jupyter Notebooks.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -50,15 +50,15 @@
 
 Or Install locally by cloning the repo and running `pip install .`
 
 # Dependencies
 - `docopt==0.6.2`,
 - `docstring-parser==0.15`,
 - `pipreqs==0.4.11`,
-- `PyYAML==5.4.1`,
+- `PyYAML==6.0.1`,
 - `yarg==0.1.9`
 
 # GCP Services
 AutoMLOps makes use of the following products by default:
 - [Vertex AI Pipelines](https://cloud.google.com/vertex-ai/docs/pipelines/introduction)
 - [Artifact Registry](https://cloud.google.com/artifact-registry/docs/overview)
 - [Google Cloud Storage](https://cloud.google.com/storage/docs/introduction)
@@ -99,14 +99,28 @@
 - roles/cloudtasks.enqueuer
 - roles/cloudscheduler.admin
 
 # User Guide
 
 For a user-guide, please view these [slides](./AutoMLOps_Implementation_Guide_External.pdf).
 
+# List of Examples
+
+Training
+- [00_introduction_training_example](./examples/training/00_introduction_training_example.ipynb)
+- [00_introduction_training_example_no_notebook](./examples/training/00_introduction_training_example_no_notebook.py)
+- [01_clustering_example](./examples/training/01_clustering_example.ipynb)
+- [02_tensorflow_transfer_learning_gpu_example](./examples/training/02_tensorflow_transfer_learning_gpu_example.ipynb)
+- [03_bqml_introduction_training_example](./examples/training/03_bqml_introduction_training_example.ipynb)
+- [04_bqml_forecasting-retail-demand](./examples/training/04_bqml_forecasting-retail-demand.ipynb)
+
+Inferencing
+- [00_batch_prediction_example](./examples/inferencing/00_batch_prediction_example.ipynb)
+- [01_customer_churn_model_monitoring_example](./examples/inferencing/01_customer_churn_model_monitoring_example.ipynb)
+
 # Options
 
 AutoMLOps CI/CD options:
 1. `run_local`: Bool that specifies whether to use generate files resources locally or use cloud CI/CD workflow (see below). Defaults to True. See [CI/CD Workflow](#cloud-continuous-integration-and-continuous-deployment-workflow)
 
 Required parameters:
 1. `project_id: str`
@@ -233,18 +247,16 @@
 - [Model Registry](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/model_registry)
 - [Experiments](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/experiments)
 - [ExplainableAI](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/explainable_ai)
 - [Vertex AI Pipelines](https://cloud.google.com/vertex-ai/docs/pipelines/notebooks)
 - [Google Cloud Pipeline Components](https://github.com/GoogleCloudPlatform/vertex-ai-samples/blob/main/notebooks/official/pipelines/custom_model_training_and_batch_prediction.ipynb)
 
 # Next Steps / Backlog
-- Refine unit tests
 - Use [terraform](https://github.com/GoogleCloudPlatform/vertex-pipelines-end-to-end-samples/tree/main/terraform) for the creation of resources.
 - Allow multiple AutoMLOps pipelines within the same directory
-- Adding model monitoring part
 - Alternatives to Pipreqs
 
 # Contributors
 
 [Sean Rastatter](mailto:srastatter@google.com): Tech Lead
 
 [Tony DiLoreto](mailto:tonydiloreto@google.com): Project Manager
```

### Comparing `google-cloud-automlops-1.1.3/README.md` & `google-cloud-automlops-1.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 Or Install locally by cloning the repo and running `pip install .`
 
 # Dependencies
 - `docopt==0.6.2`,
 - `docstring-parser==0.15`,
 - `pipreqs==0.4.11`,
-- `PyYAML==5.4.1`,
+- `PyYAML==6.0.1`,
 - `yarg==0.1.9`
 
 # GCP Services
 AutoMLOps makes use of the following products by default:
 - [Vertex AI Pipelines](https://cloud.google.com/vertex-ai/docs/pipelines/introduction)
 - [Artifact Registry](https://cloud.google.com/artifact-registry/docs/overview)
 - [Google Cloud Storage](https://cloud.google.com/storage/docs/introduction)
@@ -78,14 +78,28 @@
 - roles/cloudtasks.enqueuer
 - roles/cloudscheduler.admin
 
 # User Guide
 
 For a user-guide, please view these [slides](./AutoMLOps_Implementation_Guide_External.pdf).
 
+# List of Examples
+
+Training
+- [00_introduction_training_example](./examples/training/00_introduction_training_example.ipynb)
+- [00_introduction_training_example_no_notebook](./examples/training/00_introduction_training_example_no_notebook.py)
+- [01_clustering_example](./examples/training/01_clustering_example.ipynb)
+- [02_tensorflow_transfer_learning_gpu_example](./examples/training/02_tensorflow_transfer_learning_gpu_example.ipynb)
+- [03_bqml_introduction_training_example](./examples/training/03_bqml_introduction_training_example.ipynb)
+- [04_bqml_forecasting-retail-demand](./examples/training/04_bqml_forecasting-retail-demand.ipynb)
+
+Inferencing
+- [00_batch_prediction_example](./examples/inferencing/00_batch_prediction_example.ipynb)
+- [01_customer_churn_model_monitoring_example](./examples/inferencing/01_customer_churn_model_monitoring_example.ipynb)
+
 # Options
 
 AutoMLOps CI/CD options:
 1. `run_local`: Bool that specifies whether to use generate files resources locally or use cloud CI/CD workflow (see below). Defaults to True. See [CI/CD Workflow](#cloud-continuous-integration-and-continuous-deployment-workflow)
 
 Required parameters:
 1. `project_id: str`
@@ -212,18 +226,16 @@
 - [Model Registry](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/model_registry)
 - [Experiments](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/experiments)
 - [ExplainableAI](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/explainable_ai)
 - [Vertex AI Pipelines](https://cloud.google.com/vertex-ai/docs/pipelines/notebooks)
 - [Google Cloud Pipeline Components](https://github.com/GoogleCloudPlatform/vertex-ai-samples/blob/main/notebooks/official/pipelines/custom_model_training_and_batch_prediction.ipynb)
 
 # Next Steps / Backlog
-- Refine unit tests
 - Use [terraform](https://github.com/GoogleCloudPlatform/vertex-pipelines-end-to-end-samples/tree/main/terraform) for the creation of resources.
 - Allow multiple AutoMLOps pipelines within the same directory
-- Adding model monitoring part
 - Alternatives to Pipreqs
 
 # Contributors
 
 [Sean Rastatter](mailto:srastatter@google.com): Tech Lead
 
 [Tony DiLoreto](mailto:tonydiloreto@google.com): Project Manager
```

### Comparing `google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/PKG-INFO` & `google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.1.3
+Version: 1.1.4
 Summary: AutoMLOps is a service that generates a production-style         MLOps pipeline from Jupyter Notebooks.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -50,15 +50,15 @@
 
 Or Install locally by cloning the repo and running `pip install .`
 
 # Dependencies
 - `docopt==0.6.2`,
 - `docstring-parser==0.15`,
 - `pipreqs==0.4.11`,
-- `PyYAML==5.4.1`,
+- `PyYAML==6.0.1`,
 - `yarg==0.1.9`
 
 # GCP Services
 AutoMLOps makes use of the following products by default:
 - [Vertex AI Pipelines](https://cloud.google.com/vertex-ai/docs/pipelines/introduction)
 - [Artifact Registry](https://cloud.google.com/artifact-registry/docs/overview)
 - [Google Cloud Storage](https://cloud.google.com/storage/docs/introduction)
@@ -99,14 +99,28 @@
 - roles/cloudtasks.enqueuer
 - roles/cloudscheduler.admin
 
 # User Guide
 
 For a user-guide, please view these [slides](./AutoMLOps_Implementation_Guide_External.pdf).
 
+# List of Examples
+
+Training
+- [00_introduction_training_example](./examples/training/00_introduction_training_example.ipynb)
+- [00_introduction_training_example_no_notebook](./examples/training/00_introduction_training_example_no_notebook.py)
+- [01_clustering_example](./examples/training/01_clustering_example.ipynb)
+- [02_tensorflow_transfer_learning_gpu_example](./examples/training/02_tensorflow_transfer_learning_gpu_example.ipynb)
+- [03_bqml_introduction_training_example](./examples/training/03_bqml_introduction_training_example.ipynb)
+- [04_bqml_forecasting-retail-demand](./examples/training/04_bqml_forecasting-retail-demand.ipynb)
+
+Inferencing
+- [00_batch_prediction_example](./examples/inferencing/00_batch_prediction_example.ipynb)
+- [01_customer_churn_model_monitoring_example](./examples/inferencing/01_customer_churn_model_monitoring_example.ipynb)
+
 # Options
 
 AutoMLOps CI/CD options:
 1. `run_local`: Bool that specifies whether to use generate files resources locally or use cloud CI/CD workflow (see below). Defaults to True. See [CI/CD Workflow](#cloud-continuous-integration-and-continuous-deployment-workflow)
 
 Required parameters:
 1. `project_id: str`
@@ -233,18 +247,16 @@
 - [Model Registry](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/model_registry)
 - [Experiments](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/experiments)
 - [ExplainableAI](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/explainable_ai)
 - [Vertex AI Pipelines](https://cloud.google.com/vertex-ai/docs/pipelines/notebooks)
 - [Google Cloud Pipeline Components](https://github.com/GoogleCloudPlatform/vertex-ai-samples/blob/main/notebooks/official/pipelines/custom_model_training_and_batch_prediction.ipynb)
 
 # Next Steps / Backlog
-- Refine unit tests
 - Use [terraform](https://github.com/GoogleCloudPlatform/vertex-pipelines-end-to-end-samples/tree/main/terraform) for the creation of resources.
 - Allow multiple AutoMLOps pipelines within the same directory
-- Adding model monitoring part
 - Alternatives to Pipreqs
 
 # Contributors
 
 [Sean Rastatter](mailto:srastatter@google.com): Tech Lead
 
 [Tony DiLoreto](mailto:tonydiloreto@google.com): Project Manager
```

### Comparing `google-cloud-automlops-1.1.3/google_cloud_automlops.egg-info/SOURCES.txt` & `google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -23,14 +23,21 @@
 AutoMLOps/utils/utils.py
 google_cloud_automlops.egg-info/PKG-INFO
 google_cloud_automlops.egg-info/SOURCES.txt
 google_cloud_automlops.egg-info/dependency_links.txt
 google_cloud_automlops.egg-info/requires.txt
 google_cloud_automlops.egg-info/top_level.txt
 tests/__init__.py
-tests/unit/AutoMLOps_test.py
 tests/unit/__init__.py
 tests/unit/deployments/__init__.py
 tests/unit/frameworks/__init__.py
+tests/unit/frameworks/base_test.py
 tests/unit/frameworks/kfp/__init__.py
+tests/unit/frameworks/kfp/builder_test.py
+tests/unit/frameworks/kfp/scaffold_test.py
+tests/unit/frameworks/kfp/constructs/__init__.py
+tests/unit/frameworks/kfp/constructs/cloudrun_test.py
+tests/unit/frameworks/kfp/constructs/component_test.py
+tests/unit/frameworks/kfp/constructs/pipeline_test.py
+tests/unit/frameworks/kfp/constructs/scripts_test.py
 tests/unit/utils/__init__.py
 tests/unit/utils/utils_test.py
```

### Comparing `google-cloud-automlops-1.1.3/setup.py` & `google-cloud-automlops-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as file:
     readme_contents = file.read()
 
 setup(
     name='google-cloud-automlops',
-    version='1.1.3',
+    version='1.1.4',
     description='AutoMLOps is a service that generates a production-style \
         MLOps pipeline from Jupyter Notebooks.',
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     url='https://github.com/GoogleCloudPlatform/automlops',
     author='Sean Rastatter',
     author_email='srastatter@google.com',
```

### Comparing `google-cloud-automlops-1.1.3/tests/__init__.py` & `google-cloud-automlops-1.1.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/tests/unit/__init__.py` & `google-cloud-automlops-1.1.4/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/tests/unit/deployments/__init__.py` & `google-cloud-automlops-1.1.4/tests/unit/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/tests/unit/frameworks/__init__.py` & `google-cloud-automlops-1.1.4/tests/unit/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/tests/unit/frameworks/kfp/__init__.py` & `google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.3/tests/unit/utils/__init__.py` & `google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/__init__.py`

 * *Files identical despite different names*

