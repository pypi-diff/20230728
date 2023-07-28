# Comparing `tmp/iitkgp_erp_login-2.1.3.tar.gz` & `tmp/iitkgp_erp_login-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iitkgp_erp_login-2.1.3.tar", last modified: Sun Jul 23 10:28:40 2023, max compression
+gzip compressed data, was "iitkgp_erp_login-2.2.0.tar", last modified: Fri Jul 28 21:27:58 2023, max compression
```

## Comparing `iitkgp_erp_login-2.1.3.tar` & `iitkgp_erp_login-2.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:28:40.508271 iitkgp_erp_login-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-23 10:27:54.000000 iitkgp_erp_login-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-07-23 10:28:40.508271 iitkgp_erp_login-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17104 2023-07-23 10:27:54.000000 iitkgp_erp_login-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-23 10:28:21.000000 iitkgp_erp_login-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 10:28:40.508271 iitkgp_erp_login-2.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:28:40.504271 iitkgp_erp_login-2.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:28:40.508271 iitkgp_erp_login-2.1.3/src/iitkgp_erp_login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 10:27:54.000000 iitkgp_erp_login-2.1.3/src/iitkgp_erp_login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-23 10:27:54.000000 iitkgp_erp_login-2.1.3/src/iitkgp_erp_login/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-23 10:27:54.000000 iitkgp_erp_login-2.1.3/src/iitkgp_erp_login/erp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-23 10:27:54.000000 iitkgp_erp_login-2.1.3/src/iitkgp_erp_login/read_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-23 10:27:54.000000 iitkgp_erp_login-2.1.3/src/iitkgp_erp_login/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:28:40.508271 iitkgp_erp_login-2.1.3/src/iitkgp_erp_login.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-07-23 10:28:40.000000 iitkgp_erp_login-2.1.3/src/iitkgp_erp_login.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-23 10:28:40.000000 iitkgp_erp_login-2.1.3/src/iitkgp_erp_login.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 10:28:40.000000 iitkgp_erp_login-2.1.3/src/iitkgp_erp_login.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-23 10:28:40.000000 iitkgp_erp_login-2.1.3/src/iitkgp_erp_login.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-23 10:28:40.000000 iitkgp_erp_login-2.1.3/src/iitkgp_erp_login.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:27:58.009597 iitkgp_erp_login-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-28 21:27:13.000000 iitkgp_erp_login-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17889 2023-07-28 21:27:58.009597 iitkgp_erp_login-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17331 2023-07-28 21:27:13.000000 iitkgp_erp_login-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-28 21:27:40.000000 iitkgp_erp_login-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 21:27:58.009597 iitkgp_erp_login-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:27:58.005597 iitkgp_erp_login-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:27:58.005597 iitkgp_erp_login-2.2.0/src/iitkgp_erp_login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:27:13.000000 iitkgp_erp_login-2.2.0/src/iitkgp_erp_login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-28 21:27:13.000000 iitkgp_erp_login-2.2.0/src/iitkgp_erp_login/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-28 21:27:13.000000 iitkgp_erp_login-2.2.0/src/iitkgp_erp_login/erp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-28 21:27:13.000000 iitkgp_erp_login-2.2.0/src/iitkgp_erp_login/read_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-28 21:27:13.000000 iitkgp_erp_login-2.2.0/src/iitkgp_erp_login/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:27:58.005597 iitkgp_erp_login-2.2.0/src/iitkgp_erp_login.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17889 2023-07-28 21:27:57.000000 iitkgp_erp_login-2.2.0/src/iitkgp_erp_login.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-28 21:27:58.000000 iitkgp_erp_login-2.2.0/src/iitkgp_erp_login.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:27:57.000000 iitkgp_erp_login-2.2.0/src/iitkgp_erp_login.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 21:27:58.000000 iitkgp_erp_login-2.2.0/src/iitkgp_erp_login.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 21:27:58.000000 iitkgp_erp_login-2.2.0/src/iitkgp_erp_login.egg-info/top_level.txt
```

### Comparing `iitkgp_erp_login-2.1.3/LICENSE` & `iitkgp_erp_login-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.1.3/PKG-INFO` & `iitkgp_erp_login-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iitkgp_erp_login
-Version: 2.1.3
+Version: 2.2.0
 Summary: A package to automate login process in ERP for IIT-KGP
 Author-email: Arpit Bhardwaj <proffapt@pm.me>
 Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,18 @@
 
 - Seamless Credentials & OTP Handling
 - Effortless Session & ssoToken Management
 - Smart Token Storage for Efficiency
 
 > **Note** This package is not officially affiliated with IIT Kharagpur.
 
+https://github.com/proffapt/iitkgp-erp-login-pypi/assets/86282911/c0401f6a-80af-46ae-8a8f-ac735f0e67b5
+> Guess the number of lines of python code it will take you to achieve this.
+>> Reading this doc will give you the answer.
+
 <details>
   <summary>Table of Contents</summary>
 
 - <a href="#endpoints">Endpoints</a>
 	- <a href="#endpoints-about">About</a>
 	- <a href="#endpoints-usage">Usage</a>
 - <a href="#login">Login</a>
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 2.1.3 Summary: A package
+Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 2.2.0 Summary: A package
 to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
 pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # ERP Login Module Tired of the tedious ERP login process? Wanted to
 automate some ERP workflow but stuck at login?
 ð Introducing **iitkgp-erp-login**: Your Ultimate ERP Login Automation
 Module for _IIT-KGP_ ! ð Key Features: - Seamless Credentials & OTP Handling
 - Effortless Session & ssoToken Management - Smart Token Storage for Efficiency
-> **Note** This package is not officially affiliated with IIT Kharagpur.  Table
-of Contents - Endpoints - About - Usage - Login - Input - Output - Usage -
-Session_status_check - Input - Output - Usage - SSOToken_status_check - Input -
-Output - Usage - Get_tokens_from_file - Example
+> **Note** This package is not officially affiliated with IIT Kharagpur. https:
+//github.com/proffapt/iitkgp-erp-login-pypi/assets/86282911/c0401f6a-80af-46ae-
+8a8f-ac735f0e67b5 > Guess the number of lines of python code it will take you
+to achieve this. >> Reading this doc will give you the answer.  Table of
+Contents - Endpoints - About - Usage - Login - Input - Output - Usage - Session
+status_check - Input - Output - Usage - SSOToken_status_check - Input - Output
+- Usage - Get_tokens_from_file - Example
 ## Endpoints The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-
 pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the
 necessary endpoints for the ERP login workflow.
 ### About - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage. -
 `SECRET_QUESTION_URL`: The URL for retrieving the secret question for
 authentication. - `OTP_URL`: The URL for requesting the OTP (One-Time Password)
 for authentication. - `LOGIN_URL`: The URL for ERP login. - `WELCOMEPAGE_URL`:
```

### Comparing `iitkgp_erp_login-2.1.3/README.md` & `iitkgp_erp_login-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 - Seamless Credentials & OTP Handling
 - Effortless Session & ssoToken Management
 - Smart Token Storage for Efficiency
 
 > **Note** This package is not officially affiliated with IIT Kharagpur.
 
+https://github.com/proffapt/iitkgp-erp-login-pypi/assets/86282911/c0401f6a-80af-46ae-8a8f-ac735f0e67b5
+> Guess the number of lines of python code it will take you to achieve this.
+>> Reading this doc will give you the answer.
+
 <details>
   <summary>Table of Contents</summary>
 
 - <a href="#endpoints">Endpoints</a>
 	- <a href="#endpoints-about">About</a>
 	- <a href="#endpoints-usage">Usage</a>
 - <a href="#login">Login</a>
```

#### html2text {}

```diff
@@ -1,16 +1,19 @@
 # ERP Login Module Tired of the tedious ERP login process? Wanted to automate
 some ERP workflow but stuck at login?
 ð Introducing **iitkgp-erp-login**: Your Ultimate ERP Login Automation
 Module for _IIT-KGP_ ! ð Key Features: - Seamless Credentials & OTP Handling
 - Effortless Session & ssoToken Management - Smart Token Storage for Efficiency
-> **Note** This package is not officially affiliated with IIT Kharagpur.  Table
-of Contents - Endpoints - About - Usage - Login - Input - Output - Usage -
-Session_status_check - Input - Output - Usage - SSOToken_status_check - Input -
-Output - Usage - Get_tokens_from_file - Example
+> **Note** This package is not officially affiliated with IIT Kharagpur. https:
+//github.com/proffapt/iitkgp-erp-login-pypi/assets/86282911/c0401f6a-80af-46ae-
+8a8f-ac735f0e67b5 > Guess the number of lines of python code it will take you
+to achieve this. >> Reading this doc will give you the answer.  Table of
+Contents - Endpoints - About - Usage - Login - Input - Output - Usage - Session
+status_check - Input - Output - Usage - SSOToken_status_check - Input - Output
+- Usage - Get_tokens_from_file - Example
 ## Endpoints The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-
 pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the
 necessary endpoints for the ERP login workflow.
 ### About - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage. -
 `SECRET_QUESTION_URL`: The URL for retrieving the secret question for
 authentication. - `OTP_URL`: The URL for requesting the OTP (One-Time Password)
 for authentication. - `LOGIN_URL`: The URL for ERP login. - `WELCOMEPAGE_URL`:
```

### Comparing `iitkgp_erp_login-2.1.3/pyproject.toml` & `iitkgp_erp_login-2.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iitkgp_erp_login"
-version = "2.1.3"
+version = "2.2.0"
 authors = [
   { name="Arpit Bhardwaj", email="proffapt@pm.me" },
 ]
 description = "A package to automate login process in ERP for IIT-KGP"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+  "bs4",
+  "ping3",
+  "requests",
   "google-auth",
   "google-auth-oauthlib",
   "google-auth-httplib2",
   "google-api-python-client",
-  "requests",
-  "bs4",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/proffapt/iitkgp-erp-login-pypi"
 "Bug Tracker" = "https://github.com/proffapt/iitkgp-erp-login-pypi/issues"
```

### Comparing `iitkgp_erp_login-2.1.3/src/iitkgp_erp_login/erp.py` & `iitkgp_erp_login-2.2.0/src/iitkgp_erp_login/erp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import re
 import sys
+import ping3
 import inspect
 import logging
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 from bs4 import BeautifulSoup as bs
 from iitkgp_erp_login.read_mail import getOTP
 from iitkgp_erp_login.endpoints import *
@@ -64,29 +65,28 @@
                 secret_answer = ERPCREDS.SECURITY_QUESTIONS_ANSWERS[secret_question]
             else:
                 print ("Your secret question: " + secret_question)
                 secret_answer = getpass.getpass("Enter the answer to the secret question: ")
         except (requests.exceptions.RequestException, KeyError) as e:
             raise ErpLoginError(f"Failed to fetch Security Question: {str(e)}")
 
-        try:
-            r = session.post(OTP_URL, data={'typeee': 'SI', 'loginid': ROLL_NUMBER, 'pass': PASSWORD}, headers=headers)
-        except requests.exceptions.RequestException as e:
-            raise ErpLoginError(f"Failed to request OTP: {str(e)}")
-        
         login_details = {
             'user_id': ROLL_NUMBER,
             'password': PASSWORD,
             'answer': secret_answer,
             'sessionToken': sessionToken,
             'requestedUrl': HOMEPAGE_URL,
         }
 
-        if r.status_code == 200:
-            logging.info(" Requested OTP") if LOGGING else None
+        if not ping3.ping("iitkgp.ac.in"):
+            try:
+                r = session.post(OTP_URL, data={'typeee': 'SI', 'loginid': ROLL_NUMBER, 'pass': PASSWORD}, headers=headers)
+                logging.info(" Requested OTP") if LOGGING else None
+            except requests.exceptions.RequestException as e:
+                raise ErpLoginError(f"Failed to request OTP: {str(e)}")
             
             if OTP_CHECK_INTERVAL != None:
                     try:
                         logging.info(" Waiting for OTP...") if LOGGING else None
                         otp = getOTP(OTP_CHECK_INTERVAL)
                         logging.info(" Received OTP") if LOGGING else None
                     except Exception as e:
```

### Comparing `iitkgp_erp_login-2.1.3/src/iitkgp_erp_login/read_mail.py` & `iitkgp_erp_login-2.2.0/src/iitkgp_erp_login/read_mail.py`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.1.3/src/iitkgp_erp_login/utils.py` & `iitkgp_erp_login-2.2.0/src/iitkgp_erp_login/utils.py`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.1.3/src/iitkgp_erp_login.egg-info/PKG-INFO` & `iitkgp_erp_login-2.2.0/src/iitkgp_erp_login.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iitkgp-erp-login
-Version: 2.1.3
+Version: 2.2.0
 Summary: A package to automate login process in ERP for IIT-KGP
 Author-email: Arpit Bhardwaj <proffapt@pm.me>
 Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,18 @@
 
 - Seamless Credentials & OTP Handling
 - Effortless Session & ssoToken Management
 - Smart Token Storage for Efficiency
 
 > **Note** This package is not officially affiliated with IIT Kharagpur.
 
+https://github.com/proffapt/iitkgp-erp-login-pypi/assets/86282911/c0401f6a-80af-46ae-8a8f-ac735f0e67b5
+> Guess the number of lines of python code it will take you to achieve this.
+>> Reading this doc will give you the answer.
+
 <details>
   <summary>Table of Contents</summary>
 
 - <a href="#endpoints">Endpoints</a>
 	- <a href="#endpoints-about">About</a>
 	- <a href="#endpoints-usage">Usage</a>
 - <a href="#login">Login</a>
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1 Name: iitkgp-erp-login Version: 2.1.3 Summary: A package
+Metadata-Version: 2.1 Name: iitkgp-erp-login Version: 2.2.0 Summary: A package
 to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
 pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # ERP Login Module Tired of the tedious ERP login process? Wanted to
 automate some ERP workflow but stuck at login?
 ð Introducing **iitkgp-erp-login**: Your Ultimate ERP Login Automation
 Module for _IIT-KGP_ ! ð Key Features: - Seamless Credentials & OTP Handling
 - Effortless Session & ssoToken Management - Smart Token Storage for Efficiency
-> **Note** This package is not officially affiliated with IIT Kharagpur.  Table
-of Contents - Endpoints - About - Usage - Login - Input - Output - Usage -
-Session_status_check - Input - Output - Usage - SSOToken_status_check - Input -
-Output - Usage - Get_tokens_from_file - Example
+> **Note** This package is not officially affiliated with IIT Kharagpur. https:
+//github.com/proffapt/iitkgp-erp-login-pypi/assets/86282911/c0401f6a-80af-46ae-
+8a8f-ac735f0e67b5 > Guess the number of lines of python code it will take you
+to achieve this. >> Reading this doc will give you the answer.  Table of
+Contents - Endpoints - About - Usage - Login - Input - Output - Usage - Session
+status_check - Input - Output - Usage - SSOToken_status_check - Input - Output
+- Usage - Get_tokens_from_file - Example
 ## Endpoints The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-
 pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the
 necessary endpoints for the ERP login workflow.
 ### About - `HOMEPAGE_URL`: The URL of the ERP homepage/loginpage. -
 `SECRET_QUESTION_URL`: The URL for retrieving the secret question for
 authentication. - `OTP_URL`: The URL for requesting the OTP (One-Time Password)
 for authentication. - `LOGIN_URL`: The URL for ERP login. - `WELCOMEPAGE_URL`:
```

