# Comparing `tmp/easypost-8.0.0.tar.gz` & `tmp/easypost-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypost-8.0.0.tar", last modified: Tue Jun  6 21:45:20 2023, max compression
+gzip compressed data, was "easypost-8.1.0.tar", last modified: Fri Jul 28 16:09:19 2023, max compression
```

## Comparing `easypost-8.0.0.tar` & `easypost-8.1.0.tar`

### file list

```diff
@@ -1,138 +1,144 @@
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.447738 easypost-8.0.0/
--rw-r--r--   0 jhammond   (502) staff       (20)    11825 2023-06-06 21:44:38.000000 easypost-8.0.0/CHANGELOG.md
--rw-r--r--   0 jhammond   (502) staff       (20)     1092 2021-11-01 16:53:26.000000 easypost-8.0.0/LICENSE
--rw-r--r--   0 jhammond   (502) staff       (20)       13 2021-11-01 16:53:26.000000 easypost-8.0.0/MANIFEST.in
--rw-r--r--   0 jhammond   (502) staff       (20)     7249 2023-06-06 21:45:20.447541 easypost-8.0.0/PKG-INFO
--rw-r--r--   0 jhammond   (502) staff       (20)     6163 2023-05-31 19:04:35.000000 easypost-8.0.0/README.md
--rw-r--r--   0 jhammond   (502) staff       (20)     7100 2023-06-06 21:44:38.000000 easypost-8.0.0/UPGRADE_GUIDE.md
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.432503 easypost-8.0.0/easypost/
--rw-r--r--   0 jhammond   (502) staff       (20)      373 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1947 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/constant.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3728 2023-06-06 21:44:36.000000 easypost-8.0.0/easypost/easypost_client.py
--rw-r--r--   0 jhammond   (502) staff       (20)     6705 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/easypost_object.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.433339 easypost-8.0.0/easypost/errors/
--rw-r--r--   0 jhammond   (502) staff       (20)       87 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/__init__.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.436463 easypost-8.0.0/easypost/errors/api/
--rw-r--r--   0 jhammond   (502) staff       (20)     1187 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2327 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/api_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/encoding_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       96 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/external_api_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/forbidden_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/gateway_timeout_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       89 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/http_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/internal_server_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/invalid_request_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       89 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/json_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      101 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/method_not_allowed_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/not_found_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/payment_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/rate_limit_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/redirect_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      103 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/service_unavailable_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/timeout_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       97 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/unauthorized_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)       95 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/unknown_api_error.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.437578 easypost-8.0.0/easypost/errors/general/
--rw-r--r--   0 jhammond   (502) staff       (20)      560 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)      206 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/easypost_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      119 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/end_of_pagination_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      113 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/filtering_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      117 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/invalid_object_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      120 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/invalid_parameter_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      120 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/missing_parameter_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)      125 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/signature_verification_error.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.440616 easypost-8.0.0/easypost/models/
--rw-r--r--   0 jhammond   (502) staff       (20)     1145 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/address.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/api_key.py
--rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/batch.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/billing.py
--rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/brand.py
--rw-r--r--   0 jhammond   (502) staff       (20)      101 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/carrier_account.py
--rw-r--r--   0 jhammond   (502) staff       (20)       98 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/customs_info.py
--rw-r--r--   0 jhammond   (502) staff       (20)       98 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/customs_item.py
--rw-r--r--   0 jhammond   (502) staff       (20)       97 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/end_shipper.py
--rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/event.py
--rw-r--r--   0 jhammond   (502) staff       (20)       96 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/insurance.py
--rw-r--r--   0 jhammond   (502) staff       (20)      477 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/order.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/parcel.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/payload.py
--rw-r--r--   0 jhammond   (502) staff       (20)      495 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/pickup.py
--rw-r--r--   0 jhammond   (502) staff       (20)       97 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/pickup_rate.py
--rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/postage_label.py
--rw-r--r--   0 jhammond   (502) staff       (20)       91 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/rate.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/refund.py
--rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/report.py
--rw-r--r--   0 jhammond   (502) staff       (20)       95 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/scan_form.py
--rw-r--r--   0 jhammond   (502) staff       (20)      483 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/shipment.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/tracker.py
--rw-r--r--   0 jhammond   (502) staff       (20)       91 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/user.py
--rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/webhook.py
--rw-r--r--   0 jhammond   (502) staff       (20)        0 2022-07-05 19:20:56.000000 easypost-8.0.0/easypost/py.typed
--rw-r--r--   0 jhammond   (502) staff       (20)    11789 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/requestor.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.444168 easypost-8.0.0/easypost/services/
--rw-r--r--   0 jhammond   (502) staff       (20)     1650 2023-06-06 21:44:36.000000 easypost-8.0.0/easypost/services/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2469 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/address_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     4159 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/base_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3266 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/batch_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1244 2023-06-06 21:44:36.000000 easypost-8.0.0/easypost/services/beta_carrier_metadata_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)      898 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/beta_rate_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2339 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/beta_referral_customer_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2805 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/billing_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2470 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/carrier_account_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1013 2023-06-06 21:44:36.000000 easypost-8.0.0/easypost/services/carrier_metadata_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)      546 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/customs_info_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)      546 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/customs_item_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1665 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/end_shipper_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1972 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/event_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1102 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/insurance_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1650 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/order_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)      511 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/parcel_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1823 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/pickup_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)      361 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/rate_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     5366 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/referral_customer_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1102 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/refund_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2390 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/report_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1091 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/scan_form_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     5750 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/shipment_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1956 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/tracker_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3131 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/user_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)      996 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/webhook_service.py
--rw-r--r--   0 jhammond   (502) staff       (20)     4560 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/util.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.433205 easypost-8.0.0/easypost.egg-info/
--rw-r--r--   0 jhammond   (502) staff       (20)     7249 2023-06-06 21:45:20.000000 easypost-8.0.0/easypost.egg-info/PKG-INFO
--rw-r--r--   0 jhammond   (502) staff       (20)     3994 2023-06-06 21:45:20.000000 easypost-8.0.0/easypost.egg-info/SOURCES.txt
--rw-r--r--   0 jhammond   (502) staff       (20)        1 2023-06-06 21:45:20.000000 easypost-8.0.0/easypost.egg-info/dependency_links.txt
--rw-r--r--   0 jhammond   (502) staff       (20)      249 2023-06-06 21:45:20.000000 easypost-8.0.0/easypost.egg-info/requires.txt
--rw-r--r--   0 jhammond   (502) staff       (20)        9 2023-06-06 21:45:20.000000 easypost-8.0.0/easypost.egg-info/top_level.txt
--rw-r--r--   0 jhammond   (502) staff       (20)      272 2023-05-10 20:00:27.000000 easypost-8.0.0/pyproject.toml
--rw-r--r--   0 jhammond   (502) staff       (20)       38 2023-06-06 21:45:20.447799 easypost-8.0.0/setup.cfg
--rw-r--r--   0 jhammond   (502) staff       (20)     2125 2023-05-31 19:04:35.000000 easypost-8.0.0/setup.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.447335 easypost-8.0.0/tests/
--rw-r--r--   0 jhammond   (502) staff       (20)     4221 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_address.py
--rw-r--r--   0 jhammond   (502) staff       (20)     4436 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_batch.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1162 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_beta_carrier_metadata.py
--rw-r--r--   0 jhammond   (502) staff       (20)      792 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_beta_rate.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1854 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_beta_referral_customer.py
--rw-r--r--   0 jhammond   (502) staff       (20)     4084 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_billing.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3344 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_carrier_account.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1108 2023-06-06 21:44:36.000000 easypost-8.0.0/tests/test_carrier_metadata.py
--rw-r--r--   0 jhammond   (502) staff       (20)      719 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_customs_info.py
--rw-r--r--   0 jhammond   (502) staff       (20)      708 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_customs_item.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1818 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_easypost_client.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1739 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_end_shipper.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2285 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_error.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3548 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_event.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2167 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_insurance.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2323 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_order.py
--rw-r--r--   0 jhammond   (502) staff       (20)      574 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_parcel.py
--rw-r--r--   0 jhammond   (502) staff       (20)     4184 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_pickup.py
--rw-r--r--   0 jhammond   (502) staff       (20)      322 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_rate.py
--rw-r--r--   0 jhammond   (502) staff       (20)     4655 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_referral_customer.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1887 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_refund.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2825 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_report.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1776 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_scan_form.py
--rw-r--r--   0 jhammond   (502) staff       (20)    13013 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_shipment.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2128 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_tracker.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3078 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_user.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3263 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_webhook.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-07-28 16:09:19.507383 easypost-8.1.0/
+-rw-r--r--   0 jhammond   (502) staff       (20)    12151 2023-07-28 16:08:36.000000 easypost-8.1.0/CHANGELOG.md
+-rw-r--r--   0 jhammond   (502) staff       (20)     1092 2021-11-01 16:53:26.000000 easypost-8.1.0/LICENSE
+-rw-r--r--   0 jhammond   (502) staff       (20)       13 2021-11-01 16:53:26.000000 easypost-8.1.0/MANIFEST.in
+-rw-r--r--   0 jhammond   (502) staff       (20)     8048 2023-07-28 16:09:19.507221 easypost-8.1.0/PKG-INFO
+-rw-r--r--   0 jhammond   (502) staff       (20)     6962 2023-07-21 15:49:10.000000 easypost-8.1.0/README.md
+-rw-r--r--   0 jhammond   (502) staff       (20)     7100 2023-06-26 19:26:52.000000 easypost-8.1.0/UPGRADE_GUIDE.md
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-07-28 16:09:19.488638 easypost-8.1.0/easypost/
+-rw-r--r--   0 jhammond   (502) staff       (20)      373 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1947 2023-07-28 16:08:36.000000 easypost-8.1.0/easypost/constant.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4549 2023-07-19 16:33:01.000000 easypost-8.1.0/easypost/easypost_client.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     6705 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/easypost_object.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-07-28 16:09:19.489587 easypost-8.1.0/easypost/errors/
+-rw-r--r--   0 jhammond   (502) staff       (20)       87 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/__init__.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-07-28 16:09:19.492442 easypost-8.1.0/easypost/errors/api/
+-rw-r--r--   0 jhammond   (502) staff       (20)     1253 2023-07-21 17:45:32.000000 easypost-8.1.0/easypost/errors/api/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2327 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/api_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       95 2023-07-21 17:45:32.000000 easypost-8.1.0/easypost/errors/api/bad_request_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/encoding_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       96 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/external_api_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/forbidden_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/gateway_timeout_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       89 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/http_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/internal_server_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/invalid_request_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       89 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/json_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      101 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/method_not_allowed_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/not_found_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/payment_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/rate_limit_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/redirect_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      103 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/service_unavailable_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/timeout_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       97 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/unauthorized_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       95 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/api/unknown_api_error.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-07-28 16:09:19.494040 easypost-8.1.0/easypost/errors/general/
+-rw-r--r--   0 jhammond   (502) staff       (20)      560 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/general/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      206 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/general/easypost_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      119 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/general/end_of_pagination_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      113 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/general/filtering_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      117 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/general/invalid_object_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      120 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/general/invalid_parameter_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      120 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/general/missing_parameter_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      125 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/errors/general/signature_verification_error.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-07-28 16:09:19.494559 easypost-8.1.0/easypost/hooks/
+-rw-r--r--   0 jhammond   (502) staff       (20)      169 2023-07-19 16:33:01.000000 easypost-8.1.0/easypost/hooks/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      475 2023-07-19 16:33:01.000000 easypost-8.1.0/easypost/hooks/event_hook.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      147 2023-07-19 16:33:01.000000 easypost-8.1.0/easypost/hooks/request_hook.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      154 2023-07-19 16:33:01.000000 easypost-8.1.0/easypost/hooks/response_hook.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-07-28 16:09:19.498726 easypost-8.1.0/easypost/models/
+-rw-r--r--   0 jhammond   (502) staff       (20)     1145 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/address.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/api_key.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/batch.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/billing.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/brand.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      101 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/carrier_account.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       98 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/customs_info.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       98 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/customs_item.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       97 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/end_shipper.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/event.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       96 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/insurance.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      477 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/order.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/parcel.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/payload.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      495 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/pickup.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       97 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/pickup_rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/postage_label.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       91 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/refund.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/report.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       95 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/scan_form.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      483 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/shipment.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/tracker.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       91 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/user.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/models/webhook.py
+-rw-r--r--   0 jhammond   (502) staff       (20)        0 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/py.typed
+-rw-r--r--   0 jhammond   (502) staff       (20)    12807 2023-07-21 17:45:32.000000 easypost-8.1.0/easypost/requestor.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-07-28 16:09:19.502732 easypost-8.1.0/easypost/services/
+-rw-r--r--   0 jhammond   (502) staff       (20)     1650 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2469 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/address_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4159 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/base_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3266 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/batch_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1244 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/beta_carrier_metadata_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      898 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/beta_rate_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2339 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/beta_referral_customer_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2805 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/billing_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2470 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/carrier_account_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1013 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/carrier_metadata_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      546 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/customs_info_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      546 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/customs_item_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1665 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/end_shipper_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1972 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/event_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1102 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/insurance_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1650 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/order_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      511 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/parcel_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1823 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/pickup_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      361 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/rate_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     5365 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/referral_customer_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1102 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/refund_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2390 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/report_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1091 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/scan_form_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     5750 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/shipment_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1956 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/tracker_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3131 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/user_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      996 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/services/webhook_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4560 2023-06-26 19:26:52.000000 easypost-8.1.0/easypost/util.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-07-28 16:09:19.489427 easypost-8.1.0/easypost.egg-info/
+-rw-r--r--   0 jhammond   (502) staff       (20)     8048 2023-07-28 16:09:19.000000 easypost-8.1.0/easypost.egg-info/PKG-INFO
+-rw-r--r--   0 jhammond   (502) staff       (20)     4158 2023-07-28 16:09:19.000000 easypost-8.1.0/easypost.egg-info/SOURCES.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)        1 2023-07-28 16:09:19.000000 easypost-8.1.0/easypost.egg-info/dependency_links.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)      249 2023-07-28 16:09:19.000000 easypost-8.1.0/easypost.egg-info/requires.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)        9 2023-07-28 16:09:19.000000 easypost-8.1.0/easypost.egg-info/top_level.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)       38 2023-07-28 16:09:19.507439 easypost-8.1.0/setup.cfg
+-rw-r--r--   0 jhammond   (502) staff       (20)     2125 2023-07-28 16:08:36.000000 easypost-8.1.0/setup.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-07-28 16:09:19.506968 easypost-8.1.0/tests/
+-rw-r--r--   0 jhammond   (502) staff       (20)     4220 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_address.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4435 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_batch.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1162 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_beta_carrier_metadata.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      791 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_beta_rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1853 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_beta_referral_customer.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4083 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_billing.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3343 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_carrier_account.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1108 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_carrier_metadata.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      718 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_customs_info.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      707 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_customs_item.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1817 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_easypost_client.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1738 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_end_shipper.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2284 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3547 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_event.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2238 2023-07-19 16:33:01.000000 easypost-8.1.0/tests/test_hook.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2166 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_insurance.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2322 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_order.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      573 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_parcel.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4183 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_pickup.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      321 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4654 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_referral_customer.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1886 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_refund.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2824 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_report.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1775 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_scan_form.py
+-rw-r--r--   0 jhammond   (502) staff       (20)    13012 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_shipment.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2127 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_tracker.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3077 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_user.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3262 2023-06-26 19:26:52.000000 easypost-8.1.0/tests/test_webhook.py
```

### Comparing `easypost-8.0.0/CHANGELOG.md` & `easypost-8.1.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # CHANGELOG
 
+## v8.1.0 (2023-07-28)
+
+- Adds new `RequestHook` and `ResponseHook` events. (un)subscribe to them with the new `subscribe_to_request_hook`, `subscribe_to_response_hook`, `unsubscribe_from_request_hook`, or `unsubscribe_from_response_hook` methods of an `EasyPostClient`
+- Maps 400 status codes to new `BadRequestError` class
+
 ## v8.0.0 (2023-06-06)
 
 See our [Upgrade Guide](UPGRADE_GUIDE.md#upgrading-from-7x-to-80) for more details.
 
 - New `EasyPostClient` object
   - Logic is grouped together in Services and each EasyPost object has a new model (eg: `client.shipment.create()`)
 - Error handling overhaul
```

### Comparing `easypost-8.0.0/LICENSE` & `easypost-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/PKG-INFO` & `easypost-8.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypost
-Version: 8.0.0
+Version: 8.1.0
 Summary: EasyPost Shipping API Client Library for Python
 Home-page: https://easypost.com/
 Author: EasyPost
 Author-email: support@easypost.com
 Project-URL: Docs, https://www.easypost.com/docs/api
 Project-URL: Tracker, https://github.com/EasyPost/easypost-python/issues
 Project-URL: Source, https://github.com/EasyPost/easypost-python
@@ -85,14 +85,32 @@
 )
 
 bought_shipment = client.shipment.buy(shipment.id, rate=shipment.lowest_rate())
 
 print(bought_shipment)
 ```
 
+### HTTP Hooks
+
+Users can subscribe to HTTP requests and responses via the `RequestHook` and `ResponseHook` objects. To do so, pass a function to the `subscribe_to_request_hook` or `subscribe_to_response_hook` methods of an `EasyPostClient` object:
+
+```python
+def custom_function(**kwargs):
+    """Pass your code here, data about the request/response is contained within `kwargs`."""
+    print(f"Received a request with the status code of: {kwargs.get('http_status')}")
+
+client = easypost.EasyPostClient(os.getenv('EASYPOST_API_KEY'))
+
+client.subscribe_to_response_hook(custom_function)
+
+# Make your API calls here, your custom_function will trigger once a response is received
+```
+
+You can also unsubscribe your functions in a similar manner by using the `unsubscribe_from_request_hook` and `unsubscribe_from_response_hook` methods of a client object.
+
 ## Documentation
 
 API documentation can be found at: <https://easypost.com/docs/api>.
 
 Library documentation can be found on the web at: <https://easypost.github.io/easypost-python/> or by building them locally via the `make docs` command.
 
 Upgrading major versions of this project? Refer to the [Upgrade Guide](UPGRADE_GUIDE.md).
@@ -107,33 +125,28 @@
 
 ```bash
 # Install dependencies
 make install
 
 # Lint project
 make lint
-
-# Format project
-make format
+make lint-fix
 
 # Run tests
 EASYPOST_TEST_API_KEY=123... EASYPOST_PROD_API_KEY=123... make test
-
-# Run test coverage
 EASYPOST_TEST_API_KEY=123... EASYPOST_PROD_API_KEY=123... make coverage
 
 # Run security analysis
 make scan
 
 # Generate library documentation
 make docs
 
 # Update submodules
-git submodule init
-git submodule update --remote
+make update-examples-submodule
 ```
 
 ### Testing
 
 The test suite in this project was specifically built to produce consistent results on every run, regardless of when they run or who is running them. This project uses [VCR](https://github.com/kevin1024/vcrpy) to record and replay HTTP requests and responses via "cassettes". When the suite is run, the HTTP requests and responses for each test function will be saved to a cassette if they do not exist already and replayed from this saved file if they do, which saves the need to make live API calls on every test run. If you receive errors about a cassette expiring, delete and re-record the cassette to ensure the data is up-to-date.
 
 **Sensitive Data:** We've made every attempt to include scrubbers for sensitive data when recording cassettes so that PII or sensitive info does not persist in version control; however, please ensure when recording or re-recording cassettes that prior to committing your changes, no PII or sensitive information gets persisted by inspecting the cassette.
```

### Comparing `easypost-8.0.0/README.md` & `easypost-8.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -58,14 +58,32 @@
 )
 
 bought_shipment = client.shipment.buy(shipment.id, rate=shipment.lowest_rate())
 
 print(bought_shipment)
 ```
 
+### HTTP Hooks
+
+Users can subscribe to HTTP requests and responses via the `RequestHook` and `ResponseHook` objects. To do so, pass a function to the `subscribe_to_request_hook` or `subscribe_to_response_hook` methods of an `EasyPostClient` object:
+
+```python
+def custom_function(**kwargs):
+    """Pass your code here, data about the request/response is contained within `kwargs`."""
+    print(f"Received a request with the status code of: {kwargs.get('http_status')}")
+
+client = easypost.EasyPostClient(os.getenv('EASYPOST_API_KEY'))
+
+client.subscribe_to_response_hook(custom_function)
+
+# Make your API calls here, your custom_function will trigger once a response is received
+```
+
+You can also unsubscribe your functions in a similar manner by using the `unsubscribe_from_request_hook` and `unsubscribe_from_response_hook` methods of a client object.
+
 ## Documentation
 
 API documentation can be found at: <https://easypost.com/docs/api>.
 
 Library documentation can be found on the web at: <https://easypost.github.io/easypost-python/> or by building them locally via the `make docs` command.
 
 Upgrading major versions of this project? Refer to the [Upgrade Guide](UPGRADE_GUIDE.md).
@@ -80,33 +98,28 @@
 
 ```bash
 # Install dependencies
 make install
 
 # Lint project
 make lint
-
-# Format project
-make format
+make lint-fix
 
 # Run tests
 EASYPOST_TEST_API_KEY=123... EASYPOST_PROD_API_KEY=123... make test
-
-# Run test coverage
 EASYPOST_TEST_API_KEY=123... EASYPOST_PROD_API_KEY=123... make coverage
 
 # Run security analysis
 make scan
 
 # Generate library documentation
 make docs
 
 # Update submodules
-git submodule init
-git submodule update --remote
+make update-examples-submodule
 ```
 
 ### Testing
 
 The test suite in this project was specifically built to produce consistent results on every run, regardless of when they run or who is running them. This project uses [VCR](https://github.com/kevin1024/vcrpy) to record and replay HTTP requests and responses via "cassettes". When the suite is run, the HTTP requests and responses for each test function will be saved to a cassette if they do not exist already and replayed from this saved file if they do, which saves the need to make live API calls on every test run. If you receive errors about a cassette expiring, delete and re-record the cassette to ensure the data is up-to-date.
 
 **Sensitive Data:** We've made every attempt to include scrubbers for sensitive data when recording cassettes so that PII or sensitive info does not persist in version control; however, please ensure when recording or re-recording cassettes that prior to committing your changes, no PII or sensitive information gets persisted by inspecting the cassette.
```

### Comparing `easypost-8.0.0/UPGRADE_GUIDE.md` & `easypost-8.1.0/UPGRADE_GUIDE.md`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/constant.py` & `easypost-8.1.0/easypost/constant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # flake8: noqa
 # Library version
-VERSION = "8.0.0"
+VERSION = "8.1.0"
 VERSION_INFO = [str(number) for number in VERSION.split(".")]
 
 # Client defaults
 API_BASE = "https://api.easypost.com"
 API_VERSION = "v2"
 AUTHOR = "EasyPost <oss@easypost.com>"
 SUPPORT_EMAIL = "support@easypost.com"
```

### Comparing `easypost-8.0.0/easypost/easypost_object.py` & `easypost-8.1.0/easypost/easypost_object.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/errors/api/__init__.py` & `easypost-8.1.0/easypost/errors/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # flake8: noqa
 from easypost.errors.api.api_error import ApiError
+from easypost.errors.api.bad_request_error import BadRequestError
 from easypost.errors.api.encoding_error import EncodingError
 from easypost.errors.api.external_api_error import ExternalApiError
 from easypost.errors.api.forbidden_error import ForbiddenError
 from easypost.errors.api.gateway_timeout_error import GatewayTimeoutError
 from easypost.errors.api.http_error import HttpError
 from easypost.errors.api.internal_server_error import InternalServerError
 from easypost.errors.api.invalid_request_error import InvalidRequestError
```

### Comparing `easypost-8.0.0/easypost/errors/api/api_error.py` & `easypost-8.1.0/easypost/errors/api/api_error.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/errors/general/__init__.py` & `easypost-8.1.0/easypost/errors/general/__init__.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/models/__init__.py` & `easypost-8.1.0/easypost/models/__init__.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/requestor.py` & `easypost-8.1.0/easypost/requestor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import datetime
 import json
 import platform
 import time
+import uuid
 from enum import Enum
 from json import JSONDecodeError
 from typing import (
     Any,
     Dict,
     List,
     Optional,
     Tuple,
     Union,
 )
 from urllib.parse import urlencode
 
 import requests
-
 from easypost.constant import (
     API_VERSION,
     COMMUNICATION_ERROR,
     INVALID_REQUEST_LIB_ERROR,
     INVALID_REQUEST_METHOD_ERROR,
     INVALID_REQUEST_PARAMETERS_ERROR,
     INVALID_RESPONSE_BODY_ERROR,
     SUPPORT_EMAIL,
     TIMEOUT_ERROR,
     VERSION,
 )
 from easypost.easypost_object import EasyPostObject
 from easypost.errors import (
+    BadRequestError,
     EasyPostError,
     ForbiddenError,
     GatewayTimeoutError,
     HttpError,
     InternalServerError,
     InvalidRequestError,
     JsonError,
@@ -45,14 +46,15 @@
     TimeoutError,
     UnauthorizedError,
     UnknownApiError,
 )
 
 
 STATUS_CODE_TO_ERROR_MAPPING: Dict[int, Any] = {
+    400: BadRequestError,
     401: UnauthorizedError,
     402: PaymentError,
     403: ForbiddenError,
     404: NotFoundError,
     405: MethodNotAllowedError,
     408: TimeoutError,
     422: InvalidRequestError,
@@ -197,25 +199,48 @@
         )
 
         headers = {
             "Authorization": "Bearer %s" % self._client.api_key,
             "User-Agent": user_agent,
         }
 
+        request_uuid = uuid.uuid4()
+        request_timestamp = datetime.datetime.now(datetime.timezone.utc)
+        self._client._request_hook(
+            method=method,
+            path=abs_url,
+            headers=headers,
+            request_body=params,
+            request_timestamp=request_timestamp,
+            request_uuid=request_uuid,
+        )
+
         if self._client._request_lib == "urlfetch":
-            http_body, http_status = self.urlfetch_request(
+            http_body, http_status, http_headers = self.urlfetch_request(
                 method=method, abs_url=abs_url, headers=headers, params=params
             )
         elif self._client._request_lib == "requests":
-            http_body, http_status = self.requests_request(
+            http_body, http_status, http_headers = self.requests_request(
                 method=method, abs_url=abs_url, headers=headers, params=params
             )
         else:
             raise EasyPostError(INVALID_REQUEST_LIB_ERROR.format(self._client._request_lib, SUPPORT_EMAIL))
 
+        response_timestamp = datetime.datetime.now(datetime.timezone.utc)
+        self._client._response_hook(
+            http_status=http_status,
+            method=method,
+            path=abs_url,
+            headers=http_headers,
+            response_body=http_body,
+            request_timestamp=request_timestamp,
+            response_timestamp=response_timestamp,
+            request_uuid=request_uuid,
+        )
+
         return http_body, http_status
 
     def interpret_response(self, http_body: str, http_status: int) -> Dict[str, Any]:
         """Interpret the response body we receive from the API."""
         if http_status == 204:
             # HTTP 204 does not have any response body and we can just return here
             return {}
@@ -232,15 +257,15 @@
 
     def requests_request(
         self,
         method: RequestMethod,
         abs_url: str,
         headers: Dict[str, Any],
         params: Dict[str, Any],
-    ) -> Tuple[str, int]:
+    ) -> Tuple[str, int, Dict[str, Any]]:
         """Make a request by using the `request` library."""
         if method in [RequestMethod.GET, RequestMethod.DELETE]:
             url_params = params
             body = None
         elif method in [RequestMethod.POST, RequestMethod.PATCH, RequestMethod.PUT]:
             url_params = None
             body = params
@@ -258,28 +283,29 @@
                 headers=headers,
                 json=body,
                 timeout=self._client.timeout,
                 verify=True,
             )
             http_body = result.text
             http_status = result.status_code
+            http_headers = result.headers
         except requests.exceptions.Timeout:
             raise TimeoutError(TIMEOUT_ERROR)
         except Exception as e:
             raise HttpError(COMMUNICATION_ERROR.format(SUPPORT_EMAIL, e))
 
-        return http_body, http_status
+        return http_body, http_status, http_headers
 
     def urlfetch_request(
         self,
         method: RequestMethod,
         abs_url: str,
         headers: Dict[str, Any],
         params: Dict[str, Any],
-    ) -> Tuple[str, int]:
+    ) -> Tuple[str, int, Dict[str, Any]]:
         """Make a request by using the `urlfetch` library."""
         fetch_args = {
             "method": method.value,
             "headers": headers,
             "validate_certificate": False,
             "deadline": self._client.timeout,
         }
@@ -297,15 +323,15 @@
         try:
             from google.appengine.api import urlfetch  # type: ignore
 
             result = urlfetch.fetch(**fetch_args)  # type: ignore
         except Exception as e:
             raise HttpError(COMMUNICATION_ERROR.format(SUPPORT_EMAIL, e))
 
-        return result.content, result.status_code
+        return result.content, result.status_code, result.headers
 
     def handle_api_error(self, http_status: int, http_body: str, response: Dict[str, Any]) -> None:
         """Handles API errors returned from the EasyPost API."""
         try:
             error = response["error"]
         except (KeyError, TypeError):
             raise JsonError(
@@ -315,15 +341,19 @@
             )
 
         if http_status >= 300 and http_status < 400:
             raise RedirectError(message=error, http_status=http_status, http_body=http_body)
 
         error_type = STATUS_CODE_TO_ERROR_MAPPING.get(http_status, UnknownApiError)
 
-        raise error_type(message=error.get("message", ""), http_status=http_status, http_body=http_body)
+        raise error_type(
+            message=error.get("message", ""),
+            http_status=http_status,
+            http_body=http_body,
+        )
 
     def _utf8(self, value: Union[str, bytes]) -> str:
         # Python3's str(bytestring) returns "b'bytestring'" so we use .decode instead
         if isinstance(value, bytes):
             return value.decode(encoding="utf-8")
         return value
```

### Comparing `easypost-8.0.0/easypost/services/__init__.py` & `easypost-8.1.0/easypost/services/__init__.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/address_service.py` & `easypost-8.1.0/easypost/services/address_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/base_service.py` & `easypost-8.1.0/easypost/services/base_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/batch_service.py` & `easypost-8.1.0/easypost/services/batch_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/beta_carrier_metadata_service.py` & `easypost-8.1.0/easypost/services/beta_carrier_metadata_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/beta_rate_service.py` & `easypost-8.1.0/easypost/services/beta_rate_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/beta_referral_customer_service.py` & `easypost-8.1.0/easypost/services/beta_referral_customer_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/billing_service.py` & `easypost-8.1.0/easypost/services/billing_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/carrier_account_service.py` & `easypost-8.1.0/easypost/services/carrier_account_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/carrier_metadata_service.py` & `easypost-8.1.0/easypost/services/carrier_metadata_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/customs_info_service.py` & `easypost-8.1.0/easypost/services/customs_info_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/customs_item_service.py` & `easypost-8.1.0/easypost/services/customs_item_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/end_shipper_service.py` & `easypost-8.1.0/easypost/services/end_shipper_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/event_service.py` & `easypost-8.1.0/easypost/services/event_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/insurance_service.py` & `easypost-8.1.0/easypost/services/insurance_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/order_service.py` & `easypost-8.1.0/easypost/services/order_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/pickup_service.py` & `easypost-8.1.0/easypost/services/pickup_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/referral_customer_service.py` & `easypost-8.1.0/easypost/services/referral_customer_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import (
     Any,
     Dict,
     Optional,
 )
 
 import requests
-
 from easypost.constant import (
     SEND_STRIPE_DETAILS_ERROR,
     TIMEOUT,
 )
 from easypost.easypost_object import convert_to_easypost_object
 from easypost.errors import ExternalApiError
 from easypost.models import User
```

### Comparing `easypost-8.0.0/easypost/services/refund_service.py` & `easypost-8.1.0/easypost/services/refund_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/report_service.py` & `easypost-8.1.0/easypost/services/report_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/scan_form_service.py` & `easypost-8.1.0/easypost/services/scan_form_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/shipment_service.py` & `easypost-8.1.0/easypost/services/shipment_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/tracker_service.py` & `easypost-8.1.0/easypost/services/tracker_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/user_service.py` & `easypost-8.1.0/easypost/services/user_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/services/webhook_service.py` & `easypost-8.1.0/easypost/services/webhook_service.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost/util.py` & `easypost-8.1.0/easypost/util.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/easypost.egg-info/PKG-INFO` & `easypost-8.1.0/easypost.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypost
-Version: 8.0.0
+Version: 8.1.0
 Summary: EasyPost Shipping API Client Library for Python
 Home-page: https://easypost.com/
 Author: EasyPost
 Author-email: support@easypost.com
 Project-URL: Docs, https://www.easypost.com/docs/api
 Project-URL: Tracker, https://github.com/EasyPost/easypost-python/issues
 Project-URL: Source, https://github.com/EasyPost/easypost-python
@@ -85,14 +85,32 @@
 )
 
 bought_shipment = client.shipment.buy(shipment.id, rate=shipment.lowest_rate())
 
 print(bought_shipment)
 ```
 
+### HTTP Hooks
+
+Users can subscribe to HTTP requests and responses via the `RequestHook` and `ResponseHook` objects. To do so, pass a function to the `subscribe_to_request_hook` or `subscribe_to_response_hook` methods of an `EasyPostClient` object:
+
+```python
+def custom_function(**kwargs):
+    """Pass your code here, data about the request/response is contained within `kwargs`."""
+    print(f"Received a request with the status code of: {kwargs.get('http_status')}")
+
+client = easypost.EasyPostClient(os.getenv('EASYPOST_API_KEY'))
+
+client.subscribe_to_response_hook(custom_function)
+
+# Make your API calls here, your custom_function will trigger once a response is received
+```
+
+You can also unsubscribe your functions in a similar manner by using the `unsubscribe_from_request_hook` and `unsubscribe_from_response_hook` methods of a client object.
+
 ## Documentation
 
 API documentation can be found at: <https://easypost.com/docs/api>.
 
 Library documentation can be found on the web at: <https://easypost.github.io/easypost-python/> or by building them locally via the `make docs` command.
 
 Upgrading major versions of this project? Refer to the [Upgrade Guide](UPGRADE_GUIDE.md).
@@ -107,33 +125,28 @@
 
 ```bash
 # Install dependencies
 make install
 
 # Lint project
 make lint
-
-# Format project
-make format
+make lint-fix
 
 # Run tests
 EASYPOST_TEST_API_KEY=123... EASYPOST_PROD_API_KEY=123... make test
-
-# Run test coverage
 EASYPOST_TEST_API_KEY=123... EASYPOST_PROD_API_KEY=123... make coverage
 
 # Run security analysis
 make scan
 
 # Generate library documentation
 make docs
 
 # Update submodules
-git submodule init
-git submodule update --remote
+make update-examples-submodule
 ```
 
 ### Testing
 
 The test suite in this project was specifically built to produce consistent results on every run, regardless of when they run or who is running them. This project uses [VCR](https://github.com/kevin1024/vcrpy) to record and replay HTTP requests and responses via "cassettes". When the suite is run, the HTTP requests and responses for each test function will be saved to a cassette if they do not exist already and replayed from this saved file if they do, which saves the need to make live API calls on every test run. If you receive errors about a cassette expiring, delete and re-record the cassette to ensure the data is up-to-date.
 
 **Sensitive Data:** We've made every attempt to include scrubbers for sensitive data when recording cassettes so that PII or sensitive info does not persist in version control; however, please ensure when recording or re-recording cassettes that prior to committing your changes, no PII or sensitive information gets persisted by inspecting the cassette.
```

### Comparing `easypost-8.0.0/easypost.egg-info/SOURCES.txt` & `easypost-8.1.0/easypost.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 UPGRADE_GUIDE.md
-pyproject.toml
 setup.py
 easypost/__init__.py
 easypost/constant.py
 easypost/easypost_client.py
 easypost/easypost_object.py
 easypost/py.typed
 easypost/requestor.py
@@ -16,14 +15,15 @@
 easypost.egg-info/SOURCES.txt
 easypost.egg-info/dependency_links.txt
 easypost.egg-info/requires.txt
 easypost.egg-info/top_level.txt
 easypost/errors/__init__.py
 easypost/errors/api/__init__.py
 easypost/errors/api/api_error.py
+easypost/errors/api/bad_request_error.py
 easypost/errors/api/encoding_error.py
 easypost/errors/api/external_api_error.py
 easypost/errors/api/forbidden_error.py
 easypost/errors/api/gateway_timeout_error.py
 easypost/errors/api/http_error.py
 easypost/errors/api/internal_server_error.py
 easypost/errors/api/invalid_request_error.py
@@ -41,14 +41,18 @@
 easypost/errors/general/easypost_error.py
 easypost/errors/general/end_of_pagination_error.py
 easypost/errors/general/filtering_error.py
 easypost/errors/general/invalid_object_error.py
 easypost/errors/general/invalid_parameter_error.py
 easypost/errors/general/missing_parameter_error.py
 easypost/errors/general/signature_verification_error.py
+easypost/hooks/__init__.py
+easypost/hooks/event_hook.py
+easypost/hooks/request_hook.py
+easypost/hooks/response_hook.py
 easypost/models/__init__.py
 easypost/models/address.py
 easypost/models/api_key.py
 easypost/models/batch.py
 easypost/models/billing.py
 easypost/models/brand.py
 easypost/models/carrier_account.py
@@ -108,14 +112,15 @@
 tests/test_carrier_metadata.py
 tests/test_customs_info.py
 tests/test_customs_item.py
 tests/test_easypost_client.py
 tests/test_end_shipper.py
 tests/test_error.py
 tests/test_event.py
+tests/test_hook.py
 tests/test_insurance.py
 tests/test_order.py
 tests/test_parcel.py
 tests/test_pickup.py
 tests/test_rate.py
 tests/test_referral_customer.py
 tests/test_refund.py
```

### Comparing `easypost-8.0.0/setup.py` & `easypost-8.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ]
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="easypost",
-    version="8.0.0",
+    version="8.1.0",
     description="EasyPost Shipping API Client Library for Python",
     author="EasyPost",
     author_email="support@easypost.com",
     url="https://easypost.com/",
     packages=find_packages(
         exclude=[
             "docs",
```

### Comparing `easypost-8.0.0/tests/test_address.py` & `easypost-8.1.0/tests/test_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.constant import (
     _TEST_FAILED_INTENTIONALLY_ERROR,
     NO_MORE_PAGES_ERROR,
 )
 from easypost.errors import ApiError
 from easypost.models import Address
```

### Comparing `easypost-8.0.0/tests/test_batch.py` & `easypost-8.1.0/tests/test_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import inspect
 import os
 import time
 
 import pytest
-
 from easypost.models import Batch
 
 
 @pytest.mark.vcr()
 def test_batch_create(one_call_buy_shipment, test_client):
     batch = test_client.batch.create(shipments=[one_call_buy_shipment])
```

### Comparing `easypost-8.0.0/tests/test_beta_carrier_metadata.py` & `easypost-8.1.0/tests/test_beta_carrier_metadata.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/tests/test_beta_rate.py` & `easypost-8.1.0/tests/test_beta_rate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.util import get_lowest_stateless_rate
 
 
 @pytest.mark.vcr()
 def test_beta_retrieve_stateless_rates(basic_shipment, test_client):
     """Tests that we can retrieve stateless rates when basic shipment data."""
     stateless_rates = test_client.beta_rate.retrieve_stateless_rates(**basic_shipment)
```

### Comparing `easypost-8.0.0/tests/test_beta_referral_customer.py` & `easypost-8.1.0/tests/test_beta_referral_customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.errors.api.api_error import ApiError
 
 
 @pytest.mark.vcr()
 def test_beta_referral_customer_add_payment_method(referral_customer_prod_client):
     """This test requires a referral customer's production API key via REFERRAL_CUSTOMER_PROD_API_KEY.
```

### Comparing `easypost-8.0.0/tests/test_billing.py` & `easypost-8.1.0/tests/test_billing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from unittest.mock import patch
 
-import pytest
-
 import easypost
+import pytest
 from easypost.errors import InvalidObjectError
 
 
 @patch(
     "easypost.services.billing_service.BillingService._get_payment_method_info", return_value=["/endpoint", "card_123"]
 )
 @patch("easypost.services.billing_service.Requestor.request", return_value={"mock": "response"})
```

### Comparing `easypost-8.0.0/tests/test_carrier_account.py` & `easypost-8.1.0/tests/test_carrier_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.errors.api.api_error import ApiError
 from easypost.models import CarrierAccount
 
 
 @pytest.mark.vcr()
 def test_carrier_account_create(prod_client, basic_carrier_account):
     carrier_account = prod_client.carrier_account.create(**basic_carrier_account)
```

### Comparing `easypost-8.0.0/tests/test_carrier_metadata.py` & `easypost-8.1.0/tests/test_carrier_metadata.py`

 * *Files identical despite different names*

### Comparing `easypost-8.0.0/tests/test_customs_info.py` & `easypost-8.1.0/tests/test_customs_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.models import CustomsInfo
 
 
 @pytest.mark.vcr()
 def test_customs_info_create(basic_customs_info, test_client):
     customs_info = test_client.customs_info.create(**basic_customs_info)
```

### Comparing `easypost-8.0.0/tests/test_customs_item.py` & `easypost-8.1.0/tests/test_customs_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.models import CustomsItem
 
 
 @pytest.mark.vcr()
 def test_customs_item_create(basic_customs_item, test_client):
     customs_item = test_client.customs_item.create(**basic_customs_item)
```

### Comparing `easypost-8.0.0/tests/test_easypost_client.py` & `easypost-8.1.0/tests/test_easypost_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 from unittest.mock import patch
 
 import pytest
 import requests
-
 from easypost.easypost_client import EasyPostClient
 from easypost.errors import TimeoutError
 
 
 def test_api_key():
     """Tests setting and getting API keys from different client objects."""
     client1 = EasyPostClient(api_key="123")
```

### Comparing `easypost-8.0.0/tests/test_end_shipper.py` & `easypost-8.1.0/tests/test_end_shipper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.models import EndShipper
 
 
 @pytest.mark.vcr()
 def test_endshipper_create(ca_address_1, test_client):
     endshipper = test_client.end_shipper.create(**ca_address_1)
```

### Comparing `easypost-8.0.0/tests/test_error.py` & `easypost-8.1.0/tests/test_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.errors.api.api_error import ApiError
 
 
 @pytest.mark.vcr()
 def test_error(test_client):
     """Tests that we assign properties of an error correctly."""
     try:
```

### Comparing `easypost-8.0.0/tests/test_event.py` & `easypost-8.1.0/tests/test_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import inspect
 import os
 import time
 
 import pytest
-
 from easypost.constant import (
     _TEST_FAILED_INTENTIONALLY_ERROR,
     NO_MORE_PAGES_ERROR,
 )
 from easypost.errors import ApiError
 from easypost.models import (
     Event,
```

### Comparing `easypost-8.0.0/tests/test_insurance.py` & `easypost-8.1.0/tests/test_insurance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.constant import (
     _TEST_FAILED_INTENTIONALLY_ERROR,
     NO_MORE_PAGES_ERROR,
 )
 from easypost.models import Insurance
```

### Comparing `easypost-8.0.0/tests/test_order.py` & `easypost-8.1.0/tests/test_order.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.errors import FilteringError
 from easypost.models import (
     Order,
     Rate,
 )
```

### Comparing `easypost-8.0.0/tests/test_parcel.py` & `easypost-8.1.0/tests/test_parcel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.models import Parcel
 
 
 @pytest.mark.vcr()
 def test_parcel_create(basic_parcel, test_client):
     parcel = test_client.parcel.create(**basic_parcel)
```

### Comparing `easypost-8.0.0/tests/test_pickup.py` & `easypost-8.1.0/tests/test_pickup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.constant import (
     _TEST_FAILED_INTENTIONALLY_ERROR,
     NO_MORE_PAGES_ERROR,
 )
 from easypost.errors import FilteringError
 from easypost.models import Pickup
```

### Comparing `easypost-8.0.0/tests/test_referral_customer.py` & `easypost-8.1.0/tests/test_referral_customer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 from unittest.mock import patch
 
 import pytest
-
 from easypost.constant import (
     _TEST_FAILED_INTENTIONALLY_ERROR,
     NO_MORE_PAGES_ERROR,
 )
 from easypost.models import User
```

### Comparing `easypost-8.0.0/tests/test_refund.py` & `easypost-8.1.0/tests/test_refund.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.constant import (
     _TEST_FAILED_INTENTIONALLY_ERROR,
     NO_MORE_PAGES_ERROR,
 )
 from easypost.models import Refund
```

### Comparing `easypost-8.0.0/tests/test_report.py` & `easypost-8.1.0/tests/test_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.constant import (
     _TEST_FAILED_INTENTIONALLY_ERROR,
     NO_MORE_PAGES_ERROR,
 )
 from easypost.models import Report
```

### Comparing `easypost-8.0.0/tests/test_scan_form.py` & `easypost-8.1.0/tests/test_scan_form.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.constant import (
     _TEST_FAILED_INTENTIONALLY_ERROR,
     NO_MORE_PAGES_ERROR,
 )
 from easypost.models import ScanForm
```

### Comparing `easypost-8.0.0/tests/test_shipment.py` & `easypost-8.1.0/tests/test_shipment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.constant import (
     _TEST_FAILED_INTENTIONALLY_ERROR,
     NO_MORE_PAGES_ERROR,
 )
 from easypost.errors import (
     FilteringError,
     InvalidParameterError,
```

### Comparing `easypost-8.0.0/tests/test_tracker.py` & `easypost-8.1.0/tests/test_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.constant import (
     _TEST_FAILED_INTENTIONALLY_ERROR,
     NO_MORE_PAGES_ERROR,
 )
 from easypost.models import Tracker
```

### Comparing `easypost-8.0.0/tests/test_user.py` & `easypost-8.1.0/tests/test_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.models import (
     ApiKey,
     Brand,
     User,
 )
```

### Comparing `easypost-8.0.0/tests/test_webhook.py` & `easypost-8.1.0/tests/test_webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from easypost.errors import SignatureVerificationError
 from easypost.models import Webhook
 from easypost.util import validate_webhook
 
 
 @pytest.mark.vcr()
 def test_webhook_create(webhook_url, test_client):
```

