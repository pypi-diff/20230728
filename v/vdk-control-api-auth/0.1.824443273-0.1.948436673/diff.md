# Comparing `tmp/vdk-control-api-auth-0.1.824443273.tar.gz` & `tmp/vdk-control-api-auth-0.1.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-control-api-auth-0.1.824443273.tar", last modified: Fri Mar 31 14:25:02 2023, max compression
+gzip compressed data, was "vdk-control-api-auth-0.1.948436673.tar", last modified: Fri Jul 28 09:42:33 2023, max compression
```

## Comparing `vdk-control-api-auth-0.1.824443273.tar` & `vdk-control-api-auth-0.1.948436673.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:02.163044 vdk-control-api-auth-0.1.824443273/
--rw-r--r--   0 root         (0) root         (0)     1729 2023-03-31 14:25:02.163044 vdk-control-api-auth-0.1.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1122 2023-03-31 14:24:50.000000 vdk-control-api-auth-0.1.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:25:02.163044 vdk-control-api-auth-0.1.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1519 2023-03-31 14:24:54.000000 vdk-control-api-auth-0.1.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:02.159044 vdk-control-api-auth-0.1.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:02.159044 vdk-control-api-auth-0.1.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:02.159044 vdk-control-api-auth-0.1.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:02.159044 vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/
--rw-rw-rw-   0 root         (0) root         (0)     6416 2023-03-31 14:24:50.000000 vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/auth_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2040 2023-03-31 14:24:50.000000 vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/auth_exception.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2023-03-31 14:24:50.000000 vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/auth_request_values.py
--rw-rw-rw-   0 root         (0) root         (0)     5714 2023-03-31 14:24:50.000000 vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)    15320 2023-03-31 14:24:50.000000 vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/autorization_code_auth.py
--rw-rw-rw-   0 root         (0) root         (0)    10772 2023-03-31 14:24:50.000000 vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/base_auth.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-03-31 14:24:50.000000 vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/login_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:02.159044 vdk-control-api-auth-0.1.824443273/src/vdk_control_api_auth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1729 2023-03-31 14:25:02.000000 vdk-control-api-auth-0.1.824443273/src/vdk_control_api_auth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      700 2023-03-31 14:25:02.000000 vdk-control-api-auth-0.1.824443273/src/vdk_control_api_auth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:25:02.000000 vdk-control-api-auth-0.1.824443273/src/vdk_control_api_auth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-03-31 14:25:02.000000 vdk-control-api-auth-0.1.824443273/src/vdk_control_api_auth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:25:02.000000 vdk-control-api-auth-0.1.824443273/src/vdk_control_api_auth.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:02.163044 vdk-control-api-auth-0.1.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-03-31 14:24:50.000000 vdk-control-api-auth-0.1.824443273/tests/test_api_token_auth.py
--rw-rw-rw-   0 root         (0) root         (0)     3499 2023-03-31 14:24:50.000000 vdk-control-api-auth-0.1.824443273/tests/test_authorization_code_auth.py
--rw-rw-rw-   0 root         (0) root         (0)     8443 2023-03-31 14:24:50.000000 vdk-control-api-auth-0.1.824443273/tests/test_core_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:33.414756 vdk-control-api-auth-0.1.948436673/
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-07-28 09:42:33.414756 vdk-control-api-auth-0.1.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2023-07-28 09:42:10.000000 vdk-control-api-auth-0.1.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:42:33.414756 vdk-control-api-auth-0.1.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2023-07-28 09:42:20.000000 vdk-control-api-auth-0.1.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:33.410756 vdk-control-api-auth-0.1.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:33.410756 vdk-control-api-auth-0.1.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:33.410756 vdk-control-api-auth-0.1.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:33.414756 vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/
+-rw-rw-rw-   0 root         (0) root         (0)     6416 2023-07-28 09:42:10.000000 vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/auth_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2023-07-28 09:42:10.000000 vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/auth_exception.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2023-07-28 09:42:10.000000 vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/auth_request_values.py
+-rw-rw-rw-   0 root         (0) root         (0)     5714 2023-07-28 09:42:10.000000 vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)    15320 2023-07-28 09:42:10.000000 vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/autorization_code_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    10772 2023-07-28 09:42:10.000000 vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/base_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-28 09:42:10.000000 vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/login_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:33.414756 vdk-control-api-auth-0.1.948436673/src/vdk_control_api_auth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-07-28 09:42:33.000000 vdk-control-api-auth-0.1.948436673/src/vdk_control_api_auth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      700 2023-07-28 09:42:33.000000 vdk-control-api-auth-0.1.948436673/src/vdk_control_api_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:33.000000 vdk-control-api-auth-0.1.948436673/src/vdk_control_api_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-28 09:42:33.000000 vdk-control-api-auth-0.1.948436673/src/vdk_control_api_auth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:42:33.000000 vdk-control-api-auth-0.1.948436673/src/vdk_control_api_auth.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:33.414756 vdk-control-api-auth-0.1.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-28 09:42:10.000000 vdk-control-api-auth-0.1.948436673/tests/test_api_token_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     3499 2023-07-28 09:42:10.000000 vdk-control-api-auth-0.1.948436673/tests/test_authorization_code_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     8443 2023-07-28 09:42:10.000000 vdk-control-api-auth-0.1.948436673/tests/test_core_auth.py
```

### Comparing `vdk-control-api-auth-0.1.824443273/PKG-INFO` & `vdk-control-api-auth-0.1.948436673/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-api-auth
-Version: 0.1.824443273
+Version: 0.1.948436673
 Summary: Versatile Data Kit plugin library provides support for authentication.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-control-api-auth-0.1.824443273/README.md` & `vdk-control-api-auth-0.1.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-api-auth-0.1.824443273/setup.py` & `vdk-control-api-auth-0.1.948436673/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 "plugin-template" is the name of the plugin contained within this package. Note that you can include
 more than one plugin in a single package. Also note that the contained plugin may have the same name as the package.
 
 "plugin_template" is the Python file which contains the plugin hooks for the corresponding plugin.
 """
 
-__version__ = "0.1.824443273"
+__version__ = "0.1.948436673"
 
 setuptools.setup(
     name="vdk-control-api-auth",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit plugin library provides support for "
     "authentication.",
```

### Comparing `vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/auth_config.py` & `vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/auth_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/auth_exception.py` & `vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/auth_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/auth_request_values.py` & `vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/auth_request_values.py`

 * *Files identical despite different names*

### Comparing `vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/authentication.py` & `vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/autorization_code_auth.py` & `vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/autorization_code_auth.py`

 * *Files identical despite different names*

### Comparing `vdk-control-api-auth-0.1.824443273/src/vdk/plugin/control_api_auth/base_auth.py` & `vdk-control-api-auth-0.1.948436673/src/vdk/plugin/control_api_auth/base_auth.py`

 * *Files identical despite different names*

### Comparing `vdk-control-api-auth-0.1.824443273/src/vdk_control_api_auth.egg-info/PKG-INFO` & `vdk-control-api-auth-0.1.948436673/src/vdk_control_api_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-api-auth
-Version: 0.1.824443273
+Version: 0.1.948436673
 Summary: Versatile Data Kit plugin library provides support for authentication.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-control-api-auth-0.1.824443273/src/vdk_control_api_auth.egg-info/SOURCES.txt` & `vdk-control-api-auth-0.1.948436673/src/vdk_control_api_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-control-api-auth-0.1.824443273/tests/test_api_token_auth.py` & `vdk-control-api-auth-0.1.948436673/tests/test_api_token_auth.py`

 * *Files identical despite different names*

### Comparing `vdk-control-api-auth-0.1.824443273/tests/test_authorization_code_auth.py` & `vdk-control-api-auth-0.1.948436673/tests/test_authorization_code_auth.py`

 * *Files identical despite different names*

### Comparing `vdk-control-api-auth-0.1.824443273/tests/test_core_auth.py` & `vdk-control-api-auth-0.1.948436673/tests/test_core_auth.py`

 * *Files identical despite different names*

