# Comparing `tmp/pixelpay-sdk-2.1.0.tar.gz` & `tmp/pixelpay-sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelpay-sdk-2.1.0.tar", last modified: Wed Jul 19 22:30:43 2023, max compression
+gzip compressed data, was "pixelpay-sdk-2.1.1.tar", last modified: Thu Jul 27 22:10:34 2023, max compression
```

## Comparing `pixelpay-sdk-2.1.0.tar` & `pixelpay-sdk-2.1.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-19 22:30:43.989982 pixelpay-sdk-2.1.0/
--rw-r--r--   0 javiercano   (501) staff       (20)     1088 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/LICENSE.md
--rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-07-19 22:30:43.989810 pixelpay-sdk-2.1.0/PKG-INFO
--rw-r--r--   0 javiercano   (501) staff       (20)      455 2023-06-07 22:52:21.000000 pixelpay-sdk-2.1.0/README.md
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-19 22:30:43.966158 pixelpay-sdk-2.1.0/pixelpay_sdk.egg-info/
--rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-07-19 22:30:43.000000 pixelpay-sdk-2.1.0/pixelpay_sdk.egg-info/PKG-INFO
--rw-r--r--   0 javiercano   (501) staff       (20)     2026 2023-07-19 22:30:43.000000 pixelpay-sdk-2.1.0/pixelpay_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 javiercano   (501) staff       (20)        1 2023-07-19 22:30:43.000000 pixelpay-sdk-2.1.0/pixelpay_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 javiercano   (501) staff       (20)       31 2023-07-19 22:30:43.000000 pixelpay-sdk-2.1.0/pixelpay_sdk.egg-info/requires.txt
--rw-r--r--   0 javiercano   (501) staff       (20)        9 2023-07-19 22:30:43.000000 pixelpay-sdk-2.1.0/pixelpay_sdk.egg-info/top_level.txt
--rw-r--r--   0 javiercano   (501) staff       (20)       85 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/pyproject.toml
--rw-r--r--   0 javiercano   (501) staff       (20)       38 2023-07-19 22:30:43.990021 pixelpay-sdk-2.1.0/setup.cfg
--rw-r--r--   0 javiercano   (501) staff       (20)     1398 2023-07-19 22:28:45.000000 pixelpay-sdk-2.1.0/setup.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-19 22:30:43.957370 pixelpay-sdk-2.1.0/src/
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-19 22:30:43.966422 pixelpay-sdk-2.1.0/src/pixelpay/
--rw-r--r--   0 javiercano   (501) staff       (20)      365 2023-07-18 20:28:51.000000 pixelpay-sdk-2.1.0/src/pixelpay/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-19 22:30:43.969695 pixelpay-sdk-2.1.0/src/pixelpay/assets/
--rw-r--r--   0 javiercano   (501) staff       (20)     5438 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/assets/countries.json
--rw-r--r--   0 javiercano   (501) staff       (20)    18333 2023-01-26 21:25:46.000000 pixelpay-sdk-2.1.0/src/pixelpay/assets/formats.json
--rw-r--r--   0 javiercano   (501) staff       (20)    88971 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/assets/states.json
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-19 22:30:43.973611 pixelpay-sdk-2.1.0/src/pixelpay/base/
--rw-r--r--   0 javiercano   (501) staff       (20)     3185 2023-07-19 22:25:29.000000 pixelpay-sdk-2.1.0/src/pixelpay/base/Helpers.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1612 2023-07-19 20:05:04.000000 pixelpay-sdk-2.1.0/src/pixelpay/base/RequestBehaviour.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1804 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/base/Response.py
--rw-r--r--   0 javiercano   (501) staff       (20)     8045 2023-07-19 22:22:36.000000 pixelpay-sdk-2.1.0/src/pixelpay/base/ServiceBehaviour.py
--rw-r--r--   0 javiercano   (501) staff       (20)      248 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/base/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-19 22:30:43.974711 pixelpay-sdk-2.1.0/src/pixelpay/entities/
--rw-r--r--   0 javiercano   (501) staff       (20)     1812 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/entities/CardResult.py
--rw-r--r--   0 javiercano   (501) staff       (20)     3028 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/entities/TransactionResult.py
--rw-r--r--   0 javiercano   (501) staff       (20)      142 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/entities/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-19 22:30:43.975729 pixelpay-sdk-2.1.0/src/pixelpay/exceptions/
--rw-r--r--   0 javiercano   (501) staff       (20)       55 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/exceptions/InvalidCredentialsException.py
--rw-r--r--   0 javiercano   (501) staff       (20)       59 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/exceptions/InvalidTransactionTypeException.py
--rw-r--r--   0 javiercano   (501) staff       (20)      235 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/exceptions/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-19 22:30:43.978679 pixelpay-sdk-2.1.0/src/pixelpay/models/
--rw-r--r--   0 javiercano   (501) staff       (20)      512 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/models/Billing.py
--rw-r--r--   0 javiercano   (501) staff       (20)      656 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/models/Card.py
--rw-r--r--   0 javiercano   (501) staff       (20)      653 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/models/Item.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1873 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/models/Order.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1914 2023-07-19 22:22:39.000000 pixelpay-sdk-2.1.0/src/pixelpay/models/Settings.py
--rw-r--r--   0 javiercano   (501) staff       (20)      214 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/models/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-19 22:30:43.982708 pixelpay-sdk-2.1.0/src/pixelpay/requests/
--rw-r--r--   0 javiercano   (501) staff       (20)      105 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/requests/AuthTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      358 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/requests/CaptureTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)     3233 2023-07-19 20:14:45.000000 pixelpay-sdk-2.1.0/src/pixelpay/requests/CardTokenization.py
--rw-r--r--   0 javiercano   (501) staff       (20)     5282 2023-07-19 22:22:43.000000 pixelpay-sdk-2.1.0/src/pixelpay/requests/PaymentTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1020 2023-06-07 22:41:02.000000 pixelpay-sdk-2.1.0/src/pixelpay/requests/SaleTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      198 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/requests/StatusTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      372 2023-06-07 22:21:17.000000 pixelpay-sdk-2.1.0/src/pixelpay/requests/VoidTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      518 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/requests/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-19 22:30:43.983946 pixelpay-sdk-2.1.0/src/pixelpay/resources/
--rw-r--r--   0 javiercano   (501) staff       (20)      123 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/resources/Environment.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1657 2023-01-26 21:27:02.000000 pixelpay-sdk-2.1.0/src/pixelpay/resources/Locations.py
--rw-r--r--   0 javiercano   (501) staff       (20)      121 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/resources/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-19 22:30:43.988534 pixelpay-sdk-2.1.0/src/pixelpay/responses/
--rw-r--r--   0 javiercano   (501) staff       (20)       70 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/responses/ErrorResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/responses/FailureResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       75 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/responses/InputErrorResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/responses/NetworkFailureResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/responses/NoAccessResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/responses/NotFoundResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/responses/PayloadResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       80 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/responses/PaymentDeclinedResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/responses/PreconditionalResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/responses/SuccessResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/responses/TimeoutResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)      838 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/responses/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-19 22:30:43.989431 pixelpay-sdk-2.1.0/src/pixelpay/services/
--rw-r--r--   0 javiercano   (501) staff       (20)     2081 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/services/Tokenization.py
--rw-r--r--   0 javiercano   (501) staff       (20)     2471 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/services/Transaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      130 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.0/src/pixelpay/services/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.518496 pixelpay-sdk-2.1.1/
+-rw-r--r--   0 javiercano   (501) staff       (20)     1088 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/LICENSE.md
+-rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-07-27 22:10:34.518328 pixelpay-sdk-2.1.1/PKG-INFO
+-rw-r--r--   0 javiercano   (501) staff       (20)      455 2023-06-07 22:52:21.000000 pixelpay-sdk-2.1.1/README.md
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.503161 pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/
+-rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-07-27 22:10:34.000000 pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 javiercano   (501) staff       (20)     2079 2023-07-27 22:10:34.000000 pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)        1 2023-07-27 22:10:34.000000 pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)       31 2023-07-27 22:10:34.000000 pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/requires.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)        9 2023-07-27 22:10:34.000000 pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/top_level.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)       85 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/pyproject.toml
+-rw-r--r--   0 javiercano   (501) staff       (20)       38 2023-07-27 22:10:34.518546 pixelpay-sdk-2.1.1/setup.cfg
+-rw-r--r--   0 javiercano   (501) staff       (20)     1398 2023-07-19 22:28:45.000000 pixelpay-sdk-2.1.1/setup.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.493820 pixelpay-sdk-2.1.1/src/
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.503446 pixelpay-sdk-2.1.1/src/pixelpay/
+-rw-r--r--   0 javiercano   (501) staff       (20)      365 2023-07-27 20:13:44.000000 pixelpay-sdk-2.1.1/src/pixelpay/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.504872 pixelpay-sdk-2.1.1/src/pixelpay/assets/
+-rw-r--r--   0 javiercano   (501) staff       (20)     5438 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/assets/countries.json
+-rw-r--r--   0 javiercano   (501) staff       (20)    18333 2023-01-26 21:25:46.000000 pixelpay-sdk-2.1.1/src/pixelpay/assets/formats.json
+-rw-r--r--   0 javiercano   (501) staff       (20)    88971 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/assets/states.json
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.506995 pixelpay-sdk-2.1.1/src/pixelpay/base/
+-rw-r--r--   0 javiercano   (501) staff       (20)     3185 2023-07-19 22:25:29.000000 pixelpay-sdk-2.1.1/src/pixelpay/base/Helpers.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1994 2023-07-27 20:23:07.000000 pixelpay-sdk-2.1.1/src/pixelpay/base/RequestBehaviour.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1804 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/base/Response.py
+-rw-r--r--   0 javiercano   (501) staff       (20)    10062 2023-07-27 22:06:41.000000 pixelpay-sdk-2.1.1/src/pixelpay/base/ServiceBehaviour.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      248 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/base/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.507742 pixelpay-sdk-2.1.1/src/pixelpay/entities/
+-rw-r--r--   0 javiercano   (501) staff       (20)     1812 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/entities/CardResult.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     3028 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/entities/TransactionResult.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      142 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/entities/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.508917 pixelpay-sdk-2.1.1/src/pixelpay/exceptions/
+-rw-r--r--   0 javiercano   (501) staff       (20)       53 2023-07-27 21:35:29.000000 pixelpay-sdk-2.1.1/src/pixelpay/exceptions/FailedEncryptionException.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       55 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/exceptions/InvalidCredentialsException.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       59 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/exceptions/InvalidTransactionTypeException.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      333 2023-07-27 21:35:45.000000 pixelpay-sdk-2.1.1/src/pixelpay/exceptions/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.510661 pixelpay-sdk-2.1.1/src/pixelpay/models/
+-rw-r--r--   0 javiercano   (501) staff       (20)      512 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/models/Billing.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      656 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/models/Card.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      653 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/models/Item.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1873 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/models/Order.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1914 2023-07-27 22:07:03.000000 pixelpay-sdk-2.1.1/src/pixelpay/models/Settings.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      214 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/models/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.513227 pixelpay-sdk-2.1.1/src/pixelpay/requests/
+-rw-r--r--   0 javiercano   (501) staff       (20)      105 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/AuthTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      358 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/CaptureTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     3925 2023-07-27 20:49:27.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/CardTokenization.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     5947 2023-07-27 22:06:29.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/PaymentTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1020 2023-06-07 22:41:02.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/SaleTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      198 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/StatusTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      372 2023-06-07 22:21:17.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/VoidTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      518 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/requests/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.514332 pixelpay-sdk-2.1.1/src/pixelpay/resources/
+-rw-r--r--   0 javiercano   (501) staff       (20)      123 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/resources/Environment.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1657 2023-01-26 21:27:02.000000 pixelpay-sdk-2.1.1/src/pixelpay/resources/Locations.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      121 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/resources/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.517348 pixelpay-sdk-2.1.1/src/pixelpay/responses/
+-rw-r--r--   0 javiercano   (501) staff       (20)       70 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/ErrorResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/FailureResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       75 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/InputErrorResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/NetworkFailureResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/NoAccessResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/NotFoundResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/PayloadResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       80 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/PaymentDeclinedResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/PreconditionalResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/SuccessResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/TimeoutResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      838 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/responses/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-07-27 22:10:34.518077 pixelpay-sdk-2.1.1/src/pixelpay/services/
+-rw-r--r--   0 javiercano   (501) staff       (20)     2081 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/services/Tokenization.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     2471 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/services/Transaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      130 2022-09-21 22:36:22.000000 pixelpay-sdk-2.1.1/src/pixelpay/services/__init__.py
```

### Comparing `pixelpay-sdk-2.1.0/LICENSE.md` & `pixelpay-sdk-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/PKG-INFO` & `pixelpay-sdk-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelpay-sdk
-Version: 2.1.0
+Version: 2.1.1
 Summary: PixelPay SDK toolkit.
 Author: Javier Cano
 Author-email: javier@pixel.hn
 License: MIT
 Keywords: pixelpay pixel pay sdk
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pixelpay-sdk-2.1.0/pixelpay_sdk.egg-info/PKG-INFO` & `pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelpay-sdk
-Version: 2.1.0
+Version: 2.1.1
 Summary: PixelPay SDK toolkit.
 Author: Javier Cano
 Author-email: javier@pixel.hn
 License: MIT
 Keywords: pixelpay pixel pay sdk
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pixelpay-sdk-2.1.0/pixelpay_sdk.egg-info/SOURCES.txt` & `pixelpay-sdk-2.1.1/pixelpay_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/pixelpay/base/RequestBehaviour.py
 src/pixelpay/base/Response.py
 src/pixelpay/base/ServiceBehaviour.py
 src/pixelpay/base/__init__.py
 src/pixelpay/entities/CardResult.py
 src/pixelpay/entities/TransactionResult.py
 src/pixelpay/entities/__init__.py
+src/pixelpay/exceptions/FailedEncryptionException.py
 src/pixelpay/exceptions/InvalidCredentialsException.py
 src/pixelpay/exceptions/InvalidTransactionTypeException.py
 src/pixelpay/exceptions/__init__.py
 src/pixelpay/models/Billing.py
 src/pixelpay/models/Card.py
 src/pixelpay/models/Item.py
 src/pixelpay/models/Order.py
```

### Comparing `pixelpay-sdk-2.1.0/setup.py` & `pixelpay-sdk-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/assets/countries.json` & `pixelpay-sdk-2.1.1/src/pixelpay/assets/countries.json`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/assets/formats.json` & `pixelpay-sdk-2.1.1/src/pixelpay/assets/formats.json`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/assets/states.json` & `pixelpay-sdk-2.1.1/src/pixelpay/assets/states.json`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/base/Helpers.py` & `pixelpay-sdk-2.1.1/src/pixelpay/base/Helpers.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/base/RequestBehaviour.py` & `pixelpay-sdk-2.1.1/src/pixelpay/base/RequestBehaviour.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,25 @@
 
         self.from_type: str = "sdk-python"
         """SDK identifier type"""
 
         self.sdk_version: str = __version__
         """SDK version"""
 
+        self.sdk_public_key: str = None
+        """For internal use to prevent encrypting same request instance twice"""
+
+    def isEncryptable(self) -> bool:
+        """Check if current request needs encryption, must be overriden by inherited classes.
+
+        Returns:
+            bool: true if request contains parameters that must be encrypted
+        """
+        return False
+
     def withEncryption(self, public_key: str) -> str:
         """Encrypt fields with sensitive data, must be overriden by inherited classes.
 
         Args:
             public_key (str): merchant public key
 
         Returns:
```

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/base/Response.py` & `pixelpay-sdk-2.1.1/src/pixelpay/base/Response.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/base/ServiceBehaviour.py` & `pixelpay-sdk-2.1.1/src/pixelpay/base/ServiceBehaviour.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 from .Response import Response
 from ..exceptions import InvalidCredentialsException
+from ..exceptions import FailedEncryptionException
 from ..responses import ErrorResponse
 from ..responses import FailureResponse
 from ..responses import InputErrorResponse
 from ..responses import NetworkFailureResponse
 from ..responses import NoAccessResponse
 from ..responses import NotFoundResponse
 from ..responses import PayloadResponse
@@ -89,14 +90,15 @@
 
         Returns:
             Response: processed response
         """
         response = FailureResponse()
         response.success = False
         response.message = str(e)
+        response.setStatus(520)
 
         return response
 
     def __buildRequest(self, url: str, method: str, transaction: RequestBehaviour) -> requests.PreparedRequest:
         """Build HTTP request to API
 
         Args:
@@ -143,24 +145,84 @@
 
         return request
 
     def __validateEncryption(self, request: RequestBehaviour):
         """Verify and set request encryption values
 
         Args:
-            body (RequestBehaviour): unencrypted request
+            request (RequestBehaviour): unencrypted request
+
+        Raises:
+            InvalidCredentialsException: When invalid or no credentials are provided
+            FailedEncryptionException: When encryption process fails
         """
+        if not request.isEncryptable():
+            return
+
+        self.__validateMerchantPublicKey()
+        self.__validateSDKPublicKey(request)
+
+        self.__sdk_public_key = request.sdk_public_key
+
+    def __validateMerchantPublicKey(self):
+        """Resiliently fetch merchant public key, trying at least 3 times before failing
+
+        Raises:
+            InvalidCredentialsException: When invalid or no credentials are provided
+        """
+        tries = 0
+
+        while not self._settings.public_key and tries < 3:
+            self._settings.public_key = self.__fetchMerchantPublicKey()
+            tries += 1
+
         if not self._settings.public_key:
-            response = self._get(PUBLIC_KEY_PATH, RequestBehaviour())
+            raise InvalidCredentialsException("Could not obtain necessary credentials for transaction.")
+
+    def __validateSDKPublicKey(self, request: RequestBehaviour):
+        """Resiliently generate keys and encrypt request, trying at least 3 times before failing
+
+        Args:
+            request (RequestBehaviour): unencrypted request
+
+        Raises:
+            FailedEncryptionException: When encryption process fails
+        """
+        tries = 0
+        last_error: FailedEncryptionException = None
+
+        while not self.__sdk_public_key and tries < 3:
+            try:
+                self.__sdk_public_key = request.withEncryption(self._settings.public_key)
+            except Exception as e:
+                last_error = e
+            finally:
+                tries += 1
+
+        if not self.__sdk_public_key and last_error:
+            raise last_error
+
+        if not self.__sdk_public_key:
+            raise FailedEncryptionException("Could not process encryption, please try again.")
+
+    def __fetchMerchantPublicKey(self) -> str:
+        """Fetch merchant public key for encryption
+
+        Raises:
+            InvalidCredentialsException: When no credentials are provided
+
+        Returns:
+            str: merchant public key or None
+        """
+        response = self._get(PUBLIC_KEY_PATH, RequestBehaviour())
 
-            if response.success:
-                self._settings.public_key = response.getData("public_key")
+        if response.success:
+            return response.getData("public_key")
 
-        if self._settings.public_key:
-            self.__sdk_public_key = request.withEncryption(self._settings.public_key)
+        return None
 
     def __getRoute(self, route: str):
         """Get API route
 
         Args:
             route (str): input route
```

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/entities/CardResult.py` & `pixelpay-sdk-2.1.1/src/pixelpay/entities/CardResult.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/entities/TransactionResult.py` & `pixelpay-sdk-2.1.1/src/pixelpay/entities/TransactionResult.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/models/Billing.py` & `pixelpay-sdk-2.1.1/src/pixelpay/models/Billing.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/models/Card.py` & `pixelpay-sdk-2.1.1/src/pixelpay/models/Card.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/models/Item.py` & `pixelpay-sdk-2.1.1/src/pixelpay/models/Item.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/models/Order.py` & `pixelpay-sdk-2.1.1/src/pixelpay/models/Order.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/models/Settings.py` & `pixelpay-sdk-2.1.1/src/pixelpay/models/Settings.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/requests/SaleTransaction.py` & `pixelpay-sdk-2.1.1/src/pixelpay/requests/SaleTransaction.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/requests/__init__.py` & `pixelpay-sdk-2.1.1/src/pixelpay/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/resources/Locations.py` & `pixelpay-sdk-2.1.1/src/pixelpay/resources/Locations.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/responses/__init__.py` & `pixelpay-sdk-2.1.1/src/pixelpay/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/services/Tokenization.py` & `pixelpay-sdk-2.1.1/src/pixelpay/services/Tokenization.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.1.0/src/pixelpay/services/Transaction.py` & `pixelpay-sdk-2.1.1/src/pixelpay/services/Transaction.py`

 * *Files identical despite different names*

