# Comparing `tmp/pixelpay-sdk-2.1.1.tar.gz` & `tmp/pixelpay-sdk-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelpay-sdk-2.1.1.tar", last modified: Thu Jul 27 22:10:34 2023, max compression
+gzip compressed data, was "pixelpay-sdk-2.1.2.tar", last modified: Fri Jul 28 15:13:43 2023, max compression
```

## Comparing `pixelpay-sdk-2.1.1.tar` & `pixelpay-sdk-2.1.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.518496 pixelpay-sdk-2.1.1/
--rw-r--r--   0 javiercano   (501) staff       (20)     1088 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/LICENSE.md
--rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-07-27 22:10:34.518328 pixelpay-sdk-2.1.1/PKG-INFO
--rw-r--r--   0 javiercano   (501) staff       (20)      455 2023-06-07 22:52:21.000000 pixelpay-sdk-2.1.1/README.md
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.503161 pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/
--rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-07-27 22:10:34.000000 pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/PKG-INFO
--rw-r--r--   0 javiercano   (501) staff       (20)     2079 2023-07-27 22:10:34.000000 pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 javiercano   (501) staff       (20)        1 2023-07-27 22:10:34.000000 pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 javiercano   (501) staff       (20)       31 2023-07-27 22:10:34.000000 pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/requires.txt
--rw-r--r--   0 javiercano   (501) staff       (20)        9 2023-07-27 22:10:34.000000 pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/top_level.txt
--rw-r--r--   0 javiercano   (501) staff       (20)       85 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/pyproject.toml
--rw-r--r--   0 javiercano   (501) staff       (20)       38 2023-07-27 22:10:34.518546 pixelpay-sdk-2.1.1/setup.cfg
--rw-r--r--   0 javiercano   (501) staff       (20)     1398 2023-07-19 22:28:45.000000 pixelpay-sdk-2.1.1/setup.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.493820 pixelpay-sdk-2.1.1/src/
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.503446 pixelpay-sdk-2.1.1/src/pixelpay/
--rw-r--r--   0 javiercano   (501) staff       (20)      365 2023-07-27 20:13:44.000000 pixelpay-sdk-2.1.1/src/pixelpay/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.504872 pixelpay-sdk-2.1.1/src/pixelpay/assets/
--rw-r--r--   0 javiercano   (501) staff       (20)     5438 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/assets/countries.json
--rw-r--r--   0 javiercano   (501) staff       (20)    18333 2023-01-26 21:25:46.000000 pixelpay-sdk-2.1.1/src/pixelpay/assets/formats.json
--rw-r--r--   0 javiercano   (501) staff       (20)    88971 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/assets/states.json
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.506995 pixelpay-sdk-2.1.1/src/pixelpay/base/
--rw-r--r--   0 javiercano   (501) staff       (20)     3185 2023-07-19 22:25:29.000000 pixelpay-sdk-2.1.1/src/pixelpay/base/Helpers.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1994 2023-07-27 20:23:07.000000 pixelpay-sdk-2.1.1/src/pixelpay/base/RequestBehaviour.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1804 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/base/Response.py
--rw-r--r--   0 javiercano   (501) staff       (20)    10062 2023-07-27 22:06:41.000000 pixelpay-sdk-2.1.1/src/pixelpay/base/ServiceBehaviour.py
--rw-r--r--   0 javiercano   (501) staff       (20)      248 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/base/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.507742 pixelpay-sdk-2.1.1/src/pixelpay/entities/
--rw-r--r--   0 javiercano   (501) staff       (20)     1812 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/entities/CardResult.py
--rw-r--r--   0 javiercano   (501) staff       (20)     3028 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/entities/TransactionResult.py
--rw-r--r--   0 javiercano   (501) staff       (20)      142 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/entities/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.508917 pixelpay-sdk-2.1.1/src/pixelpay/exceptions/
--rw-r--r--   0 javiercano   (501) staff       (20)       53 2023-07-27 21:35:29.000000 pixelpay-sdk-2.1.1/src/pixelpay/exceptions/FailedEncryptionException.py
--rw-r--r--   0 javiercano   (501) staff       (20)       55 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/exceptions/InvalidCredentialsException.py
--rw-r--r--   0 javiercano   (501) staff       (20)       59 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/exceptions/InvalidTransactionTypeException.py
--rw-r--r--   0 javiercano   (501) staff       (20)      333 2023-07-27 21:35:45.000000 pixelpay-sdk-2.1.1/src/pixelpay/exceptions/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.510661 pixelpay-sdk-2.1.1/src/pixelpay/models/
--rw-r--r--   0 javiercano   (501) staff       (20)      512 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/models/Billing.py
--rw-r--r--   0 javiercano   (501) staff       (20)      656 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/models/Card.py
--rw-r--r--   0 javiercano   (501) staff       (20)      653 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/models/Item.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1873 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/models/Order.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1914 2023-07-27 22:07:03.000000 pixelpay-sdk-2.1.1/src/pixelpay/models/Settings.py
--rw-r--r--   0 javiercano   (501) staff       (20)      214 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/models/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.513227 pixelpay-sdk-2.1.1/src/pixelpay/requests/
--rw-r--r--   0 javiercano   (501) staff       (20)      105 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/AuthTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      358 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/CaptureTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)     3925 2023-07-27 20:49:27.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/CardTokenization.py
--rw-r--r--   0 javiercano   (501) staff       (20)     5947 2023-07-27 22:06:29.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/PaymentTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1020 2023-06-07 22:41:02.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/SaleTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      198 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/StatusTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      372 2023-06-07 22:21:17.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/VoidTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      518 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.514332 pixelpay-sdk-2.1.1/src/pixelpay/resources/
--rw-r--r--   0 javiercano   (501) staff       (20)      123 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/resources/Environment.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1657 2023-01-26 21:27:02.000000 pixelpay-sdk-2.1.1/src/pixelpay/resources/Locations.py
--rw-r--r--   0 javiercano   (501) staff       (20)      121 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/resources/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.517348 pixelpay-sdk-2.1.1/src/pixelpay/responses/
--rw-r--r--   0 javiercano   (501) staff       (20)       70 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/ErrorResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/FailureResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       75 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/InputErrorResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/NetworkFailureResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/NoAccessResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/NotFoundResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/PayloadResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       80 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/PaymentDeclinedResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/PreconditionalResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/SuccessResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/TimeoutResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)      838 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.518077 pixelpay-sdk-2.1.1/src/pixelpay/services/
--rw-r--r--   0 javiercano   (501) staff       (20)     2081 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/services/Tokenization.py
--rw-r--r--   0 javiercano   (501) staff       (20)     2471 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/services/Transaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      130 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/services/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.937703 pixelpay-sdk-2.1.2/
+-rw-r--r--   0 javiercano   (501) staff       (20)     1088 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/LICENSE.md
+-rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-07-28 15:13:43.937517 pixelpay-sdk-2.1.2/PKG-INFO
+-rw-r--r--   0 javiercano   (501) staff       (20)      455 2023-06-07 22:52:21.000000 pixelpay-sdk-2.1.2/README.md
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.914011 pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/
+-rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-07-28 15:13:43.000000 pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 javiercano   (501) staff       (20)     2079 2023-07-28 15:13:43.000000 pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)        1 2023-07-28 15:13:43.000000 pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)       31 2023-07-28 15:13:43.000000 pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/requires.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)        9 2023-07-28 15:13:43.000000 pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/top_level.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)       85 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/pyproject.toml
+-rw-r--r--   0 javiercano   (501) staff       (20)       38 2023-07-28 15:13:43.937744 pixelpay-sdk-2.1.2/setup.cfg
+-rw-r--r--   0 javiercano   (501) staff       (20)     1398 2023-07-19 22:28:45.000000 pixelpay-sdk-2.1.2/setup.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.903339 pixelpay-sdk-2.1.2/src/
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.914238 pixelpay-sdk-2.1.2/src/pixelpay/
+-rw-r--r--   0 javiercano   (501) staff       (20)      365 2023-07-28 04:05:12.000000 pixelpay-sdk-2.1.2/src/pixelpay/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.917620 pixelpay-sdk-2.1.2/src/pixelpay/assets/
+-rw-r--r--   0 javiercano   (501) staff       (20)     5438 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/assets/countries.json
+-rw-r--r--   0 javiercano   (501) staff       (20)    18333 2023-01-26 21:25:46.000000 pixelpay-sdk-2.1.2/src/pixelpay/assets/formats.json
+-rw-r--r--   0 javiercano   (501) staff       (20)    88971 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/assets/states.json
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.920404 pixelpay-sdk-2.1.2/src/pixelpay/base/
+-rw-r--r--   0 javiercano   (501) staff       (20)     3185 2023-07-19 22:25:29.000000 pixelpay-sdk-2.1.2/src/pixelpay/base/Helpers.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1995 2023-07-28 03:39:52.000000 pixelpay-sdk-2.1.2/src/pixelpay/base/RequestBehaviour.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1804 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/base/Response.py
+-rw-r--r--   0 javiercano   (501) staff       (20)    10006 2023-07-28 03:40:04.000000 pixelpay-sdk-2.1.2/src/pixelpay/base/ServiceBehaviour.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      248 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/base/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.921649 pixelpay-sdk-2.1.2/src/pixelpay/entities/
+-rw-r--r--   0 javiercano   (501) staff       (20)     1812 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/entities/CardResult.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     3028 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/entities/TransactionResult.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      142 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/entities/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.923328 pixelpay-sdk-2.1.2/src/pixelpay/exceptions/
+-rw-r--r--   0 javiercano   (501) staff       (20)       53 2023-07-27 21:35:29.000000 pixelpay-sdk-2.1.2/src/pixelpay/exceptions/FailedEncryptionException.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       55 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/exceptions/InvalidCredentialsException.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       59 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/exceptions/InvalidTransactionTypeException.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      333 2023-07-27 21:35:45.000000 pixelpay-sdk-2.1.2/src/pixelpay/exceptions/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.926040 pixelpay-sdk-2.1.2/src/pixelpay/models/
+-rw-r--r--   0 javiercano   (501) staff       (20)      512 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/models/Billing.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      656 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/models/Card.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      653 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/models/Item.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1873 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/models/Order.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1914 2023-07-27 22:07:03.000000 pixelpay-sdk-2.1.2/src/pixelpay/models/Settings.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      214 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/models/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.931716 pixelpay-sdk-2.1.2/src/pixelpay/requests/
+-rw-r--r--   0 javiercano   (501) staff       (20)      105 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/AuthTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      358 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/CaptureTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     3890 2023-07-28 03:40:47.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/CardTokenization.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     5951 2023-07-28 03:40:39.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/PaymentTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1020 2023-06-07 22:41:02.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/SaleTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      198 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/StatusTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      372 2023-06-07 22:21:17.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/VoidTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      518 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/requests/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.932612 pixelpay-sdk-2.1.2/src/pixelpay/resources/
+-rw-r--r--   0 javiercano   (501) staff       (20)      123 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/resources/Environment.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1657 2023-01-26 21:27:02.000000 pixelpay-sdk-2.1.2/src/pixelpay/resources/Locations.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      121 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/resources/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.936478 pixelpay-sdk-2.1.2/src/pixelpay/responses/
+-rw-r--r--   0 javiercano   (501) staff       (20)       70 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/ErrorResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/FailureResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       75 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/InputErrorResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/NetworkFailureResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/NoAccessResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/NotFoundResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/PayloadResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       80 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/PaymentDeclinedResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/PreconditionalResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/SuccessResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/TimeoutResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      838 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/responses/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-28 15:13:43.937240 pixelpay-sdk-2.1.2/src/pixelpay/services/
+-rw-r--r--   0 javiercano   (501) staff       (20)     2081 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/services/Tokenization.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     2471 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/services/Transaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      130 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.2/src/pixelpay/services/__init__.py
```

### Comparing `pixelpay-sdk-2.1.1/LICENSE.md` & `pixelpay-sdk-2.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/PKG-INFO` & `pixelpay-sdk-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelpay-sdk
-Version: 2.1.1
+Version: 2.1.2
 Summary: PixelPay SDK toolkit.
 Author: Javier Cano
 Author-email: javier@pixel.hn
 License: MIT
 Keywords: pixelpay pixel pay sdk
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/PKG-INFO` & `pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelpay-sdk
-Version: 2.1.1
+Version: 2.1.2
 Summary: PixelPay SDK toolkit.
 Author: Javier Cano
 Author-email: javier@pixel.hn
 License: MIT
 Keywords: pixelpay pixel pay sdk
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/SOURCES.txt` & `pixelpay-sdk-2.1.2/pixelpay_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/setup.py` & `pixelpay-sdk-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/assets/countries.json` & `pixelpay-sdk-2.1.2/src/pixelpay/assets/countries.json`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/assets/formats.json` & `pixelpay-sdk-2.1.2/src/pixelpay/assets/formats.json`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/assets/states.json` & `pixelpay-sdk-2.1.2/src/pixelpay/assets/states.json`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/base/Helpers.py` & `pixelpay-sdk-2.1.2/src/pixelpay/base/Helpers.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/base/RequestBehaviour.py` & `pixelpay-sdk-2.1.2/src/pixelpay/base/RequestBehaviour.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         self.from_type: str = "sdk-python"
         """SDK identifier type"""
 
         self.sdk_version: str = __version__
         """SDK version"""
 
-        self.sdk_public_key: str = None
+        self._sdk_public_key: str = None
         """For internal use to prevent encrypting same request instance twice"""
 
     def isEncryptable(self) -> bool:
         """Check if current request needs encryption, must be overriden by inherited classes.
 
         Returns:
             bool: true if request contains parameters that must be encrypted
```

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/base/Response.py` & `pixelpay-sdk-2.1.2/src/pixelpay/base/Response.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/base/ServiceBehaviour.py` & `pixelpay-sdk-2.1.2/src/pixelpay/base/ServiceBehaviour.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,16 +157,14 @@
         """
         if not request.isEncryptable():
             return
 
         self.__validateMerchantPublicKey()
         self.__validateSDKPublicKey(request)
 
-        self.__sdk_public_key = request.sdk_public_key
-
     def __validateMerchantPublicKey(self):
         """Resiliently fetch merchant public key, trying at least 3 times before failing
 
         Raises:
             InvalidCredentialsException: When invalid or no credentials are provided
         """
         tries = 0
```

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/entities/CardResult.py` & `pixelpay-sdk-2.1.2/src/pixelpay/entities/CardResult.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/entities/TransactionResult.py` & `pixelpay-sdk-2.1.2/src/pixelpay/entities/TransactionResult.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/models/Billing.py` & `pixelpay-sdk-2.1.2/src/pixelpay/models/Billing.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/models/Card.py` & `pixelpay-sdk-2.1.2/src/pixelpay/models/Card.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/models/Item.py` & `pixelpay-sdk-2.1.2/src/pixelpay/models/Item.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/models/Order.py` & `pixelpay-sdk-2.1.2/src/pixelpay/models/Order.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/models/Settings.py` & `pixelpay-sdk-2.1.2/src/pixelpay/models/Settings.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/requests/CardTokenization.py` & `pixelpay-sdk-2.1.2/src/pixelpay/requests/CardTokenization.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,16 +93,16 @@
 
         Raises:
             FailedEncryptionException: When public key is empty or encryption fails
 
         Returns:
             str: SDK public key
         """
-        if self.sdk_public_key:
-            return self.sdk_public_key
+        if self._sdk_public_key:
+            return self._sdk_public_key
 
         if not public_key:
             raise FailedEncryptionException("Could not process transaction without merchant public key.")
 
         try:
             key_pair = Helpers.getKeyPair()
 
@@ -114,12 +114,12 @@
             sdk_public_key = key_pair.public_key.encode(encoder=Base64Encoder).decode()
 
             self.number = number
             self.cvv2 = cvv2
             self.expire_month = expire_month
             self.expire_year = expire_year
 
-            self.sdk_public_key = sdk_public_key
+            self._sdk_public_key = sdk_public_key
 
-            return key_pair.public_key.encode(encoder=Base64Encoder).decode()
+            return self._sdk_public_key
         except:
             raise FailedEncryptionException("Encryption process encountered an unexpected error.")
```

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/requests/PaymentTransaction.py` & `pixelpay-sdk-2.1.2/src/pixelpay/requests/PaymentTransaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,16 +159,16 @@
 
         Raises:
             FailedEncryptionException: When public key is empty or encryption fails
 
         Returns:
             str: SDK public key
         """
-        if self.sdk_public_key:
-            return self.sdk_public_key
+        if self._sdk_public_key:
+            return self._sdk_public_key
 
         if not public_key:
             raise FailedEncryptionException("Could not process transaction without merchant public key.")
 
         try:
             key_pair = Helpers.getKeyPair()
 
@@ -178,12 +178,12 @@
 
             sdk_public_key = key_pair.public_key.encode(encoder=Base64Encoder).decode()
 
             self.card_number = card_number
             self.card_cvv = card_cvv
             self.card_expire = card_expire
 
-            self.sdk_public_key = sdk_public_key
+            self._sdk_public_key = sdk_public_key
 
-            return self.sdk_public_key
+            return self._sdk_public_key
         except:
             raise FailedEncryptionException("Encryption process encountered an unexpected error.")
```

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/requests/SaleTransaction.py` & `pixelpay-sdk-2.1.2/src/pixelpay/requests/SaleTransaction.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/requests/__init__.py` & `pixelpay-sdk-2.1.2/src/pixelpay/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/resources/Locations.py` & `pixelpay-sdk-2.1.2/src/pixelpay/resources/Locations.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/responses/__init__.py` & `pixelpay-sdk-2.1.2/src/pixelpay/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/services/Tokenization.py` & `pixelpay-sdk-2.1.2/src/pixelpay/services/Tokenization.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.1/src/pixelpay/services/Transaction.py` & `pixelpay-sdk-2.1.2/src/pixelpay/services/Transaction.py`

 * *Files identical despite different names*

