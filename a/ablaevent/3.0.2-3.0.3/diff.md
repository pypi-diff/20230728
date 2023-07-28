# Comparing `tmp/ablaevent-3.0.2.tar.gz` & `tmp/ablaevent-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ablaevent-3.0.2.tar", last modified: Thu Jul 20 08:54:25 2023, max compression
+gzip compressed data, was "ablaevent-3.0.3.tar", last modified: Fri Jul 28 20:44:02 2023, max compression
```

## Comparing `ablaevent-3.0.2.tar` & `ablaevent-3.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 emna      (1000) emna      (1000)        0 2023-07-20 08:54:24.996512 ablaevent-3.0.2/
--rw-rw-r--   0 emna      (1000) emna      (1000)       18 2023-07-20 08:27:06.000000 ablaevent-3.0.2/MANIFEST.in
--rw-rw-r--   0 emna      (1000) emna      (1000)     1287 2023-07-20 08:54:24.996512 ablaevent-3.0.2/PKG-INFO
--rw-rw-r--   0 emna      (1000) emna      (1000)     2209 2023-07-20 08:39:22.000000 ablaevent-3.0.2/README.md
-drwxrwxr-x   0 emna      (1000) emna      (1000)        0 2023-07-20 08:54:24.992512 ablaevent-3.0.2/ablaevent.egg-info/
--rw-rw-r--   0 emna      (1000) emna      (1000)     1287 2023-07-20 08:54:24.000000 ablaevent-3.0.2/ablaevent.egg-info/PKG-INFO
--rw-rw-r--   0 emna      (1000) emna      (1000)      667 2023-07-20 08:54:24.000000 ablaevent-3.0.2/ablaevent.egg-info/SOURCES.txt
--rw-rw-r--   0 emna      (1000) emna      (1000)        1 2023-07-20 08:54:24.000000 ablaevent-3.0.2/ablaevent.egg-info/dependency_links.txt
--rw-rw-r--   0 emna      (1000) emna      (1000)      225 2023-07-20 08:54:24.000000 ablaevent-3.0.2/ablaevent.egg-info/requires.txt
--rw-rw-r--   0 emna      (1000) emna      (1000)        8 2023-07-20 08:54:24.000000 ablaevent-3.0.2/ablaevent.egg-info/top_level.txt
-drwxrwxr-x   0 emna      (1000) emna      (1000)        0 2023-07-20 08:54:24.996512 ablaevent-3.0.2/posthog/
--rw-rw-r--   0 emna      (1000) emna      (1000)    13656 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/__init__.py
--rw-rw-r--   0 emna      (1000) emna      (1000)    26631 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/client.py
--rw-rw-r--   0 emna      (1000) emna      (1000)     4306 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/consumer.py
--rw-rw-r--   0 emna      (1000) emna      (1000)    10569 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/feature_flags.py
--rw-rw-r--   0 emna      (1000) emna      (1000)      595 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/poller.py
--rw-rw-r--   0 emna      (1000) emna      (1000)     3536 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/request.py
-drwxrwxr-x   0 emna      (1000) emna      (1000)        0 2023-07-20 08:54:24.996512 ablaevent-3.0.2/posthog/sentry/
--rw-rw-r--   0 emna      (1000) emna      (1000)       39 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/sentry/__init__.py
--rw-rw-r--   0 emna      (1000) emna      (1000)      771 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/sentry/django.py
--rw-rw-r--   0 emna      (1000) emna      (1000)     2234 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/sentry/posthog_integration.py
-drwxrwxr-x   0 emna      (1000) emna      (1000)        0 2023-07-20 08:54:24.996512 ablaevent-3.0.2/posthog/test/
--rw-rw-r--   0 emna      (1000) emna      (1000)      299 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/test/__init__.py
--rw-rw-r--   0 emna      (1000) emna      (1000)    26990 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/test/test_client.py
--rw-rw-r--   0 emna      (1000) emna      (1000)     6325 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/test/test_consumer.py
--rw-rw-r--   0 emna      (1000) emna      (1000)   127297 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/test/test_feature_flags.py
--rw-rw-r--   0 emna      (1000) emna      (1000)     1099 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/test/test_module.py
--rw-rw-r--   0 emna      (1000) emna      (1000)     1702 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/test/test_request.py
--rw-rw-r--   0 emna      (1000) emna      (1000)     3188 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/test/test_utils.py
--rw-rw-r--   0 emna      (1000) emna      (1000)     3136 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/utils.py
--rw-rw-r--   0 emna      (1000) emna      (1000)       87 2023-07-20 08:27:06.000000 ablaevent-3.0.2/posthog/version.py
--rw-rw-r--   0 emna      (1000) emna      (1000)      193 2023-07-20 08:27:06.000000 ablaevent-3.0.2/pyproject.toml
--rw-rw-r--   0 emna      (1000) emna      (1000)       67 2023-07-20 08:54:25.000512 ablaevent-3.0.2/setup.cfg
--rw-rw-r--   0 emna      (1000) emna      (1000)     2140 2023-07-20 08:54:19.000000 ablaevent-3.0.2/setup.py
+drwxrwxr-x   0 emna      (1000) emna      (1000)        0 2023-07-28 20:44:02.852121 ablaevent-3.0.3/
+-rw-rw-r--   0 emna      (1000) emna      (1000)       18 2023-07-28 19:42:06.000000 ablaevent-3.0.3/MANIFEST.in
+-rw-rw-r--   0 emna      (1000) emna      (1000)     1297 2023-07-28 20:44:02.852121 ablaevent-3.0.3/PKG-INFO
+-rw-rw-r--   0 emna      (1000) emna      (1000)       20 2023-07-28 20:19:26.000000 ablaevent-3.0.3/README.md
+drwxrwxr-x   0 emna      (1000) emna      (1000)        0 2023-07-28 20:44:02.848122 ablaevent-3.0.3/ablaevent.egg-info/
+-rw-rw-r--   0 emna      (1000) emna      (1000)     1297 2023-07-28 20:44:02.000000 ablaevent-3.0.3/ablaevent.egg-info/PKG-INFO
+-rw-rw-r--   0 emna      (1000) emna      (1000)      667 2023-07-28 20:44:02.000000 ablaevent-3.0.3/ablaevent.egg-info/SOURCES.txt
+-rw-rw-r--   0 emna      (1000) emna      (1000)        1 2023-07-28 20:44:02.000000 ablaevent-3.0.3/ablaevent.egg-info/dependency_links.txt
+-rw-rw-r--   0 emna      (1000) emna      (1000)      225 2023-07-28 20:44:02.000000 ablaevent-3.0.3/ablaevent.egg-info/requires.txt
+-rw-rw-r--   0 emna      (1000) emna      (1000)        8 2023-07-28 20:44:02.000000 ablaevent-3.0.3/ablaevent.egg-info/top_level.txt
+drwxrwxr-x   0 emna      (1000) emna      (1000)        0 2023-07-28 20:44:02.852121 ablaevent-3.0.3/posthog/
+-rw-rw-r--   0 emna      (1000) emna      (1000)    13656 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/__init__.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)    26631 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/client.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)     4306 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/consumer.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)    10569 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/feature_flags.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)      595 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/poller.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)     3536 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/request.py
+drwxrwxr-x   0 emna      (1000) emna      (1000)        0 2023-07-28 20:44:02.852121 ablaevent-3.0.3/posthog/sentry/
+-rw-rw-r--   0 emna      (1000) emna      (1000)       39 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/sentry/__init__.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)      771 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/sentry/django.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)     2234 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/sentry/posthog_integration.py
+drwxrwxr-x   0 emna      (1000) emna      (1000)        0 2023-07-28 20:44:02.852121 ablaevent-3.0.3/posthog/test/
+-rw-rw-r--   0 emna      (1000) emna      (1000)      299 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/test/__init__.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)    26990 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/test/test_client.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)     6325 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/test/test_consumer.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)   127297 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/test/test_feature_flags.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)     1099 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/test/test_module.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)     1702 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/test/test_request.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)     3188 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/test/test_utils.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)     3136 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/utils.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)       87 2023-07-28 19:42:06.000000 ablaevent-3.0.3/posthog/version.py
+-rw-rw-r--   0 emna      (1000) emna      (1000)      193 2023-07-28 19:42:06.000000 ablaevent-3.0.3/pyproject.toml
+-rw-rw-r--   0 emna      (1000) emna      (1000)       67 2023-07-28 20:44:02.852121 ablaevent-3.0.3/setup.cfg
+-rw-rw-r--   0 emna      (1000) emna      (1000)     2150 2023-07-28 20:43:04.000000 ablaevent-3.0.3/setup.py
```

### Comparing `ablaevent-3.0.2/PKG-INFO` & `ablaevent-3.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ablaevent
-Version: 3.0.2
-Summary: Integrate PostHog into any python application.
-Home-page: https://github.com/posthog/posthog-python
+Version: 3.0.3
+Summary: Integrate Ablaevent into any python application.
+Home-page: https://github.com/AblaAnalytics/ablaevent-python
 Author: Posthog
 Author-email: hey@posthog.com
 Maintainer: PostHog
 Maintainer-email: hey@posthog.com
 License: MIT License
 Description: 
         Ablaevent is developer-friendly, self-hosted product analytics. ablaevent-python is the python package.
@@ -25,9 +25,9 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: dev
-Provides-Extra: test
 Provides-Extra: sentry
+Provides-Extra: test
```

### Comparing `ablaevent-3.0.2/ablaevent.egg-info/PKG-INFO` & `ablaevent-3.0.3/ablaevent.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ablaevent
-Version: 3.0.2
-Summary: Integrate PostHog into any python application.
-Home-page: https://github.com/posthog/posthog-python
+Version: 3.0.3
+Summary: Integrate Ablaevent into any python application.
+Home-page: https://github.com/AblaAnalytics/ablaevent-python
 Author: Posthog
 Author-email: hey@posthog.com
 Maintainer: PostHog
 Maintainer-email: hey@posthog.com
 License: MIT License
 Description: 
         Ablaevent is developer-friendly, self-hosted product analytics. ablaevent-python is the python package.
@@ -25,9 +25,9 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: dev
-Provides-Extra: test
 Provides-Extra: sentry
+Provides-Extra: test
```

### Comparing `ablaevent-3.0.2/ablaevent.egg-info/SOURCES.txt` & `ablaevent-3.0.3/ablaevent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/__init__.py` & `ablaevent-3.0.3/posthog/__init__.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/client.py` & `ablaevent-3.0.3/posthog/client.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/consumer.py` & `ablaevent-3.0.3/posthog/consumer.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/feature_flags.py` & `ablaevent-3.0.3/posthog/feature_flags.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/poller.py` & `ablaevent-3.0.3/posthog/poller.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/request.py` & `ablaevent-3.0.3/posthog/request.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/sentry/django.py` & `ablaevent-3.0.3/posthog/sentry/django.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/sentry/posthog_integration.py` & `ablaevent-3.0.3/posthog/sentry/posthog_integration.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/test/test_client.py` & `ablaevent-3.0.3/posthog/test/test_client.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/test/test_consumer.py` & `ablaevent-3.0.3/posthog/test/test_consumer.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/test/test_feature_flags.py` & `ablaevent-3.0.3/posthog/test/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/test/test_module.py` & `ablaevent-3.0.3/posthog/test/test_module.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/test/test_request.py` & `ablaevent-3.0.3/posthog/test/test_request.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/test/test_utils.py` & `ablaevent-3.0.3/posthog/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/posthog/utils.py` & `ablaevent-3.0.3/posthog/utils.py`

 * *Files identical despite different names*

### Comparing `ablaevent-3.0.2/setup.py` & `ablaevent-3.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,26 +26,26 @@
     ],
     "test": ["mock>=2.0.0", "freezegun==0.3.15", "pylint", "flake8", "coverage", "pytest"],
     "sentry": ["sentry-sdk", "django"],
 }
 
 setup(
     name="ablaevent",
-    version='3.0.2',
-    url="https://github.com/posthog/posthog-python",
+    version="3.0.3",
+    url="https://github.com/AblaAnalytics/ablaevent-python",
     author="Posthog",
     author_email="hey@posthog.com",
     maintainer="PostHog",
     maintainer_email="hey@posthog.com",
     test_suite="posthog.test.all",
     packages=["posthog", "posthog.test", "posthog.sentry"],
     license="MIT License",
     install_requires=install_requires,
     extras_require=extras_require,
-    description="Integrate PostHog into any python application.",
+    description="Integrate Ablaevent into any python application.",
     long_description=long_description,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

